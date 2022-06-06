#
**MySQL入门：**

MySQL基础笔记可看 [菜鸟教程](https://www.runoob.com/mysql/mysql-tutorial.html)

mysql基础视频教程 bilibili 上搜即可

---

**MySQL进阶：**

- **尚硅谷MySQL数据库高级**

  视频：https://www.bilibili.com/video/BV1KW411u7vy

  笔记链接：https://pan.baidu.com/s/1GUzPFVG3Je9uT419rHE8MQ 

  提取码：ybfi

- **黑马程序员2020最新MySQL高级教程**

  视频：https://www.bilibili.com/video/BV1UQ4y1P7Xr

  笔记：https://gitee.com/yooome/netty-study




我刚开始看的是尚硅谷的，看了一半跑去看黑马的了

这两教程内容都差不多，黑马的更多一些



推荐书籍：《深入浅出mysql》

视频内容围绕着这本书上内容讲的


# Mysql 逻辑架构简介

### 整体架构图

![img](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/540235-20160927083854563-2139392246.jpg)

和其它数据库相比，MySQL 有点与众不同，它的架构可以在多种不同场景中应用并发挥良好作用。主要体现在存储引擎的架构上，插件式的存储引擎架构将查询处理和其它的系统任务以及数据的存储提取相分离。这种架构可 以根据业务的需求和实际需要选择合适的存储引擎。

**各层介绍：**

#### 连接层

最上层是一些客户端和连接服务，包含本地 sock 通信和大多数基于客户端/服务端工具实现的类似于 tcp/ip 的通信。主要完成一些类似于连接处理、授权认证、及相关的安全方案。在该层上引入了线程池的概念，为通过认证 安全接入的客户端提供线程。同样在该层上可以实现基于 SSL 的安全链接。服务器也会为安全接入的每个客户端验 证它所具有的操作权限。

#### 服务层

- Management Serveices & Utilities

  系统管理和控制工具

- SQL Interface

  SQL 接口。接受用户的 SQL 命令，并且返回用户需要查询的结果。比如 select from 就是调用 SQL Interface

- Parser

  解析器。 SQL 命令传递到解析器的时候会被解析器验证和解析

- Optimizer

  查询优化器。 SQL 语句在查询之前会使用查询优化器对查询进行优化，比如有 where 条件时，优化器来决定先投影还是先过滤。

- Cache 和 Buffer

  查询缓存。如果查询缓存有命中的查询结果，查询语句就可以直接去查询缓存中取数据。这个缓存机制是由一系列小缓存组成的。比如表缓存，记录缓存，key 缓存， 权限缓存等
  
  注：mysql 8.X 取消了查询缓存

#### 引擎层

存储引擎层，存储引擎真正的负责了 MySQL 中数据的存储和提取，服务器通过 API 与存储引擎进行通信。不同 的存储引擎具有的功能不同，这样我们可以根据自己的实际需要进行选取。

#### 存储层

数据存储层，主要是将数据存储在运行于裸设备的文件系统之上，并完成与存储引擎的交互。



### show profile

利用 show profile 可以查看 sql 的执行周期！

**开启 profile**

查看 profile 是否开启：show variables like '%profiling%'

```sh
mysql> show variables like '%profiling%';
+------------------------+-------+
| Variable_name          | Value |
+------------------------+-------+
| have_profiling         | YES   |
| profiling              | OFF   |
| profiling_history_size | 15    |
+------------------------+-------+
3 rows in set (0.01 sec)
```

如果没有开启，可以执行 set profiling=1 开启！

**使用 profile**

执行 `show profiles;`  命令，可以查看最近的几次查询。

根据 `Query_ID`，可以进一步执行 `show profile cpu,block io for query Query_id` 来查看 sql 的具体执行步骤。



### 大致的查询流程

mysql 的查询流程大致是：

mysql 客户端通过协议与 mysql 服务器建连接，发送查询语句，先检查查询缓存，如果命中，直接返回结果， 否则进行语句解析,也就是说，在解析查询之前，服务器会先访问查询缓存(query cache)——它存储 SELECT 语句以及 相应的查询结果集。如果某个查询结果已经位于缓存中，服务器就不会再对查询进行解析、优化、以及执行。它仅仅将缓存中的结果返回给用户即可，这将大大提高系统的性能。

语法解析器和预处理：首先 mysql 通过关键字将 SQL 语句进行解析，并生成一颗对应的“解析树”。mysql 解析器将使用 mysql 语法规则验证和解析查询；预处理器则根据一些 mysql 规则进一步检查解析数是否合法。

查询优化器当解析树被认为是合法的了，并且由优化器将其转化成执行计划。一条查询可以有很多种执行方式， 最后都返回相同的结果。优化器的作用就是找到这其中最好的执行计划。

然后，mysql 默认使用的 BTREE 索引，并且一个大致方向是：无论怎么折腾 sql，至少在目前来说，mysql 最多只用到表中的一个索引。



### SQL的执行顺序

手写的顺序：

![image-20210520161848827](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520161848827.png)

真正执行的顺序：

​		随着 Mysql 版本的更新换代，其优化器也在不断的升级，优化器会分析不同执行顺序产生的性能消耗不同而动 态调整执行顺序。下面是经常出现的查询顺序：

![image-20210520161931864](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520161931864.png)

![image-20210520164022838](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520164022838.png)



## 存储引擎

### 存储引擎概述

和大多数的数据库不同, MySQL中有一个存储引擎的概念, 针对不同的存储需求可以选择最优的存储引擎。

​	存储引擎就是存储数据，建立索引，更新查询数据等等技术的实现方式 。存储引擎是基于表的，而不是基于库的。所以存储引擎也可被称为表类型。

​	Oracle，SqlServer等数据库只有一种存储引擎。MySQL提供了插件式的存储引擎架构。所以MySQL存在多种存储引擎，可以根据需要使用相应引擎，或者编写存储引擎。

​	MySQL5.0支持的存储引擎包含 ： InnoDB 、MyISAM 、BDB、MEMORY、MERGE、EXAMPLE、NDB Cluster、ARCHIVE、CSV、BLACKHOLE、FEDERATED等，其中InnoDB和BDB提供事务安全表，其他存储引擎是非事务安全表。

通过指令查询当前数据库支持的存储引擎 ： 

```sql
show engines
```

![1551186043529](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1551186043529.png)



创建新表时如果不指定存储引擎，那么系统就会使用默认的存储引擎，MySQL5.5之前的默认存储引擎是MyISAM，5.5之后就改为了InnoDB。

查看Mysql数据库默认的存储引擎 ， 指令 ：

```sql
show variables like '%storage_engine%' ； 
```

![1556086372754](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556086372754.png)

### 各种存储引擎特性

下面重点介绍几种常用的存储引擎， 并对比各个存储引擎之间的区别， 如下表所示 ： 

| 特点         | InnoDB               | MyISAM   | MEMORY | MERGE | NDB  |
| ------------ | -------------------- | -------- | ------ | ----- | ---- |
| 存储限制     | 64TB                 | 有       | 有     | 没有  | 有   |
| 事务安全     | **支持**             |          |        |       |      |
| 锁机制       | **行锁(适合高并发)** | **表锁** | 表锁   | 表锁  | 行锁 |
| B树索引      | 支持                 | 支持     | 支持   | 支持  | 支持 |
| 哈希索引     |                      |          | 支持   |       |      |
| 全文索引     | 支持(5.6版本之后)    | 支持     |        |       |      |
| 集群索引     | 支持                 |          |        |       |      |
| 数据索引     | 支持                 |          | 支持   |       | 支持 |
| 索引缓存     | 支持                 | 支持     | 支持   | 支持  | 支持 |
| 数据可压缩   |                      | 支持     |        |       |      |
| 空间使用     | 高                   | 低       | N/A    | 低    | 低   |
| 内存使用     | 高                   | 低       | 中等   | 低    | 高   |
| 批量插入速度 | 低                   | 高       | 高     | 高    | 高   |
| 支持外键     | **支持**             |          |        |       |      |

下面我们将重点介绍最长使用的两种存储引擎： InnoDB、MyISAM ， 另外两种 MEMORY、MERGE ， 了解即可。

#### InnoDB

InnoDB 存储引擎是 Mysql 的默认存储引擎。

InnoDB存储引擎提供了具有提交、回滚、崩溃恢复能力的事务安全。但是对比 MyISAM 的存储引擎，InnoDB 写的处理效率差一些，并且会占用更多的磁盘空间以保留数据和索引。

InnoDB 存储引擎不同于其他存储引擎的特点 ： 

- 事务控制

  **

  ```sql
  create table goods_innodb(
  	id int NOT NULL AUTO_INCREMENT,
  	name varchar(20) NOT NULL,
      primary key(id)
  )ENGINE=innodb DEFAULT CHARSET=utf8;
  ```

  ```sql
  #1
  start transaction;
  #2
  insert into goods_innodb(id,name)values(null,'Meta20');
  #3
  commit;
  ```

  ![1556075130115](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556075130115.png)

  测试发现在 InnoDB 中是存在事务的 ；

- 外键约束

  MySQL支持外键的存储引擎只有 InnoDB ， 在创建外键的时候， 要求父表必须有对应的索引 ，子表在创建外键的时候，也会自动的创建对应的索引。

  下面两张表中 ， country_innodb 是父表 ， country_id 为主键索引，city_innodb 表是子表，country_id 字段为外键，对应于 country_innodb 表的主键 country_id 。

  ```sql
  create table country_innodb(
  	country_id int NOT NULL AUTO_INCREMENT,
      country_name varchar(100) NOT NULL,
      primary key(country_id)
  )ENGINE=InnoDB DEFAULT CHARSET=utf8;
  
  
  create table city_innodb(
  	city_id int NOT NULL AUTO_INCREMENT,
      city_name varchar(50) NOT NULL,
      country_id int NOT NULL,
      primary key(city_id),
      key idx_fk_country_id(country_id),
      CONSTRAINT `fk_city_country` FOREIGN KEY(country_id) REFERENCES country_innodb(country_id) ON DELETE RESTRICT ON UPDATE CASCADE
  )ENGINE=InnoDB DEFAULT CHARSET=utf8;
  
  
  
  insert into country_innodb values(null,'China'),(null,'America'),(null,'Japan');
  insert into city_innodb values(null,'Xian',1),(null,'NewYork',2),(null,'BeiJing',1);
  
  ```

  在创建索引时， 可以指定在删除、更新父表时，对子表进行的相应操作，包括 RESTRICT、CASCADE、SET NULL 和 NO ACTION。

  RESTRICT 和NO ACTION 相同， 是指限制在子表有关联记录的情况下， 父表不能更新；

  CASCADE 表示父表在更新或者删除时，更新或者删除子表对应的记录；

  SET NULL 则表示父表在更新或者删除的时候，子表的对应字段被SET NULL 。

  针对上面创建的两个表， 子表的外键指定是ON DELETE RESTRICT ON UPDATE CASCADE 方式的， 那么在主表删除记录的时候， 如果子表有对应记录， 则不允许删除， 主表在更新记录的时候， 如果子表有对应记录， 则子表对应更新 。

  

  表中数据如下图所示 ： 

  ![1556087540767](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556087540767.png)

  查看外键信息

  ```sql
  show create table city_innodb ;
  ```

  ![1556087611295](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556087611295.png)

  删除 country_id为 1 的 country 数据，有外键时会删除失败

  ![1556087719145](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556087719145.png)

  更新主表country表的字段 country_id 时

  ```sql
  update country_innodb set country_id = 100 where country_id = 1;
  ```

  ![1556087759615](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556087759615.png)

  更新后， 子表的数据信息为 ：

  ![1556087793738](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556087793738.png)

  

- **存储方式**	

  InnoDB 存储表和索引有以下两种方式 ： 

  ①. 使用共享表空间存储， 这种方式创建的表的表结构保存在 `.frm`文件中， 数据和索引保存在 innodb_data_home_dir 和 innodb_data_file_path 定义的表空间中，可以是多个文件。

  ②. 使用多表空间存储， 这种方式创建的表的表结构仍然存在 `.frm` 文件中，但是每个表的数据和索引单独保存在 `.ibd` 中。

  ![1556075336630](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556075336630.png)

  

#### MyISAM

MyISAM 不支持事务、也不支持外键，其优势是访问的速度快，对事务的完整性没有要求或者以SELECT、INSERT为主的应用基本上都可以使用这个引擎来创建表 。有以下两个比较重要的特点：

- 不支持事务

  ```sql
  create table goods_myisam(
  	id int NOT NULL AUTO_INCREMENT,
  	name varchar(20) NOT NULL,
      primary key(id)
  )ENGINE=myisam DEFAULT CHARSET=utf8;
  ```
  
  ![1551347590309](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1551347590309.png)
  
  通过测试，我们发现，在MyISAM存储引擎中，是没有事务控制的 ；
  
  
  
- 文件存储方式

  每个MyISAM在磁盘上存储成3个文件，其文件名都和表名相同，但拓展名分别是 ： 

  .frm (存储表定义)；

  .MYD(MYData , 存储数据)；

  .MYI(MYIndex , 存储索引)；

  ![1556075073836](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556075073836.png)



#### MEMORY

​	Memory存储引擎将表的数据存放在内存中。每个MEMORY表实际对应一个磁盘文件，格式是.frm ，该文件中只存储表的结构，而其数据文件，都是存储在内存中，这样有利于数据的快速处理，提高整个表的效率。MEMORY 类型的表访问非常地快，因为他的数据是存放在内存中的，并且默认使用HASH索引 ， 但是服务一旦关闭，表中的数据就会丢失。

#### MERGE

​	MERGE存储引擎是一组MyISAM表的组合，这些MyISAM表必须结构完全相同，MERGE表本身并没有存储数据，对MERGE类型的表可以进行查询、更新、删除操作，这些操作实际上是对内部的MyISAM表进行的。

​	对于MERGE类型表的插入操作，是通过INSERT_METHOD子句定义插入的表，可以有3个不同的值，使用FIRST 或 LAST 值使得插入操作被相应地作用在第一或者最后一个表上，不定义这个子句或者定义为NO，表示不能对这个MERGE表执行插入操作。

​	可以对MERGE表进行DROP操作，但是这个操作只是删除MERGE表的定义，对内部的表是没有任何影响的。



![1556076359503](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556076359503.png)

**下面是一个创建和使用MERGE表的示例 ：** 

1）. 创建3个测试表 order_1990, order_1991, order_all , 其中 order_all 是前两个表的 MERGE 表 ： 

```sql
create table order_1990(
    order_id int ,
    order_money double(10,2),
    order_address varchar(50),
    primary key (order_id)
)engine = myisam default charset=utf8;


create table order_1991(
    order_id int ,
    order_money double(10,2),
    order_address varchar(50),
    primary key (order_id)
)engine = myisam default charset=utf8;


create table order_all(
    order_id int ,
    order_money double(10,2),
    order_address varchar(50),
    primary key (order_id)
)engine = merge union = (order_1990,order_1991) INSERT_METHOD=LAST default charset=utf8;
```

2）. 分别向两张表中插入记录 

```sql
insert into order_1990 values(1,100.0,'北京');
insert into order_1990 values(2,100.0,'上海');

insert into order_1991 values(10,200.0,'北京');
insert into order_1991 values(11,200.0,'上海');
```

3）. 查询3张表中的数据。

order_1990中的数据 ： 

![1551408083254](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1551408083254.png)

order_1991中的数据 ： 

![1551408133323](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1551408133323.png)

order_all中的数据 ：

![1551408216185](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1551408216185.png)

4）. 往order_all中插入一条记录 ，由于在MERGE表定义时，INSERT_METHOD 选择的是LAST，那么插入的数据会想最后一张表中插入。

```sql
insert into order_all values(100,10000.0,'西安')；
```

![1551408519889](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1551408519889.png)



## SQL 预热

常见的 Join 查询图

![image-20210520162731111](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520162731111.png)

# 索引
## 索引的概念

索引（Index）是帮助 MySQL 高效获取数据的数据结构，可以简单理解为**排好序的快速查找数据结构**。

在数据之外，数据库系统还维护着满足特定查找算法的数据结构，这些数据结构以某种方式引用（指向）数据， 这样就可以在这些数据结构上实现高级查找算法。这种数据结构，就是索引



![1555902055367](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555902055367.png)



左边是数据表，一共有两列七条记录，最左边的是数据记录的物理地址（注意逻辑上相邻的记录在磁盘上也并不是一定物理相邻的）。为了加快Col2的查找，可以维护一个右边所示的二叉查找树，每个节点分别包含索引键值和一个指向对应数据记录物理地址的指针，这样就可以运用二叉查找快速获取到相应数据。

一般来说索引本身也很大，不可能全部存储在内存中，因此索引往往以索引文件的形式存储在磁盘上。索引是数据库中用来提高性能的最常用的工具。



**索引优缺点**

优势：

- 提高数据检索的效率，降低数据库的IO成本。
- 数据排序，降低CPU消耗

劣势：

- 虽然索引大大提高了查询速度，同时却会降低更新表的速度

  如对表进行INSERT、UPDATE和DELETE。因为更新表时，MySQL不仅要保存数据，还要保存一下索引文件每次更新添加了索引列的字段，都会调整因更新所带来的键值变化后的索引信息。

- 索引本质也是一张表，保存着索引字段和指向实际记录的指针，所以也要占用数据库空间，一般而言，索引表占用的空间是数据表的1.5倍





## 推荐文章

- [MySQL 索引原理 图文讲解](https://zhuanlan.zhihu.com/p/359306500)

  涉及到树相关数据结构知识。

- [BTree和B+Tree](https://www.jianshu.com/p/ac12d2c83708)

  详细介绍

## 索引结构

### Btree 索引结构

黑马教程：https://www.bilibili.com/video/BV1UQ4y1P7Xr?p=6

**Btree又可以写成B-tree**（B-Tree，并不是B“减”树，横杠为连接符，容易被误导）

BTree又叫多路平衡搜索树，一颗 **m** 叉的BTree特性如下：

- 树中每个节点最多包含m个孩子。
- 除根节点与叶子节点外，每个节点至少有 [ceil(m/2)] 个孩子。
- 若根节点不是叶子节点，则至少有两个孩子。
- 所有的叶子节点都在同一层。
- 每个非叶子节点由 n 个 key 与 n+1 个指针组成，其中 [ceil(m/2)-1] <= n <= m-1 

celi()：向上取整，例如celi(2.5)=3



#### 演变过程

以5叉 BTree 为例，key的数量：公式推导 [ceil(m/2)-1] <= n <= m-1。所以 2 <= n <=4 。

当 n>4 时，中间节点分裂到父节点，两边节点分裂。

插入 C N G A H E K Q M F W L T Z D P R X Y S 数据为例。（插入时，按照ABCD..顺序）

1). 插入前4个字母 C N G A 

![1555944126588](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944126588.png)

2). 插入H，n>4，中间元素G字母向上分裂到新的节点

![1555944549825](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944549825.png)

3). 插入E，K，Q不需要分裂

