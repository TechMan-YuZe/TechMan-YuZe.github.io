#
## (1) MySQL安装
> 安装教程请自己进行百度
## (2) MySQL 分层、存储引擎
> ### mysql 分层
* 连接层
    * 提供与客户端连接的服务
* 服务层
    * 提供各种用户使用的接口
    * 提供 SQL 优化器（MySQL QUery Optimizer）
* 引擎层
    * 提供各种存储数据的方式
    * InnoDB
    * MyISAM
* 存储层
    * 存储数据

>### InnoDB 和 MyISAM 区别
* InnoDB
    * 事务优先
    * 适合高并发操作
    * 行锁
* MyISAM
    * 性能优先
    * 表锁
* 查询数据库支持哪些引擎
    * show engines;
* 查询默认引擎
    * show variables like '%storage_engine%';
* 创建表时指定引擎
```sql
create database myDB;
use myDB;
create table tb(
id int(4) auto_increment,
name varchar(5),
dept varchar(5),
primary key(id)
) ENGINE=MyISAM AUTO_INCREMENT=1 
DEFAULT CHARSET=utf8;
```

## (3) SQL 优化
>### 原因
* 性能低
* 执行时间长
* 等待时间长
* SQL 语句欠佳（连接查询）
* 索引失效
* 服务器参数设置不佳
    * 缓冲
    * 线程数

>### 编写过程和解析过程的差异
* 编写过程
    * select distinct ... from ... join ... on ... where ... group by ... having ... order by ... limit
* 解析过程
    * from ... on ... join ... where ... group by ... having ... select distinct... order by ... limit
* 参考文章
    * https://www.cnblogs.com/annsshadow/p/5037667.html

>### 优化索引
* 索引是帮助 MYSQL 高效获取数据的数据结构
* 索引一般采用树结构
    * B 树
    * Hash 树
* 索引弊端
    * 索引本身需要空间
    * 索引不适用
        * 少量数据
        * 频繁更新的字段
        * 很少使用的字段
    * 提高查询，降低增删改效率
* 优点
    * 降低 IO 使用率
    * 降低 CPU 使用率
        * B 树本身已经排好序，可以直接使用

## (4) B 树与索引
* 三层 B 树可以存放百万级别数据
* B 树一般都是指 B+ 树
    * 数据都保存在叶结点
* B + 树中查找数据的次数
    * n 次
    * 即 B+ 树的高度

>### 索引
>###### 分类
* 单值索引
    * 单列
    * 一个表可以有多个单值索引
* 主键索引
    * 不能重复
    * 如 id
    * 不能为 null
* 唯一索引
    * 不能重复
    * 如 id
    * 可以为 null
* 复合索引
    * 多个列构成的索引
    * 相当于二级目录

>### 创建索引
>###### 方式一
```sql
create 索引类型 索引名 on 表(字段)
```
>单值索引
```
create index dept_index on tb(dept);
```
>唯一索引
```
create unique index name_index on tb(name);
```
>复合索引
```
create index dept_name_index on tb(dept, name);
```
>###### 方式二
```
alter table 表名 索引类型 索引名(字段)
```
>单值
```
alter table tb add index dept_index(dept);
```
>唯一
```
alter table tb add unique index name_index(name);
```
>复合
```
alter table tb add index dept_name_index(dept, name);
```
DDL 语句不需要 commit; 自动提交

如果一个字段是 primary key，该字段默认是主键索引

>### 删除索引
```shell
# drop index 索引名 on 表名;

drop index name_index on tb;
```
>### 查询索引
```shell
# show index from 表名

show index from tb;
```
>### SQL 性能问题
* 分析 sql 执行计划
    * explain
    * 可以模拟 SQL 优化器执行 SQL 语句
* MYSQL 查询优化会干扰我们的优化

## (5) SQL 优化准备
* explain SQL 语句
* id 编号
* select_type 查询类型
* table 表名
* type 类型
* possible_keys 预测用到的索引
* key 实际用到的索引
* key_len 实际使用索引的长度
* ref 表之间的引用
* rows 通过索引查询到的数据量
* Extra 额外信息

>### 准备数据
```shell
create table course
(cid int(3),
cname varchar(20),
tid int(3)
);

create table teacher
(tid int(3),
tname varchar(20),
tcid int(3)
);

create table teacherCard
(
tcid int(3),
tcdesc varchar(200)
);

insert into course values(1,'java', 1);
insert into course values(2,'html', 1);
insert into course values(3,'sql', 2);
insert into course values(4,'web', 3);

insert into teacher values(1, 'tz', 1);
insert into teacher values(2, 'tw', 2);
insert into teacher values(3, 'tl', 3);
insert into teacher values(4, 'ta', 4);
insert into teacher values(5, 'tb', 5);
insert into teacher values(6, 'tc', 6);

insert into teacherCard values(1, 'tzdesc');
insert into teacherCard values(2, 'twdesc');
insert into teacherCard values(3, 'tldesc');

```
## (6) explain 中的 id、table
>### id 值相同

* id 值相同，从上往下，顺序执行
* 表的执行顺序，跟随数据量变化，原理是笛卡尔积
* 数据量小的表优先查询

>##### 查询课程编号为 2 或教师证编号为 3 的老师信息
```shell
explain select t.* from teacher t, course c, teacherCard tc 
where t.tid=c.tid and t.tid=tc.tcid and (c.cid = 2 or tc.tcid=3);
```
>##### 查询教授 SQL 课程的老师描述信息

* 多表连接形式
```shell
explain select tc.tcdesc from teacherCard tc, course c, teacher t 
where c.tid = t.tid and t.tcid = tc.tcid and c.cname='sql';
```
>### id 值不同
* id 值不同，id 值大的优先查询
* 本质：在嵌套子查询时，先查内层，再查外层

>##### 查询教授 SQL 课程的老师描述信息
* 子查询形式
```shell
explain select tc.tcdesc from teacherCard tc where tc.tcid=
(select t.tcid from teacher t where t.tid = 
(select c.tid from course c)
);
```
>### id 值相同 + id 值不同
* id 值大的优先
* id 值相同的从上往下顺序执行

>##### 查询教授 SQL 课程的老师描述信息
* 多表+子查询
```shell
explain select t.tname, tc.tcdesc from teacher t, teacherCard tc 
where t.tcid=tc.tcid and t.tid=(select c.tid from course c where cname='sql');
```
>### select_type
* primary 包含子查询 SQL 中的主查询（最外层）
* SUBQUERY 包含子查询 SQL 中的子查询（非最外层）
* simple 简单查询，不包含子查询和 union
* derived 衍生查询，使用到了临时表
    * from 子查询中只有一张表
        ```shell
        explain select cr.cname from (select * from course where tid in (1, 2)) cr;
        ```
    * from 子查询中，如果有 table1 union table2，table1 就是 derived
     ```shell
        explain select cr.cname from (select * from course where tid=1 union select * from course where tid =2) cr;
     ```
* union result
    * 告知关联关系的表是哪两张

## (7) type 级别详解
>### system

```shell
create table test01
(
tid int(3),
tname varchar(20)
);

alter table test01 add constraint tid_pk primary key(tid);

insert into test01 values(1, 'a');

explain select * from (select * from test01) t where tid=1;
```
* system>const>eq_ref>ref>range>index>all
* system 和 const 只是理想情况，一般优化很难达到
* system 只有一条数据的系统表，或衍生表只有一条数据的主查询

>### const
```shell
explain select tid from test01 where tid=1;
/* 删除 primary 索引 */
alter table test01 drop primary key;
/* 修改索引为一般索引 */
create index test01_index on test01(tid);
```
* const 只能查到一条数据的 SQL
* 只能用于 primary key 或 unique 索引
* 如果是一般索引，不会出现 const

>### eq_ref
```shell
alter table teacherCard add constraint pk_tcid primary key(tcid);
alter table teacher add constraint uk_tcid unique index(tcid);
delete from teacher where tcid>3;
explain select t.tcid from teacher t, teacherCard tc where t.tcid = tc.tcid;
```
* 对于每个索引键的查询，返回匹配有且只有一行数据
* 常见于唯一索引和主键索引
* 上述语句用到的索引是 teacher 表的 tcid 字段
* 如果 teacher 表的数据个数和连接查询的数据个数一致，才有可能满足 eq_ref 级别

>### ref
```
insert into teacher values(4, 'tz', 4);
insert into teacherCard values(4, 'tzc');

alter table teacher add index index_name(tname);

explain select * from teacher where tname='tz';
```

* 非唯一索引
* 对于每个索引键的查询，返回匹配的所有行

>### range
```shell
alter table teacher add index tid_index(tid);

explain select t.* from teacher t where t.tid <3;
```
* 检索指定范围的行，where 后面是一个范围查询
* between, in, <, >, >=, <=
* in 查询，有时会失效，从 range 级别转为 all 无索引级别

>### index，all
```shell
/* tid 有索引，只扫描 tid 列 */
explain select tid from teacher;
/* course 表无索引，扫描全部数据 */
explain select cid from course;
```
* index 查询全部索引数据
* all 查询全部数据

>### 总结
* system/const
    * 结果只有一条
* eq_ref
    * 结果多条
    * 每条数据唯一
* ref
    * 结果多条
    * 每条数据可能是多条