![1555944596893](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944596893.png)

4). 插入M，中间元素M字母向上分裂到父节点G

（M 在 K、N中间，BTree最多含有n-1个key，这里即4个key，5个指针）

![1555944652560](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944652560.png)

5). 插入F，W，L，T不需要分裂

![1555944686928](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944686928.png)

6). 插入Z，中间元素T向上分裂到父节点中

（插入Z后是，NQTWZ，把中间T提出来，方便更快的查询，所以不提出Z）

![1555944713486](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944713486.png)

7). 插入D，中间元素D向上分裂到父节点中。然后插入P，R，X，Y不需要分裂

![1555944749984](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944749984.png)

8). 最后插入S（R后面），NPQR节点n>5，中间节点Q向上分裂，但分裂后父节点DGMT的n>5，中间节点M向上分裂

![1555944848294](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555944848294.png)

到此，该BTREE树就已经构建完成了， BTREE树 和 二叉树 相比， 查询数据的效率更高， 因为对于相同的数据量来说，BTREE的层级结构比二叉树小，因此搜索速度快。



#### 其他

![image-20210520190717898](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520190717898.png)

**初始化介绍**



一颗 b 树，浅蓝色的块我们称之为一个磁盘块，可以看到每个磁盘块包含几个数据项（深蓝色所示）和指针（黄色 所示），

如磁盘块 1 包含数据项 17 和 35，包含指针 P1、P2、P3，
P1 表示小于 17 的磁盘块，P2 表示在 17 和 35 之间的磁盘块，P3 表示大于 35 的磁盘块。
真实的数据存在于叶子节点即 3、5、9、10、13、15、28、29、36、60、75、79、90、99。
非叶子节点只不存储真实的数据，只存储指引搜索方向的数据项，如 17、35 并不真实存在于数据表中

**查找过程**

如果要查找数据项 29，那么首先会把磁盘块 1 由磁盘加载到内存，此时发生一次 IO，在内存中用二分查找确定 29 在 17 和 35 之间，锁定磁盘块 1 的 P2 指针，内存时间因为非常短（相比磁盘的 IO）可以忽略不计，通过磁盘块 1 的 P2 指针的磁盘地址把磁盘块 3 由磁盘加载到内存，发生第二次 IO，29 在 26 和 30 之间，锁定磁盘块 3 的 P2 指 针，通过指针加载磁盘块 8 到内存，发生第三次 IO，同时内存中做二分查找找到 29，结束查询，总计三次 IO。



真实的情况是，3 层的 b+树可以表示上百万的数据，如果上百万的数据查找只需要三次 IO，性能提高将是巨大的， 如果没有索引，每个数据项都要发生一次 IO，那么总共需要百万次的 IO，显然成本非常非常高。



### B+tree 结构

![1555906287178](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/00001.jpg)

B+Tree为BTree的变种，B+Tree与BTree的区别为：

1). n叉B+Tree最多含有n个key，而BTree最多含有n-1个key。

2). B+Tree的叶子节点保存所有的key信息，依key大小顺序排列。

3). 所有的非叶子节点都可以看作是key的索引部分。



- B-树的关键字和记录是放在一起的，叶子节点可以看作外部节点，不包含任何信息；B+树的非叶子节点中只有关键字和指向下一个节点的索引，记录只放在叶子节点中。
- 在 B-树中，越靠近根节点的记录查找时间越快，只要找到关键字即可确定记录的存在；而 B+树中每个记录的查找时间基本是一样的，都需要从根节点走到叶子节点，而且在叶子节点中还要再比较关键字。从这个角度看 B- 树的性能好像要比 B+树好，而在实际应用中却是 B+树的性能要好些。因为 B+树的非叶子节点不存放实际的数据， 这样每个节点可容纳的元素个数比 B-树多，树高比 B-树小，这样带来的好处是减少磁盘访问次数。尽管 B+树找到 一个记录所需的比较次数要比 B-树多，但是一次磁盘访问的时间相当于成百上千次内存比较的时间，因此实际中 B+树的性能可能还会好些，而且 B+树的叶子节点使用指针连接在一起，方便顺序遍历（例如查看一个目录下的所有 文件，一个表中的所有记录等），这也是很多数据库和文件系统使用 B+树的缘故。

**为什么B+树比 B-树更适合索引？**

- B+树的磁盘读写代价更低

  B+树的内部结点并没有指向关键字具体信息的指针。因此其内部结点相对 B 树更小。如果把所有同一内部结点 的关键字存放在同一盘块中，那么盘块所能容纳的关键字数量也越多。一次性读入内存中的需要查找的关键字也就 越多。相对来说 IO 读写次数也就降低了。

- B+树的查询效率更加稳定

  由于非终结点并不是最终指向文件内容的结点，而只是叶子结点中关键字的索引。所以任何关键字的查找必须 走一条从根结点到叶子结点的路。所有关键字查询的路径长度相同，导致每一个数据的查询效率相当。

###  MySQL中的B+Tree

MySql索引数据结构对经典的B+Tree进行了优化。在原B+Tree的基础上，增加一个指向相邻叶子节点的链表指针，就形成了带有顺序指针的B+Tree，提高区间访问的性能。

MySQL中的 B+Tree 索引结构示意图: 

![1555906287178](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555906287178.png)



### 聚簇索引和非聚簇索引

聚簇索引并不是一种单独的索引类型，而是一种数据存储方式。术语‘聚簇’表示数据行和相邻的键值聚簇的存储 在一起。如下图，左侧的索引就是聚簇索引，因为数据行在磁盘的排列和索引排序保持一致。



![image-20210520211641159](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520211641159.png)

**聚簇索引的好处**

按照聚簇索引排列顺序，查询显示一定范围数据的时候，由于数据都是紧密相连，数据库不不用从多 个数据块中提取数据，所以节省了大量的 io 操作。

**聚簇索引的限制**

对于 mysql 数据库目前只有 innodb 数据引擎支持聚簇索引，而 Myisam 并不支持聚簇索引。

由于数据物理存储排序方式只能有一种，所以每个 Mysql 的表只能有一个聚簇索引。一般情况下就是该表的主键。

为了充分利用聚簇索引的聚簇的特性，所以 innodb 表的主键列尽量选用有序的顺序 id，而不建议用无序的 id，比如 uuid 这种。

### 时间复杂度

同一问题可用不同算法解决，而一个算法的质量优劣将影响到算法乃至程序的效率。算法分析的目的在于选择合适算法和改进算法。

时间复杂度是指执行算法所需要的计算工作量，用大 O 表示记为：O(…)

![image-20210520211835491](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520211835491.png)

![image-20210520212305695](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210520212305695.png)

## 索引分类

### 单值索引

概念：即一个索引只包含单个列，一个表可以有多个单列索引

- 所表一起创建

  ```sql
  CREATE TABLE customer (
    id INT (10) UNSIGNED AUTO_INCREMENT,
    customer_no VARCHAR (200),
    customer_name VARCHAR (200),
    PRIMARY KEY (id),
    KEY (customer_name)	#this
  );
  ```

- 单独建单值索引

  ```sql
  CREATE INDEX idx_customer_name
  ON customer (customer_name);
  ```

### 唯一索引

概念：索引列的值必须唯一，但允许有空值

- 随表一起创建

  ```sql
  CREATE TABLE customer (
    id INT (10) UNSIGNED AUTO_INCREMENT,
    customer_no VARCHAR (200),
    customer_name VARCHAR (200),
    PRIMARY KEY (id),
    KEY (customer_name),
    UNIQUE (customer_no)	#this
  );
  ```

- 单独建唯一索引：

  ```sql
  CREATE UNIQUE INDEX idx_customer_no
  ON customer (customer_no);
  ```



### 复合索引

概念：即一个索引包含多个列

- 随表一起建索引

  ```sql
  CREATE TABLE customer (
    id INT (10) UNSIGNED AUTO_INCREMENT,
    customer_no VARCHAR (200),
    customer_name VARCHAR (200),
    PRIMARY KEY (id),
    KEY (customer_name),
    UNIQUE (customer_name),
    KEY (customer_no, customer_name)	#this
  );
  ```

- 单独建索引：

  ```sql
  CREATE INDEX idx_no_name
  ON customer (customer_no, customer_name);
  ```

  

### 主键索引

概念：设定为主键后数据库会自动建立索引，innodb为聚簇索引

- 随表一起建索引

  ```sql
  CREATE TABLE customer (
    id INT (10) UNSIGNED AUTO_INCREMENT,
    customer_no VARCHAR (200),
    customer_name VARCHAR (200),
    PRIMARY KEY (id)	#this
  );
  ```

- 单独建主键索引：

  ```sql
  ALTER TABLE customer ADD PRIMARY KEY customer(customer_no);
  ```

- 删除主键索引

  ```sql
  ALTER TABLE customer drop PRIMARY KEY ;
  ```

- 修改建主键索引

  必须先删除掉(drop)原索引，再新建(add)索引

  

### 索引基本语法

- 创建

  ```sql
  CREATE [UNIQUE] INDEX [indexName]
  ON table_name(column))
  ```

  示例 ： 为city表中的city_name字段创建索引 ；

  ![1551438009843](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1551438009843.png)

- 删除

  ```sql
  DROP  INDEX  index_name  ON  tbl_name;
  ```

- 查看

  ```sql
  show index  from  table_name;
  ```

- AlTER

  ```
  1). alter  table  tb_name  add  primary  key(column_list); 
  
  	该语句添加一个主键，这意味着索引值必须是唯一的，且不能为NULL
  	
  2). alter  table  tb_name  add  unique index_name(column_list);
  	
  	这条语句创建索引的值必须是唯一的（除了NULL外，NULL可能会出现多次）
  	
  3). alter  table  tb_name  add  index index_name(column_list);
  
  	添加普通索引， 索引值可以出现多次。
  	
  4). alter  table  tb_name  add  fulltext  index_name(column_list);
  	
  	该语句指定了索引为FULLTEXT， 用于全文索引
  	
  ```




## 索引设计原则



索引的设计可以遵循一些已有的原则，创建索引的时候请尽量考虑符合这些原则，便于提升索引的使用效率，更高效的使用索引。

- 对查询频次较高，且数据量比较大的表建立索引。

- 索引字段的选择，最佳候选列应当从where子句的条件中提取，如果where子句中的组合比较多，那么应当挑选最常用、过滤效果最好的列的组合。

- 使用唯一索引，区分度越高，使用索引的效率越高。

- 索引可以有效的提升查询数据的效率，但索引数量不是多多益善，索引越多，维护索引的代价自然也就水涨船高。对于插入、更新、删除等DML操作比较频繁的表来说，索引过多，会引入相当高的维护代价，降低DML操作的效率，增加相应操作的时间消耗。另外索引过多的话，MySQL也会犯选择困难病，虽然最终仍然会找到一个可用的索引，但无疑提高了选择的代价。

- 使用短索引，索引创建之后也是使用硬盘来存储的，因此提升索引访问的I/O效率，也可以提升总体的访问效率。假如构成索引的字段总长度比较短，那么在给定大小的存储块内可以存储更多的索引值，相应的可以有效的提升MySQL访问索引的I/O效率。

- 利用最左前缀，N个列组合而成的组合索引，那么相当于是创建了N个索引，如果查询时where子句中使用了组成该索引的前几个字段，那么这条查询SQL可以利用组合索引来提升查询效率。

  
  
  创建复合索引
  
  ```sql
  CREATE INDEX idx_name_email_status ON tb_seller(NAME,email,STATUS);
  ```
  
  就相当于
  
	​	对 name 创建索引 ;
	​	对 name , email 创建了索引 ;
	​	对 name , email, status 创建了索引 ;

**不适合创建索引的情况**

- 表记录太少
- 经常增删改的表或者字段
- Where 条件里用不到的字段不创建索引
- 过滤性不好的不适合建索引

# 查看SQL执行频率

MySQL 客户端连接成功后，通过 `show [session|global] status` 命令可以提供服务器状态信息。