## (8)possible_keys, key
```shell
alter table course add index cname_index(cname);

explain select t.tname, tc.tcdesc from teacher t, teacherCard tc 
where t.tcid=tc.tcid and t.tid=(select c.tid from course c where cname='sql');

explain select tc.tcdesc from teacherCard tc, course c, teacher t 
where c.tid = t.tid and t.tcid = tc.tcid and c.cname='sql';

```
* possible_keys
    * 可能用到的索引
    * 是一种预测
* key
    * 实际使用到的索引
    * null 表示无索引

## (9) 索引类型及逐步优化、key_len 计算方法
```shell
create table test_kl 
(
name char(20) not null default ''
);

alter table test_kl add index index_name(name);

explain select * from test_kl where name='';

alter table test_kl add column name1 char(20);
alter table test_kl add index index_name1(name1);

explain select * from test_kl where name1='';

drop index index_name on test_kl;
drop index index_name1 on test_kl;

alter table test_kl add index name_name1_index (name, name1);

explain select * from test_kl where name1='';

alter table test_kl add column name2 varchar(20);
alter table test_kl add index name2_index(name2);

/* key_len=63 = 60+1(null)+2(varchar) */
explain select * from test_kl where name2='';
```
* 索引的长度
    * 用于判断复合索引是否被完全使用
    * utf8 中，1 个字符占 3 个字节
        * char(20)，key_len = 60
    * utf8mb4 中，1 个字符占 4 个字节
* gbk 中，1 个字符 2 个字节
* latin 中，1 个字符 1 个字节
* 如果索引字段可以为 null，mysql 底层会用 1 个字节用于标识
* 索引字段为 varchar，用 2 个字节代表可变长度

## (10) ref、rows
>##### ref
```shell
alter table course add index tid_index(tid);

explain select * from course c, teacher t where c.tid = t.tid and t.tname='tw';
```
* 与 type 中的 ref 区分
* 指明当前表所参照的字段
* select ... where a.c=b.x
* 其中 b.x 可以是常量，const
>##### rows
```shell
explain select * from course c, teacher t where c.tid = t.tid and t.tname='tz';
```
* 实际通过索引查询到的数据个数

## (11) Extra 字段
>##### Using filesort
```shell
create table test02
(
a1 char(3),
a2 char(3),
a3 char(3),
index idx_a1(a1),
index idx_a2(a2),
index idx_a3(a3)
);

/* 排序和查找不是同一个字段 Using filesort */
explain select * from test02 where a1 = '' order by a2;

drop index idx_a1 on test02;
drop index idx_a2 on test02;
drop index idx_a3 on test02;

alter table test02 add index idx_a1_a2_a3(a1, a2, a3);
/* 复合索引跨列 */
explain select * from test02 where a1='' order by a3;
explain select * from test02 where a2='' order by a3;
explain select * from test02 where a1='' order by a2;
```
* 性能消耗大，需要额外一次排序或查询
* 如果排序和查找不是同一个字段，则会出现 Using filesort
* 如果符合索引跨列，会出现 Using filesort
    * where 和 order by 按照符合索引的顺序使用，不要跨列或无序
* 常见于 order by

>##### Using temporary
```shell
explain select a1 from test02 where a1 in ('1', '2', '3') group by a2;
```
* 用到了临时表
* 常见于 group by
* 避免
    * 查询哪列就使用哪列 group by

>##### Using index
```shell
explain select a1, a2 from test02 where a1='' or a2='';

drop index idx_a1_a2_a3 on test02;
alter table test02 add index id_a1_a2(a1, a2);
explain select a1, a3 from test02 where a1='' or a3='';

/* 对 possible_keys 和 key 的影响 */
explain select a1, a2 from test02 where a1='' or a2='';
explain select a1, a2 from test02;
```
* 使用到的列都在索引中，称为索引覆盖
* 性能提升
* 不读取原文件，只从索引文件中获取数据
* 不需要回表查询
* 索引覆盖对 possible_keys 和 key 的影响
    * 如果没有 where，则索引只出现在 key 中
    * 如果有 where，则索引出现在 key 和 possible_keys 中

>##### Using where
```shell
explain select a1, a3 from test02 where a3='';
```
* 回表查询
>##### impossible where
```shell
explain select * from test02 where a1='x' and a1='y';
```
* where 子句永远为 false