show [session|global] status 可以根据需要加上参数“session”或者“global”来显示 session 级（当前连接）的计结果和 global 级（自数据库上次启动至今）的统计结果。如果不写，默认使用参数是“session”。

下面的命令显示了当前 session 中所有统计参数的值：

```sql
show status like 'Com_______';
```

Com_xxx 表示每个 xxx 语句执行的次数

![1552487172501](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552487172501.png)

```sql
show status like 'Innodb_rows_%';
```

我们通常比较关心的是以下几个统计参数

| 参数                 | 含义                                                         |
| :------------------- | ------------------------------------------------------------ |
| Com_select           | 执行 select 操作的次数，一次查询只累加 1。                   |
| Com_insert           | 执行 INSERT 操作的次数，对于批量插入的 INSERT 操作，只累加一次。 |
| Com_update           | 执行 UPDATE 操作的次数。                                     |
| Com_delete           | 执行 DELETE 操作的次数。                                     |
| Innodb_rows_read     | select 查询返回的行数。                                      |
| Innodb_rows_inserted | 执行 INSERT 操作插入的行数。                                 |
| Innodb_rows_updated  | 执行 UPDATE 操作更新的行数。                                 |
| Innodb_rows_deleted  | 执行 DELETE 操作删除的行数。                                 |
| Connections          | 试图连接 MySQL 服务器的次数。                                |
| Uptime               | 服务器工作时间。                                             |
| Slow_queries         | 慢查询的次数。                                               |

Com_***      :  这些参数对于所有存储引擎的表操作都会进行累计。

Innodb_*** :  这几个参数只是针对InnoDB 存储引擎的，累加的算法也略有不同。

## 定位低效率执行SQL



- 慢查询日志 

   通过慢查询日志定位那些执行效率较低的 SQL 语句，用 log-slow-queries[file_name] 选项启动时，mysqld 写一个包含所有执行时间超过 long_query_time 秒的 SQL 语句的日志文件。具体可以查看日志管理的相关部分。

- show processlist  

  慢查询日志在查询结束以后才纪录，所以在应用反映执行效率出现问题的时候查询慢查询日志并不能定位问题，可以使用 `show processlist` 命令查看当前MySQL在进行的线程，包括线程的状态、是否锁表等，可以实时地查看 SQL 的执行情况，同时对一些锁表操作进行优化。

![1556098544349](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556098544349.png)

1） id列，用户登录mysql时，系统分配的"connection_id"，可以使用函数connection_id()查看

2） user列，显示当前用户。如果不是root，这个命令就只显示用户权限范围的sql语句

3） host列，显示这个语句是从哪个ip的哪个端口上发的，可以用来跟踪出现问题语句的用户

4） db列，显示这个进程目前连接的是哪个数据库

5） command列，显示当前连接的执行的命令，一般取值为休眠（sleep），查询（query），连接（connect）等

6） time列，显示这个状态持续的时间，单位是秒

7） state列，显示使用当前连接的sql语句的状态，很重要的列。state描述的是语句执行中的某一个状态。一个sql语句，以查询为例，可能需要经过copying to tmp table、sorting result、sending data等状态才可以完成

8） info列，显示这个sql语句，是判断问题语句的一个重要依据

## explain分析执行计划

通过 EXPLAIN 或者 DESC命令获取 MySQL 如何执行 SELECT 语句的信息，包括在 SELECT 语句执行过程中表如何连接和连接的顺序。

```sql
explain  select * from tb_item where id = 1;
```

![1552487489859](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552487489859.png)



![1552487526919](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552487526919.png)

| 字段          | 含义                                                         |
| ------------- | ------------------------------------------------------------ |
| id            | select查询的序列号，是一组数字，表示的是查询中执行select子句或者是操作表的顺序。 |
| select_type   | 表示 SELECT 的类型，常见的取值有 SIMPLE（简单表，即不使用表连接或者子查询）、PRIMARY（主查询，即外层的查询）、UNION（UNION 中的第二个或者后面的查询语句）、SUBQUERY（子查询中的第一个 SELECT）等 |
| table         | 输出结果集的表                                               |
| type          | 表示表的连接类型，性能由好到差的连接类型为( system ---> const -----> eq_ref ------> ref -------> ref_or_null----> index_merge ---> index_subquery -----> range -----> index ------> all ) |
| possible_keys | 表示查询时，可能使用的索引                                   |
| key           | 表示实际使用的索引                                           |
| key_len       | 索引字段的长度                                               |
| rows          | 扫描行的数量                                                 |
| extra         | 执行情况的说明和描述                                         |

###  环境准备

![1556122799330](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556122799330.png)

```sql
CREATE TABLE `t_role` (
  `id` VARCHAR(32) NOT NULL,
  `role_name` VARCHAR(255) DEFAULT NULL,
  `role_code` VARCHAR(255) DEFAULT NULL,
  `description` VARCHAR(255) DEFAULT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `unique_role_name` (`role_name`)
) ENGINE=INNODB DEFAULT CHARSET=utf8;

CREATE TABLE `t_user` (
  `id` VARCHAR(32) NOT NULL,
  `username` VARCHAR(45) NOT NULL,
  `password` VARCHAR(96) NOT NULL,
  `name` VARCHAR(45) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `unique_user_username` (`username`)
) ENGINE=INNODB DEFAULT CHARSET=utf8;

CREATE TABLE `user_role` (
  `id` INT(11) NOT NULL AUTO_INCREMENT ,
  `user_id` VARCHAR(32) DEFAULT NULL,
  `role_id` VARCHAR(32) DEFAULT NULL,
  PRIMARY KEY (`id`),
  KEY `fk_ur_user_id` (`user_id`),
  KEY `fk_ur_role_id` (`role_id`),
  CONSTRAINT `fk_ur_role_id` FOREIGN KEY (`role_id`) REFERENCES `t_role` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION,
  CONSTRAINT `fk_ur_user_id` FOREIGN KEY (`user_id`) REFERENCES `t_user` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION
) ENGINE=INNODB DEFAULT CHARSET=utf8;

INSERT INTO `t_user` (`id`, `username`, `password`, `name`) VALUES('1','super','$2a$10$TJ4TmCdK.X4wv/tCqHW14.w70U3CC33CeVncD3SLmyMXMknstqKRe','超级管理员');
INSERT INTO `t_user` (`id`, `username`, `password`, `name`) VALUES('2','admin','$2a$10$TJ4TmCdK.X4wv/tCqHW14.w70U3CC33CeVncD3SLmyMXMknstqKRe','系统管理员');
INSERT INTO `t_user` (`id`, `username`, `password`, `name`) VALUES('3','itcast','$2a$10$8qmaHgUFUAmPR5pOuWhYWOr291WJYjHelUlYn07k5ELF8ZCrW0Cui','test02');
INSERT INTO `t_user` (`id`, `username`, `password`, `name`) VALUES('4','stu1','$2a$10$pLtt2KDAFpwTWLjNsmTEi.oU1yOZyIn9XkziK/y/spH5rftCpUMZa','学生1');
INSERT INTO `t_user` (`id`, `username`, `password`, `name`) VALUES('5','stu2','$2a$10$nxPKkYSez7uz2YQYUnwhR.z57km3yqKn3Hr/p1FR6ZKgc18u.Tvqm','学生2');
INSERT INTO `t_user` (`id`, `username`, `password`, `name`) VALUES('6','t1','$2a$10$TJ4TmCdK.X4wv/tCqHW14.w70U3CC33CeVncD3SLmyMXMknstqKRe','老师1');

INSERT INTO `t_role` (`id`, `role_name`, `role_code`, `description`) VALUES('5','学生','student','学生');
INSERT INTO `t_role` (`id`, `role_name`, `role_code`, `description`) VALUES('7','老师','teacher','老师');
INSERT INTO `t_role` (`id`, `role_name`, `role_code`, `description`) VALUES('8','教学管理员','teachmanager','教学管理员');
INSERT INTO `t_role` (`id`, `role_name`, `role_code`, `description`) VALUES('9','管理员','admin','管理员');
INSERT INTO `t_role` (`id`, `role_name`, `role_code`, `description`) VALUES('10','超级管理员','super','超级管理员');

INSERT INTO user_role(id,user_id,role_id) VALUES(NULL, '1', '5'),(NULL, '1', '7'),(NULL, '2', '8'),(NULL, '3', '9'),(NULL, '4', '8'),(NULL, '5', '10') ;

```

### explain 之 id

id 字段是 select查询的序列号，是一组数字，表示的是查询中执行select子句或者是操作表的顺序。id 情况有三种 

1） id 相同表示加载表的顺序是从上到下。

```sql
explain select * from t_role r, t_user u, user_role ur where r.id = ur.role_id and u.id = ur.user_id ;
```

![1556102471304](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556102471304.png)

2） id 不同id值越大，优先级越高，越先被执行。 

```sql
EXPLAIN SELECT * FROM t_role WHERE id = (SELECT role_id FROM user_role WHERE user_id = (SELECT id FROM t_user WHERE username = 'stu1'))
```

![1556103009534](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556103009534.png)

3） id 有相同，也有不同，同时存在。id相同的可以认为是一组，从上往下顺序执行；在所有的组中，id的值越大，优先级越高，越先执行。

```sql
EXPLAIN SELECT * FROM t_role r , (SELECT * FROM user_role ur WHERE ur.`user_id` = '2') a WHERE r.id = a.role_id ; 
```

![1556103294182](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556103294182.png)

### explain 之 select_type

表示 SELECT 的类型，常见的取值，如下表所示：

| select_type  | 含义                                                         |
| ------------ | ------------------------------------------------------------ |
| SIMPLE       | 简单的select查询，查询中不包含子查询或者UNION                |
| PRIMARY      | 查询中若包含任何复杂的子查询，最外层查询标记为该标识         |
| SUBQUERY     | 在SELECT 或 WHERE 列表中包含了子查询                         |
| DERIVED      | 在FROM 列表中包含的子查询，被标记为 DERIVED（衍生） MYSQL会递归执行这些子查询，把结果放在临时表中 |
| UNION        | 若第二个SELECT出现在UNION之后，则标记为UNION ； 若UNION包含在FROM子句的子查询中，外层SELECT将被标记为 ： DERIVED |
| UNION RESULT | 从UNION表获取结果的SELECT                                    |

- SIMPLE

  SIMPLE 代表单表查询

  ```sql
  EXPLAIN SELECT * FROM t_user;
  ```

  ![image-20210522183120093](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210522183120093.png)

  

- PRIMARY、SUBQUERY

  在 SELECT 或 WHERE 列表中包含了子查询。最外层查询则被标记为 Primary。

  ```sql
  explain select * from t_user where id = (select id from user_role where role_id='9' );
  ```

  ![image-20210522183137975](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210522183137975.png)

- DERIVED

  在 FROM 列表中包含的子查询被标记为 DERIVED(衍生)，MySQL 会递归执行这些子查询, 把结果放在临时表里。

  ```sql
  explain select a.* from (select * from t_user where id in('1','2') ) a;
  ```

  mysql 5.7 中为 `simple`

  ![image-20210522180244911](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210522180244911.png)

  

  mysql 5.6 中：

  ![image-20210522182540547](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210522182540547.png)

  

- union

  ```sql
  explain select * from t_user where id='1' union select * from  t_user where id='2';
  ```

  ![image-20210522183718254](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210522183718254.png)



### explain 之 table

展示这一行的数据是关于哪一张表的 

没有与之关系的表为 NULL

![image-20210522190653729](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210522190653729.png)



### explain 之 type

type 显示的是访问类型，是较为重要的一个指标，可取值为： 

| type   | 含义                                                         |
| ------ | ------------------------------------------------------------ |
| NULL   | MySQL不访问任何表，索引，直接返回结果                        |
| system | 表只有一行记录(等于系统表)，这是const类型的特例，一般不会出现 |
| const  | 表示通过索引一次就找到了，const 用于比较primary key 或者 unique 索引。因为只匹配一行数据，所以很快。如将主键置于where列表中，MySQL 就能将该查询转换为一个常亮。const于将 "主键" 或 "唯一" 索引的所有部分与常量值进行比较 |
| eq_ref | 类似ref，区别在于使用的是唯一索引，使用主键的关联查询，关联查询出的记录只有一条。常见于主键或唯一索引扫描 |
| ref    | 非唯一性索引扫描，返回匹配某个单独值的所有行。本质上也是一种索引访问，返回所有匹配某个单独值的所有行（多个） |
| range  | 只检索给定返回的行，使用一个索引来选择行。 where 之后出现 between ， < , > , in 等操作。 |
| index  | index 与 ALL的区别为 index 类型只是遍历了索引树， 通常比ALL 快， ALL 是遍历数据文件。 |
| all    | 将遍历全表以找到匹配的行                                     |

结果值从最好到最坏以此是：

- NULL > system > const > eq_ref > ref > fulltext > ref_or_null > index_merge > unique_subquery > index_subquery > range > index > ALL

- system > const > eq_ref > ref > range > index > ALL

<mark>一般来说， 我们需要保证查询至少达到 range 级别， 最好达到ref </mark>

### explain 之 key



- possible_keys :

  显示可能应用在这张表的索引， 一个或多个。 

- key 

  实际使用的索引， 如果为NULL， 则没有使用索引。

- key_len 

  表示索引中使用的字节数， 该值为索引字段最大可能长度，并非实际使用长度，在不损失精确性的前提下， 长度越短越好 。

###  explain 之 rows

扫描行的数量。

### explain 之 extra

其他的额外的执行计划信息，在该列展示 。

| extra            | 含义                                                         |
| ---------------- | ------------------------------------------------------------ |
| using  filesort  | 说明mysql会对数据使用一个外部的索引排序，而不是按照表内的索引顺序进行读取， 称为 “文件排序”, 效率低。 |
| using  temporary | 使用了临时表保存中间结果，MySQL在对查询结果排序时使用临时表。常见于 order by 和 group by； 效率低 |
| using  index     | 表示相应的select操作使用了覆盖索引， 避免访问表的数据行， 效率不错。 |

## show profile分析SQL

Mysql从5.0.37版本开始增加了对 show profiles 和 show profile 语句的支持。

show profiles 能够在做SQL优化时帮助我们了解时间都耗费到哪里去了。

通过 have_profiling 参数，能够看到当前MySQL是否支持profile：

![1552488401999](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552488401999.png)

默认profiling是关闭的，可以通过set语句在Session级别开启profiling：

![1552488372405](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552488372405.png)

```sql
set profiling=1; //开启profiling 开关；
```

通过profile，我们能够更清楚地了解SQL执行的过程。

我们可以执行一系列的操作：

```sql
show databases;

use db01;

show tables;

select * from tb_item where id < 5;

select count(*) from tb_item;
```

执行完上述命令之后，再执行 `show profiles` 指令， 来查看SQL语句执行的耗时：

![1552489017940](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552489017940.png)

通过 `show  profile for  query  query_id` 语句查看该SQL执行过程中每个线程的状态和消耗的时间

![1552489053763](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552489053763.png)

TIP：Sending data 状态表示 MySQL 线程开始访问数据行并把结果返回给客户端，而不仅仅是返回个客户端。由于在 Sending data 状态下，MySQL 线程往往需要做大量的磁盘读取操作，所以经常是整各查询中耗时最长的状态。

在获取到最消耗时间的线程状态后，MySQL支持进一步选择all、cpu、block io 、context switch、page faults等明细类型类查看MySQL在使用什么资源上耗费了过高的时间。例如，选择查看CPU的耗费时间  ：

![1552489671119](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552489671119.png)