## (12) 优化示例
```shell
create table test03
(
a1 int(4) not null,
a2 int(4) not null,
a3 int(4) not null,
a4 int(4) not null
);

alter table test03 add index idx_a1_a2_a3_4(a1, a2, a3, a4);

/* Using index */
/* 推荐按照复合索引的顺序查询 */
explain select a1, a2, a3, a4 from test03 where a1=1 and a2=2 and a3=3 and a4=4;

/* Using index */
/* 经过 SQL 优化器后，效果与上一个查询语句一致 */
explain select a1, a2, a3, a4 from test03 where a4=1 and a3=2 and a2=3 and a1=4;

/* Using where; Using index */
/* a4 跨列，索引失效，造成回表查询 */
/* where a1=1 and a2=2 ... order by a3 仍然遵循复合索引的顺序，因此有 Using index */
explain select a1, a2, a3, a4 from test03 where a1=1 and a2=2 and a4=4 order by a3;

/* Using where; Using index; Using filesort */
/* where a1=1 ... order by a3 跨列，多了一次查找/排序，出现 Using filesort */
explain select a1, a2, a3, a4 from test03 where a1=1 and a4=4 order by a3;

```
> ### 总结
* 如果复合索引使用顺序完全一致，索引全部使用
* 如果部分一致，索引部分使用
* where 和 order 拼接不要跨列

## (13) 单表优化及总结
```shell
create table book
(
bid int(4) primary key,
name varchar(20) not null,
authorid int(4) not null,
publicid int(4) not null,
typeid int(4) not null
);

insert into book values(1, 'java', 1, 1, 2);
insert into book values(2, 'html', 2, 1, 2);
insert into book values(3, 'sql', 3, 2, 1);
insert into book values(4, 'C', 4, 4, 3);

commit;

/* type:All*/
/* Using where; Using filesort */
explain select bid from book where typeid in(2, 3) and authorid=1 order by typeid desc;

/* type:index */
/* Using where; Using index; Using filesort */
alter table book add index idx_bta(bid, typeid, authorid);

/* 为避免干扰，优化之前删除老的索引 */
drop index idx_bta on book;

/* 根据 sql 实际解析的顺序，调整索引顺序 */
/* type:index */
/* Using where; Using index */
alter table book add index idx_tab(typeid, authorid, bid);


/* 删除索引，创建新索引测试 */
drop index idx_tab on book;

/* 将出现范围查询的字段 typeid 放到后面 */
alter table book add index idx_atb(authorid, typeid, bid);

/* 将范围查询 typeid in (2, 3) 放到 authorid=1 后面 */
/* type:ref */
/* Using where; Using index */
/* key_len: 4 */
explain select bid from book where authorid=1 and typeid in(2, 3) order by typeid desc;

/* Using index */
/* key_len: 8 */
/* typeid in(2, 3) 改为 typeid=3，不使用范围查询，typeid 索引有效 */
/* 通过 key_len 也可以佐证，此处有 2 个索引，typeid 索引有效 */
explain select bid from book where authorid=1 and typeid=3 order by typeid desc;

```
> #### 小结
* 索引不能跨列使用，保持索引定义和使用顺序一致性
* 索引需要逐步优化
* 将含 in 的范围查询放到条件最后，防止整个索引失效
* Using index
    * where authorid=1 ... authorid 在索引中，不需要回原表
* Using where
    * ... and typeid in (2,3) typeid 在索引中，但是使用了 in 范围查询，索引失效，需要回原表

## (14~15) 多表优化及总结，避免索引失效原则

>### 二张表
```shell
create table teacher2
(
tid int(4) primary key,
cid int(4) not null
);

insert into teacher2 values(1, 2);
insert into teacher2 values(2, 1);
insert into teacher2 values(3, 3);

create table course2
(
cid int(4),
cname varchar(20)
);

insert into course2 values(1, 'java');
insert into course2 values(2, 'python');
insert into course2 values(3, 'kotlin');
commit;

/* 左连接，将数据量少的表放到左边 */
/* type:All */
/* Extra:  */
/* type:All */
/* Extra: Using where; Using join buffer  */
select * from teacher2 t left outer join course2 c 
on t.cid=c.cid where c.cname='java';

/* 增加索引 */
/* type: index */
/* Extra: Using index */
/* type: All */
/* Extra: Using where; Using join buffer*/
alter table teacher2 add index index_teacher2_cid(cid);

/* type: ref */
/* Extra: Using where */
/* type: ref */
/* Extra: Using index*/
alter table course2 add index index_course2_cname(cname);
```
* 索引添加原则
    * 小表驱动大表
    * 索引建立在经常使用的字段上
    * 三表或更多表使用相同的原则
* 左外连接，给左表加索引
* 右外连接，给右表加索引
* Using join buffer
    * mysql 引擎使用了连接缓存

>### 避免索引失效的原则
```shell
/* 2 个索引都有效 */
/* type:ref */
/* Extra: */
/* key_len: 8 */
explain select * from book where authorid=1 and typeid=2;

/* 只有 1 个索引有效 */
/* type:ref */
/* Extra: using where */
/* key_len: 4 */
explain select * from book where authorid=1 and typeid*2=2;


/* 2 个索引都失效 */
/* type:All */
/* Extra: using where */
/* key_len: NULL */
explain select * from book where authorid*2=1 and typeid*2=2;

/* 2 个索引都失效，复合索引左边失效，整个索引失效 */
/* type:All */
/* Extra: using where */
/* key_len: NULL */
explain select * from book where authorid*2=1 and typeid=2;

/* 删除复合索引 */
drop index idx_atb on book;

alter table book add index idx_authorid(authorid);
alter table book add index idx_typeid(typeid);

/* 1 个索引都失效，独立索引，第 1 个索引失效，不影响后面的索引 */
/* type:ref */
/* Extra: using where */
/* key_len: 4 */
explain select * from book where authorid*2 = 1 and typeid=2;

/* 索引有效 */
explain select * from book where authorid =1 and typeid =2;
/* 使用了不等于，索引失效 */
explain select * from book where authorid !=1 and typeid =2;
```
* 复合索引，不要跨列或无序使用
* 尽量使用全索引匹配
* 不要在索引上进行任何操作
    * 计算
    * 函数
    * 类型转换
    * 如 ... where a.x*3
* 复合索引，左边索引失效，所有索引失效
* 复合索引使用不等于或者 is null，自身索引会失效，右侧索引可能会失效
* MySQL 本身有 sql 优化器，实际优化效果并非百分之百达到预期

>### 索引优化与预期不符合的情况
```shell
drop index idx_typeid on book;
drop index idx_authorid on book;

alter table book add index idx_book_at(authorid, typeid);

/* 复合索引全部使用 */
/* key_len:8 */
/* type: ref */
explain select * from book where authorid =1 and typeid =2;

/* where 中最左侧的索引字段有 > 号，复合索引中自身及右侧全部失效 */
/* type:All */
/* Extra: Using where */
/* key_len: NULL */
explain select * from book where authorid >1 and typeid =2;

/* 最右侧索引使用了 > 号，复合索引没有失效 */
/* type: range */
/* Extra: Using where */
/* key_len: 8 */
explain select * from book where authorid =1 and typeid>2;

/* 复合索引只有 1 个生效 */
/* type: range */
/* key_len: 4 */
/* Extra: Using where */
explain select * from book where authorid <1 and typeid=2;

/* 相比上一条 SQL，只将 authorid<1 改为 authorid<4，右侧索引也失效 */
/* type: ALL */
/* key_len: NULL */
/* Extra: Using where */
explain select * from book where authorid <4 and typeid=2;

/* 使用百分号开头，索引失效 */
/* type: ALL */
/* key_len: NULL */
/* Extra: Using where */
explain select * from teacher where tname like '%x%';

/* 不使用百分号开头，索引仍然有效 */
/* type: range */
/* key_len: NULL */
/* Extra: Using where */
explain select * from teacher where tname like 'x%';

/* 使用百分号开头，但是实现索引覆盖，仍然起到了一定的优化作用 */
/* type: index */
/* key_len: 63 */
/* Extra: Using where; Using index */
explain select tname from teacher where tname like '%x%';

/* tname 和 'abc' 都是字符形式，索引有效 */
/* type: ref */
/* key_len: 63 */
/* Extra: Using where */
explain select * from teacher where tname = 'abc';

/* tname 是字符类型，123 是整数，查找时有类型转换操作，导致索引失效 */
/* type: ALL */
/* key_len: NULL */
/* Extra: Using where */
explain select * from teacher where tname = 123;

/* 使用 and，索引仍然有效 */
/* type: ref */
/* key_len: 63 */
/* Extra: Using where */
explain select * from teacher where tname = '' and tcid>1;

/* 使用了 or，导致 or 左侧的索引也失效 */
/* type: ALL */
/* key_len: NULL */
/* Extra: Using where */
explain select * from teacher where tname = '' or tcid>1;
```
* 一般情况，范围查询之后的索引失效
* 使用索引覆盖，索引优化会完全符合预期
* like 尽量以常量开头，不以 '%' 开头，否则索引失效
* 使用类型转换（显式或隐式），会导致索引失效
* 使用 or 会导致索引失效，甚至会影响左侧的索引

## (16) 常见优化方法及慢查询 SQL 排查
>### exist 和 in
```shell
/* 有数据 */
select tname from teacher where exists(select * from teacher);

/* 无数据 */
select tname from teacher where exists(select * from teacher where tid=9999);
```
* 如果主查询数据集大，使用 in
* 如果子查询数据集大，使用 exist
* 将主查询的结构放到子查询结果中进行条件校验
    * 如果子查询有数据，则校验成功
    * 如果符合校验，则保留数据