| 字段       | 含义                           |
| ---------- | ------------------------------ |
| Status     | sql 语句执行的状态             |
| Duration   | sql 执行过程中每一个步骤的耗时 |
| CPU_user   | 当前用户占有的cpu              |
| CPU_system | 系统占有的cpu                  |

## trace分析优化器执行计划

MySQL5.6提供了对SQL的跟踪trace, 通过trace文件能够进一步了解为什么优化器选择A计划, 而不是选择B计划。

打开trace ， 设置格式为 JSON，并设置trace最大能够使用的内存大小，避免解析过程中因为默认内存过小而不能够完整展示。

```sql
SET optimizer_trace="enabled=on",end_markers_in_json=on;
set optimizer_trace_max_mem_size=1000000;
```

执行SQL语句 ：

```sql
select * from tb_item where id < 4;
```

最后， 检查 information_schema.optimizer_trace 就可以知道MySQL是如何执行SQL的 ：

```sql
select * from information_schema.optimizer_trace\G;
```

```json
*************************** 1. row ***************************
QUERY: select * from tb_item where id < 4
TRACE: {
  "steps": [
    {
      "join_preparation": {
        "select#": 1,
        "steps": [
          {
            "expanded_query": "/* select#1 */ select `tb_item`.`id` AS `id`,`tb_item`.`title` AS `title`,`tb_item`.`price` AS `price`,`tb_item`.`num` AS `num`,`tb_item`.`categoryid` AS `categoryid`,`tb_item`.`status` AS `status`,`tb_item`.`sellerid` AS `sellerid`,`tb_item`.`createtime` AS `createtime`,`tb_item`.`updatetime` AS `updatetime` from `tb_item` where (`tb_item`.`id` < 4)"
          }
        ] /* steps */
      } /* join_preparation */
    },
    {
      "join_optimization": {
        "select#": 1,
        "steps": [
          {
            "condition_processing": {
              "condition": "WHERE",
              "original_condition": "(`tb_item`.`id` < 4)",
              "steps": [
                {
                  "transformation": "equality_propagation",
                  "resulting_condition": "(`tb_item`.`id` < 4)"
                },
                {
                  "transformation": "constant_propagation",
                  "resulting_condition": "(`tb_item`.`id` < 4)"
                },
                {
                  "transformation": "trivial_condition_removal",
                  "resulting_condition": "(`tb_item`.`id` < 4)"
                }
              ] /* steps */
            } /* condition_processing */
          },
          {
            "table_dependencies": [
              {
                "table": "`tb_item`",
                "row_may_be_null": false,
                "map_bit": 0,
                "depends_on_map_bits": [
                ] /* depends_on_map_bits */
              }
            ] /* table_dependencies */
          },
          {
            "ref_optimizer_key_uses": [
            ] /* ref_optimizer_key_uses */
          },
          {
            "rows_estimation": [
              {
                "table": "`tb_item`",
                "range_analysis": {
                  "table_scan": {
                    "rows": 9816098,
                    "cost": 2.04e6
                  } /* table_scan */,
                  "potential_range_indices": [
                    {
                      "index": "PRIMARY",
                      "usable": true,
                      "key_parts": [
                        "id"
                      ] /* key_parts */
                    }
                  ] /* potential_range_indices */,
                  "setup_range_conditions": [
                  ] /* setup_range_conditions */,
                  "group_index_range": {
                    "chosen": false,
                    "cause": "not_group_by_or_distinct"
                  } /* group_index_range */,
                  "analyzing_range_alternatives": {
                    "range_scan_alternatives": [
                      {
                        "index": "PRIMARY",
                        "ranges": [
                          "id < 4"
                        ] /* ranges */,
                        "index_dives_for_eq_ranges": true,
                        "rowid_ordered": true,
                        "using_mrr": false,
                        "index_only": false,
                        "rows": 3,
                        "cost": 1.6154,
                        "chosen": true
                      }
                    ] /* range_scan_alternatives */,
                    "analyzing_roworder_intersect": {
                      "usable": false,
                      "cause": "too_few_roworder_scans"
                    } /* analyzing_roworder_intersect */
                  } /* analyzing_range_alternatives */,
                  "chosen_range_access_summary": {
                    "range_access_plan": {
                      "type": "range_scan",
                      "index": "PRIMARY",
                      "rows": 3,
                      "ranges": [
                        "id < 4"
                      ] /* ranges */
                    } /* range_access_plan */,
                    "rows_for_plan": 3,
                    "cost_for_plan": 1.6154,
                    "chosen": true
                  } /* chosen_range_access_summary */
                } /* range_analysis */
              }
            ] /* rows_estimation */
          },
          {
            "considered_execution_plans": [
              {
                "plan_prefix": [
                ] /* plan_prefix */,
                "table": "`tb_item`",
                "best_access_path": {
                  "considered_access_paths": [
                    {
                      "access_type": "range",
                      "rows": 3,
                      "cost": 2.2154,
                      "chosen": true
                    }
                  ] /* considered_access_paths */
                } /* best_access_path */,
                "cost_for_plan": 2.2154,
                "rows_for_plan": 3,
                "chosen": true
              }
            ] /* considered_execution_plans */
          },
          {
            "attaching_conditions_to_tables": {
              "original_condition": "(`tb_item`.`id` < 4)",
              "attached_conditions_computation": [
              ] /* attached_conditions_computation */,
              "attached_conditions_summary": [
                {
                  "table": "`tb_item`",
                  "attached": "(`tb_item`.`id` < 4)"
                }
              ] /* attached_conditions_summary */
            } /* attaching_conditions_to_tables */
          },
          {
            "refine_plan": [
              {
                "table": "`tb_item`",
                "access_type": "range"
              }
            ] /* refine_plan */
          }
        ] /* steps */
      } /* join_optimization */
    },
    {
      "join_execution": {
        "select#": 1,
        "steps": [
        ] /* steps */
      } /* join_execution */
    }
  ] /* steps */
}
```

# 索引的使用



索引是数据库优化最常用也是最重要的手段之一, 通过索引通常可以帮助用户解决大多数的MySQL的性能优化问题。



## 验证索引提升查询效率

在我们准备的表结构 tb_item 中， 一共存储了 300 万记录；

1). 根据ID查询 

```sql
select * from tb_item where id = 1999\G;
```

![1553261992653](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553261992653.png) 

查询速度很快， 接近0s ， 主要的原因是因为id为主键， 有索引；

![1553262044466](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553262044466.png) 



2). 根据 title 进行精确查询

```sql
select * from tb_item where title = 'iphoneX 移动3G 32G941'\G; 
```

![1553262215900](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553262215900.png) 

查看SQL语句的执行计划 ： 

![1553262469785](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553262469785.png) 



处理方案 ， 针对title字段， 创建索引 ： 

```sql
create index idx_item_title on tb_item(title);
```

![1553263229523](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553263229523.png) 



索引创建完成之后，再次进行查询 ： 

![1553263302706](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553263302706.png) 

通过 explain ， 查看执行计划，执行SQL时使用了刚才创建的索引 

![1553263355262](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553263355262.png) 



## 准备环境

```sql
create table `tb_seller` (
	`sellerid` varchar (100),
	`name` varchar (100),
	`nickname` varchar (50),
	`password` varchar (60),
	`status` varchar (1),
	`address` varchar (100),
	`createtime` datetime,
    primary key(`sellerid`)
)engine=innodb default charset=utf8mb4; 

insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('alibaba','阿里巴巴','阿里小店','e10adc3949ba59abbe56e057f20f883e','1','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('baidu','百度科技有限公司','百度小店','e10adc3949ba59abbe56e057f20f883e','1','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('huawei','华为科技有限公司','华为小店','e10adc3949ba59abbe56e057f20f883e','0','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('itcast','传智播客教育科技有限公司','传智播客','e10adc3949ba59abbe56e057f20f883e','1','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('itheima','黑马程序员','黑马程序员','e10adc3949ba59abbe56e057f20f883e','0','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('luoji','罗技科技有限公司','罗技小店','e10adc3949ba59abbe56e057f20f883e','1','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('oppo','OPPO科技有限公司','OPPO官方旗舰店','e10adc3949ba59abbe56e057f20f883e','0','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('ourpalm','掌趣科技股份有限公司','掌趣小店','e10adc3949ba59abbe56e057f20f883e','1','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('qiandu','千度科技','千度小店','e10adc3949ba59abbe56e057f20f883e','2','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('sina','新浪科技有限公司','新浪官方旗舰店','e10adc3949ba59abbe56e057f20f883e','1','北京市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('xiaomi','小米科技','小米官方旗舰店','e10adc3949ba59abbe56e057f20f883e','1','西安市','2088-01-01 12:00:00');
insert into `tb_seller` (`sellerid`, `name`, `nickname`, `password`, `status`, `address`, `createtime`) values('yijia','宜家家居','宜家家居旗舰店','e10adc3949ba59abbe56e057f20f883e','1','北京市','2088-01-01 12:00:00');


create index idx_seller_name_sta_addr on tb_seller(name,status,address);
```

## 避免索引失效

**1).  全值匹配 ，对索引中所有列都指定具体值。**

该情况下，索引生效，执行效率高。

```sql
explain select * from tb_seller where name='小米科技' and status='1' and address='北京市'\G;
```

![1556170997921](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556170997921.png) 

**2). 最左前缀法则**

如果索引了多列（复合索引），要遵守最左前缀法则。指的是查询从索引的最左前列开始，并且不跳过索引中的列。



匹配最左前缀法则，走索引：

![1556171348995](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556171348995.png)  

违法最左前缀法则 ， 索引失效：

![1556171428140](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556171428140.png) 

如果符合最左法则，但是出现跳跃某一列，只有最左列索引生效：

![1556171662203](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556171662203.png) 



**3). 范围查询，不能使用索引 。**

![1556172256791](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556172256791.png) 

根据前面的两个字段name ， status 查询是走索引的， 但是最后一个条件address 没有用到索引。



**4). 不要在索引列上进行运算操作，否则索引将失效。**

![1556172813715](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556172813715.png) 

**5). 字符串不加单引号，造成索引失效。**

![1556172967493](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556172967493.png) 

在查询时，没有对字符串加单引号，MySQL的查询优化器，会自动的进行类型转换，造成索引失效。

**6). 尽量使用覆盖索引，避免select **

尽量使用覆盖索引（只访问索引的查询（索引列完全包含查询列）），减少select * 。

![1556173928299](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556173928299.png) 

如果查询列，超出索引列，也会降低性能。

![1556173986068](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556173986068.png) 

**Extra：**

- using index

  使用覆盖索引的时候就会出现

- using where

  在查找使用索引的情况下，需要回表去查询所需的数据

- using index condition

  查找使用了索引，但是需要回表查询数据

- using index ; using where

  查找使用了索引，但是需要的数据都在索引列中能找到，所以不需要回表查询数据



**7). 用or分割开的条件， 如果or前的条件中的列有索引，而后面的列中没有索引，那么涉及的索引都不会被用到。**

示例，name字段是索引列 ， 而createtime不是索引列，中间是or进行连接是不走索引的 ： 

```sql
explain select * from tb_seller where name='黑马程序员' or createtime = '2088-01-01 12:00:00'\G;	
```

![1556174994440](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556174994440.png) 



**8).  以%开头的Like模糊查询，索引失效。**

如果仅仅是尾部模糊匹配，索引不会失效。如果是头部模糊匹配，索引失效。

```sql
explain select * from tb_seller where name like "%黑马程序员";
```

![1556175114369](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556175114369.png) 

解决方案 ： 

通过覆盖索引来解决 (不用 select *)

![1556247686483](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556247686483.png) 

**9). 如果MySQL评估使用索引比全表更慢，则不使用索引。**

我们先给 address 创建索引

```sql
create index idx_seller_address on tb_seller(address);
```

在我们表 tb_seller 中，12条地区数据其中11个是北京市

查北京地区的走全表扫描

![1556175445210](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556175445210.png) 



使用覆盖查询会走索引

```sql
 explain select address  from tb_seller where address='北京市';
```

**10). is  NULL ， is NOT NULL  <font color='red'>有时</font>索引失效。**

和上一条（9）差不多。

![1556180634889](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556180634889.png)  

**11). in 走索引， not in 索引失效。**

在mysql 5.6中

![1556249602732](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556249602732.png)  



个人理解：not in 判断不存在的，需要对表进行大部分数据扫描，类似于第九条



mysql 5.7中都不失效：

![image-20210523131109106](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210523131109106.png)

**12). 单列索引和复合索引。**

尽量使用复合索引，而少使用单列索引 。

创建复合索引 

```sql
create index idx_name_sta_address on tb_seller(name, status, address);

--就相当于创建了三个索引 ： 
--	name
--	name + status
--	name + status + address
```



创建单列索引 

```sql
create index idx_seller_name on tb_seller(name);
create index idx_seller_status on tb_seller(status);
create index idx_seller_address on tb_seller(address);
```

数据库会选择一个最优的索引（辨识度最高索引）来使用，并不会使用全部索引 。

## 查看索引使用情况

```sql
show status like 'Handler_read%';	--当前会话级别

show global status like 'Handler_read%';	--全局级别
```

![1552885364563](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1552885364563.png)

- Handler_read_first

  索引中第一条被读的次数。如果较高，表示服务器正执行大量全索引扫描（这个值越低越好）。

- Handler_read_key

  如果索引正在工作，这个值代表一个行被索引值读的次数，如果值越低，表示索引得到的性能改善不高，因为索引不经常使用（这个值越高越好）。

- Handler_read_next

  按照键顺序读下一行的请求数。如果你用范围约束或如果执行索引扫描来查询索引列，该值增加。

- Handler_read_prev

  按照键顺序读前一行的请求数。该读方法主要用于优化ORDER BY ... DESC。

- Handler_read_rnd

  根据固定位置读一行的请求数。如果你正执行大量查询并需要对结果进行排序该值较高。你可能使用了大量需要MySQL扫描整个表的查询或你的连接没有正确使用键。这个值较高，意味着运行效率低，应该建立索引来补救。

- Handler_read_rnd_next

  在数据文件中读下一行的请求数。如果你正进行大量的表扫描，该值较高。通常说明你的表索引不正确或写入的查询没有利用索引。

  

## 练习

假设 index(a,b,c)；

| Where 语句                                              | 索引是否被使用                             |
| ------------------------------------------------------- | ------------------------------------------ |
| where a = 3                                             | Y,使用到 a                                 |
| where a = 3 and b = 5                                   | Y,使用到 a，b                              |
| where a = 3 and b = 5 and c = 4                         | Y,使用到 a,b,c                             |
| where b = 3 或者 where b = 3 and c = 4 或者 where c = 4 | N（第二条，左前缀法则）                    |
| where a = 3 and c = 5                                   | 使用到 a， 但是 c 不可以，b 中间断了       |
| where a = 3 and b > 4 and c = 5                         | 使用到 a 和 b， c 不能用在范围之后，b 断了 |
| where a is null and b is not null                       | is null 支持索引 但是 is not null 不支持   |
| where a <> 3                                            | 不能使用索引                               |
| where abs(a) =3                                         | 不能使用索引                               |
| where a = 3 and b like 'kk%' and c = 4                  | Y,使用到 a,b,c                             |
| where a = 3 and b like '%kk' and c = 4                  | Y,只用到 a                                 |
| where a = 3 and b like '%kk%' and c = 4                 | Y,只用到 a                                 |
| where a = 3 and b like 'k%kk%' and c = 4                | Y,使用到 a,b,c                             |

# sql优化

## 大批量插入数据时

环境准备：

```sql
CREATE TABLE `tb_user_2` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `username` varchar(45) NOT NULL,
  `password` varchar(96) NOT NULL,
  `name` varchar(45) NOT NULL,
  `birthday` datetime DEFAULT NULL,
  `sex` char(1) DEFAULT NULL,
  `email` varchar(45) DEFAULT NULL,
  `phone` varchar(45) DEFAULT NULL,
  `qq` varchar(32) DEFAULT NULL,
  `status` varchar(32) NOT NULL COMMENT '用户状态',
  `create_time` datetime NOT NULL,
  `update_time` datetime DEFAULT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `unique_user_username` (`username`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8 ;
```

当使用 `load` 命令导入数据的时候，适当的设置可以提高导入的效率。

![1556269346488](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556269346488.png) 

对于 InnoDB 类型的表，有以下几种方式可以提高导入的效率：

**1） 主键顺序插入**

因为InnoDB类型的表是按照主键的顺序保存的，所以将导入的数据按照主键的顺序排列，可以有效的提高导入数据的效率。如果InnoDB表没有主键，那么系统会自动默认创建一个内部列作为主键，所以如果可以给表创建一个主键，将可以利用这点，来提高导入数据的效率。

> 脚本文件介绍 :
>
> ​	sql1.log  ----> 主键有序
>
> ​	sql2.log  ----> 主键无序



插入ID顺序排列数据：

![1555771750567](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555771750567.png)

插入ID无序排列数据：

![1555771959734](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555771959734.png) 



**2） 关闭唯一性校验**

在导入数据前执行 SET UNIQUE_CHECKS=0，关闭唯一性校验

在导入结束后执行SET UNIQUE_CHECKS=1，恢复唯一性校验，可以提高导入的效率。

![1555772132736](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555772132736.png) 



**3） 手动提交事务**

建议在导入前执行 SET AUTOCOMMIT=0，关闭自动提交

导入结束后再执行 SET AUTOCOMMIT=1，打开自动提交，也可以提高导入的效率。

![1555772351208](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555772351208.png)



> <mark> load执行可能会报错</mark>

The used command is not allowed with this MySQL version

错误的原因是没有开启 local_infile 模块。

**解决方法：**

首先看一下 local_infile 模块是否打开：

```msyql
show global variables like 'local_infile';
```

显示如下：

![image](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/20190406131719389.png)

然后可以发现这个模块已经启用了：

![image](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/20190406131859826.png)



之后重启一下Mysql服务即可

## 优化insert语句



1.）如果需要同时对一张表插入很多行数据时，应该尽量使用多个值表的insert语句，这种方式将大大的缩减客户端与数据库之间的连接、关闭等消耗。使得效率比分开执行的单个insert语句快。

-  原始方式为：

  ```sql
  insert into tb_test values(1,'Tom');
  insert into tb_test values(2,'Cat');
  insert into tb_test values(3,'Jerry');
  ```

  优化后的方案为 ： 

  ```sql
  insert into tb_test values(1,'Tom'),(2,'Cat')，(3,'Jerry');
  ```


2.）在事务中进行数据插入。

```sql
start transaction;
insert into tb_test values(1,'Tom');
insert into tb_test values(2,'Cat');
insert into tb_test values(3,'Jerry');
commit;
```

3.）数据有序插入

- 原

  ```sql
  insert into tb_test values(4,'Tim');
  insert into tb_test values(1,'Tom');
  insert into tb_test values(3,'Jerry');
  insert into tb_test values(5,'Rose');
  insert into tb_test values(2,'Cat');
  ```

- 优化后

  ```sql
  insert into tb_test values(1,'Tom');
  insert into tb_test values(2,'Cat');
  insert into tb_test values(3,'Jerry');
  insert into tb_test values(4,'Tim');
  insert into tb_test values(5,'Rose');
  ```



## 优化order by语句

### 环境准备

```SQL
CREATE TABLE `emp` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(100) NOT NULL,
  `age` int(3) NOT NULL,
  `salary` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=utf8mb4;

insert into `emp` (`id`, `name`, `age`, `salary`) values('1','Tom','25','2300');
insert into `emp` (`id`, `name`, `age`, `salary`) values('2','Jerry','30','3500');
insert into `emp` (`id`, `name`, `age`, `salary`) values('3','Luci','25','2800');
insert into `emp` (`id`, `name`, `age`, `salary`) values('4','Jay','36','3500');
insert into `emp` (`id`, `name`, `age`, `salary`) values('5','Tom2','21','2200');
insert into `emp` (`id`, `name`, `age`, `salary`) values('6','Jerry2','31','3300');
insert into `emp` (`id`, `name`, `age`, `salary`) values('7','Luci2','26','2700');
insert into `emp` (`id`, `name`, `age`, `salary`) values('8','Jay2','33','3500');
insert into `emp` (`id`, `name`, `age`, `salary`) values('9','Tom3','23','2400');
insert into `emp` (`id`, `name`, `age`, `salary`) values('10','Jerry3','32','3100');
insert into `emp` (`id`, `name`, `age`, `salary`) values('11','Luci3','26','2900');
insert into `emp` (`id`, `name`, `age`, `salary`) values('12','Jay3','37','4500');

create index idx_emp_age_salary on emp(age,salary);
```

### 两种排序方式

1). 第一种是通过对返回数据进行排序，也就是通常说的 filesort 排序

不是通过索引直接返回排序结果的排序都叫 FileSort 排序。

![1556335817763](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556335817763.png) 

2). 第二种通过有序索引顺序扫描直接返回有序数据，这种情况即为 using index，不需要额外排序，操作效率高。

![1556335866539](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556335866539.png) 

多字段排序

![1556336352061](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556336352061.png) 



了解了MySQL的排序方式，优化目标就清晰了：尽量减少额外的排序，通过索引直接返回有序数据。where 条件和Order by 使用相同的索引，并且Order By 的顺序和索引顺序相同， 并且Order  by 的字段都是升序，或者都是降序。否则肯定需要额外的操作，这样就会出现 FileSort。



### Filesort 的优化

通过创建合适的索引，能够减少 Filesort 的出现，但是在某些情况下，条件限制不能让 Filesort 消失，那就需要加快 Filesort的排序操作。对于Filesort ，MySQL 有两种排序算法：

1） 两次扫描算法 ：MySQL4.1 之前，使用该方式排序。首先根据条件取出排序字段和行指针信息，然后在排序区 sort buffer 中排序，如果sort buffer不够，则在临时表 temporary table 中存储排序结果。完成排序之后，再根据行指针回表读取记录，该操作可能会导致大量随机I/O操作。

2）一次扫描算法：一次性取出满足条件的所有字段，然后在排序区 sort  buffer 中排序后直接输出结果集。排序时内存开销较大，但是排序效率比两次扫描算法要高。



MySQL 通过比较系统变量 max_length_for_sort_data 的大小和 Query 语句取出的字段总大小， 来判定是否那种排序算法，如果 max_length_for_sort_data 更大，那么使用第二种优化之后的算法；否则使用第一种。

可以适当提高 sort_buffer_size  和 max_length_for_sort_data  系统变量，来增大排序区的大小，提高排序的效率。

![1556338367593](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556338367593.png) 



## 优化group by 语句

由于 GROUP BY 实际上也同样会进行排序操作，而且与 ORDER BY 相比，GROUP BY 主要只是多了排序之后的分组操作。当然，如果在分组的时候还使用了其他的一些聚合函数，那么还需要一些聚合函数的计算。所以，在GROUP BY 的实现过程中，与 ORDER BY 一样也可以利用到索引。

如果查询包含 group by 但是想要避免排序结果的消耗， 则可以执行order by null 禁止排序。如下 ：

```sql
drop index idx_emp_age_salary on emp; -- 删除之前创建的索引

explain select age,count(*) from emp group by age;
```

![1556339573979](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556339573979.png)  

优化后

```sql
explain select age,count(*) from emp group by age order by null;
```

![1556339633161](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556339633161.png)  

从上面的例子可以看出，第一个SQL语句需要进行"filesort"，而第二个SQL由于 `order  by  null` 不需要进行 "filesort"， 而上文提过 Filesort 往往非常耗费时间。



创建索引 ：

```SQL
create index idx_emp_age_salary on emp(age,salary);
```

![1556339688158](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556339688158.png) 



**但是在 mysql 5.7 中：**

![image-20210523150730770](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210523150730770.png)



## 优化嵌套查询

Mysql4.1版本之后，开始支持SQL的子查询。这个技术可以使用SELECT语句来创建一个单列的查询结果，然后把这个结果作为过滤条件用在另一个查询中。使用子查询可以一次性的完成很多逻辑上需要多个步骤才能完成的SQL操作，同时也可以避免事务或者表锁死，并且写起来也很容易。但是，有些情况下，子查询是可以被更高效的连接（JOIN）替代。

示例 ，查找有角色的所有的用户信息 : 

```SQL
 explain select * from t_user where id in (select user_id from user_role );
```

执行计划为 : 

![1556359399199](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556359399199.png)   

优化后 :

```SQL
explain select * from t_user u , user_role ur where u.id = ur.user_id;
```

![1556359482142](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556359482142.png)   

连接(Join)查询之所以更有效率一些 ，是因为MySQL不需要在内存中创建临时表来完成这个逻辑上需要两个步骤的查询工作。

在 mysql 5.7 中

![image-20210523151026166](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/image-20210523151026166.png)



## 优化OR条件

对于包含OR的查询子句，如果要利用索引，则OR之间的每个条件列都必须用到索引 ， 而且不能使用到复合索引； 如果没有索引，则应该考虑增加索引。

获取 emp 表中的所有的索引 ： 

![1556354464657](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556354464657.png)  

示例 ： 

```SQL
explain select * from emp where id = 1 or age = 30;
```

![1556354887509](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556354887509.png)

![1556354920964](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556354920964.png)  

建议使用 union 替换 or ： 

![1556355027728](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556355027728.png) 

我们来比较下重要指标，发现主要差别是 type 和 ref 这两项

type 显示的是访问类型，是较为重要的一个指标，结果值从好到坏依次是：

```
system > const > eq_ref > ref > fulltext > ref_or_null  > index_merge > unique_subquery > index_subquery > range > index > ALL
```

UNION 语句的 type 值为 ref，OR 语句的 type 值为 range，可以看到这是一个很明显的差距

UNION 语句的 ref 值为 const，OR 语句的 type 值为 null，const 表示是常量值引用，非常快

这两项的差距就说明了 UNION 要优于 OR 。

<mark>在 mysql 8.0 中，默认优化了，具体自行测试。</mark>



## 优化分页查询

一般分页查询时，通过创建覆盖索引能够比较好地提高性能。一个常见又非常头疼的问题就是 limit 2000000,10  ，此时需要MySQL排序前2000010 记录，仅仅返回2000000 - 2000010 的记录，其他记录丢弃，查询排序的代价非常大 。

![1556361314783](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556361314783.png) 

**优化思路一**

在索引上完成排序分页操作，最后根据主键关联回原表查询所需要的其他列内容。

![1556416102800](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556416102800.png) 



**优化思路二**

该方案适用于主键自增的表，可以把Limit 查询转换成某个位置的查询 。

![1556363928151](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556363928151.png) 



## 使用SQL提示

SQL提示，是优化数据库的一个重要手段，简单来说，就是在SQL语句中加入一些人为的提示来达到优化操作的目的。



**USE INDEX**

在查询语句中表名的后面，添加 use index 来提供希望MySQL去参考的索引列表，就可以让MySQL不再考虑其他可用的索引。

```
create index idx_seller_name on tb_seller(name);
```

![1556370971576](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556370971576.png) 



**IGNORE INDEX**

如果用户只是单纯的想让MySQL忽略一个或者多个索引，则可以使用 ignore index 作为 hint 。

```
 explain select * from tb_seller ignore index(idx_seller_name) where name = '小米科技';
```

![1556371004594](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556371004594.png) 



**FORCE INDEX**

为强制MySQL使用一个特定的索引，可在查询中使用 force index 作为hint 。 

``` SQL
create index idx_seller_address on tb_seller(address);
```

![1556371355788](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556371355788.png) 


# 缓存查询概述

开启Mysql的查询缓存，当执行完全相同的SQL语句的时候，服务器就会直接从缓存中读取结果，当数据被修改，之前的缓存会失效，修改比较频繁的表不适合做查询缓存。



 ![20180919131632347](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/20180919131632347.png) 

1. 客户端发送一条查询给服务器；
2. 服务器先会检查查询缓存，如果命中了缓存，则立即返回存储在缓存中的结果。否则进入下一阶段；
3. 服务器端进行SQL解析、预处理，再由优化器生成对应的执行计划；
4. MySQL根据优化器生成的执行计划，调用存储引擎的API来执行查询；
5. 将结果返回给客户端。

## 查询缓存配置

- 查看当前的MySQL数据库是否支持查询缓存：

```SQL
SHOW VARIABLES LIKE 'have_query_cache';	
```

![1555249929012](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555249929012.png)

<font color='red'>在Mysql8，已经取消了查询缓存</font>



- 查看当前MySQL是否开启了查询缓存 ：

```SQL
SHOW VARIABLES LIKE 'query_cache_type'; 
```

![1555250015377](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555250015377.png)

- 查看查询缓存的占用大小 ：

```SQL
SHOW VARIABLES LIKE 'query_cache_size';
```

![1555250142451](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555250142451.png)  	

- 查看查询缓存的状态变量：

```SQL
SHOW STATUS LIKE 'Qcache%';
```

![1555250443958](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555250443958.png) 

各个变量的含义如下：

| 参数                    | 含义                                                         |
| ----------------------- | ------------------------------------------------------------ |
| Qcache_free_blocks      | 查询缓存中的可用内存块数                                     |
| Qcache_free_memory      | 查询缓存的可用内存量                                         |
| Qcache_hits             | 查询缓存命中数                                               |
| Qcache_inserts          | 添加到查询缓存的查询数                                       |
| Qcache_lowmen_prunes    | 由于内存不足而从查询缓存中删除的查询数                       |
| Qcache_not_cached       | 非缓存查询的数量（由于 query_cache_type 设置而无法缓存或未缓存） |
| Qcache_queries_in_cache | 查询缓存中注册的查询数                                       |
| Qcache_total_blocks     | 查询缓存中的块总数                                           |



## 开启查询缓存

MySQL的查询缓存默认是关闭的，需要手动配置参数 query_cache_type ， 来开启查询缓存。

query_cache_type 该参数的可取值有三个 ：

| 值          | 含义                                                         |
| ----------- | ------------------------------------------------------------ |
| OFF 或 0    | 查询缓存功能关闭                                             |
| ON 或 1     | 查询缓存功能打开，SELECT的结果符合缓存条件即会缓存，否则，不予缓存，显式指定 SQL_NO_CACHE，不予缓存 |
| DEMAND 或 2 | 查询缓存功能按需进行，显式指定 SQL_CACHE 的SELECT语句才会缓存；其它均不予缓存 |

在 `/usr/my.cnf` 配置中（宝塔在 `/etc/my.cnf` ），增加以下配置 ： 

```properties
# 开启mysql的查询缓存
query_cache_type=1
```

配置完毕之后，重启服务既可生效 , `service mysqld restart `；

然后就可以在命令行执行SQL语句进行验证 ，执行一条比较耗时的SQL语句，然后再多执行几次，查看后面几次的执行时间；获取通过查看查询缓存的缓存命中数，来判定是否走查询缓存。

## 查询缓存SELECT选项