>### order by 优化
* Using filesort
    * 双路排序 MySQL 4.1 之前
        * 扫描 2 次磁盘
        * 第 1 次
            * 从磁盘读取排序字段
            * 对排序字段进行排序
            * 在 buffer 中进行排序
        * 第 2 次：扫描其他字段
    * 单路排序
        * 一次性读取全部磁盘
        * 在 buffer 中进行排序
        * 不一定是真正的单路，仍然可能是多次 IO
            * 数据量过大时，分片读取
* 单路排序比双路排序占用更多 buffer
* 调整 buffer
    * set max_length_for_sort_data=1024
* 单路自动切换到双路的条件
    * 需要排序的列总大小超过 set max_length_for_sort_data=1024 定义的字节数
* 提供 order by 效率的策略
    * 选择使用单路，双路
    * 调整 buffer 容量大小
    * 避免使用 select *
    * 复合索引避免跨列
    * 保证全部排序字段顺序的一致性

>### 慢查询日志
* MySQL 用于记录响应时间超过阈值的 SQL 语句
* long_query_time 阈值默认 10 秒
* 慢查询日志默认关闭
* 建议在调优时打开，部署上线时关闭
* 检查是否开启了慢查询日志
    * show variables like '%slow_query_log%';
* 开启慢查询日志
    * 临时开启
        * set global slow_query_log =1;
        * mysql 服务重启后失效
    * 永久开启
        * vi /etc/my.cnf
          ```shell
          [mysqld] 
          slow_query_log=1 
          slow_query_log_file=/var/lib/mysql/localhost-slow.log
          ```

* 慢查询阈值修改
    * show variables like '%long_query_time%';
    * 临时修改
        ```shell
        # 重新登录后生效
        set global long_query_time=5;
        ```
    * 永久修改
        * vi /etc/my.cnf
        ```shell
        [mysqld] 
        long_query_time=3
        ```

## (17) 慢查询阈值和 mysqldumpslow 工具
* 休眠模拟慢查询
```shell
select sleep(4);
```
* 查询超过阈值的 SQL 数量
```shell
show global status like '%slow_queries%';
```
* 在 linux 命令行，通过日志查看慢查询 SQL 的详情
```shell
cat /var/lib/mysql/localhost-slow.log
```

>### 通过 mysqldumpslow 工具查看慢 SQL
```shell
/* 模拟慢查询 */
select sleep(5);
select sleep(4);
select sleep(3);

/* 获取返回记录最多的 3 个 SQL */
mysqldumpslow -s r -t 3 /var/lib/mysql/bigdata01-slow.log

/* 获取访问次数最多的 3 个 SQL */
mysqldumpslow -s c -t 3 /var/lib/mysql/bigdata01-slow.log

/* 按照时间排序，前 10 条包含 left join 查询语句的 SQL */
mysqldumpslow -s t -t 10 -g "left join" /var/lib/mysql/bigdata01-slow.log

```

* mysqldumpslow
* 常用参数
    * s 排序方式
    * r 逆序
    * l 锁定时间
    * g 正则匹配模式
* 标准语法
    * mysqldumpslow 各种参数 慢查询日志文件路径

## (18) 模拟并通过 profiles 分析海量数据
>#### 模拟海量数据，存储过程/存储函数
```shell
create database testdata;
use testdata;

create table dept 
(
dno int(5) primary key default 0,
dname varchar(20) not null default '',
loc varchar(30) default ''
) engine=innodb default charset=utf8;

create table emp
(
eid int(5) primary key,
ename varchar(20) not null default '',
job varchar(20) not null default '',
deptno int(5) not null default 0
)engine=innodb default charset=utf8;
```
>### 创建存储函数
```shell
use testdata;
delimiter $
create function randstring(n int) returns varchar(255)
begin 

    declare all_str varchar(100) default 'abcdefghijklmnopqrestuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ';
    declare return_str varchar(255) default '';
    declare i int default 0;
    while i<n
    do
        set return_str=concat(return_str, substring(all_str, FLOOR(1+rand()*52), 1));
        set i=i+1;
    end while;
    return return_str;
end $
```
>### 冲突与解决
```shell
/* 开启慢查询日志，再创建存储过程/存储函数，报如下错误   */
/* ERROR 1418 (HY000): 
This function has none of DETERMINISTIC, NO SQL, or READS SQL DATA 
in its declaration and binary logging is enabled 
(you *might* want to use the less safe log_bin_trust_function_creators variable) */

/* 临时解决 */
set global log_bin_trust_function_creators=1;
```
* 永久解决
vi /etc/my.cnf
```shell
[mysqld] 
log_bin_trust_function_creators=1
```