可以在 SELECT 语句中指定两个与查询缓存相关的选项 ：

- SQL_CACHE

  如果查询结果是可缓存的，并且 query_cache_type 系统变量的值为 ON 或 DEMAND ，则缓存查询结果 。

- SQL_NO_CACHE

  服务器不使用查询缓存。它既不检查查询缓存，也不检查结果是否已缓存，也不缓存查询结果。

例子：

```SQL
SELECT SQL_CACHE id, name FROM customer;
SELECT SQL_NO_CACHE id, name FROM customer;
```

​	

## 查询缓存失效的情况

1） SQL 语句不一致的情况， 要想命中查询缓存，查询的SQL语句必须一致。

```SQL
-- SQL1 : 
select count(*) from tb_item;
-- SQL2 : 
Select count(*) from tb_item;
```

2） 当查询语句中有一些不确定的时，则不会缓存。如 ： now() , current_date() , curdate() , curtime() , rand() , uuid() , user() , database() 。

```SQL
select * from tb_item where updatetime < now() limit 1;
select user();
select database();
```

3） 不使用任何表查询语句。

```SQL
select 'A';
```

4）  查询 mysql， information_schema或  performance_schema 系统数据库中的表时，不会走查询缓存。

```SQL
select * from information_schema.engines;
```

5） 在存储的函数，触发器或事件的主体内执行的查询。

6） 如果表更改，则使用该表的所有高速缓存查询都将变为无效并从高速缓存中删除。这包括使用`MERGE`映射到已更改表的表的查询。一个表可以被许多类型的语句，如被改变 INSERT， UPDATE， DELETE， TRUNCATE TABLE， ALTER TABLE， DROP TABLE，或 DROP DATABASE 。

# Mysql内存管理及优化

## 内存优化原则

1） 将尽量多的内存分配给MySQL做缓存，但要给操作系统和其他程序预留足够内存。

2） MyISAM 存储引擎的数据文件读取依赖于操作系统自身的IO缓存，因此，如果有MyISAM表，就要预留更多的内存给操作系统做IO缓存。

3） 排序区、连接区等缓存是分配给每个数据库会话（session）专用的，其默认值的设置要根据最大连接数合理分配，如果设置太大，不但浪费资源，而且在并发连接较高时会导致物理内存耗尽。



## MyISAM 内存优化

了解即可，我们平时用的都是 InnoDB



myisam存储引擎使用 key_buffer 缓存索引块，加速myisam索引的读写速度。对于myisam表的数据块，mysql没有特别的缓存机制，完全依赖于操作系统的IO缓存。



- key_buffer_size

key_buffer_size决定MyISAM索引块缓存区的大小，直接影响到MyISAM表的存取效率。可以在MySQL参数文件中设置key_buffer_size的值，对于一般MyISAM数据库，建议至少将1/4可用内存分配给key_buffer_size。

在 `/usr/my.cnf` 中做如下配置：

```properties
key_buffer_size=512M
```

```sql
SHOW VARIABLES LIKE 'key_buffer_size' -- 查看大小
```

- read_buffer_size

如果需要经常顺序扫描myisam表，可以通过增大read_buffer_size的值来改善性能。但需要注意的是read_buffer_size是每个session独占的，如果默认值设置太大，就会造成内存浪费。



- read_rnd_buffer_size

对于需要做排序的myisam表的查询，如带有order by子句的sql，适当增加 read_rnd_buffer_size 的值，可以改善此类的sql性能。但需要注意的是 read_rnd_buffer_size 是每个session独占的，如果默认值设置太大，就会造成内存浪费。



## InnoDB 内存优化

innodb用一块内存区做IO缓存池，该缓存池不仅用来缓存innodb的索引块，而且也用来缓存innodb的数据块。



- innodb_buffer_pool_size

该变量决定了 innodb 存储引擎表数据和索引数据的最大缓存区大小。在保证操作系统及其他程序有足够内存可用的情况下，innodb_buffer_pool_size 的值越大，缓存命中率越高，访问InnoDB表需要的磁盘I/O 就越少，性能也就越高。

```properties
innodb_buffer_pool_size=512M
```



- innodb_log_buffer_size

决定了 Innodb 重做日志缓存的大小，对于可能产生大量更新记录的大事务，增加innodb_log_buffer_size的大小，可以避免innodb在事务提交前就执行不必要的日志写入磁盘操作。

```properties
innodb_log_buffer_size=10M
```

# 并发参数
## max_connections

采用max_connections 控制允许连接到MySQL数据库的最大数量，默认值是 151。如果状态变量 connection_errors_max_connections 不为零，并且一直增长，则说明不断有连接请求因数据库连接数已达到允许最大值而失败，这是可以考虑增大max_connections 的值。

Mysql 最大可支持的连接数，取决于很多因素，包括给定操作系统平台的线程库的质量、内存大小、每个连接的负荷、CPU的处理速度，期望的响应时间等。在Linux 平台下，性能好的服务器，支持 500-1000 个连接不是难事，需要根据服务器性能进行评估设定。



## back_log

back_log 参数控制MySQL监听TCP端口时设置的积压请求栈大小。如果MySql的连接数达到 max_connections时，新来的请求将会被存在堆栈中，以等待某一连接释放资源，该堆栈的数量即 back_log，如果等待连接的数量超过back_log，将不被授予连接资源，将会报错。5.6.6 版本之前默认值为 50 ， 之后的版本默认为 50 + （max_connections / 5）， 但最大不超过900。

如果需要数据库在较短的时间内处理大量连接请求， 可以考虑适当增大 back_log 的值。



## table_open_cache

该参数用来控制所有SQL语句执行线程可打开表缓存的数量， 而在执行SQL语句时，每一个SQL执行线程至少要打开 1 个表缓存。该参数的值应该根据设置的最大连接数 max_connections 以及每个连接执行关联查询中涉及的表的最大数量来设定 ：max_connections x N ；

```sql
SHOW VARIABLES LIKE 'table_open_cache' -- 查看大小
```



## thread_cache_size

为了加快连接数据库的速度，MySQL 会缓存一定数量的客户服务线程以备重用，通过参数 thread_cache_size 可控制 MySQL 缓存客户服务线程的数量。



## innodb_lock_wait_timeout

该参数是用来设置InnoDB 事务等待行锁的时间，默认值是50ms ， 可以根据需要进行动态设置。对于需要快速反馈的业务系统来说，可以将行锁的等待时间调小，以避免事务长时间挂起； 对于后台运行的批量处理程序来说， 可以将行锁的等待时间调大， 以避免发生大的回滚操作。

# 锁问题
## 简介

- **锁概述**

锁是计算机协调多个进程或线程并发访问某一资源的机制（避免争抢）。

在数据库中，除传统的计算资源（如 CPU、RAM、I/O 等）的争用以外，数据也是一种供许多用户共享的资源。如何保证数据并发访问的一致性、有效性是所有数据库必须解决的一个问题，锁冲突也是影响数据库并发访问性能的一个重要因素。从这个角度来说，锁对数据库而言显得尤其重要，也更加复杂。



- **锁分类：**

从对数据操作的粒度分 ： 

1） 表锁：操作时，会锁定整个表。

2） 行锁：操作时，会锁定当前操作行。

从对数据操作的类型分：

1） 读锁（共享锁）：针对同一份数据，多个读操作可以同时进行而不会互相影响。

2） 写锁（排它锁）：当前操作没有完成之前，它会阻断其他写锁和读锁。



- **Mysql 锁**

相对其他数据库而言，MySQL的锁机制比较简单，其最显著的特点是不同的存储引擎支持不同的锁机制。

下表中罗列出了各存储引擎对锁的支持情况：

| 存储引擎 | 表级锁 | 行级锁 | 页面锁 |
| -------- | ------ | ------ | ------ |
| MyISAM   | 支持   | 不支持 | 不支持 |
| InnoDB   | 支持   | 支持   | 不支持 |
| MEMORY   | 支持   | 不支持 | 不支持 |
| BDB      | 支持   | 不支持 | 支持   |

MySQL这3种锁的特性可大致归纳如下 ：

| 锁类型 | 特点                                                         |
| ------ | ------------------------------------------------------------ |
| 表级锁 | 偏向MyISAM 存储引擎，开销小，加锁快；不会出现死锁；锁定粒度大，发生锁冲突的概率最高,并发度最低。 |
| 行级锁 | 偏向InnoDB 存储引擎，开销大，加锁慢；会出现死锁；锁定粒度最小，发生锁冲突的概率最低,并发度也最高。 |
| 页面锁 | 开销和加锁时间界于表锁和行锁之间；会出现死锁；锁定粒度界于表锁和行锁之间，并发度一般。 |

从上述特点可见，很难笼统地说哪种锁更好，只能就具体应用的特点来说哪种锁更合适！仅从锁的角度来说：表级锁更适合于以查询为主，只有少量按索引条件更新数据的应用，如Web 应用；而行级锁则更适合于有大量按索引条件并发更新少量不同数据，同时又有并查询的应用，如一些在线事务处理（OLTP）系统。




## MyISAM 表锁

MyISAM 存储引擎只支持表锁，这也是MySQL开始几个版本中唯一支持的锁类型。



### 如何加表锁

MyISAM 在执行查询语句（SELECT）前，会自动给涉及的所有表加读锁，在执行更新操作（UPDATE、DELETE、INSERT 等）前，会自动给涉及的表加写锁，这个过程并不需要用户干预，因此，用户一般不需要直接用 LOCK TABLE 命令给 MyISAM 表显式加锁。

```SQL
lock table table_name read;	--加读锁

lock table table_name writ;	--加写锁
```



### 读锁案例 

准备环境

```SQL
create database demo_03 default charset=utf8mb4;

use demo_03;

CREATE TABLE `tb_book` (
  `id` INT(11) auto_increment,
  `name` VARCHAR(50) DEFAULT NULL,
  `publish_time` DATE DEFAULT NULL,
  `status` CHAR(1) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=myisam DEFAULT CHARSET=utf8 ;

INSERT INTO tb_book (id, name, publish_time, status) VALUES(NULL,'java编程思想','2088-08-01','1');
INSERT INTO tb_book (id, name, publish_time, status) VALUES(NULL,'solr编程思想','2088-08-08','0');



CREATE TABLE `tb_user` (
  `id` INT(11) auto_increment,
  `name` VARCHAR(50) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=myisam DEFAULT CHARSET=utf8 ;

INSERT INTO tb_user (id, name) VALUES(NULL,'令狐冲');
INSERT INTO tb_user (id, name) VALUES(NULL,'田伯光');

```



客户端 一 ：

1）加 tb_book 表的读锁

```sql
lock table tb_book read;
```



2） 执行查询操作

```sql
select * from tb_book;
```

![1553906896564](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553906896564.png) 

可以正常执行 ， 查询出数据。

客户端 二 ：

3） 执行查询操作

```sql
select * from tb_book;
```

![1553907044500](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553907044500.png) 



客户端 一 ：

4）查询未锁定的表

```sql
select name from tb_seller;
```

![1553908913515](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553908913515.png) 

客户端 二 ：

5）查询未锁定的表

```sql
select name from tb_seller;
```

![1553908973840](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553908973840.png) 

可以正常查询出未锁定的表；



客户端 一 ：

6） 执行插入操作 

```sql
insert into tb_book values(null,'Mysql高级','2088-01-01','1');
```

![1553907198462](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553907198462.png) 

执行插入， 直接报错 ， 由于当前tb_book 获得的是 读锁， 不能执行更新操作。



客户端 二 ：

7） 执行插入操作 

```sql
insert into tb_book values(null,'Mysql高级','2088-01-01','1');
```

![1553907403957](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553907403957.png) 



当在客户端一中释放锁指令 unlock tables  后 ， 客户端二中的 inesrt 语句 ， 立即执行 ；

### 写锁案例

客户端 一 :

1）给 tb_book 表的写锁 

```sql
lock table tb_book write ;
```

2）执行查询操作

```sql
select * from tb_book ;
```

![1553907849829](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553907849829.png) 

查询操作执行成功；

3）执行更新操作

```sql
update tb_book set name = 'java编程思想（第二版）' where id = 1;
```

![1553907875221](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553907875221.png) 

更新操作执行成功 ；



客户端 二 :

4）执行查询操作

```
select * from tb_book ;
```

![1553908019755](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553908019755.png) 



当在客户端一中释放锁指令 unlock tables  后 ， 客户端二中的 select 语句 ， 立即执行 ；

![1553908131373](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553908131373.png) 



### 结论

锁模式的相互兼容性如表中所示：

![1553905621992](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553905621992.png) 

由上表可见： 

​	1） 对MyISAM 表的读操作，不会阻塞其他用户对同一表的读请求，但会阻塞对同一表的写请求；

​	2） 对MyISAM 表的写操作，会都阻塞其他用户对同一表的读和写操作；

​	简而言之，就是读锁会阻塞写，但是不会阻塞读。而写锁，则既会阻塞读，又会阻塞写。



此外，MyISAM 的读写锁调度是写优先，这也是MyISAM不适合做写为主的表的存储引擎的原因。因为写锁后，其他线程不能做任何操作，大量的更新会使查询很难得到锁，从而造成永远阻塞。

### 查看锁的争用情况

``` sql
show open tables；
```

![1556443073322](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556443073322.png) 

In_user : 表当前被查询使用的次数。如果该数为零，则表是打开的，但是当前没有被使用。

Name_locked：表名称是否被锁定。名称锁定用于取消表或对表进行重命名等操作。



```sql
show status like 'Table_locks%';
```

![1556443170082](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556443170082.png) 

Table_locks_immediate ： 指的是能够立即获得表级锁的次数，每立即获取锁，值加1。

Table_locks_waited ： 指的是不能立即获取表级锁而需要等待的次数，每等待一次，该值加1，此值高说明存在着较为严重的表级锁争用情况。

## InnoDB 行锁

### 行锁介绍

行锁特点 ：偏向InnoDB 存储引擎，开销大，加锁慢；会出现死锁；锁定力度最小，发生锁冲突的概率最低，并发度也最高。

InnoDB 与 MyISAM 的最大不同有两点：一是支持事务；二是采用了行级锁。



### 背景知识

**事务及其ACID属性**

事务是由一组SQL语句组成的逻辑处理单元。

事务具有以下4个特性，简称为事务ACID属性。

| ACID属性             | 含义                                                         |
| -------------------- | ------------------------------------------------------------ |
| 原子性（Atomicity）  | 事务是一个原子操作单元，其对数据的修改，要么全部成功，要么全部失败。 |
| 一致性（Consistent） | 在事务开始和完成时，数据都必须保持一致状态。                 |
| 隔离性（Isolation）  | 数据库系统提供一定的隔离机制，保证事务在不受外部并发操作影响的 “独立” 环境下运行。 |
| 持久性（Durable）    | 事务完成之后，对于数据的修改是永久的。                       |



**并发事务处理带来的问题**

| 问题                               | 含义                                                         |
| ---------------------------------- | ------------------------------------------------------------ |
| 丢失更新（Lost Update）            | 当两个或多个事务选择同一行，最初的事务修改的值，会被后面的事务修改的值覆盖。 |
| 脏读（Dirty Reads）                | 当一个事务正在访问数据，并且对数据进行了修改，而这种修改还没有提交到数据库中，这时，另外一个事务也访问这个数据，然后使用了这个数据。 |
| 不可重复读（Non-Repeatable Reads） | 一个事务在读取某些数据后的某个时间，再次读取以前读过的数据，却发现和以前读出的数据不一致。 |
| 幻读（Phantom Reads）              | 一个事务按照相同的查询条件重新读取以前查询过的数据，却发现其他事务插入了满足其查询条件的新数据。 |



**事务隔离级别**

为了解决上述提到的事务并发问题，数据库提供一定的事务隔离机制来解决这个问题。数据库的事务隔离越严格，并发副作用越小，但付出的代价也就越大，因为事务隔离实质上就是使用事务在一定程度上“串行化” 进行，这显然与“并发” 是矛盾的。 

数据库的隔离级别有4个，由低到高依次为 Read uncommitted、Read committed、Repeatable read、Serializable，这四个级别可以逐个解决 脏写、脏读、不可重复读、幻读 这几类问题。

| 隔离级别                | 丢失更新 | 脏读 | 不可重复读 | 幻读 |
| ----------------------- | -------- | ---- | ---------- | ---- |
| Read uncommitted        | ×        | √    | √          | √    |
| Read committed          | ×        | ×    | √          | √    |
| Repeatable read（默认） | ×        | ×    | ×          | √    |
| Serializable            | ×        | ×    | ×          | ×    |

<mark>备注 ： √  代表可能出现 ， × 代表不会出现 。</mark>

Mysql 的数据库的默认隔离级别为 Repeatable read ， 查看方式：

```sql
show variables like 'tx_isolation';
```

![1554331600009](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554331600009.png)  



### InnoDB 的行锁模式

InnoDB  实现了以下两种类型的行锁。

- 共享锁（S）：又称为读锁，简称 `S` 锁，共享锁就是多个事务对于同一数据可以共享一把锁，都能访问到数据，但是只能读不能修改。
- 排他锁（X）：又称为写锁，简称 `X` 锁，排他锁就是不能与其他锁并存，如一个事务获取了一个数据行的排他锁，其他事务就不能再获取该行的其他锁，包括共享锁和排他锁，但是获取排他锁的事务是可以对数据就行读取和修改。

对于 UPDATE、DELETE、INSERT 语句，InnoDB 会自动给涉及数据集加 排他锁（X)

对于普通SELECT语句，InnoDB不会加任何锁；



可以通过以下语句显示给记录集加共享锁或排他锁 。

```sql
-- 共享锁（S）
SELECT * FROM table_name WHERE ... LOCK IN SHARE MODE
-- 排他锁（X)
SELECT * FROM table_name WHERE ... FOR UPDATE
```

### 行锁基本演示

准备 sql

```sql
create table test_innodb_lock(
	id int(11),
	name varchar(16),
	sex varchar(1)
)engine = innodb default charset=utf8;

insert into test_innodb_lock values(1,'100','1');
insert into test_innodb_lock values(3,'3','1');
insert into test_innodb_lock values(4,'400','0');
insert into test_innodb_lock values(5,'500','1');
insert into test_innodb_lock values(6,'600','0');
insert into test_innodb_lock values(7,'700','0');
insert into test_innodb_lock values(8,'800','1');
insert into test_innodb_lock values(9,'900','1');
insert into test_innodb_lock values(1,'200','0');

create index idx_test_innodb_lock_id on test_innodb_lock(id);
create index idx_test_innodb_lock_name on test_innodb_lock(name);
```

开启两个会话

| Session-1                                                    | Session-2                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![1554354615030](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554354615030.png)关闭自动提交功能 | ![1554354601867](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554354601867.png)关闭自动提交功能 |
| ![1554354713628](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554354713628.png)可以正常的查询出全部的数据 | ![1554354717336](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554354717336.png)可以正常的查询出全部的数据 |
| ![1554354830589](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554354830589.png)查询id 为3的数据 ； | ![1554354832708](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554354832708.png)获取id为3的数据 ； |
| ![1554382789984](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554382789984.png)更新id为3的数据，但是不提交； | ![1554382905352](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554382905352.png) 更新id为3 的数据， 出于等待状态 |
| ![1554382977653](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554382977653.png)通过commit， 提交事务 | ![1554383044542](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554383044542.png) 解除阻塞，更新正常进行 |
| 以上， 操作的都是同一行的数据，接下来，演示不同行的数据 ：   |                                                              |
| ![1554385220580](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554385220580.png) 更新id为3数据，正常的获取到行锁 ，执行更新 | ![1554385236768](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554385236768.png) 由于与 Session-1 操作不是同一行，获取当前行锁，执行更新； |

###  无索引行锁升级为表锁

如果不通过索引条件检索数据，那么InnoDB将对表中的所有记录加锁，实际效果跟表锁一样。

```sql
 --查看当前表的索引 ：
 show  index  from test_innodb_lock ;
```

![1554385956215](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554385956215.png) 

| Session-1                                                    | Session-2                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![1554386287454](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554386287454.png)关闭事务的自动提交 | ![1554386312524](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554386312524.png)关闭事务的自动提交 |
| ![1554386654793](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554386654793-1621851044615.png)执行更新语句 | ![1554386685610](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554386685610.png)执行更新语句， 但处于阻塞状态 |
| ![1554386721653](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554386721653.png)提交事务 | ![1554386750004](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554386750004.png)解除阻塞，执行更新成功 |
|                                                              | ![1554386804807](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554386804807.png)执行提交操作 |

由于执行更新时，name字段本来为varchar类型， 我们是作为数字类型使用，存在类型转换，索引失效，最终行锁变为表锁 ；



### 间隙锁危害

当我们用范围条件，而不是使用相等条件检索数据，并请求共享或排他锁时，InnoDB会给符合条件的已有数据进行加锁； 对于键值在条件范围内但并不存在的记录，叫做 "间隙（GAP）" ， InnoDB也会对这个 "间隙" 加锁，这种锁机制就是所谓的 间隙锁（Next-Key锁） 。

示例 ： 