>### 通过存储函数插入随机整数
```shell
use testdata;
create function ran_num() returns int(5)
begin 

declare i int default 0;
set i=floor(rand()*100);
return i;

end$
```

>### 通过存储过程插入海量数据
emp 表
```shell
create procedure insert_emp(in eid_start int(10), in data_times int(10))
begin 
declare i int default 0;
set autocommit =0;

repeat 
insert into emp values(eid_start+i, randstring(5), 'other', ran_num());
set i=i+1;
until i=data_times
end repeat;

commit;

end $
```

dept 表

```shell
create procedure insert_dept(in dno_start int(10), in data_times int(10))
begin 
declare i int default 0;
set autocommit =0;

repeat 
insert into dept values(dno_start+i, randstring(6), randstring(8));
set i=i+1;
until i=data_times
end repeat;

commit;

end $
```

>### 插入数据
```shell
delimiter ;

call insert_emp(1000, 800000);
call insert_dept(10, 30);

/* 验证插入数据量 */
select count(1) from emp;
```

>### 分析海量数据
```shell
show variables like '%profiling%';
/* profiling 影响性能，在部署实施前，应关闭此项 */
set profiling=on;

/* 记录 profiling 打开之后的所有 SQL 语句消耗的时间 */
show profiles;

/* 精确查询更多详情，Query_Id 参考上个语句的查询结果 */
show profile all for query 2;
show profile cpu, block io for query 2;
```
## (19) 全局查询日志
```shell
show variables like '%general_log%';

/* 开启全局日志，记录开启之后的所有 SQL 语句 */
set global general_log=1;
/* 将日志记入表中 */
set global log_output='table';

/* 设置后执行一条查询 */
select count(1) from dept;

/* 显示日志信息 */
select * from mysql.general_log;

/* 将日志记入文件 */
set global log_output='file';

/* 通过默认保存地址查看日志文件 */
cat /var/lib/mysql/bigdata01.log;
```

* 开启 general_log 后，所有 SQL 会被记录到系统自带的 mysql.general_log 表中

## (20) 锁机制详解

* 解决因资源共享造成的并发问题

>### 分类
* 操作类型
    * 读锁（共享锁）
        * 对同一条数据，多个读操作可以同时进行，互不干扰
    * 写锁（互斥锁）
        * 如果当前写操作没有完毕，则无法进行其他读操作
* 操作范围
    * 表锁
        * 对整张表加锁
        * 开销小，加锁快
        * 无死锁
        * 容易发生锁冲突
            * 同时操作一条数据的概率增高
        * 并发度低
        * MyISAM 采用表锁
    * 行锁
        * 对一条数据加锁
        * 开销大，加锁慢
        * 容易出现死锁
        * 锁的范围较小，不易发生锁冲突
        * 高并发概率低
        * InnoDB 行锁
    * 页锁

>### 表锁
```shell
/* MYSQL/SQLSERVER 支持自增，Oracle 需要借助于序列来实现自增 */
create table tablelock
(
id int primary key auto_increment,
name varchar(20)
) engine myisam;

insert into tablelock(name) values('a1');
insert into tablelock(name) values('a2');
insert into tablelock(name) values('a3');
insert into tablelock(name) values('a4');
insert into tablelock(name) values('a5');

/* 查看加锁情况 */
show open tables;

/* 加锁 */
lock table tablelock read;

/* 加锁后可以读 */
select * from tablelock;

/* 加锁后不能写 */
/* ERROR 1099 (HY000): Table 'tablelock' was locked with a READ lock and can't be updated */
delete from tablelock where id=1;

/* 加锁后，当前会话不能对其他表进行读操作 */
/* ERROR 1100 (HY000): Table 'dept' was not locked with LOCK TABLES */
select count(1) from dept;

/* 加锁后，当前会话不能对其他表进行写操作 */
/* ERROR 1100 (HY000): Table 'dept' was not locked with LOCK TABLES */
insert into dept values(39,'xxxxxx', 'yyyyyyyy');

/* 释放锁 */
unlock tables;
```

* 会话
    * 每一个访问数据库的 dos 命令行，数据库客户端工具，都是一个会话
* 如果一个会话，对 A 表加了 read 锁
    * 该会话对 A 表
        * 读：可以
        * 写：不能
    * 该会话对其他表
        * 读：不能
        * 写：不能
* 此时其他会话
    * 对 A 表
        * 读：可以
        * 写，可以，需要等待锁释放
    * 对其他表
        * 读：可以
        * 写：可以

## (21) 写锁示例与 MyISAM 模式特征
```shell
/* 加写锁 */
lock table tablelock write;

/* 不能对其他表进行任何操作 */
/* ERROR 1100 (HY000): Table 'dept' was not locked with LOCK TABLES */
select count(1) from dept;
```
* 对 A 表加写锁
    * 当前会话对 A 表
        * 读：可以
        * 写：可以
    * 当前会话对其他表
        * 读：不能
        * 写：不能
* 其他会话
    * 对 A 表
        * 读：可以, 需要等待锁释放
        * 写，可以，需要等待锁释放
    * 对其他表
        * 读：可以
        * 写：可以

>### MySQL 表级锁的锁模式
* MyISAM 在执行查询语句前，会自动给涉及的所有表加读锁
* MyISAM 在执行更新操作（DML）前，会自动给涉及的表加写锁
* 对 MyISAM 表进行读操作
    * 其他进程对同一表的操作
        * 读：不阻塞
        * 写：阻塞
* 只有读锁释放后，才会执行其他进程的写操作
    * 对 MyISAM 表进行写操作
        * 其他进程对同一表操作
            * 读：阻塞
            * 写：阻塞
* 只有写锁释放后，才会执行其他进程的写操作

## (22) 写锁情况分析及行锁解析
* 分析表锁定
    * 查看哪些表加了锁
        ```shell
        show open tables
        ```
    * 分析表锁定的严重程度
        ```shell
        show status like '%table%'

        # Table_locks_immediate 能够获取到的锁
        # Table_locks_waited 需要等待的锁
        ```
        * Table_locks_immediate/Table_locks_waited> 5000
            * 建议采用 InnoDB 引擎
            * 否则使用 MyISAM 引擎
            * 能够获取到的资源充分时，使用行锁，因此采用 InnoDB

>### 行锁
```shell
create table linelock
(
id int(5) primary key auto_increment,
name varchar(20)
)engine=innodb;

insert into linelock(name) values('1');
insert into linelock(name) values('2');
insert into linelock(name) values('3');
insert into linelock(name) values('4');
insert into linelock(name) values('5');

set autocommit=0;
/* 当前会话操作第 6 行 */
insert into linelock values(6, 'a6');
/* 其他会话操作第 6 行 */
/* 无法操作，需要等待锁释放 */
update linelock set name='ax' where id=6;
/* 其他会话操作第 8 行，没有锁，可以操作 */
insert into linelock values(8, 'a8');

```
* 某个会话对一行数据进行 DML 操作时，其他会话需要等待锁释放
* 释放锁
    * 表锁：unlock tables; 或 commit/rollback 事务提交
    * 行锁：commit/rollback 事务提交

## (23) 行锁的注意事项
>### 行锁转为表锁
```shell
show index from linelock;
/* 为 name 列增加索引 */
alter table linelock add index idx_linelock_name(name);

/* 当前会话操作 name='3' 的行 */
update linelock set name='a3x' where name='3';
/* 其他会话操作 name='4' 的行 */
/* name 列索引有效，不同的行操作互不影响 */
update linelock set name='a4x' where name='4';

/* 当前会话操作 name=3 的行 */
/* name 列是 varchar 类型，而 3 是整数类型，类型转换时索引失效，行锁转为表锁 */
update linelock set name='a3x' where name=3;
/* 其他会话操作 name='4' 的行 */
/* name 列索引失效，表被锁定，无法操作 name='4' 行，需要等待锁释放 */
update linelock set name='a4x' where name='4';

```
* 如果没有索引，行锁会转为表锁

>### 间隙锁
```shell
/* 不存在 id=7 的数据，此时 MySQL 会自动加上间隙锁 */
update linelock set name='x' where id>1 and id<9;

/* 其他会话操作 id=7 需要等待锁释放 */
insert into linelock value(7, 'a7');
```

* 行锁的一种特殊情况
* MySQL 会自动给间隙加锁

>### 行锁
* 如果加锁时有 where 语句，where 范围内的数据都会被加锁
* 并发能力强，效率高

>### 行锁分析
```shell
show status like '%innodb_row_lock%';
```

|  类型   | 说明  |
|  ----  | ----  |
| Innodb_row_lock_current_waits  | 当前正在等待锁的进程数量 |
| Innodb_row_lock_time  | 从系统启动到现在，等待总时长 |
| Innodb_row_lock_time_avg  | 从系统启动到现在，平均等待时长 |
| Innodb_row_lock_time_max  | 从系统启动到现在，最大等待时长 |
| Innodb_row_lock_waits  | 从系统启动到现在，等待次数 |
## (24) 查询行锁如果锁定一行
```shell
/* for update 为查询语句加锁 */
select * from linelock where id=2 for update;

/* 其他会话操作该行要等待锁释放 */
update linelock set name='x' where id=2;
```
* 通过 for update 对 query 语句加锁
* 关闭事务自动提交的三种方式
    * set autocommit =0;
    * start transaction;
    * begin;