| Session-1                                                    | Session-2                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![1554387987130](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554387987130.png)关闭事务自动提交 ! | ![](https://cdn.jsdelivr.net/gh/oddfar/static/img/20210524221100.png)关闭事务自动提交 |
| ![1554388492478](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554388492478.png)根据id范围更新数据 |                                                              |
|                                                              | ![1554388515936](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554388515936.png)插入id为2的记录， 出于阻塞状态! |
| ![1554388149305](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554388149305.png)提交事务 |                                                              |
|                                                              | ![1554388548562](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554388548562.png)解除阻塞 ， 执行插入操作 |
|                                                              | 提交事务                                                     |



### InnoDB 行锁争用情况

```sql
show  status like 'innodb_row_lock%';
```

![1556455943670](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1556455943670.png)

- Innodb_row_lock_current_waits

  当前正在等待锁定的数量

- Innodb_row_lock_time

  从系统启动到现在锁定总时间长度

- Innodb_row_lock_time_avg

  每次等待所花平均时长

- Innodb_row_lock_time_max

  从系统启动到现在等待最长的一次所花的时间

- Innodb_row_lock_waits

  系统启动后到现在总共等待的次数

当等待的次数很高，而且每次等待的时长也不小的时候，我们就需要分析系统中为什么会有如此多的等待，然后根据分析结果着手制定优化计划。





### 总结

InnoDB存储引擎由于实现了行级锁定，虽然在锁定机制的实现方面带来了性能损耗可能比表锁会更高一些，但是在整体并发处理能力方面要远远由于MyISAM的表锁的。当系统并发量较高的时候，InnoDB的整体性能和MyISAM相比就会有比较明显的优势。

但是，InnoDB的行级锁同样也有其脆弱的一面，当我们使用不当的时候，可能会让InnoDB的整体性能表现不仅不能比MyISAM高，甚至可能会更差。



优化建议：

- 尽可能让所有数据检索都能通过索引来完成，避免无索引行锁升级为表锁。
- 合理设计索引，尽量缩小锁的范围
- 尽可能减少索引条件，及索引范围，避免间隙锁
- 尽量控制事务大小，减少锁定资源量和时间长度
- 尽可使用低级别事务隔离（但是需要业务层面满足需求）

# 常用sql技巧

## SQL执行顺序

编写顺序

```SQL
SELECT DISTINCT
	<select list>
FROM
	<left_table> <join_type>
JOIN
	<right_table> ON <join_condition>
WHERE
	<where_condition>
GROUP BY
	<group_by_list>
HAVING
	<having_condition>
ORDER BY
	<order_by_condition>
LIMIT
	<limit_params>
```

执行顺序

``` sql
FROM	<left_table>

ON 		<join_condition>

<join_type>		JOIN	<right_table>

WHERE		<where_condition>

GROUP BY 	<group_by_list>

HAVING		<having_condition>

SELECT DISTINCT		<select list>

ORDER BY	<order_by_condition>

LIMIT		<limit_params>
```



## 正则表达式使用

正则表达式（Regular Expression）是指一个用来描述或者匹配一系列符合某个句法规则的字符串的单个字符串。

| 符号   | 含义                          |
| ------ | ----------------------------- |
| ^      | 在字符串开始处进行匹配        |
| $      | 在字符串末尾处进行匹配        |
| .      | 匹配任意单个字符, 包括换行符  |
| [...]  | 匹配出括号内的任意字符        |
| [^...] | 匹配不出括号内的任意字符      |
| a*     | 匹配零个或者多个a(包括空串)   |
| a+     | 匹配一个或者多个a(不包括空串) |
| a?     | 匹配零个或者一个a             |
| a1\|a2 | 匹配a1或a2                    |
| a(m)   | 匹配m个a                      |
| a(m,)  | 至少匹配m个a                  |
| a(m,n) | 匹配m个a 到 n个a              |
| a(,n)  | 匹配0到n个a                   |
| (...)  | 将模式元素组成单一元素        |

```
select * from emp where name regexp '^T';

select * from emp where name regexp '2$';

select * from emp where name regexp '[uvw]';
```



## MySQL 常用函数

数字函数

| 函数名称        | 作 用                                                      |
| --------------- | ---------------------------------------------------------- |
| ABS             | 求绝对值                                                   |
| SQRT            | 求二次方根                                                 |
| MOD             | 求余数                                                     |
| CEIL 和 CEILING | 两个函数功能相同，都是返回不小于参数的最小整数，即向上取整 |
| FLOOR           | 向下取整，返回值转化为一个BIGINT                           |
| RAND            | 生成一个0~1之间的随机数，传入整数参数是，用来产生重复序列  |
| ROUND           | 对所传参数进行四舍五入                                     |
| SIGN            | 返回参数的符号                                             |
| POW 和 POWER    | 两个函数的功能相同，都是所传参数的次方的结果值             |
| SIN             | 求正弦值                                                   |
| ASIN            | 求反正弦值，与函数 SIN 互为反函数                          |
| COS             | 求余弦值                                                   |
| ACOS            | 求反余弦值，与函数 COS 互为反函数                          |
| TAN             | 求正切值                                                   |
| ATAN            | 求反正切值，与函数 TAN 互为反函数                          |
| COT             | 求余切值                                                   |

字符串函数

| 函数名称  | 作 用                                                        |
| --------- | ------------------------------------------------------------ |
| LENGTH    | 计算字符串长度函数，返回字符串的字节长度                     |
| CONCAT    | 合并字符串函数，返回结果为连接参数产生的字符串，参数可以使一个或多个 |
| INSERT    | 替换字符串函数                                               |
| LOWER     | 将字符串中的字母转换为小写                                   |
| UPPER     | 将字符串中的字母转换为大写                                   |
| LEFT      | 从左侧字截取符串，返回字符串左边的若干个字符                 |
| RIGHT     | 从右侧字截取符串，返回字符串右边的若干个字符                 |
| TRIM      | 删除字符串左右两侧的空格                                     |
| REPLACE   | 字符串替换函数，返回替换后的新字符串                         |
| SUBSTRING | 截取字符串，返回从指定位置开始的指定长度的字符换             |
| REVERSE   | 字符串反转（逆序）函数，返回与原始字符串顺序相反的字符串     |

日期函数

| 函数名称                | 作 用                                                        |
| ----------------------- | ------------------------------------------------------------ |
| CURDATE 和 CURRENT_DATE | 两个函数作用相同，返回当前系统的日期值                       |
| CURTIME 和 CURRENT_TIME | 两个函数作用相同，返回当前系统的时间值                       |
| NOW 和  SYSDATE         | 两个函数作用相同，返回当前系统的日期和时间值                 |
| MONTH                   | 获取指定日期中的月份                                         |
| MONTHNAME               | 获取指定日期中的月份英文名称                                 |
| DAYNAME                 | 获取指定曰期对应的星期几的英文名称                           |
| DAYOFWEEK               | 获取指定日期对应的一周的索引位置值                           |
| WEEK                    | 获取指定日期是一年中的第几周，返回值的范围是否为 0〜52 或 1〜53 |
| DAYOFYEAR               | 获取指定曰期是一年中的第几天，返回值范围是1~366              |
| DAYOFMONTH              | 获取指定日期是一个月中是第几天，返回值范围是1~31             |
| YEAR                    | 获取年份，返回值范围是 1970〜2069                            |
| TIME_TO_SEC             | 将时间参数转换为秒数                                         |
| SEC_TO_TIME             | 将秒数转换为时间，与TIME_TO_SEC 互为反函数                   |
| DATE_ADD 和 ADDDATE     | 两个函数功能相同，都是向日期添加指定的时间间隔               |
| DATE_SUB 和 SUBDATE     | 两个函数功能相同，都是向日期减去指定的时间间隔               |
| ADDTIME                 | 时间加法运算，在原始时间上添加指定的时间                     |
| SUBTIME                 | 时间减法运算，在原始时间上减去指定的时间                     |
| DATEDIFF                | 获取两个日期之间间隔，返回参数 1 减去参数 2 的值             |
| DATE_FORMAT             | 格式化指定的日期，根据参数返回指定格式的值                   |
| WEEKDAY                 | 获取指定日期在一周内的对应的工作日索引                       |

聚合函数

| 函数名称 | 作用                             |
| -------- | -------------------------------- |
| MAX      | 查询指定列的最大值               |
| MIN      | 查询指定列的最小值               |
| COUNT    | 统计查询结果的行数               |
| SUM      | 求和，返回指定列的总和           |
| AVG      | 求平均值，返回指定列数据的平均值 |


# 常用工具
## mysql

该mysql不是指mysql服务，而是指mysql的客户端工具。

**语法 ：**

```sh
mysql [options] [database]
```

**连接选项：**

| 参数               | 说明               |
| ------------------ | ------------------ |
| -u, --user=txt     | 指定用户名         |
| -p, --password=txt | 指定密码           |
| -h, --host=txt     | 指定服务器IP或域名 |
| -p, --port=#       | 指定连接端口       |


示例 ：

```sql
mysql -h 127.0.0.1 -P 3306 -u root -p
	
mysql -h127.0.0.1 -P3306 -uroot -p2143	-- 可不加空格
```

**执行选项**

| 参数               | 说明              |
| ------------------ | ----------------- |
| -e, --execute=name | 执行SQL语句并退出 |

此选项可以在Mysql客户端执行SQL语句，而不用连接到MySQL数据库再执行，对于一些批处理脚本，这种方式尤其方便。

示例：

```sh
mysql -uroot -p2143 db01 -e "select * from tb_book";
```

![1555325632715](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555325632715.png) 

## mysqladmin

mysqladmin 是一个执行管理操作的客户端程序。可以用它来检查服务器的配置和当前状态、创建并删除数据库等。

查看帮助文档指令

```sh
mysqladmin --help
```



![1555326108697](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1555326108697.png)

示例 ： 

```sh
mysqladmin -uroot -p2143 create 'test01';  
mysqladmin -uroot -p2143 drop 'test01';
mysqladmin -uroot -p2143 version;
```

## mysqlbinlog

由于服务器生成的二进制日志文件以二进制格式保存，所以如果想要检查这些文本的文本格式，就会使用到mysqlbinlog 日志管理工具。

语法 ：

```sh
mysqlbinlog [options]  log-files1 log-files2 ...
```

| 参数选项                                      | 说明                                         |
| --------------------------------------------- | -------------------------------------------- |
| -d, --database=name                           | 指定数据库名称，只列出指定的数据库相关操作。 |
| -o, --offset=#                                | 忽略掉日志中的前n行命令。                    |
| -r,--result-file=name                         | 将输出的文本格式日志输出到指定文件。         |
| -s, --short-form                              | 显示简单格式， 省略掉一些信息。              |
| --start-datatime=date1  --stop-datetime=date2 | 指定日期间隔内的所有日志。                   |
| --start-position=pos1 --stop-position=pos2    | 指定位置间隔内的所有日志。                   |



## mysqldump

mysqldump 客户端工具用来备份数据库或在不同数据库之间进行数据迁移。备份内容包含创建表，及插入表的SQL语句。

语法 ：

```sh
mysqldump [options] db_name [tables]

mysqldump [options] --database/-B db1 [db2 db3...]

mysqldump [options] --all-databases/-A
```

**连接选项**

| 参数                  | 说明               |
| --------------------- | ------------------ |
| -u, --user=name       | 指定用户名         |
| -p, --password[=name] | 指定密码           |
| -h, --host=name       | 指定服务器IP或域名 |
| -P, --port=#          | 指定连接端口       |

​	

**输出内容选项**



| 参数                 | 说明                                                         |
| -------------------- | ------------------------------------------------------------ |
| --add-drop-database  | 在每个数据库创建语句前加上 Drop database 语句                |
| --add-drop-table     | 在每个表创建语句前加上 Drop table 语句 , 默认开启 ; 不开启 (--skip-add-drop-table) |
| -n, --no-create-db   | 不包含数据库的创建语句                                       |
| -t, --no-create-info | 不包含数据表的创建语句                                       |
| -d --no-data         | 不包含数据                                                   |
| -T, --tab=name       | 自动生成两个文件：<br/>一个.sql文件，创建表结构的语句；<br/>一个.txt文件，数据文件，相当于 select into outfile ； |

示例 ：
```sh
mysqldump -uroot -p2143 db01 tb_book --add-drop-database --add-drop-table > a
	
mysqldump -uroot -p2143 -T /tmp test city
```

## mysqlimport和source

mysqlimport 是客户端数据导入工具，用来导入 mysqldump 加 -T 参数后导出的文本文件。

也就是表的数据内容（txt内容）

语法：

```sh
mysqlimport [options]  db_name  textfile1  [textfile2...]
```

示例：

```sh
mysqlimport -uroot -p2143 test /tmp/city.txt
```



如果需要导入sql文件,可以使用mysql中的source 指令 : 

```sh
source /root/tb_book.sql
```

## mysqlshow

mysqlshow 客户端对象查找工具，用来很快地查找存在哪些数据库、数据库中的表、表中的列或者索引。

语法：

```sh
mysqlshow [options] [db_name [table_name [col_name]]]
```

参数：

| 参数    | 说明                                                |
| ------- | --------------------------------------------------- |
| --count | 显示数据库及表的统计信息（数据库，表 均可以不指定） |
| -i      | 显示指定数据库或者指定表的状态信息                  |



示例：

```sh
#查询每个数据库的表的数量及表中记录的数量
mysqlshow -uroot -p2143 --count

#查询test库中每个表中的字段书，及行数
mysqlshow -uroot -p2143 test --count

#查询test库中book表的详细情况
mysqlshow -uroot -p2143 test book --count
```

# 日志
## 错误日志

错误日志是 MySQL 中最重要的日志之一，它记录了当 `mysqld` 启动和停止时，以及服务器在运行过程中发生任何严重错误时的相关信息。当数据库出现任何故障导致无法正常使用时，可以首先查看此日志。

该日志是默认开启的 ， 默认存放目录为 mysql 的数据目录：`var/lib/mysql `

默认的日志文件名为  `hostname.err`（hostname是主机名）。



查看日志位置指令 ： 

```sh
show variables like 'log_error%';
```

![1553993244446](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553993244446.png) 



查看日志内容 ： 

```sh
tail -f /var/lib/mysql/xaxh-server.err
```

![1553993537874](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1553993537874.png) 

##  二进制日志

### 概述

二进制日志（BINLOG）记录了所有的 DDL（数据定义语言）语句和 DML（数据操纵语言）语句，但是**不包括数据查询语句**。此日志对于灾难时的数据恢复起着极其重要的作用，MySQL的主从复制， 就是通过该 binlog 实现的。

二进制日志，默认情况下是没有开启的，需要到MySQL的配置文件中开启，并配置MySQL日志的格式。 

配置文件位置 :  `/usr/my.cnf`

日志存放位置 : 配置时，给定了文件名但是没有指定路径，日志默认写入Mysql的数据目录。

```properties
#配置开启 binlog 日志，
#日志的文件前缀为 mysqlbin
#生成的文件名如 : mysqlbin.000001，mysqlbin.000002
log_bin=mysqlbin

#配置二进制日志的格式
binlog_format=STATEMENT
```



### 日志格式

**STATEMENT**

该日志格式在日志文件中记录的都是SQL语句（statement），每一条对数据进行修改的 SQL 都会记录在日志文件中，通过 Mysql 提供的 mysqlbinlog 工具，可以清晰的查看到每条语句的文本。

主从复制的时候，从库（slave）会将日志解析为原文本，并在从库重新执行一次。



**ROW**

该日志格式在日志文件中记录的是每一行的数据变更，而不是记录SQL语句。

比如，执行SQL语句 ： `update tb_book set status='1' `

如果是 STATEMENT 日志格式，在日志中会记录一行SQL文件； 

如果是 ROW，由于是对全表进行更新，也就是每一行记录都会发生变更，ROW 格式的日志中会记录每一行的数据变更。



**MIXED**

这是目前MySQL默认的日志格式，即混合了 STATEMENT 和 ROW 两种格式。

默认情况下采用STATEMENT，但是在一些特殊情况下采用ROW来进行记录。

MIXED 格式能尽量利用两种模式的优点，而避开他们的缺点。



### 日志读取

由于日志以二进制方式存储，不能直接读取，需要用 mysqlbinlog 工具来查看，语法如下 ：

```sh
mysqlbinlog log-file；
```



**查看STATEMENT格式日志** 

执行插入语句 ：

```SQL
insert into tb_book values(null,'Lucene','2088-05-01','0');
```

 查看日志文件 ：

![1554079717375](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554079717375.png) 

`mysqlbin.index` : 该文件是日志索引文件 ， 记录日志的文件名；

`mysqlbing.000001` ：日志文件

查看日志内容 ：

```sh
mysqlbinlog mysqlbing.000001；
```

![1554080016778](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554080016778.png) 



**查看ROW格式日志**

配置 :

```properties
#配置开启 binlog 日志， 
#日志的文件前缀为 mysqlbin
#生成的文件名如 : mysqlbin.000001，mysqlbin.000002
log_bin=mysqlbin

#配置二进制日志的格式
binlog_format=ROW

```

插入数据 :

```sql
insert into tb_book values(null,'SpringCloud实战','2088-05-05','0');
```

如果日志格式是 ROW , 直接查看数据 , 是查看不懂的 ; 可以在 mysqlbinlog 后面加上参数 -vv  

```sh
mysqlbinlog -vv mysqlbin.000002 
```

![1554095452022](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554095452022.png) 



### 日志删除

对于比较繁忙的系统，由于每天生成日志量大 ，这些日志如果长时间不清楚，将会占用大量的磁盘空间。下面我们将会讲解几种删除日志的常见方法 ：

- **方式一** 

通过 `Reset Master` 指令删除全部 binlog 日志，删除之后，日志编号，将从 xxxx.000001重新开始 。

查询之前 ，先查询下日志文件 ： 

![1554118609489](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554118609489.png)   

执行删除日志指令： 

```sh
Reset Master
```

执行之后， 查看日志文件 ：

![1554118675264](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554118675264.png) 



- **方式二**

执行指令 ``` purge  master logs to 'mysqlbin.******'``` ，该命令将删除  ``` ******``` 编号之前的所有日志。 



- **方式三**

执行指令： ``` purge master logs before 'yyyy-mm-dd hh24:mi:ss'``` 

该命令将删除日志为 "yyyy-mm-dd hh24:mi:ss" 之前产生的所有日志 。



- **方式四**

设置参数 `--expire_logs_days=#` ，此参数的含义是设置日志的过期天数， 过了指定的天数后日志将会被自动删除，这样将有利于减少DBA 管理日志的工作量。

配置如下 ： 

![1554125506938](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554125506938.png) 



## 查询日志

查询日志中记录了客户端的所有操作语句，而二进制日志不包含查询数据的SQL语句。

默认情况下， 查询日志是未开启的。如果需要开启查询日志，可以设置以下配置 ：

```properties
#该选项用来开启查询日志
#可选值：0 或者 1 ；0 代表关闭， 1 代表开启 
general_log=1

#设置日志的文件名，如果没有指定，默认的文件名为 host_name.log 
general_log_file=file_name
```

在 mysql 的配置文件 `/usr/my.cnf` 中配置如下内容 ： 

![1554128184632](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554128184632.png) 



配置完毕之后，在数据库执行以下操作 ：

```sql
select * from tb_book;
select * from tb_book where id = 1;
update tb_book set name = 'lucene入门指南' where id = 5;
select * from tb_book where id < 8;
```



执行完毕之后， 再次来查询日志文件 ： 

![1554128089851](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554128089851.png) 

## 慢查询日志

慢查询日志记录了所有执行时间超过参数 long_query_time 设置值并且扫描记录数不小于 min_examined_row_limit 的所有的SQL语句的日志。

long_query_time 默认为 10 秒，最小为 0， 精度可以到微秒。



### 文件位置和格式

慢查询日志默认是关闭的 。可以通过两个参数来控制慢查询日志 ：

```properties
# 该参数用来控制慢查询日志是否开启
#可取值： 1 和 0 ， 1 代表开启， 0 代表关闭
slow_query_log=1 

# 该参数用来指定慢查询日志的文件名
slow_query_log_file=slow_query.log

# 该选项用来配置查询的时间限制
#超过这个时间将认为值慢查询，将需要进行日志记录
#默认10s
long_query_time=10
```



### 日志的读取

和错误日志、查询日志一样，慢查询日志记录的格式也是纯文本，可以被直接读取。

1） 查询 long_query_time 的值。

![1554130333472](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554130333472.png) 



2） 执行查询操作

```sql
select id, title,price,num ,status from tb_item where id = 1;
```

![1554130448709](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554130448709.png)

由于该语句执行时间很短，为0s ， 所以不会记录在慢查询日志中。



```sql
select * from tb_item where title like '%阿尔卡特 (OT-927) 炭黑 联通3G手机 双卡双待165454%' ;
```

![1554130532577](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554130532577.png) 

该SQL语句 ， 执行时长为 26.77s ，超过10s ， 所以会记录在慢查询日志文件中。



3） 查看慢查询日志文件

直接通过cat 指令查询该日志文件 ： 

![1554130669360](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554130669360.png) 



如果慢查询日志内容很多， 直接查看文件，比较麻烦

这个时候可以借助于 mysql 自带的 mysqldumpslow 工具， 来对慢查询日志进行分类汇总。 

![1554130856485](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554130856485.png) 

# 主从复制

## 复制概述

复制是指将主数据库的DDL 和 DML 操作通过二进制日志传到从库服务器中，然后在从库上对这些日志重新执行（也叫重做），从而使得从库和主库的数据保持同步。

MySQL支持一台主库同时向多台从库进行复制， 从库同时也可以作为其他从服务器的主库，实现链状复制。



## 复制原理

MySQL 的主从复制原理如下。

![1554423698190](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1.jpg) 

从上层来看，复制分成三步：

- Master 主库在事务提交时，会把数据变更作为时间 Events 记录在二进制日志文件 Binlog 中。
- 主库推送二进制日志文件 Binlog 中的日志事件到从库的中继日志 Relay Log 。

- slave 重做中继日志中的事件，将改变反映它自己的数据。



## 复制优势

MySQL 复制的有点主要包含以下三个方面：

- 主库出现问题，可以快速切换到从库提供服务。

- 可以在从库上执行查询操作，从主库中更新，实现读写分离，降低主库的访问压力。

- 可以在从库中执行备份，以避免备份期间影响主库的服务。



## 搭建步骤

### master

1） 在master 的配置文件（/usr/my.cnf）中，配置如下内容：

```properties
#mysql 服务ID,保证整个集群环境中唯一
server-id=1

#mysql binlog 日志的存储路径和文件名
log-bin=/var/lib/mysql/mysqlbin

#错误日志,默认已经开启
#log-err

#mysql的安装目录
#basedir

#mysql的临时目录
#tmpdir

#mysql的数据存放目录
#datadir

#是否只读,1 代表只读, 0 代表读写
read-only=0

#忽略的数据, 指不需要同步的数据库
binlog-ignore-db=mysql

#指定同步的数据库
#binlog-do-db=db01
```

2） 执行完毕之后，需要重启Mysql：

```sh
service mysql restart
#有的是这个
service mysqld restart
```

3） 创建同步数据的账户，并且进行授权操作：

```sql
grant replication slave on *.* to 'itcast'@'192.168.192.131' identified by 'itcast';	

flush privileges;
```

4） 查看master状态：

```sql
show master status;
```

![1554477759735](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554477759735.png) 




| 字段             | 含义                           |
| ---------------- | ------------------------------ |
| File             | 从哪个日志文件开始推送日志文件 |
| Position         | 从哪个位置开始推送日志         |
| Binlog_Ignore_DB | 指定不需要同步的数据库         |



### slave

1） 在 slave 端配置文件中，配置如下内容：

```properties
#mysql服务端ID,唯一
server-id=2

#指定binlog日志
log-bin=/var/lib/mysql/mysqlbin
```

2）  执行完毕之后，需要重启Mysql：

```sh
service mysql restart；
```

3） 执行如下指令 ：

```sql
change master to master_host= '192.168.192.130', master_user='itcast', master_password='itcast', master_log_file='mysqlbin.000001', master_log_pos=413;
```

指定当前从库对应的主库的IP地址，用户名，密码，从哪个日志文件开始的那个位置开始同步推送日志。

4） 开启同步操作

```sql
start slave;

show slave status;
```

![1554479387365](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554479387365.png) 

5） 停止同步操作

```sql
stop slave;
```



### 验证同步操作

1） 在主库中创建数据库，创建表，并插入数据 ：

```sql
create database db01;

user db01;

create table user(
	id int(11) not null auto_increment,
	name varchar(50) not null,
	sex varchar(1),
	primary key (id)
)engine=innodb default charset=utf8;

insert into user(id,name,sex) values(null,'Tom','1');
insert into user(id,name,sex) values(null,'Trigger','0');
insert into user(id,name,sex) values(null,'Dawn','1');
```

2） 在从库中查询数据，进行验证 ：

在从库中，可以查看到刚才创建的数据库：

![1554544658640](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554544658640.png) 

在该数据库中，查询user表中的数据：

![1554544679538](https://cdn.jsdelivr.net/gh/oddfar/static/img/MySQL高级.assets/1554544679538.png) 





