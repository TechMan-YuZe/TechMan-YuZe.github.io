#
# 初始java

## Java : 一个帝国的诞生

### 1、C语言帝国的统治

现在是公元1995年， C语言帝国已经统治了我们20多年， 实在是太久了。 



1972年， 随着C语言的诞生和Unix的问世， 帝国迅速建立统治， 从北美到欧洲， 从欧洲到亚洲，  无数程序员臣服在他的脚下。



帝国给我们提供了极好的福利：贴近硬件，  运行极快， 效率极高。  



使用这些福利， 程序员们用C 开发了很多系统级软件，操作系统， 编译器， 数据库，网络系统.....



但是帝国也给我们安上了两个沉重的枷锁： 指针和内存管理



虽然指针无比强大， 能直接操作内存， 但是帝国却没有给我们工具去做越界的检查， 导致很多新手程序员轻易犯错。



至于内存管理， 帝国更完全是放任的态度： 你自己分配的空间， 自己去释放 ！



更要命的是这些问题在编译期发现不了， 在运行时才会突然暴露， 常常让我们手忙脚乱， 昏天黑地去调试。 



我们的大量时间和宝贵的精力都被浪费在小心翼翼的处理指针和内存分配上。 



每个程序员都被这两个东西搞的焦头烂额！

 

帝国宣称的可移植性骗了我们，他宣称我们在一个机器上写的程序， 只要在另外一个机器上编译就可以了， 实际上不是这样。 他要求我们尽量用标准的C函数库。其次，如果遇到了一些针对特定平台的调用， 需要对每个平台都得写一份 ！  有一点点小错误，都会导致编译失败。 



1982年，帝国又推出了一门新的语言C++, 添加了面向对象的功能，兼容C, 有静态类型检查， 性能也很好。  



但是这门新的语言实在是太复杂了， 复杂到比我聪明的多的人都没有办法完全掌握这门语言，它的很多特性复杂的让人吃惊。 



C++在图形领域和游戏上取得了一些成功， 但是我一直学不好它。 

### 2、反抗

我决定反抗这个庞大的帝国，  我偷偷的带领着一帮志同道合的兄弟离开了，我们要新建一块清新自由的领地。 



为了吸引更多的程序员加入我们， 我们要建立一个新的语言，这个语言应该有这样的特性：



语法有点像C ， 这样大家容易接受

没有C语言那样的指针 

再也不要考虑内存管理了， 实在受不了了

真正的可移植性， 编写一次， 到处运行

面向对象

类型安全

还有，我们要提供一套高质量的类库， 随语言发行。 



我想把这个语言命名为C++--  , 即C++减减，  因为我想在C++的基础上改进，把它简化。 



后来发现不行， 设计理念差别太大。



干脆重启炉灶。 



我看到门口的一棵橡树， 就把这个语言叫做Oak。 

但是后来发布的时候， 发现Oak已经被别人用了， 我们讨论很久， 最终决定把这门新的语言叫做 Java。 



为了实现跨平台， 我们在操作系统和应用程序之间增加了一个抽象层： Java 虚拟机



用Java写的程序都跑在虚拟机上， 除非个别情况， 都不用看到操作系统。

### 3、一鸣惊人

为了吸引更多的人加入我们的新领地， 我们决定搞一个演示， 向大家展示Java 的能力。 



出世未久的Java其实还远不完善。 搞点什么好呢？



我们把眼光盯上了刚刚兴起的互联网， 1995年的网页简单而粗糙， 缺乏互动性。 于是我们在浏览器上弄了个小插件， 把java 运行环境放了上去。



然后在上面开发了一个图形界面的程序(Applet)， 让它看起来美轮美奂， 震撼人心。 



每一个看到他的程序员都会发出“Wow”的惊叹 ！为之倾倒。 



Java 活了！



通过Applet , 无数的程序员看到了Java这门语言，了解了这门语言特性以后， 很多无法忍受C帝国暴政的程序员， 很快加入了我们， 我们的领地开始迅速扩大。 



连C语言帝国里的一些商业巨头也纷纷来和我们合作， 其中就包括Oracle , 微软这样的巨头 ， 微软的头领Bill Gates还说 ：这是迄今为止设计的最好的语言！



但是Bill Gates非常的不地道， 买了我们的Java 许可以后，虽然在自家的浏览器上也支持Applet, 但是他们却偷偷的试图修改Java ,  想把Java绑死在自家的操作系统上赚钱， Java会变的不可移植。 



这是我们难于忍受的， 我们和微软发起了一场旷日持久的游击战争， 逼着微软退出了Java领域， 开发了自己的.NET , 这是后话。

### 4、开拓疆土

从1995年到1997年，我们依靠 Java 不断的攻城略地， 开拓疆土，我们王国的子民不断增加， 达到了几十万之众， 已经是一个不可忽视的力量了。

 

但是大家发现， Java除了Applet, 以及一些小程序之外， 似乎干不了别的事情。 



C帝国的人还不断的嘲笑我们慢， 像个玩具。



到了1998年， 经过密谋， 我们Java 王国决定派出三只军队向外扩展：

Java 2 标准版(J2SE)： 去占领桌面

Java 2 移动版(J2ME)： 去占领手机

Java 2 企业版(J2EE)： 去占领服务器



其中的两只大军很快败下阵来。



J2SE 的首领发现， 开发桌面应用的程序员根本接受不了Java， 虽然我们有做的很优雅的Swing 可以开发界面， 但是开发出的界面非常难看， 和原生的桌面差距很大。 尤其是为了运行程序还得安装一个虚拟机， 大家都受不了。  



J2ME也是， 一直不受待见，  当然更重要的原因是乔布斯还没有重新发明手机， 移动互联网还没有启动。 



失之东隅，收之桑榆， J2EE赶上了好时候， 互联网大发展， 大家忽然发现， Java简直是为写服务器端程序所发明的！



强大， 健壮， 安全， 简单， 跨平台 ！



在J2EE规范的指导下， 特别适合团队开发复杂的大型项目。



我们授权BEA公司第一个使用J2EE许可证， 推出了Weblogic,  凭借其集群功能， 第一次展示了复杂应用的可扩展性和高可用性。 



这个后来被称为中间件的东西把程序员从事务管理，安全管理，权限管理等方面解放出来， 让他们专注于业务开发。  这立刻捕获了大量程序员的心。



很快Java 王国的子民就达到数百万之众。 



榜样的力量是无穷的， 很快其他商业巨头也纷纷入场， 尤其是IBM，在Java 上疯狂投入，不仅开发了自己的应用服务器 Websphere,  还推出了Eclipse这个极具魅力的开源开发平台。



当然IBM利用java 获得了非常可观的效益， 软件+硬件+服务  三驾马车滚滚向前， 把IBM推向了一个新的高峰。

### 5、帝国的诞生

大家也没有想到，除了商业巨头以外， 程序员们也会对Java王国 这么热爱， 他们基于Java 开发了巨多的平台，系统，工具，例如：



构建工具: Ant，Maven, Jekins



应用服务器： Tomcat，Jetty, Jboss, Websphere, weblogic



Web开发：  Struts,Spring,Hibernate, myBatis



开发工具： Eclipse, Netbean,intellij idea, Jbuilder

。。。。等等等等。。。。



并且绝大部分都是开源的 ！



微软眼睁睁的看着服务器端的市场被Java 王国占据， 岂能善罢甘休？ 他们赶紧推出.NET来对抗， 但我们已经不在乎了， 因为他的系统是封闭的，所有的软件都是自家的：

开发工具是Visual Studio, 应用服务器是IIS, 数据库是SQL Server，只要你用.NET，基本上就会绑定微软。 



另外他们的系统只能运行在Windows服务器上， 这个服务器在高端市场的占有率实在是太低了。 



2005年底， 一个新的王国突然崛起， 他们号称开发效率比java 快5-10倍， 由此吸引了大批程序员前往加盟。 



这个新的王国叫做Ruby on Rails, 它结合了PHP体系的优点（快速开发）和Java体系的优点（程序规整）， 特别适合快速的开发简单的Web网站。 



虽然发展很快， 但没有对Java 王国产生实质性的威胁， 使用Ruby on Rails搭建大型商业系统的还很少。



除了Ruby on Rails  ，还有PHP， Python ， 都适合快速开发不太复杂的Web系统。 但是关键的，复杂的商业系统开发还是Java 王国的统治之下。 所以我们和他们相安无事。



2006年， 一只叫Hadoop的军队让Java王国入侵了大数据领域， 由于使用Java 语言， 绝大多数程序员在理解了Map/Reduce , 分布式文件系统在Hadoop中的实现以后， 很快就能编写处理处理海量数据的程序， Java 王国的领地得到了极大的扩展。



2008年，  一个名叫Android 的系统横空出世， 并且随着移动互联网的爆发迅速普及，  运行在Android之上的正是Java ！  



Java 王国在Google的支持下， 以一种意想不到的方式占领了手机端， 完成了当年J2ME 壮志未酬的事业 ！



到今年为止， 全世界估计有1000万程序员加入了Java王国，它领土之广泛， 实力之强大， 是其他语言无法比拟的。 



Java 占据了大部分的服务器端开发，尤其是关键的复杂的系统， 绝大多数的手机端， 以及大部分的大数据领域。 



一个伟大的帝国诞生了。 



## Java的特性和优势

### 八大特性

**1、跨平台/可移植性**

这是Java的核心优势。Java在设计时就很注重移植和跨平台性。比如：Java的int永远都是32位。不像C++可能是16，32，可能是根据编译器厂商规定的变化。这样的话程序的移植就会非常麻烦。

 **2、安全性**

Java适合于网络/分布式环境，为了达到这个目标，在安全性方面投入了很大的精力，使Java可以很容易构建防病毒，防篡改的系统。

 **3、面向对象**

面向对象是一种程序设计技术，非常适合大型软件的设计和开发。由于C++为了照顾大量C语言使用者而兼容了C，使得自身仅仅成为了带类的C语言，多少影响了其面向对象的彻底性！

Java则是完全的面向对象语言。

**4、简单性**

Java就是C++语法的简化版，我们也可以将Java称之为“C++-”。跟我念“C加加减”，指的就是将C++的一些内容去掉；比如：头文件，指针运算，结构，联合，操作符重载，虚基类等等。

同时，由于语法基于C语言，因此学习起来完全不费力。

 **5、高性能**

Java最初发展阶段，总是被人诟病“性能低”；客观上，高级语言运行效率总是低于低级语言的，这个无法避免。Java语言本身发展中通过虚拟机的优化提升了几十倍运行效率。

比如，通过JIT(JUST IN TIME)即时编译技术提高运行效率。 将一些“热点”字节码编译成本地机器码，并将结果缓存起来，在需要的时候重新调用。这样的话，使Java程序的执行效率大大提高，

某些代码甚至接待C++的效率。因此，Java低性能的短腿，已经被完全解决了。业界发展上，我们也看到很多C++应用转到Java开发，很多C++程序员转型为Java程序员。

 **6、分布式**

Java是为Internet的分布式环境设计的，因为它能够处理TCP/IP协议。事实上，通过URL访问一个网络资源和访问本地文件是一样简单的。Java还支持远程方法调用(RMI,Remote Method Invocation)，

使程序能够通过网络调用方法。

 **7、多线程**

多线程的使用可以带来更好的交互响应和实时行为。 Java多线程的简单性是Java成为主流服务器端开发语言的主要原因之一。

 **8、健壮性**

Java是一种健壮的语言，吸收了C/C++ 语言的优点，但去掉了其影响程序健壮性的部分（如：指针、内存的申请与释放等）。Java程序不可能造成计算机崩溃。即使Java程序也可能有错误。

如果出现某种出乎意料之事，程序也不会崩溃，而是把该异常抛出，再通过异常处理机制加以处理。

### 核心优势

![img](https://cdn.jsdelivr.net/gh/oddfar/static/img/初识java.assets/v2-9992d6134d870ebd7d6b93c11440329d_720w.jpg)

　　跨平台是Java语言的核心优势，赶上最初互联网的发展，并随着互联网的发展而发展，建立了强大的生态体系，目前已经覆盖IT各行业的“第一大语言”，是计算机界的“英语”。

　　虽然，目前也有很多跨平台的语言，但是已经失去先机，无法和Java强大的生态体系抗衡。Java仍将在未来几十年成为编程语言的主流语言。

JAVA虚拟机是JAVA实现跨平台的核心。事实上，基于JAVA虚拟机(JVM)的编程语言还有很多种：

![img](https://cdn.jsdelivr.net/gh/oddfar/static/img/初识java.assets/v2-646ad77cd0889ca096285ba5f7e4f3ee_720w.jpg)

基于JAVA生态建立的产品将会越来越多；基于JAVA虚拟机的编程语言也将会越来越多；生态系统的强大，是JAVA能长盛不衰的根本。

## Java三大版本

**JAVA最大的特点：**

 Java的主要优势在于其做出的WORA：即一次编写（Write Once）、随处运行（Run Anywhere）。简单来讲，这意味着开发团队能够利用Java编写一款应用程序，并将其编译为可执行形式，而后将其运行 在任何支持Java的平台之上。这显然能够极大提高编程工作的实际效率，这种优势来源于Java Virtual Machine(JAVA虚拟机的缩写)，JVM是一种用于计算设备的规范，它是一个虚构出来的计算机，是通过在 实际的计算机上仿真模拟各种计算机功能来实现的。JAVA语言的一个非常重要的特点就是与平台的无关 性，而使用Java虚拟机是实现这一特点的关键。

**JAVA三大版本：**

1. JAVA SE：它是JAVA的标准版，是整个JAVA的基础和核心，这是我们主要学习的一个部分，也是 JAVAEE和JAVAME技术的基础，主要用于开发桌面应用程序。学会后可以做一些简单的桌面应用 如：扫雷，连连看等。 
2. JAVA ME：它是JAVA的微缩版，主要应用于嵌入式开发，比如手机程序的开发。目前来说就业范围不是很广，在一些城市可能相对的不好找工作。 
3. JAVA EE：也叫JAVA的企业版，它提供了企业级应用开发的完整解决方案，比如开发网站，还有企业的一些应用系统，是JAVA技术应用最广泛的领域。主要还是偏向于WEB的开发，而JAVA EE的基础就是JAVA SE，所以我们在学习JAVA SE的时候，基础一定要打好，因为这是最基本的，也是最核 心的。

## JDK 和 JRE

**JDK**

Java 2 SDK (Development Kit)包含：JRE的超集，包含编译器和调试器等用于程序开发的文件

**JRE**

Java Runtime Environment (JRE) 包含：Java虚拟机、库函数、运行Java应用程序和Applet所必须文件

Java运行环境的三项主要功能：

- 加载代码：由class loader 完成；
- 校验代码：由bytecode verifier 完成；
- 执行代码：由 runtime interpreter完成。

**区别和联系**：

sdk（也就是jdk）是jre的超集，是在jre的基础上增加了编译器及其他一些开发工具。

jre就是java运行时环境，包括了jvm和其它一些java核心api,任何一台电脑，只有安装了jre才可以行 java程序.

如果只是要运行JAVA程序，之需要JRE就可以。 JRE通常非常小，也包含了JVM.

如果要开发JAVA程序，就需要安装JDK。

## 初识JVM

JVM（JAVA Virtual Machine）

JVM是一种规范，可以使用软件来实现，也可以使用硬件来实现，就是一个虚拟的用于执byte-codes 字节码的计算机。他也定义了指令集、寄存器集、结构栈、垃圾收集堆、内存区域。

JVM负责将java字节码解释运行，边解释边运行，这样，速度就会受到一定的影响。JAVA提供了另一种 解释运行的方法JIT（just in time），可以一次解释完，再运行特定平台上的机器码，高级的JIT可以只能 分析热点代码，并将这些代码转成本地机器码，并将结果缓存起来，下次直接从内存中调用，这样就大 大提高了执行JAVA代码的效率。这样就实现了跨平台、可移植的功能。

1. JVM是指在一台计算机上由软件或硬件模拟的计算机；它类似一个小巧而高效的CPU。 

2. byte-code代码是与平台无关的是虚拟机的机器指令。 

3. java字节代码运行的两种方式:

   -  interpreter(解释)

      运行期解释字节码并执行

   -  Just-in-time(即时编译)

      由代码生成器将字节代码转换成本机的机器代码,然后可以以较高速度执行。

[^初识JVM]:  https://www.jianshu.com/p/17ab51b87a13
JAVA的跨平台实现的核心是不同平台使用不同的虚拟机 

不同的操作系统有不同的虚拟机。Java 虚拟机机制屏蔽了底层运行平台的差别，实现了“一次编译，随处运行”。



## JAVA程序运行机制

说到Java的运行机制，不得不提一下什么是编译型语言，什么是解释型语言。

### **编译型语言**

编译型语言是先将源代码编译成机器语言（机器可以读懂的语言），再由机器运行机器码，这样执行程序的效率比较高。像C和C++就是典型的编译型语言。

### **解释型语言**

其实解释型语言是相对编译型语言存在的，解释型语言是在运行的时候才进行编译，每次运行都需要编译，这样效率比较低。像JavaScript，Python就是典型的解释型语言

### **二者的区别**

简单的举个例子：同样一本英文书，找人翻译成中文版的书然后拿给你看就是编译，找一个翻译员在你旁边给你解读书的含义就是解释。两者各有利弊，编译型语言执行效率高，翻译一次可以多次运行。解释性语言执行效率低，每次运行都需要重新翻译。但是解释型的跨平台性相对要好，比如解释给一个懂中文和解释给一个懂日文的人就叫做兼容性。

### **Java的运行机制**

Java属于两者都有，既有编译过程，又是解释型语言

Java语言虽然比较接近解释型语言的特征，但在执行之前已经预先进行一次预编译，生成的代码是介 于机器码和Java源代码之间的中介代码，运行的时候则由JVM（Java的虚拟机平台，可视为解释器）解 释执行。它既保留了源代码的高抽象、可移植的特点，又已经完成了对源代码的大部分预编译工作，所以 执行起来比“纯解释型”程序要快许多。

总之，随着设计技术与硬件的不断发展，编译型与解释型两种方式的界限正在不断变得模糊。

::: tip 第一步：编译

:::

利用编译器（javac）将源程序编译成字节码à 字节码文件名：源文件名.class

::: tip 第二部：运行

:::



利用虚拟机（解释器，java）解释执行class字节码文件。

![image-20210319180207773](https://cdn.jsdelivr.net/gh/oddfar/static/img/初识java.assets/image-20210319180207773.png)


## Hello World

需要先配置好开发环境

参考链接：https://www.runoob.com/java/java-environment-setup.html

测试代码一定要写HelloWorld！代表你向这个世界的呐喊，仪式感很重要，就像你生活 中和家人，朋友，妻子在节日中或者纪念日一定要做一些事情，这就是仪式感。

1. 新建文件 Hello.java

2. 编写我们的HelloWorld程序！

   ```java
   public class Hello{
       public static void main(String[] args){
           System.out.println("Hello,World!");
       }
   }
   ```

3. 保存文件，cmd打开命令行，利用javac编译！

   ```cmd
   javac Hello.java
   # 如果没有报错，查看文件夹下是否有新的一个文件
   # Hello.class
   # 如果没有出现，恭喜！说明你遇到了你在学Java当中的第一个Bug
   ```

4. java 执行！

   ```cdm
   java Hello
   # 成功输出Hello，World！
   ```

如果出现错误，检查字母大小写是否有错误，或者是否标点符号错误，文件名错误等等，一定要确保成功输出

**编写 Java 程序时，应注意以下几点：**

- 大小写敏感

  Java 是大小写敏感的，这就意味着标识符 Hello 与 hello 是不同的。

- 类名

  对于所有的类来说，类名的首字母应该大写。如果类名由若干单词组成，那么每个单词的首字母应该大写，例如 MyFirstJavaClass 。

- 方法名

  所有的方法名都应该以小写字母开头。如果方法名含有若干单词，则后面的每个单词首字 母大写。

- 源文件名

  源文件名必须和类名相同。当保存文件的时候，你应该使用类名作为文件名保存（切记 Java 是大小写敏感的），文件名的后缀为 .java。（如果文件名和类名不相同则会导致编译错误）。

- 主方法入口

  所有的 Java 程序由 public static void main(String []args) 方法开始执行。



# JavaSE-基础语法

## 注释

平时我们编写代码，在代码量比较少的时候，我们还可以看懂自己写的，但是当项目结构一旦复杂起来，我们就需要用到一个注释了，注释就类似于我们上学时候写的笔记，我们看着笔记就知道自己写的 什么东西了！在程序中也是如此。我们来看一下Java中的注释怎么写，看以下代码：

```java
/*
* @Description HelloWorld类
* @Author Diamond 狂神
**/
public class HelloWorld {
    /*
    这是我们Java程序的主入口，
    main方法也是程序的主线程。
    */
    public static void main(String[] args) {
        //输出HelloWorld！
        System.out.println("Hello,World!");
    }
}

```

注释并不会被执行，是给我们写代码的人看的，书写注释是一个非常好的习惯。

**Java中的注释有三种：**

单行注释：只能注释当前行，以//开始，直到行结束

```java
//输出HelloWorld！
```

多行注释：注释一段文字，以/*开始， */结束！

```java
/*
    这是我们Java程序的主入口，
    main方法也是程序的主线程。
*/
```

文档注释：用于生产API文档，配合JavaDoc。

```java
/*
* @Description HelloWorld类
* @Author Diamond 狂神
**/
```


## 标识符

每个人从出生开始就有一个名字，咋们生活中的所有事物也都有名字，这名字是谁规定呢？回答是：造物主，谁生产出来的谁规定名字，在我们的程序中也不例外。

我们作为造物主，需要给所有的东西给上一个名字，比如我们的HelloWorld程序：

HelloWorld是类名，也是我们的文件名。它前面的 public class是关键字，不过是搞Java那群人已经定 义好的有特殊作用的，下面的每一个代码都有自己的意思和名字对吧，就是用来作区分！和我们的名字 一样，拿来被叫或者称呼的，程序一切都源自于生活，一定要把学程序和生活中的一切联系起来，你会发现这一切都是息息相关的。

![image-20210319190451624](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210319190451624.png)

我们来看看有哪些是Java自己定义好的关键字呢？

![image-20210319190649910](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210319190649910.png)

我们自己起名字有哪些要求呢？ 

表示类名的标识符用大写字母开始。

> 如：Man, GoodMan

表示方法和变量的标识符用小写字母开始，后面的描述性词以大写开始。

> 如：eat(),eatFood()

具体可参考《阿里巴巴Java开发手册》

**关于 Java 标识符，有以下几点需要注意：**

- 所有的标识符都应该以字母（A-Z 或者 a-z）美元符（$）或者下划线（_）开始
- 首字符之后可以是字母（A-Z 或者 a-z）美元符（$）下划线（_）或数字的任何字符组合
- 不能使用关键字作为变量名或方法名。
- 标识符是大小写敏感的
- 合法标识符举例：age、$salary、_value、__1_value
- 非法标识符举例：123abc、-salary、#abc

JAVA不采用通常语言使用的ASCII字符集，而是采用unicode这样的标准的国际字符集。因此，这里的 字母的含义：可以表示英文、汉字等等。

可以使用中文命名，但是一般不建议这样去使用，也不建议使用拼音，很Low



## 数据类型

Java是一种强类型语言，每个变量都必须声明其类型。

扩展：各种字符集和编码详解(https://www.cnblogs.com/cmt/p/14553189.html)

### 1、强弱类型语言

- 强类型语言

  强类型语言是一种强制类型定义的语言，一旦某一个变量被定义类型，如果不经过强制转换，则它永远就是该数据类型了，强类型语言包括Java、.net 、Python、C++等语言。

  举个例子：定义了一个整数，如果不进行强制的类型转换，则不可以将该整数转化为字符串。

- 弱类型语言

  弱类型语言是一种弱类型定义的语言，某一个变量被定义类型，该变量可以根据环境变化自动进行转换，不需要经过显性强制转换。弱类型语言包括vb 、PHP、javascript等语言。

  在VB Script中，可以将字符串‘12’和整数3进行连接得到字符串‘123’，也可以把它看成整数123，而不需 要显示转换。是不是十分的随便，我们Java就不是这样的。

- 区别

  无论是强类型语言还是弱类型语言，判别的根本是是否会隐性的进行语言类型转变。强类型语言在速度上略逊于弱类型语言，但是强类型定义语言带来的严谨性又能避免不必要的错误。

### 2、数据类型

Java的数据类型分为两大类：基本类型（primitive type）和引用类型 （reference type）

![image-20210319191956137](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210319191956137.png)

【注：引用数据类型的大小统一为4个字节，记录的是其引用对象的地址！】

![image-20210319192043592](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210319192043592.png)

如果你看到这一堆头疼的话，没关系，不用记，JDK中类型对应的包装类都帮忙写好了，我们需要时候可 以直接看到！可以把以下代码拷贝进行查看结果：

```java
public static void main(String[] args) {
    // byte
    System.out.println("基本类型：byte 二进制位数：" + Byte.SIZE);
    System.out.println("包装类：java.lang.Byte");
    System.out.println("最小值：Byte.MIN_VALUE=" + Byte.MIN_VALUE);
    System.out.println("最大值：Byte.MAX_VALUE=" + Byte.MAX_VALUE);
    System.out.println();
    // short
    System.out.println("基本类型：short 二进制位数：" + Short.SIZE);
    System.out.println("包装类：java.lang.Short");
    System.out.println("最小值：Short.MIN_VALUE=" + Short.MIN_VALUE);
    System.out.println("最大值：Short.MAX_VALUE=" + Short.MAX_VALUE);
    System.out.println();
    // int
    System.out.println("基本类型：int 二进制位数：" + Integer.SIZE);
    System.out.println("包装类：java.lang.Integer");
    System.out.println("最小值：Integer.MIN_VALUE=" + Integer.MIN_VALUE);
    System.out.println("最大值：Integer.MAX_VALUE=" + Integer.MAX_VALUE);
    System.out.println();
    // long
    System.out.println("基本类型：long 二进制位数：" + Long.SIZE);
    System.out.println("包装类：java.lang.Long");
    System.out.println("最小值：Long.MIN_VALUE=" + Long.MIN_VALUE);
    System.out.println("最大值：Long.MAX_VALUE=" + Long.MAX_VALUE);
    System.out.println();
    // float
    System.out.println("基本类型：float 二进制位数：" + Float.SIZE);
    System.out.println("包装类：java.lang.Float");
    System.out.println("最小值：Float.MIN_VALUE=" + Float.MIN_VALUE);
    System.out.println("最大值：Float.MAX_VALUE=" + Float.MAX_VALUE);
    System.out.println();
    // double
    System.out.println("基本类型：double 二进制位数：" + Double.SIZE);
    System.out.println("包装类：java.lang.Double");
    System.out.println("最小值：Double.MIN_VALUE=" + Double.MIN_VALUE);
    System.out.println("最大值：Double.MAX_VALUE=" + Double.MAX_VALUE);
    System.out.println();
    // char
    System.out.println("基本类型：char 二进制位数：" + Character.SIZE);
    System.out.println("包装类：java.lang.Character");
    // 以数值形式而不是字符形式将Character.MIN_VALUE输出到控制台
    System.out.println("最小值：Character.MIN_VALUE="+ (int) Character.MIN_VALUE);
    // 以数值形式而不是字符形式将Character.MAX_VALUE输出到控制台
    System.out.println("最大值：Character.MAX_VALUE="+ (int) Character.MAX_VALUE);
}
```

字节相关知识：

> 位（bit）：是计算机 内部数据 储存的最小单位，11001100是一个八位二进制数。
>
> 字节（byte）：是计算机中 数据处理 的基本单位，习惯上用大写 B 来表示。
>
> ​	1B（byte,字节）= 8bit（位）
>
> 字符：是指计算机中使用的字母、数字、字和符号

ASCIIS码：

| 内容                      | 占用大小 |
| ------------------------- | -------- |
| 1个英文字符（不分大小写） | 1个字节  |
| 1个中文汉字               | 2个字节  |
| 1个ASCII码                | 1个字节  |

UTF-8编码：

| 内容            | 占用大小 |
| --------------- | -------- |
| 1个英文字符     | 1个字节  |
| 英文标点        | 1个字节  |
| 1个中文（含繁体 | 3个字节  |
| 中文标点        | 3个字节  |

Unicode编码：

| 内容            | 占用大小 |
| --------------- | -------- |
| 1个英文字符     | 2个字节  |
| 英文标点        | 2个字节  |
| 1个中文（含繁体 | 2个字节  |
| 中文标点        | 2个字节  |

1bit表示1位
1Byte表示一个字节

1B=8b
1024B=1KB
1024KB=1M
1024M=1G

------

那有人会问：电脑的32位和64位的区别是什么呢？

- 32位操作系统只可以使用32位的cpu，而64位的CPU既可以安装32位操作系统也可以安装64位操作 系统。

- 寻址能力简单点说就是支持的内存大小能力，64位系统最多可以支达128 GB的内存，而32位系统最 多只可以支持4G内存。

- 32位操作系统只可以安装使用32位架构设计的软件，而64位的CPU既可以安装使用32位软件也可以 安装使用64位软件。

- 现在的电脑都是64位了！

回到正题，我们了解了这些知识后，我们自己定义一些变量来看！

```java
public static void main(String[] args) {
    //整型
    int i1=100;
    //长整型
    long i2=998877665544332211L;
    //短整型
    short i3=235;
    //浮点型
    double d1=3.5; //双精度
    double d2=3;
    float f1=(float)3.5; //单精度
    float f2=3.5f; //单精度
    //布尔类型 boolean true真/false假
    boolean isPass=true;
    boolean isOk=false;
    boolean isBig=5>8;
    if(isPass){
    System.out.println("通过了");
    }else{
    System.out.println("未通过");
    }
    //单字符
    char f='女';
    char m='男';
}
```

Java语言的整型常数默认为int型，浮点数默认是Double

### 3、整型拓展

在我们计算机中存在很多进制问题，十进制，八进制，十六进制等等的问题，他们怎么表示呢？

- 十进制整数，如：99, -500, 0。 

- 八进制整数，要求以 0 开头，如：015。 

- 十六进制数，要求 0x 或 0X 开头，如：0x15 。

演示：

```java
//整型
int i= 10;
int i2= 010;
int i3= 0x10;
System.out.println(i); //10
System.out.println(i2); //8
System.out.println(i3); //16
```

### 4、浮点型拓展

【金融面试问：银行金融业务用什么类型表示？】

浮点类型float, double的数据不适合在不容许舍入误差的金融计算领域。 

如果需要进行不产生舍入误差的精确数字计算，需要使用BigDecimal类。

```java
public static void main(String[] args) {
    float f = 0.1f;
    double d = 1.0/10;
    System.out.println(f==d); //false
    
    float d1 = 2131231231f;
    float d2 = d1+1;
    if(d1==d2){
        System.out.println("d1==d2");
    }else{
        System.out.println("d1!=d2");
    }
}
```

最后运行结果：

>false
>d1==d2

**主要理由：**

由于字长有限，浮点数能够精确表示的数是有限的，因而也是离散的。浮点数一般都存在舍入误差，很 多数字无法精确表示，其结果只能是接近，但不等于；二进制浮点数不能精确的表示0.1,0.01,0.001这样10的负次幂。并不是所有的小数都能可以精确的用二进制浮点数表示。

大数值：Java.math下面的两个有用的类：BigInteger和BigDecimal，这两个类可以处理任意长度的数 值。BigInteger实现了任意精度的整数运算。BigDecimal实现了任意精度的浮点运算。

**浮点数使用总结：**

1. 默认是double
2. 浮点数存在舍入误差，很多数字不能精确表示。如果需要进行不产生舍入误差的精确数字计算，需 要使用BigDecimal类。
3. 避免比较中使用浮点数

### 5、字符型拓展

单引号用来表示字符常量。例如‘A’是一个字符，它与“A”是不同的，“A”表示一个字符串。

 char 类型用来表示在Unicode编码表中的字符。

Unicode编码被设计用来处理各种语言的所有文字，它占2个字节，可允许有65536个字符；

科普：2字节=16位，2的16次方=65536，我们用的Excel原来就只有这么多行，并不是无限的

【代码演示：字符转int看结果】

```java
public static void main(String[] args) {
    char c1 = 'a';
    char c2 = '中';
    System.out.println(c1);
    System.out.println((int) c1); //97
    System.out.println(c2);
    System.out.println((int) c2); //20013
}
```

Unicode具有从0到65535之间的编码，他们通常用从’u0000’到’uFFFF’之间的十六进制值来表示（前缀为 u表示Unicode）

```java
char c3 = '\u0061';
System.out.println(c3); //a
```

Java 语言中还允许使用转义字符 ‘’ 来将其后的字符转变为其它的含义，有如下常用转义字符：

![image-20210326234124183](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210326234124183.png)

【以后我们学的String类，其实是字符序列(char sequence)。在这里给大家一个思考题】

```java
//代码1
String sa=new String("Hello world");
String sb=new String("Hello world");
System.out.println(sa==sb); // false
//代码2
String sc="Hello world";
String sd="Hello world";
System.out.println(sc==sd); // true
```

大家可以先思考下为什么，之后我们学到对象的时候，会给大家进行内存级别的分析，那时候你会恍然 大悟！

### 6、布尔型拓展

boolean类型（一位，不是一个字节），就是0|1 

boolean类型有两个值，true和false,不可以 0 或非 0 的整数替代 true 和 false ，这点和C语言不同。 

boolean 类型用来判断逻辑条件，一般用于程序流程控制。

```java
boolean flag = false;
if(flag){
    // true分支
}else{
    // false分支
}
```

【编码规范：很多新手程序员喜欢这样写】

```java
if (is == true && un == false ) {...}
```

只有新手才那么写。对于一个熟练的人来说，应该用如下方式来表示：

```java
if ( is && !un ) {....}
```

前面加个 ! 表示否定

这点都不难理解吧。所以要习惯去掉所有的==fasle 和 ==true。Less is More！！ 代码要精简易读！


## 类型转换

由于Java是强类型语言，所以要进行有些运算的时候的，需要用到类型转换。

整型、实型（常量）、字符型数据可以混合运算。

运算中，不同类型的数据先转化为同一类型，然后进行运算。

转换从低级到高级（根据容量来看）。

> 低 ------------------------------------> 高
>
> byte,short,char—> int —> long—> float —> double

数据类型转换必须满足如下规则：

- 不能对boolean类型进行类型转换。

- 不能把对象类型转换成不相关类的对象。

- 在把容量大的类型转换为容量小的类型时必须使用强制类型转换。

- 转换过程中可能导致溢出或损失精度，例如：

  ```java
  int i = 128;
  byte b = (byte)i;
  ```

  因为 byte 类型是 8 位，最大值为127，所以当 int 强制转换为 byte 类型时，值 128 时候就会导致溢出。

  推荐文章：[细谈为什么单字节的整数范围是[-128 ~ 127]](https://blog.csdn.net/lirui1212/article/details/114950520)

浮点数到整数的转换是通过舍弃小数得到，而不是四舍五入，例如：

> (int)23.7 == 23;
> (int)-45.89f == -45

### 1、自动类型转换

自动类型转换：容量小的数据类型可以自动转换为容量大的数据类型。

例如: short数据类型的位数为16位，就可以自动转换位数为32的int类型，同样float数据类型的位数为 32，可以自动转换为64位的double类型。

```java
public static void main(String[] args) {
    char c1 = 'a';//定义一个char类型
    int i1 = c1;//char自动类型转换为int
    System.out.println("char自动类型转换为int后的值等于" + i1);
    char c2 = 'A';//定义一个char类型
    int i2 = c2 + 1;//char 类型和 int 类型计算
    System.out.println("char类型和int计算后的值等于" + i2);
}
```

解析：c1 的值为字符 a ,查 ASCII 码表可知对应的 int 类型值为 97，所以i1=97。 A 对应值为 65，所以 i2=65+1=66。

### 2、强制类型转换

强制类型转换，又被称为造型，用于显式的转换一个数值的类型。

在有可能丢失信息的情况下进行的转换是通过造型来完成的，但可能造成精度降低或溢出。

强制类型转换的语法格式：` (type)var` ，运算符 “()” 中的 type 表示将值var想要转换成的目标数据类型。 条件是转换的数据类型必须是兼容的。

```java
public static void main(String[] args) {
    double x = 3.14;
    int nx = (int) x; //值为3
    char c = 'a';
    int d = c + 1;
    System.out.println(d); //98
    System.out.println((char) d); //b
}
```

当将一种类型强制转换成另一种类型，而又超出了目标类型的表示范围，就会被截断成为一个完全不同 的值，溢出。

```java
public static void main(String[] args) {
    int x = 300;
    byte bx = (byte)x; //值为44
    System.out.println(bx);
}
```

### 3、常见错误和问题

- 操作比较大的数时，要留意是否溢出，尤其是整数操作时；

  ```java
  public static void main(String[] args) {
      int money = 1000000000; //10亿
      int years = 20;
      int total = money * years; //返回的是负数
      long total1 = money * years; //返回的仍然是负数。默认是int，因此结果会转成int值，再转成long。但是已经发生了数据丢失
      long total2 = money * ((long) years); //先将一个因子变成long，整个表达式发生提升。全部用long来计算。
      System.out.println(total); //-1474836480
      System.out.println(total1); //-1474836480
      System.out.println(total2); //20000000000
  }
  ```

- L和l 的问题：

  - 不要命名名字为l的变量

  - long类型使用大写L不要用小写。

    ```java
    public static void main(String[] args) {
        int l = 2;
        long a = 23451l;
        System.out.println(l + 1); //3
        System.out.println(a); //23451
    }
    ```

### 4、JDK7扩展

JDK7新特性: **二进制整数**

由于我们在开发中也经常使用二进制整数，因此JDK7为我们直接提供了二进制整数的类型。

我们只要以：0b开头即可。

```java
int a = 0b0101;
```

JDK7新特性：**下划线分隔符**

在实际开发和学习中，如果遇到特别长的数字，读懂它令人头疼！JDK7为我们提供了下划线分隔符，可 以按照自己的习惯进行分割。

```java
int b = 1_2234_5678;
```

我们很容易就知道这是1亿2234万5678啦！ 非常符合国人的习惯！

```java
public static void main(String[] args) {
    int a = 0b0101;
    int b = 1_2345_7893;
    System.out.println(a); //5
    System.out.println(b); //123457893
}
```



## 变量，常量

### 1、变量（variable）

变量是什么：就是可以变化的量！

我们通过变量来操纵存储空间中的数据，变量就是指代这个存储空间！空间位置是确定的，但是里面放 置什么值不确定！ 打个比方：

这就好像我们家里有一个大衣柜，里面有十分多的小格子，我们给格子上贴上标签，放衣服，放鞋子， 放手表等等，此时我们知道了哪里该放什么，但是，我们并不知道里面到底放的是什么牌子的鞋子，是 衣服还是裤子。那个标签就相当于我们的变量，我们给他起了个名字，但是里面要放什么需要我们自己 去放。

Java是一种强类型语言，每个变量都必须声明其类型。

Java变量是程序中最基本的存储单元，其要素包括变量名，变量类型和作用域。

变量在使用前必须对其声明, 只有在变量声明以后，才能为其分配相应长度的存储单元，声明格式为：

>数据类型 变量名 = 值；
>
>可以使用逗号隔开来声明多个同类型变量。

注意事项：

- 每个变量都有类型，类型可以是基本类型，也可以是引用类型。
- 变量名必须是合法的标识符。
- 变量声明是一条完整的语句，因此每一个声明都必须以分号结束

【演示】

```java
int a, b, c; // 声明三个int型整数：a、 b、c
int d = 3, e = 4, f = 5; // 声明三个整数并赋予初值
byte z = 22; // 声明并初始化 z
String s = "runoob"; // 声明并初始化字符串 s
double pi = 3.14159; // 声明了双精度浮点型变量 pi
char x = 'x'; // 声明变量 x 的值是字符 'x'。
```

【编码规范】

虽然可以在一行声明多个变量，但是不提倡这个风格，逐一声明每一个变量可以提高程序可读性。

### 2、变量作用域

变量根据作用域可划分为三种：

- 类变量（静态变量： static variable）：独立于方法之外的变量，用 static 修饰。
- 实例变量（成员变量：member variable）：独立于方法之外的变量，不过没有 static 修饰。
- 局部变量（lacal variable）：类的方法中的变量。

```java
public class Variable{
    static int allClicks = 0; // 类变量
    String str = "hello world"; // 实例变量
    
    public void method(){
        int i =0; // 局部变量
    }
}
```

#### 局部变量

方法或语句块内部定义的变量。生命周期是从声明位置开始到 ”}” 为止

在使用前必须先声明和初始化(赋初值)。

局部变量没有默认值，所以局部变量被声明后，必须经过初始化，才可以使用。

```java
public static void main(String[] args) {
    int i;
    int j = i + 5; // 编译出错，变量i还未被初始化
    System.out.println(j);
}
```

修改为：

```java
public static void main(String[] args) {
    int i=10;
    int j = i+5 ;
    System.out.println(j);
}
```

#### 实例变量

方法外部、类的内部定义的变量。

从属于对象，生命周期伴随对象始终。

如果不自行初始化，他会自动初始化成该类型的默认初始值

（数值型变量初始化成0或0.0，字符型变量的初始化值是16位的0，布尔型默认是false）

```java
public class Test {
    // 这个实例变量对子类可见
    public String name;
    // 私有变量，仅在该类可见
    private double salary;
}
```

#### 静态变量

使用static定义。

从属于类，生命周期伴随类始终，从类加载到卸载。

(注：讲完内存分析后我们再深入！先放一放这个概念！)

> 不同的类之间需要对同一个变量进行操作，比如一个水池，同时打开入水口和出水口，进水和出水这两个动作会同时影响到池中的水量，此时池中的水量就可以认为是一个共享的变量。该变量就是静态变量
>
> 静态简单的说是 被类的所有对象共享，比如有一个类，有学校，姓名，年龄三个参数，调用就需要给这三个赋上值，假如这些人都是一个学校的，每次调用都需要赋值就太重复，加上静态的话，一个赋值了，每次调用则都是那个值

如果不自行初始化，他会自动初始化成该类型的默认初始值

（数值型变量初始化成0或0.0，字符型变量的初始化值是16位的0，布尔型默认是false）

```java
public class Employee {
    //salary是静态的私有变量
    private static double salary;
    // DEPARTMENT是一个常量
    public static final String DEPARTMENT = "开发人员";
    public static void main(String[] args){
        salary = 10000;
        System.out.println(DEPARTMENT+"平均工资:"+salary);
    }
}
```

### 3、常量

常量(Constant)：初始化(initialize)后不能再改变值！不会变动的值。

所谓常量可以理解成一种特殊的变量，它的值被设定后，在程序运行过程中不允许被改变。

```java
final 常量名=值;
final double PI=3.14;
final String LOVE="hello";
```

常量名一般使用大写字符。 

程序中使用常量可以提高代码的可维护性。例如，在项目开发时，我们需要指定用户的性别，此时可以 定义一个常量 SEX，赋值为 "男"，在需要指定用户性别的地方直接调用此常量即可，避免了由于用户的 不规范赋值导致程序出错的情况。

### 4、变量的命名规范

1. 所有变量、方法、类名：见名知意 
2. 类成员变量：首字母小写和驼峰原则 : monthSalary
3. 局部变量：首字母小写和驼峰原则 
4. 常量：大写字母和下划线：MAX_VALUE 
5. 类名：首字母大写和驼峰原则: Man, GoodMan 
6. 方法名：首字母小写和驼峰原则: run(), runRun()

具体可参考《阿里巴巴Java开发手册》


## 运算符

运算符operator

Java 语言支持如下运算符：

- 算术运算符  +，-，*，/，%，++，--
- 赋值运算符 =
- 关系运算符  >，<，>=，<=，==，!= instanceof
- 逻辑运算符 &&，||，!
- 位运算符  &，|，^，~ ， >>，<<，>>> (了解！！！)
- 条件运算符 ？：
- 扩展赋值运算符  +=，-=，*=，/=

### 1、二元运算符

两个操作数，来看看我们小时候的数学运算；

```java
public static void main(String[] args) {
    int a = 10;
    int b = 20;
    int c = 25;
    int d = 25;
    System.out.println("a + b = " + (a + b) );
    System.out.println("a - b = " + (a - b) );
    System.out.println("a * b = " + (a * b) );
    System.out.println("b / a = " + (b / a) );
}
```

**整数运算**

如果两个操作数有一个为Long, 则结果也为long

没有long时，结果为int。即使操作数全为shot,byte，结果也是int.

```java
public static void main(String[] args) {
    long a = 1231321311231231L;
    int b = 1213;
    short c = 10;
    byte d = 8;

    System.out.println(a + b + c + d); //Long类型
    System.out.println(b + c + d);//Int类型
    System.out.println(c + d);//Int类型
}
```

**浮点运算**

如果两个操作数有一个为double, 则结果为double

只有两个操作数都是float, 则结果才为float

```java
public static void main(String[] args) {
    float a = 3.14565F;
    double b = 3.194546464;
    float c = 1.3123123F;
    System.out.println(a+b); //double类型
    System.out.println(b+c); //double类型
    System.out.println(a+c); //float类型
}
```

**关系运算符**

返回布尔值！

![image-20210327143549464](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210327143549464.png)

可参考 [菜鸟教程](https://www.runoob.com/java/java-operators.html)

### 2、取模运算

就是我们小学的取余； 

> 5%3 余 2

其操作数可以为浮点数,一般使用整数。如：5.9%3.9=2.000000004

**要点**：

负数%负数＝负数； 

负数%正数＝负数； 

正数%负数＝正数；

```java
public static void main(String[] args) {
    System.out.println(9 % 4); //1
    System.out.println(-9 % -4); //-1
    System.out.println(-10 % 4); //-2
    System.out.println(9 % -4); //1
}
```

【注：一般都是正整数运算，进行结果的判断！】

### 3、一元运算符

自增（++）自减（--）运算符是一种特殊的算术运算符，在算术运算符中需要两个操作数来进行运算， 而自增自减运算符是一个操作数，分为前缀和后缀两种。

```java
public static void main(String[] args) {
    int a = 3;
    int b = a++; //执行完后,b=3。先给b赋值，再自增。
    int c = ++a; //执行完后,c=5。先自增,再给b赋值
}
```

注意：java中的乘幂处理

```java
public static void main(String[] args) {
    int a = 3^2; //java中不能这么处理， ^是异或符号。
    double b = Math.pow(3, 2);
}
```

Math类提供了很多科学和工程计算需要的方法和常数。特殊的运算都需要运用到方法!

### 4、逻辑运算符

逻辑与：&&和&
逻辑或：||和|
逻辑非：！

![image-20210327144148985](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210327144148985.png)

【演示】

```java
public static void main(String[] args) {
    boolean a = true;
    boolean b = false;
    System.out.println("a && b = " + (a&&b));
    System.out.println("a || b = " + (a||b) );
    System.out.println("!(a && b) = " + !(a && b));
}
```

**逻辑与** 和 **逻辑或** 采用短路的方式。从左到右计算，如果确定值则不会再计算下去。在两个操作数都为 true时，结果才为true，但是当得到第一个操作为false时，其结果就必定是false，这时候就不会再判断 第二个操作了。

逻辑与只要有一个为false, 则直接返回false.

逻辑或只要有一个为true, 则直接返回true;

```java
public static void main(String[] args){
    int a = 5;//定义一个变量；
    boolean b = (a<4)&&(a++<10);
    System.out.println("使用短路逻辑运算符的结果为"+b);
    System.out.println("a的结果为"+a);
}
```

解析： 该程序使用到了短路逻辑运算符(&&)，首先判断 a<4 的结果为 false，则 b 的结果必定是 false， 所以不再执行第二个操作 a++<10 的判断，所以 a 的值为 5。

### 5、位运算符

Java定义了位运算符，应用于整数类型(int)，长整型(long)，短整型(short)，字符型(char)，和字节型 (byte)等类型。位运算符作用在所有的位上，并且按位运算。

假设a = 60，b = 13;它们的二进制格式表示将如下：

```
A = 0011 1100
B = 0000 1101
-----------------
A&B = 0000 1100
A | B = 0011 1101
A ^ B = 0011 0001
~A= 1100 0011
```

![image-20210327144737549](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210327144737549.png)

右移一位相当于除2取商。

左移一位相当于乘2。

【常见面试题：int a=2*8怎样运算效率最快？】

```java
public static void main(String[] args) {
    System.out.println(2 << 3);
}
```

用移位运算 int a=2<<3; 
a就是2乘以8 最后结果是16 这是最省内存 最有效率的方法

这个方法确实高效率的。我来解释一下： 
2的二进制是10 在32位存储器里面是0000 0000 0000 0010 
左移三位后变成 0000 0000 0001 0000 也就是16

解释一下，在系统中运算是以二进制的形式进行的。相比来说俩个二进制数相乘运算比移位运算慢一 些。

位操作是程序设计中对位模式按位或二进制数的一元和二元操作。 在许多古老的微处理器上， 位运算比加减运算略快， 通常位运算比乘除法运算要快很多。 在现代架构中， 情况并非如此：位运算的运算速度 通常与加法运算相同(仍然快于乘法运算). 详细的需要了解计算机的组成原理！

### 6、扩展运算符

![image-20210327150556669](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210327150556669.png)

```java
public static void main(String[] args) {
    int a=10;
    int b=20;
    
    a+=b; // a = a + b
    
    System.out.println(a+":"+b);
}
```

### 7、字符串连接符

“+” 运算符两侧的操作数中只要有一个是字符串(String)类型，系统会自动将另一个操作数转换为字符串 然后再进行连接。

```java
//字符串
String s1="Hello 中文!";
String s2=1+""; //转换成String
//int
int c = 12;
System.out.println("c=" + c);
```

### 8、三目条件运算符

三目条件运算符，语法格式：

> x ? y : z

其中x为boolean类型表达式，先计算x的值，若为true，则整个三目运算的结果为表达式y的值，否则整个运算结果为表达式z的值。

【演示】

```java
public static void main(String[] args) {
    int score = 80;
    String type = score < 60 ? "不及格" : "及格";
    System.out.println("type= " + type);
}
```

三元运算符在真实开发中十分的常见，大家可以多练习使用，之后我们会讲解分支语句，可以利用三元运算符做到更加精简代码！便于理解！

### 9、运算符优先级

我们小学都学过：先加减，后乘除，所以优先级我们并不陌生。

当多个运算符出现在一个表达式中，谁先谁后呢？这就涉及到运算符的优先级别的问题。在一个多运算符的表达式中，运算符优先级不同会导致最后得出的结果差别甚大。

下表中具有最高优先级的运算符在的表的最上面，最低优先级的在表的底部。

| 类别     | 操作符                                     | 关联性   |
| :------- | :----------------------------------------- | :------- |
| 后缀     | () [] . (点操作符)                         | 左到右   |
| 一元     | expr++ expr--                              | 从左到右 |
| 一元     | ++expr --expr + - ～ ！                    | 从右到左 |
| 乘性     | * /％                                      | 左到右   |
| 加性     | + -                                        | 左到右   |
| 移位     | >> >>>  <<                                 | 左到右   |
| 关系     | > >= < <=                                  | 左到右   |
| 相等     | == !=                                      | 左到右   |
| 按位与   | ＆                                         | 左到右   |
| 按位异或 | ^                                          | 左到右   |
| 按位或   | \|                                         | 左到右   |
| 逻辑与   | &&                                         | 左到右   |
| 逻辑或   | \| \|                                      | 左到右   |
| 条件     | ？：                                       | 从右到左 |
| 赋值     | = + = - = * = / =％= >> = << =＆= ^ = \| = | 从右到左 |
| 逗号     | ，                                         | 左到右   |

大家不需要去刻意的记住，表达式里面优先使用小括号来组织！！方便理解和使用，不建议写非常冗余 的代码运算！

```java
public static void main(String[] args) {
    boolean flag = 1<4*5&&122>3||'q'+3<5;
    System.out.println(flag);
}
```


# 包机制

## 1、问题发现

存在这样一个问题：当定义了多个类的时候，可能会发生类名的重复问题。

解决方式：在java中采用包机制处理开发者定义的类名冲突问题。

就好比我们平时的用电脑，一个文件夹下不能存在同名的文件，我们要是有这样的需求，但是又不想换 名字，我们就可以考虑使用新建一个文件夹来存放！在我们的Java中也是这样的。

我们在idea中创建包，输入代码后，第一行idea默认会有：package 包名路径，例如

![image-20210327152247746](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210327152247746.png)

![image-20210327152310010](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210327152310010.png)

就要求此份java文件必须保存在这样一个目录下，这样Java解释器才能找到它。 在IDEA中能正确运行， 你可以去Windows下的工程中查看，HelloWorld这个文件必是在这样的目录结构下的。

3-6行是文档注释，便于把java文件打包成文档自动生成文件信息，以后会遇到，在阿里巴巴开发手册中，要求添加@author的注释信息 ，可以下载个阿里巴巴开发手册插件配置在ide里

## 2、包的作用

为了更好地组织类，Java 提供了包机制，用于区别类名的命名空间。

**包的作用：**

1、把功能相似或相关的类或接口组织在同一个包中，方便类的查找和使用。

2、如同文件夹一样，包也采用了树形目录的存储方式。同一个包中的类名字是不同的，不同的包中的类的名字是可以相同的，当同时调用两个不同包中相同类名的类时，应该加上包名加以区别。因此，包可以避免名字冲突。

3、包也限定了访问权限，拥有包访问权限的类才能访问某个包中的类。

Java 使用包（package）这种机制是为了防止命名冲突，访问控制，提供搜索和定位类（class）、接口、枚举（enumerations）和注释（annotation）等。

包语句的语法格式为：

```java
package pkg1[．pkg2[．pkg3…]];
```

例如,一个Something.java 文件它的内容:

```java
package net.java.util;
public class Something{
...
}
```

那么它的路径应该是 net/java/util/Something.java 这样保存的。

package(包) 的作用是把不同的 java 程序分类保存，更方便的被其他 java 程序调用。

一个包（package）可以定义为一组相互联系的类型（类、接口、枚举和注释），为这些类型提供访问 保护和命名空间管理的功能。

以下是一些 Java 中的包：

- java.lang-打包基础的类
- java.io-包含输入输出功能的函数

开发者可以自己把一组类和接口等打包，并定义自己的包。而且在实际开发中这样做是值得提倡的，当你自己完成类的实现之后，将相关的类分组，可以让其他的编程者更容易地确定哪些类、接口、枚举和 注释等是相关的。

由于包创建了新的命名空间（namespace），所以不会跟其他包中的任何名字产生命名冲突。使用包这 种机制，更容易实现访问控制，并且让定位相关类更加简单。

## 3、创建包

创建包的时候，你需要为这个包取一个合适的名字。之后，如果其他的一个源文件包含了这个包提供的类、接口、枚举或者注释类型的时候，都必须将这个包的声明放在这个源文件的开头。

包声明应该在源文件的第一行，每个源文件只能有一个包声明，这个文件中的每个类型都应用于它。

如果一个源文件中没有使用包声明，那么其中的类，函数，枚举，注释等将被放在一个无名的包 （unnamed package）中。

一般利用公司域名倒置作为报名；

例子：

www.baidu.com 包名：com.baidu.www

bbs.baidu.com 包名：com.baidu.bbs

我们平时也可以按照自己的公司域名去写，比如：com.kuangstudy.utils

## 4、import 关键字

为了能够使用某一个包的成员，我们需要在 Java 程序中明确导入该包。使用 "import" 语句可完成此功能。

在 java 源文件中 import 语句应位于 package 语句之后，所有类的定义之前，可以没有，也可以有多条，其语法格式为：

```java
import package1[.package2…].(classname|*);
```

如果在一个包中，一个类想要使用本包中的另一个类，那么该包名可以省略。

要是要用到其他包下的类，就必须要先导包！

如果两个类重名，需要导入对应的包，否则就需要写出完整地址：

```java
com.kuang.dao.Hello hello = new com.kuang.dao.Hello()
```

用 **import** 关键字引入，使用通配符 "*" , 导入io包下的所有类！

```java
import java.io.*;
```

【不建议这样使用，因为会全局扫描，影响速度！】

使用 **import** 关键字引入指定类:

```java
import com.kuang.Hello;
```

【注意】类文件中可以包含任意数量的 import 声明。import 声明必须在包声明之后，类声明之前。

【编码规范：推荐参考阿里巴巴开发手册编程规范】

## JavaDoc

### 1、简介

JavaDoc是一种将注释生成HTML文档的技术，生成的HTML文档类似于Java的API，易读且清晰明了。 在简略介绍JavaDoc写法之后，再看一下在Intellij Idea 中如何将代码中的注释生成HTML文档。

 javadoc是Sun公司提供的一个技术，它从程序源代码中抽取类、方法、成员等注释形成一个和源代码配 套的API帮助文档。也就是说，只要在编写程序时以一套特定的标签作注释，在程序编写完成后，通过 Javadoc就可以同时形成程序的开发文档了。javadoc命令是用来生成自己API文档的，使用方式：使用 命令行在目标文件所在目录输入javadoc +文件名.java。

先看一段样例代码：

```java
/**
 * 这是一个Javadoc测试程序
 *
 * @author Kuangshen
 * @version 1.0
 * @since 1.5
 */
public class HelloWorld {
    public String name;

    /**
     * @param name 姓名
     * @return 返回name姓名
     * @throws Exception 无异常抛出
     */
    public String function(String name) throws Exception {
        return name;
    }

}
```

解释一下：
以 /* 开始，以 / 结束。
@author 作者名
@version 版本号
@since 指明需要最早使用的jdk版本
@param 参数名
@return 返回值情况
@throws 异常抛出情况

### 2、命令行生成Doc

打开cmd

切换到文件当前目录  `cd /d E:\java\study\package\test`

输入指令： javadoc HelloWorld.java

一般会加上`-encoding UTF-8 -charset UTF-8 ` 解决GBK乱码问题，在中间添加编码设置

```
javadoc -encoding UTF-8 -charset UTF-8 HelloWorld.java
```

![image-20210327210911496](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-基础语法.assets/image-20210327210911496.png)

之后会多出一堆文件，打开index.html查看


# JavaSE-流程控制

## 用户交互Scanner

### 1、Scanner对象

之前我们学的基本语法中我们并没有实现程序和人的交互，但是Java给我们提供了这样一个工具类，我 们可以获取用户的输入。java.util.Scanner 是 Java5 的新特征，我们可以通过 Scanner 类来获取用户的输入。

下面是创建 Scanner 对象的基本语法：

```java
Scanner s = new Scanner(System.in);
```

接下来我们演示一个最简单的数据输入，并通过 Scanner 类的 next() 与 nextLine() 方法获取输入的字符串，在读取前我们一般需要 使用 hasNext() 与 hasNextLine() 判断是否还有输入的数据。

### 2、next & nextLine

```java
public static void main(String[] args) {
    //创建一个扫描器对象，用于接收键盘数据
    Scanner scanner = new Scanner(System.in);
    //next方式接收字符串
    System.out.println("Next方式接收:");
    //判断用户还有没有输入字符
    if (scanner.hasNext()) {
        String str = scanner.next();
        System.out.println("输入内容：" + str);
    }
    //凡是属于IO流的类如果不关闭会一直占用资源.要养成好习惯用完就关掉.就好像你接水完了要关水龙头一样.很多下载软件或者视频软件如果你不彻底关, 都会自己上传下载从而占用资源, 你就会觉得卡, 这一个道理.
    scanner.close();
}
```

测试数据：Hello World！ 

结果：只输出了Hello。 

接下来我们使用另一个方法来接收数据：nextLine()

```java
public static void main(String[] args) {
    Scanner scan = new Scanner(System.in);
    // 从键盘接收数据
    // nextLine方式接收字符串
    System.out.println("nextLine方式接收：");
    // 判断是否还有输入
    if (scan.hasNextLine()) {
        String str2 = scan.nextLine();
        System.out.println("输入内容：" + str2);
    }
    scan.close();
}
```

测试数据：Hello World！ 

结果：输出了Hello World！

**两者区别：**

next():

- 一定要读取到有效字符后才可以结束输入。 
- 对输入有效字符之前遇到的空白，next() 方法会自动将其去掉。 
- 只有输入有效字符后才将其后面输入的空白作为分隔符或者结束符。 
- next() 不能得到带有空格的字符串。

nextLine()：

- 以Enter为结束符,也就是说 nextLine()方法返回的是输入回车之前的所有字符。
- 可以获得空白。

### 3、其他方法

如果要输入 int 或 float 类型的数据，在 Scanner 类中也有支持，但是在输入之前最好先使用 hasNextXxx() 方法进行验证，再使用 nextXxx() 来读取：

```java
public static void main(String[] args) {
    Scanner scan = new Scanner(System.in);
    // 从键盘接收数据
    int i = 0;
    float f = 0.0f;
    System.out.print("输入整数：");
    if (scan.hasNextInt()) {
        // 判断输入的是否是整数
        i = scan.nextInt();
        // 接收整数
        System.out.println("整数数据：" + i);
    } else {
        // 输入错误的信息
        System.out.println("输入的不是整数！");
    }
    System.out.print("输入小数：");
    if (scan.hasNextFloat()) {
        // 判断输入的是否是小数
        f = scan.nextFloat();
        // 接收小数
        System.out.println("小数数据：" + f);
    } else {
        // 输入错误的信息
        System.out.println("输入的不是小数！");
    }
    scan.close();
}
```

具体Scanner类都有什么方法，可查看其中的源码，`ctrl`+`鼠标左键` 点中idea中的Scanner

以下实例我们可以输入多个数字，并求其总和与平均数，每输入一个数字用回车确认，通过输入非数字来结束输入，并输出执行结果：

```java
public static void main(String[] args) {
    //扫描器接收键盘数据
    Scanner scan = new Scanner(System.in);
    double sum = 0; //和
    int m = 0; //输入了多少个数字
    //通过循环判断是否还有输入，并在里面对每一次进行求和和统计
    while (scan.hasNextDouble()) {
        double x = scan.nextDouble();
        m = m + 1;
        sum = sum + x;
    }
    System.out.println(m + "个数的和为" + sum);
    System.out.println(m + "个数的平均值是" + (sum / m));
    scan.close();
}
```

可能很多小伙伴到这里就看不懂写的什么东西了！这里我们使用了我们一会要学的流程控制语句，我们 接下来就去学习这些语句的具体作用！

Java中的流程控制语句可以这样分类：顺序结构，选择结构，循环结构！这三种结构就足够解决所有的 问题了！

## 顺序结构

JAVA的基本结构就是顺序结构，除非特别指明，否则就按照顺序一句一句执行。

顺序结构是最简单的算法结构。

![image-20210327214132289](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/image-20210327214132289.png)

语句与语句之间，框与框之间是按从上到下的顺序进行的，它是由若干个依次执行的处理步骤组成的， 它是任何一个算法都离不开的一种基本算法结构。

顺序结构在程序流程图中的体现就是用流程线将程序框自上而地连接起来，按顺序执行算法步骤。

```java
public static void main(String[] args) {
    System.out.println("Hello1");
    System.out.println("Hello2");
    System.out.println("Hello3");
    System.out.println("Hello4");
    System.out.println("Hello5");
}
//按照自上而下的顺序执行！依次输出。
```

## 选择结构

### 1、if单选择结构

我们很多时候需要去判断一个东西是否可行，然后我们才去执行，这样一个过程在程序中用if语句来表 示：

![image-20210327214322066](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/image-20210327214322066.png)

```java
if(布尔表达式){
    //如果布尔表达式为true将执行的语句
}
```

意义：if语句对条件表达式进行一次测试，若测试为真，则执行下面的语句，否则跳过该语句。

【演示】比如我们来接收一个用户输入，判断输入的是否为Hello字符串：

```java
public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    //接收用户输入
    System.out.print("请输入内容：");
    String s = scanner.nextLine();
    
    if (s.equals("Hello")){
        System.out.println("输入的是："+s);
    }
    
    System.out.println("End");
    scanner.close();
}
```

equals方法是用来进行字符串的比较的，之后会详解，这里大家只需要知道他是用来比较字符串是否 一致的即可！和==是有区别的。

### 2、if双选择结构

那现在有个需求，公司要收购一个软件，成功了，给人支付100万元，失败了，自己找人开发。这样的 需求用一个if就搞不定了，我们需要有两个判断，需要一个双选择结构，所以就有了if-else结构。

![image-20210327214623634](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/image-20210327214623634.png)

```java
if(布尔表达式){
    //如果布尔表达式的值为true
    }else{
    //如果布尔表达式的值为false
}
```

意义：当条件表达式为真时，执行语句块1，否则，执行语句块2。也就是else部分。

【演示】我们来写一个示例：考试分数大于60就是及格，小于60分就不及格。

```java
public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    
    System.out.print("请输入成绩：");
    int score = scanner.nextInt();
    
    if (score>60){
        System.out.println("及格");
    }else {
        System.out.println("不及格");
    }
    
    scanner.close();
}
```

### 3、if多选择结构

我们发现上面的示例不符合实际情况，真实的情况还可能存在ABCD，存在区间多级判断。比如90-100 就是A，80-90 就是B.....，在生活中我们很多时候的选择也不仅仅只有两个，所以我们需要一个多选 择结构来处理这类问题！

![image-20210327214751941](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/image-20210327214751941.png)

```java
if(布尔表达式 1){
    //如果布尔表达式 1的值为true执行代码
}else if(布尔表达式 2){
    //如果布尔表达式 2的值为true执行代码
}else if(布尔表达式 3){
    //如果布尔表达式 3的值为true执行代码
}else {
    //如果以上布尔表达式都不为true执行代码
}
```

if 语句后面可以跟 else if…else 语句，这种语句可以检测到多种可能的情况。

使用 if，else if，else 语句的时候，需要注意下面几点：

- if 语句至多有 1 个 else 语句，else 语句在所有的 else if 语句之后。
- if 语句可以有若干个 else if 语句，它们必须在 else 语句之前。
- 一旦其中一个 else if 语句检测为 true，其他的 else if 以及 else 语句都将跳过执行。

【演示】我们来改造一下上面的成绩案例，学校根据分数区间分为ABCD四个等级！

```java
public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    
    System.out.print("请输入成绩：");
    int score = scanner.nextInt();
    
    if (score==100){
        System.out.println("恭喜满分");
    }else if (score<100 && score >=90){
        System.out.println("A级");
    }else if (score<90 && score >=80){
        System.out.println("B级");
    }else if (score<80 && score >=70){
        System.out.println("C级");
    }else if (score<70 && score >=60){
        System.out.println("D级");
    }else if (score<60 && score >=0){
        System.out.println("不及格！");
    }else {
        System.out.println("成绩输入不合法！");
    }
    scanner.close();
}
```

我们平时写程序一定要严谨，不然之后修补Bug是一件十分头疼的事情，要在编写代码的时候就把所有的问题都思考清除，再去一个个解决，这才是一个优秀的程序员应该做的事情，多思考，少犯错！

### 4、嵌套的if结构

使用嵌套的 if…else 语句是合法的。也就是说你可以在另一个 if 或者 else if 语句中使用 if 或者 else if 语 句。你可以像 if 语句一样嵌套 else if...else。

```java
if(布尔表达式 1){
    ////如果布尔表达式 1的值为true执行代码
    if(布尔表达式 2){
        ////如果布尔表达式 2的值为true执行代码
    }
}
```

有时候我们在解决某些问题的时候，需要缩小查找范围，需要有层级条件判断，提高效率。比如：我们需要寻找一个数，在1-100之间，我们不知道这个数是多少的情况下，我们最笨的方式就是一个个去对比，看他到底是多少，这会花掉你大量的时间，如果可以利用if嵌套比较，我们可以节省大量的成本，如果你有这个思想，你已经很优秀了，因为很多大量的工程师就在寻找能够快速提高，查找和搜索效率的方式。为此提出了一系列的概念，我们生活在大数据时代，我们需要不断的去思考如何提高效率，或许哪一天，你们想出一个算法，能够将分析数据效率提高，或许你就可以在历史的长河中留下一些痕迹了，当然这是后话。

【记住一点就好，所有的流程控制语句都可以互相嵌套，互不影响！】

### 5、switch多选择结构

多选择结构还有一个实现方式就是switch case 语句。

switch case 语句判断一个变量与一系列值中某个值是否相等，每个值称为一个分支。

```java
switch(expression){
    case value :
        //语句
        break; //可选
    case value :
        //语句
        break; //可选
    //你可以有任意数量的case语句
    default : //可选
        //语句
}
```

switch case 语句有如下规则：

- switch 语句中的变量类型可以是： byte、short、int 或者 char。从 Java SE 7 开始，switch 支持字符串 String 类型了，同时 case 标签必须为字符串常量或字面量。
- switch 语句可以拥有多个 case 语句。每个 case 后面跟一个要比较的值和冒号。
- case 语句中的值的数据类型必须与变量的数据类型相同，而且只能是常量或者字面常量。
- 当变量的值与 case 语句的值相等时，那么 case 语句之后的语句开始执行，直到 break 语句出现才会跳出 switch 语句。
- 当遇到 break 语句时，switch 语句终止。程序跳转到 switch 语句后面的语句执行。case 语句不必须要包含 break 语句。如果没有 break 语句出现，程序会继续执行下一条 case 语句，直到出现 break 语句。
- switch 语句可以包含一个 default 分支，该分支一般是 switch 语句的最后一个分支（可以在任何位置，但建议在最后一个）。default 在没有 case 语句的值和变量值相等的时候执行。default 分支不需要 break 语句。

switch case 执行时，一定会先进行匹配，匹配成功返回当前 case 的值，再根据是否有 break，判断是否继续输出，或是跳出判断。

```java
public static void main(String[] args) {
    char grade = 'C';
    switch (grade) {
        case 'A':
            System.out.println("优秀");
            break;
        case 'B':
            System.out.println("秀");
            break;
        case 'C':
            System.out.println("良好");
            break;
        case 'D':
            System.out.println("及格");
            break;
        case 'F':
            System.out.println("你需要再努力努力");
            break;
        default:
            System.out.println("未知等级");
    }
    System.out.println("你的等级是 " + grade);
}

```

如果 case 语句块中没有 break 语句时，匹配成功后，从当前 case 开始，后续所有 case 的值都会输 出。如果后续的 case 语句块有 break 语句则会跳出判断。

```java
public static void main(String[] args) {
    int i = 1;
    switch (i) {
        case 0:
            System.out.println("0");
        case 1:
            System.out.println("1");
        case 2:
            System.out.println("2");
        case 3:
            System.out.println("3");
            break;
        default:
            System.out.println("default");
    }
}
```

输出：1，2，3。

【JDK7增加了字符串表达式】

case 后边的可以是字符串的表达形式

```java
public static void main(String[] args) {
    String name = "你好";

    switch (name) {
        //JDK7的新特性，表达式结果可以是字符串！！！
        case "你好":
            System.out.println("你好");
            break;
        case "我好":
            System.out.println("我好");
            break;
        default:
            System.out.println("啥都不好");
            break;
    }
}
```
## 循环结构

上面选择结构中，我们始终无法让程序一直跑着，我们每次运行就停止了。我们需要规定一个程序运行多少次，运行多久，等等。所以按照我们编程是为了解决人的问题的思想，我们是不是得需要有一个结构来搞定这个事情！于是循环结构自然的诞生了！

顺序结构的程序语句只能被执行一次。如果您想要同样的操作执行多次,，就需要使用循环结构。

Java中有三种主要的循环结构：

- while 循环
- do…while 循环
- for 循环

在Java5中引入了一种主要用于数组的增强型for循环。

### 1、while 循环

while是最基本的循环，它的结构为：

```java
while( 布尔表达式 ) {
    //循环内容
}
```

![image-20210327220634511](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/image-20210327220634511.png)

【图解】在循环刚开始时，会计算一次“布尔表达式”的值，若条件为真，执行循环体。而对于后来每一 次额外的循环，都会在开始前重新计算一次判断是否为真。直到条件不成立，则循环结束。

我们大多数情况是会让循环停止下来的，我们需要一个让表达式失效的方式来结束循环。

方式有：循环内部控制，外部设立标志位！等

```java
public static void main(String[] args) {
    int i = 0;
    //i小于100就会一直循环
    while (i<100){
        i++;
        System.out.println(i);
    }
}
```

少部分情况需要循环一直执行，比如服务器的请求响应监听等。

```java
public static void main(String[] args) {
    while (true){
        //等待客户端连接
        //定时检查
        //......
    }
}
```

循环条件一直为true就会造成无限循环【死循环】，我们正常的业务编程中应该尽量避免死循环。会影 响程序性能或者造成程序卡死奔溃！

【案例：计算1+2+3+…+100=?】

```java
public static void main(String[] args) {
    int i = 0;
    int sum = 0;
    while (i <= 100) {
        sum = sum+i;
        i++;
    }
    System.out.println("Sum= " + sum);
}
```

【高斯的故事】

德国大数学家高斯（Gauss）：高斯是一对普通夫妇的儿子。他的母亲是一个贫穷石匠的女儿，虽然十分聪明，但却没有接受过教育，近似于文盲。在她成为高斯父亲的第二个妻子之前，她从事女佣工作。他的父亲曾做过园丁，工头，商人的助手和一个小保险公司的评估师。当高斯三岁时便能够纠正他父亲的借债账目的事情， 已经成为一个轶事流传至今。他曾说，他在麦仙翁堆上学会计算。能够在头脑中进行复杂的计算，是上帝赐予他一生的天赋。

高斯用很短的时间计算出了小学老师布置的任务：对自然数从1到100的求和.他所使用的方法是：对50 对构造成和101的数列求和（1＋100,2＋99,3＋98……）,同时得到结果：5050.这一年,高斯9岁.

这个故事我们在高中数学中的“等差数列求和”听过，当时我们用的公式求解。

![img](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/5882b2b7d0a20cf4863461a066094b36acaf992d)

编程难的不是语言，是算法。数学能让你写的程序运算次数更少，效率更高。

如果求1+2+3.....+100万呢，虽然100万次的运算加法，对于计算机不算什么，但我们为了效率可以用数学公式进行求解。

有能力的同学可以看下编程程序比赛，考验算法能力的，例如：“传智杯”，“蓝桥杯”

### 2、do…while 循环

对于 while 语句而言，如果不满足条件，则不能进入循环。但有时候我们需要即使不满足条件，也至少 执行一次。

do…while 循环和 while 循环相似，不同的是，do…while 循环至少会执行一次。

```java
do {
    //代码语句
}while(布尔表达式);
```

![image-20210327222224162](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/image-20210327222224162.png)

注意：布尔表达式在循环体的后面，所以语句块在检测布尔表达式之前已经执行了。 如果布尔表达式的值为 true，则语句块一直执行，直到布尔表达式的值为 false。

我们用do...while改造一下上面的案例！

```java
public static void main(String[] args) {
    int i = 0;
    int sum = 0;
    do {
        sum = sum+i;
        i++;
    }while (i <= 100);
    System.out.println("Sum= " + sum);
}
```

执行结果当然是一样的！

While和do-While的区别：

while先判断后执行。dowhile是先执行后判断！

Do...while总是保证循环体会被至少执行一次！这是他们的主要差别。

```java
public static void main(String[] args) {
    int a = 0;
    while(a<0){
        System.out.println(a);
        a++;
    }
    System.out.println("-----");
    do{
        System.out.println(a);
        a++;
    } while (a<0);
}
```

### 3、For循环

虽然所有循环结构都可以用 while 或者 do...while表示，但 Java 提供了另一种语句 —— for 循环，使一些循环结构变得更加简单。

for循环语句是支持迭代的一种通用结构，是最有效、最灵活的循环结构。

for循环执行的次数是在执行前就确定的。语法格式如下：

```java
for(初始化; 布尔表达式; 更新) {
    //代码语句
}
```

![image-20210327222651145](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-流程控制.assets/image-20210327222651145.png)

关于 for 循环有以下几点说明：

- 最先执行初始化步骤。可以声明一种类型，但可初始化一个或多个循环控制变量，也可以是空语句。
- 然后，检测布尔表达式的值。如果为 true，循环体被执行。如果为false，循环终止，开始执行循环体后面的语句。
- 执行一次循环后，更新循环控制变量(迭代因子控制循环变量的增减。
- 再次检测布尔表达式。循环执行上面的过程。

【演示：while和for输出】

```java
public static void main(String[] args) {
    int a = 1; //初始化
    
    while(a<=100){ //条件判断
        System.out.println(a); //循环体
        a+=2; //迭代
    }
    System.out.println("while循环结束！");
    
    for(int i = 1;i<=100;i++){ //初始化//条件判断 //迭代
        System.out.println(i); //循环体
    }
    System.out.println("while循环结束！");
}
```

我们发现，for循环在知道循环次数的情况下，简化了代码，提高了可读性。我们平时用到的最多的也是 我们的for循环！

### 4、练习

【练习1：计算0到100之间的奇数和偶数的和】

```java
public static void main(String[] args) {
    int oddSum = 0; //用来保存奇数的和
    int evenSum = 0; //用来存放偶数的和
    for (int i = 0; i <= 100; i++) {
        if (i % 2 != 0) {
            oddSum += i;
        } else {
            evenSum += i;
        }
    }
    System.out.println("奇数的和：" + oddSum);
    System.out.println("偶数的和：" + evenSum);
}
```

【练习2：用while或for循环输出1-1000之间能被5整除的数，并且每行输出3个】

```
public static void main(String[] args) {
    for (int j = 1; j <= 1000; j++) {
        if (j % 5 == 0) {
            System.out.print(j + "\t");
        }
        if (j % (5 * 3) == 0) {
            System.out.println();
        }
    }
}
```

【练习3：打印九九乘法表】

```
1*1=1
1*2=2 2*2=4
1*3=3 2*3=6 3*3=9
1*4=4 2*4=8 3*4=12 4*4=16
1*5=5 2*5=10 3*5=15 4*5=20 5*5=25
1*6=6 2*6=12 3*6=18 4*6=24 5*6=30 6*6=36
1*7=7 2*7=14 3*7=21 4*7=28 5*7=35 6*7=42 7*7=49
1*8=8 2*8=16 3*8=24 4*8=32 5*8=40 6*8=48 7*8=56 8*8=64
1*9=9 2*9=18 3*9=27 4*9=36 5*9=45 6*9=54 7*9=63 8*9=72 9*9=81
```

当然，成功的路不止一条，但是我们要追求最完美的一条，如果你做不到，不妨试试笨办法，依旧可以 完成任务！比如一行行输出，也是可以搞定的。一定要多分析！

我们使用嵌套for循环就可以很轻松解决这个问题了！

第一步：我们先打印第一列，这个大家应该都会

```java
for (int i = 1; i <= 9; i++) {
	System.out.println(1 + "*" + i + "=" + (1 * i));
}
```

第二步：我们把固定的1再用一个循环包起来

```java
for (int i = 1; i <= 9 ; i++) {
    for (int j = 1; j <= 9; j++) {
        System.out.println(i + "*" + j + "=" + (i * j));
    }
}
```

第三步：去掉重复项，j<=i

```java
for (int i = 1; i <= 9 ; i++) {
    for (int j = 1; j <= i; j++) {
        System.out.println(j + "*" + i + "=" + (i * j));
    }
}
```

第四步：调整样式

```java
for (int i = 1; i <= 9 ; i++) {
    for (int j = 1; j <= i; j++) {
        System.out.print(j + "*" + i + "=" + (i * j)+ "\t");
    }
    System.out.println();
}
```

通过本练习，大家要体会如何分析问题、如何切入问题！在我们以后写代码的过程中，一定要学会将一 个大问题分解成若干小问题，然后，由易到难，各个击破！这也是我们以后开发项目时的基本思维过程。希望大家好好体会！

### 5、增强for循环

Java5 引入了一种主要用于数组或集合的增强型 for 循环。

Java 增强 for 循环语法格式如下:

```java
for(声明语句 : 表达式)
{
    //代码句子
}
```

声明语句：声明新的局部变量，该变量的类型必须和数组元素的类型匹配。其作用域限定在循环语句 块，其值与此时数组元素的值相等。

表达式：表达式是要访问的数组名，或者是返回值为数组的方法。

【演示：增强for循环遍历输出数组元素】

```java
public static void main(String[] args) {
    
    int [] numbers = {10, 20, 30, 40, 50};
    for(int x : numbers ){
        System.out.print( x );
        System.out.print(",");
    }
    System.out.print("\n");
    
    String [] names ={"James", "Larry", "Tom", "Lacy"};
    for( String name : names ) {
        System.out.print( name );
        System.out.print(",");
    }
}
```

我们现在搞不懂这个没关系，就是拉出来和大家见一面，下章就讲解数组了！

## break & continue

### 1、break 关键字

break 主要用在循环语句或者 switch 语句中，用来跳出整个语句块。

break 跳出最里层的循环，并且继续执行该循环下面的语句。

【演示：跳出循环】

```java
public static void main(String[] args) {
    int i = 0;
    while (i < 100) {
        i++;
        System.out.println(i);
        if (i == 30) {
            break;
        }
    }
}
```

switch 语句中break在上面已经详细说明了

### 2、continue 关键字

continue 适用于任何循环控制结构中。作用是让程序立刻跳转到下一次循环的迭代。

在 for 循环中，continue 语句使程序立即跳转到更新语句。

在 while 或者 do…while 循环中，程序立即跳转到布尔表达式的判断语句。

```java
public static void main(String[] args) {
    int i = 0;
    while (i < 100) {
        i++;
        if (i % 10 == 0) {
            System.out.println();
            continue;
        }
        System.out.print(i);
    }
}
```

### 3、两者区别

break在任何循环语句的主体部分，均可用break控制循环的流程。break用于强行退出循环，不执行循环中剩余的语句。(break语句也在switch语句中使用)

continue 语句用在循环语句体中，用于终止某次循环过程，即跳过循环体中尚未执行的语句，接着进行下一次是否执行循环的判定。

### 4、带标签的continue

【了解即可】

1. goto关键字很早就在程序设计语言中出现。尽管goto仍是Java的一个保留字，但并未在语言中得到正式使用；Java没有goto。然而，在break和continue这两个关键字的身上，我们仍然能看出一些 goto的影子---带标签的break和continue。

2. “标签”是指后面跟一个冒号的标识符，例如：label:

3. 对Java来说唯一用到标签的地方是在循环语句之前。而在循环之前设置标签的唯一理由是：我们希望在其中嵌套另一个循环，由于break和continue关键字通常只中断当前循环，但若随同标签使用，它们就会中断到存在标签的地方。

4. 带标签的break和continue的例子：

   【演示：打印101-150之间所有的质数】

   ```java
   public static void main(String[] args) {
       int count = 0;
       outer: for (int i = 101; i < 150; i ++) {
           for (int j = 2; j < i / 2; j++) {
               if (i % j == 0){
                    continue outer;
               }
           }
           System.out.print(i+ " ");
       }
   }
   ```

【看不懂没关系，只是了解一下即可，知道goto这个保留字和标签的写法】


# JavaSE-方法

## 1、何谓方法？

在前面几个章节中我们经常使用到 System.out.println()，那么它是什么呢？

- println() 是一个方法。
- System 是系统类。
- out 是标准输出对象。 

这句话的用法是调用系统类 System 中的标准输出对象 out 中的方法 println()。

**那么什么是方法呢？**

Java方法是语句的集合，它们在一起执行一个功能。

- 方法是解决一类问题的步骤的有序组合
- 方法包含于类或对象中
- 方法在程序中被创建，在其他地方被引用

设计方法的原则：方法的本意是功能块，就是实现某个功能的语句块的集合。我们设计方法的时候，最 好保持方法的原子性，就是一个方法只完成1个功能，这样利于我们后期的扩展。

**方法的优点**

- 使程序变得更简短而清晰。
- 有利于程序维护。
- 可以提高程序开发的效率。
- 提高了代码的重用性。

回顾：方法的命名规则？

## 2、方法的定义

Java的方法类似于其它语言的函数，是一段用来完成特定功能的代码片段，一般情况下，定义一个方法 包含以下语法：

```
修饰符 返回值类型 方法名(参数类型 参数名){
    ...
    方法体
    ...
    return 返回值;
}
```

方法包含一个方法头和一个方法体。下面是一个方法的所有部分：

- 修饰符

  修饰符，这是可选的，告诉编译器如何调用该方法。定义了该方法的访问类型。

- 返回值类型

  方法可能会返回值。returnValueType 是方法返回值的数据类型。有些方法执行所需 的操作，但没有返回值。在这种情况下，returnValueType 是关键字void。

- 方法名

  是方法的实际名称。方法名和参数表共同构成方法签名。

- 参数类型

  参数像是一个占位符。当方法被调用时，传递值给参数。这个值被称为实参或变量。参数列表是指方法的参数类型、顺序和参数的个数。参数是可选的，方法可以不包含任何参数。

  - 形式参数：在方法被调用时用于接收外界输入的数据。
  - 实参：调用方法时实际传给方法的数据。

  ![image-20210328114438468](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-方法.assets/image-20210328114438468.png)

- 方法体

  方法体包含具体的语句，定义该方法的功能。

比如我们写一个比大小的方法：

【演示】下面的方法包含 2 个参数 num1 和 num2，它返回这两个参数的最大值。

```java
/** 返回两个整型变量数据的较大值 */
public static int max(int num1, int num2) {
    int result;
    if (num1 > num2){
        result = num1;
    }
    else{
        result = num2;
    }
        
    return result;
}
```

【演示：加法】

```java
public int add(int num1, int num2) {
    return num1+num2;
}
```

## 3、方法调用

Java 支持两种调用方法的方式，根据方法是否返回值来选择。

当程序调用一个方法时，程序的控制权交给了被调用的方法。当被调用方法的返回语句执行或者到达方法体闭括号时候交还控制权给程序。

当方法返回一个值的时候，方法调用通常被当做一个值。例如：

```java
int larger = max(30, 40);
```

Java语言中使用下述形式调用方法：对象名.方法名(实参列表)

如果方法返回值是void，方法调用一定是一条语句。例如，方法println返回void。下面的调用是个语句：

```java
System.out.println("Hello,kuangshen!");
```

【演示：定义方法并且调用它】

```java
public static void main(String[] args) {
    int i = 5;
    int j = 2;
    int k = max(i, j);
    System.out.println( i + " 和 " + j + " 比较，最大值是：" + k);
}

/** 返回两个整数变量较大的值 */
public static int max(int num1, int num2) {
    int result;
    if (num1 > num2){
        result = num1;
    }  
    else{
        result = num2;
    }
    return result;
}
```

这个程序包含 main 方法和 max 方法。main 方法是被 JVM 调用的，除此之外，main 方法和其它方法 没什么区别。**JAVA中只有值传递！**

main 方法的头部是不变的，如例子所示，带修饰符 public 和 static,返回 void 类型值，方法名字是 main,此外带个一个 String[] 类型参数。String[] 表明参数是字符串数组。

## 4、方法的重载

上面使用的max方法仅仅适用于int型数据。但如果你想得到两个浮点类型数据的最大值呢？

解决方法是创建另一个有相同名字但参数不同的方法，如下面代码所示：

```java
public static double max(double num1, double num2) {
    if (num1 > num2)
    return num1;
    else
    return num2;
}

public static int max(int num1, int num2) {
    int result;
    if (num1 > num2)
    result = num1;
    else
    result = num2;
    return result;
}
```

如果你调用max方法时传递的是int型参数，则 int型参数的max方法就会被调用；

如果传递的是double型参数，则double类型的max方法体会被调用，这叫做方法重载；

就是说一个类的两个方法拥有相同的名字，但是有不同的参数列表。

Java编译器根据方法签名判断哪个方法应该被调用。

方法重载可以让程序更清晰易读。执行密切相关任务的方法应该使用相同的名字。

重载的方法必须拥有不同的参数列表。你不能仅仅依据修饰符或者返回类型的不同来重载方法。

## 5、拓展命令行传参

有时候你希望运行一个程序时候再传递给它消息。这要靠传递命令行参数给main()函数实现。

命令行参数是在执行程序时候紧跟在程序名字后面的信息。

【下面的程序打印所有的命令行参数】

```java
public class CommandLine {
	public static void main(String args[]){
		for(int i=0; i<args.length; i++){
			System.out.println("args[" + i + "]: " + args[i]);
		}
	}
}
```

【命令行】

```
javac CommandLine.java
java CommandLine this is a command line 200 -100
```

> args[0]: this
> args[1]: is
> args[2]: a
> args[3]: command
> args[4]: line
> args[5]: 200
> args[6]: -100

## 6、可变参数

JDK 1.5 开始，Java支持传递同类型的可变参数给一个方法。

方法的可变参数的声明如下所示：

> typeName... parameterName

在方法声明中，在指定参数类型后加一个省略号(...) 

一个方法中只能指定一个可变参数，它必须是方法的最后一个参数。任何普通的参数必须在它之前声明。

```java
public static void main(String[] args) {
    // 调用可变参数的方法
    printMax(34, 3, 3, 2, 56.5);
    printMax(new double[]{1, 2, 3});
}

public static void printMax(double... numbers) {
    if (numbers.length == 0) {
        System.out.println("No argument passed");
        return;
    }
    double result = numbers[0];
    //排序！
    for (int i = 1; i < numbers.length; i++) {
        if (numbers[i] > result) {
            result = numbers[i];
        }
    }
    System.out.println("The max value is " + result);
}
```

## 7、递归

A方法调用B方法，我们很容易理解！

递归就是：A方法调用A方法！就是自己调用自己，因此我们在设计递归算法时，一定要指明什么时候自己不调用自己。否则，就是个死循环！

**递归算法重点：**

递归是一种常见的解决问题的方法，即把问题逐渐简单化。递归的基本思想就是“自己调用自己”，一个使用递归技术的方法将会直接或者间接的调用自己。

利用递归可以用简单的程序来解决一些复杂的问题。它通常把一个大型复杂的问题层层转化为一个与原 问题相似的规模较小的问题来求解，递归策略只需少量的程序就可描述出解题过程所需要的多次重复计 算，大大地减少了程序的代码量。递归的能力在于用有限的语句来定义对象的无限集合。

递归结构包括两个部分：

- 递归头

  什么时候不调用自身方法。如果没有头，将陷入死循环。

-  递归体

  什么时候需要调用自身方法。

【演示：利用代码计算5的乘阶！】 

```java
//5*4*3*2*1
public static void main(String[] args) {
    System.out.println(f(5));
}
public static int f(int n) {
    if (1 == n)
    	return 1;
    else
    	return n*f(n-1);
}
```

![image-20210328140142727](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-方法.assets/image-20210328140142727.png)

此题中，按照递归的三个条件来分析： 

(1)边界条件：阶乘，乘到最后一个数，即1的时候，返回1，程序执行到底；
(2)递归前进段：当前的参数不等于1的时候，继续调用自身； 
(3)递归返回段：从最大的数开始乘，如果当前参数是5，那么就是5* 4，即5 (5-1)，即n * (n-1)

递归其实是方便了程序员难为了机器，递归可以通过数学公式很方便的转换为程序。其优点就是易理 解，容易编程。但递归是用栈机制实现的，每深入一层，都要占去一块栈数据区域，对嵌套层数深的一 些算法，递归会力不从心，空间上会以内存崩溃而告终，而且递归也带来了大量的函数调用，这也有许 多额外的时间开销。所以在深度大时，它的时空性就不好了。（会占用大量的内存空间）

而迭代虽然效率高，运行时间只因循环次数增加而增加，没什么额外开销，空间上也没有什么增加，但 缺点就是不容易理解，编写复杂问题时困难。

能不用递归就不用递归，递归都可以用迭代来代替


# JavaSE-数组

## 数组概述

关于数组我们可以把它看作是一个类型的所有数据的一个集合，并用一个数组下标来区分或指定每一个数，例如一个足球队通常会有几十个人，但是我们来认识他们的时候首先会把他们看作是某某对的成员，然后再利用他们的号码来区分每一个队员，这时候，球队就是一个数组，而号码就是数组的下标， 当我们指明是几号队员的时候就找到了这个队员。 同样在编程中，如果我们有一组相同数据类型的数据，例如有10个数字，这时候如果我们要用变量来存放它们的话，就要分别使用10个变量，而且要记住这10个变量的名字，这会十分的麻烦，这时候我们就可以用一个数组变量来存放他们，例如在VB中我们 就可以使用dim a(9) as integer（注意：数组的下标是从0开始的，所以第10个数的话，下标就是 9，a(0)=1）。 使用数组会让程序变的简单，而且避免了定义多个变量的麻烦。

数组的定义：

- 数组是相同类型数据的有序集合
- 数组描述的是相同类型的若干个数据,按照一定的先后次序排列组合而成
- 其中,每一个数据称作一个数组元素,每个数组元素可以通过一个下标来访问它们.

**数组的四个基本特点：**

- 其长度是确定的。数组一旦被创建，它的大小就是不可以改变的。
-  其元素必须是相同类型，不允许出现混合类型。
- 数组中的元素可以是任何数据类型，包括基本类型和引用类型。
- 数组变量属引用类型，数组也可以看成是对象，数组中的每个元素相当于该对象的成员变量。数组本身就是对象，Java中对象是在堆中的，因此数组无论保存原始类型还是其他对象类型，数组对象本身是在堆中的。

## 数组声明创建

### 1、声明数组

首先必须声明数组变量，才能在程序中使用数组。下面是声明数组变量的语法：

```java
dataType[] arrayRefVar; // 首选的方法

dataType arrayRefVar[]; // 效果相同，但不是首选方法
```

建议使用 dataType[] arrayRefVar 的声明风格声明数组变量。 
dataType arrayRefVar[] 风格是来自 C/C++ 语言 ，在Java中采用是为了让 C/C++ 程序员能够快速理解java语言。

```java
double[] myList; // 首选的方法
double myList[]; // 效果相同，但不是首选方法
```

### 2、创建数组

Java语言使用new操作符来创建数组，语法如下：

```java
arrayRefVar = new dataType[arraySize];
```

上面的语法语句做了两件事：

- 使用 dataType[arraySize] 创建了一个数组。
- 把新创建的数组的引用赋值给变量 arrayRefVar。

数组变量的声明，和创建数组可以用一条语句完成，如下所示：

```java
dataType[] arrayRefVar = new dataType[arraySize];
//例如，创建一个类型ini，大小为10的数组
int[] myList =  new int[10];
```

获取数组长度：arrayRefVar.length

数组的元素是通过索引访问的。数组索引从 0 开始，所以索引值从 0 到 arrayRefVar.length-1

【演示创建一个数组，并赋值，进行访问】

```java
public static void main(String[] args) {
    //1.声明一个数组
    int[] myList = null;
    //2.创建一个数组
    myList = new int[10];
    //3.像数组中存值
    myList[0] = 1;
    myList[1] = 2;
    myList[2] = 3;
    myList[3] = 4;
    myList[4] = 5;
    myList[5] = 6;
    myList[6] = 7;
    myList[7] = 8;
    myList[8] = 9;
    myList[9] = 10;
    // 计算所有元素的总和
    double total = 0;
    for (int i = 0; i < myList.length; i++) {
        total += myList[i];
    }
    System.out.println("总和为： " + total);
}
```

### 3、内存分析

Java内存分析 ：

![image-20210328141316453](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-数组.assets/image-20210328141316453.png)

1. 声明的时候并没有实例化任何对象，只有在实例化数组对象时，JVM才分配空间，这时才与长度有关。因此，声明数组时不能指定其长度(数组中元素的个数)

   例如： int a[5]; //非法

2. 声明一个数组的时候并没有数组被真正的创建。

3.  构造一个数组，必须指定长度

```java
//1.声明一个数组
int[] myList = null;
```

![image-20210328141500346](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-数组.assets/image-20210328141500346.png)

```java
//2.创建一个数组
myList = new int[10];
```

![image-20210328141525203](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-数组.assets/image-20210328141525203.png)

```java
//3.像数组中存值
myList[0] = 1;
myList[1] = 2;
myList[2] = 3;
myList[3] = 4;
myList[4] = 5;
myList[5] = 6;
myList[6] = 7;
myList[7] = 8;
myList[8] = 9;
myList[9] = 10;
```

![image-20210328141543324](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-数组.assets/image-20210328141543324.png)

### 4、三种初始化

1、静态初始化

除了用new关键字来产生数组以外,还可以直接在定义数组的同时就为数组元素分配空间并赋值。

```java
int[] a = {1,2,3};
Man[] mans = {new Man(1,1),new Man(2,2)};
```

2、动态初始化

数组定义、为数组元素分配空间、赋值的操作、分开进行。

```java
int[] a = new int[2];
a[0]=1;
a[1]=2;
```

3、数组的默认初始化

数组是引用类型，它的元素相当于类的实例变量，因此数组一经分配空间，其中的每个元素也被按照实例变量同样的方式被隐式初始化。

```java
public static void main(String[] args) {
    int[] a=new int[2];
    boolean[] b = new boolean[2];
    String[] s = new String[2];
    System.out.println(a[0]+":"+a[1]); //0,0
    System.out.println(b[0]+":"+b[1]); //false,false
    System.out.println(s[0]+":"+s[1]); //null, null
}
```

### 5、数组边界

下标的合法区间：[0, length-1]，如果越界就会报错；

```java
public static void main(String[] args) {
    int[] a=new int[2];
    System.out.println(a[2]);
}
```

> Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException: 2

ArrayIndexOutOfBoundsException : 数组下标越界异常！

### 6、小结

数组是相同数据类型(数据类型可以为任意类型)的有序集合

数组也是对象。数组元素相当于对象的成员变量(详情请见内存图)

数组长度的确定的，不可变的。如果越界，则报：ArrayIndexOutofBounds



## 数组使用

数组的元素类型和数组的大小都是确定的，所以当处理数组元素时候，我们通常使用基本循环或者 ForEach 循环。

【该实例完整地展示了如何创建、初始化和操纵数组】

```java
public static void main(String[] args) {
    double[] myList = {1.9, 2.9, 3.4, 3.5};
    // 打印所有数组元素
    for (int i = 0; i < myList.length; i++) {
        System.out.println(myList[i] + " ");
    }
    // 计算所有元素的总和
    double total = 0;
    for (int i = 0; i < myList.length; i++) {
        total += myList[i];
    }
    System.out.println("Total is " + total);
    // 查找最大元素
    double max = myList[0];
    for (int i = 1; i < myList.length; i++) {
        if (myList[i] > max) {
            max = myList[i];
        }
    }
    System.out.println("Max is " + max);

}
```

### 1、For-Each 循环

JDK 1.5 引进了一种新的循环类型，被称为 For-Each 循环或者加强型循环，它能在不使用下标的情况下遍历数组。

```java
for(type element: array){
    System.out.println(element);
}
```

【示例】

```java
public static void main(String[] args) {
    double[] myList = {1.9, 2.9, 3.4, 3.5};
    
    // 打印所有数组元素
    for (double element: myList) {
        System.out.println(element);
    }
}
```

### 2、数组作方法入参

数组可以作为参数传递给方法。

例如，下面的例子就是一个打印 int 数组中元素的方法 :

```java
public static void printArray(int[] array) {
    for (int i = 0; i < array.length; i++) {
        System.out.print(array[i] + " ");
    }
}
```

### 3、数组作返回值

```java
public static int[] reverse(int[] list) {
    int[] result = new int[list.length];
    
    for (int i = 0, j = result.length - 1; i < list.length; i++, j--) {
        result[j] = list[i];
    }
    return result;
}
```

以上实例中 result 数组作为函数的返回值。

## 多维数组

多维数组可以看成是数组的数组，比如二维数组就是一个特殊的一维数组，其每一个元素都是一个一维数组。

**1、多维数组的动态初始化：（以二维数组为例）**

直接为每一维分配空间，格式如下：

```java
type[][] typeName = new type[typeLength1][typeLength2];
```



type 可以为基本数据类型和复合数据类型，arraylenght1 和 arraylenght2 必须为正整数， arraylenght1 为行数，arraylenght2 为列数。

比如定义一个二维数组：

```java
int a[][] = new int[2][5];
```

解析：二维数组 a 可以看成一个两行三列的数组。

**2、多维数组的引用（以二维数组为例）**

对二维数组中的每个元素，引用方式为 arrayName[index1] [index2]，例如：

> num[1] [0];

其实二维甚至多维数组十分好理解，我们把两个或者多个值当做定位就好。

原来的数组就是一条线，我们知道一个位置就好

二维就是一个面，两点确定一个位置

三维呢，就需要三个点来确定

**3、获取数组长度：**

a.length获取的二维数组第一维数组的长度，a[0].length才是获取第二维第一个数组长度。

## Arrays 类

数组的工具类java.util.Arrays

由于数组对象本身并没有什么方法可以供我们调用,但API中提供了一个工具类Arrays供我们使用,从 而可以对数据对象进行一些基本的操作。

**文档简介：**

​	![image-20210328143104527](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-数组.assets/image-20210328143104527.png)

这个文档，百度即可下载：jdk1.8中文文档

Arrays类中的方法都是static修饰的静态方法,在使用的时候可以直接使用类名进行调用，而"不用"使用对象来调用(注意：是"不用" 而不是 "不能")

java.util.Arrays 类能方便地操作数组. 使用之前需要导包！

具有以下常用功能：

- 给数组赋值：通过 fill 方法。
- 对数组排序：通过 sort 方法,按升序。
- 比较数组：通过 equals 方法比较数组中元素值是否相等。
- 查找数组元素：通过 binarySearch 方法能对排序好的数组进行二分查找法操作。

具体说明请查看下表：

| 序号 | 方法和说明                                                   |
| :--- | :----------------------------------------------------------- |
| 1    | **public static int binarySearch(Object[] a, Object key)** 用二分查找算法在给定数组中搜索给定值的对象(Byte,Int,double等)。数组在调用前必须排序好的。如果查找值包含在数组中，则返回搜索键的索引；否则返回 (-(*插入点*) - 1)。 |
| 2    | **public static boolean equals(long[] a, long[] a2)** 如果两个指定的 long 型数组彼此*相等*，则返回 true。如果两个数组包含相同数量的元素，并且两个数组中的所有相应元素对都是相等的，则认为这两个数组是相等的。换句话说，如果两个数组以相同顺序包含相同的元素，则两个数组是相等的。同样的方法适用于所有的其他基本数据类型（Byte，short，Int等）。 |
| 3    | **public static void fill(int[] a, int val)** 将指定的 int 值分配给指定 int 型数组指定范围中的每个元素。同样的方法适用于所有的其他基本数据类型（Byte，short，Int等）。 |
| 4    | **public static void sort(Object[] a)** 对指定对象数组根据其元素的自然顺序进行升序排列。同样的方法适用于所有的其他基本数据类型（Byte，short，Int等）。 |

来源[菜鸟教程](https://www.runoob.com/java/java-array.html)，一个编程的基础技术教程网站，适合初学者查看资料，我PHP基础就是在这里学的。

### 1、打印数组

```	java
public static void main(String[] args) {
    int[] a = {1,2};
    System.out.println(a); //[I@1b6d3586
    System.out.println(Arrays.toString(a)); //[1, 2]
}
```

### 2、数组排序

对指定的 int 型数组按数字升序进行排序

```java
public static void main(String[] args) {
    int[] a = {1,2,323,23,543,12,59};
    System.out.println(Arrays.toString(a));
    Arrays.sort(a);
    System.out.println(Arrays.toString(a));
}
```

### 3、二分法查找

在数组中查找指定元素并返回其下标

注意：使用二分搜索法来搜索指定的数组，以获得指定的值。必须在进行此调用之前对数组进行排序(通过sort方法等)。如果没有对数组进行排序，则结果是不确定的。

如果数组包含多个带有指定值的元素，则无法保证找到的是哪一个。

```java
public static void main(String[] args) {
    int[] a = {1,2,323,23,543,12,59};
    Arrays.sort(a); //使用二分法查找，必须先对数组进行排序
    System.out.println("该元素的索引："+Arrays.binarySearch(a, 12));
}
```

### 4、元素填充

```java
public static void main(String[] args) {
    int[] a = {1,2,323,23,543,12,59};
    Arrays.sort(a); //使用二分法查找，必须先对数组进行排序
    Arrays.fill(a, 2, 4, 100); //将2到4索引的元素替换为100
    System.out.println(Arrays.toString(a));//[1, 2, 100, 100, 59, 323, 543]
}
```

### 5、数组转换为List集合

```java
int[] a = {3,5,1,9,7};
List<int[]> list = Arrays.asList(a);
```

我们写代码的时候，可以不用刻意去记住`List<int[]>` 在idea中，输入`Arrays.asList(a);` 按下alt + 回车键，会自动补全全面的信息，非常方便。

学校中教学一般用的是eclipse，别问为啥，问就是这个免费，idea要钱。想用的小伙伴自行百度解决:muscle:，学计算机的人，pojie版的资源找不到就说不过去了。:blush:

## 常见排序算法

### 1、冒泡排序

冒泡排序（Bubble Sort），是一种计算机科学领域的较简单的排序算法。

它重复地走访过要排序的元素列，依次比较两个相邻的[元素](https://baike.baidu.com/item/元素/9563223)，如果顺序（如从大到小、首字母从Z到A）错误就把他们交换过来。走访元素的工作是重复地进行直到没有相邻元素需要交换，也就是说该元素列已经排序完成。

这个算法的名字由来是因为越小的元素会经由交换慢慢“浮”到数列的顶端（升序或降序排列），就如同碳酸饮料中[二氧化碳](https://baike.baidu.com/item/二氧化碳/349143)的气泡最终会上浮到顶端一样，故名“冒泡排序”。

冒泡排序算法的原理如下：

- 比较相邻的元素。如果第一个比第二个大，就交换他们两个。
- 对每一对相邻元素做同样的工作，从开始第一对到结尾的最后一对。在这一点，最后的元素应该会是最大的数
- 针对所有的元素重复以上的步骤，除了最后一个。
- 持续每次对越来越少的元素重复上面的步骤，直到没有任何一对数字需要比较。

 [冒泡排序——《图解算法》](https://blog.csdn.net/zcl_love_wx/article/details/83576962)

```java
class Bubble {
    public int[] sort(int[] array) {
        int temp = 0;
        // 外层循环，它决定一共走几趟 //-1为了防止溢出
        for (int i = 0; i < array.length - 1; i++) {
            int flag = 0; //通过符号位可以减少无谓的比较，如果已经有序了，就退出循环
            //内层循环，它决定每趟走一次
            for (int j = 0; j < array.length - i - 1; j++) {
                //如果后一个大于前一个,则换位
                if (array[j + 1] > array[j]) {
                    temp = array[j];
                    array[j] = array[j + 1];
                    array[j + 1] = temp;
                    flag = 1;
                }
            }
            if (flag == 0) {
                break;
            }
        }
        return array;
    }

    public static void main(String[] args) {
        Bubble bubble = new Bubble();
        int[] array = {2, 5, 1, 6, 4, 9, 8, 5, 3, 1, 2, 0};
        int[] sort = bubble.sort(array);
        for (int num : sort) {
            System.out.print(num + "\t");
        }
    }
}
```

### 2、选择排序

选择排序（Selection sort）是一种简单直观的排序算法。它的工作原理是每一次从待排序的数据元素中
选出最小（或最大）的一个元素，存放在序列的起始位置，然后，再从剩余未排序元素中继续寻找最小
（大）元素，然后放到排序序列的末尾。以此类推，直到全部待排序的数据元素排完。 选择排序是不稳
定的排序方法。

```java
class SelectSort {
    public int[] sort(int arr[]) {
        int temp = 0;
        for (int i = 0; i < arr.length - 1; i++) {
            // 认为目前的数就是最小的, 记录最小数的下标
            int minIndex = i;
            for (int j = i + 1; j < arr.length; j++) {
                if (arr[minIndex] > arr[j]) {// 修改最小值的下标
                    minIndex = j;
                }
            }// 当退出for就找到这次的最小值,就需要交换位置了
            if (i != minIndex) {//交换当前值和找到的最小值的位置
                temp = arr[i];
                arr[i] = arr[minIndex];
                arr[minIndex] = temp;
            }
        }
        return arr;
    }

    public static void main(String[] args) {
        SelectSort selectSort = new SelectSort();
        int[] array = {2, 5, 1, 6, 4, 9, 8, 5, 3, 1, 2, 0};
        int[] sort = selectSort.sort(array);
        for (int num : sort) {
            System.out.print(num + "\t");
        }
    }
}
```

###  3、直接插入排序

排序原理：基本操作是将一条记录插入到已排好的有序表中，从而得到一个新的、记录数量增1的有序表。

例如：

```txt
原始数据： 49,38,65,97,76,13,27

[49],38,65,97,76,13,27 从1索引开始插入
[38,49],65,97,76,13,27
[38,49,65],97,76,13,27
[38,49,65,97],76,13,27
[38,49,65,76,97],13,27
[13,38,49,65,76,97],27
[13,27,38,49,65,76,97]
```

代码实现：

```java
int arr[]={49,38,65,97,76,13,27};
for (int i = 1; i < arr.length; i++) {
    for(int j=i; j>0;j--){
        if(arr[j]<arr[j-1]){
            int f=arr[j];
            arr[j]=arr[j-1];
            arr[j-1]=f;
        }
    }
}
System.out.println(Arrays.toString(arr));
```

### 4、希尔排序

### 5、快速排序

### 6、归并排序

### 7、基数排序

### 8、堆排序

##  稀疏数组

https://blog.csdn.net/baolingye/article/details/99943083


# JavaSE-异常机制

## 异常概念

在我们日常生活中，有时会出现各种各样的异常。例如：职工小王开车去上班，在正常情况下，小王会准时到达单位。但是天有不测风云，在小王去上班时，可能会遇到一些异常情况，比如小王的车子出了故障，小王只能改为步行。

实际工作中，遇到的情况不可能是非常完美的。比如：你写的某个模块，用户输入不一定符合你的要求、你的程序要打开某个文件，这个文件可能不存在或者文件格式不对，你要读取数据库的数据，数据可能是空的等。我们的程序再跑着，内存或硬盘可能满了。等等。

软件程序在运行过程中，非常可能遇到刚刚提到的这些异常问题，我们叫**异常**，英文是：`Exception`， 意思是例外。这些，例外情况，或者叫异常，怎么让我们写的程序做出合理的处理。而不至于程序崩溃。

**异常**：指程序运行中出现的不期而至的各种状况，如:文件找不到、网络连接失败、非法参数等。 异常发生在程序运行期间，它影响了正常的程序执行流程。

比如说，你的代码少了一个分号，那么运行出来结果是提示是错误 `java.lang.Error` ；

如果你用 `System.out.println(11/0)` ，因为你用0做了除数，会抛出 `java.lang.ArithmeticException` 的异常。

异常发生的原因有很多，通常包含以下几大类：

- 用户输入了非法数据。
- 要打开的文件不存在。
- 网络通信时连接中断，或者JVM内存溢出。

这些异常有的是因为用户错误引起，有的是程序错误引起的，还有其它一些是因为物理错误引起的。

要理解Java异常处理是如何工作的，你需要掌握以下三种类型的异常：

- **检查性异常**：

  最具代表的检查性异常是用户错误或问题引起的异常，这是程序员无法预见的。例如，要打开一个不存在文件时，一个异常就发生了，这些异常在编译时不能被简单地忽略。

- **运行时异常：**

  运行时异常是可能被程序员避免的异常。与检查性异常相反，运行时异常可以在编译时被忽略。

- **错误：**

  错误不是异常，而是脱离程序员控制的问题。错误在代码中通常被忽略。例如，当栈溢出 时，一个错误就发生了，它们在编译也检查不到的。

异常指不期而至的各种状况，如：文件找不到、网络连接失败、除0操作、非法参数等。异常是一个 事件，它发生在程序运行期间，干扰了正常的指令流程。

Java语言在设计的当初就考虑到这些问题，提出异常处理的框架的方案，所有的异常都可以用一个 异常类 来表示，不同类型的异常对应不同的子类异常（目前我们所说的异常包括错误概念），定义异常处理的规范，在 **JDK1.4** 版本以后增加了异常链机制，从而便于跟踪异常。

Java异常是一个描述在代码段中发生异常的对象，当发生异常情况时，一个代表该异常的对象被创建并且在导致该异常的方法中被抛出，而该方法可以选择自己处理异常或者传递该异常。

## 异常体系结构

Java把异常当作对象来处理，并定义一个基类 `java.lang.Throwable`作为所有异常的超类。

在Java API中已经定义了许多异常类，这些异常类分为两大类，错误**Error**和异常**Exception**。

Java异常层次结构图：

![image-20210329151713728](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-异常机制.assets/image-20210329151713728.png)

从图中可以看出所有异常类型都是内置类 `Throwable` 的子类，因而 `Throwable` 在异常类的层次结构的顶层。

接下来 `Throwable` 分成了两个不同的分支，一个分支是`Error`，它表示不希望被程序捕获或者是程序无法处理的错误。另一个分支是`Exception`，它表示用户程序可能捕捉的异常情况或者说是程序可以处理的异常。

其中异常类 `Exception` 又分为运行时异常( `RuntimeException` )和非运行时异常。Java异常又可以分为不受检查异常（ `Unchecked Exception` ）和检查异常（ `Checked Exception` ）。

## 异常之间的区别与联系

### 1、Error

`Error` 类对象由 Java 虚拟机生成并抛出，大多数错误与代码编写者所执行的操作无关。

比如说：

Java虚拟机运行错误（ `Virtual MachineError` ），当JVM不再有继续执行操作所需的内存资源时， 将出现 `OutOfMemoryError` 。这些异常发生时，Java虚拟机（JVM）一般会选择线程终止；

还有发生在虚拟机试图执行应用时，如类定义错误（ `NoClassDefFoundError` )、链接错误 (`LinkageError `) 
这些错误是不可查的，因为它们在应用程序的控制和处理能力之外，而且绝大多数是程序运行时不允许出现的状况。

对于设计合理的应用程序来说，即使确实发生了错误，本质上也不应该试图去处理它所引起的异常状 况。在Java中，错误通常是使用 Error 的子类描述。

### 2、Exception

在 `Exception` 分支中有一个重要的子类` RuntimeException` （运行时异常），该类型的异常自动为你所编写的程序定义 `ArrayIndexOutOfBoundsException` （数组下标越界）、 `NullPointerException` （空指针异常）、`ArithmeticException` （算术异常）、 `MissingResourceException` （丢失资源）、 `ClassNotFoundException` （找不到类）等异常，这些异常是不检查异常，程序中可以选择捕获处 理，也可以不处理。

这些异常一般是由程序逻辑错误引起的，程序应该从逻辑角度尽可能避免这类异常的发生；而 `RuntimeException` 之外的异常我们统称为非运行时异常，类型上属于 `Exception` 类及其子类，

从程序语法角度讲是必须进行处理的异常，如果不处理，程序就不能编译通过。如 `IOException` 、 `SQLException` 等以及用户自定义的 `Exception` 异常，一般情况下不自定义检查异常。

注意： `Error` 和 `Exception` 的区别： `Error` 通常是灾难性的致命的错误，是程序无法控制和处理的，当出现这些异常时，Java虚拟机（JVM）一般会选择终止线程； `Exception` 通常情况下是可以被程序处理的，并且在程序中应该尽可能的去处理这些异常。

### 3、检查异常和不受检查异常

**检查异常**：在正确的程序运行过程中，很容易出现的、情理可容的异常状况，在一定程度上这种异常的发生是可以预测的，并且一旦发生该种异常，就必须采取某种方式进行处理。

解析：除了`RuntimeException`及其子类以外，其他的`Exception`类及其子类都属于检查异常，当程序中可能出现这类异常，要么使用try-catch语句进行捕获，要么用throws子句抛出，否则编译无法通过。

**不受检查异常**：包括`RuntimeException`及其子类和`Error`。

分析： **不受检查异常** 为编译器不要求强制处理的异常， **检查异常** 则是编译器要求必须处置的异常。

## Java异常处理机制

java异常处理本质：抛出异常和捕获异常

### 1、抛出异常

要理解抛出异常，首先要明白什么是异常情形（exception condition），它是指阻止当前方法或作用域继续执行的问题。其次把异常情形和普通问题相区分，普通问题是指在当前环境下能得到足够的信息， 总能处理这个错误。

对于异常情形，已经无法继续下去了，因为在当前环境下无法获得必要的信息来解决问题，你所能做的就是从当前环境中跳出，并把问题提交给上一级环境，这就是抛出异常时所发生的事情。抛出异常后，会有几件事随之发生。

首先，是像创建普通的java对象一样将使用 new 在堆上创建一个异常对象；然后，当前的执行路径 （已经无法继续下去了）被终止，并且从当前环境中弹出对异常对象的引用。此时，异常处理机制接管程序，并开始寻找一个恰当的地方继续执行程序

这个恰当的地方就是异常处理程序或者异常处理器，它的任务是将程序从错误状态中恢复，以使程序要 么换一种方式运行，要么继续运行下去。

举例：

假使我们创建了一个学生对象Student的一个引用stu，在调用的时候可能还没有初始化。所以在使用这个对象引用调用其他方法之前，要先对它进行检查，可以创建一个代表错误信息的对象，并且将它从当前环境中抛出，这样就把错误信息传播到更大的环境中。

```java
if(stu == null){
    throw new NullPointerException();
}
```

### 2、捕获异常

在方法抛出异常之后，运行时系统将转为寻找合适的异常处理器（exception handler）。潜在的异常处理器是异常发生时依次存留在调用栈中的方法的集合。当异常处理器所能处理的异常类型与方法抛出的异常类型相符时，即为合适的异常处理器。运行时系统从发生异常的方法开始，依次回查调用栈中的方法，直至找到含有合适异常处理器的方法并执行。当运行时系统遍历调用栈而未找到合适的异常处理器，则运行时系统终止。同时，意味着Java程序的终止。

注意：

对于 运行时异常 、错误 和 检查异常 ，Java技术所要求的异常处理方式有所不同。

由于运行时异常及其子类的不可查性，为了更合理、更容易地实现应用程序，Java规定，运行时异常将由Java运行时系统自动抛出，允许应用程序忽略运行时异常。

对于方法运行中可能出现的`Error` ，当运行方法不欲捕捉时，Java允许该方法不做任何抛出声明。因为，大多数 `Error` 异常属于永远不能被允许发生的状况，也属于合理的应用程序不该捕捉的异常。

> 对于所有的检查异常，Java规定：一个方法必须捕捉，或者声明抛出方法之外。也就是说，当一个方法选择不捕捉检查异常时，它必须声明将抛出异常。

### 3、异常处理五个关键字

分别是： `try` 、 `catch` 、 `finally` 、 `throw` 、 `throws`

try ：用于监听。将要被监听的代码（可能抛出异常的代码）放在try语句块之内，当try语句块内发生异常时，异常就被抛出。

catch ： 用于捕获异常。catch用来捕获try语句块中发生的异常。

finally ：finally语句块总是会被执行。它主要用于回收在try块里打开的物力资源（如数据库连接、网络 连接和磁盘文件）。只有finally块，执行完成之后，才会回来执行try或者catch块中的return或者throw语 句，如果finally中使用了return或者throw等终止方法的语句，则就不会跳回执行，直接停止。

throw ： 用于抛出异常。

throws ： 用在方法签名中，用于声明该方法可能抛出的异常。

## 处理异常

### 1、try -catch

```java
try{
	//code that might generate exceptions
}catch(Exception e){
	//the code of handling exception1
}catch(Exception e){
	//the code of handling exception2
}
```

要明白异常捕获，还要理解 监控区域 （guarded region）的概念。它是一段可能产生异常的代码， 并且后面跟着处理这些异常的代码。

因而可知，上述 `try-catch` 所描述的即是监控区域，关键词 `try`后的一对大括号将一块可能发生异常的代码包起来，即为监控区域。Java方法在运行过程中发生了异常，则创建异常对象。

将异常抛出监控区域之外，由Java运行时系统负责寻找匹配的 catch 子句来捕获异常。若有一个 catch 语句匹配到了，则执行该 catch 块中的异常处理代码，就不再尝试匹配别的 catch 块 了。

匹配原则：如果抛出的异常对象属于 catch 子句的异常类，或者属于该异常类的子类，则认为生成的异常对象与 catch 块捕获的异常类型相匹配。

【演示】

```java
public class TestException {
    public static void main(String[] args) {
        int a = 1;
        int b = 0;
        try { // try监控区域
            if (b == 0) throw new ArithmeticException(); // 通过throw语句抛出
            异常
            System.out.println("a/b的值是：" + a / b);
            System.out.println("this will not be printed!");
        }
        catch (ArithmeticException e) { // catch捕捉异常
            System.out.println("程序出现异常，变量b不能为0！");
        }
        System.out.println("程序正常结束。");
    }
}
```

> 输出：
>
> 程序出现异常，变量b不能为0！ 
> 程序正常结束。

注意：显示一个异常的描述， `Throwable` 重载了 `toString( )` 方法（由 Object 定义），所以 它将返回一个包含异常描述的字符串。例如，将前面的 `catch` 块重写成：

```java
catch (ArithmeticException e) { // catch捕捉异常
    System.out.println("程序出现异常" + e);
}
//输出
// 程序出现异常java.lang.ArithmeticException
```

算术异常属于运行时异常，因而实际上该异常不需要程序抛出，运行时系统自动抛出。如果不用try-catch程序就不会往下执行了。

【演示】

```java
public class TestException {
    public static void main(String[] args) {
        int a = 1;
        int b = 0;
        System.out.println("a/b的值是：" + a / b);
        System.out.println("this will not be printed!");
    }
}
/*
结果：
Exception in thread "main" java.lang.ArithmeticException: / by zero
at TestException.main(TestException.java:7)
*/
```

**使用多重的catch语句**：很多情况下，由单个的代码段可能引起多个异常。处理这种情况，我们需要定义两个或者更多的 catch 子句，每个子句捕获一种类型的异常，当异常被引发时，每个 catch 子 句被依次检查，第一个匹配异常类型的子句执行，当一个 catch 子句执行以后，其他的子句将被旁路。

编写多重catch语句块注意事项：

顺序问题：先小后大，即先子类后父类

**注意：**

Java通过异常类描述异常类型。对于有多个 catch 子句的异常程序而言，应该尽量将捕获底层异常类的 catch 子句放在前面，同时尽量将捕获相对高层的异常类的 catch 子句放在后面。否则，捕获 底层异常类的 catch 子句将可能会被屏蔽。

**嵌套try语句**： try 语句可以被嵌套。也就是说，一个 try 语句可以在另一个 try 块的内部。每次进入 try 语句，异常的前后关系都会被推入堆栈。如果一个内部的 try 语句不含特殊异常的 catch 处理程序，堆栈将弹出，下一个 try 语句的 catch 处理程序将检查是否与之匹配。这个 过程将继续直到一个 catch 语句被匹配成功，或者是直到所有的嵌套 try 语句被检查完毕。如果没有 catch 语句匹配，Java运行时系统将处理这个异常。

【演示】

```java
public class NestTry {
    public static void main(String[] args) {
        try {
            int a = args.length;
            int b = 42 / a;
            System.out.println("a = " + a);
            try {
                if (a == 1) {
                    a = a / (a - a);
                }
                if (a == 2) {
                    int c[] = {1};
                    c[42] = 99;
                }
            } catch (ArrayIndexOutOfBoundsException e) {
                System.out.println("ArrayIndexOutOfBounds :" + e);
            }
        } catch (ArithmeticException e) {
            System.out.println("Divide by 0" + e);
        }
    }
}
```

> 分析运行：
>
> javac NestTry.java
>
> java NestTry one
> a = 1
> Divide by 0java.lang.ArithmeticException: / by zero
>
> java NestTry one two
> a = 2
> ArrayIndexOutOfBounds :java.lang.ArrayIndexOutOfBoundsException: 42

分析：正如程序中所显示的，该程序在一个try块中嵌套了另一个 try 块。程序工作如下：当你在没有命令行参数的情况下执行该程序，外面的 try 块将产生一个被0除的异常。

程序在有一个命令行参数条件下执行，由嵌套的 try 块产生一个被0除的异常，由于内部的 catch 块不匹配这个异常，它将把异常传给外部的 try 块，在外部异常被处理。如果你在具有两个命令行参数的条件下执行该程序，将由内部 try 块产生一个数组边界异常。

**注意**：当有方法调用时， try 语句的嵌套可以很隐蔽的发生。例如，我们可以将对方法的调用放在一 个 try 块中。在该方法的内部，有另一个 try 语句。

在这种情况下，方法内部的 try 仍然是嵌套在外部调用该方法的 try 块中的。下面我们将对上述例子进行修改，嵌套的 try 块移到方法nesttry()的内部：结果依旧相同！

```java
public class NestTry {
    static void nesttry(int a) {
        try {
            if (a == 1) {
                a = a / (a - a);
            }
            if (a == 2) {
                int c[] = {1};
                c[42] = 99;
            }
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("ArrayIndexOutOfBounds :" + e);
        }
    }

    public static void main(String[] args) {
        try {
            int a = args.length;
            int b = 42 / a;
            System.out.println("a = " + a);
            nesttry(a);
        } catch (ArithmeticException e) {
            System.out.println("Divide by 0" + e);
        }
    }
}
```

### 2、thorw

到目前为止，我们只是获取了被Java运行时系统引发的异常。然而，我们还可以用`throw`语句抛出明确的异常。

语法形式：**throw ThrowableInstance;**

这里的ThrowableInstance一定是 Throwable 类类型或者 Throwable 子类类型的一个对象。简单的数据类型，例如 int ,char 以及非 Throwable 类，例如 String 或 Object ，不能用作异常。

有两种方法可以获取 Throwable 对象：在 catch 子句中使用参数或者使用 new 操作符创建。程序执行完 throw 语句之后立即停止；throw 后面的任何语句不被执行，最邻近的 try 块用来检 查它是否含有一个与异常类型匹配的 catch 语句。

如果发现了匹配的块，控制转向该语句；如果没有发现，次包围的 try 块来检查，以此类推。如果没有发现匹配的 catch 块，默认异常处理程序中断程序的执行并且打印堆栈轨迹。

```java
class TestThrow {
    static void proc() {
        try {
            throw new NullPointerException("demo");
        } catch (NullPointerException e) {
            System.out.println("Caught inside proc");
            throw e;
        }
    }

    public static void main(String[] args) {
        try {
            proc();
        } catch (NullPointerException e) {
            System.out.println("Recaught: " + e);
        }
    }
}
```

该程序两次处理相同的错误，首先， main() 方法设立了一个异常关系然后调用proc( )。proc( )方法设立了另一个异常处理关系并且立即抛出一个 `NullPointerException` 实例，`NullPointerException` 在 main() 中被再次捕获。

该程序阐述了怎样创建Java的标准异常对象，特别注意这一行：

```java
throw new NullPointerException("demo");
```

分析：此处 new 用来构造一个 `NullPointerException` 实例，所有的Java内置的运行时异常有两个构造方法：一个没有参数，一个带有一个字符串参数。

当用第二种形式时，参数指定描述异常的字符串。如果对象用作 print( ) 或者 println( ) 的参数 时，该字符串被显示。这同样可以通过调用getMessage( )来实现，getMessage( )是由 Throwable 定义的。

### 3、throws

如果一个方法可以导致一个异常但不处理它，它必须指定这种行为以使方法的调用者可以保护它们自己而不发生异常。要做到这点，我们可以在方法声明中包含一个 `throws` 子句。

一个 throws 子句列举了一个方法可能引发的所有异常类型。这对于除了 Error 或 RuntimeException 及它们子类以外类型的所有异常是必要的。一个方法可以引发的所有其他类型的异常必须在 throws 子句中声明，否则会导致编译错误。

```java
public void info() throws Exception
{
    //body of method
}
```

 Exception 是该方法可能引发的所有的异常，也可以是异常列表，中间以逗号隔开。

【例子】

```java
class TestThrows{
    static void throw1(){
        System.out.println("Inside throw1 . ");
        throw new IllegalAccessException("demo");
    }
    
    public static void main(String[] args){
        throw1();
    }
}
```

上述例子中有两个地方存在错误，你看出来了吗？

该例子中存在两个错误，首先，throw1( )方法不想处理所导致的异常，因而它必须声明 throws 子句 来列举可能引发的异常即 IllegalAccessException ；其次， main() 方法必须定义 try/catch 语句来捕获该异常。

正确例子如下：

```java
class TestThrows {
    static void throw1() throws IllegalAccessException {
        System.out.println("Inside throw1 . ");
        throw new IllegalAccessException("demo");
    }

    public static void main(String[] args) {
        try {
            throw1();
        } catch (IllegalAccessException e) {
            System.out.println("Caught " + e);
        }
    }
}
```

throws 抛出异常的规则：

- 如果是不受检查异常（ unchecked exception ），即 Error 、 RuntimeException 或它们的子类，那么可以不使用 throws 关键字来声明要抛出的异常，编译仍能顺利通过，但在运行时会被系统抛出。
- 必须声明方法可抛出的任何检查异常（ checked exception ）。即如果一个方法可能出现受可查异常，要么用 try-catch 语句捕获，要么用 throws 子句声明将它抛出，否则会导致编译错误
- 仅当抛出了异常，该方法的调用者才必须处理或者重新抛出该异常。当方法的调用者无力处理该异常的时候，应该继续抛出，而不是囫囵吞枣。
- 调用方法必须遵循任何可查异常的处理和声明规则。若覆盖一个方法，则不能声明与覆盖方法不同的异常。声明的任何异常必须是被覆盖方法所声明异常的同类或子类。

### 4、finally

当异常发生时，通常方法的执行将做一个陡峭的非线性的转向，它甚至会过早的导致方法返回。例如， 如果一个方法打开了一个文件并关闭，然后退出，你不希望关闭文件的代码被异常处理机制旁路。 `finally` 关键字为处理这种意外而设计。

finally 创建的代码块在 try/catch 块完成之后另一个 try/catch 出现之前执行。 finally 块无论有没有异常抛出都会执行。如果抛出异常，即使没有 catch 子句匹配， finally 也会执行。

一个方法将从一个 try/catch 块返回到调用程序的任何时候，经过一个未捕获的异常或者是一个明确的返回语句， finally 子句在方法返回之前仍将执行。这在关闭文件句柄和释放任何在方法开始时被分配的其他资源是很有用。

注意： finally 子句是可选项，可以有也可以无，但是每个 try 语句至少需要一个 catch 或 者 finally 子句。

【例子】

```java
class TestFinally {
    static void proc1() {
        try {
            System.out.println("inside proc1");
            throw new RuntimeException("demo");
        } finally {
            System.out.println("proc1's finally");
        }
    }

    static void proc2() {
        try {
            System.out.println("inside proc2");
            return;
        } finally {
            System.out.println("proc2's finally");
        }
    }

    static void proc3() {
        try {
            System.out.println("inside proc3");
        } finally {
            System.out.println("proc3's finally");
        }
    }

    public static void main(String[] args) {
        try {
            proc1();
        } catch (Exception e) {
            System.out.println("Exception caught");
        }
        proc2();
        proc3();
    }
}
```

> 执行结果：
>
> inside proc1
> proc1's finally
> Exception caught
> inside proc2
> proc2's finally
> inside proc3
> proc3's finally

注：如果 finally 块与一个 try 联合使用， finally 块将在 try 结束之前执行。

### 执行顺序

**try, catch,finally ,return 执行顺序**

1. 执行try，catch ， 给返回值赋值
2. 执行finally
3. return

## 自定义异常

使用Java内置的异常类可以描述在编程时出现的大部分异常情况。除此之外，用户还可以自定义异常。 用户自定义异常类，只需继承 `Exception` 类即可。

在程序中使用自定义异常类，大体可分为以下几个步骤：

- 创建自定义异常类。
- 在方法中通过 throw 关键字抛出异常对象。
- 如果在当前抛出异常的方法中处理异常，可以使用 try-catch 语句捕获并处理；否则在方法的声明处通过 throws 关键字指明要抛出给方法调用者的异常，继续进行下一步操作。
- 在出现异常方法的调用者中捕获并处理异常。

【举例】

```java
class MyException extends Exception {
    private int detail;
    MyException(int a){
        detail = a;
    }
    public String toString(){
        return "MyException ["+ detail + "]";
    }
}
```

```java
public class TestMyException {
    static void compute(int a) throws MyException {
        System.out.println("Called compute(" + a + ")");
        if (a > 10) {
            throw new MyException(a);
        }
        System.out.println("Normal exit!");
    }

    public static void main(String[] args) {
        try {
            compute(1);
            compute(20);
        } catch (MyException me) {
            System.out.println("Caught " + me);
        }
    }
}
```

> 输出：
>
> Called compute(1)
> Normal exit!
> Called compute(20)
> Caught MyException [20]

举例二：输入年龄时，年龄不能为负数，否则就报错

```java
public class AgeException extends Exception{
    public AgeException() {
    }

    public AgeException(String message) {
        super(message);
    }
}
```

```java
public class Demo {
    public static void main(String[] args) {
        try {
            check(-10);
        } catch (AgeException e) {
            e.printStackTrace();
        }
    }

    public static void check(int age) throws AgeException {
        if (age < 0) {
            throw new AgeException("年龄不能小于0");
        } else {
            System.out.println(age);
        }

    }
}
```

![image-20210329171254831](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-异常机制.assets/image-20210329171254831.png)

## 总结

![image-20210329171311748](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-异常机制.assets/image-20210329171311748.png)

**实际应用中的经验与总结**

1. 处理运行时异常时，采用逻辑去合理规避同时辅助try-catch处理

2. 在多重catch块后面，可以加一个catch ( Exception )来处理可能会被遗漏的异常

3. 对于不确定的代码，也可以加上try-catch，处理潜在的异常

4. 尽量去处理异常，切忌只是简单的调用printStackTrace)去打印输出
5. 具体如何处理异常，要根据不同的业务需求和异常类型去决定
6. 尽量添加finally语句块去释放占用的资源


# JavaSE-面向对象

## 面向过程&面向对象

语言的进化发展跟生物的进化发展其实是一回事，都是”物以类聚”。相近的感光细胞聚到一起变成了我们的眼睛，相近的嗅觉细胞聚到一起变成了我们的鼻子。

语句多了，我们将完成同样功能的相近的语句，聚到了一块儿，便于我们使用。于是，方法出现了！

变量多了，我们将功能相近的变量组在一起，聚到一起归类，便于我们调用。于是，结构体出现了！

再后来，方法多了，变量多了！结构体不够用了！我们就将功能相近的变量和方法聚到了一起，于是类和对象出现了！

寥寥数语，就深刻的展示了语言的进化历史！其实，都非常自然，”物以类聚”。希望大家能记住这句话。

企业的发展也是”物以类聚”的过程，完成市场推广的人员聚到一起形成了市场部。完成技术开发的人员聚到一起形成了开发部！

**面向过程的思维模式**

面向过程的思维模式是简单的线性思维，思考问题首先陷入第一步做什么、第二步做什么的细节中。这种思维模式适合处理简单的事情，比如：上厕所。

如果面对复杂的事情，这种思维模式会陷入令人发疯的状态！比如：如何造神舟十号！

**面向对象的思维模式**

面向对象的思维模式说白了就是分类思维模式。思考问题首先会解决问题需要哪些分类，然后对这些分类进行单独思考。最后，才对某个分类下的细节进行面向过程的思索。

这样就可以形成很好的协作分工。比如：设计师分了10个类，然后将10个类交给了10个人分别进行详细设计和编码！

显然，面向对象适合处理复杂的问题，适合处理需要多人协作的问题！

如果一个问题需要多人协作一起解决，那么你一定要用面向对象的方式来思考！

**对于描述复杂的事物，为了从宏观上把握、从整体上合理分析，我们需要使用面向对象的思路来分析整 个系统。但是，具体到微观操作，仍然需要面向过程的思路去处理。**

## OOP详解

### 1、什么是面向对象

 Java的编程语言是面向对象的，采用这种语言进行编程称为面向对象编程(Object-Oriented Programming, OOP)。

面向对象编程的本质就是：以类的方式组织代码，以对象的组织(封装)数据。

**抽象(abstract)**

忽略一个主题中与当前目标无关的那些方面，以便更充分地注意与当前目标有关的方面。抽象并不打算了
解全部问题，而只是选择其中的一部分，暂时不用关注细节。

> 例如：要设计一个学生成绩管理系统，那么对于学生，只关心他的班级、学号、成绩等，而不用去关心他的
> 身高、体重这些信息。 抽象是什么？就是将多个物体共同点归纳出来，就是抽出像的部分！

**封装(Encapsulation)**

封装是面向对象的特征之一，是对象和类概念的主要特性。封装是把过程和数据包围起来，对数据的访 问只能通过指定的方式。

在定义一个对象的特性的时候，有必要决定这些特性的可见性，即哪些特性对外部是可见的，哪些特性用于表示内部状态。

通常，应禁止直接访问一个对象中数据的实际表示，而应通过操作接口来访问，这称为信息隐藏。

信息隐藏是用户对封装性的认识，封装则为信息隐藏提供支持。

封装保证了模块具有较好的独立性，使得程序维护修改较为容易。对应用程序的修改仅限于类的内部， 因而可以将应用程序修改带来的影响减少到最低限度。

**继承(inheritance)**

继承是一种联结类的层次模型，并且允许和支持类的重用，它提供了一种明确表述共性的方法

新类继承了原始类后,新类就继承了原始类的特性，新类称为原始类的派生类(子类)，而原始类称为新类的基类(父类)。

派生类(子类)可以从它的基类(父类)那里继承方法和实例变量，并且派生类(子类)中可以修改或增加新的方法使之更适合特殊的需要继承性很好的解决了软件的可重用性问题。比如说，所有的Windows应用程序都有一个窗口，它们可以看作都是从一个窗口类派生出来的。但是有的应用程序用于文字处理，有的应用程序用于绘图，这是由于派生出了不同的子类，各个子类添加了不同的特性。

**多态(polymorphism)**

多态性是指允许不同类的对象对同一消息作出响应。

多态性语言具有灵活、抽象、行为共享、代码共享的优势，很好的解决了应用程序函数同名问题。

相同类域的不同对象,调用相同方法,表现出不同的结果

**从认识论角度考虑是先有对象后有类。对象，是具体的事物。类，是抽象的，是对对象的抽象。**

**从代码运行角度考虑是先有类后有对象。类是对象的模板。**

### 2、类与对象的关系

类是一种抽象的数据类型,它是对某一类事物整体描述/定义,但是并不能代表某一个具体的事物

> 例如：我们生活中所说的词语：动物、植物、手机、电脑等等。这些也都是抽象的概念，而不是指的某一个 具体的东西。

例如: Person类、Pet类、Car类等，这些类都是用来 描述/定义 某一类具体的事物应该具备的特点和行为

对象是抽象概念的具体实例

> 例如：张三就是人的一个具体实例，张三家里的旺财就是狗的一个具体实例。能够体现出特点，展现出功能的是具体的实例，而不是一个抽象的概念。

【示例】

```java
Student s = new Student(1,"tom",20);
s.study();

Car c = new Car(1,"BWM",500000);
c.run();
```

对象s就是Student类的一个实例，对象c就是Car类的一个具体实例，能够使用的是具体实例，而不是类。类只是给对象的创建提供了一个参考的模板而已。

但是在java中，没有类就没有对象，然而类又是根据具体的功能需求，进行实际的分析，最终抽象出来的。

### 3、对象和引用的关系

引用 "指向" 对象

使用类类型、数组类型、接口类型声明出的变量，都可以指向对象，这种变量就是引用类型变量，简称引用。

在程序中，创建出对象后，直接使用并不方便，所以一般会用一个引用类型的变量去接收这个对象，这个就是所说的引用指向对象。

总结：对象和引用的关系，就如电视机和遥控器，风筝和线的关系一样。

## 方法回顾及加深

方法一定是定义在类中的，属于类的成员。

### 1、方法的定义

> 格式： 修饰符 返回类型 方法名(参数列表)异常抛出类型{...}

1. **修饰符**

   public、static、abstract、final等等都是修饰符，一个方法可以有多个修饰符。例如程序入口 main方法，就使用了public static这个俩个修饰符

   注：如果一个方法或者属性有多个修饰符，这多个修饰符是没有先后顺序的

2. **返回类型**

   方法执行完如果有要返回的数据，那么就要声明返回数据的类型，如果没有返回的数据，那么返回类型就必须写void

   只有构造方法(构造器)不写任何返回类型也不写void

   【示例】

   ```java
   public String sayHello(){
       return "hello";
   }
   public int max(int a,int b){
       return a>b?a:b;
   }
   public void print(String msg){
       System.out.println(msg);
   }
   ```

   思考：声明返回类型的方法中一定要出现return语句，那么没有返回类型(void)的方法中，能不能出现 return语句?

   **break和return的区别**

   return 语句的作用

   > (1) return 从当前的方法中退出,返回到该调用的方法的语句处,继续执行。 
   > (2) return 返回一个值给调用该方法的语句，返回值的数据类型必须与方法的声明中的返回值的类型一致。 
   > (3) return后面也可以不带参数，不带参数就是返回空，其实主要目的就是用于想中断函数执行，返回 调用函数处。

   break语句的作用

   > (1)break在循环体内，强行结束循环的执行，也就是结束整个循环过程，不在判断执行循环的条件是否成立，直接转向循环语句下面的语句。
   >
   > (2)当break出现在循环体中的switch语句体内时，其作用只是跳出该switch语句体。

3. **方法名**

   遵守java中标示符的命名规则即可.

4. 参数列表

   根据需求定义,方法可以是无参的,也可以有一个参数,也可以有多个参数

5. 异常抛出类型

   如果方法中的代码在执行过程中，可能会出现一些异常情况，那么就可以在方法上把这些异常声明并抛出， 也可以同时声明抛出多个异常，使用逗号隔开即可。

   ```java
   public void readFile(String file)throws IOException{
   }
   
   public void readFile(String file)throws IOException,ClassNotFoundException{
   }
   ```

### 2、方法调用

在类中定义了方法，这个方法中的代码并不会执行，当这个方法被调用的时候，方法中的代码才会被一行一 行顺序执行。

1. **非静态方法**

   没有使用static修饰符修饰的方法，就是非静态方法。

   调用这种方法的时候，是"一定"要使用对象的调用。因为非静态方法是属于对象的。(非静态属性也是一样的)

   【例子】

   >public class Student{
   >	public void say(){}
   >}
   >
   >main: 
   >
   >Student s = new Student(); 
   >
   >s.say();

2. **静态方法**

   使用static修饰符修饰的方法,就是静态方法。

   调用这种方法的时候，"可以"使用对象调用，也"可以"使用类来调用，但是推荐使用类进行调用。因为静态方法是属于类的。(静态属性也是一样的)

   【例子】

   >public class Student{
   >	public static void say(){}
   >}
   >
   >
   >
   >main:
   >
   >Student.say();

3. **类中方法之间的调用**

   假设同一个类中有俩个方法，a方法和b方法，a和b都是非静态方法，相互之间可以直接调用。

   ```java
   public void a(){
       b();
   }
   public void b(){
       
   }
   ```

   a和b都是静态方法,相互之间可以直接调用

   ```java
   public static void a(){
       b();
   }
   public static void b(){
       
   }
   ```

   a静态方法，b是非静态方法，a方法中不能直接调用b方法，但是b方法中可以直接调用a方法。静态方法不能 调用非静态方法！

   ```java
   public static void a(){
       //b();报错
   }
   public void b(){
       a();
   }
   ```

   另外：在同一个类中，静态方法内不能直接访问到类中的非静态属性。

   总结：类中方法中的调用，两个方法都是静态或者非静态都可以互相调用，当一个方法是静态，一个方 法是非静态的时候，非静态方法可以调用静态方法，反之不能。

### 3、调用方法时的传参

**1、形参和实参**

```java
public static void test(int a){

}

public static void main(String[] args) {
    int x = 1;
    test(x);
}
```

参数列表中的a是方法test的形参(形式上的参数)
调用方法时的x是方法test的实参(实际上的参数)

注意：形参的名字和实参的名字都只是一个变量的名字,是可以随便写的,我们并不关心这个名字,而是关 心变量的类型以及变量接收的值。

**2、值传递和引用传递**

调用方法进行传参时，分为值传递和引用传递两种。

如果参数的类型是基本数据类型，那么就是值传递。

如果参数的类型是引用数据类型，那么就是引用传递。

值传递是实参把自己变量本身存的简单数值赋值给形参。
引用传递是实参把自己变量本身存的对象内存地址值赋值给形参。

所以值传递和引用传递本质上是一回事，只不过传递的东西的意义不同而已。

【示例：值传递】

```
public static void changeNum(int a) {
    a = 10;
}

public static void main(String[] args) {
    int a = 1;
    System.out.println("before: a = " + a); //1
    changeNum(a);
    System.out.println("after: a = " + a); //1
}
```

【示例：引用传递】

```
public class Test {
    public static void changeName(Student s) {
        s.name = "tom";
    }

    public static void main(String[] args) {
        Student s = new Student();
        System.out.println("before: name = " + s.name); //null
        changeName(s);
        System.out.println("after: name = " + s.name); //tom
    }

    static class Student {
        String name;
    }

}
```

### 4、this关键字

在类中，可以使用this关键字表示一些特殊的作用。

**1、this在类中的作用**

区别成员变量和局部变量

```java
public class Student{
    private String name;
    public void setName(String name){
        //this.name表示类中的属性name
        this.name = name;
    }
}
```

调用类中的其他方法

```java
public class Student{
    private String name;
    public void setName(String name){
        this.name = name;
    }
    public void print(){
        //表示调用当前类中的setName方法
        this.setName("tom");
    }
}
```

注：默认情况下，setName("tom")和this.setName("tom")的效果是一样的。

调用类中的其他构造器

```java
public class Student{
    private String name;
    public Student(){
        //调用一个参数的构造器,并且参数的类型是String
        this("tom");
    }
    public Student(String name){
        this.name = name;
    }
}
```

注：this的这种用法，只能在构造器中使用。普通的方法是不能用的。并且这局调用的代码只能出现在构造器中的第一句。

【示例】

```java
public class Student{
    private String name;
    //编译报错,因为this("tom")不是构造器中的第一句代码.
    public Student(){
        System.out.println("hello");
        this("tom");
    }
    public Student(String name){
        this.name = name;
    }
}
```

**2、this关键字在类中的意义**

this在类中表示当前类将来创建出的对象。

【例子】

```java
public class Student {
    private String name;

    public Student() {
        System.out.println("this = " + this);
    }

    public static void main(String[] args) {
        Student s = new Student();
        System.out.println("s = " + s);
    }
}
```

运行后看结果可知，this和s打印的结果是一样的，那么其实也就是变量s是从对象的外部执行对象，而this是在对象的内部执行对象本身。

这样也就能理解为什么this.name代表的是成员变量，this.setName("tom")代表的是调用成员方法。因为这俩句代码从本质上讲，和在对象外部使用变量s来调用是一样的，s.name和s.setName("tom")

【this和s打印出来的内存地址是一样的，使用==比较的结果为true。】

```java
public class Student{
    public Student getStudent(){
        return this;
    }
    public static void main(String[] args) {
        Student s1 = new Student();
        Student s2 = s1.getStudent();
        System.out.println(s1 == s2);//true
    }
}
```

【调用类中的this，s1和s2不相等】

```java
public class Student{
    private String name;
    public void test(){
        System.out.println(this);
    }
    public static void main(String[] args) {
        Student s1 = new Student();
        Student s2 = new Student();
        s1.test();
        s2.test();
    }
}
```

注：这句话是要这么来描述的，s1对象中的this和s1相等，s2对象中的this和s2相等，因为类是模板，模板中写的this并不是只有一个，每个对象中都有一个属于自己的this，就是每个对象中都一个属于自己的name属性一样。

## 创建与初始化对象

**使用new关键字创建对象**

使用new关键字创建的时候，除了分配内存空间之外，还会给创建好的对象进行默认的初始化，以及对类中构造器的调用。

那么对main方法中的以下代码：Student s = new Student();

1） 为对象分配内存空间，将对象的实例变量自动初始化默认值为0/false/null。(实例变量的隐式赋值)

2） 如果代码中实例变量有显式赋值，那么就将之前的默认值覆盖掉。(之后可以通过例子看到这个现象)

   	例如：显式赋值，private String name = "tom";

3） 调用构造器

4） 把对象内存地址值赋值给变量。(=号赋值操作)

## 构造器

类中的构造器也称为构造方法，是在进行创建对象的时候必须要调用的。并且构造器有以下俩个特点:

1. 必须和类的名字相同
2. 必须没有返回类型,也不能写void

**构造器的作用:**

1. 使用new创建对象的时候必须使用类的构造器
2. 构造器中的代码执行后，可以给对象中的属性初始化赋值

【演示】

```java
public class Student{
    private String name;
    
    public Student(){
        name = "tom";
    }
}
```

**构造器重载**

除了无参构造器之外，很多时候我们还会使用有参构造器，在创建对象时候可以给属性赋值。

【例子】

```java
public class Student{
    private String name;
    public Student(){
        name = "tom";
    }
    public Student(String name){
        this.name = name;
    }
}
```

**构造器之间的调用**

使用this关键字，在一个构造器中可以调用另一个构造器的代码。

注意：this的这种用法不会产生新的对象，只是调用了构造器中的代码而已。一般情况下只有使用new关键字才会创建新对象。

【演示】

```java
public class Student{
    private String name;
    public Student(){
        this();
    }
    public Student(String name){
        this.name = name;
    }
}
```

**默认构造器**

在java中，即使我们在编写类的时候没有写构造器，那么在编译之后也会自动的添加一个无参构造器，这个无参构造器也被称为默认的构造器。

【示例】

```java
public class Student{
    
}

main:
//编译通过,因为有无参构造器
Student s = new Student();
```

但是,如果我们手动的编写了一个构造器,那么编译后就不会添加任何构造器了

【示例】

```java
public class Student{
    private String name;
    public Student(String name){
        this.name = name;
    }
}

main:
//编译报错,因为没有无参构造器
Student s = new Student();
```



## 内存分析

JAVA程序运行的内存分析

**栈 stack：**

1. 每个线程私有，不能实现线程间的共享！
2. 局部变量放置于栈中。
3. 栈是由系统自动分配，速度快！栈是一个连续的内存空间！

**堆 heap：**

1. 放置new出来的对象！
2. 堆是一个不连续的内存空间，分配灵活，速度慢！

**方法区(也是堆)：**

1. 被所有线程共享！
2. 用来存放程序中永远是不变或唯一的内容。（类代码信息、静态变量、字符串常量）

![image-20210328212049006](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-面向对象.assets/image-20210328212049006.png)

注意：本次内存分析，我们的主要目的是让大家了解基本的内存概念。类加载器、Class对象这些更加详细的内容，我们将在后面专门讲反射的课程里面讲。

**引用类型的概念**

1. java中，除了基本数据类型之外的其他类型称之为引用类型。
2. java中的对象是通过引用来操作的。(引用：reference)说白了，引用指的就是对象的地址！

**属性（field，或者叫成员变量）**

1. 属性用于定义该类或该类对象包含的数据或者说静态属性。

2. 属性作用范围是整个类体。

3.  属性的默认初始化：

   在定义成员变量时可以对其初始化，如果不对其初始化，Java使用默认的值对其初始化(数值：0,0.0 char：u0000, boolean：false, 所有引用类型：null)

4. 属性定义格式：

   > [修饰符] 属性类型 属性名 = [默认值]

**类的方法**

方法是类和对象动态行为特征的抽象。方法很类似于面向过程中的函数。面向过程中，函数是最基本单位，整个程序有一个个函数调用组成；面向对象中，整个程序的基本单位是类，方法是从属于类或对象的。

方法定义格式：

```java
[修饰符] 方法返回值类型 方法名(形参列表) {
    // n条语句
}
```

**java对象的创建和使用**

- 必须使用 new 关键字创建对象。

  Person person= new Person ();

- 使用对象（引用）.成员变量来引用对象的成员变量。

  person.age

- 使用对象（引用）. 方法（参数列表）来调用对象的方法

  person.setAge(18)

类中就是：静态的数据 动态的行为

学习完类与对象终于认识到什么是类，什么是对象了。

接下来要看的就是java的三大特征：继承、封 装、多态。

## 封装

我要看电视，只需要按一下开关和换台就可以了。有必要了解电视机内部的结构吗？有必要碰碰显像管吗？

制造厂家为了方便我们使用电视，把复杂的内部细节全部封装起来，只给我们暴露简单的接口，比如： 电源开关。需要让用户知道的暴露出来，不需要让用户了解的全部隐藏起来。这就是封装。

白话：该露的露，该藏的藏

专业：我们程序设计要追求“高内聚，低耦合”。高内聚就是类的内部数据操作细节自己完成，不允许外部干涉；低耦合：仅暴露少量的方法给外部使用。

**封装（数据的隐藏）**

在定义一个对象的特性的时候，有必要决定这些特性的可见性，即哪些特性对外部是可见的，哪些特性用于表示内部状态。

通常，应禁止直接访问一个对象中数据的实际表示，而应通过操作接口来访问，这称为信息隐藏。

### 1、封装的步骤

1. 使用private 修饰需要封装的成员变量。

2. 提供一个公开的方法设置或者访问私有的属性

   设置 通过set方法，命名格式： set属性名（）; 属性的首字母要大写

   访问 通过get方法，命名格式： get属性名（）; 属性的首字母要大写

【演示】

```java
//对象能在类的外部"直接"访问
public class Student{
    public String name;
    public void println(){
        System.out.println(this.name);
    }
}
public class Test{
    public static void main(String[] args){
        Student s = new Student();
        s.name = "tom";
    }
}
```

在类中一般不会把数据直接暴露在外部的，而使用private(私有)关键字把数据隐藏起来

【演示】

```java
public class Student{
    private String name;
}
public class Test{
    public static void main(String[] args){
        Student s = new Student();
        //编译报错,在类的外部不能直接访问类中的私有成员
        s.name = "tom";
    }
}
```

如果在类的外部需要访问这些私有属性,那么可以在类中提供对于的get和set方法,以便让用户在类的外部 可以间接的访问到私有属性

【示例】

```java
//set负责给属性赋值
//get负责返回属性的值
public class Student{
    private String name;
    public void setName(String name){
    this.name = name;
	}
	public String getName(){
        return this.name;
	}
}
public class Test{
    public static void main(String[] args){
        Student s = new Student();
        s.setName("tom");
        System.out.println(s.getName());
    }
}

```

### 2、作用和意义

1. 提高程序的安全性，保护数据。
2. 隐藏代码的实现细节
3. 统一用户的调用接口
4. 提高系统的可维护性
5. 便于调用者调用。

良好的封装，便于修改内部代码，提高可维护性。

良好的封装，可进行数据完整性检测，保证数据的有效性。

### 3、方法重载

类中有多个方法，有着相同的方法名，但是方法的参数各不相同,这种情况被称为方法的重载。方法的重载可以提供方法调用的灵活性。

思考：HelloWorld中的System.out.println()方法，为什么可以把不同类型的参数传给这个方法?

【演示：查看println方法的重载】 idea中`ctrl`+`左键`点击`println`

例如:

```java
public class Test{
    public void test(String str){
        
    }
    public void test(int a){
        
    }
}
```

**方法重载必须满足以下条件**

1. 方法名必须相同

2. 参数列表必须不同(参数的类型、个数、顺序的不同)

   ```java
   public void test(Strig str){}
   public void test(int a){}
   
   public void test(Strig str,double d){}
   public void test(Strig str){}
   
   public void test(Strig str,double d){}
   public void test(double d,Strig str){}
   ```

3. 方法的返回值可以不同，也可以相同。

**在java中，判断一个类中的俩个方法是否相同，主要参考俩个方面：方法名字和参数列表**

## 继承

继承：extands

现实世界中的继承无处不在。比如：

动物：哺乳动物、爬行动物

哺乳动物：灵长目、鲸目等。

**继承的本质是对某一批类的抽象，从而实现对现实世界更好的建模。**

**为什么需要继承？继承的作用？**

第一好处：继承的本质在于抽象。类是对对象的抽象，继承是对某一批类的抽象。

第二好处：为了提高代码的复用性。

extands的意思是“扩展”。子类是父类的扩展。

【注】JAVA中类只有单继承，没有多继承！ 接口可以多继承！

### 1、继承

1. 继承是类和类之间的一种关系。除此之外,类和类之间的关系还有依赖、组合、聚合等。

2. 继承关系的俩个类，一个为子类(派生类),一个为父类(基类)。子类继承父类，使用关键字extends来表示。

   ```java
   public class student extends Person{
   }
   ```

3. 子类和父类之间，从意义上讲应该具有"is a"的关系。

   > student is a person 
   >
   > dog is a animal

4. 类和类之间的继承是单继承

   一个子类只能"直接"继承一个父类,就像是一个人只能有一个亲生父亲
   一个父类可以被多子类继承,就像一个父亲可以有多个孩子

   注:java中接口和接口之间,有可以继承,并且是多继承。

5. 父类中的属性和方法可以被子类继承

   子类中继承了父类中的属性和方法后,在子类中能不能直接使用这些属性和方法,是和这些属性和方法原有 的修饰符(public protected default private)相关的。

   例如：

   父类中的属性和方法使用public修饰，在子类中继承后"可以直接"使用
   父类中的属性和方法使用private修饰，在子类中继承后"不可以直接"使用
   
   **注：具体细则在修饰符部分详细说明**
   
   父类中的构造器是不能被子类继承的，但是子类的构造器中，会隐式的调用父类中的无参构造器（默认使用 super关键字）。
   
   **注:具体细节在super关键字部分详细说明**

### 2、Object类

 java中的每一个类都是"直接" 或者 "间接"的继承了Object类。所以每一个对象都和Object类有"is a"的关系。从API文档中，可以看到任何一个类最上层的父类都是Object。(Object类本身除外)AnyClass is a Object。

> System.out.println(任何对象 instanceof Object);
>
> 输出结果:true
> 注:任何对象也包含数组对象

例如:

```java
//编译后,Person类会默认继承Object
public class Person{}

//Student是间接的继承了Object
public class Student extends Person{}
```

在Object类中，提供了一些方法被子类继承，那么就意味着，在java中，任何一个对象都可以调用这些被继承过来的方法。(因为Object是所以类的父类)

例如：toString方法、equals方法、getClass方法等

### 3、Super关键字

子类继承父类之后，在子类中可以使用this来表示访问或调用子类中的属性或方法，使用super就表示访问或调用父类中的属性和方法。

**1、super的使用**

【访问父类中的属性】

```java
public class Person{
    protected String name = "zs";
}
```

```java
public class Student extends Person{
    private String name = "lisi";
    public void tes(String name){
        System.out.println(name);
        System.out.println(this.name);
        System.out.println(super.name);
    }
}
```

【调用父类中的方法】

```java
public class Person{
    public void print(){
        System.out.println("Person");
    }
}

```

```java
public class Student extends Person{
    public void print(){
        System.out.println("Student");
    }
    public void test(){
        print();
        this.print();
        super.print();
    }
}
```

【调用父类中的构造器】

```java
public class Person{
}

public class Student extends Person{
    //编译通过,子类构造器中会隐式的调用父类的无参构造器
    //super();
    public Student(){
    }
}
```

父类没有无参构造

```java
public class Person{
    protected String name;
    public Person(String name){
        this.name = name;
    }
}
public class Student extends Person{
    //编译报错,子类构造器中会隐式的调用父类的无参构造器,但是父类中没有无参构造器
    //super();
    public Student(){
        
    }
}
```

【显式的调用父类的有参构造器】

```java
public class Person{
    protected String name;
    public Person(String name){
    this.name = name;
	}
}

public class Student extends Person{
    //编译通过,子类构造器中显式的调用父类的有参构造器
    public Student(){
        super("tom");
    }
}
```

注：不管是显式还是隐式的父类的构造器，super语句一定要出现在子类构造器中第一行代码。所以this和 super不可能同时使用它们调用构造器的功能，因为它们都要出现在第一行代码位置。

【例子】

```java
public class Person{
    protected String name;
    public Person(String name){
        this.name = name;
    }
}

public class Student extends Person{
    //编译报错,super调用构造器的语句不是第一行代码
    public Student(){
        System.out.println("Student");
        super("tom");
    }
}
```

【例子】

```java
public class Person{
    protected String name;
    public Person(String name){
        this.name = name;
    }
}
//编译通过
public class Student extends Person{
    private int age;
    public Student(){
        this(20);
    }
    public Student(int age){
        super("tom");
        this.age = age;
    }
}
```

**super使用的注意的地方**

- 用super调用父类构造方法，必须是构造方法中的第一个语句。
- super只能出现在子类的方法或者构造方法中
- super 和 this 不能够同时调用构造方法。（因为this也是在构造方法的第一个语句）

**super 和 this 的区别**

1. 代表的事物不一样：

   this：代表所属方法的调用者对象。

   super：代表父类对象的引用空间。

2. 使用前提不一致：

   this：在非继承的条件下也可以使用。

   super：只能在继承的条件下才能使用。

3. 调用构造方法：

   this：调用本类的构造方法。

   super：调用的父类的构造方法



### 4、方法重写

方法的重写（override）

- 方法重写只存在于子类和父类(包括直接父类和间接父类)之间。在同一个类中方法只能被重载，不能被重写
- 静态方法不能重写
  1. 父类的静态方法不能被子类重写为非静态方法 //编译出错
  2. 父类的非静态方法不能被子类重写为静态方法；//编译出错
  3. 子类可以定义与父类的静态方法同名的静态方法(但是这个不是覆盖)

【例子】

> A类继承B类 A和B中都一个相同的静态方法test
>
> B a = new A(); 
> a.test();//调用到的是B类中的静态方法test
>
> A a = new A(); 
> a.test();//调用到的是A类中的静态方法test
>
> 可以看出静态方法的调用只和变量声明的类型相关
> 这个和非静态方法的重写之后的效果完全不同

私有方法不能被子类重写，子类继承父类后,是不能直接访问父类中的私有方法的,那么就更谈不上重写了

```java
public class Person{
    private void run(){}
    
}

//编译通过,但这不是重写,只是俩个类中分别有自己的私有方法
public class Student extends Person{
    private void run(){}
}
```

**重写的语法**

1. 方法名必须相同

2. 参数列表必须相同

3. 访问控制修饰符可以被扩大，但是不能被缩小： public protected default private

4. 抛出异常类型的范围可以被缩小,但是不能被扩大

   ClassNotFoundException ---> Exception（不能扩大）

5. 返回类型可以相同，也可以不同。

   如果不同的话，子类重写后的方法返回类型必须是父类方法返回类型的子类型。

   **例如**：父类方法的返回类型是Person，子类重写后的返回类可以是Person也可以是Person的子类型

**注**：一般情况下，重写的方法会和父类中的方法的声明完全保持一致，只有方法的实现不同。(也就是大括号中代码不一样)

```java
public class Person{
    public void run(){}
    protected Object test()throws Exception{
        return null;
    }
}

//编译通过,子类继承父类,重写了run和test方法.
public class Student extends Person{
    public void run(){}
    public String test(){
        return "";
    }
}
```

为什么要重写？

子类继承父类，继承了父类中的方法，但是父类中的方法并不一定能满足子类中的功能需要，所以子类中需要把方法进行重写。

**总结：**

1. 方法重写的时候，必须存在继承关系。
2. 方法重写的时候，方法名和形式参数必须跟父类是一致的。
3. 方法重写的时候，子类的权限修饰符必须要大于或者等于父类的权限修饰符。( private < protected < public，friendly < public )
4. 方法重写的时候，子类的返回值类型必须小于或者等于父类的返回值类型。( 子类 < 父类 ) 数据类型没有明确的上下级关系
5. 方法重写的时候，子类的异常类型要小于或者等于父类的异常类型。

## 多态

### 1、认识多态

多态性是OOP中的一个重要特性，主要是用来实现动态联编的，换句话说，就是程序的最终状态只有在执行过程中才被决定而非在编译期间就决定了。这对于大型系统来说能提高系统的灵活性和扩展性。

多态可以让我们不用关心某个对象到底是什么具体类型，就可以使用该对象的某些方法，从而实现更加灵活的编程，提高系统的可扩展性。

允许不同类的对象对同一消息做出响应。即同一消息可以根据发送对象的不同而采用多种不同的行为方式。

相同类域的不同对象,调用相同的方法,执行结果是不同的

1. 一个对象的实际类型是确定的

   例如: new Student(); new Person();等

2. 可以指向对象的引用的类型有很多

   一个对象的实现类型虽然是确定的，但是这个对象所属的类型可能有很多种。

   例如：Student继承了Person类

   ```java
   Student s1 = new Student();
   Person s2 = new Student();
   Object s3 = new Student();
   ```

   因为Person和Object都是Student的父类型

   ![image-20210328222401861](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-面向对象.assets/image-20210328222401861.png)

注：一个对象的实际类型是确定，但是可以指向这个对象的引用的类型，却是可以是这对象实际类型的任意父类型。

**一个父类引用可以指向它的任何一个子类对象**

例如：

```java
Object o = new AnyClass();
Person p = null;
p = new Student();
p = new Teacher();
p = new Person();
```

**多态中的方法调用**

```java
public class Person{
    public void run(){}
}

public class Student extends Person{

}
```

调用到的run方法,是Student从Person继承过来的run方法

```java
Person p = new Student();
p.run();
```

例如：

```java
public class Person{
    public void run(){}
}

public class Student extends Person{
    public void run(){
    //重写run方法
    }
}

//调用到的run方法,是Student中重写的run方法
public static void main(String[] args) {
    Person p = new Student();
    p.run();
}

```

注：子类继承父类,调用a方法，如果a方法在子类中没有重写,那么就是调用的是子类继承父类的a方法, 如果重写了,那么调用的就是重写之后的方法。

子类中独有方法的调用

```java
public class Person{
    public void run(){}
}

public class Student extends Person{
    public void test(){
    }
}

main:
Person p = new Student();
//调用到继承的run方法
p.run();

//编译报错,因为编译器检查变量p的类型是Person,但是在Person类中并没有发现test方法,所以编译报错.
p.test();
```

注：一个变量x，调用一个方法test，编译器是否能让其编译通过，主要是看声明变量x的类型中有没有定义 test方法，如果有则编译通过，如果没有则编译报错。而不是看x所指向的对象中有没有test方法。

原理：编译看左边，运行不一定看右边。

> 编译看左边的意思：java 编译器在编译的时候会检测引用类型中含有指定的成员，如果没有就会报错。 子类的成员是特有的，父类的没有的，所以他是找不到的。
>
> 所以看左边，Person 中没有test()方法，于是编译报错

**子类引用和父类引用指向对象的区别**

```java
Student s = new Student();
Person p = new Student();
```

变量s能调用的方法是Student中有的方法(包括继承过来的)，变量p能调用的方法是Person中有的方法(包括继承过来的)。

但是变量p是父类型的，p不仅可以指向Student对象，还可以指向Teacher类型对象等，但是变量s只能指 Studnet类型对象，及Student子类型对象。变量p能指向对象的范围是比变量s大的。

Object类型的变量o，能指向所有对象，它的范围最大，但是使用变量o能调用到的方法也是最少的，只能调用到Object中的声明的方法，因为变量o声明的类型就是Object。

注：java中的方法调用,是运行时动态和对象绑定的,不到运行的时候,是不知道到底哪个方法被调用的。

**多态的好处与弊端**

- 好处：提高了程序的拓展性

  具体表现：定义方法的时候，使用父类型作为参数，将来在使用的时候，使用具体的子类型参与操作

- 弊端：不能使用子类的特有功能

### 2、重写、重载和多态的关系

重载是编译时多态

> 调用重载的方法,在编译期间就要确定调用的方法是谁,如果不能确定则编译报错

重写是运行时多态

> 调用重写的方法，在运行期间才能确定这个方法到底是哪个对象中的。这个取决于调用方法的引用，在运行 期间所指向的对象是谁，这个引用指向哪个对象那么调用的就是哪个对象中的方法。(java中的方法调用，是运行时动态和对象绑定的)

### 3、多态的注意事项

1.  多态是方法的多态，属性没有多态性。
2. 编写程序时，如果想调用运行时类型的方法，只能进行类型转换。不然通不过编译器的检查。但是如果两个没有关联的类进行强制转换，会报：ClassCastException。 比如：本来是狗，我把它转成猫。就会报这个异常。
3. 多态的存在要有3个必要条件：要有继承，要有方法重写，父类引用指向子类对象



### 4、多态存在的条件

- 有继承关系
- 子类重写父类方法
- 父类引用指向子类对象

补充一下第二点，既然多态存在必须要有“子类重写父类方法”这一条件，那么以下三种类型的方法是没有办法表现出多态特性的（因为不能被重写）：

1. static方法，因为被static修饰的方法是属于类的，而不是属于实例的
2. final方法，因为被final修饰的方法无法被子类重写
3. private方法和protected方法，前者是因为被private修饰的方法对子类不可见，后者是因为尽管被 protected修饰的方法可以被子类见到，也可以被子类重写，但是它是无法被外部所引用的，一个不能被外部引用的方法，怎么能谈多态呢

### 5、方法绑定(method binding)

执行调用方法时，系统根据相关信息，能够执行内存地址中代表该方法的代码。分为静态绑定和动态绑定。

**静态绑定：**

在编译期完成，可以提高代码执行速度。

**动态绑定：**

通过对象调用的方法，采用动态绑定机制。这虽然让我们编程灵活，但是降低了代码的执行速度。这也是JAVA比C/C++速度慢的主要因素之一。JAVA中除了final类、final方、static方法，所有方法都是JVM在运行期才进行动态绑定的。

多态：如果编译时类型和运行时类型不一致，就会造成多态。

### 6、instanceof和类型转换

**1、instanceof**

三个不同java文件

```java
public class Person{
    public void run(){}
}

public class Student extends Person{
}

public class Teacher extends Person{
}
```

main：方法下

```java
Object o = new Student();
System.out.println(o instanceof Student);//true
System.out.println(o instanceof Person);//true
System.out.println(o instanceof Object);//true
System.out.println(o instanceof Teacher);//false
System.out.println(o instanceof String);//false
```

```java
Person o = new Student();
System.out.println(o instanceof Student);//true
System.out.println(o instanceof Person);//true
System.out.println(o instanceof Object);//true
System.out.println(o instanceof Teacher);//false
//编译报错
System.out.println(o instanceof String);
```

```java
Student o = new Student();
System.out.println(o instanceof Student);//true
System.out.println(o instanceof Person);//true
System.out.println(o instanceof Object);//true
//编译报错
System.out.println(o instanceof Teacher);
//编译报错
System.out.println(o instanceof String);
```

>  **System.out.println(x instanceof Y);**

【分析1】

该代码能否编译通过，主要是看声明变量x的类型和Y是否存在子父类的关系。有"子父类关"系就编译通过，没有子父类关系就是编译报错。

之后学习到的接口类型和这个是有点区别的。

【分析2】

输出结果是true还是false,主要是看变量x所指向的对象实际类型是不是Y类型的"子类型".

```java
Object o = new Person();
System.out.println(o instanceof Student);//false
System.out.println(o instanceof Person);//true
System.out.println(o instanceof Object);//true
System.out.println(o instanceof Teacher);//false
System.out.println(o instanceof String);//false
```

**2、类型转换**

```java
public class Person{
    public void run(){}
}

public class Student extends Person{
    public void go(){}
}

public class Teacher extends Person{
}
```

**为什么要类型转换**

```java
//编译报错,因为p声明的类型Person中没有go方法
Person p = new Student();
p.go();

//需要把变量p的类型进行转换
Person p = new Student();
Student s = (Student)p;
s.go();

//或者
//注意这种形式前面必须要俩个小括号
Person p = new Student();
((Student)p).go();
```

**类型转换中的问题**

```java
//编译通过 运行没问题
Object o = new Student();
Person p = (Person)o;

//编译通过 运行没问题
Object o = new Student();
Student s = (Student)o;

//编译通过,运行报错
Object o = new Teacher();
Student s = (Student)o;

```

即:   X x = (X)o; 

运行是否报错，主要是变量o所指向的对象实现类型，是不是X类型的子类型，如果不是则运行就会报错。

**【总结】**

1. 父类引用可以指向子类对象，子类引用不能指向父类对象。

2. 把子类对象直接赋给父类引用叫向上转型（upcasting），不用强制转型。

   如Father father = new Son();

3. 把指向子类对象的父类引用赋给子类引用叫向下转型（downcasting），要强制转型。

   如father就是一个指向子类对象的父类引用，把father赋给子类引用son

   即Son son =（Son） father；

   其中father前面的（Son）必须添加，进行强制转换。

4. upcasting 会丢失子类特有的方法，但是子类overriding 父类的方法，子类方法有效

5. 向上转型的作用，减少重复代码，父类为参数，调有时用子类作为参数，就是利用了向上转型。这样使代码变得简洁。体现了JAVA的抽象编程思想。

## 修饰符

### 1、static修饰符

**1、static变量**

在类中,使用static修饰的成员变量,就是静态变量,反之为非静态变量。

**静态变量和非静态变量的区别**

静态变量属于类的，"可以"使用类名来访问，非静态变量是属于对象的，"必须"使用对象来访问。

```java
public class Student{
    private static int age;
    private double score;
    public static void main(String[] args) {
        Student s = new Student();
        //推荐使用类名访问静态成员
        System.out.println(Student.age);
        System.out.println(s.age);
        
        System.out.println(s.score);
    }
}
```

静态变量对于类而言在内存中只有一个，能被类的所有实例所共享。实例变量对于类的每个实例都有一份, 它们之间互不影响。（在**基础语法**中粗略解释过静态变量）

```
public class Student {
    private static int count;
    private int num;

    public Student() {
        count++;
        num++;
    }

    public static void main(String[] args) {
        Student s1 = new Student();
        Student s2 = new Student();
        Student s3 = new Student();
        Student s4 = new Student();
        //因为还是在类中,所以可以直接访问私有属性
        System.out.println(s1.num);//1
        System.out.println(s2.num);
        System.out.println(s3.num);
        System.out.println(s4.num);
        System.out.println(Student.count);
        
        System.out.println(s1.count);//4
        System.out.println(s2.count);
        System.out.println(s3.count);
        System.out.println(s4.count);
    }
}
```

在加载类的过程中为静态变量分配内存，实例变量在创建对象时分配内存，所以静态变量可以使用类名来直接访问，而不需要使用对象来访问。

**2、static方法**

在类中，使用static修饰的成员方法，就是静态方法，反之为非静态方法。

**静态方法和非静态方法的区别**

> 静态方法数属于类的，"可以"使用类名来调用，非静态方法是属于对象的，"必须"使用对象来调用。

静态方法"不可以"直接访问类中的非静态变量和非静态方法，但是"可以"直接访问类中的静态变量和静态方法

注意：this和super在类中属于非静态的变量.(静态方法中不能使用)

```
public class Student {
    private static int count;
    private int num;
    public void run(){}
    public static void go(){}
    public static void test(){
        //编译通过
        System.out.println(count);
        go();
        
        //编译报错
        System.out.println(num);
        run();
    }
}
```

非静态方法"可以"直接访问类中的非静态变量和非静态方法，也"可以"直接访问类中的静态变量和静态方法

```
public class Student {
    private static int count;
    private int num;

    public void run() {
    }

    public static void go() {
    }
    public void test() {
        //编译通过
        System.out.println(count);
        go();
        //编译通过
        System.out.println(num);
        run();
    }
}
```

思考：为什么静态方法和非静态方法不能直接相互访问？ 加载顺序的问题！

父类的静态方法可以被子类继承，但是不能被子类重写

```java
public class Person {
    public static void method() {}
}

//编译报错
public class Student extends Person {
    public void method(){}
}

```

```java
public class Person {
    public static void test() {
        System.out.println("Person");
    }
}
//编译通过,但不是重写
public class Student extends Person {
    public static void test(){
        System.out.println("Student");
    }
}
```

```java
//main:
Perosn p = new Student();
p.test();//输出Person
p = new Person();
p.test();//输出Perosn
```

父类的非静态方法不能被子类重写为静态方法 ；

```java
public class Person {
    public void test() {
        System.out.println("Person");
    }
}
//编译报错
public class Student extends Person {
    public static void test(){
        System.out.println("Student");
    }
}
```

**3、代码块和静态代码块**

【类中可以编写代码块和静态代码块】

```java
public class Person {
    {
        //代码块(匿名代码块)
    }
    static{
        //静态代码块
    }
}
```

【匿名代码块和静态代码块的执行】

因为没有名字,在程序并不能主动调用这些代码块。

匿名代码块是在创建对象的时候自动执行的，并且在构造器执行之前，在静态代码块之后。同时匿名代码块在每次创建对象的时候都会自动执行。

静态代码块是在类加载完成之后就自动执行，并且只执行一次。

注：每个类在第一次被使用的时候就会被加载，并且一般只会加载一次。

```java
public class Student {
    {
        System.out.println("匿名代码块");
    }
    
    static{
        System.out.println("静态代码块");
    }
    
    public Student(){
        System.out.println("构造器");
    }
}
```

```java
//main:
Student s1 = new Student();
Student s2 = new Student();
Student s3 = new Student();
```

输出：

> 静态代码块
> 匿名代码块
> 构造器
>
> 匿名代码块
> 构造器
>
> 匿名代码块
> 构造器

【匿名代码块和静态代码块的作用】

匿名代码块的作用是给对象的成员变量初始化赋值，但是因为构造器也能完成这项工作，所以匿名代码块使用的并不多。

静态代码块的作用是给类中的静态成员变量初始化赋值。

```java
public class Person {
    public static String name;
    static{
        name = "tom";
    }
    public Person(){
        name = "zs";
    }
}
```

> main:
> System.out.println( Person.name ); //tom

**注**：在构造器中给静态变量赋值，并不能保证能赋值成功，因为构造器是在创建对象的时候才指向，但是静态变量可以不创建对象而直接使用类名来访问。

**4、创建和初始化对象的过程**

```java
Student s = new Student();
```

【Student类之前没有进行类加载的过程】

1. 类加载，同时初始化类中静态的属性
2. 执行静态代码块
3. 分配内存空间，同时初始化非静态的属性(赋默认值,0/false/null)
4. 调用Student的父类构造器
5. 对Student中的属性进行显示赋值(如果有的话)
6. 执行匿名代码块
7. 执行构造器
8. 返回内存地址

注：子类中非静态属性的显示赋值是在父类构造器执行完之后和子类中的匿名代码块执行之前的时候

```java
public class Person{
    private String name = "zs";
    public Person() {
        System.out.println("Person构造器");
        print();
    }
    public void print(){
        System.out.println("Person print方法: name = "+name);
    }
}
```

```java
public class Student extends Person{
    private String name = "tom";
    {
        System.out.println("Student匿名代码块");
    }
    static{
        System.out.println("Student静态代码块");
    }
    public Student(){
        System.out.println("Student构造器");
    }
    public void print(){
        System.out.println("student print方法: name = "+name);
    }
    public static void main(String[] args) {
        new Student();
    }
}
```

输出：

>Student静态代码块
>Person构造器
>student print方法: name = null
>Student匿名代码块
>Student构造器

```java
Student s = new Student();
//Student类之前已经进行了类加载
//1.分配内存空间,同时初始化非静态的属性(赋默认值,0/false/null)
//2.调用Student的父类构造器
//3.对Student中的属性进行显示赋值(如果有的话)
//4.执行匿名代码块
//5.执行构造器
//6.返回内存地址
```

**5、静态导入**

静态导包就是java包的静态导入，用import static代替import静态导入包是JDK1.5中的新特性。

意思是导入这个类里的静态方法。

好处：这种方法的好处就是可以简化一些操作，例如打印操作System.out.println(…);就可以将其写入一 个静态方法print(…)，在使用时直接print(…)就可以了。但是这种方法建议在有很多重复调用的时候使用，如果仅有一到两次调用，不如直接写来的方便。

```java
import static java.lang.Math.random;
import static java.lang.Math.PI;

public class Test {
    public static void main(String[] args) {
        //之前是需要Math.random()调用的
        System.out.println(random());
        System.out.println(PI);
    }
}
```

### 2、final修饰符

**1、修饰类**

用final修饰的**类**不能被继承，没有子类

例如：我们是无法写一个类去继承String类，然后对String类型扩展的。因为API中已经被String类定义为final

我们也可以定义final修饰的类:

```java
public final class Action{
    
}

//编译报错
public class Go extends Action{
    
}
```

**2、修饰方法**

用final修饰的**方法**可以被继承，但是不能被子类的重写。

例如：每个类都是Object类的子类，继承了Object中的众多方法，在子类中可以重写toString方法、equals方法等，但是不能重写getClass方法、wait方法等，因为这些方法都是使用fianl修饰的。

我们也可以定义final修饰的方法：

```java
public class Person{
    public final void print(){}
}

//编译报错
public class Student extends Person{
    public void print(){
    }
}
```

**3、修饰变量**

用final修饰的**变量**表示**常量**，只能被赋一次值。使用final修饰的变量也就成了常量了，因为值不会再变了。

【修饰局部变量】

```java
public class Person{
    public void print(final int a){
    //编译报错,不能再次赋值,传参的时候已经赋过了
    a = 1;
    }
}

public class Person{
    public void print(){
        final int a;
        a = 1;
        //编译报错,不能再次赋值
        a = 2;
    }
}
```

【修饰成员变量-非静态成员变量】

```java
public class Person{
    private final int a;
}
/*
只有一次机会,可以给此变量a赋值的位置:
声明的同时赋值
匿名代码块中赋值
构造器中赋值(类中出现的所有构造器都要写)
*/
```

【修饰成员变量-静态成员变量】

```java
public class Person{
    private static final int a;
}
/*
只有一次机会,可以给此变量a赋值的位置:
声明的同时赋值
静态代码块中赋值
*/
```

【修饰引用对象】

```java
final Student s = new Student();
//编译通过
s.setName("tom");
s.setName("zs");

//编译报错,不能修改引用s指向的内存地址
s = new Student();
```

### 3、abstract修饰符

 abstract修饰符可以用来修饰方法也可以修饰类，如果修饰方法，那么该方法就是抽象方法。如果修饰类，那么该类就是抽象类。

**1、抽象类和抽象方法的关系**

抽象类中可以没有抽象方法，但是有抽象方法的类一定要声明为抽象类。

**2、语法**

```java
public abstract class Action{
    public abstract void doSomething();
}

public void doSomething(){...}
```

对于这个普通方法来讲：

"public void doSomething()"这部分是方法的声明。
"{...}"这部分是方法的实现,如果大括号中什么都没写,就叫方法的空实现

声明类的同时，加上abstract修饰符就是抽象类
声明方法的时候，加上abstract修饰符，并且去掉方法的大口号，同时结尾加上分号，该方法就是抽象方法。

### 3、特点及作用

抽象类，不能使用new关键字来创建对象，它是用来让子类继承的。 
抽象方法，只有方法的声明，没有方法的实现，它是用来让子类实现的。

注：子类继承抽象类后，需要实现抽象类中没有实现的抽象方法，否则这个子类也要声明为抽象类。

```java
public abstract class Action{
    public abstract void doSomething();
}

main:
//编译报错,抽象类不能new对象
Action a = new Action();

//子类继承抽象类
public class Eat extends Action{
    //实现父类中没有实现的抽象方法
    public void doSomething(){
        //code
    }
}

main:
Action a = new Eat();
a.doSomething();
```

注：子类继承抽象类，那么就必须要实现抽象类没有实现的抽象方法，否则该子类也要声明为抽象类。

**4、思考**

思考1 : 抽象类不能new对象，那么抽象类中有没有构造器？

> 抽象类是不能被实例化，抽象类的目的就是为实现多态中的共同点，抽象类的构造器会在子类实例化时调用，因此它也是用来实现多态中的共同点构造，不建议这样使用！

思考2 : 抽象类和抽象方法意义（为什么要编写抽象类、抽象方法）

> 打个比方，要做一个游戏。如果要创建一个角色，如果反复创建类和方法会很繁琐和麻烦。建一个抽象类
> 后。若要创建角色可直接继承抽象类中的字段和方法，而抽象类中又有抽象方法。如果一个角色有很多种
> 职业，每个职业又有很多技能，要是依次实例这些技能方法会显得想当笨拙。定义抽象方法，在需要时继
> 承后重写调用，可以省去很多代码。
>
> 总之抽象类和抽象方法起到一个框架作用。很方便后期的调用和重写
> 抽象方法是为了程序的可扩展性。重写抽象方法时即可实现同名方法但又非同目的的要求。

## 接口

### 1、接口的本质

普通类：只有具体实现
抽象类：具体实现和规范(抽象方法) 都有！
接口：只有规范！

**为什么需要接口？接口和抽象类的区别？**

- 接口就是比“抽象类”还“抽象”的“抽象类”，可以更加规范的对子类进行约束。全面地专业地实现了：规范和具体实现的分离。
- 抽象类还提供某些具体实现，接口不提供任何实现，接口中所有方法都是抽象方法。接口是完全面向规范的，规定了一批类具有的公共方法规范。
- 从接口的实现者角度看，接口定义了可以向外部提供的服务。
- 从接口的调用者角度看，接口定义了实现者能提供那些服务。
- 接口是两个模块之间通信的标准，通信的规范。如果能把你要设计的系统之间模块之间的接口定义好，就相当于完成了系统的设计大纲，剩下的就是添砖加瓦的具体实现了。大家在工作以后，做系统时往往就是使用“面向接口”的思想来设计系统。

**接口的本质探讨**

- 接口就是规范，定义的是一组规则，体现了现实世界中”如果你是…则必须能…“的思想。如果你是天使，则必须能飞。如果你是汽车，则必须能跑。
- 接口的本质是契约，就像我们人间的法律一样。制定好后大家都遵守。
- OO的精髓，是对对象的抽象，最能体现这一点的就是接口。为什么我们讨论设计模式都只针对具备了抽象能力的语言（比如c++、java、c#等），就是因为设计模式所研究的，实际上就是如何合理的去抽象。

### 2、接口与抽象类的区别

抽象类也是类，除了可以写抽象方法以及不能直接new对象之外，其他的和普通类没有什么不一样的。接口已经另一种类型了，和类是有本质的区别的，所以不能用类的标准去衡量接口。

**声明类的关键字是class，声明接口的关键字是interface。**

抽象类是用来被继承的，java中的类是单继承。

类A继承了抽象类B，那么类A的对象就属于B类型了，可以使用多态
一个父类的引用，可以指向这个父类的任意子类对象
注：继承的关键字是extends

接口是用来被类实现的，java中的接口可以被多实现。
类A实现接口B、C、D、E..，那么类A的对象就属于B、C、D、E等类型了，可以使用多态
一个接口的引用，可以指向这个接口的任意实现类对象
注：实现的关键字是implements

### 3、接口中的方法都是抽象方法

接口中可以不写任何方法，但如果写方法了，该方法必须是抽象方法

```java
public interface Action{
    public abstract void run();
    
    //默认就是public abstract修饰的
    void test();
    public void go();
}
```

### 4、接口中的变量都是静态常量

public static final修饰

接口中可以不写任何属性，但如果写属性了，该属性必须是public static final修饰的静态常量。
注：可以直接使用接口名访问其属性。因为是public static修饰的

注：声明的同时就必须赋值(因为接口中不能编写静态代码块)

```java
public interface Action{
    public static final String NAME = "tom";
    //默认就是public static final修饰的
    int AGE = 20;
}

main:
System.out.println(Action.NAME);
System.out.println(Action.AGE);
```

### 5、一个类可以实现多个接口

```java
public class Student implements A,B,C,D{
    //Student需要实现接口A B C D中所有的抽象方法
    //否则Student类就要声明为抽象类,因为有抽象方法没实现
}

main:
A s1 = new Student();
B s2 = new Student();
C s3 = new Student();
D s4 = new Student();
```

注：
s1只能调用接口A中声明的方法以及Object中的方法
s2只能调用接口B中声明的方法以及Object中的方法
s3只能调用接口C中声明的方法以及Object中的方法
s4只能调用接口D中声明的方法以及Object中的方法

注：必要时可以类型强制转换

例如 : 接口A 中有test() ， 接口B 中有run()

### 6、一个接口可以继承多个父接口

```java
public interface A{
    public void testA();
}

public interface B{
    public void testB();
}

//接口C把接口A B中的方法都继承过来了
public interface C extends A,B{
    public void testC();
}

//Student相当于实现了A B C三个接口,需要实现所有的抽象方法
//Student的对象也就同时属于A类型 B类型 C类型
public class Student implements C{
    public viod testA(){}
    public viod testB(){}
    public viod testC(){}
}

main:

C o = new Student();
System.out.println(o instanceof A);//true
System.out.println(o instanceof B);//true
System.out.println(o instanceof C);//true
System.out.println(o instanceof Student);//true
System.out.println(o instanceof Object);//true
System.out.println(o instanceof Teacher);//false

//编译报错
System.out.println(o instanceof String);
```

注：System.out.println(o instanceof X);

> 如果o是一个接口类型声明的变量，那么只要X不是一个final修饰的类，该代码就能通过编译，至于其结果是不是true，就要看变量o指向的对象的实际类型，是不是X的子类或者实现类了。

注：一个引用所指向的对象，是有可能实现任何一个接口的。(java中的多实现)

### 7、接口的作用

接口的最主要的作用是达到统一访问，就是在创建对象的时候用接口创建

【接口名】 【对象名】= new 【实现接口的类】

这样你像用哪个类的对象就可以new哪个对象了，不需要改原来的代码。

假如我们两个类中都有个function()的方法，如果我用接口，那样我new a()；就是用a的方法，new b() 就是用b的方法。

这个就叫统一访问，因为你实现这个接口的类的方法名相同，但是实现内容不同

总结：

1. Java接口中的成员变量默认都是public,static,final类型的(都可省略)，必须被显示初始化，即接口中的成员变量为常量(大写,单词之间用"_"分隔)
2. Java接口中的方法默认都是public,abstract类型的(都可省略)，没有方法体,不能被实例化
3. Java接口中只能包含public,static,final类型的成员变量和public,abstract类型的成员方法
4. 接口中没有构造方法,不能被实例化
5. 一个接口不能实现(implements)另一个接口,但它可以继承多个其它的接口
6. Java接口必须通过类来实现它的抽象方法
7. 当类实现了某个Java接口时，它必须实现接口中的所有抽象方法，否则这个类必须声明为抽象类
8. 不允许创建接口的实例（实例化），但允许定义接口类型的引用变量，该引用变量引用实现了这个接口的类的实例
9. 一个类只能继承一个直接的父类，但可以实现多个接口，间接的实现了多继承。

```java
interface SwimInterface{
    void swim();
}

class Fish{
    int fins=4;
}

class Duck {
    int leg=2;
    void egg(){};
}

class Goldfish extends Fish implements SwimInterface {
    @Override
    public void swim() {
        System.out.println("Goldfish can swim ");
    }
}

class SmallDuck extends Duck implements SwimInterface {
    public void egg(){
        System.out.println("SmallDuck can lay eggs ");
    }
    @Override
    public void swim() {
  	  System.out.println("SmallDuck can swim ");
    }
}

public class InterfaceDemo {
    public static void main(String[] args) {
        Goldfish goldfish=new Goldfish();
        goldfish.swim();
        
        SmallDuck smallDuck= new SmallDuck();
        smallDuck.swim();
        smallDuck.egg();
    }
}
```

## 内部类

上一小节，我们学习了接口，在以后的工作中接口是我们经常要碰到的，所以一定要多去回顾。接下来介绍一下内部类。很多时候我们创建类的对象的时候并不需要使用很多次，每次只使用一次，这个时候我们就可以使用内部类了。

### 1、内部类概述

内部类就是在一个类的内部在定义一个类，比如，A类中定义一个B类，那么B类相对A类来说就称为内部类，而A类相对B类来说就是外部类了。

内部类不是在一个java源文件中编写俩个平行的俩个类，而是在一个类的内部再定义另外一个类。 我们可以把外边的类称为外部类，在其内部编写的类称为内部类。

内部类分为四种：

1. 成员内部类
2. 静态内部类
3. 局部内部类
4.  匿名内部类

### 2、成员内部类

**成员内部类（实例内部类、非静态内部类）**

注：成员内部类中不能写静态属性和方法

【定义一个内部类】

```java
//在A类中申明了一个B类，此B类就在A的内部，并且在成员变量的位置上，所以就称为成员内部类
public class Outer {
    private int id;
    public void out(){
        System.out.println("这是外部类方法");
    }
    
    class Inner{
        public void in(){
     	   System.out.println("这是内部类方法");
        }
    }
}
```

【实例化内部类】

实例化内部类，首先需要实例化外部类，通过外部类去调用内部类

```java
public class Outer {
    private int id;
    public void out(){
  	  System.out.println("这是外部类方法");
    }
    
    class Inner{
        public void in(){
        System.out.println("这是内部类方法");
    }
    }
}

public class Test{
    public static void main(String[] args) {
        //实例化成员内部类分两步
        //1、实例化外部类
        Outer outObject = new Outer();
        //2、通过外部类调用内部类
        Outer.Inner inObject = outObject.new Inner();
        //测试，调用内部类中的方法
        inObject.in();//打印：这是内部类方法
    }
}
```

分析：想想如果你要使用一个类中方法或者属性，你就必须要先有该类的一个对象，同理，一个类在另 一个类的内部，那么想要使用这个内部类，就必须先要有外部类的一个实例对象，然后在通过该对象去使用内部类。

【成员内部类能干什么？】

- 访问外部类的所有属性(这里的属性包括私有的成员变量，方法)

```java
public class Outer {
    private int id;
    public void out(){
        System.out.println("这是外部类方法");
    }
    
    class Inner{
        public void in(){
            System.out.println("这是内部类方法");
        }
        //内部类访问外部类私有的成员变量
        public void useId(){
            System.out.println(id+3);。
        }
        //内部类访问外部类的方法
        public void useOut(){
            out();
        }
    }
}

public class Test{
    public static void main(String[] args) {
        //实例化成员内部类分两步
        //1、实例化外部类
        Outer outObject = new Outer();
        //2、通过外部类调用内部类
        Outer.Inner inObject = outObject.new Inner();
        //测试
        inObject.useId();//打印3，因为id初始化值为0，0+3就为3，其中在内部类就使用了外部类的私有成员变量id。
        inObject.useOut();//打印：这是外部类方法
    }
}
```

- 如果内部类中的变量名和外部类的成员变量名一样，要通过创建外部类对象"."属性来访问外部类属性，通过this.属性访问内部类成员属性

```java
public class Outer {
    private int id;//默认初始化0

    public void out() {
        System.out.println("这是外部类方法");
    }

    class Inner {
        private int id = 8; //这个id跟外部类的属性id名称一样。

        public void in() {
            System.out.println("这是内部类方法");
        }

        public void test() {
            System.out.println(id);//输出8，内部类中的变量会暂时将外部类的成员变量给隐藏
            // 如何调用外部类的成员变量呢？通过Outer.this
            // 想要知道为什么能通过这个来调用，就得明白下面这个原理
            // 想实例化内部类对象，就必须通过外部类对象，当外部类对象来new出内部类对象时，会把自己(外部类对象)的引用传到了内部类中，
            // 所以内部类就可以通过Outer.this来访问外部类的属性和方法
            // 到这里，你也就可以知道为什么内部类可以访问外部类的属性和方法，这里由于有两个相同的属性名称，

            // 所以需要显示的用Outer.this来调用外部类的属性，平常如果属性名不重复
            // 那么我们在内部类中调用外部类的属性和方法时，前面就隐式的调用了Outer.this。
            System.out.println(Outer.this.id);//输出外部类的属性id。也就是输出0
        }
    }
}
```

借助成员内部类，来总结内部类(包括4种内部类)的通用用法：

1. 要想访问内部类中的内容，必须通过外部类对象来实例化内部类。

2. 能够访问外部类所有的属性和方法，原理就是在通过外部类对象实例化内部类对象时，外部类对象把自己的引用传进了内部类，使内部类可以用通过Outer.this去调用外部类的属性和方法。

   一般都是隐式调用了，但是当内部类中有属性或者方法名和外部类中的属性或方法名相同的时候，就需要通过显式调用Outer.this了。

【写的一个小例子】

```java
public class MemberInnerClassTest {
    private String name;
    private static int age;

    public void run() {
    }

    public static void go() {
    }

    public class MemberInnerClass {
        private String name;

        //内部类访问外部类
        public void test(String name) {
            System.out.println(name);
            System.out.println(this.name);
            System.out.println(MemberInnerClassTest.this.name);
            System.out.println(MemberInnerClassTest.age);
            MemberInnerClassTest.this.run();
            MemberInnerClassTest.go();
        }
    }

    //外部类访问成员内部类
    //成员内部类的对象要 依赖于外部类的对象的存在
    public void test() {
        //MemberInnerClass mic = MemberInnerClassTest.this.new MemberInnerClass();
        //MemberInnerClass mic = this.new MemberInnerClass();
        MemberInnerClass mic = new MemberInnerClass();
        mic.name = "tom";
        mic.test("hua");
    }

    public static void main(String[] args) {
        //MemberInnerClass mic = new MemberInnerClass();这个是不行的，this是动态的。
        //所以要使用要先创建外部类对象，才能使用
        MemberInnerClassTest out = new MemberInnerClassTest();
        MemberInnerClass mic = out.new MemberInnerClass();
        //如果内部类是private,则不能访问，只能铜鼓内部方法来调用内部类
        mic.name = "jik";
        mic.test("kkk");
    }
}
```

### 3、静态内部类

看到名字就知道，使用static修饰的内部类就叫静态内部类。

既然提到了static，那我们就来复习一下它的用法：一般只修饰变量和方法，平常不可以修饰类，但是内部类却可以被static修饰。

1. static修饰成员变量：整个类的实例共享静态变量
2. static修饰方法：静态方法，只能够访问用static修饰的属性或方法，而非静态方法可以访问static修饰的方法或属性
3. 被static修饰了的成员变量和方法能直接被类名调用。
4. static不能修饰局部变量，切记，不要搞混淆了，static平常就用来修饰成员变量和方法。

例子：

```java
public class StaticInnerClassTest {

    private String name;
    private static int age;

    public void run() {
    }

    public static void go() {
    }

    //外部类访问静态内部类
    public void test() {
        StaticInnerClass sic = new StaticInnerClass(); //静态的内部类不需要依赖外部类，所以不用this
        sic.name = "tom";

        sic.test1("jack");
        StaticInnerClass.age = 10;
        StaticInnerClass.test2("xixi");
    }

    private static class StaticInnerClass {
        private String name;
        private static int age;

        public void test1(String name) {
            System.out.println(name);
            System.out.println(this.name);
            System.out.println(StaticInnerClass.age);
            System.out.println(StaticInnerClassTest.age);
            //System.out.println(StaticInnerClassTest.this.name);静态类不能访问非静态属性
            StaticInnerClassTest.go();
            //StaticInnerClassTest.this.run();静态类不能访问非静态方法
        }

        public static void test2(String name) {
            //只能访问自己和外部类的静态属性和方法
            System.out.println(name);
            //System.out.println(this.name);静态方法里面连自己类的非静态属性都不能访问
            System.out.println(StaticInnerClass.age);
            System.out.println(StaticInnerClassTest.age);
            //System.out.println(StaticInnerClassTest.this.name);静态方法不能访问非静态属性
            StaticInnerClassTest.go();
            //StaticInnerClassTest.this.run();静态方法不能访问非静态方法
        }
    }
}
```

注意：

1. 我们上面说的内部类能够调用外部类的方法和属性，在静态内部类中就行了，因为静态内部类没有 了指向外部类对象的引用。除非外部类中的方法或者属性也是静态的。这就回归到了static关键字的用法。

2. 静态内部类能够直接被外部类给实例化，不需要使用外部类对象

   ```jav
   Outer.Inner inner = new Outer.Inner();
   ```

3. 静态内部类中可以声明静态方法和静态变量，但是非静态内部类中就不可以声明静态方法和静态变量

### 4、局部内部类

局部内部类是在一个方法内部声明的一个类
局部内部类中可以访问外部类的成员变量及方法
局部内部类中如果要访问该内部类所在方法中的局部变量，那么这个局部变量就必须是final修饰的

```java
public class Outer {
    private int id;

    //在method01方法中有一个Inner内部类，这个内部类就称为局部内部类
    public void method01() {
        class Inner {
            public void in() {
                System.out.println("这是局部内部类");
            }
        }
    }
}
```

局部内部类一般的作用跟在成员内部类中总结的差不多，但是有两个要注意的地方：

**1、在局部内部类中，如果要访问局部变量，那么该局部变量要用final修饰**

为什么需要使用final？

final修饰变量：变为常量，会在常量池中放着，逆向思维想这个问题，如果不实用final修饰，当局部内部类被实例化后，方法弹栈，局部变量随着跟着消失，这个时候局部内部类对象在想去调用该局部变量，就会报错，因为该局部变量已经没了，当局部变量用fanal修饰后，就会将其加入常量池中，即使方法弹栈了，该局部变量还在常量池中呆着，局部内部类也就是够调用。所以局部内部类想要调用局部变 量时，需要使用final修饰，不使用，编译度通不过。

```java
public class Outer {
    private int id;

    public void method01() {
        //这个就是局部变量cid。要让局部内部类使用，就得变为final并且赋值，如果不使用final修饰，就会报错
        final int cid = 3;
        class Inner {
            //内部类的第一个方法
            public void in() {
                System.out.println("这是局部内部类");
            }

            //内部类中的使用局部变量cid的方法
            public void useCid() {
                System.out.println(cid);
            }
        }
    }
}
```

**2、局部内部类不能通过外部类对象直接实例化，而是在方法中实例化出自己来，然后通过内部类对象 调用自己类中的方法。**

看下面例子就知道如何用了。

```java
public class Outer {
    private int id;

    public void out() {
        System.out.println("外部类方法");
    }

    public void method01() {
        class Inner {
            public void in() {
                System.out.println("这是局部内部类");
            }
        }
        //关键在这里，如需要在method01方法中自己创建内部类实例，
        // 然后调用内部类中的方法，等待外部类调用method01方法，
        // 就可以执行到内部类中的方法了。
        Inner In = new Inner();
        In.in();
    }
}
```

使用局部内部类需要注意的地方就刚才上面说的：

1. 在局部内部类中，如果要访问局部变量，那么该局部变量要用final修饰

2. 如何调用局部内部类方法。

   ```java
   public class LocalInnerClassTest {
       private String name;
       private static int age;
   
       public void run() {
       }
   
       public static void go() {
       }
   
       //局部内部类要定义在方法中
       public void test() {
           final String myname = "";
           class LocalInnerClass {
               private String name;
   
               // private static int age;不能定义静态属性
               public void test(String name) {
                   System.out.println(name);
                   System.out.println(this.name);
                   System.out.println(myname);
                   System.out.println(LocalInnerClassTest.this.name);
                   LocalInnerClassTest.this.run();
                   LocalInnerClassTest.go();
               }
           }
           // 局部内部类只能在自己的方法中用
           // 因为局部内部类相当于一个局部变量，出了方法就找不到了。
           LocalInnerClass lic = new LocalInnerClass();
           lic.name = "tom";
           lic.test("test");
           
       }
       
   }
   ```

   

### 5、匿名内部类

在这四种内部类中，以后的工作可能遇到最多的是匿名内部类，所以说匿名内部类是最常用的一种 内部类。

什么是匿名对象？如果一个对象只要使用一次，那么我们就是需要new Object().method()。 就可以了，而不需要给这个实例保存到该类型变量中去。这就是匿名对象。

```java
public class Test {
    public static void main(String[] args) {
        //讲new出来的Apple实例赋给apple变量保存起来，但是我们只需要用一次，就可以这样写
        Apple apple = new Apple();
        apple.eat();
        //这种就叫做匿名对象的使用，不把实例保存到变量中。
        new Apple().eat();
    }
}

class Apple{
    public void eat(){
        System.out.println("我要被吃了");
	}
}
```

匿名内部类跟匿名对象是一个道理：

匿名对象：我只需要用一次，那么我就不用声明一个该类型变量来保存对象了，

匿名内部类：我也只需要用一次，那我就不需要在类中先定义一个内部类，而是等待需要用的时候，我就在临时实现这个内部类，因为用次数少，可能就这一次，那么这样写内部类，更方便。不然先写出一 个内部类的全部实现来，然后就调用它一次，岂不是用完之后就一直将其放在那，那就没必要那样。

1. 匿名内部类需要依托于其他类或者接口来创建
   - 如果依托的是类，那么创建出来的匿名内部类就默认是这个类的子类
   - 如果依托的是接口，那么创建出来的匿名内部类就默认是这个接口的实现类。
2. 匿名内部类的声明必须是在使用new关键字的时候
   - 匿名内部类的声明及创建对象必须一气呵成，并且之后能反复使用，因为没有名字

【示例】

A是一个类(普通类、抽象类都可以)，依托于A类创建一个匿名内部类对象

```java
main:

A a = new A(){
    //实现A中的抽象方法
    //或者重写A中的普通方法
};

注:这个大括号里面其实就是这个内部类的代码,只不过是声明该内部类的同时就是要new创建了其对象,
并且不能反复使用,因为没有名字。
    
例如:
B是一个接口，依托于B接口创建一个匿名内部类对象

B b = new B(){
	//实现B中的抽象方法
};
```

1. 匿名内部类除了依托的类或接口之外，不能指定继承或者实现其他类或接口，同时也不能被其他类所继承，因为没有名字。
2. 匿名内部中，我们不能写出其构造器，因为没有名字。
3. 匿名内部中，除了重写上面的方法外，一般不会再写其他独有的方法，因为从外部不能直接调用到。(间接是调用到的)

```java
public interface Work{
    void doWork();
}

public class AnonymousOutterClass{
    private String name;
    private static int age;
    public void say(){}
    public static void go(){}
    
    public void test(){
        final int i = 90;
        
        Work w = new Work(){
            public void doWork(){
                System.out.println(AnonymousOutterClass.this.name);
                System.out.println(AnonymousOutterClass.age);
                AnonymousOutterClass.this.say();
                AnonymousOutterClass.go();
                
                System.out.println(i);
            }
        };
        w.doWork();
    }
}
```

我们可以试一下不 用匿名内部类 和 用匿名内部类 实现一个接口中的方法的区别

【不用匿名内部类】

```java
public class Test {
    public static void main(String[] args) {
        // 如果我们需要使用接口中的方法，我们就需要走3步，
        // 1、实现接口 2、创建实现接口类的实例对象 3、通过对象调用方法
        //第二步
        Test02 test = new Test02();
        //第三步
        test.method();
    }
}

//接口Test1
interface Test01{
    public void method();
}

//第一步、实现Test01接口
class Test02 implements Test01{
    @Override
    public void method() {
        System.out.println("实现了Test接口的方法");
    }
}
```

【使用匿名内部类】

```java
public class Test {
    public static void main(String[] args) {
		//如果我们需要使用接口中的方法，我们只需要走一步，就是使用匿名内部类，直接将其类的对象创建出来。
        new Test1(){
            public void method(){
                System.out.println("实现了Test接口的方法");
            }
        }.method();
    }
}

interface Test1{
    public void method();
}
```

解析：

其实只要明白一点，new Test1( ){ 实现接口中方法的代码 }; 

Test1(){...} 这个的作用就是将接口给实现了，只不过这里实现该接口的是一个匿名类，也就是说这个类没名字，只能使用这一次，我们知道了这是一个类， 将其new出来，就能获得一个实现了Test1接口的类的实例对象，通过该实例对象，就能调用该类中的方法了，因为其匿名类是在一个类中实现的，所以叫其匿名内部类。

不要纠结为什么 Test1( ){...} 就相当于实现了Test1接口，这其中的原理等足够强大了，在去学习，不要钻牛角尖，这里就仅仅是需要知道他的作用是什么，做了些什么东西就行。


# JavaSE-常用类

[[toc]]



## Object类


理论上Object类是所有类的父类，即直接或间接的继承java.lang.Object类。

由于所有的类都继承在Object类，因此省略了extends Object关键字。

该类中主要有以下方法：

- toString( )
- getClass( )
- equals( )
- clone( )
- finalize( )

其中toString()，getClass()，equals是其中最重要的方法。

查看Object类源码

![image-20210329172035497](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210329172035497.png)

看图可知，在jdk15中最后一个方法过时了，但我们运营一般都是jdk1.8

**注意： Object类中的getClass(),notify(),notifyAll(),wait()等方法被定义为final类型，因此不能重写。**

### 1  clone() 方法

详解文章：https://blog.csdn.net/zhangjg_blog/article/details/18369201#0-qzone-1-28144-d020d2d2a4e8d1a374a433f596ad1440

```java
 protected native Object clone() throws CloneNotSupportedException;
```

clone顾名思义就是复制， 在Java语言中， clone方法被对象调用，所以会复制对象。所谓的复制对象，首先要分配一个和源对象同样大小的空间，在这个空间中创建一个新的对象。那么在java语言中，有几种方式可以创建对象呢？

- 使用new操作符创建一个对象
- 使用clone方法复制一个对象

那么这两种方式有什么相同和不同呢？ new操作符的本意是分配内存。程序执行到new操作符时， 首先去看new操作符后面的类型，因为知道了类型，才能知道要分配多大的内存空间。分配完内存之后， 再调用构造函数，填充对象的各个域，这一步叫做对象的初始化，构造方法返回后，一个对象创建完毕，可以把他的引用（地址）发布到外部，在外部就可以使用这个引用操纵这个对象。而clone在第一步是和new相似的， 都是分配内存，调用clone方法时，分配的内存和源对象（即调用clone方法的对象）相同，然后再使用原对象中对应的各个域，填充新对象的域，填充完成之后，clone方法返回，一个新的相同的对象被创建，同样可以把这个新对象的引用发布到外部。

**clone与copy的区别**

假设现在有一个Employee对象，Employee tobby = new Employee(“CMTobby”,5000)

通常我们会有这样的赋值Employee cindyelf = tobby，这个时候只是简单了copy了一下reference。cindyelf和tobby都指向内存中同一个object，这样cindyelf或者tobby的一个操作都可能影响到对方。打个比方，如果我们通过cindyelf.raiseSalary()方法改变了salary域的值，那么tobby通过getSalary()方法，得到的就是修改之后的salary域的值，显然这不是我们愿意看到的。我们希望得到tobby的一个精确拷贝，同时两者互不影响，这时候， 我们就可以使用Clone来满足我们的需求。Employee cindy=tobby.clone()，这时会生成一个新的Employee对象，并且和tobby具有相同的属性值和方法。

**Shallow Clone与Deep Clone**

 浅克隆和深克隆

- **浅克隆：**

  是指拷贝对象时仅仅拷贝对象本身（包括对象中的基本变量），而不拷贝对象包含的引用指向的对象。

- **深克隆：**

  不仅拷贝对象本身，而且拷贝对象包含的引用指向的所有对象。

举例来说更加清楚。

![image-20210329221102470](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210329221102470.png)

主要是JAVA里除了8种基本类型传参数是值传递，其他的类对象传参数都是引用，我们有时候不希望在方法里将参数改变，这是就需要在类中复写clone方法（实现深复制）。

Clone是如何完成的呢？Object在对某个对象实施Clone时对其是一无所知的，它仅仅是简单地执行域对域的copy，这就是Shallow Clone。这样，问题就来了咯。

以Employee为例，它里面有一个域hireDay不是基本数据类型的变量，而是一个reference变量，经过Clone之后就会产生一个新的Date型的reference，

它和原始对象中对应的域指向同一个Date对象，这样克隆类就和原始类共享了一部分信息，而这样显然是不利的，过程下图所示：

![image-20210329220750868](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210329220750868-1617026885587.png)

这个时候我们就需要进行deep Clone了，对那些非基本类型的域进行特殊的处理，例如本例中的 hireDay。我们可以重新定义Clone方法，对hireDay做特殊处理，如下代码所示：

```java
class Employee implements Cloneable {
    public Object clone() throws CloneNotSupportedException {
        Employee cloned = (Employee) super.clone();
        cloned.hireDay = (Date) hireDay.clone()
        return cloned;
    }
}
```

**clone方法的保护机制**

在Object中Clone()是被声明为protected的，这样做是有一定的道理的，以Employee类为例，通过声明为protected，就可以保证只有Employee类里面才能“克隆”Employee对象。

**clone方法的使用**

什么时候使用shallow Clone，什么时候使用deep Clone，这个主要看具体对象的域是什么性质的，基本型别还是reference variable

调用Clone()方法的对象所属的类(Class)必须implements Clonable接口，否则在调用Clone方法的时候 会抛出CloneNotSupportedException

推荐： [浅克隆(ShallowClone)和深克隆(DeepClone)区别以及实现](https://blog.csdn.net/qiaziliping/article/details/105566397)

### 2  toString()方法

```java
public String toString() {
	return getClass().getName() + "@" + Integer.toHexString(hashCode());
}
```

Object 类的 toString 方法返回一个字符串，该字符串由类名（对象是该类的一个实例）、at 标记符“@” 和此对象[哈希码](https://baike.baidu.com/item/%E5%93%88%E5%B8%8C%E7%A0%81/5035512?fr=aladdin)的无符号十六进制表示组成。

该方法用得比较多，**一般子类都有覆盖。**

```java
public static void main(String[] args){
    Object o1 = new Object();
    System.out.println(o1.toString());
}
```

### 3  getClass()方法

```java
public final native Class<?> getClass();
```

返回次Object的运行时类类型。

不可重写，要调用的话，一般和getName()联合使用，如getClass().getName();

```java
public static void main(String[] args) {
    Object o = new Object();
    System.out.println(o.getClass());
    //class java.lang.Object
}
```

### 4  finalize()方法

```java
protected void finalize() throws Throwable { }
```

该方法用于释放资源。因为无法确定该方法什么时候被调用，很少使用。

Java允许在类中定义一个名为finalize()的方法。它的工作原理是：一旦垃圾回收器准备好释放对象占用的存储空间，将首先调用其finalize()方法。并且在下一次垃圾回收动作发生时，才会真正回收对象占用的内存。

关于垃圾回收，有三点需要记住：

1、对象可能不被垃圾回收。只要程序没有濒临存储空间用完的那一刻，对象占用的空间就总也得不到释放。

2、垃圾回收并不等于“析构”。

​	科普：析构函数(destructor) 与构造函数相反，当对象结束其生命周期，如对象所在的函数已调用完毕时，系统自动执行析构函数。析构函数往往用来做“清理善后” 的工作（例如在建立对象时用new开辟了一片内存空间，delete会自动调用析构函数后释放内存）。

3、垃圾回收只与内存有关。使用垃圾回收的唯一原因是为了回收程序不再使用的内存。

**finalize()的用途：**

无论对象是如何创建的，垃圾回收器都会负责释放对象占据的所有内存。

这就将对finalize()的需求限制到一种特殊情况，即通过某种创建对象方式以外的方式为对象分配了存储空间。不过这种情况一般发生在使用“本地方法”的情况下，本地方法是一种在Java中调用非Java代码的方式。

### 5  equals()方法

```java
public boolean equals(Object obj) {
	return (this == obj);
}
```

Object中的equals方法是直接判断this和obj本身的值是否相等，即用来判断调用equals的对象和形参 obj所引用的对象是否是同一对象

所谓同一对象就是指内存中同一块存储单元，如果this和obj指向的是同一块内存对象，则返回true，如果this和obj指向的不是同一块内存，则返回false。

注意：即便是内容完全相等的两块不同的内存对象，也返回false。

如果是同一块内存，则object中的equals方法返回true，如果是不同的内存，则返回false

如果希望不同内存但相同内容的两个对象equals时返回true，则我们需要重写父类的equal方法

String类已经重写了object中的equals方法（这样就是比较内容是否相等了）

**查看String类源码equals方法**

```java
public boolean equals(Object anObject) {
    if (this == anObject) {
        return true;
    }
    if (anObject instanceof String) {
        String anotherString = (String)anObject;
        int n = value.length;
        if (n == anotherString.value.length) {
            char v1[] = value;
            char v2[] = anotherString.value;
            int i = 0;
            while (n-- != 0) {
                if (v1[i] != v2[i])
                    return false;
                i++;
            }
            return true;
        }
    }
    return false;
}
```

### 6  hashCode()方法

```java
public native int hashCode();
```

返回该对象的哈希码值。

该方法用于哈希查找，可以减少在查找中使用equals的次数，重写了equals方法一般都要重写 hashCode方法。这个方法在一些具有哈希功能的Collection中用到。

一般必须满足obj1.equals(obj2)==true。可以推出obj1.hashCode() == obj2.hashCode()，但是 hashCode相等不一定就满足equals。不过为了提高效率，应该尽量使上面两个条件接近等价。

### 7  wait()方法

```java
public final void wait(long timeoutMillis, int nanos) throws InterruptedException {
    if (timeoutMillis < 0) {
        throw new IllegalArgumentException("timeoutMillis value is negative");
    }

    if (nanos < 0 || nanos > 999999) {
        throw new IllegalArgumentException(
                            "nanosecond timeout value out of range");
    }

    if (nanos > 0 && timeoutMillis < Long.MAX_VALUE) {
        timeoutMillis++;
    }

    wait(timeoutMillis);
}
```

可以看到有三种重载，wait什么意思呢？

![image-20210329225829453](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210329225829453.png)

方法中的异常：

![image-20210329225858173](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210329225858173.png)

wait方法就是使当前线程等待该对象的锁，当前线程必须是该对象的拥有者，也就是具有该对象的锁。 

wait()方法一直等待，直到获得锁或者被中断。wait(long timeout)设定一个超时间隔

如果在规定时间内没有获得锁就返回。

调用该方法后当前线程进入睡眠状态，直到以下事件发生。

（1）其他线程调用了该对象的notify方法。 
（2）其他线程调用了该对象的notifyAll方法。 
（3）其他线程调用了interrupt中断该线程。 
（4）时间间隔到了。

此时该线程就可以被调度了，如果是被中断的话就抛出一个InterruptedException异常。

### 8  notify()方法

```java
public final native void notify();
```

该方法唤醒在该对象上等待的某个线程。

```java
public final native void notifyAll();
```

该方法唤醒在该对象上等待的所有线程。

## 包装类

### 1、包装类介绍

虽然 Java 语言是典型的面向对象编程语言，但其中的八种基本数据类型并不支持面向对象编程，基本类型的数据不具备“对象”的特性——不携带属性、没有方法可调用。 沿用它们只是为了迎合人类根深蒂固的习惯，并的确能简单、有效地进行常规数据处理。

这种借助于非面向对象技术的做法有时也会带来不便，比如引用类型数据均继承了 Object 类的特性，要转换为 String 类型（经常有这种需要）时只要简单调用 Object 类中定义的toString()即可，而基本数据类型转换为 String 类型则要麻烦得多。为解决此类问题 ，Java为每种基本数据类型分别设计了对应的类，称之为包装类(Wrapper Classes)，也有教材称为外覆类或数据类型类。

| 基本数据类型 | 对应的包装类 |
| ------------ | ------------ |
| byte         | Byte         |
| short        | Short        |
| int          | Integer      |
| long         | Long         |
| char         | Character    |
| float        | Float        |
| double       | Double       |
| boolean      | Boolean      |

每个包装类的对象可以封装一个相应的基本类型的数据，并提供了其它一些有用的方法。包装类对象一 经创建，其内容（所封装的基本类型数据值）不可改变。

基本类型和对应的包装类可以相互装换：

- 由基本类型向对应的包装类转换称为装箱，例如把 int 包装成 Integer 类的对象；
- 包装类向对应的基本类型转换称为拆箱，例如把 Integer 类的对象重新简化为 int。

### 2、包装类的应用

**1、 实现 int 和 Integer 的相互转换**

可以通过 Integer 类的构造方法将 int 装箱，通过 Integer 类的 intValue 方法将 Integer 拆箱。

```java
public static void main(String[] args) {
    int m = 500;
    Integer obj = new Integer(m); // 手动装箱
    int n = obj.intValue(); // 手动拆箱
    System.out.println("n = " + n);
    
    Integer obj1 = new Integer(500);
    System.out.println("obj 等价于 obj1？" + obj.equals(obj1));
}
```

**2、 将字符串转换为整数**

Integer 类有一个静态的 paseInt() 方法，可以将字符串转换为整数，语法为：

```java
parseInt(String s, int radix);
//s 为要转换的字符串，radix 为进制，可选，默认为十进制。
```

下面的代码将会告诉你什么样的字符串可以转换为整数：

```java
public static void main(String[] args) {
    String[] strs = {"123", "123abc", "abc123", "abcxyz"};
    for (String str : strs) {
        try {
            int m = Integer.parseInt(str, 10);
            System.out.println(str + " 可以转换为整数 " + m);
        } catch (Exception e) {
            System.out.println(str + " 无法转换为整数");
        }
    }
}
```

结果：

>  123 可以转换为整数 123 
>  123abc 无法转换为整数 
>  abc123 无法转换为整数 
>  abcxyz 无法转换为整数

###  3、将整数转换为字符串

Integer 类有一个静态的 toString() 方法，可以将整数转换为字符串。或者直接在整数后面加空字符串！

```java
public static void main(String[] args) {
    int m = 500;
    String s = Integer.toString(m);
    
    String s2 = m +"";
    System.out.println("s = " + s);
}
```

### 3、自动拆箱和装箱

上面的例子都需要手动实例化一个包装类，称为手动拆箱装箱。Java 1.5(5.0) 之前必须手动拆箱装箱。

Java 1.5 之后可以自动拆箱装箱，也就是在进行基本数据类型和对应的包装类转换时，系统将自动进行，这将大大方便程序员的代码书写。

```java
public static void main(String[] args) {
    int m = 500;
    Integer obj = m; // 自动装箱
    int n = obj; // 自动拆箱
    System.out.println("n = " + n);
    Integer obj1 = 500;
    System.out.println("obj 等价于 obj1？" + obj.equals(obj1));
}
//结果：
// n = 500
// obj 等价于 obj1？true
```

自动装箱与拆箱的功能事实上是编译器来帮您的忙，编译器在编译时期依您所编写的语法，决定是否进行装箱或拆箱动作。例如：

```java
Integer i = 100;
//相当于编译器自动为您作以下的语法编译：
Integer i = new Integer(100);
```

所以自动装箱与拆箱的功能是所谓的“编译器蜜糖”(Compiler Sugar)，虽然使用这个功能很方便，但在程序运行阶段你要了解Java的语义。例如下面的程序是可以通过编译的：

```java
Integer i = null;
int j = i;
```

这样的语法在编译时期是合法的，但是在运行时期会有错误，因为这种写法相当于：

```java
Integer i = null;
int j = i.intValue();
```

null表示i 没有参考至任何的对象实体，它可以合法地指定给对象参考名称。由于实际上 i 并没有参考至任何的对象，所以也就不可能操作intValue()方法，这样上面的写法在运行时会出现NullPointerException 错误。

自动拆箱装箱是常用的一个功能，需要重点掌握。

一般地，当需要使用数字的时候，我们通常使用内置数据类型，如：byte、int、long、double 等。然而，在实际开发过程中，我们经常会遇到需要使用对象，而不是内置数据类型的情形。为了解决这个问题，Java 语言为每一个内置数据类型提供了对应的包装类。

所有的包装类（Integer、Long、Byte、Double、Float、Short）都是抽象类 Number 的子类。

## Math类

Java 的 Math 包含了用于执行基本数学运算的属性和方法，如初等指数、对数、平方根和三角函数。

Math 的方法都被定义为 static 形式，通过 Math 类可以在主函数中直接调用

**【演示：查看Math类的源码】**

```java
public final class Math{
	//数学方法
}
```

【常用值与函数】

Math.PI 记录的圆周率
Math.E 记录e的常量

Math中还有一些类似的常量，都是一些工程数学常用量。

Math.abs 求绝对值
Math.sin 正弦函数 Math.asin 反正弦函数
Math.cos 余弦函数 Math.acos 反余弦函数
Math.tan 正切函数 Math.atan 反正切函数 Math.atan2 商的反正切函数
Math.toDegrees 弧度转化为角度 Math.toRadians 角度转化为弧度
Math.ceil 得到不小于某数的最大整数
Math.floor 得到不大于某数的最大整数
Math.IEEEremainder 求余
Math.max 求两数中最大
Math.min 求两数中最小
Math.sqrt 求开方
Math.pow 求某数的任意次方, 抛出ArithmeticException处理溢出异常

Math.exp 求e的任意次方
Math.log10 以10为底的对数
Math.log 自然对数
Math.rint 求距离某数最近的整数（可能比某数大，也可能比它小）
Math.round 同上，返回int型或者long型（上一个函数返回double型）
Math.random 返回0，1之间的一个随机数

```java
public static void main(String[] args) {
    /**
     *Math.sqrt()//计算平方根
     *Math.cbrt()//计算立方根
     *Math.pow(a, b)//计算a的b次方
     *Math.max( , );//计算最大值
     *Math.min( , );//计算最小值
     */
    System.out.println(Math.sqrt(16)); //4.0
    System.out.println(Math.cbrt(8)); //2.0
    System.out.println(Math.pow(3, 2)); //9.0
    System.out.println(Math.max(2.3, 4.5));//4.5
    System.out.println(Math.min(2.3, 4.5));//2.3
    /**
     * abs求绝对值
     */
    System.out.println(Math.abs(-10.4)); //10.4
    System.out.println(Math.abs(10.1)); //10.1
    /**
     * ceil天花板的意思，就是返回大的值
     */
    System.out.println(Math.ceil(-10.1)); //-10.0
    System.out.println(Math.ceil(10.7)); //11.0
    System.out.println(Math.ceil(-0.7)); //-0.0
    System.out.println(Math.ceil(0.0)); //0.0
    System.out.println(Math.ceil(-0.0)); //-0.0
    System.out.println(Math.ceil(-1.7)); //-1.0
    /**
     * floor地板的意思，就是返回小的值
     */
    System.out.println(Math.floor(-10.1)); //-11.0
    System.out.println(Math.floor(10.7)); //10.0
    System.out.println(Math.floor(-0.7)); //-1.0
    System.out.println(Math.floor(0.0)); //0.0
    System.out.println(Math.floor(-0.0)); //-0.0
    /**
     * random 取得一个大于或者等于0.0小于不等于1.0的随机数 [0,1)
     */
    System.out.println(Math.random()); //小于1大于0的double类型的数
    System.out.println(Math.random() + 1);//大于1小于2的double类型的数
    /**
     * rint 四舍五入，返回double值
     * 注意.5的时候会取偶数 异常的尴尬=。=
     */
    System.out.println(Math.rint(10.1)); //10.0
    System.out.println(Math.rint(10.7)); //11.0
    System.out.println(Math.rint(11.5)); //12.0
    System.out.println(Math.rint(10.5)); //10.0
    System.out.println(Math.rint(10.51)); //11.0
    System.out.println(Math.rint(-10.5)); //-10.0
    System.out.println(Math.rint(-11.5)); //-12.0
    System.out.println(Math.rint(-10.51)); //-11.0
    System.out.println(Math.rint(-10.6)); //-11.0
    System.out.println(Math.rint(-10.2)); //-10.0
    /**
     * round 四舍五入，float时返回int值，double时返回long值
     */
    System.out.println(Math.round(10.1)); //10
    System.out.println(Math.round(10.7)); //11
    System.out.println(Math.round(10.5)); //11
    System.out.println(Math.round(10.51)); //11
    System.out.println(Math.round(-10.5)); //-10
    System.out.println(Math.round(-10.51)); //-11
    System.out.println(Math.round(-10.6)); //-11
    System.out.println(Math.round(-10.2)); //-10
}
```

## Random类

Java中存在着两种Random函数：

 **1、java.lang.Math.Random;**

调用这个Math.Random()函数能够返回带正号的double值，该值大于等于0.0且小于1.0，即取值范围是 [0.0,1.0)的左闭右开区间，返回值是一个伪随机选择的数，在该范围内（近似）均匀分布。例子如下：

```java
public static void main(String[] args) {
    // 结果是个double类型的值，区间为[0.0,1.0）
    System.out.println("Math.random()=" + Math.random());
    int num = (int) (Math.random() * 3);
    // 注意不要写成(int)Math.random()*3，这个结果为0或1，因为先执行了强制转换
    System.out.println("num=" + num);
}
```



**2、java.util.Random**

下面是Random()的两种构造方法：

 Random()：创建一个新的随机数生成器
 Random(long seed)：使用单个 long 种子创建一个新的随机数生成器。

你在创建一个Random对象的时候可以给定任意一个合法的种子数，种子数只是随机算法的起源数字，和生成的随机数的区间没有任何关系。

如下面的Java代码：

【演示一】

在没带参数构造函数生成的Random对象的种子是当前系统时间的毫秒数。

rand.nextInt(100)中的100是随机数的上限,产生的随机数为0-100的整数，不包括100。

```java
public static void main(String[] args) {
    Random rand = new Random();
    int i = rand.nextInt(100);
    System.out.println(i);
}
```

【演示二】

对于种子相同的Random对象，多次执行后生成的随机数序列是一样的。

```java
public static void main(String[] args) {
    Random ran1 = new Random(25);
    System.out.println("使用种子为25的Random对象生成[0,100)内随机整数序列: ");
    for (int i = 0; i < 10; i++) {
        System.out.print(ran1.nextInt(100) + " ");
    }
    System.out.println();
}
```

【方法摘要】

1. protected int next(int bits)：生成下一个伪随机数。
2. boolean nextBoolean()：返回下一个伪随机数，它是取自此随机数生成器序列的均匀分布的 boolean值。
3. void nextBytes(byte[] bytes)：生成随机字节并将其置于用户提供的 byte 数组中。
4.  double nextDouble()：返回下一个伪随机数，它是取自此随机数生成器序列的、在0.0和1.0之间 均匀分布的 double值。
5. float nextFloat()：返回下一个伪随机数，它是取自此随机数生成器序列的、在0.0和1.0之间均匀分布float值。
6.  double nextGaussian()：返回下一个伪随机数，它是取自此随机数生成器序列的、呈高斯（“正态”）分布的double值，其平均值是0.0标准差是1.0。
7. int nextInt()：返回下一个伪随机数，它是此随机数生成器的序列中均匀分布的 int 值。
8. int nextInt(int n)：返回一个伪随机数，它是取自此随机数生成器序列的、在（包括和指定值（不包括）之间均匀分布的int值。
9.  long nextLong()：返回下一个伪随机数，它是取自此随机数生成器序列的均匀分布的 long 值。
10.  void setSeed(long seed)：使用单个 long 种子设置此随机数生成器的种子。

【例子】

1. 生成[0,1.0)区间的小数：double d1 = r.nextDouble();
2. 生成[0,5.0)区间的小数：double d2 = r.nextDouble() * 5;
3. 生成[1,2.5)区间的小数：double d3 = r.nextDouble() * 1.5 + 1;
4. 生成[0,10)区间的整数：int n2 = r.nextInt(10);

## 日期时间类

### 1	Date类

java.util 包提供了 Date 类来封装当前的日期和时间。

Date 类提供两个构造函数来实例化 Date 对象。

第一个构造函数使用当前日期和时间来初始化对象。

```java
Date()
```

第二个构造函数接收一个参数，该参数是从1970年1月1日起的毫秒数。

```java
Date(long millisec)
```

Date对象创建以后，可以调用下面的方法。

| 序号 | 方法和描述                                                   |
| :--- | :----------------------------------------------------------- |
| 1    | **boolean after(Date date)** 若当调用此方法的Date对象在指定日期之后返回true,否则返回false。 |
| 2    | **boolean before(Date date)** 若当调用此方法的Date对象在指定日期之前返回true,否则返回false。 |
| 3    | **Object clone( )** 返回此对象的副本。                       |
| 4    | **int compareTo(Date date)** 比较当调用此方法的Date对象和指定日期。两者相等时候返回0。调用对象在指定日期之前则返回负数。调用对象在指定日期之后则返回正数。 |
| 5    | **int compareTo(Object obj)** 若obj是Date类型则操作等同于compareTo(Date) 。否则它抛出ClassCastException。 |
| 6    | **boolean equals(Object date)** 当调用此方法的Date对象和指定日期相等时候返回true,否则返回false。 |
| 7    | **long getTime( )** 返回自 1970 年 1 月 1 日 00:00:00 GMT 以来此 Date 对象表示的毫秒数。 |
| 8    | **int hashCode( )**  返回此对象的哈希码值。                  |
| 9    | **void setTime(long time)**   用自1970年1月1日00:00:00 GMT以后time毫秒数设置时间和日期。 |
| 10   | **String toString( )** 把此 Date 对象转换为以下形式的 String： dow mon dd hh:mm:ss zzz yyyy 其中： dow 是一周中的某一天 (Sun, Mon, Tue, Wed, Thu, Fri, Sat)。 |

【演示：获取当前日期时间】

Java中获取当前日期和时间很简单，使用 Date 对象的 toString() 方法来打印当前日期和时间

```java
public static void main(String args[]) {
    // 初始化 Date 对象
    Date date = new Date();

    // 使用 toString() 函数显示日期时间
    System.out.println(date.toString());
    //Tue Mar 30 10:24:19 CST 2021
}
```

【演示：日期比较】

使用 getTime() 方法获取两个日期（自1970年1月1日经历的毫秒数值），然后比较这两个值。

```java
public static void main(String[] args) {
    // 初始化 Date 对象
    Date date = new Date();

    long time = date.getTime();
    long time2 = date.getTime();
    System.out.println(time==time2);//true
}
```

使用方法 before()，after() 和 equals()。例如，一个月的12号比18号早，则 new Date(99, 2, 12).before(new Date (99, 2, 18)) 返回true。

```java
public static void main(String[] args) {
    boolean before = new Date(99, 01, 05).before(new Date(99, 11, 16));
    System.out.println(before);
}
```

### 2、SimpleDateFormat

格式化日期

SimpleDateFormat 是一个以语言环境敏感的方式来格式化和分析日期的类。SimpleDateFormat 允许你选择任何用户自定义日期时间格式来运行。例如：

```java
public static void main(String args[]) {
    Date dNow = new Date( );
    SimpleDateFormat ft = new SimpleDateFormat ("yyyy-MM-dd hh:mm:ss");
    System.out.println("当前时间为: " + ft.format(dNow));
}
```

其中 yyyy 是完整的公元年，MM 是月份，dd 是日期，HH:mm:ss 是时、分、秒。

注意：有的格式大写，有的格式小写，例如 MM 是月份，mm 是分；HH 是 24 小时制，而 hh 是 12 小时制。

时间模式字符串用来指定时间格式。在此模式中，所有的 ASCII 字母被保留为模式字母，定义如下：

| **字母** | **描述**                 | **示例**                |
| :------- | :----------------------- | :---------------------- |
| G        | 纪元标记                 | AD                      |
| y        | 四位年份                 | 2001                    |
| M        | 月份                     | July or 07              |
| d        | 一个月的日期             | 10                      |
| h        | A.M./P.M. (1~12)格式小时 | 12                      |
| H        | 一天中的小时 (0~23)      | 22                      |
| m        | 分钟数                   | 30                      |
| s        | 秒数                     | 55                      |
| S        | 毫秒数                   | 234                     |
| E        | 星期几                   | Tuesday                 |
| D        | 一年中的日子             | 360                     |
| F        | 一个月中第几周的周几     | 2 (second Wed. in July) |
| w        | 一年中第几周             | 40                      |
| W        | 一个月中第几周           | 1                       |
| a        | A.M./P.M. 标记           | PM                      |
| k        | 一天中的小时(1~24)       | 24                      |
| K        | A.M./P.M. (0~11)格式小时 | 10                      |
| z        | 时区                     | Eastern Standard Time   |
| '        | 文字定界符               | Delimiter               |
| "        | 单引号                   | `                       |

【演示：使用printf格式化日期】

Java 格式化输出 printf 例子：https://www.runoob.com/w3cnote/java-printf-formate-demo.html

printf 方法可以很轻松地格式化时间和日期。使用两个字母格式，它以 %t 开头并且以下面表格中的一个字母结尾。

```java
public static void main(String[] args) {
    // 初始化 Date 对象
    Date date = new Date();
    //c的使用
    System.out.printf("全部日期和时间信息：%tc%n",date);
    //f的使用
    System.out.printf("年-月-日格式：%tF%n",date);
    //d的使用
    System.out.printf("月/日/年格式：%tD%n",date);
    //r的使用
    System.out.printf("HH:MM:SS PM格式（12时制）：%tr%n",date);
    //t的使用
    System.out.printf("HH:MM:SS格式（24时制）：%tT%n",date);
    //R的使用
    System.out.printf("HH:MM格式（24时制）：%tR",date);
}
```

结果：

>全部日期和时间信息：周二 3月 30 10:37:02 CST 2021
>年-月-日格式：2021-03-30
>月/日/年格式：03/30/21
>HH:MM:SS PM格式（12时制）：10:37:02 上午
>HH:MM:SS格式（24时制）：10:37:02
>HH:MM格式（24时制）：10:37

【时间休眠：休眠(sleep)】

sleep()使当前线程进入停滞状态（阻塞当前线程），让出CPU的使用、目的是不让当前线程独自霸占该进程所获的CPU资源，以留一定时间给其他线程执行的机会。

你可以让程序休眠一毫秒的时间或者到您的计算机的寿命长的任意段时间。例如，下面的程序会休眠3秒：

```java
public static void main(String args[]) {
    try {
        System.out.println(new Date( ) + "\n");
        Thread.sleep(1000*3); // 休眠3秒
        System.out.println(new Date( ) + "\n");
    } catch (Exception e) {
        System.out.println("Got an exception!");
    }
}
```

### 3、Calendar类

我们现在已经能够格式化并创建一个日期对象了，但是我们如何才能设置和获取日期数据的特定部分呢，比如说小时，日，或者分钟? 我们又如何在日期的这些部分加上或者减去值呢? 答案是使用Calendar类。Date中有很多方法都已经废弃了！

Calendar类的功能要比Date类强大很多，而且在实现方式上也比Date类要复杂一些。

Calendar类是一个抽象类，在实际使用时实现特定的子类的对象，创建对象的过程对程序员来说是透明的，只需要使用getInstance方法创建即可。

**创建一个代表系统当前日期的Calendar对象**

```java
public static void main(String args[]) {
    Calendar c = Calendar.getInstance();//默认是当前日期
    System.out.println(c);
}
```

输出：
> java.util.GregorianCalendar[time=1617072097924,areFieldsSet=true,areAllFieldsSet=true,lenient=true,zone=sun.util.calendar.ZoneInfo[id="Asia/Shanghai",offset=28800000,dstSavings=0,useDaylight=false,transitions=31,lastRule=null],firstDayOfWeek=1,minimalDaysInFirstWeek=1,ERA=1,YEAR=2021,MONTH=2,WEEK_OF_YEAR=14,WEEK_OF_MONTH=5,DAY_OF_MONTH=30,DAY_OF_YEAR=89,DAY_OF_WEEK=3,DAY_OF_WEEK_IN_MONTH=5,AM_PM=0,HOUR=10,HOUR_OF_DAY=10,MINUTE=41,SECOND=37,MILLISECOND=924,ZONE_OFFSET=28800000,DST_OFFSET=0]

**创建一个指定日期的Calendar对象**

使用Calendar类代表特定的时间，需要首先创建一个Calendar的对象，然后再设定该对象中的年月日参数来完成。

```java
//创建一个代表2019年4月27日的Calendar对象
Calendar c1 = Calendar.getInstance();
c1.set(2019, 4 - 1, 27);
```

**Calendar类对象字段类型**

Calendar类中用以下这些常量表示不同的意义，jdk内的很多类其实都是采用的这种思想

| 常量                  | 描述                           |
| :-------------------- | :----------------------------- |
| Calendar.YEAR         | 年份                           |
| Calendar.MONTH        | 月份                           |
| Calendar.DATE         | 日期                           |
| Calendar.DAY_OF_MONTH | 日期，和上面的字段意义完全相同 |
| Calendar.HOUR         | 12小时制的小时                 |
| Calendar.HOUR_OF_DAY  | 24小时制的小时                 |
| Calendar.MINUTE       | 分钟                           |
| Calendar.SECOND       | 秒                             |
| Calendar.DAY_OF_WEEK  | 星期几                         |

```java
// 获得年份
int year = c1.get(Calendar.YEAR);
// 获得月份
int month = c1.get(Calendar.MONTH) + 1;
// 获得日期
int date = c1.get(Calendar.DATE);
// 获得小时
int hour = c1.get(Calendar.HOUR_OF_DAY);
// 获得分钟
int minute = c1.get(Calendar.MINUTE);
// 获得秒
int second = c1.get(Calendar.SECOND);
// 获得星期几（注意（这个与Date类是不同的）：1代表星期日、2代表星期1、3代表星期二，以此类推）
int day = c1.get(Calendar.DAY_OF_WEEK);
```

设置完整日期

```java
Calendar c1 = Calendar.getInstance();
c1.set(2009, 6 - 1, 12);//把Calendar对象c1的年月日分别设这为：2009、6、12
```

设置某个字段

```java
c1.set(Calendar.DATE,10);
c1.set(Calendar.YEAR,2008);
//其他字段属性set的意义以此类推
```

add设置

```java
//把c1对象的日期加上10，也就是c1也就表示为10天后的日期，其它所有的数值会被重新计算
c1.add(Calendar.DATE, 10);
//把c1对象的日期减去10，也就是c1也就表示为10天前的日期，其它所有的数值会被重新计算
c1.add(Calendar.DATE, -10);
```

【演示：GregorianCalendar】

```java
public static void main(String[] args) {
    String months[] = {
            "Jan", "Feb", "Mar", "Apr",
            "May", "Jun", "Jul", "Aug",
            "Sep", "Oct", "Nov", "Dec"};

    int year;
    // 初始化 Gregorian 日历
    // 使用当前时间和日期
    // 默认为本地时间和时区
    GregorianCalendar gcalendar = new GregorianCalendar();
    // 显示当前时间和日期的信息
    System.out.print("Date: ");
    System.out.print(months[gcalendar.get(Calendar.MONTH)]);
    System.out.print(" " + gcalendar.get(Calendar.DATE) + " ");
    System.out.println(year = gcalendar.get(Calendar.YEAR));
    System.out.print("Time: ");
    System.out.print(gcalendar.get(Calendar.HOUR) + ":");
    System.out.print(gcalendar.get(Calendar.MINUTE) + ":");
    System.out.println(gcalendar.get(Calendar.SECOND));

    // 测试当前年份是否为闰年
    if (gcalendar.isLeapYear(year)) {
        System.out.println("当前年份是闰年");
    } else {
        System.out.println("当前年份不是闰年");
    }

}
```

输出：

> Date: Mar 30 2021
> Time: 10:49:35
> 当前年份不是闰年

**注意：Calender的月份是从0开始的，但日期和年份是从1开始的**

【演示】

```java
public static void main(String[] args) {
    Calendar c1 = Calendar.getInstance();
    c1.set(2017, 1, 1);
    System.out.println(c1.get(Calendar.YEAR)
            + "-" + c1.get(Calendar.MONTH)
            + "-" + c1.get(Calendar.DATE));
    c1.set(2017, 1, 0);
    System.out.println(c1.get(Calendar.YEAR)
            + "-" + c1.get(Calendar.MONTH)
            + "-" + c1.get(Calendar.DATE));
}
/*
输出
2017-1-1
2017-0-31
    /*
```

可见，将日期设为0以后，月份变成了上个月，但月份可以为0，把月份改为2试试：

```java
public static void main(String[] args) {
    Calendar c1 = Calendar.getInstance();
    c1.set(2017, 2, 1);
    System.out.println(c1.get(Calendar.YEAR)
            + "-" + c1.get(Calendar.MONTH)
            + "-" + c1.get(Calendar.DATE));
    c1.set(2017, 2, 0);
    System.out.println(c1.get(Calendar.YEAR)
            + "-" + c1.get(Calendar.MONTH)
            + "-" + c1.get(Calendar.DATE));
}
/*
输出
2017-2-1
2017-1-28
*/
```

可以看到上个月的最后一天是28号，所以Calendar.MONTH为1的时候是2月 。

## String类

### 1、String概述

在API中是这样描述：

 String 类代表字符串。Java 程序中的所有字符串字面值（如 "abc" ）都作为此类的实例实现。 字符串是常量；它们的值在创建之后不能更改。字符串缓冲区支持可变的字符串。因为 String 对象是不可变的， 所以可以共享。

【演示：查看String源码】

```java
public final class String
implements java.io.Serializable, Comparable<String>, CharSequence {
    
}
```

【String的成员变量】

```java
//String的属性值
private final char value[];

//数组被使用的开始位置
private final int offset;

//String中元素的个数
private final int count;

//String类型的hash值
private int hash; // Default to 0

private static final long serialVersionUID = -6849794470754667710L;
private static final ObjectStreamField[] serialPersistentFields =
new ObjectStreamField[0];
```

从源码看出String底层使用一个字符数组来维护的。

成员变量可以知道String类的值是final类型的，不能被改变的，所以只要一个值改变就会生成一个新的 String类型对象，存储String数据也不一定从数组的第0个元素开始的，而是从offset所指的元素开始。

【String的构造方法】

```java
String()
//初始化一个新创建的 String 对象，使其表示一个空字符序列。
    
String(byte[] bytes)
//通过使用平台的默认字符集解码指定的 byte 数组，构造一个新的 String。
    
String(byte[] bytes, Charset charset)
//通过使用指定的 charset 解码指定的 byte 数组，构造一个新的 String。
    
String(byte[] bytes, int offset, int length)
//通过使用平台的默认字符集解码指定的 byte 子数组，构造一个新的 String。
    
String(byte[] bytes, int offset, int length, Charset charset)
//通过使用指定的 charset 解码指定的 byte 子数组，构造一个新的 String。
    
String(byte[] bytes, int offset, int length, String charsetName)
//通过使用指定的字符集解码指定的 byte 子数组，构造一个新的 String。
    
String(byte[] bytes, String charsetName)
//通过使用指定的 charset 解码指定的 byte 数组，构造一个新的 String。
    
String(char[] value)
//分配一个新的 String，使其表示字符数组参数中当前包含的字符序列。
    
String(char[] value, int offset, int count)
//分配一个新的 String，它包含取自字符数组参数一个子数组的字符。
    
String(int[] codePoints, int offset, int count)
//分配一个新的 String，它包含 Unicode 代码点数组参数一个子数组的字符。
    
String(String original)
//初始化一个新创建的 String 对象，使其表示一个与参数相同的字符序列；换句话说，新创建的字符串是该参数字符串的副本。
    
String(StringBuffer buffer)
//分配一个新的字符串，它包含字符串缓冲区参数中当前包含的字符序列。
    
String(StringBuilder builder)
//分配一个新的字符串，它包含字符串生成器参数中当前包含的字符序列。
```

### 2、创建字符串对象方式

直接赋值方式创建对象是在方法区的常量池

```java
String str="hello";//直接赋值的方式
```

通过构造方法创建字符串对象是在堆内存

```java
String str=new String("hello");//实例化的方式
```

【两种实例化方式的比较】

 编写代码比较

```java
public static void main(String[] args) {
    String str1 = "Lance";
    String str2 = new String("Lance");
    String str3 = str2; //引用传递，str3直接指向st2的堆内存地址
    String str4 = "Lance";
    /**
     * ==:
     * 基本数据类型：比较的是基本数据类型的值是否相同
     * 引用数据类型：比较的是引用数据类型的地址值是否相同
     * 所以在这里的话：String类对象==比较，比较的是地址，而不是内容
     */
    System.out.println(str1 == str2);//false
    System.out.println(str1 == str3);//false
    System.out.println(str3 == str2);//true
    System.out.println(str1 == str4);//true
}
```

内存图分析

![image-20210330110521687](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210330110521687.png)

可能这里还是不够明显，构造方法实例化方式的内存图：String str = new String("Hello");

![image-20210330110555759](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210330110555759.png)

当我们再一次的new一个String对象时：

![image-20210330110629270](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210330110629270.png)

【字符串常量池】

在字符串中，如果采用直接赋值的方式（String str="Lance"）进行对象的实例化，则会将匿名对象 “Lance”放入对象池，每当下一次对不同的对象进行直接赋值的时候会直接利用池中原有的匿名对象，我们可以用对象手工入池；

```java
public static void main(String args[]){
    String str = new String("Lance").intern();//对匿名对象进行手工入池操作
    String str1 = "Lance";
    System.out.println(str==str1);//true
}
```

【两种实例化方式的区别】

1. 直接赋值（String str = "hello"）

   只开辟一块堆内存空间，并且会自动入池，不会产生垃圾。

2. 构造方法（String str= new String("hello");）

   会开辟两块堆内存空间，其中一块堆内存会变成垃圾被系统回收，而且不能够自动入池，需要通过public String intern();方法进行手工入池。

3.  在开发的过程中不会采用构造方法进行字符串的实例化。

【避免空指向】

首先了解： == 和public boolean equals()比较字符串的区别

==在对字符串比较的时候，对比的是内存地址，而equals比较的是字符串内容，在开发的过程中， equals()通过接受参数，可以避免空指向。

```java
String str = null;
if(str.equals("hello")){//此时会出现空指向异常

}

if("hello".equals(str)){//此时equals会处理null值，可以避免空指向异常

}
```

String类对象一旦声明则不可以改变；而改变的只是地址，原来的字符串还是存在的，并且产生垃圾

![image-20210330111048863](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210330111048863.png)

### 3、String常用的方法

![image-20210330111326341](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210330111326341.png)

#### String的判断

> boolean equals(Object obj)：比较字符串的内容是否相同
> boolean equalsIgnoreCase(String str)： 比较字符串的内容是否相同,忽略大小写
> boolean startsWith(String str)： 判断字符串对象是否以指定的str开头
> boolean endsWith(String str)： 判断字符串对象是否以指定的str结尾

演示：

```java
public static void main(String[] args) {
    // 创建字符串对象
    String s1 = "hello";
    String s2 = "hello";
    String s3 = "Hello";
    
    // boolean equals(Object obj):比较字符串的内容是否相同
    System.out.println(s1.equals(s2)); //true
    System.out.println(s1.equals(s3)); //false
    System.out.println("-----------");
    
    // boolean equalsIgnoreCase(String str):比较字符串的内容是否相同,忽略大小写
    System.out.println(s1.equalsIgnoreCase(s2)); //true
    System.out.println(s1.equalsIgnoreCase(s3)); //true
    System.out.println("-----------");
    
    // boolean startsWith(String str):判断字符串对象是否以指定的str开头
    System.out.println(s1.startsWith("he")); //true
    System.out.println(s1.startsWith("ll")); //false
}
```

#### String的截取

> int length():获取字符串的长度，其实也就是字符个数
> char charAt(int index):获取指定索引处的字符
> int indexOf(String str):获取str在字符串对象中第一次出现的索引
> String substring(int start):从start开始截取字符串
> String substring(int start,int end):从start开始，到end结束截取字符串。包括start，不包括end

演示

```java
public static void main(String args[]) {
    // 创建字符串对象
    String s = "helloworld";
    // int length():获取字符串的长度，其实也就是字符个数
    System.out.println(s.length()); //10
    System.out.println("--------");
    // char charAt(int index):获取指定索引处的字符
    System.out.println(s.charAt(0)); //h
    System.out.println(s.charAt(1)); //e
    System.out.println("--------");
    // int indexOf(String str):获取str在字符串对象中第一次出现的索引
    System.out.println(s.indexOf("l")); //2
    System.out.println(s.indexOf("owo")); //4
    System.out.println(s.indexOf("ak")); //-1
    System.out.println("--------");
    // String substring(int start):从start开始截取字符串
    System.out.println(s.substring(0)); //helloworld
    System.out.println(s.substring(5)); //world
    System.out.println("--------");
    // String substring(int start,int end):从start开始，到end结束截取字符串
    System.out.println(s.substring(0, s.length())); //helloworld
    System.out.println(s.substring(3, 8)); //lowor
}
```

#### String的转换

> char[] toCharArray()：把字符串转换为字符数组
> String toLowerCase()：把字符串转换为小写字符串
> String toUpperCase()：把字符串转换为大写字符串

演示

```java
public static void main(String args[]) {
	// 创建字符串对象
    String s = "abcde";
    
    // char[] toCharArray():把字符串转换为字符数组
    char[] chs = s.toCharArray();
    for (int x = 0; x < chs.length; x++) {
        System.out.println(chs[x]);
    }
    
    System.out.println("-----------");
    
    // String toLowerCase():把字符串转换为小写字符串
    System.out.println("HelloWorld".toLowerCase());
    // String toUpperCase():把字符串转换为大写字符串
    System.out.println("HelloWorld".toUpperCase());
}
```

#### 其他方法

> 去除字符串两端空格：String trim() 
>
> 按照指定符号分割字符串：String[] split(String str)

```java
public static void main(String args[]) {
    // 创建字符串对象
    String s1 = "helloworld";
    String s2 = " helloworld ";
    String s3 = " hello world ";
    System.out.println("---" + s1 + "---");
    System.out.println("---" + s1.trim() + "---");
    System.out.println("---" + s2 + "---");
    System.out.println("---" + s2.trim() + "---");
    System.out.println("---" + s3 + "---");
    System.out.println("---" + s3.trim() + "---");
    System.out.println("-------------------");
    
    // String[] split(String str)
    // 创建字符串对象
    String s4 = "aa,bb,cc";
    String[] strArray = s4.split(",");
    for (int x = 0; x < strArray.length; x++) {
        System.out.println(strArray[x]);
    }
}
```

### 4、String的不可变性

当我们去阅读源代码的时候，会发现有这样的一句话：

> Strings are constant; their values cannot be changed after they are created.

意思就是说：String是个常量，从一出生就注定不可变

我想大家应该就知道为什么String不可变了，String类被final修饰，官方注释说明创建后不能被改变，但 是为什么String要使用final修饰呢？

了解一个经典的面试题

```java
public static void main(String[] args) {
    String a = "abc";
    String b = "abc";
    String c = new String("abc");
    System.out.println(a==b); //true
    System.out.println(a.equals(b)); //true
    System.out.println(a==c); //false
    System.out.println(a.equals(c)); //true
}
```

![image-20210330112025681](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210330112025681.png)

因为String太过常用，JAVA类库的设计者在实现时做了个小小的变化，即采用了享元模式，每当生成一个新内容的字符串时，他们都被添加到一个共享池中，当第二次再次生成同样内容的字符串实例时，就共享此对象，而不是创建一个新对象，但是这样的做法仅仅适合于通过=符号进行的初始化。

需要说明一点的是，在object中，equals()是用来比较内存地址的，但是String重写了equals()方 法，用来比较内容的，即使是不同地址，只要内容一致，也会返回true，这也就是为什么a.equals(c)返回true的原因了。

**String不可变的好处**

- 可以实现多个变量引用堆内存中的同一个字符串实例，避免创建的开销。
- 我们的程序中大量使用了String字符串，有可能是出于安全性考虑。
- 大家都知道HashMap中key为String类型，如果可变将变的多么可怕。
- 当我们在传参的时候，使用不可变类不需要去考虑谁可能会修改其内部的值，如果使用可变类的话，可能需要每次记得重新拷贝出里面的值，性能会有一定的损失。

### 5、字符串常量池

字符串常量池概述：

1、常量池表（Constant_Pool table）

Class文件中存储所有常量（包括字符串）的table。这是Class文件中的内容，还不是运行时的内容，不要理解它是个池子，其实就是Class文件中的字节码指令。

2、运行时常量池（Runtime Constant Pool）

JVM内存中方法区的一部分，这是运行时的内容。这部分内容（绝大部分）是随着JVM运行时候，从常量池转化而来，每个Class对应一个运行时常量池。上一句中说绝大部分是因为：除了 Class中常量池内 容，还可能包括动态生成并加入这里的内容。

3、字符串常量池（String Pool）

这部分也在方法区中，但与Runtime Constant Pool不是一个概念，String Pool是JVM实例全局共享的，全局只有一个。JVM规范要求进入这里的String实例叫“被驻留的interned string”，各个JVM可以有不同的实现，HotSpot是设置了一个哈希表StringTable来引用堆中的字符串实例，被引用就是被驻留。

【亨元模式】

其实字符串常量池这个问题涉及到一个设计模式，叫“享元模式”，顾名思义 - - - > 共享元素模式 也就是说：一个系统中如果有多处用到了相同的一个元素，那么我们应该只存储一份此元素，而让所有地方都引用这一个元素

Java中String部分就是根据享元模式设计的，而那个存储元素的地方就叫做“字符串常量池 - String Pool”

【详细分析】

```java
int x = 10;
String y = "hello";
```

**①** 首先， `10 `和 `"hello" `会在经过javac（或者其他编译器）编译过后变为Class文件中 `constant_pool table` 的内容

**②** 当我们的程序运行时，也就是说JVM运行时，每个Class constant_pool table 中的内容会被加载到JVM内存中的方法区中各自Class的 Runtime Constant Pool。

**③** 一个没有被String Pool包含的Runtime Constant Pool中的字符串（这里是"hello"）会被加入到 String Pool中（HosSpot使用hashtable引用方式），步骤如下：

1. 在Java Heap（堆）中根据"hello"字面量create一个字符串对象

2. 将字面量"hello"与字符串对象的引用在hashtable中关联起来键 - 值

   形式是："hello" = 对象的引用地址。

另外来说，当一个新的字符串出现在Runtime Constant Pool中时怎么判断需不需要在Java Heap中创建 新对象呢？

策略是这样：会先去根据equals来比较Runtime Constant Pool中的这个字符串是否和String Pool中某一个是相等的（也就是找是否已经存在），如果有那么就不创建，直接使用其引用；反之，就如同上面的第三步。

如此，就实现了享元模式，提高的内存利用效率。

举例：

> 使用String s = new String("hello");会创建几个对象 
> 答：会创建2个对象
>
> 首先，出现了字面量"hello"，那么去String Pool中查找是否有相同字符串存在，因为程序就这一行代码所以肯定没有，那么就在Java Heap中用字面量"hello"首先创建1个String对象。
>
> 接着，new String("hello")，关键字new又在Java Heap中创建了1个对象，然后调用接收String 参数的构造器进行了初始化。最终s的引用是这个String对象.

## StringBuilder和StringBuffer

### 1、概述

【演示：查看源码及API文档】

```java
public final class StringBuilder
    extends AbstractStringBuilder
    implements java.io.Serializable, CharSequence{
    
}
```

StringBuilder 是一个可变的字符序列。它继承于AbstractStringBuilder，实现了CharSequence接口。 StringBuffer 也是继承于AbstractStringBuilder的子类；
但是，StringBuilder和StringBuffer不同，前者是非线程安全的，后者是线程安全的。

StringBuilder 和 CharSequence之间的关系图如下：

![image-20210330113151662](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-常用类.assets/image-20210330113151662.png)

【源码概览】

```java
package java.lang;
public final class StringBuilder
    extends AbstractStringBuilder
    implements java.io.Serializable, CharSequence {
    
    static final long serialVersionUID = 4383685877147921099L;
    // 构造函数。默认的字符数组大小是16。
    public StringBuilder() {
        super(16);
    }
    
    // 构造函数。指定StringBuilder的字符数组大小是capacity。
        public StringBuilder(int capacity) {
        super(capacity);
    }
    
    // 构造函数。指定字符数组大小=str长度+15，且将str的值赋值到当前字符数组中。
    public StringBuilder(String str) {
        super(str.length() + 16);
        append(str);
    }
    
    // 构造函数。指定字符数组大小=seq长度+15，且将seq的值赋值到当前字符数组中。
    public StringBuilder(CharSequence seq) {
        this(seq.length() + 16);
        append(seq);
    }
    
    // 追加“对象obj对应的字符串”。String.valueOf(obj)实际上是调用obj.toString()
    public StringBuilder append(Object obj) {
        return append(String.valueOf(obj));
    }
    
    // 追加“str”。
    public StringBuilder append(String str) {
        super.append(str);
        return this;
    }
    
      // 追加“sb的内容”。
    private StringBuilder append(StringBuilder sb) {
        if (sb == null)
        	return append("null");
        int len = sb.length();
        int newcount = count + len;
        if (newcount > value.length)
        	expandCapacity(newcount);
        sb.getChars(0, len, value, count);
        count = newcount;
        return this;
    }
    
    // 追加“sb的内容”。
    public StringBuilder append(StringBuffer sb) {
        super.append(sb);
        return this;
    }
    
    // 追加“s的内容”。
    public StringBuilder append(CharSequence s) {
        if (s == null)
            s = "null";
        if (s instanceof String)
            return this.append((String)s);
        if (s instanceof StringBuffer)
            return this.append((StringBuffer)s);
        if (s instanceof StringBuilder)
            return this.append((StringBuilder)s);
        return this.append(s, 0, s.length());
    }

    // 追加“s从start(包括)到end(不包括)的内容”。
    public StringBuilder append(CharSequence s, int start, int end) {
        super.append(s, start, end);
        return this;
    }
    
    // 追加“str字符数组对应的字符串”
    public StringBuilder append(char[] str) {
        super.append(str);
        return this;
    }
    
    // 追加“str从offset开始的内容，内容长度是len”
    public StringBuilder append(char[] str, int offset, int len) {
        super.append(str, offset, len);
        return this;
    }
    
    // 追加“b对应的字符串”
    public StringBuilder append(boolean b) {
        super.append(b);
        return this;
    }
    
    // 追加“c”
    public StringBuilder append(char c) {
        super.append(c);
        return this;
    }
    
    // 追加“i”
    public StringBuilder append(int i) {
        super.append(i);
        return this;
    }
    
    // 追加“lng”
    public StringBuilder append(long lng) {
        super.append(lng);
        return this;
    }
    
    // 追加“f”
    public StringBuilder append(float f) {
        super.append(f);
        return this;
    }
    
    // 追加“d”
    public StringBuilder append(double d) {
        super.append(d);
        return this;
    }
    
    // 追加“codePoint”
    public StringBuilder appendCodePoint(int codePoint) {
        super.appendCodePoint(codePoint);
        return this;
    }
    
    // 删除“从start(包括)到end的内容”
    public StringBuilder delete(int start, int end) {
        super.delete(start, end);
        return this;
    }
    
    // 删除“位置index的内容”
    public StringBuilder deleteCharAt(int index) {
        super.deleteCharAt(index);
        return this;
    }
    
    // “用str替换StringBuilder中从start(包括)到end(不包括)的内容”
    public StringBuilder replace(int start, int end, String str) {
        super.replace(start, end, str);
        return this;
    }
    
    // “在StringBuilder的位置index处插入‘str中从offset开始的内容’，插入内容长度是len”
    public StringBuilder insert(int index, char[] str, int offset,
    int len)
    {
        super.insert(index, str, offset, len);
        return this;
    }
    
    // “在StringBuilder的位置offset处插入obj对应的字符串”
    public StringBuilder insert(int offset, Object obj) {
    	return insert(offset, String.valueOf(obj));
    }
    
    // “在StringBuilder的位置offset处插入str”
    public StringBuilder insert(int offset, String str) {
        super.insert(offset, str);
        return this;
    }
    
    // “在StringBuilder的位置offset处插入str”
    public StringBuilder insert(int offset, char[] str) {
        super.insert(offset, str);
        return this;
    }
    
    // “在StringBuilder的位置dstOffset处插入s”
    public StringBuilder insert(int dstOffset, CharSequence s) {
        if (s == null)
       	 	s = "null";
        if (s instanceof String)
        	return this.insert(dstOffset, (String)s);
        return this.insert(dstOffset, s, 0, s.length());
    }
    
    // “在StringBuilder的位置dstOffset处插入's中从start到end的内容'”
    public StringBuilder insert(int dstOffset, CharSequence s,
    int start, int end)
    {
        super.insert(dstOffset, s, start, end);
        return this;
    }
    
    // “在StringBuilder的位置Offset处插入b”
    public StringBuilder insert(int offset, boolean b) {
        super.insert(offset, b);
        return this;
    }
    
    // “在StringBuilder的位置Offset处插入c”
    public StringBuilder insert(int offset, char c) {
        super.insert(offset, c);
        return this;
    }
    
    // “在StringBuilder的位置Offset处插入i”
    public StringBuilder insert(int offset, int i) {
    	return insert(offset, String.valueOf(i));
    }

    // “在StringBuilder的位置Offset处插入l”
    public StringBuilder insert(int offset, long l) {
    	return insert(offset, String.valueOf(l));
    }
    
    // “在StringBuilder的位置Offset处插入f”
    public StringBuilder insert(int offset, float f) {
    	return insert(offset, String.valueOf(f));
    }
    
    // “在StringBuilder的位置Offset处插入d”
    public StringBuilder insert(int offset, double d) {
   		 return insert(offset, String.valueOf(d));
    }	
    
    // 返回“str”在StringBuilder的位置
    public int indexOf(String str) {
   		 return indexOf(str, 0);
    }
    
    // 从fromIndex开始查找，返回“str”在StringBuilder的位置
    public int indexOf(String str, int fromIndex) {
        return String.indexOf(value, 0, count,
        	str.toCharArray(), 0, str.length(),fromIndex);
    }
    
    // 从后向前查找，返回“str”在StringBuilder的位置
    public int lastIndexOf(String str) {
   		 return lastIndexOf(str, count);
    }
    
    // 从fromIndex开始，从后向前查找，返回“str”在StringBuilder的位置
    public int lastIndexOf(String str, int fromIndex) {
    return String.lastIndexOf(value, 0, count,
    	str.toCharArray(), 0, str.length(),fromIndex);
    }
    
    // 反转StringBuilder
    public StringBuilder reverse() {
        super.reverse();
        return this;
    }
    
    public String toString() {
    // Create a copy, don't share the array
    	return new String(value, 0, count);
    }
    
    // 序列化对应的写入函数
    private void writeObject(java.io.ObjectOutputStream s)
        throws java.io.IOException {
            s.defaultWriteObject();
            s.writeInt(count);
            s.writeObject(value);
    }
    
        // 序列化对应的读取函数
    private void readObject(java.io.ObjectInputStream s)
        throws java.io.IOException, ClassNotFoundException {
            s.defaultReadObject();
            count = s.readInt();
            value = (char[]) s.readObject();
    }
```

### 2、常用方法

#### insert

```java
public static void main(String[] args) {
    StringBuilder sbuilder = new StringBuilder();
    // 在位置0处插入字符数组
    sbuilder.insert(0, new char[]{'a', 'b', 'c', 'd', 'e'});
    // 在位置0处插入字符数组。0表示字符数组起始位置，3表示长度
    sbuilder.insert(0, new char[]{'A', 'B', 'C', 'D', 'E'}, 0, 3);
    // 在位置0处插入float
    sbuilder.insert(0, 1.414f);
    // 在位置0处插入double
    sbuilder.insert(0, 3.14159d);
    // 在位置0处插入boolean
    sbuilder.insert(0, true);
    // 在位置0处插入char
    sbuilder.insert(0, '\n');
    // 在位置0处插入int
    sbuilder.insert(0, 100);
    // 在位置0处插入long
    sbuilder.insert(0, 12345L);
    // 在位置0处插入StringBuilder对象
    sbuilder.insert(0, new StringBuilder("StringBuilder"));
    // 在位置0处插入StringBuilder对象。6表示被在位置0处插入对象的起始位置(包括)，13是结束位置(不包括)
    sbuilder.insert(0, new StringBuilder("STRINGBUILDER"), 6, 13);
    // 在位置0处插入StringBuffer对象。
    sbuilder.insert(0, new StringBuffer("StringBuffer"));
    // 在位置0处插入StringBuffer对象。6表示被在位置0处插入对象的起始位置(包括)，12是结束位置(不包括)
    sbuilder.insert(0, new StringBuffer("STRINGBUFFER"), 6, 12);
    // 在位置0处插入String对象。
    sbuilder.insert(0, "String");
    // 在位置0处插入String对象。1表示被在位置0处插入对象的起始位置(包括)，6是结束位置(不包括)
    sbuilder.insert(0, "0123456789", 1, 6);
    sbuilder.insert(0, '\n');
    
    // 在位置0处插入Object对象。此处以HashMap为例
    HashMap map = new HashMap();
    map.put("1", "one");
    map.put("2", "two");
    map.put("3", "three");
    
    sbuilder.insert(0, map);
    
    System.out.printf("%s\n\n", sbuilder);
}
```

#### append

```java
public static void main(String[] args) {
    StringBuilder sbuilder = new StringBuilder();
    // 追加字符数组
    sbuilder.append(new char[]{'a', 'b', 'c', 'd', 'e'});
    // 追加字符数组。0表示字符数组起始位置，3表示长度
    sbuilder.append(new char[]{'A', 'B', 'C', 'D', 'E'}, 0, 3);
    // 追加float
    sbuilder.append(1.414f);
    // 追加double
    sbuilder.append(3.14159d);
    // 追加boolean
    sbuilder.append(true);
    // 追加char
    sbuilder.append('\n');
    // 追加int
    sbuilder.append(100);
    // 追加long
    sbuilder.append(12345L);
    // 追加StringBuilder对象
    sbuilder.append(new StringBuilder("StringBuilder"));
    // 追加StringBuilder对象。6表示被追加对象的起始位置(包括)，13是结束位置(不包括)
    sbuilder.append(new StringBuilder("STRINGBUILDER"), 6, 13);
    // 追加StringBuffer对象。
    sbuilder.append(new StringBuffer("StringBuffer"));
    // 追加StringBuffer对象。6表示被追加对象的起始位置(包括)，12是结束位置(不包括)
    sbuilder.append(new StringBuffer("STRINGBUFFER"), 6, 12);
    // 追加String对象。
    sbuilder.append("String");
    // 追加String对象。1表示被追加对象的起始位置(包括)，6是结束位置(不包括)
    sbuilder.append("0123456789", 1, 6);

    sbuilder.append('\n');

    // 追加Object对象。此处以HashMap为例
    HashMap map = new HashMap();
    map.put("1", "one");
    map.put("2", "two");
    map.put("3", "three");
    sbuilder.append(map);
    sbuilder.append('\n');

    // 追加unicode编码
    sbuilder.appendCodePoint(0x5b57); // 0x5b57是“字”的unicode编码
    sbuilder.appendCodePoint(0x7b26); // 0x7b26是“符”的unicode编码
    sbuilder.appendCodePoint(0x7f16); // 0x7f16是“编”的unicode编码
    sbuilder.appendCodePoint(0x7801); // 0x7801是“码”的unicode编码

    System.out.printf("%s\n\n", sbuilder);
}
```

#### replace

```java
public static void main(String[] args) {
    StringBuilder sbuilder;
    
    sbuilder = new StringBuilder("0123456789");
    sbuilder.replace(0, 3, "ABCDE");
    System.out.printf("sbuilder=%s\n", sbuilder);

    sbuilder = new StringBuilder("0123456789");
    sbuilder.reverse();
    System.out.printf("sbuilder=%s\n", sbuilder);

    sbuilder = new StringBuilder("0123456789");
    sbuilder.setCharAt(0, 'M');
    System.out.printf("sbuilder=%s\n", sbuilder);
    System.out.println();
    /*
    sbuilder=ABCDE3456789
    sbuilder=9876543210
    sbuilder=M123456789
*/
}

```

#### delete

```java
public static void main(String[] args) {
    StringBuilder sbuilder = new StringBuilder("0123456789");

    // 删除位置0的字符，剩余字符是“123456789”。
    sbuilder.deleteCharAt(0);
    // 删除位置3(包括)到位置6(不包括)之间的字符，剩余字符是“123789”。
    sbuilder.delete(3, 6);

    // 获取sb中从位置1开始的字符串
    String str1 = sbuilder.substring(1);
    // 获取sb中从位置3(包括)到位置5(不包括)之间的字符串
    String str2 = sbuilder.substring(3, 5);
    // 获取sb中从位置3(包括)到位置5(不包括)之间的字符串，获取的对象是CharSequence对象，此处转型为String
    String str3 = (String) sbuilder.subSequence(3, 5);
    
    System.out.printf("sbuilder=%s\nstr1=%s\nstr2=%s\nstr3=%s\n",
            sbuilder, str1, str2, str3);

}
```

#### index

```java
public static void main(String[] args) {
    StringBuilder sbuilder = new StringBuilder("abcAbcABCabCaBcAbCaBCabc");
    
    System.out.printf("sbuilder=%s\n", sbuilder);
    
    // 1. 从前往后，找出"bc"第一次出现的位置
    System.out.printf("%-30s = %d\n", "sbuilder.indexOf(\"bc\")", sbuilder.indexOf("bc"));
    
    // 2. 从位置5开始，从前往后，找出"bc"第一次出现的位置
    System.out.printf("%-30s = %d\n", "sbuilder.indexOf(\"bc\", 5)", sbuilder.indexOf("bc", 5));
    
    // 3. 从后往前，找出"bc"第一次出现的位置
    System.out.printf("%-30s = %d\n", "sbuilder.lastIndexOf(\"bc\")", sbuilder.lastIndexOf("bc"));
    
    // 4. 从位置4开始，从后往前，找出"bc"第一次出现的位置
    System.out.printf("%-30s = %d\n", "sbuilder.lastIndexOf(\"bc\", 4)", sbuilder.lastIndexOf("bc", 4));
}
```

#### 其他API

```java
public static void main(String[] args) {
    StringBuilder sbuilder = new StringBuilder("0123456789");

    int cap = sbuilder.capacity();
    System.out.printf("cap=%d\n", cap);

    /*
    capacity()返回的是字符串缓冲区的容量
    StringBuffer( ); 分配16个字符的缓冲区
    StringBuffer( int len ); 分配len个字符的缓冲区
    StringBuffer( String s ); 除了按照s的大小分配空间外,再分配16个 字符的缓冲区
    你的StringBuffer是用字符构造的，"0123456789"的长度是10另外再分配16个字符，所以一共是26。
    */

    char c = sbuilder.charAt(6);
    System.out.printf("c=%c\n", c);
    
    char[] carr = new char[4];
    sbuilder.getChars(3, 7, carr, 0);
    for (int i = 0; i < carr.length; i++) {
        System.out.printf("carr[%d]=%c ", i, carr[i]);
    }
    System.out.println();

}
```

### 3、StringBuffer

和StringBulider用法差不多，不过多介绍，主要看一下三者的区别

StringBuffer是线程安全的，推荐在多线程里使用。

### 4、小结

String、StringBuffer、StringBuilder之间的区别

首先需要说明的是：

- String 字符串常量 
- StringBuffer 字符串变量（线程安全） 
- StringBuilder 字符串变量（非线程安全）

在大多数情况下三者在执行速度方面的比较：StringBuilder > StringBuffer > String

解释：

String 类型和 StringBuffer 类型的主要性能区别其实在于 String 是不可变的对象，因此在每次对 String 类型进行改变的时候其实都等同于生成了一个新的 String 对象，然后将指针指向新的 String 对象，所以经常改变内容的字符串最好不要用 String ，因为每次生成对象都会对系统性能产生影响，特别当内存中无引用对象多了以后， JVM 的 GC 就会开始工作，那速度是一定会相当慢的。

而如果是使用 StringBuffer 类则结果就不一样了，每次结果都会对 StringBuffer 对象本身进行操作，而不是生成新的对象，再改变对象引用。所以在一般情况下我们推荐使用 StringBuffer ，特别是字符串对象经常改变的情况下。

为什么是大多数情况呢？

在某些特别情况下， String 对象的字符串拼接其实是被 JVM 解释成了 StringBuffer 对象的拼接， 所以这些时候 String 对象的速度并不会比 StringBuffer 对象慢，而特别是以下的字符串对象生成中， String 效率是远要比 StringBuffer 快的：

```java
String S1 = “This is only a” + “ simple” + “ test”;
StringBuffer Sb = new StringBuilder(“This is only a”).append(“simple”).append(“ test”);
```

你会很惊讶的发现，生成 String S1 对象的速度简直太快了，而这个时候 StringBuffer 居然速度上根本 一点都不占优势。其实这是 JVM 的一个把戏，在 JVM 眼里，这个

String S1 = “This is only a” + “ simple” + “test”;

其实就是：String S1 = “This is only a simple test”;

所以当然不需要太多的时间了。但大家这里要注意的是，如果你的字符串是来自另外的 String 对象 的话，速度就没那么快了，譬如：

> String S2 = “This is only a”;
> String S3 = “ simple”;
> String S4 = “ test”;

大部分情况下StringBuilder的速度要大于StringBuffer：

java.lang.StringBuilder一个可变的字符序列是5.0新增的。（大多数情况下就是我们是在单线程下进行的操作，所以大多数情况下是建议用StringBuilder而不用StringBuffer的）此类提供一个与 StringBuffer 兼容的 API，但不保证同步。该类被设计用作 StringBuffer 的一个简易替换，用在字符串缓冲区被单个 线程使用的时候（这种情况很普遍）。如果可能，建议优先采用该类，因为在大多数实现中，它比 StringBuffer 要快。两者的方法基本相同。

对于三者使用的总结：

- 如果要操作少量的数据用 ：String
- 单线程操作字符串缓冲区 下操作大量数据 ：StringBuilder
- 多线程操作字符串缓冲区 下操作大量数据 ： StringBuffer

### 5、面试题的回答

StringBuilder 与StringBuffer的区别，StringBuilder与String的区别。

1）StringBuilder效率高，线程不安全，StringBuffer对比之下没它高，线程安全。

2）String是不可变字符串，StringBuilder是可变字符串。为什么有这样的差异，可以深入源码去解析， 比如String类内的 priver final char value[] 等方法的原因。

3）如果是简单的声明一个字符串没有后续过多的操作，使用String,StringBuilder均可，若后续对字符穿做频繁的添加，删除操作,或者是在循环当中动态的改变字符穿的长度应该用StringBuilder。使用String 会产生多余的字符串，占用内存空间。

## File类

### 1、File类的基本用法

 java.io.File类：文件和目录路径名的抽象表示形式。

File类的常见构造方法：

```java
public File(String pathname)
```

以pathname为路径创建File对象，如果pathname是相对路径，则默认的当前路径在系统属性user.dir 中存储。

File的静态属性String separator存储了当前系统的路径分隔符。

通过File对象可以访问文件的属性。

```java
public boolean canRead()
public boolean exists()
public boolean isFile()
public long lastModified()
public String getName()
public boolean canWrite()
public boolean isDirectory()
public boolean isHidden()
public long length()
public String getPath()
```

通过File对象创建空文件或目录（在该对象所指的文件或目录不存在的情况下）。

```java
public boolean createNewFile()throws IOException
public boolean delete()
public boolean mkdir()， mkdirs()
```

常见构造器，方法

```java
import java.io.File;
import java.io.IOException;
public class TestFile {
    /**
    * File文件类 1.代表文件 2.代表目录
    */
    public static void main(String[] args) {
        File f = new File("d:/src3/TestObject.java");
        File f2 = new File("d:/src3");
        File f3 = new File(f2, "TestFile.java");
        File f4 = new File(f2, "TestFile666.java");
        File f5 = new File("d:/src3/aa/bb/cc/dd");
        //f5.mkdirs();
        f5.delete();

        try {
            f4.createNewFile();
            System.out.println("文件创建成功！");
        } catch (IOException e) {
            e.printStackTrace();
        }
        if (f.isFile()) {
            System.out.println("是一个文件！");
        }
        if (f2.isDirectory()) {
            System.out.println("是一个目录！");
        }
        if (f3.isFile()) {
            System.out.println("是一个文件奥");
        }
    }
}
```
## 集合概序

### 1、为什么使用集合框架？

假设，一个班级有30个人，我们需要存储学员的信息，是不是我们可以用一个一维数组就解决了？

那换一个问题，一个网站每天要存储的新闻信息，我们知道新闻是可以实时发布的，我们并不知道需要多大的空间去存储，我要是去设置一个很大的数组，要是没有存满，或者不够用，都会影响我们，前者浪费的空间，后者影响了业务！

如果并不知道程序运行时会需要多少对象，或者需要更复杂的方式存储对象，那我们就可以使用Java的集合框架！

### 2、集合框架包含的内容

 Java集合框架提供了一套性能优良，使用方便的接口和类，他们位于java.util包中。

接口和具体类

![image-20210330134353432](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330134353432.png)

算法

Collections 类提供了对集合进行排序，遍历等多种算法实现！

【重中之重】

- Collection 接口存储一组不唯一，无序的对象

- List 接口存储一组不唯一，有序的对象。

- Set 接口存储一组唯一，无序的对象

- Map 接口存储一组键值对象，提供key到value的映射

- ArrayList实现了长度可变的数组，在内存中分配连续的空间。遍历元素和随机访问元素的效率比较高

  ![image-20210330134530971](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330134530971.png)

  ![image-20210330134636140](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330134636140.png)

- LinkedList采用链表存储方式。插入、删除元素时效率比较高

  ![image-20210330134556335](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330134556335.png)

  ![image-20210330134705021](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330134705021.png)

- HashSet:采用哈希算法实现的Set

  HashSet的底层是用HashMap实现的，因此查询效率较高，由于采用hashCode算法直接确定 元素的内存地址，增删效率也挺高的。

  # ArrayList

## ArrayList概述

ArrayList是可以动态增长和缩减的索引序列，它是基于数组实现的List类。

该类封装了一个动态再分配的Object[]数组，每一个类对象都有一个capacity【容量】属性，表示它们所封装的Object[]数组的长度，当向ArrayList中添加元素时，该属性值会自动增加。如果想 ArrayList中添加大量元素，可使用ensureCapacity方法一次性增加capacity，可以减少增加重分配的次数提高性能。

ArrayList的用法和Vector向类似，但是Vector是一个较老的集合，具有很多缺点，不建议使用。

另外，ArrayList和Vector的区别是：ArrayList是线程不安全的，当多条线程访问同一个ArrayList集合时，程序需要手动保证该集合的同步性，而Vector则是线程安全的。

ArrayList和Collection的关系：

![image-20210330144341316](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330144341316.png)

## ArrayList的数据结构

分析一个类的时候，数据结构往往是它的灵魂所在，理解底层的数据结构其实就理解了该类的实现思 路，具体的实现细节再具体分析。

ArrayList的数据结构是：

![image-20210330144539830](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330144539830.png)

说明：底层的数据结构就是数组，数组元素类型为Object类型，即可以存放所有类型数据。我们对 ArrayList类的实例的所有的操作底层都是基于数组的。

## ArrayList源码分析

### 1、继承结构和层次关系

IDEA快捷键：Ctrl+H

![image-20210330144845625](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330144845625.png)

```java
public class ArrayList<E> extends AbstractList<E>
implements List<E>, RandomAccess, Cloneable, java.io.Serializable{
    
}
```

我们看一下ArrayList的继承结构：

ArrayList extends AbstractList       AbstractList extends AbstractCollection

所有类都继承Object 所以ArrayList的继承结构就是上图这样。

【分析】

**为什么要先继承AbstractList，而让AbstractList先实现List？而不是让ArrayList直接实现List？**

这里是有一个思想，接口中全都是抽象的方法，而抽象类中可以有抽象方法，还可以有具体的实现方法，正是利用了这一点，让AbstractList是实现接口中一些通用的方法，而具体的类，如ArrayList就继承这个AbstractList类，拿到一些通用的方法，然后自己在实现一些自己特有的方法，这样一来，让代码更简洁，就继承结构最底层的类中通用的方法都抽取出来，先一起实现了，减少重复代码。所以一般看到 一个类上面还有一个抽象类，应该就是这个作用。

**ArrayList实现了哪些接口？**

**List接口**：我们会出现这样一个疑问，在查看了ArrayList的父类 AbstractList也实现了List接口，那为什么子类ArrayList还是去实现一遍呢？

这是想不通的地方，查资料显示，有的人说是为了查看代码方便，使观看者一目了然，说法不 一，但每一个让我感觉合理的，但是在stackOverFlow中找到了答案，这里其实很有趣。

开发这个collection 的作者Josh说：

这其实是一个mistake[失误]，因为他写这代码的时候觉得这个会有用处，但是其实并没什么用，但因为没什么影响，就一直留到了现在。

**RandomAccess接口**：这个是一个标记性接口，通过查看api文档，它的作用就是用来快速随机存取， 有关效率的问题，在实现了该接口的话，那么使用普通的for循环来遍历，性能更高，例如ArrayList。而没有实现该接口的话，使用Iterator来迭代，这样性能更高，例如linkedList。所以这个标记性只是为了 让我们知道我们用什么样的方式去获取数据性能更好。

**Cloneable接口**：实现了该接口，就可以使用Object.Clone()方法了。

**Serializable接口**：实现该序列化接口，表明该类可以被序列化，什么是序列化？简单的说，就是能够 从类变成字节流传输，然后还能从字节流变成原来的类。

### 2、类中的属性

```java
public class ArrayList<E> extends AbstractList<E>
implements List<E>, RandomAccess, Cloneable, java.io.Serializable
    {
    // 版本号
    private static final long serialVersionUID = 8683452581122892189L;
    // 缺省容量
    private static final int DEFAULT_CAPACITY = 10;
    // 空对象数组
    private static final Object[] EMPTY_ELEMENTDATA = {};
    // 缺省空对象数组
    private static final Object[] DEFAULTCAPACITY_EMPTY_ELEMENTDATA = {};
    // 元素数组
    transient Object[] elementData;
    // 实际元素大小，默认为0
    private int size;
    // 最大数组容量
    private static final int MAX_ARRAY_SIZE = Integer.MAX_VALUE - 8;
}
```

### 3、构造方法

![image-20210330145750383](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330145750383.png)

无参构造方法

```java
/*
    Constructs an empty list with an initial capacity of ten.
    这里就说明了默认会给10的大小，所以说一开始arrayList的容量是10.
*/
//ArrayList中储存数据的其实就是一个数组，这个数组就是elementData.
public ArrayList() {
    super(); //调用父类中的无参构造方法，父类中的是个空的构造方法
    this.elementData = EMPTY_ELEMENTDATA;
    //EMPTY_ELEMENTDATA：是个空的Object[]， 将elementData初始化，elementData也是个Object[]类型。空的Object[]会给默认大小10，等会会解释什么时候赋值的。
}
```

有参构造方法1

```java
/*
Constructs an empty list with the specified initial capacity.
构造具有指定初始容量的空列表。

@param initialCapacity the initial capacity of the list
初始容量列表的初始容量

@throws IllegalArgumentException if the specified initial capacity is negative
如果指定的初始容量为负，则为IllegalArgumentException
*/

public ArrayList(int initialCapacity) {
    if (initialCapacity > 0) {
        //将自定义的容量大小当成初始化 initialCapacity 的大小
        this.elementData = new Object[initialCapacity];
    } else if (initialCapacity == 0) {
        this.elementData = EMPTY_ELEMENTDATA; //等同于无参构造方法
    } else {
        //判断如果自定义大小的容量小于0，则报下面这个非法数据异常
        throw new IllegalArgumentException("Illegal Capacity: "+initialCapacity);
    }
}
```

有参构造方法 2

```java
/*
    Constructs a list containing the elements of the specified collection,in the order they are returned by the collection's iterator.
    按照集合迭代器返回元素的顺序构造包含指定集合的元素的列表。
    @param c the collection whose elements are to be placed into this list
    @throws NullPointerException if the specified collection is null
*/
public ArrayList(Collection<? extends E> c) {
    elementData = c.toArray(); //转换为数组
    //每个集合的toarray()的实现方法不一样，所以需要判断一下，如果不是Object[].class类型，那么久需要使用ArrayList中的方法去改造一下。
    if ((size = elementData.length) != 0) {
   		 // c.toArray might (incorrectly) not return Object[] (see 6260652)
   		 if (elementData.getClass() != Object[].class)
    		 elementData = Arrays.copyOf(elementData, size, Object[].class);
    } else {
        // replace with empty array.
    	this.elementData = EMPTY_ELEMENTDATA;
    }
}
```

这个构造方法不常用，举个例子就能明白什么意思

举个例子： Strudent exends Person ， ArrayList、 Person这里就是泛型 ， 我还有一个Collection、 由于这个Student继承了Person，那么根据这个构造方法，我就可以把这个Collection转换为ArrayList ， 这就是这个构造方法的作用 。

【总结】ArrayList的构造方法就做一件事情，就是初始化一下储存数据的容器，其实本质上就是一个数 组，在其中就叫elementData。

### 4、核心方法-add

**alt+7 查看方法列表，ctrl+左键 选中add进去后查看**

**boolean add(E)**

```java
/**
* Appends the specified element to the end of this list.
* 添加一个特定的元素到list的末尾。
* @param e element to be appended to this list
* @return <tt>true</tt> (as specified by {@link Collection#add})
*/
public boolean add(E e) {
    //确定内部容量是否够了，size是数组中数据的个数，因为要添加一个元素，所以size+1，先判断size+1的这个数数组能否放得下，就在这个方法中去判断是否数组.length是否够用了。
    ensureCapacityInternal(size + 1); // Increments modCount!!
    elementData[size++] = e; //在数据中正确的位置上放上元素e，并且size++
    return true;
}
```

【分析：ensureCapacityInternal(xxx); 确定内部容量的方法】

```java
private void ensureCapacityInternal(int minCapacity) {
	ensureExplicitCapacity(calculateCapacity(elementData, minCapacity));
}

private static int calculateCapacity(Object[] elementData, int minCapacity){
    //看，判断初始化的elementData是不是空的数组，也就是没有长度
    if (elementData == DEFAULTCAPACITY_EMPTY_ELEMENTDATA) {
        //因为如果是空的话，minCapacity=size+1；其实就是等于1，空的数组没有长度就存放不了，所以就将minCapacity变成10，也就是默认大小，但是在这里，还没有真正的初始化这个elementData的大小。
        return Math.max(DEFAULT_CAPACITY, minCapacity);
    }
    //确认实际的容量，上面只是将minCapacity=10，这个方法就是真正的判断elementData是否够用
    return minCapacity;
}

private void ensureExplicitCapacity(int minCapacity) {
    modCount++;
    //  overflow-conscious code
    //minCapacity如果大于了实际elementData的长度，那么就说明elementData数组的长度不够用，不够用那么就要增加elementData的length。这里有的同学就会模糊minCapacity到底是什么呢，这里给你们分析一下
    /*
    第一种情况：由于elementData初始化时是空的数组，那么第一次add的时候，minCapacity=size+1；也就minCapacity=1，在上一个方法(确定内部容量ensureCapacityInternal)就会判断出是空的数组，就会给将minCapacity=10，到这一步为止，还没有改变elementData的大小。
    
	第二种情况：elementData不是空的数组了，那么在add的时候，minCapacity=size+1；也就是minCapacity代表着elementData中增加之后的实际数据个数，拿着它判断elementData的length是否够用，如果length不够用，那么肯定要扩大容量，不然增加的这个元素就会溢出。
*/
    if (minCapacity - elementData.length > 0)
		grow(minCapacity);
}
//arrayList核心的方法，能扩展数组大小的真正秘密。
private void grow(int minCapacity) {
    // overflow-conscious code
    
    //将扩充前的elementData大小给oldCapacity
    int oldCapacity = elementData.length;
    
    //newCapacity就是1.5倍的oldCapacity
    int newCapacity = oldCapacity + (oldCapacity >> 1);
    
    //这句话就是适应于elementData就空数组的时候，length=0，那么oldCapacity=0，newCapacity=0，所以这个判断成立，在这里就是真正的初始化elementData的大小了，就是为10.前面的工作都是准备工作。
    if (newCapacity - minCapacity < 0)
		newCapacity = minCapacity;
    
    //如果newCapacity超过了最大的容量限制，就调用hugeCapacity，也就是将能给的最大值给newCapacity
    if (newCapacity - MAX_ARRAY_SIZE > 0)
        newCapacity = hugeCapacity(minCapacity);
    // minCapacity is usually close to size, so this is a win:
    //新的容量大小已经确定好了，就copy数组，改变容量大小咯。
    elementData = Arrays.copyOf(elementData, newCapacity);
}
    

//这个就是上面用到的方法，很简单，就是用来赋最大值
private static int hugeCapacity(int minCapacity) {
    if (minCapacity < 0) // overflow
        throw new OutOfMemoryError();
    
//如果minCapacity都大于MAX_ARRAY_SIZE，那么就Integer.MAX_VALUE返回，反之将MAX_ARRAY_SIZE返回。因为maxCapacity是三倍的minCapacity，可能扩充的太大了，就用minCapacity来判断了。

//Integer.MAX_VALUE:2147483647 MAX_ARRAY_SIZE：2147483639 也就是说最大也就能给到第一个数值。还是超过了这个限制，就要溢出了。相当于arraylist给了两层防护。    
    return (minCapacity > MAX_ARRAY_SIZE) ?
        Integer.MAX_VALUE :
    MAX_ARRAY_SIZE;
}

    
```



**void add(int，E)**

```java
public void add(int index, E element) {
    //检查index也就是插入的位置是否合理。
    rangeCheckForAdd(index);
    
    ensureCapacityInternal(size + 1); // Increments modCount!!
    
    //这个方法就是用来在插入元素之后，要将index之后的元素都往后移一位，
    System.arraycopy(elementData, index, elementData, index + 1,
    					size - index);
    
    //在目标位置上存放元素
    elementData[index] = element;
    size++;
}
```

【分析：rangeCheckForAdd(index)】

```java
private void rangeCheckForAdd(int index) {
    //插入的位置肯定不能大于size 和小于0
    if (index > size || index < 0)
        //如果是，就报这个越界异常
        throw new IndexOutOfBoundsException(outOfBoundsMsg(index));
}
```

【System.arraycopy(...)：就是将elementData在插入位置后的所有元素，往后面移一位】

```java
public static void arraycopy(Object src,
            int srcPos,
            Object dest,
            int destPos,
            int length)

    //src：源对象
    //srcPos：源对象对象的起始位置
    //dest：目标对象
    //destPost：目标对象的起始位置
    //length：从起始位置往后复制的长度。
  
```

**注释解读：**

这段的大概意思就是解释这个方法的用法，复制src到dest，复制的位置是从src的srcPost开始，到srcPost+length-1的位置结束，复制到destPost上，从destPost开始到destPost+length-1的位置上

![image-20210330155111328](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330155111328.png)

告诉你复制的一种情况，如果A和B是一样的，那么先将A复制到临时数组C，然后通过C复制到B，用了一个第三方参数

![image-20210330155151694](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330155151694.png)

这一大段，就是来说明会出现的一些问题，NullPointerException和IndexOutOfBoundsException 还有ArrayStoreException 这三个异常出现的原因。

![image-20210330155313786](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330155313786.png)

这里描述了一种特殊的情况，就是当A的长度大于B的长度的时候，会复制一部分，而不是完全失败。

![image-20210330155350320](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330155350320.png)

这些是参数列表的解释和异常

![image-20210330155421252](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330155421252.png)

:scream:读别人源码是件很头疼的事，新手会用就行，原理等以后回来复习的时候再看~

【总结】

正常情况下会扩容1.5倍，特殊情况下（新扩展数组大小已经达到了最大值）则只取最大值。

当我们调用add方法时，实际上的函数调用如下：

![image-20210330161507771](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330161507771.png)

说明：程序调用add，实际上还会进行一系列调用，可能会调用到grow，grow可能会调用hugeCapacity。

【举例】

```java
List<Integer> lists = new ArrayList<Integer>;
lists.add(8);
```

说明：初始化lists大小为0，调用的ArrayList()型构造函数，那么在调用lists.add(8)方法时，会经过怎样 的步骤呢？下图给出了该程序执行过程和最初与最后的elementData的大小。

![image-20210330161955630](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330161955630.png)

说明：我们可以看到，在add方法之前开始elementData = {}；调用add方法时会继续调用，直至 grow，最后elementData的大小变为10，之后再返回到add函数，把8放在elementData[0]中。

【举例说明二】

```java
List<Integer> lists = new ArrayList<Integer>(6);
lists.add(8);
```

说明：调用的ArrayList(int)型构造函数，那么elementData被初始化为大小为6的Object数组，在调用add(8)方法时，具体的步骤如下：

![image-20210330162415006](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330162415006.png)

说明：我们可以知道，在调用add方法之前，elementData的大小已经为6，之后再进行传递，不会进行 扩容处理。

推荐文章系列： [【集合框架】JDK1.8源码分析之HashMap（一）](https://www.cnblogs.com/leesf456/p/5242233.html)

### 5、核心方法-remove

其实这几个删除方法都是类似的。我们选择几个讲，其中fastRemove(int)方法是private的，是提供给 remove(Object)这个方法用的。

remove(int)：通过删除指定位置上的元素

```java
public E remove(int index) {
    rangeCheck(index);//检查index的合理性
    
    modCount++;//这个作用很多，比如用来检测快速失败的一种标志。
    E oldValue = elementData(index);//通过索引直接找到该元素
    
    int numMoved = size - index - 1;//计算要移动的位数。
    if (numMoved > 0)
    	//这个方法也已经解释过了，就是用来移动元素的。
    	System.arraycopy(elementData, index+1, elementData, index,numMoved);
    //将--size上的位置赋值为null，让gc(垃圾回收机制)更快的回收它。
    elementData[--size] = null; // clear to let GC do its work
    //返回删除的元素。
    return oldValue;
}
```

remove(Object)：这个方法可以看出来，arrayList是可以存放null值

```java
//通过元素来删除该元素，就依次遍历，如果有这个元素，就将该元素的索引传给fastRemobe(index)，使用这个方法来删除该元素，
//fastRemove(index)方法的内部跟remove(index)的实现几乎一样，这里最主要是知道arrayList可以存储null值
public boolean remove(Object o) {
    if (o == null) {
    	for (int index = 0; index < size; index++)
        	if (elementData[index] == null) {
                fastRemove(index);
                return true;
    		}
    } else {
        for (int index = 0; index < size; index++)
            if (o.equals(elementData[index])) {
                fastRemove(index);
                return true;
            }
    }
    return false;
}
```

clear()：将elementData中每个元素都赋值为null，等待垃圾回收将这个给回收掉，所以叫clear

```java
public void clear() {
    modCount++;
    
    // clear to let GC do its work
    for (int i = 0; i < size; i++)
    	elementData[i] = null;
    size = 0;
}
```

removeAll(collection c)

```java
public boolean removeAll(Collection<?> c) {
	return batchRemove(c, false);//批量删除
}
```

batchRemove(xx,xx)：用于两个方法，一个removeAll()：它只清楚指定集合中的元素，retainAll() 用来测试两个集合是否有交集。

```java
//这个方法，用于两处地方，如果complement为false，则用于removeAll如果为true，则给retainAll()用，retainAll（）是用来检测两个集合是否有交集的。

private boolean batchRemove(Collection<?> c, boolean complement) {
        final Object[] elementData = this.elementData; //将原集合，记名为A
        int r = 0, w = 0;  //r用来控制循环，w是记录有多少个交集
        boolean modified = false;
        try {
            for (; r < size; r++)
                //参数中的集合C一次检测集合A中的元素是否有，
                if (c.contains(elementData[r]) == complement)
                    //有的话，就给集合A
                    elementData[w++] = elementData[r];
        } finally {
            // Preserve behavioral compatibility with AbstractCollection,
            // even if c.contains() throws.
            //如果contains方法使用过程报异常
            if (r != size) {
                //将剩下的元素都赋值给集合A，
                System.arraycopy(elementData, r,
                                 elementData, w,
                                 size - r);
                w += size - r;
            }
            if (w != size) {
                // clear to let GC do its work
                //这里有两个用途，在removeAll()时，w一直为0，就直接跟clear一样，全是为null。
                //retainAll()：没有一个交集返回true，有交集但不全交也返回true，而两个集合相等的时候，返回false，所以不能根据返回值来确认两个集合是否有交集，而是通过原集合的大小是否发生改变来判断，如果原集合中还有元素，则代表有交集，而元集合没有元素了，说明两个集合没有交集。

                for (int i = w; i < size; i++)
                    elementData[i] = null;
                modCount += size - w;
                size = w;
                modified = true;
            }
        }
        return modified;
    }
```

总结：remove函数，用户移除指定下标的元素，此时会把指定下标到数组末尾的元素向前移动一个单 位，并且会把数组最后一个元素设置为null，这样是为了方便之后将整个数组不被使用时，会被GC，可 以作为小的技巧使用。

### 6、其他方法

**set()方法**

说明：设定指定下标索引的元素值

```java
public E set(int index, E element) {
    // 检验索引是否合法
    rangeCheck(index);
    // 旧值
    E oldValue = elementData(index);
    // 赋新值
    elementData[index] = element;
    // 返回旧值
    return oldValue;
}
```

**indexOf()方法**

说明：从头开始查找与指定元素相等的元素，注意，是可以查找null元素的，意味着ArrayList中可以存放null元素的。与此函数对应的lastIndexOf，表示从尾部开始查找。

```java
// 从首开始查找数组里面是否存在指定元素
public int indexOf(Object o) {
    if (o == null) { // 查找的元素为空
        for (int i = 0; i < size; i++) // 遍历数组，找到第一个为空的元素，返回下标
        	if (elementData[i]==null)
        		return i;
    } else { // 查找的元素不为空
        for (int i = 0; i < size; i++) // 遍历数组，找到第一个和指定元素相等的元素，返回下标
        if (o.equals(elementData[i]))
        	return i;
    }
    // 没有找到，返回空
    return -1;
}
```

**get()方法**

```java
public E get(int index) {
    // 检验索引是否合法
    rangeCheck(index);
    return elementData(index);
}
```

说明：get函数会检查索引值是否合法（只检查是否大于size，而没有检查是否小于0），值得注意的 是，在get函数中存在element函数，element函数用于返回具体的元素，具体函数如下：

```java
E elementData(int index) {
	return (E) elementData[index];
}
```

说明：返回的值都经过了向下转型（Object -> E），这些是对我们应用程序屏蔽的小细节。

## ArrayList实践

问题：我们现在有4只小狗，我们如何存储它的信息，获取总数，并能够逐条打印狗狗信息！

分析：通过List 接口的实现类ArrayList 实现该需求。

- 元素个数不确定
- 要求获得元素的实际个数
- 按照存储顺序获取并打印元素信息

```java
class Dog {
    private String name;
    //构造。。。set、get、。。。toString（）
}
```

```java
public class TestArrayList {
    public static void main(String[] args) {
        //创建ArrayList对象 , 并存储狗狗
        List dogs = new ArrayList();
        
        dogs.add(new Dog("小狗一号"));
        dogs.add(new Dog("小狗二号"));
        dogs.add(new Dog("小狗三号"));
        dogs.add(2,new Dog("小狗四号"));// 添加到指定位置
        
        // .size() ： ArrayList大小
        System.out.println("共计有" + dogs.size() + "条狗狗。");
        System.out.println("分别是：");
        
        // .get(i) ： 逐个获取个元素
        for (int i = 0; i < dogs.size(); i++) {
            Dog dog = (Dog) dogs.get(i);
            System.out.println(dog.getName());
        }
    }
}
```

问题联想：

- 删除第一个狗狗 ：remove（index）
- 删除指定位置的狗狗 ：remove（object）
- 判断集合中是否包含指定狗狗 ： contains（object）

分析：使用List接口提供的remove()、contains()方法

【常用方法】

![image-20210330141203456](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330141203456.png)



## 总结

* 1）arrayList可以存放null。
* 2）arrayList本质上就是一个elementData数组。
* 3）arrayList区别于数组的地方在于能够自动扩展大小，其中关键的方法就是gorw()方法。
* 4）arrayList中removeAll(collection c)和clear()的区别就是removeAll可以删除批量指定的元素，而clear是全是删除集合中的元素。
* 5）arrayList由于本质是数组，所以它在数据的查询方面会很快，而在插入删除这些方面，性能下降很多，有移动很多数据才能达到应有的效果
* 6）arrayList实现了RandomAccess，所以在遍历它的时候推荐使用for循环。

# LinkedList

## 引入

问题：在集合的任何位置（头部，中间，尾部）添加，获取，删除狗狗对象！

插入，删除操作频繁时，可使用LinkedList来提高效率

LinkedList提供对头部和尾部元素进行添加和删除操作的方法！

![image-20210330184629619](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330184629619.png)

**LinkedList的特殊方法**

![image-20210330184756855](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330184756855.png)

集合框架有何好处？
Java集合框架中包含哪些接口和类？
ArrayList和LinkedList有何异同？



## LinkedList概述

我们都知道它的底层是由链表实现的，所以我们要明白什么是链表？

![img](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/050053434697439.png)

LinkedList是一种可以在任何位置进行高效地插入和移除操作的有序序列，它是基于双向链表实现的。

LinkedList 是一个继承于AbstractSequentialList的双向链表。它也可以被当作堆栈、队列或双端队列进行操作。

LinkedList 实现 List 接口，能对它进行队列操作。

LinkedList 实现 Deque 接口，即能将LinkedList当作双端队列使用。

LinkedList 实现了Cloneable接口，即覆盖了函数clone()，能克隆。

LinkedList 实现java.io.Serializable接口，这意味着LinkedList支持序列化，能通过序列化去传输。

LinkedList 是非同步的。

推荐文章：[LinkList详解](https://blog.csdn.net/qedgbmwyz/article/details/80108618)

## 链表的数据结构

**单向链表：**

 element：用来存放元素

 next：用来指向下一个节点元素

通过每个结点的指针指向下一个结点从而链接起来的结构，最后一个节点的next指向null。

![image-20210330215243376](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330215243376.png)

**单向循环链表：**

 element、next 跟前面一样，在单向链表的最后一个节点的next会指向头节点，而不是指向null，这样存成一个环

![image-20210330215349904](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330215349904.png)



**双向链表：**

element：存放元素

pre：用来指向前一个元素

next：指向后一个元素

双向链表是包含两个指针的，pre指向前一个节点，next指向后一个节点，但是第一个节点head的pre指向null，最后一个节点的tail指向null。

![image-20210330215814374](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330215814374.png)



**双向循环链表：**

 element、pre、next 跟前面的一样

第一个节点的pre指向最后一个节点，最后一个节点的next指向第一个节点，也形成一个“环”。

![image-20210330215757946](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330215757946.png)

**【LinkedList的数据结构】**

![image-20210330215856514](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330215856514.png)

如上图所示，LinkedList底层使用的双向链表结构，有一个头结点和一个尾结点，双向链表意味着我们可以从头开始正向遍历，或者是从尾开始逆向遍历，并且可以针对头部和尾部进行相应的操作。



## LinkedList源码分析

接下来又到了大家喜欢的读源码环节**:smile:**

### 1、LinkedList的特性

在我们平常中，我们只知道一些常识性的特点：

1）是通过链表实现的 
2）如果在频繁的插入，或者删除数据时，就用linkedList性能会更好。

那我们通过API去查看它的一些特性

>Doubly-linked list implementation of the List and Deque interfaces. Implements all optional list operations, and permits all elements (including null).
>
>这告诉我们，linkedList是一个双向链表，并且实现了List和Deque接口中所有的列表操作，并且能存储任何元素，包括null，这里我们可以知道linkedList除了可以当链表使用，还可以当作队列使用，并能进行相应的操作。
>
>All of the operations perform as could be expected for a doubly-linked list. Operations that index into the list will traverse the list from the beginning or the end, whichever is closer to the specified index.
>
>这个告诉我们，linkedList在执行任何操作的时候，都必须先遍历此列表来靠近通过index查找我们所需要的的值。通俗点讲，这就告诉了我们这个是顺序存取，每次操作必须先按开始到结束的顺序遍历，随机存取，就是arrayList，能够通过index。随便访问其中的任意位置的数据，这就是随机列表的意思。

3）api中接下来讲的一大堆，就是说明linkedList是一个非线程安全的(异步)，其中在操作Interator时， 如果改变列表结构(adddelete等)，会发生fail-fast。

**通过API再次总结一下LinkedList的特性：**

1. 异步，也就是非线程安全

2. 双向链表。由于实现了list和Deque接口，能够当作队列来使用。

   链表：查询效率不高，但是插入和删除这种操作性能好。

3. 是顺序存取结构（注意和随机存取结构两个概念搞清楚）



### 2、继承结构以及层次关系

ctrl+h

![image-20210330221055477](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330221055477.png)

我们可以看到，linkedList在最底层，说明他的功能最为强大，并且细心的还会发现，arrayList有四层，这里多了一层AbstractSequentialList的抽象类，为什么呢？

**通过API我们会发现：**

 1）减少实现顺序存取（例如LinkedList）这种类的工作，通俗的讲就是方便，抽象出类似LinkedList这种类的一些共同的方法

2）既然有了上面这句话，那么以后如果自己想实现顺序存取这种特性的类(就是链表形式)，那么就继承这个AbstractSequentialList抽象类，如果想像数组那样的随机存取的类，那么就去实现AbstracList抽象类。

3）这样的分层，就很符合我们抽象的概念，越在高处的类，就越抽象，往在底层的类，就越有自己独特的个性。自己要慢慢领会这种思想。

4）LinkedList的类继承结构很有意思，我们着重要看是Deque接口，Deque接口表示是一个双端队列，那么也意味着LinkedList是双端队列的一种实现，所以，基于双端队列的操作在LinkedList中全部有效。

```java
public abstract class AbstractSequentialList<E>
extends AbstractList<E>
```



![image-20210330221915604](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330221915604.png)

第一段：

> 这里第一段就解释了这个类的作用，这个类为实现list接口提供了一些重要的方法，
> 尽最大努力去减少实现这个“顺序存取”的特性的数据存储(例如链表)的什么
> 随机存取数据(例如数组)的类应该优先使用AbstractList
> 从上面就可以大概知道，AbstractSwquentialList这个类是为了减少LinkedList这种顺序存取的类的代码复杂度而抽象的一个类，

第二段：

> 这一段大概讲的就是这个AbstractSequentialList这个类和AbstractList这个类是完全相反 的。比如get、add这个方法的实现

第三段：

> 这里就是讲一些我们自己要继承该类，该做些什么事情，一些规范。



**【接口实现分析】**

```java
public class LinkedList<E>
    extends AbstractSequentialList<E>
    implements List<E>, Deque<E>, Cloneable, java.io.Serializable
    {
    
    }
```

1. List接口：列表，add、set、等一些对列表进行操作的方法

2. Deque接口：有队列的各种特性，

3. Cloneable接口：能够复制，使用那个copy方法。

4. Serializable接口：能够序列化。

5. 应该注意到没有RandomAccess：那么就推荐使用iterator，在其中就有一个foreach，增强的for循环，其中原理也就是iterator，我们在使用的时候，使用foreach或者iterator都可以。

   iterator：

   ```java
   public static void method() {
       List<String> l = new ArrayList<>();
   
       l.add("hello");
       l.add(0, "123");
       l.add("789");
       l.set(0, "456");
       l.remove(0);
   
       ListIterator<String> lit = l.listIterator();
       while (lit.hasNext()) {
           String next = lit.next();
   //            l.add("111");
           lit.add("111");
           System.out.println(next);
   
       }
       System.out.println(l);
   }
   ```

### 3、类的属性

```java
public class LinkedList<E>
    extends AbstractSequentialList<E>
    implements List<E>, Deque<E>, Cloneable, java.io.Serializable
{
    // 实际元素个数
    transient int size = 0;
    // 头结点
    transient Node<E> first;
    // 尾结点
    transient Node<E> last;
}
```

LinkedList的属性非常简单，一个头结点、一个尾结点、一个表示链表中实际元素个数的变量。注意， 头结点、尾结点都有transient关键字修饰，这也意味着在序列化时该域是不会序列化的。

### 4、构造方法

两个构造方法(两个构造方法都是规范规定需要写的）

【空参构造函数】

```java
public LinkedList() {
    
}
```

【有参构造函数】

```java
//将集合c中的各个元素构建成LinkedList链表。
public LinkedList(Collection<? extends E> c) {
    // 调用无参构造函数
    this();
    // 添加集合中所有的元素
    addAll(c);
}
```

说明：会调用无参构造函数，并且会把集合中所有的元素添加到LinkedList中。

### 5、内部类（Node）

```java
//根据前面介绍双向链表就知道这个代表什么了，linkedList的奥秘就在这里。
private static class Node<E> {
    E item; // 数据域（当前节点的值）
    Node<E> next; // 后继（指向当前一个节点的后一个节点）
    Node<E> prev; // 前驱（指向当前节点的前一个节点）
    
    // 构造函数，赋值前驱后继
    Node(Node<E> prev, E element, Node<E> next) {
        this.item = element;
        this.next = next;
        this.prev = prev;
    }
}
```

说明：内部类Node就是实际的结点，用于存放实际元素的地方。

### 6、核心方法

#### add()方法

```java
public boolean add(E e) {
    // 添加到末尾
    linkLast(e);
    return true;
}
```

说明：add函数用于向LinkedList中添加一个元素，并且添加到链表尾部。具体添加到尾部的逻辑是由 linkLast函数完成的。



**【LinkLast(XXXXX)】**

```java
/**
 * Links e as last element.
 */
void linkLast(E e) {
    final Node<E> l = last; //临时节点l(L的小写)保存last，也就是l指向了最后一个节点
    final Node<E> newNode = new Node<>(l, e, null);////将e封装为节点，并且e.prev指向了最后一个节点
    last = newNode;//newNode成为了最后一个节点，所以last指向了它
    if (l == null)//判断是不是一开始链表中就什么都没有，如果没有，则newNode就成为了第一个节点，first和last都要指向它
        first = newNode;
    else  //正常的在最后一个节点后追加，那么原先的最后一个节点的next就要指向现在真正的最后一个节点，原先的最后一个节点就变成了倒数第二个节点
        l.next = newNode;
    size++; ;//添加一个节点，size自增
    modCount++;
}
```

说明：对于添加一个元素至链表中会调用add方法 -> linkLast方法。

【举例一】

```java
List<Integer> lists = new LinkedList<Integer>();
lists.add(5);
lists.add(6);
```

首先调用无参构造函数，之后添加元素5，之后再添加元素6。具体的示意图如下：

![image-20210330223637307](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330223637307.png)

上图的表明了在执行每一条语句后，链表对应的状态。

#### addAll()方法

addAll有两个重载函数，addAll(Collection)型和addAll(int, Collection) 型，我们平时习惯调用的addAll(Collection)型会转化为addAll(int, Collection)型。

```java
public boolean addAll(Collection<? extends E> c) {
//继续往下看
return addAll(size, c);
}
```

addAll(size，c)：这个方法，能包含三种情况下的添加，我们这里分析的只是构造方法，空链表的情况，看的时候只需要按照不同的情况分析下去就行了。

```java
//真正核心的地方就是这里了，记得我们传过来的是size，c
public boolean addAll(int index, Collection<? extends E> c) {
    //检查index这个是否为合理。这个很简单，自己点进去看下就明白了。
    checkPositionIndex(index);
	//将集合c转换为Object数组 a
    Object[] a = c.toArray();
    //数组a的长度numNew，也就是由多少个元素
    int numNew = a.length;
    if (numNew == 0)
        //集合c是个空的，直接返回false，什么也不做。
        return false;
	//集合c是非空的，定义两个节点(内部类)，每个节点都有三个属性，item、next、prev。注意：不要管这两个什么含义，就是用来做临时存储节点的。这个Node看下面一步的源码分析，Node就是linkedList的最核心的实现，可以直接先跳下一个去看Node的分析
    Node<E> pred, succ;
    //构造方法中传过来的就是index==size
    if (index == size) {
        //linkedList中三个属性：size、first、last。 size：链表中的元素个数。first：头节点 last：尾节点，就两种情况能进来这里
        //情况一、：构造方法创建的一个空的链表，那么size=0，last、和first都为null。linkedList中是空的。什么节点都没有。succ=null、pred=last=null
        
        //情况二、：链表中有节点，size就不是为0，first和last都分别指向第一个节点，和最后一个节点，在最后一个节点之后追加元素，就得记录一下最后一个节点是什么，所以把last保存到pred临时节点中。

        succ = null;
        pred = last;
    } else {
        //情况三、index！=size，说明不是前面两种情况，而是在链表中间插入元素，那么就得知道index上的节点是谁，保存到succ临时节点中，然后将succ的前一个节点保存到pred中，这样保存了这两个节点，就能够准确的插入节点了
        //举个简单的例子，有2个位置，1、2、如果想插数据到第二个位置，双向链表中，就需要知道第一个位置是谁，原位置也就是第二个位置上是谁，然后才能将自己插到第二个位置上。如果这里还不明白，先看一下文章开头对于各种链表的删除，add操作是怎么实现的。
        succ = node(index);
        pred = succ.prev;
    }
	//前面的准备工作做完了，将遍历数组a中的元素，封装为一个个节点。
    for (Object o : a) {
        @SuppressWarnings("unchecked") E e = (E) o;
        //pred就是之前所构建好的，可能为null、也可能不为null，为null的话就是属于情况一、不为null则可能是情况二、或者情况三

        Node<E> newNode = new Node<>(pred, e, null);
        //如果pred==null，说明是情况一，构造方法，是刚创建的一个空链表，此时的newNode就当作第一个节点，所以把newNode给first头节点
        if (pred == null)
            first = newNode;
        else
            //如果pred！=null，说明可能是情况2或者情况3，如果是情况2，pred就是last，那么在最后一个节点之后追加到newNode，如果是情况3，在中间插入，pred为原index节点之前的一个节点，将它的next指向插入的节点，也是对的
            pred.next = newNode;
        //然后将pred换成newNode，注意，这个不在else之中，请看清楚了。
        pred = newNode;
    }

    if (succ == null) {
        /*如果succ==null，说明是情况一或者情况二，
		情况一、构造方法，也就是刚创建的一个空链表，pred已经是newNode了，last=newNode，所以linkedList的first、last都指向第一个节点。
		情况二、在最后节后之后追加节点，那么原先的last就应该指向现在的最后一个节点
了，就是newNode。*/
        last = pred;
    } else {
        //如果succ！=null，说明可能是情况三、在中间插入节点，举例说明这几个参数的意义，有1、2两个节点，现在想在第二个位置插入节点newNode，根据前面的代码，pred=newNode，succ=2，并且1.next=newNode，已经构建好了，pred.next=succ，相当于在newNode.next =2； succ.prev = pred，相当于 2.prev = newNode， 这样一来，这种指向关系就完成了。first和last不用变，因为头节点和尾节点没变
        pred.next = succ;
        succ.prev = pred;
    }
	//增加了几个元素，就把 size = size +numNew 就可以了
    size += numNew;
    modCount++;
    return true;
}
```

说明：参数中的index表示在索引下标为index的结点（实际上是第index + 1个结点）的前面插入。

在addAll函数中，addAll函数中还会调用到node函数，get函数也会调用到node函数，此函数是根据索引下标找到该结点并返回，具体代码如下：

```java
Node<E> node(int index) {
    // assert isElementIndex(index);
	// 判断插入的位置在链表前半段或者是后半段
    if (index < (size >> 1)) {// 插入位置在前半段
        Node<E> x = first;
        for (int i = 0; i < index; i++)// 从头结点开始正向遍历
            x = x.next;
        return x;// 返回该结点
    } else {// 插入位置在后半段
        Node<E> x = last;
        for (int i = size - 1; i > index; i--)// 从尾结点开始反向遍历
            x = x.prev;
        return x;// 返回该结点
    }
}
```

说明：在根据索引查找结点时，会有一个小优化，结点在前半段则从头开始遍历，在后半段则从尾开始遍历，这样就保证了只需要遍历最多一半结点就可以找到指定索引的结点。

举例说明调用addAll函数后的链表状态：

```java
List<Integer> lists = new LinkedList<Integer>();
lists.add(5);
lists.addAll(0, Arrays.asList(2, 3, 4, 5));
```

上述代码内部的链表结构如下：

![image-20210330225517390](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330225517390.png)

**addAll()中的一个问题：**

在addAll函数中，传入一个集合参数和插入位置，然后将集合转化为数组，然后再遍历数组，挨个添加数组的元素，但是问题来了，为什么要先转化为数组再进行遍历，而不是直接遍历集合呢？

从效果上两者是完全等价的，都可以达到遍历的效果。关于为什么要转化为数组的问题，我的思考如 下：

1. 如果直接遍历集合的话，那么在遍历过程中需要插入元素，在堆上分配内存空间，修改指针域，这个过程中就会一直占用着这个集合，考虑正确同步的话，其他线程只能一直等待。
2. 如果转化为数组，只需要遍历集合，而遍历集合过程中不需要额外的操作，所以占用的时间相对是较短的，这样就利于其他线程尽快的使用这个集合。说白了，就是有利于提高多线程访问该集合的效率，尽可能短时间的阻塞。

#### remove(Object o)

```java
/**
 * Removes the first occurrence of the specified element from this list,
 * if it is present.  If this list does not contain the element, it is
 * unchanged.  More formally, removes the element with the lowest index
 * {@code i} such that
 * <tt>(o==null&nbsp;?&nbsp;get(i)==null&nbsp;:&nbsp;o.equals(get(i)))</tt>
 * (if such an element exists).  Returns {@code true} if this list
 * contained the specified element (or equivalently, if this list
 * changed as a result of the call).
 *
 * @param o element to be removed from this list, if present
 * @return {@code true} if this list contained the specified element
 */

///首先通过看上面的注释，我们可以知道，如果我们要移除的值在链表中存在多个一样的值，那么我们会移除index最小的那个，也就是最先找到的那个值，如果不存在这个值，那么什么也不做。
public boolean remove(Object o) {
    //这里可以看到，linkedList也能存储null
    if (o == null) {
        //循环遍历链表，直到找到null值，然后使用unlink移除该值。下面的这个else中也一样
        for (Node<E> x = first; x != null; x = x.next) {
            if (x.item == null) {
                unlink(x);
                return true;
            }
        }
    } else {
        for (Node<E> x = first; x != null; x = x.next) {
            if (o.equals(x.item)) {
                unlink(x);
                return true;
            }
        }
    }
    return false;
}
```

【unlink(xxxx)】

```java
// Unlinks non-null node x.
//不能传一个null值过，注意，看之前要注意之前的next、prev这些都是谁。
E unlink(Node<E> x) {
    // assert x != null;
    //拿到节点x的三个属性
    final E element = x.item;
    final Node<E> next = x.next;
    final Node<E> prev = x.prev;
	
    //这里开始往下就进行移除该元素之后的操作，也就是把指向哪个节点搞定。
    if (prev == null) {
        //说明移除的节点是头节点，则first头节点应该指向下一个节点
        first = next;
    } else {
        //不是头节点，prev.next=next：有1、2、3，将1.next指向3
        prev.next = next;
        //然后解除x节点的前指向。
        x.prev = null;
    }

    if (next == null) {
        //说明移除的节点是尾节点
        last = prev;
    } else {
        //不是尾节点，有1、2、3，将3.prev指向1. 然后将2.next=解除指向。
        next.prev = prev;
        x.next = null;
    }

    //x的前后指向都为null了，也把item为null，让gc回收它
    x.item = null;
    size--;//移除一个节点，size自减
    modCount++;
    return element;//由于一开始已经保存了x的值到element，所以返回。
}
```

#### get(index)

【get(index)查询元素的方法】

```java
/**
    * Returns the element at the specified position in this list.
    *
    * @param index index of the element to return
    * @return the element at the specified position in this list
    * @throws IndexOutOfBoundsException {@inheritDoc}
*/
//这里没有什么，重点还是在node(index)中
public E get(int index) {
    checkElementIndex(index);
    return node(index).item;
}
```

【node(index)】

```java
/**
* Returns the (non-null) Node at the specified element index.
*/
//这里查询使用的是先从中间分一半查找
Node<E> node(int index) {
    // assert isElementIndex(index);
    //"<<":*2的几次方 “>>”:/2的几次方，例如：size<<1：size*2的1次方，
    //这个if中就是查询前半部分
    if (index < (size >> 1)) {//index<size/2
        Node<E> x = first;
        for (int i = 0; i < index; i++)
            x = x.next;
        return x;
    } else {//前半部分没找到，所以找后半部分
        Node<E> x = last;
        for (int i = size - 1; i > index; i--)
            x = x.prev;
        return x;
    }
}
```

#### indexOf(Object o)

```java
//这个很简单，就是通过实体元素来查找到该元素在链表中的位置。跟remove中的代码类似，只是返回类型不一样。
public int indexOf(Object o) {
    int index = 0;
    if (o == null) {
        for (Node<E> x = first; x != null; x = x.next) {
            if (x.item == null)
                return index;
            index++;
        }
    } else {
        for (Node<E> x = first; x != null; x = x.next) {
            if (o.equals(x.item))
                return index;
            index++;
        }
    }
    return -1;
}
```

### 7、LinkedList的迭代器

在LinkedList中除了有一个Node的内部类外，应该还能看到另外两个内部类，那就是ListItr，还有一个是DescendingIterator。

【ListItr内部类】

```java
private class ListItr implements ListIterator<E> {
}
```

看一下他的继承结构，发现只继承了一个ListIterator，到ListIterator中一看：

![image-20210330232202554](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330232202554.png)

看到方法名之后，就发现不止有向后迭代的方法，还有向前迭代的方法，所以我们就知道了这个ListItr 这个内部类干嘛用的了，就是能让linkedList不光能像后迭代，也能向前迭代。

看一下ListItr中的方法，可以发现，在迭代的过程中，还能移除、修改、添加值得操作。

![image-20210330232338517](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210330232338517.png)

【DescendingIterator内部类】

```java
private class DescendingIterator implements Iterator<E> {
    //看一下这个类，还是调用的ListItr，作用是封装一下Itr中几个方法，让使用者以正常的思维去写代码，例如，在从后往前遍历的时候，也是跟从前往后遍历一样，使用next等操作，而不用使用特殊的previous。
    private final ListItr itr = new ListItr(size());
    public boolean hasNext() {
        return itr.hasPrevious();
    }
    public E next() {
        return itr.previous();
    }
    public void remove() {
        itr.remove();
    }
}
```

## 总结

1.  linkedList本质上是一个双向链表，通过一个Node内部类实现的这种链表结构
2. 能存储null值
3. 跟arrayList相比较，就真正的知道了，LinkedList在删除和增加等操作上性能好，而ArrayList在查询的性能上好
4. . 从源码中看，它不存在容量不足的情况
5. . linkedList不光能够向前迭代，还能像后迭代，并且在迭代的过程中，可以修改值、添加值、还能移除值。
6. linkedList不光能当链表，还能当队列使用，这个就是因为实现了Deque接口。

代码在 `LinkedList源码分析`中`3、类的属性`

# Vevtor和Stack

前面写了一篇关于的是LinkedList的除了它的数据结构稍微有一点复杂之外，其他的都很好理解的。这 一篇说的大家在开发中很少去用到，有的时候也可能是会用到的，了解就行。

注意在学习这一篇之前，需要有多线程的知识：

**1）锁机制：对象锁、方法锁、类锁**

对象锁就是方法锁：就是在一个类中的方法上加上synchronized关键字，这就是给这个方法加锁了。

类锁：锁的是整个类，当有多个线程来声明这个类的对象的时候将会被阻塞，直到拥有这个类锁的对象被销毁或者主动释放了类锁。这个时候在被阻塞住的线程被挑选出一个占有该类锁，声明该类的对象。 其他线程继续被阻塞住。例如：在类A上有关键字synchronized，那么就是给类A加了类锁，线程1第一 个声明此类的实例，则线程1拿到了该类锁，线程2在想声明类A的对象，就会被阻塞。

2）在本文中，使用的是方法锁。

3）每个对象只有一把锁，有线程A，线程B，还有一个集合C类，线程A操作C拿到了集合中的锁（在集合C中有用synchronized关键字修饰的），并且还没有执行完，那么线程A就不会释放锁，当轮到线程B去操作集合C中的方法时 ，发现锁被人拿走了，所以线程B只能等待那个拿到锁的线程使用完，然后才能拿到锁进行相应的操作。

### 1、Vector概述

![image-20210331092950219](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331092950219.png)



通过API中可以知道：

1. Vector是一个可变化长度的数组
2. Vector增加长度通过的是capacity和capacityIncrement这两个变量，目前还不知道如何实现自动 扩增的，等会源码分析
3.  Vector也可以获得iterator和listIterator这两个迭代器，并且他们发生的是fail-fast，而不是failsafe，注意这里，不要觉得这个vector是线程安全就搞错了，具体分析在下面会说
4.  Vector是一个线程安全的类，如果使用需要线程安全就使用Vector，如果不需要，就使用arrayList
5. Vector和ArrayList很类似，就少许的不一样，从它继承的类和实现的接口来看，跟arrayList一模一 样。

注意：java1.5推出的java.uitl.concurrent包，为了解决复杂的并发问题的。所以开发中，不建议用vector，原因在文章的结束会有解释，需要线程安全的集合类直接用java.util.concurrent包下的类。

### 2、Vector源码分析

```java
public class Vector<E>
    extends AbstractList<E>
    implements List<E>, RandomAccess, Cloneable, java.io.Serializable
    {
    
	}
```

我们发现Vector的继承关系和层次结构和ArrayList中的一模一样，忘记的可以去ArrayList标题查看！

#### 构造方法

一共有四个构造方法。

构造方法作用：

- 初始化存储元素的容器，也就是数组，elementData，
- 初始化capacityIncrement的大小，默认是0，这个的作用就是扩展数组的时候，增长的大小，为0 则每次扩展2倍

Vector()：空构造

```java
/**
 * Constructs an empty vector so that its internal data array
 * has size {@code 10} and its standard capacity increment is
 * zero.
 */
///看注释，这个是一个空的Vector构造方法，所以让他使用内置的数组，这里还不知道什么是内置的数组，看它调用了自身另外一个带一个参数的构造器
public Vector() {
    this(10);
}
```

Vector(int)

```java
/**
 * Constructs an empty vector with the specified initial capacity and
 * with its capacity increment equal to zero.
 *
 * @param   initialCapacity   the initial capacity of the vector
 * @throws IllegalArgumentException if the specified initial capacity
 *         is negative
 */
//注释说，给空的cector构造器用和带有一个特定初始化容量用的，并且又调用了另外一个带两个参数的构造器，并且给容量增长值(capacityIncrement=0)为0，查看vector中的变量可以发现capacityIncrement是一个成员变量

public Vector(int initialCapacity) {
    this(initialCapacity, 0);
}
```

ector(int，int)

```java
/**
 * Constructs an empty vector with the specified initial capacity and
 * capacity increment.
 *
 * @param   initialCapacity     the initial capacity of the vector
 * @param   capacityIncrement   the amount by which the capacity is
 *                              increased when the vector overflows
 * @throws IllegalArgumentException if the specified initial capacity
 *         is negative
 */
//构建一个有特定的初始化容量和容量增长值的空的Vector，
public Vector(int initialCapacity, int capacityIncrement) {
    super();//调用父类的构造，是个空构造
    if (initialCapacity < 0)//小于0，会报非法参数异常：不合法的容量
        throw new IllegalArgumentException("Illegal Capacity: "+
                                           initialCapacity);
    this.elementData = new Object[initialCapacity];//elementData是一个成员变量数组，初始化它，并给它初始化长度。默认就是10，除非自己给值。
    this.capacityIncrement = capacityIncrement;//capacityIncrement的意思是如果要扩增数组，每次增长该值，如果该值为0，那数组就变为两倍的原长度，这个之后会分析到
}
```

Vector(Collection c)

```java
/**
 * Constructs a vector containing the elements of the specified
 * collection, in the order they are returned by the collection's
 * iterator.
 *
 * @param c the collection whose elements are to be placed into this
 *       vector
 * @throws NullPointerException if the specified collection is null
 * @since   1.2
 */
//将集合c变为Vector，返回Vector的迭代器。
public Vector(Collection<? extends E> c) {
    elementData = c.toArray();
    elementCount = elementData.length;
    // c.toArray might (incorrectly) not return Object[] (see 6260652)
    if (elementData.getClass() != Object[].class)
        elementData = Arrays.copyOf(elementData, elementCount, Object[].class);
}
```

#### 核心方法

add()方法

```java
/**
 * Appends the specified element to the end of this Vector.
 *
 * @param e element to be appended to this Vector
 * @return {@code true} (as specified by {@link Collection#add})
 * @since 1.2
 */

//就是在vector中的末尾追加元素。但是看方法，synchronized，明白了为什么vector是线程安全的，因为在方法前面加了synchronized关键字，给该方法加锁了，哪个线程先调用它，其它线程就得等着，如果不清楚的就去看看多线程的知识，到后面我也会一一总结的。
public synchronized boolean add(E e) {
    modCount++;
    //通过arrayList的源码分析经验，这个方法应该是在增加元素前，检查容量是否够用
    ensureCapacityHelper(elementCount + 1);
    elementData[elementCount++] = e;
    return true;
}
```

ensureCapacityHelper(int)

```java
/**
 * This implements the unsynchronized semantics of ensureCapacity.
 * Synchronized methods in this class can internally call this
 * method for ensuring capacity without incurring the cost of an
 * extra synchronization.
 *
 * @see #ensureCapacity(int)
 */
////这里注释解释，这个方法是异步(也就是能被多个线程同时访问)的，原因是为了让同步方法都能调用到这个检测容量的方法，比如add的同时，另一个线程调用了add的重载方法，那么两个都需要同时查询容量够不够，所以这个就不需要用synchronized修饰了。因为不会发生线程不安全的问题
private void ensureCapacityHelper(int minCapacity) {
    // overflow-conscious code
    if (minCapacity - elementData.length > 0)
        //容量不够，就扩增，核心方法
        grow(minCapacity);
}
```

grow(int)

```java
//看一下这个方法，其实跟arrayList一样，唯一的不同就是在扩增数组的方式不一样，如果capacityIncrement不为0，那么增长的长度就是capacityIncrement，如果为0，那么扩增为2倍的原容量
    
private void grow(int minCapacity) {
    // overflow-conscious code
    int oldCapacity = elementData.length;
    int newCapacity = oldCapacity + ((capacityIncrement > 0) ?
                                     capacityIncrement : oldCapacity);
    if (newCapacity - minCapacity < 0)
        newCapacity = minCapacity;
    if (newCapacity - MAX_ARRAY_SIZE > 0)
        newCapacity = hugeCapacity(minCapacity);
    elementData = Arrays.copyOf(elementData, newCapacity);
}
```

只要能看的懂ArrayList，这个就是在每个方法上比arrayList多了一个synchronized，其他都一 样。这里就不再分析了！

```java
public synchronized E get(int index) {
    if (index >= elementCount)
    	throw new ArrayIndexOutOfBoundsException(index);
    
    return elementData(index);
}
```

### 3、Stack

现在来看看Vector的子类Stack，学过数据结构都知道，这个就是栈的意思。那么该类就是跟栈的用法一 样了

```java
class Stack<E> extends Vector<E> {}
```

通过查看他的方法，和查看api文档，很容易就能知道他的特性。就几个操作，出栈，入栈等，构造方法也是空的，用的还是数组，父类中的构造，跟父类一样的扩增方式，并且它的方法也是同步的，所以也是线程安全。

![image-20210331133023382](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331133023382.png)

### 4、总结Vector和Stack

【Vector总结（通过源码分析）】

1. Vector线程安全是因为它的方法都加了synchronized关键字
2. Vector的本质是一个数组，特点能是能够自动扩增，扩增的方式跟capacityIncrement的值有关
3. 它也会fail-fast，还有一个fail-safe两个的区别在下面的list总结中会讲到。

【Stack的总结】

1. 对栈的一些操作，先进后出
2. 底层也是用数组实现的，因为继承了Vector
3. 也是线程安全的

# List总结

**arrayList和LinkedList区别**

		arrayList底层是用数组实现的顺序表，是随机存取类型，可自动扩增，并且在初始化时，数组的长度是0，只有在增加元素时，长度才会增加。默认是10，不能无限扩增，有上限，在查询操作的时候性能更好
	
		LinkedList底层是用链表来实现的，是一个双向链表，注意这里不是双向循环链表，顺序存取类型。 在源码中，似乎没有元素个数的限制。应该能无限增加下去，直到内存满了在进行删除，增加操作时性能更好。

两个都是线程不安全的，在iterator时，会发生fail-fast：快速失效。



**arrayList和Vector的区别**

		arrayList线程不安全，在用iterator，会发生fail-fast
	
		Vector线程安全，因为在方法前加了Synchronized关键字。也会发生fail-fast



**fail-fast和fail-safe区别和什么情况下会发生**

		简单的来说：在java.util下的集合都是发生fail-fast，而在java.util.concurrent下的发生的都是failsafe。
	
		1）fail-fast

快速失败，例如在arrayList中使用迭代器遍历时，有另外的线程对arrayList的存储数组进行了改变，比如add、delete、等使之发生了结构上的改变，所以Iterator就会快速报一个 java.util.ConcurrentModificationException 异常（并发修改异常），这就是快速失败。

		2）fail-safe

安全失败，在java.util.concurrent下的类，都是线程安全的类，他们在迭代的过程中，如果有线程进行结构的改变，不会报异常，而是正常遍历，这就是安全失败。

		3）为什么在java.util.concurrent包下对集合有结构的改变，却不会报异常？

在concurrent下的集合类增加元素的时候使用Arrays.copyOf()来拷贝副本，在副本上增加元素，如果有其他线程在此改变了集合的结构，那也是在副本上的改变，而不是影响到原集合，迭代器还是照常遍 历，遍历完之后，改变原引用指向副本，所以总的一句话就是如果在此包下的类进行增加删除，就会出现一个副本。所以能防止fail-fast，这种机制并不会出错，所以我们叫这种现象为fail-safe。

		4）vector也是线程安全的，为什么是fail-fast呢？

这里搞清楚一个问题，并不是说线程安全的集合就不会报fail-fast，而是报fail-safe，你得搞清楚前面所说答案的原理，出现fail-safe是因为他们在实现增删的底层机制不一样，就像上面说的，会有一个副本，而像arrayList、linekdList、verctor等，他们底层就是对着真正的引用进行操作，所以才会发生异常。

		5）既然是线程安全的，为什么在迭代的时候，还会有别的线程来改变其集合的结构呢(也就是对其删除和增加等操作)？

首先，我们迭代的时候，根本就没用到集合中的删除、增加，查询的操作，就拿vector来说，我们都没有用那些加锁的方法，也就是方法锁放在那没人拿，在迭代的过程中，有人拿了那把锁，我们也没有办法，因为那把锁就放在那边。



【举例说明fail-fast和fail-safe的区别】

- fail-fast

![image-20210331135807175](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331135807175.png)

- fail-safe

通过CopyOnWriteArrayList这个类来做实验，不用管这个类的作用，但是他确实没有报异常， 并且还通过第二次打印，来验证了上面我们说创建了副本的事情。

原理是在添加操作时会创建副本，在副本上进行添加操作，等迭代器遍历结束后，会将原引用 改为副本引用，所以我们在创建了一个list的迭代器，结果打印的就是123444了，

证明了确实改变成为了副本引用，后面为什么是三个4，原因是我们循环了3次，不就添加了3 个4吗。如果还感觉不爽的话，看下add的源码。

![image-20210331151011751](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331151011751.png)

![image-20210331151024361](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331151024361.png)

【为什么现在都不提倡使用vector了】

1）vector实现线程安全的方法是在每个操作方法上加锁，这些锁并不是必须要的，在实际开发中， 一般都是通过锁一系列的操作来实现线程安全，也就是说将需要同步的资源放一起加锁来保证线程安全。

2）如果多个Thread并发执行一个已经加锁的方法，但是在该方法中，又有vector的存在，vector本身实现中已经加锁了，那么相当于锁上又加锁，会造成额外的开销。

3）就如上面第三个问题所说的，vector还有fail-fast的问题，也就是说它也无法保证遍历安全，在遍历时又得额外加锁，又是额外的开销，还不如直接用arrayList，然后再加锁呢。

总结：Vector在你不需要进行线程安全的时候，也会给你加锁，也就导致了额外开销，所以在 jdk1.5之后就被弃用了，现在如果要用到线程安全的集合，都是从java.util.concurrent包下去拿相应的类。

# HashMap

### HashMap引入

问题：建立学生学号和学生姓名间的键值映射，并通过key对value进行操作，应该如何实现数据的存储和操作呢？

 Map接口专门处理键值映射数据的存储，可以根据键实现对值的操作。 最常用的实现类是HashMap。

```java
public static void main(String[] args) {
    Map<String,String> map = new HashMap<String,String>();
    map.put("004","李清照");
    map.put("001","李白");
    map.put("003","王羲之");
    map.put("002","杜甫");

    System.out.println(map.get("003"));

    //获取所有key 值
    Set<String> keySet = map.keySet();
    for (String s : keySet){
        String s1 = map.get(s);
        System.out.println(s+"    "+s1);
    }

    //获取所有值
    Collection<String> values = map.values();
    for (String s : values){
        System.out.println(s);
    }
    
    //entrySet() 获取值
    Set<Map.Entry<String, String>> entrySet = map.entrySet();
    for (Map.Entry<String, String> m : entrySet){
        String key = m.getKey();
        String value = m.getValue();
        System.out.println(key+","+value);
    }
}
```

### HashMa数据结构

HashMap是基于哈希表的Map接口实现的，它存储的是内容是键值对映射。此类不保证映 射的顺序，假定哈希函数将元素适当的分布在各桶之间，可为基本操作(get和put)提供稳定的性能。

在API中给出了相应的定义：

又到了最激动人心的源码分析环节**:smile:**

![image-20210331153042083](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331153042083.png)

	第一段：

哈希表基于map接口的实现，这个实现提供了map所有的操作，并且提供了key和value，可以为 null，(HashMap和HashTable大致上是一样的，除了hashmap是异步的，和允许key和value为 null)

这个类不确定map中元素的位置，特别要提的是，这个类也不确定元素的位置随着时间会不会保持不变。

	第二段：

假设哈希函数将元素合适的分到了每个桶（其实就是指的数组中位置上的链表）中，则这个实现为基本的操作(get、put)提供了稳定的性能，迭代这个集合视图需要的时间跟hashMap实例（key-value映射的数量）的容量（在桶中）成正比，因此，如果迭代的性能很重要的话，就不要将初始容量设置的太高或者 loadfactor设置的太低，【这里的桶，相当于在数组中每个位置上放一个桶装元素】

	第三段：

HashMap的实例有两个参数影响性能，初始化容量（initialCapacity）和loadFactor加载因子， 在哈希表中这个容量是桶的数量【也就是数组的长度】，一个初始化容量仅仅是在哈希表被创建时容量， 在容量自动增长之前加载因子是衡量哈希表被允许达到的多少的。当entry的数量在哈希表中超过了加载 因子乘以当前的容量，那么哈希表被修改（内部的数据结构会被重新建立）所以哈希表有大约两倍的桶的数量.

	第四段：

通常来讲，默认的加载因子(0.75)能够在时间和空间上提供一个好的平衡，更高的值会减少空间上的开支但是会增加查询花费的时间（体现在HashMap类中get、put方法上），当设置初始化容量时，应该考虑到map中会存放entry的数量和加载因子，以便最少次数的进行rehash操作，如果初始容量大于最大条目数除以加载因子，则不会发生 rehash 操作。

	第五段：

如果很多映射关系要存储在 HashMap 实例中，则相对于按需执行自动的 rehash 操作以增大表的 容量来说，使用足够大的初始容量创建它将使得映射关系能更有效地存储。

#### HashMap在JDK1.8以前数据结构和存储原理

【链表散列】

首先我们要知道什么是链表散列？通过数组和链表结合在一起使用，就叫做链表散列。这其实就是 hashmap存储的原理图。

![image-20210331153544575](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331153544575.png)

【HashMap的数据结构和存储原理】

HashMap的数据结构就是用的链表散列。那HashMap底层是怎么样使用这个数据结构进行数据存取的呢？分成两个部分：

第一步：HashMap内部有一个entry的内部类，其中有四个属性，我们要存储一个值，则需要一个key 和一个value，存到map中就会先将key和value保存在这个Entry类创建的对象中。

```java
static class Entry<K,V> implements Map.Entry<K,V> {
    final K key; //就是我们说的map的key
    V value; //value值，这两个都不陌生
    Entry<K,V> next;//指向下一个entry对象
    int hash;//通过key算过来的你hashcode值。
}
```

Entry的物理模型图：

![image-20210331154056812](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331154056812.png)

第二步：构造好了entry对象，然后将该对象放入数组中，如何存放就是这hashMap的精华所在了。

大概的一个存放过程是：通过entry对象中的hash值来确定将该对象存放在数组中的哪个位置上，如果在这个位置上还有其他元素，则通过链表来存储这个元素。

![image-20210331154430064](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331154430064.png)

【Hash存放元素的过程】

通过key、value封装成一个entry对象，然后通过key的值来计算该entry的hash值，通过entry的hash值和数组的长度length来计算出entry放在数组中的哪个位置上面，

每次存放都是将entry放在第一个位置。在这个过程中，就是通过hash值来确定将该对象存放在数组中 的哪个位置上。

#### JDK1.8后HashMap的数据结构

![image-20210331160154030](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331160154030.png)

上图很形象的展示了HashMap的数据结构（数组+链表+红黑树），桶中的结构可能是链表，也可能是红黑树，红黑树的引入是为了提高效率。

![hashMap内存结构图](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/20181227162958496)

### HashMap的属性

HashMap的实例有两个参数影响其性能。

初始容量：哈希表中桶的数量

加载因子：哈希表在其容量自动增加之前可以达到多满，的一种尺度

当哈希表中条目数超出了当前容量*加载因子(其实就是HashMap的实际容量)时，则对该哈希表进行 rehash操作，将哈希表扩充至两倍的桶数。

Java中默认初始容量为16，加载因子为0.75。

```java
static final int DEFAULT_INITIAL_CAPACITY = 1 << 4; // aka 16
static final float DEFAULT_LOAD_FACTOR = 0.75f;
```

【loadFactor加载因子】

定义：loadFactor译为装载因子。装载因子用来衡量HashMap满的程度。loadFactor的默认值为 0.75f。计算HashMap的实时装载因子的方法为：size/capacity，而不是占用桶的数量去除以capacity。

 loadFactor加载因子是控制数组存放数据的疏密程度，loadFactor越趋近于1，那么数组中存放的数据 (entry)也就越多，也就越密，也就是会让链表的长度增加，loadFactor越小，也就是趋近于0，那么数组中存放的数据也就越稀，也就是可能数组中每个位置上就放一个元素。

那有人说，就把loadFactor变为1最好吗，存的数据很多，但是这样会有一个问题，就是我们在通过key拿到我们的value时，是先通过key的hashcode值，找到对应数组中的位置，如果该位置中有很多元素，则需要通过equals来依次比较链表中的元素，拿到我们的value值，这样花费的性能就很高，如果能让数组上的每个位置尽量只有一个元素最好，我们就能直接得到value值了，所以有人又会说，那把loadFactor变得很小不就好了，但是如果变得太小，在数组中的位置就会太稀，也就是分散的太开，浪费很多空间，这样也不好，所以在hashMap 中loadFactor的初始值就是0.75，一般情况下不需要更改它。

```java
static final float DEFAULT_LOAD_FACTOR = 0.75f;
```

【桶】

根据前面画的HashMap存储的数据结构图，你这样想，数组中每一个位置上都放有一个桶，每个桶里 就是装一个链表，链表中可以有很多个元素(entry)，这就是桶的意思。也就相当于把元素都放在桶中。

【capacity】

capacity译为容量代表的数组的容量，也就是数组的长度，同时也是HashMap中桶的个数。默认值是 16。

一般第一次扩容时会扩容到64，之后好像是2倍。总之，容量都是2的幂。

```java
static final int DEFAULT_INITIAL_CAPACITY = 1 << 4; // aka 16
```

【size的含义】

 size就是在该HashMap的实例中实际存储的元素的个数

【threshold的作用】

```java
int threshold;
```

 threshold = capacity * loadFactor，当Size>=threshold的时候，那么就要考虑对数组的扩增了，也就是说，这个的意思就是衡量数组是否需要扩增的一个标准。

注意这里说的是考虑，因为实际上要扩增数组，除了这个size>=threshold条件外，还需要另外一个条 件。

什么时候会扩增数组的大小？在put一个元素时先size>=threshold并且还要在对应数组位置上有元素， 这才能扩增数组。

我们通过一张HashMap的数据结构图来分析：

![image-20210331160910195](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331160910195.png)

### HashMap的源码分析

#### 1、HashMap的层次关系与继承结构

【HashMap继承结构】

![image-20210331161138894](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331161138894.png)

上面就继承了一个abstractMap，也就是用来减轻实现Map接口的编写负担。

【实现接口】

```java
public class HashMap<K,V> extends AbstractMap<K,V>
implements Map<K,V>, Cloneable, Serializable {
    
}
```

Map<K,V>：在AbstractMap抽象类中已经实现过的接口，这里又实现，实际上是多余的。但每个集合都有这样的错误，也没过大影响

 Cloneable：能够使用Clone()方法，在HashMap中，实现的是浅层次拷贝，即对拷贝对象的改变会影响 被拷贝的对象。

 Serializable：能够使之序列化，即可以将HashMap对象保存至本地，之后可以恢复状态。



#### 2、HashMap类的属性

```java
public class HashMap<K,V> extends AbstractMap<K,V> implements Map<K,V>,Cloneable, Serializable {
    // 序列号
    private static final long serialVersionUID = 362498820763181265L;
    // 默认的初始容量是16
    static final int DEFAULT_INITIAL_CAPACITY = 1 << 4;
    // 最大容量
    static final int MAXIMUM_CAPACITY = 1 << 30;
    // 默认的填充因子
    static final float DEFAULT_LOAD_FACTOR = 0.75f;
    // 当桶(bucket)上的结点数大于这个值时会转成红黑树
    static final int TREEIFY_THRESHOLD = 8;
    // 当桶(bucket)上的结点数小于这个值时树转链表
    static final int UNTREEIFY_THRESHOLD = 6;
    // 桶中结构转化为红黑树对应的table的最小大小
    static final int MIN_TREEIFY_CAPACITY = 64;
    // 存储元素的数组，总是2的幂次倍
    transient Node<k,v>[] table;
    // 存放具体元素的集
    transient Set<map.entry<k,v>> entrySet;
    // 存放元素的个数，注意这个不等于数组的长度。
    transient int size;
    // 每次扩容和更改map结构的计数器
    transient int modCount;
    // 临界值 当实际大小(容量*填充因子)超过临界值时，会进行扩容
    int threshold;
    // 填充因子
    final float loadFactor;
}
```

#### 3、HashMap的构造方法

有四个构造方法，构造方法的作用就是记录一下16这个数给threshold（这个数值最终会当作第一次组的长度。）和初始化加载因子。注意，hashMap中table数组一开始就已经是个没有长度的数组了。

构造方法中，并没有初始化数组的大小，数组在一开始就已经被创建了，构造方法只做两件事情，一个 是初始化加载因子，另一个是用threshold记录下数组初始化的大小。注意是记录。

【HashMap()】

```java
//看上面的注释就已经知道，DEFAULT_INITIAL_CAPACITY=16，DEFAULT_LOAD_FACTOR=0.75
//初始化容量：也就是初始化数组的大小
//加载因子：数组上的存放数据疏密程度。

public HashMap() {
	this(DEFAULT_INITIAL_CAPACITY, DEFAULT_LOAD_FACTOR);
}
```

【HashMap(int)】

```java
public HashMap(int initialCapacity) {
	this(initialCapacity, DEFAULT_LOAD_FACTOR);
}
```

【HashMap(int,float)】

```java
public HashMap(int initialCapacity, float loadFactor) {
    // 初始容量不能小于0，否则报错
    if (initialCapacity < 0)
    throw new IllegalArgumentException("Illegal initial capacity: " +
    										initialCapacity);
    // 初始容量不能大于最大值，否则为最大值
    if (initialCapacity > MAXIMUM_CAPACITY)
    initialCapacity = MAXIMUM_CAPACITY;
    // 填充因子不能小于或等于0，不能为非数字
    if (loadFactor <= 0 || Float.isNaN(loadFactor))
    throw new IllegalArgumentException("Illegal load factor: " +
    										loadFactor);
    // 初始化填充因子
    this.loadFactor = loadFactor;
    // 初始化threshold大小
    this.threshold = tableSizeFor(initialCapacity);
}

```

【HashMap(Map<? extends K, ? extends V> m) 】

```java
public HashMap(Map<? extends K, ? extends V> m) {
    // 初始化填充因子
    this.loadFactor = DEFAULT_LOAD_FACTOR;
    // 将m中的所有元素添加至HashMap中
    putMapEntries(m, false);
}
```

【putMapEntries(Map<? extends K, ? extends V> m, boolean evict)函数将m的所有元素存入本
HashMap实例中】

```java

    /**
     * Implements Map.putAll and Map constructor.
     *
     * @param m the map
     * @param evict false when initially constructing this map, else
     * true (relayed to method afterNodeInsertion).
     */
    final void putMapEntries(Map<? extends K, ? extends V> m, boolean evict) {
        int s = m.size();
        if (s > 0) {
            // 判断table是否已经初始化
            if (table == null) { // pre-size
                // 未初始化，s为m的实际元素个数
                float ft = ((float)s / loadFactor) + 1.0F;
                int t = ((ft < (float)MAXIMUM_CAPACITY) ?
                         (int)ft : MAXIMUM_CAPACITY);
                // 计算得到的t大于阈值，则初始化阈值
                if (t > threshold)
                    threshold = tableSizeFor(t);
            }
            // 已初始化，并且m元素个数大于阈值，进行扩容处理
            else if (s > threshold)
                resize();
            // 将m中的所有元素添加至HashMap中
            for (Map.Entry<? extends K, ? extends V> e : m.entrySet()) {
                K key = e.getKey();
                V value = e.getValue();
                putVal(hash(key), key, value, false, evict);
            }
        }
    }
```

#### 4、HashMap常用方法

【put(K key, V value)】

```java
public V put(K key, V value) {
return putVal(hash(key), key, value, false, true);
}
```

【putVal(int hash, K key, V value, boolean onlyIfAbsent,boolean evict)】

```java
final V putVal(int hash, K key, V value, boolean onlyIfAbsent,
               boolean evict) {
    Node<K,V>[] tab; Node<K,V> p; int n, i;
    // table未初始化或者长度为0，进行扩容
    if ((tab = table) == null || (n = tab.length) == 0)
        n = (tab = resize()).length;
    // (n - 1) & hash 确定元素存放在哪个桶中，桶为空，新生成结点放入桶中(此时，这个结点是放在数组中)
    if ((p = tab[i = (n - 1) & hash]) == null)
        tab[i] = newNode(hash, key, value, null);
    // 桶中已经存在元素
    else {
        Node<K,V> e; K k;
        // 比较桶中第一个元素(数组中的结点)的hash值相等，key相等
        if (p.hash == hash &&
            ((k = p.key) == key || (key != null && key.equals(k))))
            // 将第一个元素赋值给e，用e来记录
            e = p;
        // hash值不相等，即key不相等；为红黑树结点
        else if (p instanceof TreeNode)
            // 放入树中
            e = ((TreeNode<K,V>)p).putTreeVal(this, tab, hash, key, value);
        // 为链表结点
        else {
            // 在链表最末插入结点
            for (int binCount = 0; ; ++binCount) {
                // 到达链表的尾部
                if ((e = p.next) == null) {
                    // 在尾部插入新结点
                    p.next = newNode(hash, key, value, null);
                    // 结点数量达到阈值，转化为红黑树
                    if (binCount >= TREEIFY_THRESHOLD - 1) // -1 for 1st
                        treeifyBin(tab, hash);
                    // 跳出循环
                    break;
                }
                // 判断链表中结点的key值与插入的元素的key值是否相等
                if (e.hash == hash &&
                    ((k = e.key) == key || (key != null && key.equals(k))))
                    // 相等，跳出循环
                    break;
                // 用于遍历桶中的链表，与前面的e = p.next组合，可以遍历链表
                p = e;
            }
        }
        // 表示在桶中找到key值、hash值与插入元素相等的结点
        if (e != null) { // existing mapping for key
            // 记录e的value
            V oldValue = e.value;
            // onlyIfAbsent为false或者旧值为null
            if (!onlyIfAbsent || oldValue == null)
                //用新值替换旧值
                e.value = value;
            // 访问后回调
            afterNodeAccess(e);
            // 返回旧值
            return oldValue;
        }
    }
    // 结构性修改
    ++modCount;
    // 实际大小大于阈值则扩容
    if (++size > threshold)
        resize();
    // 插入后回调
    afterNodeInsertion(evict);
    return null;
}
```

HashMap并没有直接提供putVal接口给用户调用，而是提供的put函数，而put函数就是通过putVal来插入元素的。

【get(Object key)】

```java
public V get(Object key) {
    Node<K,V> e;
    return (e = getNode(hash(key), key)) == null ? null : e.value;
}
```

【getNode(int hash,Pbject key)】

```java
final Node<K,V> getNode(int hash, Object key) {
    Node<K,V>[] tab; Node<K,V> first, e; int n; K k;
    // table已经初始化，长度大于0，根据hash寻找table中的项也不为空
    if ((tab = table) != null && (n = tab.length) > 0 &&
        (first = tab[(n - 1) & hash]) != null) {
        // 桶中第一项(数组元素)相等
        if (first.hash == hash && // always check first node
            ((k = first.key) == key || (key != null && key.equals(k))))
            return first;
        // 桶中不止一个结点
        if ((e = first.next) != null) {
            // 为红黑树结点
            if (first instanceof TreeNode)
                // 在红黑树中查找
                return ((TreeNode<K,V>)first).getTreeNode(hash, key);
            // 否则，在链表中查找
            do {
                if (e.hash == hash &&
                    ((k = e.key) == key || (key != null && key.equals(k))))
                    return e;
            } while ((e = e.next) != null);
        }
    }
    return null;
}
```

 HashMap并没有直接提供getNode接口给用户调用，而是提供的get函数，而get函数就是通过 getNode来取得元素的。



【resize方法】

```java
final Node<K,V>[] resize() {
    // 当前table保存
    Node<K,V>[] oldTab = table;
    // 保存table大小
    int oldCap = (oldTab == null) ? 0 : oldTab.length;
    // 保存当前阈值
    int oldThr = threshold;
    int newCap, newThr = 0;
    // 之前table大小大于0
    if (oldCap > 0) {
        // 之前table大于最大容量
        if (oldCap >= MAXIMUM_CAPACITY) {
            // 阈值为最大整形
            threshold = Integer.MAX_VALUE;
            return oldTab;
        }
        // 容量翻倍，使用左移，效率更高
        else if ((newCap = oldCap << 1) < MAXIMUM_CAPACITY &&
                 oldCap >= DEFAULT_INITIAL_CAPACITY)
            // 阈值翻倍
            newThr = oldThr << 1; // double threshold
    }
    // 之前阈值大于0
    else if (oldThr > 0) // initial capacity was placed in threshold
        newCap = oldThr;
    // oldCap = 0并且oldThr = 0，使用缺省值（如使用HashMap()构造函数，之后再插入一个元素会调用resize函数，会进入这一步）
    else {               // zero initial threshold signifies using defaults
        newCap = DEFAULT_INITIAL_CAPACITY;
        newThr = (int)(DEFAULT_LOAD_FACTOR * DEFAULT_INITIAL_CAPACITY);
    }
    // 新阈值为0
    if (newThr == 0) {
        float ft = (float)newCap * loadFactor;
        newThr = (newCap < MAXIMUM_CAPACITY && ft < (float)MAXIMUM_CAPACITY ?
                  (int)ft : Integer.MAX_VALUE);
    }
    threshold = newThr;
    @SuppressWarnings({"rawtypes","unchecked"})
    // 初始化table
    Node<K,V>[] newTab = (Node<K,V>[])new Node[newCap];
    table = newTab;
    // 之前的table已经初始化过
    if (oldTab != null) {
        // 复制元素，重新进行hash
        for (int j = 0; j < oldCap; ++j) {
            Node<K,V> e;
            if ((e = oldTab[j]) != null) {
                oldTab[j] = null;
                if (e.next == null)
                    newTab[e.hash & (newCap - 1)] = e;
                else if (e instanceof TreeNode)
                    ((TreeNode<K,V>)e).split(this, newTab, j, oldCap);
                else { // preserve order
                    Node<K,V> loHead = null, loTail = null;
                    Node<K,V> hiHead = null, hiTail = null;
                    Node<K,V> next;
                    // 将同一桶中的元素根据(e.hash & oldCap)是否为0进行分割，分成两个不同的链表，完成rehash
                    do {
                        next = e.next;
                        if ((e.hash & oldCap) == 0) {
                            if (loTail == null)
                                loHead = e;
                            else
                                loTail.next = e;
                            loTail = e;
                        }
                        else {
                            if (hiTail == null)
                                hiHead = e;
                            else
                                hiTail.next = e;
                            hiTail = e;
                        }
                    } while ((e = next) != null);
                    if (loTail != null) {
                        loTail.next = null;
                        newTab[j] = loHead;
                    }
                    if (hiTail != null) {
                        hiTail.next = null;
                        newTab[j + oldCap] = hiHead;
                    }
                }
            }
        }
    }
    return newTab;
}
```

进行扩容，会伴随着一次重新hash分配，并且会遍历hash表中所有的元素，是非常耗时的。在编写程序中，要尽量避免resize。

在resize前和resize后的元素布局如下:

![image-20210331163600275](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331163600275.png)

上图只是针对了数组下标为2的桶中的各个元素在扩容后的分配布局，其他各个桶中的元素布局可以以此类推。

#### 5、总结

【关于数组扩容】

从putVal源代码中我们可以知道，当插入一个元素的时候size就加1，若size大于threshold的时候，就会进行扩容。假设我们的capacity大小为32，loadFator为0.75，则threshold为24 = 32 * 0.75，

此时，插入了25个元素，并且插入的这25个元素都在同一个桶中，桶中的数据结构为红黑树，则还 有31个桶是空的，也会进行扩容处理，其实，此时，还有31个桶是空的，好像似乎不需要进行扩容处 理，但是是需要扩容处理的，因为此时我们的capacity大小可能不适当。我们前面知道，扩容处理会遍 历所有的元素，时间复杂度很高；前面我们还知道，经过一次扩容处理后，元素会更加均匀的分布在各 个桶中，会提升访问效率。所以，说尽量避免进行扩容处理，也就意味着，遍历元素所带来的坏处大于 元素在桶中均匀分布所带来的好处。

【总结】

1. 要知道hashMap在JDK1.8以前是一个链表散列这样一个数据结构，而在JDK1.8以后是一个数组加 链表加红黑树的数据结构。
2. 通过源码的学习，hashMap是一个能快速通过key获取到value值得一个集合，原因是内部使用的 是hash查找值得方法。

# Set

Set注重独一无二的性质，该体系集合可以知道某物是否已经存在于集合中，不会存储重复的元素，用于存储无序**（存入和取出的顺序不一定相同）**元素，值不能重复

对象的相等性：
引用到堆上同一个对象的两个引用是相等的。如果对两个引用调用hashcode方法，会得到相同的结果，如果对象所属的类没有覆盖object的hashcode方法的话，hashcode会返回每个对象特有的序号（java是依据对象的内存地址计算出的此序号），所以两个不同的对象的hashcode值是不可能相等的。

如果想要让两个不同的Person对象视为相等的，就必须覆盖Object继承下来的hashcode方法和equals方法，因为Object hashcode返回的是该对象的内存地址，所以必须重写hashcode方法，才能保证两个不同的对象具有相同的hashcode，同时也需要两个不同对象比较equals方法返回true。

该集合中没有特有的方法，直接继承自Collection

```java
/**
 * Collection
 *      \--List
 *          有序（存储顺序和取出顺序一致），可重复
 *      \--Set
 *          无序（存储顺序和取出顺序不一致），唯一
 * HashSet:它不保证set的迭代顺序；特别是它不保证该顺序恒久不变
 * 注意：虽然set集合的元素无序，但是，作为集合来说，它肯定有它自己的存储顺序，
 * 而你的顺序恰巧和它的存储顺序一致，这代表不了有序，你可以多存储一些数据就能看到效果
 **/
```

案例：set集合添加元素并使用增强for循环遍历

```java
public static void method1() {
    Set<String> set = new HashSet<>();
    set.add("1");
    set.add("5");
    set.add("2");

    set.add("5");//重复的不会添加进去
    for (String s : set) {
        System.out.println(s);
    }
}
```

最后输出顺序是： 1、2、5

# HashSet

HashSet是一个没有重复元素的集合，它其实是由HashMap实现的，HashMap保存的是建值对，然而我们只能向HashSet中添加Key，原因在于HashSet的Value其实都是同一个对象，这是HashSet添加元素的方法，可以看到辅助实现HashSet的map中的value其实都是Object类的同一个对象。

特点：

- 底层数据结构是哈希表
- 对集合的迭代顺序不作任何保证，也就是说不保证存储和取出的元素顺序一致
- 没有带索引的方法，所以不能使用普通for循环遍历
- 由于是Set集合，所以是不包含重复元素的集合



### 存储规则

**哈希表边存放的是哈希值。**HashSet存储元素的顺序并不是按照存入时的顺序（和List显然不同） 是按照哈希值来存的所以取数据也是按照哈希值取得。

HashSet不存入重复元素的规则.使用hashcode和equals

由于Set集合是不能存入重复元素的集合。那么HashSet也是具备这一特性的。HashSet如何检查重复？HashSet会通过元素的hashcode（）和equals方法进行判断元素师否重复。

当你试图把对象加入HashSet时，HashSet会使用对象的hashCode来判断对象加入的位置。同时也会与其他已经加入的对象的hashCode进行比较，如果没有相等的hashCode，HashSet就会假设对象没有重复出现。

简单一句话，如果对象的hashCode值是不同的，那么HashSet会认为对象是不可能相等的。

因此我们自定义类的时候需要重写hashCode，来确保对象具有相同的hashCode值。

如果元素(对象)的hashCode值相同，是不是就无法存入HashSet中了？当然不是，会继续使用equals 进行比较。如果 equals为true 那么HashSet认为新加入的对象重复了，所以加入失败。如果equals 为false那么HashSet 认为新加入的对象没有重复，新元素可以存入。

**总结：**

元素的哈希值是通过元素的hashcode方法来获取的, HashSet首先判断两个元素的哈希值，如果哈希值一样，接着会比较equals方法 如果 equls结果为true ，HashSet就视为同一个元素。如果equals 为false就不是同一个元素。

哈希值相同equals为false的元素是怎么存储呢,就是在同样的哈希值下顺延（可以认为哈希值相同的元素放在一个哈希桶中）。也就是哈希一样的存一列。
![image-20210331235903905](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331235903905.png)

### HashSet用处

问题：现在有一批数据，要求不能重复存储元素，而且要排序。ArrayList 、 LinkedList不能去除重复数据。HashSet可以去除重复，但是是无序。

所以这时候就要使用TreeSet了

案例：创建一个学生类，并重写equals和hashcode

```java
import java.util.Objects;

public class HashSetStudent {
    public String name;
    public int age;

    public HashSetStudent(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        HashSetStudent that = (HashSetStudent) o;
        return age == that.age && Objects.equals(name, that.name);
    }

    @Override
    public int hashCode() {
        return Objects.hash(name, age);
    }
}
```

代码：

```java
public class HashSetTest {
    public static void main(String[] args) {
        HashSetStudent s1 = new HashSetStudent("李白1",15);
        HashSetStudent s2 = new HashSetStudent("李白2",16);

        HashSetStudent s3 = new HashSetStudent("李白1",15);//重复值不插入
        
        HashSetStudent s4 = new HashSetStudent("李白1",10);
        HashSetStudent s5 = new HashSetStudent("李白2",10);

        HashSet<HashSetStudent> hs = new HashSet<>();
        hs.add(s1);
        hs.add(s2);
        hs.add(s3);
        hs.add(s4);
        hs.add(s5);

        for(HashSetStudent S:hs){
            System.out.println(S.name+"--"+S.age);
        }

    }
}
```

最后输出：

> 李白2--10
> 李白1--10
> 李白1--15
> 李白2--16

### LinkedHashSet

特点：

- 哈希表和链表实现的Set接口，具有可预测的迭代次序
- 由链表保证元素有序，也就是说元素的存储和取出顺序是一致的
- 由哈希表保证元素唯一，也就是说没有重复的元素

待补充......

# TreeSet

**TreeSet简介**

红-黑树的数据结构，默认对元素进行自然排序

TreeSet 是一个有序的集合，它的作用是提供有序的Set集合。它继承于AbstractSet抽象类，实现了NavigableSet<E>, Cloneable, java.io.Serializable接口。

TreeSet 继承于AbstractSet，所以它是一个Set集合，具有Set的属性和方法。

TreeSet 实现了NavigableSet接口，意味着它支持一系列的导航方法。比如查找与指定目标最匹配项。

TreeSet 实现了Cloneable接口，意味着它能被克隆。

TreeSet 实现了java.io.Serializable接口，意味着它支持序列化。

TreeSet是基于TreeMap实现的。TreeSet中的元素支持2种排序方式：自然排序 或者 根据创建TreeSet 时提供的 Comparator 进行排序。这取决于使用的构造方法。

TreeSet为基本操作（add、remove 和 contains）提供受保证的 log(n) 时间开销。
另外，TreeSet是非同步的。 它的iterator 方法返回的迭代器是fail-fast的。

**特点：**

- 元素有序，这里的顺序不是指存储和取出的顺序，而是按照一定的规则进行排序，具体排序方式取决于构造方法

  TreeSet():根据其元素的自然非序进行排序

  TreeSet(Comparator comparator):根据指定的比较器进行排序

- 没有带索引的方法，所以不能使用普通for循环遍历

- 由于是Set集合，所以不包含重复元素的集合



### TreeSet自然顺序

即类要实现Comparable接口，并重写compareTo()方法，TreeSet对象调用add()方法时，会将存入的对象提升为Comparable类型，然后调用对象中的compareTo()方法进行比较，根据比较的返回值进行存储。

因为TreeSet底层是二叉树，当compareTo方法返回0时，不存储；当compareTo方法返回正数时，存入二叉树的右子树；当compareTo方法返回负数时，存入二叉树的左子树。如果一个类没有实现Comparable接口就将该类对象存入TreeSet集合，会发生类型转换异常。


### TreeSet自定义排序

方式一：元素自身具备比较性

元素自身具备比较性，需要元素实现Comparable接口，重写compareTo方法，也就是让元素自身具备比较性，这种方式叫做元素的自然排序也叫做默认排序。

**让元素自身具备比较性**



也就是元素需要实现Comparable接口，覆盖compareTo 方法。

案例：创建Student类，有姓名，年龄。存入集合后，先根据年龄大小，再根据姓名来进行排序插入集合中

```java
public class Student implements Comparable<Student> {
    public String name;
    public int age;

    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public int compareTo(Student o) {
        int i = this.age-o.age;
        int n = i==0?this.name.compareTo(o.name):i;
        return n;
    }
}
```

重写compareTo()方法，返回值有三种情况

1. 返回值为0：不插入集合
2. 返回值为1：往后插入集合
3. 返回值为-1：往前插入集合

```java
public class Demo {
    public static void main(String[] args) {
        Student s1 = new Student("xishi",25);
        Student s2 = new Student("yangyuhuan",29);
        Student s3 = new Student("diaochan",28);
        Student s4 = new Student("wangzhaojun",30);
        Student s5 = new Student("libai",30);
        Student s6 = new Student("libai",30);

        TreeSet<Student> ts = new TreeSet<>();

        ts.add(s1);
        ts.add(s2);
        ts.add(s3);
        ts.add(s4);
        ts.add(s5);
        ts.add(s6);

        for(Student s : ts){
            System.out.println(s.name+"---"+s.age);
        }

    }
}
```



**让容器自身具备比较性，自定义比较器。**

需求：当元素自身不具备比较性，或者元素自身具备的比较性不是所需的。

那么这时只能让容器自身具备。

定义一个类实现Comparator 接口，覆盖compare方法。

并将该接口的子类对象作为参数传递给TreeSet集合的构造函数。

当Comparable比较方式，及Comparator比较方式同时存在，以Comparator比较方式为主。


```java
public class Demo5 {
	public static void main(String[] args) {
		TreeSet ts = new TreeSet(new MyComparator());
		ts.add(new Book("think in java", 100));
		ts.add(new Book("java 核心技术", 75));
		ts.add(new Book("现代操作系统", 50));
		ts.add(new Book("java就业教程", 35));
		ts.add(new Book("think in java", 100));
		ts.add(new Book("ccc in java", 100));
 
		System.out.println(ts); 
	}
}
 
class MyComparator implements Comparator {
 
	public int compare(Object o1, Object o2) {
		Book b1 = (Book) o1;
		Book b2 = (Book) o2;
		System.out.println(b1+" comparator "+b2);
		if (b1.getPrice() > b2.getPrice()) {
			return 1;
		}
		if (b1.getPrice() < b2.getPrice()) {
			return -1;
		}
		return b1.getName().compareTo(b2.getName());
	}
 
}
 
class Book {
	private String name;
	private double price;
 
	public Book() {
 
	}
 
	public String getName() {
		return name;
	}
 
	public void setName(String name) {
		this.name = name;
	}
 
	public double getPrice() {
		return price;
	}
 
	public void setPrice(double price) {
		this.price = price;
	}
 
	public Book(String name, double price) {
 
		this.name = name;
		this.price = price;
	}
 
	@Override
	public String toString() {
		return "Book [name=" + name + ", price=" + price + "]";
	}
 
}
```
# 迭代器

所有实现了Collection接口的容器类都有一个iterator方法用以返回一个实现Iterator接口的对象

Iterator对象称作为迭代器，用以方便的对容器内元素的遍历操作，Iterator接口定义了如下方法：

- boolean hashNext();//判断是否有元素没有被遍历
- Object next();//返回游标当前位置的元素并将游标移动到下一个位置
- void remove();//删除游标左边的元素，在执行完next之后该操作只能执行一次



**问题：如何遍历Map集合呢？**



**方法1：通过迭代器Iterator实现遍历**

获取Iterator ：Collection 接口的iterator()方法

Iterator的方法：

- boolean hasNext(): 判断是否存在另一个可访问的元素
- Object next(): 返回要访问的下一个元素

```java
Set keys = dogMap.keySet(); //取出所有key的集合
Iterator it = keys.iterator(); //获取Iterator对象
while (it.hasNext()) {
    String key = (String) it.next(); //取出key
    Dog dog = (Dog) dogMap.get(key); //根据key取出对应的值
    System.out.println(key + "\t" + dog.getStrain());
}
```

**方法2：增强for循环**

```java
for(元素类型t 元素变量x : 数组或集合对象){
	引用了x的java语句
}
```
# 泛型

Java 泛型（generics）是 JDK 5 中引入的一个新特性, 泛型提供了编译时类型安全检测机制，该机制允许 程序员在编译时检测到非法的类型。

**泛型的本质是参数化类型，也就是说所操作的数据类型被指定为一个参数。**

如何解决以下强制类型转换时容易出现的异常问题?

 List的get(int index)方法获取元素
 Map的get(Object key)方法获取元素
 Iterator的next()方法获取元素

分析：通过泛型 ， JDK1.5使用泛型改写了集合框架中的所有接口和类

![image-20210331222202938](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331222202938.png)

![image-20210331222216052](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331222216052.png)



？ 通配符： < ? >

# Collections工具类

【前言】

Java提供了一个操作Set、List和Map等集合的工具类：Collections，该工具类提供了大量方法对集合进 行排序、查询和修改等操作，还提供了将集合对象置为不可变、对集合对象实现同步控制等方法。

这个类不需要创建对象，内部提供的都是静态方法。

### 1、Collectios概述

![image-20210331222908814](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331222908814.png)

此类完全由在 collection 上进行操作或返回 collection 的静态方法组成。它包含在 collection 上操作的多态算法，即“包装器”，包装器返回由指定 collection 支持的新 collection，以及少数其他内容。如果为 此类的方法所提供的 collection 或类对象为 null，则这些方法都将抛出 NullPointerException 。



### 2、排序操作

```java
static void reverse(List<?> list)//反转列表中元素的顺序。

static void shuffle(List<?> list) //对List集合元素进行随机排序。

static void sort(List<T> list) //根据元素的自然顺序 对指定列表按升序进行排序

static <T> void sort(List<T> list, Comparator<? super T> c) //根据指定比较器产生的顺序对指定列表进行排序。
    
static void swap(List<?> list, int i, int j)   //在指定List的指定位置i,j处交换元素。

static void rotate(List<?> list, int distance)
 //当distance为正数时，将List集合的后distance个元素“整体”移到前面；当distance为负数时，将list集合的前distance个元素“整体”移到后边。该方法不会改变集合的长度。
```

【演示】

```java
public static void main(String[] args) {
    ArrayList list = new ArrayList();
    list.add(3);
    list.add(-2);
    list.add(9);
    list.add(5);
    list.add(-1);
    list.add(6);

    //输出：[3, -2, 9, 5, -1, 6]
    System.out.println(list);
    //集合元素的次序反转
    Collections.reverse(list);
    //输出：[6, -1, 5, 9, -2, 3]
    System.out.println(list);
    //排序：按照升序排序
    Collections.sort(list);
    //[-2, -1, 3, 5, 6, 9]
    System.out.println(list);
    //根据下标进行交换
    Collections.swap(list, 2, 5);
    //输出：[-2, -1, 9, 5, 6, 3]
    System.out.println(list);
    
    /*//随机排序
    Collections.shuffle(list);
    //每次输出的次序不固定
    System.out.println(list);*/
    
    //后两个整体移动到前边
    Collections.rotate(list, 2);
    //输出：[6, 9, -2, -1, 3, 5]
    System.out.println(list);
}
```

【演示】

创建学生集合，加入数据，并**自定义排序**，先根据年龄，再根据首字母

pojo类

```java
public class Student {
    public String name;
    public int age;

    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }
}
```

test代码

```java
public static void main(String[] args) {
    ArrayList<Student> array = new ArrayList<>();
    Student s1 = new Student("lingqingxia",20);
    Student s2 = new Student("wangxizhi",30);
    Student s3 = new Student("libai",25);
    Student s4 = new Student("dufu",25);
	//Student s5 = new Student("dufu",25);

    array.add(s1);
    array.add(s2);
    array.add(s3);
    array.add(s4);
	//array.add(s5);
    Collections.sort(array, new Comparator<Student>() {
        @Override
        public int compare(Student o1, Student o2) {
            int i = o1.age-o2.age;
            int n = i==0?o1.name.compareTo(o2.name):i;
            return n;
        }
    });

    for (Student s:array){
        System.out.println(s.name+","+s.age);
    }
}
```

### 3、查找、替换操作

【方法】

```java
//使用二分搜索法搜索指定列表，以获得指定对象在List集合中的索引。
//注意：此前必须保证List集合中的元素已经处于有序状态。
static <T> int binarySearch(List<? extends Comparable<? super T>> list, T key)

//根据元素的自然顺序，返回给定collection 的最大元素。
static Object max(Collection coll)

   	//根据指定比较器产生的顺序，返回给定 collection 的最大元素。
    static Object max(Collection coll,Comparator comp)

    //根据元素的自然顺序，返回给定collection 的最小元素。
    static Object min(Collection coll)
    
    //根据指定比较器产生的顺序，返回给定 collection 的最小元素。
    static Object min(Collection coll,Comparator comp)
    
    使用指定元素替换指定列表中的所有元素。
    static <T> void fill(List<? super T> list, T obj)
    
    //返回指定 collection 中等于指定对象的出现次数。
    static int frequency(Collection<?> c, Object o)
    
    //返回指定源列表中第一次出现指定目标列表的起始位置；如果没有出现这样的列表，则返回-1。
    static int indexOfSubList(List<?> source, List<?> target) 
    
    //返回指定源列表中最后一次出现指定目标列表的起始位置；如果没有出现这样的列表，则返回-1。
    static int lastIndexOfSubList(List<?> source, List<?> target)
    
    //使用一个新值替换List对象的所有旧值oldVal
    static <T> boolean replaceAll(List<T> list, T oldVal, T newVal)

```

【演示：实例使用查找、替换操作】

```java
public static void main(String[] args) {
    ArrayList list = new ArrayList();
    list.add(3);
    list.add(-2);
    list.add(9);
    list.add(5);
    list.add(-1);
    list.add(6);
    //[3, -2, 9, 5, -1, 6]
    System.out.println(list);
    //输出最大元素9
    System.out.println(Collections.max(list));
    //输出最小元素：-2
    System.out.println(Collections.min(list));
    //将list中的-2用1来代替
    System.out.println(Collections.replaceAll(list, -2, 1));
    //[3, 1, 9, 5, -1, 6]
    System.out.println(list);
    list.add(9);
    //判断9在集合中出现的次数，返回2
    System.out.println(Collections.frequency(list, 9));
    //对集合进行排序
    Collections.sort(list);
    //[-1, 1, 3, 5, 6, 9, 9]
    System.out.println(list);
    //只有排序后的List集合才可用二分法查询，输出2
    System.out.println(Collections.binarySearch(list, 3));
}
```

### 4、同步控制

Collectons提供了多个synchronizedXxx()方法，该方法可以将指定集合包装成线程同步的集合，从 而解决多线程并发访问集合时的线程安全问题。

正如前面介绍的HashSet，TreeSet，arrayList,LinkedList,HashMap,TreeMap都是线程不安全的。 Collections提供了多个静态方法可以把他们包装成线程同步的集合。

【方法】

```java
//返回指定 collection 支持的同步（线程安全的）collection。
static <T> Collection<T> synchronizedCollection(Collection<T> c)
    
//返回指定列表支持的同步（线程安全的）列表。
static <T> List<T> synchronizedList(List<T> list)

//返回由指定映射支持的同步（线程安全的）映射。
static <K,V> Map<K,V> synchronizedMap(Map<K,V> m)

//返回指定 set 支持的同步（线程安全的）set
static <T> Set<T> synchronizedSet(Set<T> s)
```

【实例】

```java
public static void main(String[] args) {
    //下面程序创建了四个同步的集合对象
    Collection c = Collections.synchronizedCollection(new ArrayList());
    List list = Collections.synchronizedList(new ArrayList());
    Set s = Collections.synchronizedSet(new HashSet());
    Map m = Collections.synchronizedMap(new HashMap());

}
```

### 5、Collesction设置不可变集合

【方法】

```java
//返回一个空的、不可变的集合对象，此处的集合既可以是List，也可以是Set，还可以是Map。
emptyXxx()

//返回一个只包含指定对象（只有一个或一个元素）的不可变的集合对象，此处的集合可以是：List，Set，Map。
singletonXxx()
    
//返回指定集合对象的不可变视图，此处的集合可以是：List，Set，Map。
unmodifiableXxx():
```

上面三类方法的参数是原有的集合对象，返回值是该集合的”只读“版本。

【实例】

```java
public static void main(String[] args) {
    //创建一个空的、不可改变的List对象
    List<String> unmodifiableList = Collections.emptyList();
    //unmodifiableList.add("java");
    //添加出现异常：java.lang.UnsupportedOperationException
    System.out.println(unmodifiableList);// []
    //创建一个只有一个元素，且不可改变的Set对象
    Set unmodifiableSet = Collections.singleton("Struts2权威指南");
    //[Struts2权威指南]
    System.out.println(unmodifiableSet);
    //创建一个普通Map对象
    Map scores = new HashMap();
    scores.put("语文", 80);
    scores.put("Java", 82);
    //返回普通Map对象对应的不可变版本
    Map unmodifiableMap = Collections.unmodifiableMap(scores);
    //下面任意一行代码都将引发UnsupportedOperationException异常
    unmodifiableList.add("测试元素");
    unmodifiableSet.add("测试元素");
    unmodifiableMap.put("语文", 90);
    
}
```

### 总结和测试

实体类：Pojo

```java
import java.util.*;


public class CollectionsTest {
    public static void main(String[] args) {
        //创建一个空的、不可改变的List对象
        List<String> unmodifiableList = Collections.emptyList();
        //unmodifiableList.add("java");
        //添加出现异常：java.lang.UnsupportedOperationException
        System.out.println(unmodifiableList);// []
        //创建一个只有一个元素，且不可改变的Set对象
        Set unmodifiableSet = Collections.singleton("Struts2权威指南");
        //[Struts2权威指南]
        System.out.println(unmodifiableSet);
        //创建一个普通Map对象
        Map scores = new HashMap();
        scores.put("语文", 80);
        scores.put("Java", 82);
        //返回普通Map对象对应的不可变版本
        Map unmodifiableMap = Collections.unmodifiableMap(scores);
        //下面任意一行代码都将引发UnsupportedOperationException异常
        unmodifiableList.add("测试元素");
        unmodifiableSet.add("测试元素");
        unmodifiableMap.put("语文", 90);

    }

}
```

测试类代码如下

```java
import java.util.ArrayList;
import java.util.List;

public class Test01 {
    public static void main(String[] args) throws Exception {
        //一个对象对应了一行记录！
        Employee e1 = new Employee(0301, "狂神", 3000, "项目部", "2017-10");
        Employee e2 = new Employee(0302, "小明", 3500, "教学部", "2016-10");
        Employee e3 = new Employee(0303, "小红", 3550, "教学部", "2016-10");
        List<Employee> list = new ArrayList<Employee>();
        list.add(e1);
        list.add(e2);
        list.add(e3);
        printEmpName(list);
    }

    public static void printEmpName(List<Employee> list) {
        for (int i = 0; i < list.size(); i++) {
            System.out.println(list.get(i).getName() + "-" + list.get(i).getHireDate());
        }
    }
}
```

### 斗地主案例

简易版本

```java
public static void main(String[] args) {
    ArrayList<String> array = new ArrayList<>();

    String[] colors = {"方片", "梅花", "黑桃", "红桃"};
    String[] numbers = {"1","2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K"};

    for (String c : colors) {
        for (String n : numbers) {
            array.add(c + n);
        }
    }
    array.add("小王");
    array.add("大王");
    Collections.shuffle(array);//洗牌

    //发牌
    ArrayList<String> wj1 = new ArrayList<>();//玩家1
    ArrayList<String> wj2 = new ArrayList<>();
    ArrayList<String> wj3 = new ArrayList<>();
    ArrayList<String> dp = new ArrayList<>();//底牌


    for (int i = 0; i < array.size(); i++) {
        String s = array.get(i);
        if (i >= array.size() - 3) {
            dp.add(s);
        }else{
            int i1 = i % 3;
            switch (i1){
                case 0:
                    wj1.add(s);
                    break;
                case 1:
                    wj2.add(s);
                    break;
                case 2:
                    wj3.add(s);
                    break;
            }
        }
    }
    //看牌
    System.out.println("底牌："+dp);
    System.out.println("玩家1的牌"+wj1);
    System.out.println("玩家2的牌"+wj2);
    System.out.println("玩家3的牌"+wj3);

}
```


>底牌：[梅花1, 黑桃2, 红桃Q]
>
>玩家1的牌[黑桃10, 大王, 方片7, 梅花5, 方片9, 方片3, 黑桃4, 红桃8, 梅花4, 红桃9, 红桃2, 红桃4, 小王, 方片K, 红桃6, 黑桃6, 红桃K]
>
>玩家2的牌[红桃1, 红桃7, 黑桃7, 方片J, 红桃J, 梅花3, 梅花7, 梅花8, 梅花9, 梅花2, 梅花J, 红桃10, 方片10, 黑桃5, 方片1, 黑桃K, 黑桃Q]
>
>玩家3的牌[方片5, 方片4, 黑桃9, 方片8, 黑桃3, 方片Q, 方片6, 红桃5, 梅花6, 黑桃8, 黑桃1, 梅花Q, 红桃3, 梅花10, 方片2, 梅花K, 黑桃J]

可以看到，能实现洗牌，发牌，看牌

但是牌的顺序不是从小到大的，我们来改进一下

![image-20210331233413189](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaSE-集合.assets/image-20210331233413189.png)

1. 用HashMap键值对从0到53序号，存储牌
2. 用ArrayList存牌的序号
3. 用TreeSet存玩家的牌的序号，TreeSet可以自动排序
4. 通过TreeSet的序号，从HashMap中查取牌

```java
public class Poker {
    public static void main(String[] args) {
        //编号，牌
        HashMap<Integer,String> hm = new HashMap<>();
        //储存编号
        ArrayList<Integer> array = new ArrayList<>();

        String[] colors = {"方片", "梅花", "黑桃", "红桃"};
        String[] numbers = { "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K","A","2"};
        int index=0;
        for (String c:colors){
            for (String n:numbers){
                hm.put(index,c+n);
                array.add(index);
                index++;
            }
        }
        hm.put(index,"小王");
        array.add(index);
        index++;
        hm.put(index,"大王");
        array.add(index);

        Collections.shuffle(array);//洗牌
        //发牌
        TreeSet<Integer> wj1 = new TreeSet<>();//玩家1
        TreeSet<Integer> wj2 = new TreeSet<>();
        TreeSet<Integer> wj3 = new TreeSet<>();
        TreeSet<Integer> dp  = new TreeSet<>();//底牌

        for (int i = 0; i < array.size(); i++) {
            Integer s = array.get(i);
            if (i >= array.size() - 3) {
                dp.add(s);
            }else{
                int i1 = i % 3;
                switch (i1){
                    case 0:
                        wj1.add(s);
                        break;
                    case 1:
                        wj2.add(s);
                        break;
                    case 2:
                        wj3.add(s);
                        break;
                }
            }
        }
        lookpoke("玩家1",wj1 ,hm);
        lookpoke("玩家2",wj2 ,hm);
        lookpoke("玩家3",wj3 ,hm);
        lookpoke("底牌",dp ,hm);

    }
    public  static void lookpoke(String name,TreeSet<Integer> ts,HashMap<Integer,String> hm){
        System.out.print(name+"的牌：   ");
        for (Integer t:ts){
            System.out.print(hm.get(t)+" ");
        }
        System.out.println();

    }
}
```
# 多线程

## 1、简介

### 什么是JUC

JUC是java.util.concurrent 的简写，在并发编程中使用的工具类。

在jdk官方手册中可以看到juc相关的jar包有三个。

用中文概括一下，JUC的意思就是java并发编程工具包

实现多线程有三种方式：Thread、Runnable、Callable，其中Callable就位于concurrent包下 

### 进程和线程

>  进程 / 线程是什么？

进程：进程是一个具有一定独立功能的程序关于某个数据集合的一次运行活动。它是操作系统动态执行的基本单元，在传统的操作系统中，进程既是基本的分配单元，也是基本的执行单元。

线程：通常在一个进程中可以包含若干个线程，当然一个进程中至少有一个线程，不然没有存在的意义，线程可以利用进程所有拥有的资源。在引入线程的操作系统中，通常都是把进程作为分配资源的基本单位，而把线程作为独立运行和独立调度的基本单位，由于线程比进程小，基本上不拥有系统资源， 故对它的调度所付出的开销就会小得多，能更高效的提高系统多个程序间并发执行的程度。

白话： 

进程：就是操作系统中运行的一个程序，QQ.exe，music.exe，word.exe ，这就是多个进程 

线程：每个进程中都存在一个或者多个线程，比如用word写文章时，就会有一个线程默默帮你定时自动保存。

> 并发 / 并行是什么？

做并发编程之前，必须首先理解什么是并发，什么是并行。

并发和并行是两个非常容易混淆的概念。它们都可以表示两个或多个任务一起执行，但是偏重点有点不同。并发偏重于多个任务交替执行，而多个任务之间有可能还是串行的。并发是逻辑上的同时发生（simultaneous），而并行是物理上的同时发生。然而并行的偏重点在于”同时执行”。

严格意义上来说，并行的多个任务是真实的同时执行，而对于并发来说，这个过程只是交替的，一会运行任务一,一会儿又运行任务二，系统会不停地在两者间切换。但对于外部观察者来说，即使多个任务是串行并发的，也会造成是多个任务并行执行的错觉。

实际上，如果系统内只有一个CPU，而现在而使用多线程或者多线程任务，那么真实环境中这些任务不可能真实并行的，毕竟一个CPU一次只能执行一条指令，这种情况下多线程或者多线程任务就是并发的，而不是并行，操作系统会不停的切换任务。真正的并发也只能够出现在拥有多个CPU的系统中（多核CPU）。

**并发的动机**：在计算能力恒定的情况下处理更多的任务, 就像我们的大脑, 计算能力相对恒定, 要在一天中处理更多的问题, 我们就必须具备多任务的能力. 现实工作中有很多事情可能会中断你的当前任务, 处理这种多任务的能力就是你的并发能力。

**并行的动机**：用更多的CPU核心更快的完成任务. 就像一个团队, 一个脑袋不够用了, 一个团队来一起处理 一个任务。

例子：
你吃饭吃到一半，电话来了，你一直到吃完了以后才去接，这就说明你不支持并发也不支持并行。
你吃饭吃到一半，电话来了，你停了下来接了电话，接完后继续吃饭，这说明你支持并发。 （不一定是
同时的）
你吃饭吃到一半，电话来了，你一边打电话一边吃饭，这说明你支持并行。
所以并发编程的目标是充分的利用处理器的每一个核，以达到最高的处理性能。

 

> 线程的状态

Java的线程有6种状态：可以分析源码：

```java
public enum State {
    //线程刚创建
    NEW,
    
    //在JVM中正在运行的线程
    RUNNABLE,
    
    //线程处于阻塞状态，等待监视锁，可以重新进行同步代码块中执行
    BLOCKED,
    
    //等待状态
    WAITING,
    
    //调用sleep() join() wait()方法可能导致线程处于等待状态
    TIMED_WAITING,
    
    //线程执行完毕，已经退出
    TERMINATED;
}
```

![image-20210513145542628](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/image-20210513145542628.png)

> wait / sleep 的区别

**1、来自不同的类**

这两个方法来自不同的类分别是，sleep来自Thread类，和wait来自Object类。

sleep是Thread的静态类方法，谁调用的谁去睡觉，即使在a线程里调用了b的sleep方法，实际上还是a去睡觉，要让b线程睡觉要在b的代码中调用sleep。

**2、有没有释放锁(释放资源)**

最主要是sleep方法没有释放锁

而wait方法释放了锁，使得其他线程可以使用同步控制块或者方法。



sleep是线程被调用时，占着cpu去睡觉，其他线程不能占用cpu，os认为该线程正在工作，不会让出系统资源，wait是进入等待池等待，让出系统资源，其他线程可以占用cpu。



sleep(100L)是占用cpu，线程休眠100毫秒，其他进程不能再占用cpu资源，wait（100L）是进入等待池中等待，交出cpu等系统资源供其他进程使用，在这100毫秒中，该线程可以被其他线程notify，但不同的是其他在等待池中的线程不被notify不会出来，但这个线程在等待100毫秒后会自动进入就绪队列等待系统分配资源，换句话说，sleep（100）在100毫秒后肯定会运行，但wait在100毫秒后还有等待os调用分配资源，所以wait100的停止运行时间是不确定的，但至少是100毫秒。
就是说sleep有时间限制的就像闹钟一样到时候就叫了，而wait是无限期的除非用户主动notify。

**3、使用范围不同**

wait，notify和notifyAll只能在同步控制方法或者同步控制块里面使用，而sleep可以在任何地方使用

```java
synchronized(x){
    //或者wait()
    x.notify()
}
```

**4、是否需要捕获异常** 

sleep必须捕获异常，而wait，notify和notifyAll不需要捕获异常

## 2、Lock锁

### synchronized锁

```java
public class SaleTicketTest1 {
    /*
     * 题目：三个售票员 卖出 30张票
     * 多线程编程的企业级套路：
     * 1. 在高内聚低耦合的前提下， 线程 操作(对外暴露的调用方法) 资源类
     */

    public static void main(String[] args) {
        Ticket ticket = new Ticket();

        new Thread(new Runnable() {
            @Override
            public void run() {
                for (int i = 1; i <= 40; i++) {
                    ticket.saleTicket();
                }
            }
        }, "A").start();

        new Thread(new Runnable() {
            @Override
            public void run() {
                for (int i = 1; i <=40; i++) {
                    ticket.saleTicket();
                }
            }
        }, "B").start();

        new Thread(new Runnable() {
            @Override
            public void run() {
                for (int i = 1; i <= 40; i++) {
                    ticket.saleTicket();
                }
            }
        }, "C").start();

    }
    
}

class Ticket { // 资源类
    private int number = 30;

    public synchronized void saleTicket() {
        if (number > 0) {
            System.out.println(Thread.currentThread().getName() + "卖出第 " + (number--) + "票,还剩下:" + number);
        }
    }
}
```

### Lock 锁

```java
public class SaleTicketTest2 {
    public static void main(String[] args) {
        Ticket2 ticket2 = new Ticket2();

        new Thread(() -> {
            for (int i = 1; i <= 40; i++) {
                ticket2.saleTicket();
            }
        }, "A").start();

        new Thread(() -> {
            for (int i = 1; i <= 40; i++) {
                ticket2.saleTicket();
            }
        }, "B").start();

        new Thread(() -> {
            for (int i = 1; i <= 40; i++) {
                ticket2.saleTicket();
            }
        }, "C").start();

    }
}

class Ticket2 { // 资源类
    private Lock lock = new ReentrantLock();

    private int number = 30;

    public void saleTicket() {
        lock.lock();

        try {
            if (number > 0) {
                System.out.println(Thread.currentThread().getName() + "卖出第 " + (number--) + "票,还剩下:" + number);
            }
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }

    }
}
```

###  区别

1. 首先synchronized是java内置关键字，在jvm层面，Lock是个java类；
2. synchronized无法判断是否获取锁的状态，Lock可以判断是否获取到锁；
3. synchronized会自动释放锁(a 线程执行完同步代码会释放锁 ；b 线程执行过程中发生异常会释放
锁)，Lock需在finally中手工释放锁（unlock()方法释放锁），否则容易造成线程死锁；
4. 用synchronized关键字的两个线程1和线程2，如果当前线程1获得锁，线程2线程等待。如果线程1
阻塞，线程2则会一直等待下去，而Lock锁就不一定会等待下去，如果尝试获取不到锁，线程可以
不用一直等待就结束了；
5. synchronized的锁可重入、不可中断、非公平，而Lock锁可重入、可判断、可公平（两者皆可）
6. Lock锁适合大量同步的代码的同步问题，synchronized锁适合代码少量的同步问题。

##  3、生产者和消费者

### synchroinzed 

生产者和消费者 synchroinzed 版

```java
public class ProducerConsumer {
    /**
     * 题目：现在两个线程，可以操作初始值为0的一个变量
     * 实现一个线程对该变量 + 1，一个线程对该变量 -1
     * 实现交替10次
     * <p>
     * 诀窍：
     * 1. 高内聚低耦合的前提下，线程操作资源类
     * 2. 判断 、干活、通知
     */

    public static void main(String[] args) {
        Data data = new Data();

        //A线程增加
        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.increment();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "A").start();

        //B线程减少
        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.decrement();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "B").start();
    }
}

class Data {
    private int number = 0;

    public synchronized void increment() throws InterruptedException {
        // 判断该不该这个线程做
        if (number != 0) {
            this.wait();
        }
        // 干活
        number++;
        System.out.println(Thread.currentThread().getName() + "\t" + number);
        // 通知
        this.notifyAll();
    }

    public synchronized void decrement() throws InterruptedException {
        // 判断该不该这个线程做
        if (number == 0) {
            this.wait();
        }
        // 干活
        number--;
        System.out.println(Thread.currentThread().getName() + "\t" + number);
        // 通知
        this.notifyAll();
    }

}
```

问题升级：防止虚假唤醒，4个线程，两个加，两个减

【重点】if 和 while

```java
public class ProducerConsumerPlus {
    /**
     * 题目：现在四个线程，可以操作初始值为0的一个变量
     * 实现两个线程对该变量 + 1，两个线程对该变量 -1
     * 实现交替10次
     *
     * 诀窍：
     * 1. 高内聚低耦合的前提下，线程操作资源类
     * 2. 判断 、干活、通知
     * 3. 多线程交互中，必须要防止多线程的虚假唤醒，即（判断不能用if，只能用while）
     */

    public static void main(String[] args) {
        Data2 data = new Data2();

        //A线程增加
        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.increment();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "A").start();

        //B线程减少
        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.decrement();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "B").start();

        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.increment();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "C").start();

        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.decrement();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "D").start();
    }
}

class Data2 {
    private int number = 0;

    public synchronized void increment() throws InterruptedException {
        // 判断该不该这个线程做
        while (number != 0) {
            this.wait();
        }
        // 干活
        number++;
        System.out.println(Thread.currentThread().getName() + "\t" + number);
        // 通知
        this.notifyAll();
    }

    public synchronized void decrement() throws InterruptedException {
        // 判断该不该这个线程做
        while (number == 0) {
            this.wait();
        }
        // 干活
        number--;
        System.out.println(Thread.currentThread().getName() + "\t" + number);
        // 通知
        this.notifyAll();
    }

}
```



### lock



```java
public class ProducerConsumerPlus {
    /**
     * 题目：现在四个线程，可以操作初始值为0的一个变量
     * 实现两个线程对该变量 + 1，两个线程对该变量 -1
     * 实现交替10次
     * <p>
     * 诀窍：
     * 1. 高内聚低耦合的前提下，线程操作资源类
     * 2. 判断 、干活、通知
     * 3. 多线程交互中，必须要防止多线程的虚假唤醒，即（判断不能用if，只能用while）
     */

    public static void main(String[] args) {
        Data2 data = new Data2();

        //A线程增加
        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.increment();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "A").start();

        //B线程减少
        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.decrement();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "B").start();

        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.increment();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "C").start();

        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                try {
                    data.decrement();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "D").start();
    }
}

class Data2 {
    private int number = 0;
    private Lock lock = new ReentrantLock();
    private Condition condition = lock.newCondition();

    public void increment() throws InterruptedException {

        lock.lock();
        try {
            // 判断该不该这个线程做
            while (number != 0) {
                condition.await();
            }
            // 干活
            number++;
            System.out.println(Thread.currentThread().getName() + "\t" + number);
            // 通知
            condition.signalAll();
        } catch (InterruptedException e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }
    }

    public void decrement() throws InterruptedException {
        lock.lock();
        try {
            // 判断该不该这个线程做
            while (number == 0) {
                condition.await();
            }
            // 干活
            number--;
            System.out.println(Thread.currentThread().getName() + "\t" + number);
            // 通知
            condition.signalAll();
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }
    }

}
```

以上写的程序并不会按照ABCD线程顺序，只会按照 “生产” “消费”顺序

### 按照线程顺序执行

精确通知顺序访问

```java
public class c {
    /**
     * 题目：多线程之间按顺序调用，实现 A->B->C
     * 重点：标志位
     */

    public static void main(String[] args) {
        Resources resources = new Resources();

        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                resources.a();
            }

        }, "A").start();

        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                resources.b();
            }

        }, "B").start();

        new Thread(() -> {
            for (int i = 1; i <= 10; i++) {
                resources.c();
            }

        }, "C").start();

    }
}

class Resources {
    private int number = 1; // 1A 2B 3C
    private Lock lock = new ReentrantLock();
    private Condition condition1 = lock.newCondition();
    private Condition condition2 = lock.newCondition();
    private Condition condition3 = lock.newCondition();

    public void a() {
        lock.lock();
        try {
            // 判断
            while (number != 1) {
                condition1.await();
            }
            // 干活
            System.out.println(Thread.currentThread().getName());
            // 通知,指定的干活！
            number = 2;
            condition2.signal();
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }
    }

    public void b() {
        lock.lock();
        try {
            // 判断
            while (number != 2) {
                condition2.await();
            }
            // 干活
            System.out.println(Thread.currentThread().getName() );

            // 通知,指定的干活！
            number = 3;
            condition3.signal();
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }
    }

    public void c() {
        lock.lock();
        try {
            // 判断
            while (number != 3) {
                condition3.await();
            }
            // 干活
            System.out.println(Thread.currentThread().getName());

            // 通知,指定的干活！
            number = 1;
            condition1.signal();
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }
    }
}
```



## 4、8锁的现象




### 问题一

1、标准访问，请问先打印邮件还是短信？

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

public class A {
    /**
     * 多线程的8锁
     * 1、标准访问，请问先打印邮件还是短信？
     */
    public static void main(String[] args) throws InterruptedException {
        Phone phone = new Phone();
        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        //休眠一秒
        //Thread.sleep(1000);
        TimeUnit.SECONDS.sleep(1);
        
        new Thread(() -> {
            try {
                phone.sendSMS();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone {
    public synchronized void sendEmail(){
        System.out.println("sendEmail");
    }

    public synchronized void sendSMS(){
        System.out.println("sendSMS");
    }
}

```

答案：sendEmail

结论：被synchronized修饰的方法，锁的对象是方法的调用者。因为两个方法的调用者是同一个，所以两个方法用的是同一个锁，先调用方法的先执行。



### 问题二

2、邮件方法暂停4秒钟，请问先打印邮件还是短信？

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

public class B {
    /**
     * 多线程的8锁
     * 2、邮件方法暂停4秒钟，请问先打印邮件还是短信？
     */
    public static void main(String[] args) throws InterruptedException {
        Phone2 phone = new Phone2();
        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            try {
                phone.sendSMS();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone2 {
    public synchronized void sendEmail() throws Exception {
        TimeUnit.SECONDS.sleep(4);
        System.out.println("sendEmail");
    }

    public synchronized void sendSMS(){
        System.out.println("sendSMS");
    }
}
```

答案：sendEmail  

结论：被synchronized修饰的方法，锁的对象是方法的调用者。因为两个方法的调用者是同一个，所以两个方法用的是同一个锁，先调用方法的先执行，第二个方法只有在第一个方法执行完释放锁之后才能执行。

### 问题三

3、新增一个普通方法hello()不加锁，请问先打印邮件还是hello？

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

/**
 * @author zhiyuan
 */
public class C {
    /**
     * 多线程的8锁
     * 3、新增一个普通方法hello()不加锁，请问先打印邮件还是hello？
     */
    public static void main(String[] args) throws InterruptedException {
        Phone3 phone = new Phone3();
        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            try {
                phone.hello();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone3 {
    public synchronized void sendEmail() throws Exception {
        TimeUnit.SECONDS.sleep(4);
        System.out.println("sendEmail");
    }
    
    // 没有 synchronized，没有 static 就是普通方式
    public void hello() {
        System.out.println("Hello");
    }
}
```

答案：Hello

结论：如果一个方法没有被synchronized修饰，不是同步方法，不受锁的影响，所以不需要等待。

### 问题四

4、两个手机，一个手机发邮件，另一个发短信，请问先执行sendEmail 还是 sendSMS

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

public class D {
    /**
     * 多线程的8锁
     * 4、两个手机，请问先执行sendEmail 还是 sendSMS
     */
    public static void main(String[] args) throws InterruptedException {
        Phone4 phone = new Phone4();
        Phone4 phone2 = new Phone4();

        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            try {
                phone2.sendSMS();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone4 {
    public synchronized void sendEmail() throws Exception {
        TimeUnit.SECONDS.sleep(4);
        System.out.println("sendEmail");
    }

    public synchronized void sendSMS() {
        System.out.println("sendSMS");
    }
}
```



答案：先执行“sendSMS”

结论：被synchronized修饰的方法，锁的对象是方法的调用者。用了两个对象调用各自的方法，所以两个方法的调用者不是同一个，于是两个方法用的不是同一个锁，后调用的方法不需要等待先调用的方法。

### 问题五

5、两个静态同步方法，同一部手机，请问先打印邮件还是短信？

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

public class E {
    /**
     * 多线程的8锁
     * 5、两个静态同步方法，同一部手机，请问先打印邮件还是短信？
     */
    public static void main(String[] args) throws InterruptedException {
        Phone5 phone = new Phone5();

        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            try {
                phone.sendSMS();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone5 {
    public static synchronized void sendEmail() throws Exception {
        TimeUnit.SECONDS.sleep(4);
        System.out.println("sendEmail");
    }

    public static synchronized void sendSMS() {
        System.out.println("sendSMS");
    }
}
```



答案：先执行“sendEmail”

结论：被synchronized和static修饰的方法，锁的对象是类的class模板对象，这个则全局唯一！两个方法都被static修饰了，所以两个方法用的是同一个锁，后调用的方法需要等待先调用的方法。

### 问题六

6、两个静态同步方法，2部手机，一个手机发邮件，另一个发短信，请问先打印邮件还是短信？

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

/**
 * @author zhiyuan
 */
public class F {
    /**
     * 多线程的8锁
     * 6、两个静态同步方法，2部手机，一个手机发邮件，另一个发短信，请问先打印邮件还是短信？
     */
    public static void main(String[] args) throws InterruptedException {
        Phone6 phone = new Phone6();

        Phone6 phone2 = new Phone6();

        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            try {
                phone2.sendSMS();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone6 {
    public static synchronized void sendEmail() throws Exception {
        TimeUnit.SECONDS.sleep(4);
        System.out.println("sendEmail");
    }

    public static synchronized void sendSMS() {
        System.out.println("sendSMS");
    }
}
```

答案：先输出“sendEmail”

结论：被synchronized和static修饰的方法，锁的对象就是Class模板对象，这个则全局唯一！所以说这里是同一个

### 问题七

7、一个普通同步方法，一个静态同步方法，同一部手机，请问先打印邮件还是短信？

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

public class G {
    /**
     * 多线程的8锁
     * 7、一个普通同步方法，一个静态同步方法，同一部手机，请问先打印邮件还是短信？
     */
    public static void main(String[] args) throws InterruptedException {
        Phone7 phone = new Phone7();

        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            try {
                phone.sendSMS();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone7 {
    public static synchronized void sendEmail() throws Exception {
        TimeUnit.SECONDS.sleep(4);
        System.out.println("sendEmail");
    }

    public synchronized void sendSMS() {
        System.out.println("sendSMS");
    }
}
```

答案：先执行“sendSMS”

结论：synchronized 锁的是这个调用的对象。被synchronized和static修饰的方法，锁的是这个类的Class模板 。这里是两个锁！

### 问题八

8、一个普通同步方法，一个静态同步方法，2部手机，一个发邮件，一个发短信，请问哪个先执行？

```java
package com.oddfar.lock8;

import java.util.concurrent.TimeUnit;

/**
 * @author zhiyuan
 */
public class H {
    /**
     * 多线程的8锁
     * 8、一个普通同步方法，一个静态同步方法，2部手机，一个发邮件，一个发短信，请问先打印邮件还是短信？
     */
    public static void main(String[] args) throws InterruptedException {
        Phone8 phone = new Phone8();
        Phone8 phone2 = new Phone8();

        new Thread(() -> {
            try {
                phone.sendEmail();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "A").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            try {
                phone2.sendSMS();
            } catch (Exception e) {
                e.printStackTrace();
            }
        }, "B").start();

    }
}

class Phone8 {
    public static synchronized void sendEmail() throws Exception {
        TimeUnit.SECONDS.sleep(4);
        System.out.println("sendEmail");
    }

    public synchronized void sendSMS() {
        System.out.println("sendSMS");
    }
}
```

答案：sendSMS

结论：被synchronized和static修饰的方法，锁的对象是类的class对象。仅被synchronized修饰的方法，锁的对象是方法的调用者。即便是用同一个对象调用两个方法，锁的对象也不是同一个，所以两个方法用的不是同一个锁，后调用的方法不需要等待先调用的方法。

### 小结

1、new this 调用的这个对象，是一个具体的对象！

2、static class 唯一的一个模板！

一个对象里面如果有多个synchronized方法，某个时刻内，只要一个线程去调用其中一个synchronized 方法了，其他的线程都要等待，换句话说，在某个时刻内，只能有唯一一个线程去访问这些 synchronized方法，锁的是当前对象this，被锁定后，其他的线程都不能进入到当前对象的其他的 synchronized方法

加个普通方法后发现和同步锁无关，换成两个对象后，不是同一把锁，情况变化

都换成静态同步方法后，情况又变化了。所有的非静态的同步方法用的都是同一把锁（锁的class模板）

**具体的表现为以下三种形式：** 

- 对于普通同步方法，锁的是当前实例对象 

- 对于静态同步方法，锁的是当前的Class对象。 

- 对于同步方法块，锁是synchronized括号里面的配置对象

当一个线程试图访问同步代码块时，他首先必须得到锁，退出或者是抛出异常时必须释放锁，也就是说 如果一个实例对象的非静态同步方法获取锁后，该实例对象的其他非静态同步方法必须等待获取锁的方法释放锁后才能获取锁，可以是别的实例对象非非静态同步方法因为跟该实例对象的非静态同步方法用 的是不同的锁，所以必须等待该实例对象已经获取锁的非静态同步方法释放锁就可以获取他们自己的 锁。

所有的静态同步方法用的也是同一把锁（类对象本身） ，这两把锁的是两个不同的对象，所以静态的同步方法与非静态的同步方法之间是不会有竞争条件的，但是一旦一个静态同步方法获取锁后，其他的静态同步方法都必须等待该方法释放锁后才能获取锁，而不是同一个实例对象的静态同步方法之间，还是不同的实例对象的静态同步方法之间，只要他们用一个的是同一个类的实例对象。

## 5、多线程下集合类的不安全

### list 

多线程下

```java
public class ListTest {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        // 对比3个线程 和 30个线程，看区别
        for (int i = 1; i <= 30; i++) {
            new Thread(() -> {
                list.add(UUID.randomUUID().toString().substring(0, 8));
                System.out.println(list);
            }, String.valueOf(i)).start();
        }
    }
}
```

运行报错：`java.util.ConcurrentModificationException`

导致原因：add 方法没有加锁

解决方案：

```java
/**
 * 换一个集合类
 *  1、List<String> list = new Vector<>(); JDK1.0 就存在了！
 *  2、List<String> list = Collections.synchronizedList(new ArrayList<>());
 *  3、List<String> list = new CopyOnWriteArrayList<>();
 */
public class ListTest {
    public static void main(String[] args) {

        List<String> list = new CopyOnWriteArrayList<>();

        for (int i = 1; i <= 30; i++) {
            new Thread(() -> {
                list.add(UUID.randomUUID().toString().substring(0, 8));
                System.out.println(list);
            }, String.valueOf(i)).start();
        }
    }
}
```

**写入时复制（CopyOnWrite）思想**

写入时复制（CopyOnWrite，简称COW）思想是计算机程序设计领域中的一种优化策略。其核心思想是，如果有多个调用者（Callers）同时要求相同的资源（如内存或者是磁盘上的数据存储），他们会共同获取相同的指针指向相同的资源，直到某个调用者视图修改资源内容时，系统才会真正复制一份专用副本（private copy）给该调用者，而其他调用者所见到的最初的资源仍然保持不变。这过程对其他的调用者都是透明的（transparently）。此做法主要的优点是如果调用者没有修改资源，就不会有副本 （private copy）被创建，因此多个调用者只是读取操作时可以共享同一份资源。

**CopyOnWriteArrayList为什么并发安全且性能比Vector好**

Vector是增删改查方法都加了synchronized，保证同步，但是每个方法执行的时候都要去获得锁，性能就会大大下降，而CopyOnWriteArrayList 只是在增删改上加锁，但是读不加锁，在读方面的性能就好于Vector，CopyOnWriteArrayList支持读多写少的并发情况。

### set



```java
/**
 * 1、Set<String> set = Collections.synchronizedSet(new HashSet<>());
 * 2、Set<String> set = new CopyOnWriteArraySet();
 */
public class SetTest {
    public static void main(String[] args) {

        Set<String> set = new CopyOnWriteArraySet();

        for (int i = 1; i <= 30; i++) {
            new Thread(() -> {
                set.add(UUID.randomUUID().toString().substring(0, 8));
                System.out.println(set);
            }, String.valueOf(i)).start();
        }
    }
}
```

### map

hashMap底层是数组+链表+红黑树

```java
Map<String,String> map = new HashMap<>();
// 等价于
Map<String,String> map = new HashMap<>(16,0.75);
// 工作中，常常会自己根据业务来写参数，提高效率
```

map不安全测试：

```java
public class MapSet {
    public static void main(String[] args) {
        Map<String, String> map = new HashMap<>();

        for (int i = 1; i <= 30; i++) {
            new Thread(() -> {
                map.put(Thread.currentThread().getName(),
                        UUID.randomUUID().toString().substring(0, 8));
                System.out.println(map);
            }, String.valueOf(i)).start();
        }
    }
}
```

解决：

```java
Map<String,String> map = new ConcurrentHashMap<>();
```

## 6、Callable

我们已经知道Java中常用的两种线程实现方式：分别是继承Thread类和实现Runnable接口。

![img](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/95eef01f3a292df5cb9047105febf76635a87341.jpeg)

从上图中，我们可以看到，第三种实现Callable接口的线程，而且还带有返回值的。我们来对比下实现Runnable和实现Callable接口的两种方式不同点：

1：需要实现的方法名称不一样：一个run方法，一个call方法

2：返回值不同：一个void无返回值，一个带有返回值的。其中返回值的类型和泛型V是一致的。

3：异常：一个无需抛出异常，一个需要抛出异常。

### 基础入门

```java
public class CallableDemo {
    public static void main(String[] args) throws Exception {
        MyThread myThread = new MyThread();
        FutureTask futureTask = new FutureTask(myThread); // 适配类
        Thread t1 = new Thread(futureTask, "A"); // 调用执行
        t1.start();
        Integer result = (Integer) futureTask.get(); // 获取返回值
        System.out.println(result);
    }
}

class MyThread implements Callable<Integer> {
    @Override
    public Integer call() throws Exception {
        System.out.println("call 被调用");
        return 1024;
    }
}
```

![image-20210516160612609](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/image-20210516160612609.png)

### 多个线程调用

```java
public class CallableDemo {
    public static void main(String[] args) throws Exception {
        MyThread myThread = new MyThread();
        FutureTask futureTask = new FutureTask(myThread); // 适配类

        new Thread(futureTask, "A").start(); // 调用执行
        // 第二次调用执行，在同一个futureTask对象，不输出结果，可理解为“缓存”
        new Thread(futureTask, "B").start(); 

        //get 方法获得返回结果! 一般放在最后一行！否则可能会阻塞
        Integer result = (Integer) futureTask.get(); // 获取返回值
        System.out.println(result);
    }
}

class MyThread implements Callable<Integer> {
    @Override
    public Integer call() throws Exception {
        System.out.println(Thread.currentThread().getName() + "\tcall 被调用");
        TimeUnit.SECONDS.sleep(2);
        return 1024;
    }
}
```

### 参考资料

- https://baijiahao.baidu.com/s?id=1666820818587296272

## 7、常用辅助类

### CountDownLatch

“倒计时锁存器”

例如，执行完6个线程输出执行完毕

```java
public class CountDownLatchDemo {
    public static void main(String[] args) throws InterruptedException {
        // 计数器
        CountDownLatch countDownLatch = new CountDownLatch(6);
        for (int i = 1; i <= 6; i++) {
            new Thread(() -> {
                System.out.println(Thread.currentThread().getName() + "\tStart");
                countDownLatch.countDown(); // 计数器-1
            }, String.valueOf(i)).start();
        }
        //阻塞等待计数器归零
        countDownLatch.await();
        System.out.println(Thread.currentThread().getName() + "\tEnd");
    }
    
}
```



CountDownLatch 主要有两个方法，当一个或多个线程调用 `await` 方法时，这些线程会阻塞

其他线程调用`CountDown()`方法会将计数器减1（调用CountDown方法的线程不会阻塞）

当计数器变为0时，await 方法阻塞的线程会被唤醒，继续执行



### CyclicBarrier

翻译：CyclicBarrier 篱栅

作用：和上面的减法相反，这里是加法，好比集齐7个龙珠召唤神龙，或者人到齐了再开会！

```java
public class CyclicBarrierDemo {
    public static void main(String[] args) {
        // CyclicBarrier(int parties, Runnable barrierAction)
        CyclicBarrier cyclicBarrier = new CyclicBarrier(7, () -> {
            System.out.println("召唤神龙成功");
        });

        for (int i = 1; i <= 7; i++) {
            final int tempInt = i;
            new Thread(() -> {
                System.out.println(Thread.currentThread().getName() + 
                        "收集了第" + tempInt + "颗龙珠");

                try {
                    cyclicBarrier.await(); // 等待
                } catch (InterruptedException e) {
                    e.printStackTrace();
                } catch (BrokenBarrierException e) {
                    e.printStackTrace();
                }

            }).start();
        }
    }
}
```



### Semaphore

翻译：Semaphore 信号量;信号灯;信号

举个“抢车位”的例子

```java
public class SemaphoreDemo {
    public static void main(String[] args) {
        // 模拟资源类，有3个空车位
        Semaphore semaphore = new Semaphore(3);
        for (int i = 1; i <= 6; i++) { // 模拟6个车
            new Thread(() -> {
                try {
                    semaphore.acquire(); // acquire 得到
                    System.out.println(Thread.currentThread().getName() + " 抢到了车位");
                    TimeUnit.SECONDS.sleep(3); // 停3秒钟
                    System.out.println(Thread.currentThread().getName() + " 离开了车位");
                } catch (InterruptedException e) {
                    e.printStackTrace();
                } finally {
                    semaphore.release(); // 释放这个位置
                }
            }, String.valueOf(i)).start();
        }

    }
}
```

在信号量上我们定义两种操作：

- acquire（获取）

  当一个线程调用 acquire 操作时，他要么通过成功获取信号量（信号量-1）

  要么一直等下去，直到有线程释放信号量，或超时

- release （释放）

  会将信号量的值 + 1，然后唤醒等待的线程

  

信号量主要用于两个目的：一个是用于多个共享资源的互斥使用，另一个用于并发线程数的控制。

## 8、读写锁

**ReadWriteLock**

独占锁（写锁）：指该锁一次只能被一个线程锁持有。对于ReentranrLock和 Synchronized 而言都是独占锁。

共享锁（读锁）：该锁可被多个线程所持有。

对于ReentrantReadWriteLock其读锁时共享锁，写锁是独占锁，读锁的共享锁可保证并发读是非常高效的。

```java
public class ReadWriteLockDemo {
    /**
     * 多个线程同时读一个资源类没有任何问题，所以为了满足并发量，读取共享资源应该可以同时进行。
     * 但是，如果有一个线程想去写共享资源，就不应该再有其他线程可以对该资源进行读或写。
     * 1. 读-读 可以共存
     * 2. 读-写 不能共存
     * 3. 写-写 不能共存
     */
    public static void main(String[] args) {
        MyCacheLock myCache = new MyCacheLock();
        // 写
        for (int i = 1; i <= 5; i++) {
            final int tempInt = i;
            new Thread(() -> {
                myCache.put(tempInt + "", tempInt + "");
            }, String.valueOf(i)).start();
        }

        // 读
        for (int i = 1; i <= 5; i++) {
            final int tempInt = i;
            new Thread(() -> {
                myCache.get(tempInt + "");
            }, String.valueOf(i)).start();
        }
    }

}

// 测试发现问题: 写入的时候，还没写入完成，会存在其他的写入！造成问题
class MyCache {
    private volatile Map<String, Object> map = new HashMap<>();

    public void put(String key, Object value) {
        System.out.println(Thread.currentThread().getName() + " 写入" + key);
        map.put(key, value);
        System.out.println(Thread.currentThread().getName() + " 写入成功!");
    }

    public void get(String key) {
        System.out.println(Thread.currentThread().getName() + " 读取" + key);
        Object result = map.get(key);
        System.out.println(Thread.currentThread().getName() + " 读取结果：" + result);
    }
}

// 加锁
class MyCacheLock {
    private volatile Map<String, Object> map = new HashMap<>();
    private ReadWriteLock readWriteLock = new ReentrantReadWriteLock(); // 读写锁

    public void put(String key, Object value) {
        // 写锁
        readWriteLock.writeLock().lock();
        try {
            System.out.println(Thread.currentThread().getName() + " 写入" + key);
            map.put(key, value);
            System.out.println(Thread.currentThread().getName() + " 写入成功!");
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            //解锁
            readWriteLock.writeLock().unlock();
        }
    }

    public void get(String key) {
        // 读锁
        readWriteLock.readLock().lock();
        try {
            System.out.println(Thread.currentThread().getName() + " 读取" + key);
            Object result = map.get(key);
            System.out.println(Thread.currentThread().getName() + " 读取结果：" + result);
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            readWriteLock.readLock().unlock();
        }
    }
}
```

## 9、阻塞队列

```java
Interface  BlockingQueue<E>
```

### 阻塞队列简介

阻塞：必须要阻塞、不得不阻塞

阻塞队列是一个队列，在数据结构中起的作用如下图：

![image-20210517173258323](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/image-20210517173258323.png)

当队列是空的，从队列中**获取**元素的操作将会被阻塞。

当队列是满的，从队列中**添加**元素的操作将会被阻塞。

试图从空的队列中获取元素的线程将会被阻塞，直到其他线程往空的队列插入新的元素。

试图向已满的队列中添加新元素的线程将会被阻塞，直到其他线程从队列中移除一个或多个元素或者完全清空，使队列变得空闲起来并后续新增。

### 阻塞队列的用处

在多线程领域：所谓阻塞，在某些情况下会挂起线程（即阻塞），一旦条件满足，被挂起的线程又会自 动被唤起。

为什么需要 BlockingQueue？

好处是我们不需要关心什么时候需要阻塞线程，什么时候需要唤醒线程，因为这一切BlockingQueue 都 给你一手包办了。

在 concurrent 包发布以前，在多线程环境下，我们每个程序员都必须自己去控制这些细节，尤其还要兼顾效率和线程安全，而这会给我们的程序带来不小的复杂度。

### 接口架构图

![image-20210517173544418](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/image-20210517173544418.png)

- ArrayBlockingQueue

  由数组结构组成的有界阻塞队列。

- LinkedBlockingQueue

  由链表结构组成的有界（默认值为：integer.MAX_VALUE）阻塞队列。

- PriorityBlockingQueue

  支持优先级排序的无界阻塞队列

- DelayQueue

  使用优先级队列实现的延迟无界阻塞队列。

- SynchronousQueue

  不存储元素的阻塞队列，也即单个元素的队列。

- LinkedTransferQueue

  由链表组成的无界阻塞队列

- LinkedBlockingDeque

  由链表组成的双向阻塞队列。

  

### API的使用

| 方法\处理方式 | 抛出异常  | 返回特殊值 | 一直阻塞 | 超时退出           |
| ------------- | --------- | ---------- | -------- | ------------------ |
| 插入方法      | add(e)    | offer(e)   | put(e)   | offer(e,time,unit) |
| 移除方法      | remove()  | poll()     | take()   | poll(time,unit)    |
| 检查方法      | element() | peek()     | 不可用   | 不可用             |

解释：

- 抛出异常

当阻塞队列满时，再往队列里add插入元素会抛出 `IllegalStateException: Queue full`

当阻塞队列空时，再往队列里remove移除元素会抛 NoSuchElementException` 

- 返回特殊值

插入方法，成功返回true，失败则false

移除方法，成功返回队列元素，队列里没有则返回null

- 一直阻塞

当阻塞队列满时，生产者线程继续往队列里put元素，队列会一直阻塞生产者线程直到put数据或响应中断退出

当阻塞队列空时，消费者线程从队列里take元素，队列会一直阻塞消费者线程直到队列可用

- 超时退出

当阻塞队列满时，队列会阻塞生产者线程一定时间，超过限时后生产者线程会退出



**抛出异常**

```java
package com.oddfar.bq;

import java.util.concurrent.ArrayBlockingQueue;

/**
 * @author zhiyuan
 */
public class BlockingQueueDemo {

    public static void main(String[] args) {
        // 队列大小
        ArrayBlockingQueue blockingQueue = new ArrayBlockingQueue<>(3);
        System.out.println(blockingQueue.add("a"));
        System.out.println(blockingQueue.add("b"));
        System.out.println(blockingQueue.add("c"));

        //java.lang.IllegalStateException: Queue full
//        System.out.println(blockingQueue.add("d"));

        System.out.println("首元素：" + blockingQueue.element()); // 检测队列队首元素！
        // public E remove() 返回值E，就是移除的值
        System.out.println(blockingQueue.remove()); //a
        System.out.println(blockingQueue.remove()); //b
        System.out.println(blockingQueue.remove()); //c
        // java.util.NoSuchElementException
//        System.out.println(blockingQueue.remove());

    }
}
```

**返回特殊值**

```java
public class BlockingQueueDemo2 {
    public static void main(String[] args) {
        // 队列大小
        ArrayBlockingQueue blockingQueue = new ArrayBlockingQueue<>(3);

        System.out.println(blockingQueue.offer("a")); // true
        System.out.println(blockingQueue.offer("b")); // true
        System.out.println(blockingQueue.offer("c")); // true
        //System.out.println(blockingQueue.offer("d")); // false

        System.out.println("首元素：" + blockingQueue.peek()); // 检测队列队首元素！

        // public E poll()
        System.out.println(blockingQueue.poll()); // a
        System.out.println(blockingQueue.poll()); // b
        System.out.println(blockingQueue.poll()); // c
        System.out.println(blockingQueue.poll()); // null
    }
}
```

**一直阻塞**

```java
public class BlockingQueueDemo3 {
    public static void main(String[] args) throws InterruptedException {
        // 队列大小
        ArrayBlockingQueue blockingQueue = new ArrayBlockingQueue<>(3);

        // 一直阻塞
        blockingQueue.put("a");
        blockingQueue.put("b");
        blockingQueue.put("c");
//         blockingQueue.put("d");
        System.out.println(blockingQueue.take()); // a
        System.out.println(blockingQueue.take()); // b
        System.out.println(blockingQueue.take()); // c
        System.out.println(blockingQueue.take()); // 阻塞不停止等待
    }
}
```

**超时退出**

```java
public class BlockingQueueDemo4 {
    public static void main(String[] args) throws InterruptedException {
        // 队列大小
        ArrayBlockingQueue blockingQueue = new ArrayBlockingQueue<>(3);

        // 一直阻塞
        blockingQueue.put("a");
        blockingQueue.put("b");
        blockingQueue.put("c");
        blockingQueue.offer("d",2L, TimeUnit.SECONDS); // 等待2秒超时退出

        System.out.println(blockingQueue.take()); // a
        System.out.println(blockingQueue.take()); // b
        System.out.println(blockingQueue.take()); // c
        System.out.println(blockingQueue.take()); // 阻塞不停止等待
    }
}
```

## 11、线程池

::: tip 池化技术

:::

程序的运行，其本质上，是对系统资源(CPU、内存、磁盘、网络等等)的使用。如何高效的使用这些资源 是我们编程优化演进的一个方向。今天说的线程池就是一种对CPU利用的优化手段。

通过学习线程池原理，明白所有池化技术的基本设计思路。遇到其他相似问题可以解决。

前面提到一个名词——**池化技术**，那么到底什么是池化技术呢 ?

池化技术简单点来说，就是提前保存大量的资源，以备不时之需。在机器资源有限的情况下，使用池化 技术可以大大的提高资源的利用率，提升性能等。

在编程领域，比较典型的池化技术有：**线程池、连接池、内存池、对象池等。**

我们通过创建一个线程对象，并且实现Runnable接口就可以实现一个简单的线程。可以利用上多核 CPU。当一个任务结束，当前线程就接收。

但很多时候，我们不止会执行一个任务。如果每次都是如此的创建线程->执行任务->销毁线程，会造成很大的性能开销。

那能否一个线程创建后，执行完一个任务后，又去执行另一个任务，而不是销毁。这就是线程池。

这也就是池化技术的思想，通过预先创建好多个线程，放在池中，这样可以在需要使用线程的时候直接获取，避免多次重复创建、销毁带来的开销。

::: tip 为什么使用线程池

:::

10 年前单核CPU电脑，假的多线程，像马戏团小丑玩多个球 ，CPU 需要来回切换。

现在是多核电脑，多个线程各自跑在独立的CPU上，不用切换效率高。

**线程池的优势：**

线程池做的工作主要是：控制运行的线程数量，处理过程中将任务放入队列，然后在线程创建后启动这 些任务，如果线程数量超过了最大数量，超出数量的线程排队等候，等其他线程执行完毕，再从队列中取出任务来执行。

**它的主要特点为：线程复用，控制最大并发数，管理线程。**

第一：降低资源消耗，通过重复利用已创建的线程降低线程创建和销毁造成的消耗。

第二：提高响应速度。当任务到达时，任务可以不需要等待线程创建就能立即执行。

第三：提高线程的可管理性，线程是稀缺资源，如果无限制的创建，不仅会消耗系统资源，还会降低系统的稳定性，使用线程池可以进行统一分配，调优和监控。



### ExecutorService



::: tip 线程池的三大方法

:::

Java中的线程池是通过 Executor 框架实现的，该框架中用到了 Executor ，Executors， ExecutorService，ThreadPoolExecutor 这几个类。

![JUC-00000021](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000021.png)

三大方法说明：

- `Executors.newFixedThreadPool(int)`

  执行长期任务性能好，创建一个线程池，一池有N个固定的线程，有固定线程数的线程。

  

- `Executors.newSingleThreadExecutor()`

  只有一个线程

- `Executors.newCachedThreadPool()`

  执行很多短期异步任务，线程池根据需要创建新线程，但在先构建的线程可用时将重用他们。 可扩容，遇强则强



```java
public class MyThreadPoolDemo {
    public static void main(String[] args) {
        /** 1、池子大小 5 
         * 模拟有10个顾客过来银行办理业务，池子中只有5个工作人员受理业务
         */
//        ExecutorService threadPool = Executors.newFixedThreadPool(5);


        /** 2、有且只有一个固定的线程
         * 模拟有10个顾客过来银行办理业务，池子中只有1个工作人员受理业务
         */
//        ExecutorService threadPool =  Executors.newSingleThreadExecutor();
        
        /**  3、一池N线程，可扩容伸缩
         * 模拟有10个顾客过来银行办理业务，池子中N个工作人员受理业务
         */
        ExecutorService threadPool = Executors.newCachedThreadPool();
        
        try {
            for (int i = 1; i <= 10; i++) {
                threadPool.execute(() -> {
                    System.out.println(Thread.currentThread().getName() + " 办理业务");
                });
            }
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            threadPool.shutdown(); // 用完记得关闭
        }
    }

}
```



### ThreadPoolExecutor



::: tip ThreadPoolExecutor 七大参数

:::

查看三大方法的调用源码，发现本质都是调用了 new ThreadPoolExecutor ( 7 大参数 )

```java
public ThreadPoolExecutor(int corePoolSize,
                          int maximumPoolSize,
                          long keepAliveTime,
                          TimeUnit unit,
                          BlockingQueue<Runnable> workQueue,
                          ThreadFactory threadFactory,
                          RejectedExecutionHandler handler) {

}
```

1、`corePollSize`

核心线程数。在创建了线程池后，线程中没有任何线程，等到有任务到来时才创建线程去执行任务。默认情况下，在创建了线程池后，线程池中的线程数为0，当有任务来之后，就会创建一个线程去执行任务，当线程池中的线程数目达到 corePoolSize 后，就会把到达的任务放到缓存队列当中。

2、`maximumPoolSize`

最大线程数。表明线程中最多能够创建的线程数量，此值必须大于等于1。

3、`keepAliveTime`

空闲的线程保留的时间，达到这个时间后，自动释放

4、`TimeUnit`

空闲线程的保留时间单位。

```java
TimeUnit.DAYS; //天
TimeUnit.HOURS; //小时
TimeUnit.MINUTES; //分钟
TimeUnit.SECONDS; //秒
TimeUnit.MILLISECONDS; //毫秒
TimeUnit.MICROSECONDS; //微妙
TimeUnit.NANOSECONDS; //纳秒
```

5、`BlockingQueue<Runnable> workQueue`

阻塞队列，存储等待执行的任务。参数有ArrayBlockingQueue、 LinkedBlockingQueue、SynchronousQueue可选。

6、`ThreadFactory`

线程工厂，用来创建线程，一般默认即可

7、`RejectedExecutionHandler`

队列已满，而且任务量大于最大线程的异常处理策略。有以下取值

```java
ThreadPoolExecutor.AbortPolicy:丢弃任务并抛出RejectedExecutionException异常。
ThreadPoolExecutor.DiscardPolicy：也是丢弃任务，但是不抛出异常。
ThreadPoolExecutor.DiscardOldestPolicy：丢弃队列最前面的任务，然后重新尝试执行任务（重复此过程）
ThreadPoolExecutor.CallerRunsPolicy：由调用线程处理该任务
```

::: tip ThreadPoolExecutor层工作原理

:::

![JUC-00000022](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000022.png)

举例：8个人进银行办理业务

1、1~2人被受理（核心大小core） 

2、3~5人进入队列（Queue） 

3、6~8人到最大线程池（扩容大小max） 

4、再有人进来就要被拒绝策略接受了

![JUC-00000023](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000023.png)

1、在创建了线程池后，开始等待请求。

2、当调用execute()方法添加一个请求任务时，线程池会做出如下判断：

- 如果正在运行的线程数量小于corePoolSize，那么马上创建线程运行这个任务
- 如果正在运行的线程数量大于或等于corePoolSize，那么将这个任务放入队列
- 如果这个时候队列满了且正在运行的线程数量还小于maximumPoolSize，那么还是要创建非 核心线程立刻运行这个任务
- 如果队列满了且正在运行的线程数量大于或等于1Size，那么线程池会启动饱和拒绝策略来执行。

3、当一个线程完成任务时，它会从队列中取下一个任务来执行

4、 当一个线程无事可做超过一定的时间(keepAliveTime)时，线程会判断：

如果当前运行的线程数大于corePollSize，那么这个线程就被停掉。

所以线程池的所有任务完成后，它最终会收缩到 corePoolSize 的大小。



::: tip 线程池用哪个？生产中如何设置合理参数

:::

Executors 中 JDK 已经给你提供了，为什么不用？

![JUC-00000024](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000024.png)

::: note 代码测试：

:::

线程池的拒绝策略：

```java
RejectedExecutionHandler rejected = null;

//默认，队列满了丢任务，抛出异常
rejected = new ThreadPoolExecutor.AbortPolicy();
//队列满了丢任务，不抛出异常【如果允许任务丢失这是最好的】
rejected = new ThreadPoolExecutor.DiscardPolicy();
//将最早进入队列的任务删，之后再尝试加入队列
rejected = new ThreadPoolExecutor.DiscardOldestPolicy();
////如果添加到线程池失败，那么主线程会自己去执行该任务，回退
rejected = new ThreadPoolExecutor.CallerRunsPolicy();
```





```java
public class MyThreadPoolDemo2 {

    public static void main(String[] args) {


        // 自定义 ThreadPoolExecutor
        ExecutorService threadPool = new ThreadPoolExecutor(
                2,
                Runtime.getRuntime().availableProcessors(),
                2L,
                TimeUnit.SECONDS,
                new LinkedBlockingDeque<>(3),
                Executors.defaultThreadFactory(),
                new ThreadPoolExecutor.DiscardPolicy());
        try {
            // 模拟有6,7,8,9,10个顾客过来银行办理业务，观察结果情况
            // 最大容量为：maximumPoolSize + workQueue = 最大容量数
            for (int i = 1; i <= 19; i++) {
                int num = i;
                threadPool.execute(() -> {
                    System.out.println(num + " " + Thread.currentThread().getName() + " ok");
                });
            }
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            threadPool.shutdown(); // 用完记得关闭
        }

    }
}
```

**线程是否越多越好？**

一个计算为主的程序（专业一点称为**CPU密集型程序**）。多线程跑的时候，可以充分利用起所有的 cpu 核心，比如说4个核心的cpu，开4个线程的时候，可以同时跑4个线程的运算任务，此时是最大效率。但是如果线程远远超出cpu核心数量反而会使得任务效率下降，因为频繁的切换线程也是要消耗时间的。因此对于cpu密集型的任务来说，线程数等于cpu数是最好的了。

如果是一个磁盘或网络为主的程序（**IO密集型**）。一个线程处在IO等待的时候，另一个线程还可以在 CPU里面跑，有时候CPU闲着没事干，所有的线程都在等着IO，这时候他们就是同时的了，而单线程的话此时还是在一个一个等待的。我们都知道IO的速度比起CPU来是慢到令人发指的。所以开多线程，比 方说多线程网络传输，多线程往不同的目录写文件，等等。此时线程数等于IO任务数是最佳的。



## 12、四大函数式接口

在java.util.function包下，Java 内置核心四大函数式接口，可以使用lambda表达式

![JUC-00000025](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000025.png)

::: note 函数型接口，有一个输入，有一个输出

:::

Function

```java
package com.oddfar.function;

import java.util.function.Function;

/**
 * @author zhiyuan
 */
public class Demo01 {
    public static void main(String[] args) {
//        Function<String,Integer> function = new Function<String,Integer>() {
//            @Override
//            public Integer apply(String s) {
//                return s.length();
//            }
//        };

        Function<String,Integer> function = (s)->{return  s.length();};

        System.out.println(function.apply("abc"));
    }
}
```



::: note 断定型接口，有一个输入参数，返回只有布尔值。

:::

Predicate

```java
public class Demo02 {
    public static void main(String[] args) {
//        Predicate<String> predicate = new Predicate<String>() {
//            @Override
//            public boolean test(String s) {
//                return s.isEmpty();
//            }
//        };
        Predicate<String> predicate = (s)->{return s.isEmpty();};

        System.out.println(predicate.test("abc"));

    }
}
```



::: note 消费型接口，有一个输入参数，没有返回值

:::

Consumer

```java
public class Demo03 {
    public static void main(String[] args) {

//        Consumer<String> consumer = new Consumer<String>() {
//            @Override
//            public void accept(String s) {
//                System.out.println(s);
//            }
//        };
        Consumer<String> consumer = s -> { System.out.println(s); };
        consumer.accept("abc");
    }

}
```

::: note 供给型接口，没有输入参数，只有返回参数

:::

Supplier

```java
public class Demo04 {
    public static void main(String[] args) {
//        Supplier<String> supplier = new Supplier<String>() {
//            @Override
//            public String get() {
//                return null;
//            }
//        };
        Supplier<String> supplier = () -> { return "abc";};
        System.out.println(supplier.get());
    }

}
```

## 13、Stream流式计算

::: tip 流（Stream）到底是什么呢？

:::



是数据渠道，用于操作数据源（集合、数组等）所生成的元素序列。

“集合讲的是数据，流讲的是计算！”

特点：

- Stream 自己不会存储元素

- Stream 不会改变源对象，相反，他们会返回一个持有结果的新Stream。
- Stream 操作是延迟执行的。这意味着他们会等到需要结果的时候才执行。

![JUC-00000027](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000027.png)

::: note 代码举例

:::

User实体类

```java
public class User {
    private int id;
    private String userName;
    private int age;
    //get、set、有参/无参构造器、toString
}
```

Stream算法题

```java
package com.oddfar.stream;

import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;

/**
 * 题目：请按照给出数据，找出同时满足以下条件的用户
 * 也即以下条件：
 * 1、全部满足偶数ID
 * 2、年龄大于24
 * 3、用户名转为大写
 * 4、用户名字母倒排序
 * 5、只输出一个用户名字 limit
 */
public class StreamDemo {
    public static void main(String[] args) {
        User u1 = new User(11, "a", 23);
        User u2 = new User(12, "b", 24);
        User u3 = new User(13, "c", 22);
        User u4 = new User(14, "d", 28);
        User u5 = new User(16, "e", 26);
        List<User> list = Arrays.asList(u1, u2, u3, u4, u5);

        /**
         * 1. 首先我们需要将 list 转化为stream流
         * 2. 然后将用户过滤出来，这里用到一个函数式接口 Predicate<? super T>，我们可以使用lambda表达式简化
         * 3. 这里面传递的参数，就是Stream流的泛型类型，也就是User，所以，这里可以直接返回用户id为偶数的用户信息;
         * 4. 通过forEach进行遍历，直接简化输出 System.out::println
         */
        list.stream()
                .filter(u -> {
                    return u.getId() % 2 == 0;
                })
                .filter(u -> {
                    return u.getAge() > 24;
                })
                .map(u -> {
                    return u.getUserName().toUpperCase();
                })
                //.sorted() //默认正排序 自己用 compareTo 比较
                .sorted((o1, o2) -> {
                    return o2.compareTo(o1);
                })
                .limit(1)
                .forEach(System.out::println);


        // map解释：
        List<Integer> list2 = Arrays.asList(1, 2, 3);
        list2 = list2.stream().map(x -> {
            return x * 2;
        }).collect(Collectors.toList());

        for (Integer element : list2) {
            System.out.println(element);
        }
        
    }

}
```

## 14、分支合并

::: tip 什么是ForkJoin

:::

从JDK1.7开始，Java提供 Fork/Join 框架用于并行执行任务，它的思想就是讲一个大任务分割成若干小任务，最终汇总每个小任务的结果得到这个大任务的结果。

这种思想和MapReduce很像（input --> split --> map --> reduce --> output）

主要有两步：

- 第一、任务切分
- 第二、结果合并

![JUC-00000028](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000028.png)

它的模型大致是这样的：线程池中的每个线程都有自己的工作队列

（PS：这一点和ThreadPoolExecutor 不同，ThreadPoolExecutor是所有线程公用一个工作队列，所有线程都从这个工作队列中取任务）

当 自己队列中的任务都完成以后，会从其它线程的工作队列中偷一个任务执行，这样可以充分利用资源。

::: tip 工作窃取

:::

另外，forkjoin有一个工作窃取的概念。简单理解，就是一个工作线程下会维护一个包含多个子任务的双端队列。而对于每个工作线程来说，会从头部到尾部依次执行任务。这时，总会有一些线程执行的速度较快，很快就把所有任务消耗完了。那这个时候怎么办呢，总不能空等着吧，多浪费资源啊。

工作窃取（work-stealing）算法是指某个线程从其他队列里窃取任务来执行。工作窃取的运行流程图如下：

![JUC-00000029](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000029.png)

那么为什么需要使用工作窃取算法呢？

假如我们需要做一个比较大的任务，我们可以把这个任务分割为若干互不依赖的子任务，为了减少线程间的竞争，于是把这些子任务分别放到不同的队列里，并为每个队列创建一个单独的线程来执行队列里的任务，线程和队列一一对应，比如A线程负责处理A队列里的任务。但是有的线程会先把自己队列里的任务干完，而其他线程对应的队列里还有任务等待处理。干完活的线程与其等着，不如去帮其他线程干活，于是它就去其他线程的队列里窃取一个任务来执行。而在这时它们会访问同一个队列，所以为了减少窃取任务线程和被窃取任务线程之间的竞争，通常会使用双端队列，被窃取任务线程永远从双端队列的头部拿任务执行，而窃取任务的线程永远从双端队列的尾部拿任务执行。

工作窃取算法的优点是充分利用线程进行并行计算，并减少了线程间的竞争，其缺点是在某些情况下还是存在竞争，比如双端队列里只有一个任务时。并且消耗了更多的系统资源，比如创建多个线程和多个双端队列。

于是，先做完任务的工作线程会从其他未完成任务的线程尾部依次获取任务去执行。这样就可以充分利用CPU的资源。这个非常好理解，就比如有个妹子程序员做任务比较慢，那么其他猿就可以帮她分担一 些任务，这简直是双赢的局面啊，妹子开心了，你也开心了。

::: tip 核心类

:::

**1、ForkJoinPool**

WorkQueue是一个ForkJoinPool中的内部类，它是线程池中线程的工作队列的一个封装，支持任务窃取。

什么叫线程的任务窃取呢？就是说你和你的一个伙伴一起吃水果，你的那份吃完了，他那份没吃完，那你就偷偷的拿了他的一些水果吃了。存在执行2个任务的子线程，这里要讲成存在A，B两个了。

WorkQueue在执行任务，A的任务执行完了，B的任务没执行完，那么A的WorkQueue就从B的 WorkQueue的ForkJoinTask数组中拿走了一部分尾部的任务来执行，可以合理的提高运行和计算效率。

每个线程都有一个WorkQueue，而WorkQueue中有执行任务的线程（ForkJoinWorkerThread owner），还有这个线程需要处理的任务（ForkJoinTask<?>[] array）。那么这个新提交的任务就是加到array中。

**2、ForkJoinTask**

ForkJoinTask代表运行在ForkJoinPool中的任务。

主要方法：

- fork() 在当前线程运行的线程池中安排一个异步执行。简单的理解就是再创建一个子任务
- join() 当任务完成的时候返回计算结果。
- invoke() 开始执行任务，如果必要，等待计算完成。

子类： **Recursive ：递归**

- RecursiveAction 一个递归无结果的ForkJoinTask（没有返回值）
- RecursiveTask 一个递归有结果的ForkJoinTask（有返回值）



::: note 代码测试

:::

核心代码：

```java
package com.oddfar.forkJoin;

import java.util.concurrent.RecursiveTask;

/**
 * @author zhiyuan
 */
public class ForkJoinWork extends RecursiveTask<Long> {

    private Long start;//起始值
    private Long end;//结束值
    public static final Long critical = 10000L;//临界值

    public ForkJoinWork(Long start, Long end) {
        this.start = start;
        this.end = end;
    }

    @Override
    protected Long compute() {
        //判断是否是拆分完毕
        Long lenth = end - start;
        if (lenth <= critical) {
            //如果拆分完毕就相加
            Long sum = 0L;
            for (Long i = start; i <= end; i++) {
                sum += i;
            }
            return sum;
        } else {
            //没有拆分完毕就开始拆分
            Long middle = (end + start) / 2;//计算的两个值的中间值
            ForkJoinWork right = new ForkJoinWork(start, middle);
            right.fork();//拆分，并压入线程队列
            ForkJoinWork left = new ForkJoinWork(middle + 1, end);
            left.fork();//拆分，并压入线程队列

            //合并
            return right.join() + left.join();
        }
    }
}
```



三种测试：

```java
package com.oddfar.forkJoin;

import java.util.concurrent.ExecutionException;
import java.util.concurrent.ForkJoinPool;
import java.util.concurrent.ForkJoinTask;
import java.util.stream.LongStream;

/**
 * @author zhiyuan
 */
public class ForkJoinWorkDemo {
    public static void main(String[] args) throws ExecutionException, InterruptedException {
        test1();//  15016
        test2();//  14694
        test3();//  216

    }

    // forkjoin这个框架针对的是大任务执行，效率才会明显的看出来有提升，于是我把总数调大到20亿。
    public static void test1() throws ExecutionException, InterruptedException {

        //ForkJoin实现
        long l = System.currentTimeMillis();

        ForkJoinPool forkJoinPool = new ForkJoinPool();//实现ForkJoin 就必须有ForkJoinPool的支持
        ForkJoinTask<Long> task = new ForkJoinWork(0L, 2000000000L);//参数为起始值与结束值
        ForkJoinTask<Long> result = forkJoinPool.submit(task);
        Long aLong = result.get();

        long l1 = System.currentTimeMillis();
        System.out.println("invoke = " + aLong + " time: " + (l1 - l));

    }


    public static void test2() {
        //普通线程实现
        Long x = 0L;
        Long y = 20_0000_0000L;
        long start_time = System.currentTimeMillis();
        for (Long i = 0L; i <= y; i++) {
            x += i;
        }
        long end_time = System.currentTimeMillis();
        System.out.println("invoke = " + x + " time: " + (end_time - start_time));

    }

    public static void test3() {
        //Java 8 并行流的实现
        long l = System.currentTimeMillis();

        long reduce = LongStream.rangeClosed(0, 2000000000L).parallel().reduce(0, Long::sum);

        long l1 = System.currentTimeMillis();
        System.out.println("invoke = " + reduce + " time: " + (l1 - l));
    }
}
```



打个比方，假设一个酒店有400个房间，一共有4名清洁工，每个工人每天可以打扫100个房间，这样，4 个工人满负荷工作时，400个房间全部打扫完正好需要1天。

Fork/Join的工作模式就像这样：首先，工人甲被分配了400个房间的任务，他一看任务太多了自己一个 人不行，所以先把400个房间拆成两个200，然后叫来乙，把其中一个200分给乙。紧接着，甲和乙再发现200也是个大任务，于是甲继续把200分成两个100，并把其中一个100分给丙， 类似的，乙会把其中一个100分给丁，这样，最终4个人每人分到100个房间，并发执行正好是1天。



## 15、异步回调

::: tip 概述

:::

Future设计的初衷：对将来某个时刻会发生的结果进行建模。

当我们需要调用一个函数方法时。如果这个函数执行很慢，那么我们就要进行等待。但有时候，我们可能并不急着要结果。因此,我们可以让被调用者立即返回,让他在后台慢慢处理这个请求。对于调用者来说,则可以先处理一些其他任务,在真正需要数据的场合再去尝试获取需要的数据。

它建模了一种异步计算，返回一个执行运算结果的引用，当运算结束后，这个引用被返回给调用方。在 Future 中出发那些潜在耗时的操作把调用线程解放出来，让它能继续执行其他有价值的工作，不再需要等待耗时的操作完成。

**Future的优点：**比更底层的Thread更易用。要使用Future，通常只需要将耗时的操作封装在一个 Callable对象中，再将它提交给ExecutorService。

为了让程序更加高效，让CPU最大效率的工作，我们会采用异步编程。首先想到的是开启一个新的线程去做某项工作。再进一步，为了让新线程可以返回一个值，告诉主线程事情做完了，于是乎 Future 粉墨登场。然而Future提供的方式是主线程主动问询新线程，要是有个回调函数就爽了。所以，为了满足 Future的某些遗憾，强大的CompletableFuture 随着Java8一起来了。

![JUC-00000030](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000030.png)

::: tip 实例

:::

没有返回值的 runAsync 异步调用

```java
package com.oddfar.future;

import java.util.concurrent.CompletableFuture;
import java.util.concurrent.TimeUnit;

/**
 * @author zhiyuan
 */
public class Demo01 {
    public static void main(String[] args) throws Exception {

        //没有返回值的 runAsync 异步调用
        CompletableFuture<Void> completableFuture = CompletableFuture.runAsync(
                () -> {
                    try {
                        TimeUnit.SECONDS.sleep(2);
                    } catch (InterruptedException e) {
                        e.printStackTrace();
                    }
                    int i = 1;
                    System.out.println(Thread.currentThread().getName() + " 没有返回");
                }
        );

        System.out.println("111111");
        completableFuture.get();
        System.out.println("222222");
    }
}
```



有返回值的 供给型参数接口

```java
public class Demo02 {
    public static void main(String[] args) throws Exception {
        CompletableFuture<Integer> completableFuture = CompletableFuture.supplyAsync(() -> {
                    System.out.println(Thread.currentThread().getName() + " 有返回值");
//                    int i = 10 / 0;
                    return 1024;
                }
        );

        Integer res = completableFuture.whenComplete((t, u) -> {
            //编译 完成，正常结束输出
            System.out.println("===t:" + t); //正常结果
            System.out.println("===u:" + u); //报错的信息
        }).exceptionally(e -> { //结果异常，非正常结束
            System.out.println("=======exception:" + e.getMessage());
            return 555;
        }).get();

        System.out.println(res);
    }


}
```

## 16、JMM

- **请你谈谈你对 volatile 的理解**

volitile 是 Java 虚拟机提供的轻量级的同步机制，三大特性：

1、保证可见性 

2、不保证原子性 

3、禁止指令重排



::: tip 什么是JMM

:::



JMM 本身是一种抽象的概念，并不真实存在，它描述的是一组规则或者规范~

JMM 关于同步的规定： 

1、线程解锁前，必须把共享变量的值刷新回主内存 

2、线程加锁前，必须读取主内存的最新值到自己的工作内存 

3、加锁解锁是同一把锁



JMM即为 JAVA 内存模型（java memory model）。因为在不同的硬件生产商和不同的操作系统下，内存的访问逻辑有一定的差异，结果就是当你的代码在某个系统环境下运行良好，并且线程安全，但是换了个系统就出现各种问题。Java内存模型，就是为了屏蔽系统和硬件的差异，让一套代码在不同平台下能到达相同的访问结果。JMM从java 5开始的JSR-133发布后，已经成熟和完善起来。

JMM规定了内存主要划分为**主内存**和**工作内存**两种。此处的主内存和工作内存跟JVM内存划分（堆、 栈、方法区）是在不同的层次上进行的，如果非要对应起来，主内存对应的是Java堆中的对象实例部分，工作内存对应的是栈中的部分区域，从更底层的来说，主内存对应的是硬件的物理内存，工作内存对应的是寄存器和高速缓存。

![JUC-00000031](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000031.png)

JVM在设计时候考虑到，如果JAVA线程每次读取和写入变量都直接操作主内存，对性能影响比较大，所以每条线程拥有各自的工作内存，工作内存中的变量是主内存中的一份拷贝，线程对变量的读取和写入，直接在工作内存中操作，而不能直接去操作主内存中的变量。但是这样就会出现一个问题，当一个线程修改了自己工作内存中变量，对其他线程是不可见的，会导致线程不安全的问题。因此 JMM 制定了 一套标准来保证开发者在编写多线程程序的时候，能够控制什么时候内存会被同步给其他线程。



::: tip JMM的内存模型

:::

![JUC-00000032](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000032.png)

线程A感知不到线程B操作了值的变化！如何能够保证线程间可以同步感知这个问题呢？只需要使用 Volatile关键字即可！volatile 保证线程间变量的可见性，简单地说就是当线程A对变量X进行了修改后， 在线程A后面执行的其他线程能看到变量X的变动，更详细地说是要符合以下两个规则 ：

- 线程对变量进行修改之后，要立刻回写到主内存。
- 线程对变量读取的时候，要从主内存中读，而不是缓存。

各线程的工作内存间彼此独立，互不可见，在线程启动的时候，虚拟机为每个内存分配一块工作内存， 不仅包含了线程内部定义的局部变量，也包含了线程所需要使用的共享变量（非线程内构造的对象）的副本，即，为了提高执行效率。

**内存交互操作**

内存交互操作有8种，虚拟机实现必须保证每一个操作都是原子的，不可在分的（对于double和long类型的变量来说，load、store、read和write操作在某些平台上允许例外）

- lock （锁定）：作用于主内存的变量，把一个变量标识为线程独占状态
- unlock （解锁）：作用于主内存的变量，它把一个处于锁定状态的变量释放出来，释放后的变量才可以被其他线程锁定
- read （读取）：作用于主内存变量，它把一个变量的值从主内存传输到线程的工作内存中，以便随后的load动作使用
- load （载入）：作用于工作内存的变量，它把read操作从主存中变量放入工作内存中
- use （使用）：作用于工作内存中的变量，它把工作内存中的变量传输给执行引擎，每当虚拟机遇到一个需要使用到变量的值，就会使用到这个指令
- assign （赋值）：作用于工作内存中的变量，它把一个从执行引擎中接受到的值放入工作内存的变量副本中
- store （存储）：作用于主内存中的变量，它把一个从工作内存中一个变量的值传送到主内存中，以便后续的write使用
- write （写入）：作用于主内存中的变量，它把store操作从工作内存中得到的变量的值放入主内 存的变量中

**JMM对这八种指令的使用，制定了如下规则：**

- 不允许read和load、store和write操作之一单独出现。即：使用了read必须load，使用了store必须 write
- 不允许线程丢弃他最近的assign操作，即工作变量的数据改变了之后，必须告知主存
- 不允许一个线程将没有assign的数据从工作内存同步回主内存
- 一个新的变量必须在主内存中诞生，不允许工作内存直接使用一个未被初始化的变量。就是对变量实施use、store操作之前，必须经过assign和load操作
- 一个变量同一时间只有一个线程能对其进行lock。多次lock后，必须执行相同次数的unlock才能解锁
- 如果对一个变量进行lock操作，会清空所有工作内存中此变量的值，在执行引擎使用这个变量前， 必须重新load或assign操作初始化变量的值
- 如果一个变量没有被lock，就不能对其进行unlock操作。也不能unlock一个被其他线程锁住的变量
- 对一个变量进行unlock操作之前，必须把此变量同步回主内存

JMM对这八种操作规则和对volatile的一些特殊规则就能确定哪里操作是线程安全，哪些操作是线程不 安全的了。但是这些规则实在复杂，很难在实践中直接分析。所以一般我们也不会通过上述规则进行分 析。更多的时候，使用java的happen-before规则来进行分析。

- happens-before字面翻译过来就是先行发生，A happens-before B 就是A先行发生于B？

不准确！在Java内存模型中，happens-before 应该翻译成：前一个操作的结果可以被后续的操作获取。 讲白点就是前面一个操作把变量a赋值为1，那后面一个操作肯定能知道a已经变成了1。

我们再来看看为什么需要这几条规则？

因为我们现在电脑都是多CPU,并且都有缓存，导致多线程直接的可见性问题。

所以为了解决多线程的可见性问题，就搞出了happens-before原则，让线程之间遵守这些原则。编译器 还会优化我们的语句，所以等于是给了编译器优化的约束。不能让它优化的不知道东南西北了！

- 并发Bug的源头：<https://www.jianshu.com/p/e662bb611360>

## 17、volatile

volatile是不错的机制，但是也不能保证原子性。

- 代码验证可见性

```java
public class JMMVolatileDemo01 {
    /**
     * Volatile 用来保证数据的同步，也就是可见性
     * 不加 volatile 就没有可见性，会一直循环
     */
    private volatile static int num = 0;

    public static void main(String[] args) throws InterruptedException {

        new Thread(() -> {
            while (num == 0) {
            }
        }).start();

        Thread.sleep(1000);

        num = 1;
        System.out.println(num);
    }
}
```

- 验证 volatile 不保证原子性

原子性理解：不可分割，完整性，也就是某个线程正在做某个具体的业务的时候，中间不可以被加塞或者被分割，需要整体完整，要么同时成功，要么同时失败。

```java
public class JMMVolatileDemo02 {
    private volatile static int num = 0;

    public  static void add() {
        num++;
    }

    // 结果应该是 num 为 2万，测试看结果
    public static void main(String[] args) throws InterruptedException {
        for (int i = 1; i <= 20; i++) {
            new Thread(() -> {
                for (int j = 1; j <= 1000; j++) {
                    add();
                }
            }, String.valueOf(i)).start();
        }

        // 需要等待上面20个线程都全部计算完毕，看最终结果
        // 默认一个 main线程 一个 gc 线程
        while (Thread.activeCount() > 2) {
            Thread.yield();
        }
        System.out.println(Thread.currentThread().getName() + " " + num);
    }
}
```

为我们的 add 方法没有加锁，加了 volatile ，说明 volatile 不能保证原子性；

命令行查看底层字节码代码： `javap -c JMMVolatileDemo02.class`

![JUC-00000034](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000034.png)

num++ 在多线程下是非线程安全的，如何不加 synchronized解决？

查看原子包下的类![JUC-00000035](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000035.png)

```java
public class JMMVolatileDemo02 {
    private volatile static AtomicInteger num = new AtomicInteger();

    public static void add() {
        num.getAndIncrement(); // 等价 num++
    }

    // 结果应该是 num 为 2万，测试看结果
    public static void main(String[] args) throws InterruptedException {
        for (int i = 1; i <= 20; i++) {
            new Thread(() -> {
                for (int j = 1; j <= 1000; j++) {
                    add();
                }
            }, String.valueOf(i)).start();
        }

        // 需要等待上面20个线程都全部计算完毕，看最终结果
        // 默认一个 main线程 一个 gc 线程
        while (Thread.activeCount() > 2) {
            Thread.yield();
        }
        System.out.println(Thread.currentThread().getName() + " " + num);
    }
}
```



::: tip 指令重排

:::

计算机在执行程序时，为了提高性能，编译器和处理器的常常会对指令做重排



![JUC-00000036](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000036.png)

一般分以下3种问题：

​	单线程环境里面确保程序最终执行结果和代码顺序执行的结果一致。

​	处理器在进行重排序时必须要考虑指令之间的**数据依赖性**。

​	多线程环境中线程交替执行，由于编译器优化重排的存在，两个线程中使用的变量能否保证一致性是无法确定的，结果无法预测。



**指令重排是什么**

指令队列在CPU执行时不是串行的, 当某条指令执行时消耗较多时间时, CPU资源足够时并不会在此无意义的等待, 而是开启下一个指令. 开启下一条指令是有条件的, 即上一条指令和下一条指令不存在相关性. 例如下面这个例子:

```java
a /= 2;   // 指令A
a /= 2;   // 指令B
c++;      // 指令C
```



里的指令B是依赖于指令A的执行结果的, 在A处于执行阶段时, B会被阻塞, 直到A执行完成. 而指令C与A/B均没有依赖关系, 所以在A执行或者B执行的过程中, C会同时被执行, 那么C有可能在A+B的执行过程中就执行完毕了, 这样指令队列的实际执行顺序就是 C->A->B 或者 A->C->B.

![深入理解Java虚拟机 的相关讲解](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/20180413180415453)

**指令重排小结：**

volatile 实现了禁止指令重排优化，从而避免多线程环境下程序出现乱序执行的现象



先了解一个概念，内存屏障（Memory Barrier）又称内存栅栏，是一个CPU 指令，它的作用有两个：

1、保证特定操作的执行顺序。 

2、保证某些变量的内存可见性（利用该特性实现volatile的内存可见性）。



由于编译器和处理器都能执行指令重排优化。如果在指令间插入一条 Memory Barrier 则会告诉编译器和CPU，不管什么指令都不能和这条 Memory Barrier 指令重排序，也就是说，**通过插入内存屏障禁止在内存屏障前后的指令执行重排序优化**。内存屏障另外一个作用是强制刷出各种CPU的缓存数据，因此任何CPU上的线程都能读取到这些数据的最新版本。

![JUC-00000038](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000038.png)

经过，可见性，原子性，指令重排的话，线程安全性获得保证：

对于指令重排导致的可见性问题 和 有序性问题，可以利用 volatile 关键字解决，因为 volatile 的另外一 个作用就是禁止重排序优化。



## 18、单例模式



如何防止反射 破坏单例模式？

推荐阅读：[单例模式 | 菜鸟教程](https://www.runoob.com/design-pattern/singleton-pattern.html)



### 饿汉式



```java
public class Hungry {
    private Hungry() {
    }

    private final static Hungry hungry = new Hungry();

    public static Hungry getInstance() {
        return hungry;
    }
}
```

饿汉式是最简单的单例模式的写法，保证了线程的安全

但饿汉式会有一点小问题，看下面的代码：

```java
public class Hungry {
    private byte[] data1 = new byte[1024];
    private byte[] data2 = new byte[1024];
    private byte[] data3 = new byte[1024];
    private byte[] data4 = new byte[1024];
    
    private Hungry() {
    }

    private final static Hungry hungry = new Hungry();

    public static Hungry getInstance() {
        return hungry;
    }
}
```

在 Hungry 类中，我定义了四个byte数组，当代码一运行，这四个数组就被初始化，并且放入内存了，如果长时间没有用到getInstance方法，不需要Hungry类的对象，这不是一种浪费吗？我希望的是只有用 到了 getInstance 方法，才会去初始化单例类，才会加载单例类中的数据。所以就有了第二种单例模式：<mark>懒汉式</mark>

### 懒汉式

```java
public class LazyMan {
    private LazyMan() {
        System.out.println(Thread.currentThread().getName() + "Start");
    }

    private static LazyMan lazyMan;

    public static LazyMan getInstance() {
        if (lazyMan == null) {
            lazyMan = new LazyMan();
        }
        return lazyMan;
    }

    // 测试并发环境，发现单例失效
    public static void main(String[] args) {
        for (int i = 0; i < 10; i++) {
            new Thread(() -> {
                LazyMan.getInstance();
            }).start();
        }
    }

}
```

多加一层检测可以避免问题，也就是DCL懒汉式！

```java
public class LazyMan {
    private LazyMan() {
    }

    private static LazyMan lazyMan;

    public static LazyMan getInstance() {
        if (lazyMan == null) {
            synchronized (LazyMan.class) {
                if (lazyMan == null) {
                    lazyMan = new LazyMan();
                }
            }
        }
        return lazyMan;
    }
}
```

DCL懒汉式的单例，保证了线程的安全性，又符合了懒加载，只有在用到的时候，才会去初始化，调用 效率也比较高，但是这种写法在极端情况还是可能会有一定的问题。

因为 `lazyMan = new LazyMan();` 不是原子性操作，至少会经过三个步骤：

1. 分配对象内存空间
2. 执行构造方法初始化对象
3. 设置instance指向刚分配的内存地址，此时 instance ！=null；

由于指令重排，导致A线程执行 `lazyMan = new LazyMan();` 的时候，可能先执行了第三步（还没执行第 二步），由于线程调度，当线程B进来时，发现 lazyMan 已经不为空了，直接返回了lazyMan，并且后面使用了返回的lazyMan，由于线程A还没有执行第二步，导致此时lazyMan还不完整，可能会有一些意想不到的错误，所以就有了下面一种单例模式。

这种单例模式只是在上面DCL单例模式增加一个volatile关键字来避免指令重排：

```java
public class LazyMan {
    private LazyMan() {
    }

    private volatile static LazyMan lazyMan;

    public static LazyMan getInstance() {
        if (lazyMan == null) {
            synchronized (LazyMan.class) {
                if (lazyMan == null) {
                    lazyMan = new LazyMan();
                }
            }
        }
        return lazyMan;
    }
}
```



### 静态内部类

还有这种方式是第一种饿汉式的改进版本，同样也是在类中定义static变量的对象，并且直接初始化，不 过是移到了静态内部类中，十分巧妙。既保证了线程的安全性，同时又满足了懒加载。

```java
public class Holder {
    private Holder() {
    }

    public static Holder getInstance() {
        return InnerClass.holder;
    }

    private static class InnerClass {
        private static final Holder holder = new Holder();
    }
}
```



### 万恶的反射

万恶的反射登场了，反射是一个比较霸道的东西，无视private修饰的构造方法，可以直接在外面 newInstance，破坏我们辛辛苦苦写的单例模式。



```java
public class SingletonPatternDemo {
    public static void main(String[] args) throws Exception {
        LazyMan lazyMan1 = LazyMan.getInstance();

        Constructor<LazyMan> declaredConstructor = LazyMan.class.getDeclaredConstructor(null);
        declaredConstructor.setAccessible(true);
        LazyMan lazyMan2 = declaredConstructor.newInstance();
        
        System.out.println(lazyMan1.hashCode());
        System.out.println(lazyMan2.hashCode());
        
    }
}
```

我们分别打印出lazyMan1，lazyMan2的hashcode，发现不相等

那么，怎么解决这种问题呢？

在私有的构造函数中做一个判断，如果lazyMan不为空，说明lazyMan已经被创建过了，如果正常调用 getInstance方法，是不会出现这种事情的，所以直接抛出异常！

```java
public class LazyMan {
    private LazyMan() {
        synchronized (LazyMan.class) {
            if (lazyMan != null) {
                throw new RuntimeException("不要试图用反射破坏单例模式");
            }
        }
    }

    private static LazyMan lazyMan;

    public static LazyMan getInstance() {
        if (lazyMan == null) {
            synchronized (LazyMan.class) {
                if (lazyMan == null) {
                    lazyMan = new LazyMan();
                }
            }
        }
        return lazyMan;
    }
    
}
```

但是这种写法还是有问题：

​	上面我们是先正常的调用了getInstance方法，创建了LazyMan对象，所以第二次用反射创建对象，私有构造函数里面的判断起作用了，反射破坏单例模式失败。但是如果破坏者干脆不先调用getInstance方 法，一上来就直接用反射创建对象，我们的判断就不生效了：

那么如何防止这种反射破坏呢？

```java
public class LazyMan {
    private static boolean flag = false;

    private LazyMan() {
        synchronized (LazyMan.class) {
            if (flag == false) {
                flag = true;
            } else {
                throw new RuntimeException("不要试图用反射破坏单例模式");
            }
        }
    }

    private static LazyMan lazyMan;

    public static LazyMan getInstance() {
        if (lazyMan == null) {
            synchronized (LazyMan.class) {
                if (lazyMan == null) {
                    lazyMan = new LazyMan();
                }
            }
        }
        return lazyMan;
    }
    
}
```

在这里，我定义了一个boolean变量flag，初始值是false，私有构造函数里面做了一个判断，如果 flag=false，就把flag改为true，但是如果flag等于true，就说明有问题了，因为正常的调用是不会第二 次跑到私有构造方法的，所以抛出异常。

看起来很美好，但是还是不能完全防止反射破坏单例模式，因为可以利用反射修改flag的值。

```java
public class SingletonPatternDemo {
    public static void main(String[] args) throws Exception {


        Constructor<LazyMan> declaredConstructor = LazyMan.class.getDeclaredConstructor(null);
        Field field = LazyMan.class.getDeclaredField("flag");
        field.setAccessible(true);

        // 通过反射实例化对象
        declaredConstructor.setAccessible(true);
        LazyMan lazyMan1 = declaredConstructor.newInstance();
        System.out.println(field.get(lazyMan1));
        System.out.println(lazyMan1.hashCode());

        //通过反射，修改字段的值！
        field.set(lazyMan1, false);
        LazyMan lazyMan2 = declaredConstructor.newInstance();
        System.out.println(field.get(lazyMan2));
        System.out.println(lazyMan2.hashCode());
        
    }
}
```

并没有一个很好的方案去避免反射破坏单例模式，所以轮到我们的枚举登场了。

### 枚举

枚举类型是Java 5中新增特性的一部分，它是一种特殊的数据类型，之所以特殊是因为它既是一种类 (class)类型却又比类类型多了些特殊的约束，但是这些约束的存在也造就了枚举类型的简洁性、安全性 以及便捷性。

```java
public enum EnumSingleton {

    INSTANCE;
    public EnumSingleton getInstance(){
        return INSTANCE;
    }

}
```

枚举是目前最推荐的单例模式的写法，因为足够简单，不需要开发自己保证线程的安全，同时又可以有 效的防止反射破坏我们的单例模式

## 19、CAS

CAS（Conmpare And Swap） : 比较和交换

 JAVA1.5开始引入了CAS，主要代码都放在JUC的atomic包下

```java
public class CASDemo {
    public static void main(String[] args) {
        //真实值为 5 
        AtomicInteger atomicInteger = new AtomicInteger(5);

        // 期望的是5，后面改为 2020 ， 所以结果为 true，2020
        atomicInteger.compareAndSet(5, 2020);
        System.out.println(atomicInteger.get());
        // 期望的是5，后面改为 1024 ， 所以结果为 false，2020
        System.out.println(atomicInteger.compareAndSet(5, 1024) + "=>" + atomicInteger.get());
    }
}
```

真实值和期望值相同，就修改成功，真实值和期望值不同，就修改失败！



 分析源码，如何实现的 i++ 安全的问题：`atomicInteger.getAndIncrement();`

```java
public final int getAndIncrement() {
    // this 当前对象
	// valueOffset 内存偏移量，内存地址
	// 1	固定写死
    return unsafe.getAndAddInt(this, valueOffset, 1);
}
```

跳转到 unsafe

![image-20210720230938270](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/image-20210720230938270.png)

且这个类中的方法大部分都是 native 的方法了！

- **问题：这个UnSafe类到底是什么？**

1、UnSafe

UnSafe是 CAS 的核心类，由于Java方法无法直接访问底层系统，需要通过本地（native）方法来访问， UnSafe相当于一个后门，基于该类可以直接操作特定内存的数据，Unsafe类存在于 sun.misc 包中，其内部方法操作可以像C的指针一样直接操作内存，因为Java中CAS操作的执行依赖于Unsafe类的方法。



2、变量valueOffset

表示该变量值在内存中的偏移地址，因为Unsafe就是根据内存偏移地址获取数据的

3、变量 value用volatile修饰，保证了多线程之间的内存可见性



::: tip 最后解释CAS 是什么

:::

CAS 的全称为 Compare-And-Swap，它是一条CPU并发原语。

它的功能是判断内存某个位置的值是否为预期值，如果是则更改为新的值，这个过程是原子的。

CAS并发原语体现在JAVA语言中就是 sun.misc.Unsafe 类中的各个方法。调用 UnSafe类中的 CAS 方法， JVM会帮我们实现出CAS汇编指令。这是一种完全依赖于硬件的功能，通过它实现了原子操作。再次强调，由于CAS是一种系统原语，原语属于操作系统用于范畴，是由若干条指令组成的，用于完成某个功 能的一个过程，并且原语的执行必须是连续的，在执行过程中不允许被中断，也就是说CAS是一条 CPU 的原子指令，不会造成所谓的数据不一致问题。

```java
public final int getAndAddInt(Object var1, long var2, int var4) {
    int var5;
    do {
        // 获取传入对象的地址
        var5 = this.getIntVolatile(var1, var2);
        // 比较并交换，如果var1，var2 还是原来的 var5，就执行内存偏移+1； var5 +var4
    } while(!this.compareAndSwapInt(var1, var2, var5, var5 + var4));

    return var5;
}
```



::: tip 汇编层面理解

:::

Unsafe 类中的 compareAndSwapint，是一个本地方法，该方法的实现位于 unsafe.cpp 中；

![JUC-00000044](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000044.png)



::: note 总结

:::

**CAS（CompareAndSwap）：**

比较当前工作内存中的值和主内存中的值，如果相同则执行规定操作，否则继续比较直到主内存和工作内存中的值一致为止。

**CAS 应用：**

CAS 有3个操作数，内存值V，旧的预期值A，要修改的更新值B。且仅当预期值A 和 内存值 V 相同时， 将内存值 V 修改为B，否则什么都不做。

**CAS 的缺点：**

1、循环时间长开销很大。

可以看到源码中存在 一个 do...while 操作，如果CAS失败就会一直进行尝试。

2、只能保证一个共享变量的原子操作。

当对一个共享变量执行操作时，我们可以使用循环CAS的方式来保证原子操作。但是，对多个共享变量操作时，循环CAS就无法保证操作的原子性，这时候就可以用锁来保证原子性

3、CAS实现的过程是先取出内存中某时刻的数据，在下一时刻比较并替换，那么在这个时间差会导致数据的变化，此时就会导致出现“ABA”问题



**什么是”ABA”问题？**

比如说一个线程one从内存位置V中取出A，这时候另一个线程two也从内存中取出A，并且two进行了一些操作变成了B，然后two又将V位置的数据变成A，这时候线程one进行CAS操作发现内存中仍然是A，然后one操作成功。

尽管线程one的CAS操作成功，但是不代表这个过程就是没有问题的。

## 20、原子引用

demo：

```java
public class AtomicReferenceDemo {
    public static void main(String[] args) {

        User zhangsan = new User("zhangsan", 22);
        User lisi = new User("lisi", 25);

        AtomicReference<User> atomicReference = new AtomicReference<>();
        atomicReference.set(zhangsan); // 设置

        // 期望的是zhangsan，后面改为 lisi ， 所以结果为 true，
        System.out.print(atomicReference.compareAndSet(zhangsan, lisi)+"=>");
        System.out.println(atomicReference.get().toString());
        // 期望的是zhangsan，后面改为 lisi ， 所以结果为 flase，
        System.out.print(atomicReference.compareAndSet(zhangsan, lisi));
        System.out.println(atomicReference.get().toString());

    }
}
```

::: tip 原子引用 AtomicReference 解决ABA问题

要解决ABA问题，我们就需要加一个版本号

版本号原子引用，类似乐观锁

:::



```java
public class ABASaveDemo {
    static AtomicStampedReference<Integer> atomicStampedReference = new AtomicStampedReference<>(100, 1);


    public static void main(String[] args) {

        new Thread(() -> {
            int stamp = atomicStampedReference.getStamp(); // 获得版本号
            System.out.println("T1 stamp 01=>" + stamp);
            // 暂停2秒钟，保证下面线程获得初始版本号
            try {
                TimeUnit.SECONDS.sleep(1);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }

            atomicStampedReference.compareAndSet(100, 101,
                    atomicStampedReference.getStamp(), atomicStampedReference.getStamp() + 1);

            System.out.println("T1 stamp 02=>" + atomicStampedReference.getStamp());

            atomicStampedReference.compareAndSet(101, 100,
                    atomicStampedReference.getStamp(), atomicStampedReference.getStamp() + 1);

            System.out.println("T1 stamp 03=>" + atomicStampedReference.getStamp());
        }, "T1").start();


        new Thread(() -> {
            int stamp = atomicStampedReference.getStamp(); // 获得版本号
            System.out.println("T2 stamp 01=>" + stamp);
			// 暂停3秒钟，保证上面线程先执行
            try {
                TimeUnit.SECONDS.sleep(3);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }

            boolean result = atomicStampedReference.compareAndSet(100, 2019,
                    stamp, stamp + 1);
            System.out.println("T2 是否修改成功 =>" + result);
            System.out.println("T2 最新stamp =>" + atomicStampedReference.getStamp());
            System.out.println("T2 当前的最新值  =>" + atomicStampedReference.getReference());
        }, "T2").start();


    }
}
```



## 21、Java锁

### 公平锁非公平锁

公平锁：是指多个线程按照申请锁的顺序来获取锁，类似排队打饭，先来后到。

非公平锁：是指多个线程获取锁的顺序并不是按照申请锁的顺序，有可能后申请的线程比现申请的线程优先获取锁，在高并发的情况下，有可能会造成优先级反转或者饥饿现象。

```java
// 无参
public ReentrantLock() {
	sync = new NonfairSync();
}
// 有参
public ReentrantLock(boolean fair) {
	sync = fair ? new FairSync() : new NonfairSync();
}
```



::: tip 两者区别

:::

并发包中的 ReentrantLock 的创建可以指定构造函数的 boolean 类型来得到公平锁或者非公平锁，默认是非公平锁！

公平锁：就是很公平，在并发环境中，每个线程在获取到锁时会先查看此锁维护的等待队列，如果为空，或者当前线程是等待队列的第一个，就占有锁，否则就会加入到等待队列中，以后会按照FIFO的规则从队列中取到自己。

非公平锁：非公平锁比较粗鲁，上来就直接尝试占有锁，如果尝试失败，就会采用类似公平锁那种方式。

Java ReentrantLock 而言，通过构造函数指定该锁是否是公平锁，默认是非公平锁。非公平锁的优点在 于吞吐量比公平锁大。

对于Synchronized而言，也是一种非公平锁。



### 可重入锁

可重入锁（也叫递归锁）

指的是同一线程外层函数获得锁之后，内层递归函数仍然能获取该锁的代码，在同一个线程在外层方法 获取锁的时候，在进入内层方法会自动获取锁。

也就是说，线程可以进入任何一个它已经拥有的锁，所同步着的代码块。 好比家里进入大门之后，就可以进入里面的房间了；

ReentrantLock、Synchronized 就是一个典型的可重入锁；

**可重入锁最大的作用就是避免死锁**

测试一：Synchronized



```java
public class ReentrantLockDemo {
    public static void main(String[] args) {
        Phone phone = new Phone();
        // T1 线程在外层获取锁时，也会自动获取里面的锁
        new Thread(() -> {
            phone.sendSMS();
        }, "T1").start();

        new Thread(() -> {
            phone.sendSMS();
        }, "T2").start();

    }
}
class Phone {
    public synchronized void sendSMS() {
        System.out.println(Thread.currentThread().getName() + " sendSMS");
        sendEmail();
    }

    public synchronized void sendEmail() {
        System.out.println(Thread.currentThread().getName() + " sendEmail");
    }
}
```

测试二：ReentrantLock

```java
public class ReentrantLockDemo {
    public static void main(String[] args) {
        Phone phone = new Phone();
        // T1 线程在外层获取锁时，也会自动获取里面的锁
        new Thread(phone, "T1").start();
        new Thread(phone, "T2").start();

    }
}

class Phone implements Runnable {

    Lock lock = new ReentrantLock();

    @Override
    public void run() {
        get();
    }

    public void get() {
        lock.lock();
        // lock.lock(); 锁必须匹配，如果两个锁，只有一个解锁就会失败
        try {
            System.out.println(Thread.currentThread().getName() + " get()");
            set();
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
            // lock.lock();
        }

    }

    public void set() {
        lock.lock();
        try {
            System.out.println(Thread.currentThread().getName() + " set()");
        } catch (Exception e) {
            e.printStackTrace();
        } finally {
            lock.unlock();
        }
    }
}
```



### 自旋锁

自旋锁（spinlock），是指尝试获取锁的线程不会立即阻塞，而是采用循环的方式去尝试获取锁，这样的好处是减少线程上下文切换的消耗，缺点是循环会消耗CPU。

```java
public class SpinLockDemo {
    // 原子引用线程, 没写参数，引用类型默认为null
    AtomicReference<Thread> atomicReference = new AtomicReference<>();

    //上锁
    public void myLock() {
        Thread thread = Thread.currentThread();
        System.out.println(Thread.currentThread().getName() + "==>mylock");
        // 自旋
        while (!atomicReference.compareAndSet(null, thread)) {
        }
    }

    //解锁
    public void myUnlock() {
        Thread thread = Thread.currentThread();
        atomicReference.compareAndSet(thread, null);
        System.out.println(Thread.currentThread().getName() + "==>myUnlock");
    }

    public static void main(String[] args) throws InterruptedException {
        SpinLockDemo spinLockDemo = new SpinLockDemo();

        new Thread(() -> {
            spinLockDemo.myLock();
            try {
                TimeUnit.SECONDS.sleep(4);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
            spinLockDemo.myUnlock();
        }, "T1").start();

        TimeUnit.SECONDS.sleep(1);

        new Thread(() -> {
            spinLockDemo.myLock();

            try {
                TimeUnit.SECONDS.sleep(1);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }

            spinLockDemo.myUnlock();
        }, "T2").start();
    }

}
```

### 死锁

死锁是指两个或两个以上的进程在执行过程中，因争夺资源而造成的一种互相等待的现象，若无外力干涉那它们都将无法推进下去，如果系统资源充足，进程的资源请求都能够得到满足，死锁出现的可能性就很低，否者就会因为争夺有限的资源而陷入死锁。

![JUC-00000047](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/JUC-00000047.png)

**产生死锁主要原因：** 

1、系统资源不足 

2、进程运行推进的顺序不合适 

3、资源分配不当

**测试：**

```java
public class DeadLockDemo {
    public static void main(String[] args) {
        String lockA = "lockA";
        String lockB = "lockB";
        new Thread(new HoldLockThread(lockA, lockB), "T1").start();
        new Thread(new HoldLockThread(lockB, lockA), "T2").start();
    }
}

class HoldLockThread implements Runnable {
    private String lockA;
    private String lockB;

    public HoldLockThread(String lockA, String lockB) {
        this.lockA = lockA;
        this.lockB = lockB;
    }

    @Override
    public void run() {
        synchronized (lockA) {

            System.out.println(Thread.currentThread().getName() + "lock:" + lockA + "=>get" + lockB);
            try {
                TimeUnit.SECONDS.sleep(2);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }

            synchronized (lockB) {
                System.out.println(Thread.currentThread().getName() + "lock:" + lockB + "=>get" + lockA);
            }
        }
    }
}
```



::: tip 解决

:::

1、查看JDK目录的bin目录 

2、使用 `jps -l` 命令定位进程号 

3、使用 `jstack 进程号` 找到死锁查看



![image-20210721145715854](https://cdn.jsdelivr.net/gh/oddfar/static/img/JUC学习笔记.assets/image-20210721145715854.png)


# JavaWeb笔记

## 1、基本概念

### 1.1、前言

web开发：

- web，网页的意思  ， www.baidu.com
- 静态web
  - html，css
  - 提供给所有人看的数据始终不会发生变化！
- 动态web
  - 淘宝，几乎是所有的网站；
  - 提供给所有人看的数据始终会发生变化，每个人在不同的时间，不同的地点看到的信息各不相同！
  - 技术栈：Servlet/JSP，ASP，PHP

在Java中，动态web资源开发的技术统称为JavaWeb；

### 1.2、web应用程序

web应用程序：可以提供浏览器访问的程序；

- a.html、b.html......多个web资源，这些web资源可以被外界访问，对外界提供服务；
- 你们能访问到的任何一个页面或者资源，都存在于这个世界的某一个角落的计算机上。
- URL 
- 这个统一的web资源会被放在同一个文件夹下，web应用程序-->Tomcat：服务器
- 一个web应用由多部分组成 （静态web，动态web）
  - html，css，js
  - jsp，servlet
  - Java程序
  - jar包
  - 配置文件 （Properties）

web应用程序编写完毕后，若想提供给外界访问：需要一个服务器来统一管理；

### 1.3、静态web

- *.htm, *.html,这些都是网页的后缀，如果服务器上一直存在这些东西，我们就可以直接进行读取。通络；

![1567822802516](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567822802516.png)

- 静态web存在的缺点
  - Web页面无法动态更新，所有用户看到都是同一个页面
    - 轮播图，点击特效：伪动态
    - JavaScript [实际开发中，它用的最多]
    - VBScript
  - 它无法和数据库交互（数据无法持久化，用户无法交互）



### 1.4、动态web

页面会动态展示： “Web的页面展示的效果因人而异”；

![1567823191289](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567823191289.png)

缺点：

- 加入服务器的动态web资源出现了错误，我们需要重新编写我们的**后台程序**,重新发布；
  - 停机维护

优点：

- Web页面可以动态更新，所有用户看到都不是同一个页面
- 它可以与数据库交互 （数据持久化：注册，商品信息，用户信息........）

![1567823350584](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567823350584.png)


## 2、web服务器

### 2.1、技术讲解

**ASP:**

- 微软：国内最早流行的就是ASP；

- 在HTML中嵌入了VB的脚本，  ASP + COM；

- 在ASP开发中，基本一个页面都有几千行的业务代码，页面极其换乱

- 维护成本高！

- C# 

- IIS

  ```html
  <h1>
      <h1><h1>
          <h1>
              <h1>
                  <h1>
          <h1>
              <%
              System.out.println("hello")
              %>
              <h1>
                  <h1>
     <h1><h1>
  <h1>
  ```

  

**php：**

- PHP开发速度很快，功能很强大，跨平台，代码很简单 （70% , WP）
- 无法承载大访问量的情况（局限性）



**JSP/Servlet : ** 

B/S：浏览和服务器

C/S:  客户端和服务器

- sun公司主推的B/S架构
- 基于Java语言的 (所有的大公司，或者一些开源的组件，都是用Java写的)
- 可以承载三高问题带来的影响；
- 语法像ASP ， ASP-->JSP , 加强市场强度；



.....



### 2.2、web服务器

服务器是一种被动的操作，用来处理用户的一些请求和给用户一些响应信息；



**IIS**

微软的； ASP...,Windows中自带的

**Tomcat**

![1567824446428](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567824446428.png)

面向百度编程；

Tomcat是Apache 软件基金会（Apache Software Foundation）的Jakarta 项目中的一个核心项目，最新的Servlet 和JSP 规范总是能在Tomcat 中得到体现，因为Tomcat 技术先进、性能稳定，而且**免费**，因而深受Java 爱好者的喜爱并得到了部分软件开发商的认可，成为目前比较流行的Web 应用服务器。

Tomcat 服务器是一个免费的开放源代码的Web 应用服务器，属于轻量级应用[服务器](https://baike.baidu.com/item/服务器)，在中小型系统和并发访问用户不是很多的场合下被普遍使用，是开发和调试JSP 程序的首选。对于一个Java初学web的人来说，它是最佳的选择

Tomcat 实际上运行JSP 页面和Servlet。

....

**工作3-5年之后，可以尝试手写Tomcat服务器；**

下载tomcat：

1. 安装 or  解压
2. 了解配置文件及目录结构
3. 这个东西的作用

## 3、Tomcat

### 3.1、 安装tomcat

tomcat官网：http://tomcat.apache.org/

![1567825600842](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567825600842.png)

![1567825627138](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567825627138.png)



### 3.2、Tomcat启动和配置

文件夹作用：

![1567825763180](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567825763180.png)

**启动。关闭Tomcat**

![1567825840657](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567825840657.png)

访问测试：http://localhost:8080/

可能遇到的问题：

1. Java环境变量没有配置
2. 闪退问题：需要配置兼容性
3. 乱码问题：配置文件中设置

### 3.3、配置

![1567825967256](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567825967256.png)

可以配置启动的端口号

- tomcat的默认端口号为：8080
- mysql：3306
- http：80
- https：443

```xml
<Connector port="8081" protocol="HTTP/1.1"
           connectionTimeout="20000"
           redirectPort="8443" />
```
可以配置主机的名称

- 默认的主机名为：localhost->127.0.0.1
- 默认网站应用存放的位置为：webapps

```xml
  <Host name="www.qinjiang.com"  appBase="webapps"
        unpackWARs="true" autoDeploy="true">
```
### 高难度面试题：

请你谈谈网站是如何进行访问的！

1. 输入一个域名；回车

2. 检查本机的 C:\Windows\System32\drivers\etc\hosts配置文件下有没有这个域名映射；

   1. 有：直接返回对应的ip地址，这个地址中，有我们需要访问的web程序，可以直接访问

      ```java
      127.0.0.1       www.qinjiang.com
      ```

   2. 没有：去DNS服务器找，找到的话就返回，找不到就返回找不到；

   ![1567827057913](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567827057913.png)

4. 可以配置一下环境变量（可选性）

### 3.4、发布一个web网站

不会就先模仿

- 将自己写的网站，放到服务器(Tomcat)中指定的web应用的文件夹（webapps）下，就可以访问了

网站应该有的结构

```java
--webapps ：Tomcat服务器的web目录
	-ROOT
	-kuangstudy ：网站的目录名
		- WEB-INF
			-classes : java程序
			-lib：web应用所依赖的jar包
			-web.xml ：网站配置文件
		- index.html 默认的首页
		- static 
            -css
            	-style.css
            -js
            -img
         -.....
```



HTTP协议 ： 面试

Maven：构建工具

- Maven安装包

Servlet 入门

- HelloWorld！
- Servlet配置
- 原理

# 4、Http

## 4.1、什么是HTTP

HTTP（超文本传输协议）是一个简单的请求-响应协议，它通常运行在TCP之上。

- 文本：html，字符串，~ ….
- 超文本：图片，音乐，视频，定位，地图…….
- 80

Https：安全的

- 443

## 4.2、两个时代

- http1.0

  - HTTP/1.0：客户端可以与web服务器连接后，只能获得一个web资源，断开连接

- http2.0

  - HTTP/1.1：客户端可以与web服务器连接后，可以获得多个web资源。‘

  

## 4.3、Http请求

- 客户端---发请求（Request）---服务器

百度：

```java
Request URL:https://www.baidu.com/   请求地址
Request Method:GET    get方法/post方法
Status Code:200 OK    状态码：200
Remote（远程） Address:14.215.177.39:443
```

```java
Accept:text/html  
Accept-Encoding:gzip, deflate, br
Accept-Language:zh-CN,zh;q=0.9    语言
Cache-Control:max-age=0
Connection:keep-alive
```

### 1、请求行

- 请求行中的请求方式：GET
- 请求方式：**Get，Post**，HEAD,DELETE,PUT,TRACT…
  - get：请求能够携带的参数比较少，大小有限制，会在浏览器的URL地址栏显示数据内容，不安全，但高效
  - post：请求能够携带的参数没有限制，大小没有限制，不会在浏览器的URL地址栏显示数据内容，安全，但不高效。

### 2、消息头

```java
Accept：告诉浏览器，它所支持的数据类型
Accept-Encoding：支持哪种编码格式  GBK   UTF-8   GB2312  ISO8859-1
Accept-Language：告诉浏览器，它的语言环境
Cache-Control：缓存控制
Connection：告诉浏览器，请求完成是断开还是保持连接
HOST：主机..../.
```

## 4.4、Http响应

- 服务器---响应-----客户端

百度：

```java
Cache-Control:private    缓存控制
Connection:Keep-Alive    连接
Content-Encoding:gzip    编码
Content-Type:text/html   类型
```

### 1.响应体

```java
Accept：告诉浏览器，它所支持的数据类型
Accept-Encoding：支持哪种编码格式  GBK   UTF-8   GB2312  ISO8859-1
Accept-Language：告诉浏览器，它的语言环境
Cache-Control：缓存控制
Connection：告诉浏览器，请求完成是断开还是保持连接
HOST：主机..../.
Refresh：告诉客户端，多久刷新一次；
Location：让网页重新定位；
```

### 2、响应状态码 

200：请求响应成功  200

3xx：请求重定向 

- 重定向：你重新到我给你新位置去；

4xx：找不到资源   404

- 资源不存在；

5xx：服务器代码错误   500       502:网关错误



**常见面试题：**

当你的浏览器中地址栏输入地址并回车的一瞬间到页面能够展示回来，经历了什么？


# 5、Maven

**我为什么要学习这个技术？**

1. 在Javaweb开发中，需要使用大量的jar包，我们手动去导入；

2. 如何能够让一个东西自动帮我导入和配置这个jar包。

   由此，Maven诞生了！



## 5.1 Maven项目架构管理工具

我们目前用来就是方便导入jar包的！

Maven的核心思想：**约定大于配置**

- 有约束，不要去违反。

Maven会规定好你该如何去编写我们的Java代码，必须要按照这个规范来；

## 5.2 下载安装Maven

官网;https://maven.apache.org/

![1567842350606](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567842350606.png)

下载完成后，解压即可；

小狂神友情建议：电脑上的所有环境都放在一个文件夹下，方便管理；



## 5.3 配置环境变量

在我们的系统环境变量中

配置如下配置：

- M2_HOME     maven目录下的bin目录
- MAVEN_HOME      maven的目录
- 在系统的path中配置  %MAVEN_HOME%\bin

![1567842882993](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567842882993.png)

测试Maven是否安装成功，保证必须配置完毕！

## 5.4 阿里云镜像

![1567844609399](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567844609399.png)

- 镜像：mirrors
  - 作用：加速我们的下载
- 国内建议使用阿里云的镜像

```xml
<mirror>
    <id>nexus-aliyun</id>  
    <mirrorOf>*,!jeecg,!jeecg-snapshots</mirrorOf>  
    <name>Nexus aliyun</name>  
    <url>http://maven.aliyun.com/nexus/content/groups/public</url> 
</mirror>
```

## 5.5 本地仓库

在本地的仓库，远程仓库；

**建立一个本地仓库：**localRepository

```xml
<localRepository>D:\Environment\apache-maven-3.6.2\maven-repo</localRepository>
```

## 5.6、在IDEA中使用Maven

1. 启动IDEA

2. 创建一个MavenWeb项目

   ![1567844785602](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567844785602.png)

   ![1567844841172](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567844841172.png)

   ![1567844917185](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567844917185.png)

   ![1567844956177](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567844956177.png)

   ![1567845029864](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845029864.png)

3. 等待项目初始化完毕

   ![1567845105970](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845105970.png)

   ![1567845137978](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845137978.png)

4. 观察maven仓库中多了什么东西？

5. IDEA中的Maven设置

   注意：IDEA项目创建成功后，看一眼Maven的配置

   ![1567845341956](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845341956.png)

   ![1567845413672](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845413672.png)

6. 到这里，Maven在IDEA中的配置和使用就OK了!

## 5.7、创建一个普通的Maven项目

![1567845557744](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845557744.png)

![1567845717377](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845717377.png)

这个只有在Web应用下才会有！

![1567845782034](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845782034.png)

## 5.8 标记文件夹功能

![1567845910728](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845910728.png)

![1567845957139](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567845957139.png)

![1567846034906](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846034906.png)

![1567846073511](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846073511.png)

## 5.9 在 IDEA中配置Tomcat

![1567846140348](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846140348.png)

![1567846179573](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846179573.png)

![1567846234175](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846234175.png)

![1567846369751](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846369751.png)

解决警告问题

必须要的配置：**为什么会有这个问题：我们访问一个网站，需要指定一个文件夹名字；**

![1567846421963](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846421963.png)

![1567846546465](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846546465.png)

![1567846559111](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846559111.png)

![1567846640372](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846640372.png)

## 5.10 pom文件

pom.xml 是Maven的核心配置文件

![1567846784849](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567846784849.png)

```xml
<?xml version="1.0" encoding="UTF-8"?>

<!--Maven版本和头文件-->
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>

  <!--这里就是我们刚才配置的GAV-->
  <groupId>com.kuang</groupId>
  <artifactId>javaweb-01-maven</artifactId>
  <version>1.0-SNAPSHOT</version>
  <!--Package：项目的打包方式
  jar：java应用
  war：JavaWeb应用
  -->
  <packaging>war</packaging>


  <!--配置-->
  <properties>
    <!--项目的默认构建编码-->
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    <!--编码版本-->
    <maven.compiler.source>1.8</maven.compiler.source>
    <maven.compiler.target>1.8</maven.compiler.target>
  </properties>

  <!--项目依赖-->
  <dependencies>
    <!--具体依赖的jar包配置文件-->
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.11</version>
    </dependency>
  </dependencies>

  <!--项目构建用的东西-->
  <build>
    <finalName>javaweb-01-maven</finalName>
    <pluginManagement><!-- lock down plugins versions to avoid using Maven defaults (may be moved to parent pom) -->
      <plugins>
        <plugin>
          <artifactId>maven-clean-plugin</artifactId>
          <version>3.1.0</version>
        </plugin>
        <!-- see http://maven.apache.org/ref/current/maven-core/default-bindings.html#Plugin_bindings_for_war_packaging -->
        <plugin>
          <artifactId>maven-resources-plugin</artifactId>
          <version>3.0.2</version>
        </plugin>
        <plugin>
          <artifactId>maven-compiler-plugin</artifactId>
          <version>3.8.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-surefire-plugin</artifactId>
          <version>2.22.1</version>
        </plugin>
        <plugin>
          <artifactId>maven-war-plugin</artifactId>
          <version>3.2.2</version>
        </plugin>
        <plugin>
          <artifactId>maven-install-plugin</artifactId>
          <version>2.5.2</version>
        </plugin>
        <plugin>
          <artifactId>maven-deploy-plugin</artifactId>
          <version>2.8.2</version>
        </plugin>
      </plugins>
    </pluginManagement>
  </build>
</project>

```

![1567847410771](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567847410771.png)



maven由于他的约定大于配置，我们之后可以能遇到我们写的配置文件，无法被导出或者生效的问题，解决方案：

```xml
<!--在build中配置resources，来防止我们资源导出失败的问题-->
<build>
    <resources>
        <resource>
            <directory>src/main/resources</directory>
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>
            <filtering>true</filtering>
        </resource>
        <resource>
            <directory>src/main/java</directory>
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>
            <filtering>true</filtering>
        </resource>
    </resources>
</build>
```



## 5.12 IDEA操作

![1567847630808](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567847630808.png)



![1567847662429](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567847662429.png)



## 5.13 解决遇到的问题

1. Maven 3.6.2

   解决方法：降级为3.6.1

   ![1567904721301](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567904721301.png)

2. Tomcat闪退

   

3. IDEA中每次都要重复配置Maven
   在IDEA中的全局默认配置中去配置

   ![1567905247201](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567905247201.png)

   ![1567905291002](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567905291002.png)

4. Maven项目中Tomcat无法配置

5. maven默认web项目中的web.xml版本问题

   ![1567905537026](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567905537026.png)

6. 替换为webapp4.0版本和tomcat一致

   ```xml
   <?xml version="1.0" encoding="UTF-8"?>
   <web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee
                         http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
            version="4.0"
            metadata-complete="true">
   
   
   
   </web-app>
   ```

   

7. Maven仓库的使用

   地址：https://mvnrepository.com/

   ![1567905870750](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567905870750.png)

   ![1567905982979](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567905982979.png)

   ![1567906017448](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567906017448.png)

   ![1567906039469](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567906039469.png)


## 6、Servlet

### 6.1、Servlet简介

- Servlet就是sun公司开发动态web的一门技术
- Sun在这些API中提供一个接口叫做：Servlet，如果你想开发一个Servlet程序，只需要完成两个小步骤：
  - 编写一个类，实现Servlet接口
  - 把开发好的Java类部署到web服务器中。

**把实现了Servlet接口的Java程序叫做，Servlet**

### 6.2、HelloServlet

Serlvet接口Sun公司有两个默认的实现类：HttpServlet，GenericServlet



1. 构建一个普通的Maven项目，删掉里面的src目录，以后我们的学习就在这个项目里面建立Moudel；这个空的工程就是Maven主工程；

2. 关于Maven父子工程的理解：

   父项目中会有

   ```xml
       <modules>
           <module>servlet-01</module>
       </modules>
   ```

   子项目会有

   ```xml
       <parent>
           <artifactId>javaweb-02-servlet</artifactId>
           <groupId>com.kuang</groupId>
           <version>1.0-SNAPSHOT</version>
       </parent>
   ```

   父项目中的java子项目可以直接使用

   ```java
   son extends father
   ```

3. Maven环境优化

   1. 修改web.xml为最新的
   2. 将maven的结构搭建完整

4. 编写一个Servlet程序

   ![1567911804700](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567911804700.png)

   1. 编写一个普通类

   2. 实现Servlet接口，这里我们直接继承HttpServlet

      ```java
      public class HelloServlet extends HttpServlet {
          
          //由于get或者post只是请求实现的不同的方式，可以相互调用，业务逻辑都一样；
          @Override
          protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
              //ServletOutputStream outputStream = resp.getOutputStream();
              PrintWriter writer = resp.getWriter(); //响应流
              writer.print("Hello,Serlvet");
          }
      
          @Override
          protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
              doGet(req, resp);
          }
      }
      
      ```

5. 编写Servlet的映射

   为什么需要映射：我们写的是JAVA程序，但是要通过浏览器访问，而浏览器需要连接web服务器，所以我们需要再web服务中注册我们写的Servlet，还需给他一个浏览器能够访问的路径；

   ```xml
       <!--注册Servlet-->
       <servlet>
           <servlet-name>hello</servlet-name>
           <servlet-class>com.kuang.servlet.HelloServlet</servlet-class>
       </servlet>
       <!--Servlet的请求路径-->
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello</url-pattern>
       </servlet-mapping>
   
   ```

   

6. 配置Tomcat

   注意：配置项目发布的路径就可以了

7. 启动测试，OK！

### 6.3、Servlet原理

Servlet是由Web服务器调用，web服务器在收到浏览器请求之后，会：

![1567913793252](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567913793252.png)

### 6.4、Mapping问题

1. 一个Servlet可以指定一个映射路径

   ```xml
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello</url-pattern>
       </servlet-mapping>
   ```

2. 一个Servlet可以指定多个映射路径

   ```xml
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello</url-pattern>
       </servlet-mapping>
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello2</url-pattern>
       </servlet-mapping>
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello3</url-pattern>
       </servlet-mapping>
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello4</url-pattern>
       </servlet-mapping>
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello5</url-pattern>
       </servlet-mapping>
   
   ```

3. 一个Servlet可以指定通用映射路径

   ```xml
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/hello/*</url-pattern>
       </servlet-mapping>
   ```

4. 默认请求路径

   ```xml
       <!--默认请求路径-->
       <servlet-mapping>
           <servlet-name>hello</servlet-name>
           <url-pattern>/*</url-pattern>
       </servlet-mapping>
   ```

5. 指定一些后缀或者前缀等等….

   ```xml
   <!--可以自定义后缀实现请求映射
       注意点，*前面不能加项目映射的路径
       hello/sajdlkajda.qinjiang
       -->
   <servlet-mapping>
       <servlet-name>hello</servlet-name>
       <url-pattern>*.qinjiang</url-pattern>
   </servlet-mapping>
   ```

6. 优先级问题
   指定了固有的映射路径优先级最高，如果找不到就会走默认的处理请求；

   ```xml
   <!--404-->
   <servlet>
       <servlet-name>error</servlet-name>
       <servlet-class>com.kuang.servlet.ErrorServlet</servlet-class>
   </servlet>
   <servlet-mapping>
       <servlet-name>error</servlet-name>
       <url-pattern>/*</url-pattern>
   </servlet-mapping>
   
   ```

   

### 6.5、ServletContext

web容器在启动的时候，它会为每个web程序都创建一个对应的ServletContext对象，它代表了当前的web应用；

#### 1、共享数据

我在这个Servlet中保存的数据，可以在另外一个servlet中拿到；

```java
public class HelloServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        
        //this.getInitParameter()   初始化参数
        //this.getServletConfig()   Servlet配置
        //this.getServletContext()  Servlet上下文
        ServletContext context = this.getServletContext();

        String username = "秦疆"; //数据
        context.setAttribute("username",username); //将一个数据保存在了ServletContext中，名字为：username 。值 username

    }

}

```

```java
public class GetServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        ServletContext context = this.getServletContext();
        String username = (String) context.getAttribute("username");

        resp.setContentType("text/html");
        resp.setCharacterEncoding("utf-8");
        resp.getWriter().print("名字"+username);

    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        doGet(req, resp);
    }
}

```

```XML
    <servlet>
        <servlet-name>hello</servlet-name>
        <servlet-class>com.kuang.servlet.HelloServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>hello</servlet-name>
        <url-pattern>/hello</url-pattern>
    </servlet-mapping>


    <servlet>
        <servlet-name>getc</servlet-name>
        <servlet-class>com.kuang.servlet.GetServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>getc</servlet-name>
        <url-pattern>/getc</url-pattern>
    </servlet-mapping>
```

测试访问结果；



#### 2、获取初始化参数

```xml
    <!--配置一些web应用初始化参数-->
    <context-param>
        <param-name>url</param-name>
        <param-value>jdbc:mysql://localhost:3306/mybatis</param-value>
    </context-param>
```

```java
protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
    ServletContext context = this.getServletContext();
    String url = context.getInitParameter("url");
    resp.getWriter().print(url);
}
```

#### 3、请求转发

```java
@Override
protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
    ServletContext context = this.getServletContext();
    System.out.println("进入了ServletDemo04");
    //RequestDispatcher requestDispatcher = context.getRequestDispatcher("/gp"); //转发的请求路径
    //requestDispatcher.forward(req,resp); //调用forward实现请求转发；
    context.getRequestDispatcher("/gp").forward(req,resp);
}
```

![1567924457532](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567924457532.png)

#### 4、读取资源文件

Properties

- 在java目录下新建properties
- 在resources目录下新建properties

发现：都被打包到了同一个路径下：classes，我们俗称这个路径为classpath:

思路：需要一个文件流；

```properties
username=root12312
password=zxczxczxc
```

```java
public class ServletDemo05 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {

        InputStream is = this.getServletContext().getResourceAsStream("/WEB-INF/classes/com/kuang/servlet/aa.properties");

        Properties prop = new Properties();
        prop.load(is);
        String user = prop.getProperty("username");
        String pwd = prop.getProperty("password");

        resp.getWriter().print(user+":"+pwd);

    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        doGet(req, resp);
    }
}

```

访问测试即可ok；

### 6.6、HttpServletResponse

web服务器接收到客户端的http请求，针对这个请求，分别创建一个代表请求的HttpServletRequest对象，代表响应的一个HttpServletResponse；

- 如果要获取客户端请求过来的参数：找HttpServletRequest
- 如果要给客户端响应一些信息：找HttpServletResponse

#### 1、简单分类

负责向浏览器发送数据的方法

```java
ServletOutputStream getOutputStream() throws IOException;
PrintWriter getWriter() throws IOException;
```

负责向浏览器发送响应头的方法

```java
    void setCharacterEncoding(String var1);

    void setContentLength(int var1);

    void setContentLengthLong(long var1);

    void setContentType(String var1);

    void setDateHeader(String var1, long var2);

    void addDateHeader(String var1, long var2);

    void setHeader(String var1, String var2);

    void addHeader(String var1, String var2);

    void setIntHeader(String var1, int var2);

    void addIntHeader(String var1, int var2);
```

响应的状态码

```java
    int SC_CONTINUE = 100;
    int SC_SWITCHING_PROTOCOLS = 101;
    int SC_OK = 200;
    int SC_CREATED = 201;
    int SC_ACCEPTED = 202;
    int SC_NON_AUTHORITATIVE_INFORMATION = 203;
    int SC_NO_CONTENT = 204;
    int SC_RESET_CONTENT = 205;
    int SC_PARTIAL_CONTENT = 206;
    int SC_MULTIPLE_CHOICES = 300;
    int SC_MOVED_PERMANENTLY = 301;
    int SC_MOVED_TEMPORARILY = 302;
    int SC_FOUND = 302;
    int SC_SEE_OTHER = 303;
    int SC_NOT_MODIFIED = 304;
    int SC_USE_PROXY = 305;
    int SC_TEMPORARY_REDIRECT = 307;
    int SC_BAD_REQUEST = 400;
    int SC_UNAUTHORIZED = 401;
    int SC_PAYMENT_REQUIRED = 402;
    int SC_FORBIDDEN = 403;
    int SC_NOT_FOUND = 404;
    int SC_METHOD_NOT_ALLOWED = 405;
    int SC_NOT_ACCEPTABLE = 406;
    int SC_PROXY_AUTHENTICATION_REQUIRED = 407;
    int SC_REQUEST_TIMEOUT = 408;
    int SC_CONFLICT = 409;
    int SC_GONE = 410;
    int SC_LENGTH_REQUIRED = 411;
    int SC_PRECONDITION_FAILED = 412;
    int SC_REQUEST_ENTITY_TOO_LARGE = 413;
    int SC_REQUEST_URI_TOO_LONG = 414;
    int SC_UNSUPPORTED_MEDIA_TYPE = 415;
    int SC_REQUESTED_RANGE_NOT_SATISFIABLE = 416;
    int SC_EXPECTATION_FAILED = 417;
    int SC_INTERNAL_SERVER_ERROR = 500;
    int SC_NOT_IMPLEMENTED = 501;
    int SC_BAD_GATEWAY = 502;
    int SC_SERVICE_UNAVAILABLE = 503;
    int SC_GATEWAY_TIMEOUT = 504;
    int SC_HTTP_VERSION_NOT_SUPPORTED = 505;
```

#### 2、下载文件

1. 向浏览器输出消息 （一直在讲，就不说了）
2. 下载文件
   1. 要获取下载文件的路径
   2. 下载的文件名是啥？
   3. 设置想办法让浏览器能够支持下载我们需要的东西
   4. 获取下载文件的输入流
   5. 创建缓冲区
   6. 获取OutputStream对象
   7. 将FileOutputStream流写入到buffer缓冲区
   8. 使用OutputStream将缓冲区中的数据输出到客户端！

```java
@Override
protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
    // 1. 要获取下载文件的路径
    String realPath = "F:\\班级管理\\西开【19525】\\2、代码\\JavaWeb\\javaweb-02-servlet\\response\\target\\classes\\秦疆.png";
    System.out.println("下载文件的路径："+realPath);
    // 2. 下载的文件名是啥？
    String fileName = realPath.substring(realPath.lastIndexOf("\\") + 1);
    // 3. 设置想办法让浏览器能够支持(Content-Disposition)下载我们需要的东西,中文文件名URLEncoder.encode编码，否则有可能乱码
    resp.setHeader("Content-Disposition","attachment;filename="+URLEncoder.encode(fileName,"UTF-8"));
    // 4. 获取下载文件的输入流
    FileInputStream in = new FileInputStream(realPath);
    // 5. 创建缓冲区
    int len = 0;
    byte[] buffer = new byte[1024];
    // 6. 获取OutputStream对象
    ServletOutputStream out = resp.getOutputStream();
    // 7. 将FileOutputStream流写入到buffer缓冲区,使用OutputStream将缓冲区中的数据输出到客户端！
    while ((len=in.read(buffer))>0){
        out.write(buffer,0,len);
    }

    in.close();
    out.close();
}
```

#### 3、验证码功能

验证怎么来的？

- 前端实现
- 后端实现，需要用到 Java 的图片类，生产一个图片

```java
package com.kuang.servlet;

import javax.imageio.ImageIO;
import javax.servlet.ServletException;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.awt.*;
import java.awt.image.BufferedImage;
import java.io.IOException;
import java.util.Random;

public class ImageServlet extends HttpServlet {

    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {

        //如何让浏览器3秒自动刷新一次;
        resp.setHeader("refresh","3");
        
        //在内存中创建一个图片
        BufferedImage image = new BufferedImage(80,20,BufferedImage.TYPE_INT_RGB);
        //得到图片
        Graphics2D g = (Graphics2D) image.getGraphics(); //笔
        //设置图片的背景颜色
        g.setColor(Color.white);
        g.fillRect(0,0,80,20);
        //给图片写数据
        g.setColor(Color.BLUE);
        g.setFont(new Font(null,Font.BOLD,20));
        g.drawString(makeNum(),0,20);

        //告诉浏览器，这个请求用图片的方式打开
        resp.setContentType("image/jpeg");
        //网站存在缓存，不让浏览器缓存
        resp.setDateHeader("expires",-1);
        resp.setHeader("Cache-Control","no-cache");
        resp.setHeader("Pragma","no-cache");

        //把图片写给浏览器
        ImageIO.write(image,"jpg", resp.getOutputStream());

    }

    //生成随机数
    private String makeNum(){
        Random random = new Random();
        String num = random.nextInt(9999999) + "";
        StringBuffer sb = new StringBuffer();
        for (int i = 0; i < 7-num.length() ; i++) {
            sb.append("0");
        }
        num = sb.toString() + num;
        return num;
    }


    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        doGet(req, resp);
    }
}

```

#### 4、实现重定向

![1567931587955](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567931587955.png)

B一个web资源收到客户端A请求后，B他会通知A客户端去访问另外一个web资源C，这个过程叫重定向

常见场景：

- 用户登录

```java
void sendRedirect(String var1) throws IOException;
```

测试：

```java
@Override
protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {

    /*
        resp.setHeader("Location","/r/img");
        resp.setStatus(302);
         */
    resp.sendRedirect("/r/img");//重定向
}
```

面试题：请你聊聊重定向和转发的区别？

相同点

- 页面都会实现跳转

不同点

- 请求转发的时候，url不会产生变化
- 重定向时候，url地址栏会发生变化；

![1567932163430](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567932163430.png)

#### 5、简单实现登录重定向

```jsp
<%--这里提交的路径，需要寻找到项目的路径--%>
<%--${pageContext.request.contextPath}代表当前的项目--%>

<form action="${pageContext.request.contextPath}/login" method="get">
    用户名：<input type="text" name="username"> <br>
    密码：<input type="password" name="password"> <br>
    <input type="submit">
</form>

```

```JAVA
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        //处理请求
        String username = req.getParameter("username");
        String password = req.getParameter("password");

        System.out.println(username+":"+password);

        //重定向时候一定要注意，路径问题，否则404；
        resp.sendRedirect("/r/success.jsp");
    }

```

```xml
  <servlet>
    <servlet-name>requset</servlet-name>
    <servlet-class>com.kuang.servlet.RequestTest</servlet-class>
  </servlet>
  <servlet-mapping>
    <servlet-name>requset</servlet-name>
    <url-pattern>/login</url-pattern>
  </servlet-mapping>
```

```jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>Title</title>
</head>
<body>

<h1>Success</h1>

</body>
</html>

```

### 6.7、HttpServletRequest

HttpServletRequest代表客户端的请求，用户通过Http协议访问服务器，HTTP请求中的所有信息会被封装到HttpServletRequest，通过这个HttpServletRequest的方法，获得客户端的所有信息；

![1567933996830](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567933996830.png)

![1567934023106](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567934023106.png)

#### 获取参数，请求转发

![1567934110794](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1567934110794.png)

```java
@Override
protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {

    req.setCharacterEncoding("utf-8");
    resp.setCharacterEncoding("utf-8");

    String username = req.getParameter("username");
    String password = req.getParameter("password");
    String[] hobbys = req.getParameterValues("hobbys");
    System.out.println("=============================");
    //后台接收中文乱码问题
    System.out.println(username);
    System.out.println(password);
    System.out.println(Arrays.toString(hobbys));
    System.out.println("=============================");


    System.out.println(req.getContextPath());
    //通过请求转发
    //这里的 / 代表当前的web应用
    req.getRequestDispatcher("/success.jsp").forward(req,resp);

}
```

**面试题：请你聊聊重定向和转发的区别？**

相同点

- 页面都会实现跳转

不同点

- 请求转发的时候，url不会产生变化   307
- 重定向时候，url地址栏会发生变化； 302

## 7、Cookie、Session

### 7.1、会话

**会话**：用户打开一个浏览器，点击了很多超链接，访问多个web资源，关闭浏览器，这个过程可以称之为会话；

**有状态会话**：一个同学来过教室，下次再来教室，我们会知道这个同学，曾经来过，称之为有状态会话；

**你能怎么证明你是西开的学生？**

你              西开

1. 发票                西开给你发票
2. 学校登记        西开标记你来过了

**一个网站，怎么证明你来过？**

客户端              服务端

1. 服务端给客户端一个 信件，客户端下次访问服务端带上信件就可以了； cookie
2. 服务器登记你来过了，下次你来的时候我来匹配你； seesion



### 7.2、保存会话的两种技术

**cookie**

- 客户端技术   （响应，请求）

**session**

- 服务器技术，利用这个技术，可以保存用户的会话信息？ 我们可以把信息或者数据放在Session中！



常见常见：网站登录之后，你下次不用再登录了，第二次访问直接就上去了！

### 7.3、Cookie

![1568344447291](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568344447291.png)

1. 从请求中拿到cookie信息
2. 服务器响应给客户端cookie

```java
Cookie[] cookies = req.getCookies(); //获得Cookie
cookie.getName(); //获得cookie中的key
cookie.getValue(); //获得cookie中的vlaue
new Cookie("lastLoginTime", System.currentTimeMillis()+""); //新建一个cookie
cookie.setMaxAge(24*60*60); //设置cookie的有效期
resp.addCookie(cookie); //响应给客户端一个cookie
```

**cookie：一般会保存在本地的 用户目录下 appdata；**



一个网站cookie是否存在上限！**聊聊细节问题**

- 一个Cookie只能保存一个信息；
- 一个web站点可以给浏览器发送多个cookie，最多存放20个cookie；
- Cookie大小有限制4kb；
- 300个cookie浏览器上限



**删除Cookie；**

- 不设置有效期，关闭浏览器，自动失效；
- 设置有效期时间为 0 ；



**编码解码：**

```java
URLEncoder.encode("秦疆","utf-8")
URLDecoder.decode(cookie.getValue(),"UTF-8")
```



### 7.4、Session（重点）

![1568344560794](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568344560794.png)

什么是Session：

- 服务器会给每一个用户（浏览器）创建一个Seesion对象；
- 一个Seesion独占一个浏览器，只要浏览器没有关闭，这个Session就存在；
- 用户登录之后，整个网站它都可以访问！--> 保存用户的信息；保存购物车的信息…..

![1568342773861](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568342773861.png)

Session和cookie的区别：

- Cookie是把用户的数据写给用户的浏览器，浏览器保存 （可以保存多个）
- Session把用户的数据写到用户独占Session中，服务器端保存  （保存重要的信息，减少服务器资源的浪费）
- Session对象由服务创建；



使用场景：

- 保存一个登录用户的信息；
- 购物车信息；
- 在整个网站中经常会使用的数据，我们将它保存在Session中；



使用Session：

```java
package com.kuang.servlet;

import com.kuang.pojo.Person;

import javax.servlet.ServletException;
import javax.servlet.http.*;
import java.io.IOException;

public class SessionDemo01 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        
        //解决乱码问题
        req.setCharacterEncoding("UTF-8");
        resp.setCharacterEncoding("UTF-8");
        resp.setContentType("text/html;charset=utf-8");
        
        //得到Session
        HttpSession session = req.getSession();
        //给Session中存东西
        session.setAttribute("name",new Person("秦疆",1));
        //获取Session的ID
        String sessionId = session.getId();

        //判断Session是不是新创建
        if (session.isNew()){
            resp.getWriter().write("session创建成功,ID:"+sessionId);
        }else {
            resp.getWriter().write("session以及在服务器中存在了,ID:"+sessionId);
        }

        //Session创建的时候做了什么事情；
//        Cookie cookie = new Cookie("JSESSIONID",sessionId);
//        resp.addCookie(cookie);

    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        doGet(req, resp);
    }
}

//得到Session
HttpSession session = req.getSession();

Person person = (Person) session.getAttribute("name");

System.out.println(person.toString());

HttpSession session = req.getSession();
session.removeAttribute("name");
//手动注销Session
session.invalidate();
```



**会话自动过期：web.xml配置**

```xml
<!--设置Session默认的失效时间-->
<session-config>
    <!--15分钟后Session自动失效，以分钟为单位-->
    <session-timeout>15</session-timeout>
</session-config>
```



![1568344679763](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568344679763.png)

## 8、JSP

### 8.1、什么是JSP

Java Server Pages ： Java服务器端页面，也和Servlet一样，用于动态Web技术！

最大的特点：

- 写JSP就像在写HTML
- 区别：
  - HTML只给用户提供静态的数据
  - JSP页面中可以嵌入JAVA代码，为用户提供动态数据；



### 8.2、JSP原理

思路：JSP到底怎么执行的！

- 代码层面没有任何问题

- 服务器内部工作

  tomcat中有一个work目录；

  IDEA中使用Tomcat的会在IDEA的tomcat中生产一个work目录

  ![1568345873736](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568345873736.png)

  我电脑的地址：

  ```java
  C:\Users\Administrator\.IntelliJIdea2018.1\system\tomcat\Unnamed_javaweb-session-cookie\work\Catalina\localhost\ROOT\org\apache\jsp
  ```

  发现页面转变成了Java程序！

  ![1568345948307](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568345948307.png)



**浏览器向服务器发送请求，不管访问什么资源，其实都是在访问Servlet！**

JSP最终也会被转换成为一个Java类！

**JSP 本质上就是一个Servlet**

```java
//初始化
  public void _jspInit() {
      
  }
//销毁
  public void _jspDestroy() {
  }
//JSPService
  public void _jspService(.HttpServletRequest request,HttpServletResponse response)
      
```

1. 判断请求

2. 内置一些对象

   ```java
   final javax.servlet.jsp.PageContext pageContext;  //页面上下文
   javax.servlet.http.HttpSession session = null;    //session
   final javax.servlet.ServletContext application;   //applicationContext
   final javax.servlet.ServletConfig config;         //config
   javax.servlet.jsp.JspWriter out = null;           //out
   final java.lang.Object page = this;               //page：当前
   HttpServletRequest request                        //请求
   HttpServletResponse response                      //响应
   ```

3. 输出页面前增加的代码

   ```java
   response.setContentType("text/html");       //设置响应的页面类型
   pageContext = _jspxFactory.getPageContext(this, request, response,
                                             null, true, 8192, true);
   _jspx_page_context = pageContext;
   application = pageContext.getServletContext();
   config = pageContext.getServletConfig();
   session = pageContext.getSession();
   out = pageContext.getOut();
   _jspx_out = out;
   ```

4. 以上的这些个对象我们可以在JSP页面中直接使用！

![1568347078207](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568347078207.png)



在JSP页面中；

只要是 JAVA代码就会原封不动的输出；

如果是HTML代码，就会被转换为：

```java
out.write("<html>\r\n");
```

这样的格式，输出到前端！



### 8.3、JSP基础语法

任何语言都有自己的语法，JAVA中有,。 JSP 作为java技术的一种应用，它拥有一些自己扩充的语法（了解，知道即可！），Java所有语法都支持！



#### **JSP表达式**

```jsp
  <%--JSP表达式
  作用：用来将程序的输出，输出到客户端
  <%= 变量或者表达式%>
  --%>
  <%= new java.util.Date()%>
```



#### **jsp脚本片段**

```jsp

  <%--jsp脚本片段--%>
  <%
    int sum = 0;
    for (int i = 1; i <=100 ; i++) {
      sum+=i;
    }
    out.println("<h1>Sum="+sum+"</h1>");
  %>

```



**脚本片段的再实现**

```jsp
  <%
    int x = 10;
    out.println(x);
  %>
  <p>这是一个JSP文档</p>
  <%
    int y = 2;
    out.println(y);
  %>

  <hr>


  <%--在代码嵌入HTML元素--%>
  <%
    for (int i = 0; i < 5; i++) {
  %>
    <h1>Hello,World  <%=i%> </h1>
  <%
    }
  %>
```



#### JSP声明

```jsp
  <%!
    static {
      System.out.println("Loading Servlet!");
    }

    private int globalVar = 0;

    public void kuang(){
      System.out.println("进入了方法Kuang！");
    }
  %>
```



JSP声明：会被编译到JSP生成Java的类中！其他的，就会被生成到_jspService方法中！

在JSP，嵌入Java代码即可！

```jsp
<%%>
<%=%>
<%!%>

<%--注释--%>
```

JSP的注释，不会在客户端显示，HTML就会！



### 8.4、JSP指令

```jsp
<%@page args.... %>
<%@include file=""%>

<%--@include会将两个页面合二为一--%>

<%@include file="common/header.jsp"%>
<h1>网页主体</h1>

<%@include file="common/footer.jsp"%>

<hr>


<%--jSP标签
    jsp:include：拼接页面，本质还是三个
    --%>
<jsp:include page="/common/header.jsp"/>
<h1>网页主体</h1>
<jsp:include page="/common/footer.jsp"/>

```



### 8.5、9大内置对象

- PageContext    存东西
- Request     存东西
- Response
- Session      存东西
- Application   【SerlvetContext】   存东西
- config    【SerlvetConfig】
- out
- page ，不用了解
- exception

```java
pageContext.setAttribute("name1","秦疆1号"); //保存的数据只在一个页面中有效
request.setAttribute("name2","秦疆2号"); //保存的数据只在一次请求中有效，请求转发会携带这个数据
session.setAttribute("name3","秦疆3号"); //保存的数据只在一次会话中有效，从打开浏览器到关闭浏览器
application.setAttribute("name4","秦疆4号");  //保存的数据只在服务器中有效，从打开服务器到关闭服务器
```

request：客户端向服务器发送请求，产生的数据，用户看完就没用了，比如：新闻，用户看完没用的！

session：客户端向服务器发送请求，产生的数据，用户用完一会还有用，比如：购物车；

application：客户端向服务器发送请求，产生的数据，一个用户用完了，其他用户还可能使用，比如：聊天数据；

### 8.6、JSP标签、JSTL标签、EL表达式

```xml
<!-- JSTL表达式的依赖 -->
<dependency>
    <groupId>javax.servlet.jsp.jstl</groupId>
    <artifactId>jstl-api</artifactId>
    <version>1.2</version>
</dependency>
<!-- standard标签库 -->
<dependency>
    <groupId>taglibs</groupId>
    <artifactId>standard</artifactId>
    <version>1.1.2</version>
</dependency>

```

EL表达式：  ${ }

- **获取数据**
- **执行运算**
- **获取web开发的常用对象**



**JSP标签**

```jsp
<%--jsp:include--%>

<%--
http://localhost:8080/jsptag.jsp?name=kuangshen&age=12
--%>

<jsp:forward page="/jsptag2.jsp">
    <jsp:param name="name" value="kuangshen"></jsp:param>
    <jsp:param name="age" value="12"></jsp:param>
</jsp:forward>
```



**JSTL表达式**

JSTL标签库的使用就是为了弥补HTML标签的不足；它自定义许多标签，可以供我们使用，标签的功能和Java代码一样！

**格式化标签**

**SQL标签**

**XML 标签**

**核心标签** （掌握部分）

![1568362473764](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568362473764.png)

**JSTL标签库使用步骤**

- 引入对应的 taglib
- 使用其中的方法
- **在Tomcat 也需要引入 jstl的包，否则会报错：JSTL解析错误**

c：if

```jsp
<head>
    <title>Title</title>
</head>
<body>


<h4>if测试</h4>

<hr>

<form action="coreif.jsp" method="get">
    <%--
    EL表达式获取表单中的数据
    ${param.参数名}
    --%>
    <input type="text" name="username" value="${param.username}">
    <input type="submit" value="登录">
</form>

<%--判断如果提交的用户名是管理员，则登录成功--%>
<c:if test="${param.username=='admin'}" var="isAdmin">
    <c:out value="管理员欢迎您！"/>
</c:if>

<%--自闭合标签--%>
<c:out value="${isAdmin}"/>

</body>
```

c:choose   c:when

```jsp
<body>

<%--定义一个变量score，值为85--%>
<c:set var="score" value="55"/>

<c:choose>
    <c:when test="${score>=90}">
        你的成绩为优秀
    </c:when>
    <c:when test="${score>=80}">
        你的成绩为一般
    </c:when>
    <c:when test="${score>=70}">
        你的成绩为良好
    </c:when>
    <c:when test="${score<=60}">
        你的成绩为不及格
    </c:when>
</c:choose>

</body>
```

c:forEach

```jsp
<%

    ArrayList<String> people = new ArrayList<>();
    people.add(0,"张三");
    people.add(1,"李四");
    people.add(2,"王五");
    people.add(3,"赵六");
    people.add(4,"田六");
    request.setAttribute("list",people);
%>


<%--
var , 每一次遍历出来的变量
items, 要遍历的对象
begin,   哪里开始
end,     到哪里
step,   步长
--%>
<c:forEach var="people" items="${list}">
    <c:out value="${people}"/> <br>
</c:forEach>

<hr>

<c:forEach var="people" items="${list}" begin="1" end="3" step="1" >
    <c:out value="${people}"/> <br>
</c:forEach>

```

## 9、JavaBean

实体类

JavaBean有特定的写法：

- 必须要有一个无参构造
- 属性必须私有化
- 必须有对应的get/set方法；

一般用来和数据库的字段做映射  ORM；

ORM ：对象关系映射

- 表--->类
- 字段-->属性
- 行记录---->对象

**people表**

| id   | name    | age  | address |
| ---- | ------- | ---- | ------- |
| 1    | 秦疆1号 | 3    | 西安    |
| 2    | 秦疆2号 | 18   | 西安    |
| 3    | 秦疆3号 | 100  | 西安    |

```java
class People{
    private int id;
    private String name;
    private int id;
    private String address;
}

class A{
    new People(1,"秦疆1号",3，"西安");
    new People(2,"秦疆2号",3，"西安");
    new People(3,"秦疆3号",3，"西安");
}
```



- 过滤器
- 文件上传
- 邮件发送
- JDBC 复习 ： 如何使用JDBC ,  JDBC crud， jdbc 事务



## 10、MVC三层架构

什么是MVC：  Model     view     Controller  模型、视图、控制器

### 10.1、早些年

![1568423664332](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568423664332.png)

用户直接访问控制层，控制层就可以直接操作数据库；

```java
servlet--CRUD-->数据库
弊端：程序十分臃肿，不利于维护  
servlet的代码中：处理请求、响应、视图跳转、处理JDBC、处理业务代码、处理逻辑代码

架构：没有什么是加一层解决不了的！
程序猿调用
|
JDBC
|
Mysql Oracle SqlServer ....
```

### 10.2、MVC三层架构

![1568424227281](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568424227281.png)



Model

- 业务处理 ：业务逻辑（Service）
- 数据持久层：CRUD   （Dao）

View

- 展示数据
- 提供链接发起Servlet请求 （a，form，img…）

Controller  （Servlet）

- 接收用户的请求 ：（req：请求参数、Session信息….）

- 交给业务层处理对应的代码 

- 控制视图的跳转  

  ```java
  登录--->接收用户的登录请求--->处理用户的请求（获取用户登录的参数，username，password）---->交给业务层处理登录业务（判断用户名密码是否正确：事务）--->Dao层查询用户名和密码是否正确-->数据库
  ```



## 11、Filter （重点）

Filter：过滤器 ，用来过滤网站的数据；

- 处理中文乱码
- 登录验证….

![1568424858708](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568424858708.png)

Filter开发步骤：

1. 导包

2. 编写过滤器

   1. 导包不要错

      ![1568425162525](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568425162525.png)

      实现Filter接口，重写对应的方法即可

      ```java
      public class CharacterEncodingFilter implements Filter {
      
          //初始化：web服务器启动，就以及初始化了，随时等待过滤对象出现！
          public void init(FilterConfig filterConfig) throws ServletException {
              System.out.println("CharacterEncodingFilter初始化");
          }
      
          //Chain : 链
          /*
          1. 过滤中的所有代码，在过滤特定请求的时候都会执行
          2. 必须要让过滤器继续同行
              chain.doFilter(request,response);
           */
          public void doFilter(ServletRequest request, ServletResponse response, FilterChain chain) throws IOException, ServletException {
              request.setCharacterEncoding("utf-8");
              response.setCharacterEncoding("utf-8");
              response.setContentType("text/html;charset=UTF-8");
      
              System.out.println("CharacterEncodingFilter执行前....");
              chain.doFilter(request,response); //让我们的请求继续走，如果不写，程序到这里就被拦截停止！
              System.out.println("CharacterEncodingFilter执行后....");
          }
      
          //销毁：web服务器关闭的时候，过滤会销毁
          public void destroy() {
              System.out.println("CharacterEncodingFilter销毁");
          }
      }
      
      ```

3. 在web.xml中配置 Filter

   ```xml
   <filter>
       <filter-name>CharacterEncodingFilter</filter-name>
       <filter-class>com.kuang.filter.CharacterEncodingFilter</filter-class>
   </filter>
   <filter-mapping>
       <filter-name>CharacterEncodingFilter</filter-name>
       <!--只要是 /servlet的任何请求，会经过这个过滤器-->
       <url-pattern>/servlet/*</url-pattern>
       <!--<url-pattern>/*</url-pattern>-->
   </filter-mapping>
   ```

   

## 12、监听器

实现一个监听器的接口；（有N种）

1. 编写一个监听器

   实现监听器的接口…

   ```java
   //统计网站在线人数 ： 统计session
   public class OnlineCountListener implements HttpSessionListener {
   
       //创建session监听： 看你的一举一动
       //一旦创建Session就会触发一次这个事件！
       public void sessionCreated(HttpSessionEvent se) {
           ServletContext ctx = se.getSession().getServletContext();
   
           System.out.println(se.getSession().getId());
   
           Integer onlineCount = (Integer) ctx.getAttribute("OnlineCount");
   
           if (onlineCount==null){
               onlineCount = new Integer(1);
           }else {
               int count = onlineCount.intValue();
               onlineCount = new Integer(count+1);
           }
   
           ctx.setAttribute("OnlineCount",onlineCount);
   
       }
   
       //销毁session监听
       //一旦销毁Session就会触发一次这个事件！
       public void sessionDestroyed(HttpSessionEvent se) {
           ServletContext ctx = se.getSession().getServletContext();
   
           Integer onlineCount = (Integer) ctx.getAttribute("OnlineCount");
   
           if (onlineCount==null){
               onlineCount = new Integer(0);
           }else {
               int count = onlineCount.intValue();
               onlineCount = new Integer(count-1);
           }
   
           ctx.setAttribute("OnlineCount",onlineCount);
   
       }
   
   
       /*
       Session销毁：
       1. 手动销毁  getSession().invalidate();
       2. 自动销毁
        */
   }
   
   ```

2. web.xml中注册监听器

   ```xml
   <!--注册监听器-->
   <listener>
       <listener-class>com.kuang.listener.OnlineCountListener</listener-class>
   </listener>
   ```

3. 看情况是否使用！



## 13、过滤器、监听器常见应用

**监听器：GUI编程中经常使用；**

```java
public class TestPanel {
    public static void main(String[] args) {
        Frame frame = new Frame("中秋节快乐");  //新建一个窗体
        Panel panel = new Panel(null); //面板
        frame.setLayout(null); //设置窗体的布局

        frame.setBounds(300,300,500,500);
        frame.setBackground(new Color(0,0,255)); //设置背景颜色

        panel.setBounds(50,50,300,300);
        panel.setBackground(new Color(0,255,0)); //设置背景颜色

        frame.add(panel);

        frame.setVisible(true);

        //监听事件，监听关闭事件
        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                super.windowClosing(e);
            }
        });


    }
}
```



用户登录之后才能进入主页！用户注销后就不能进入主页了！

1. 用户登录之后，向Sesison中放入用户的数据

2. 进入主页的时候要判断用户是否已经登录；要求：在过滤器中实现！

   ```java
   HttpServletRequest request = (HttpServletRequest) req;
   HttpServletResponse response = (HttpServletResponse) resp;
   
   if (request.getSession().getAttribute(Constant.USER_SESSION)==null){
       response.sendRedirect("/error.jsp");
   }
   
   chain.doFilter(request,response);
   ```




## 14、JDBC

什么是JDBC ： Java连接数据库！

![1568439601825](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568439601825.png)

需要jar包的支持：

- java.sql
- javax.sql
- mysql-conneter-java…  连接驱动（必须要导入）



**实验环境搭建**

```sql

CREATE TABLE users(
    id INT PRIMARY KEY,
    `name` VARCHAR(40),
    `password` VARCHAR(40),
    email VARCHAR(60),
    birthday DATE
);

INSERT INTO users(id,`name`,`password`,email,birthday)
VALUES(1,'张三','123456','zs@qq.com','2000-01-01');
INSERT INTO users(id,`name`,`password`,email,birthday)
VALUES(2,'李四','123456','ls@qq.com','2000-01-01');
INSERT INTO users(id,`name`,`password`,email,birthday)
VALUES(3,'王五','123456','ww@qq.com','2000-01-01');


SELECT	* FROM users;

```



导入数据库依赖

```xml
<!--mysql的驱动-->
<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>5.1.47</version>
</dependency>
```

IDEA中连接数据库：

![1568440926845](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568440926845.png)



**JDBC 固定步骤：**

1. 加载驱动
2. 连接数据库,代表数据库
3. 向数据库发送SQL的对象Statement : CRUD
4. 编写SQL （根据业务，不同的SQL）
5. 执行SQL
6. 关闭连接

```java
public class TestJdbc {
    public static void main(String[] args) throws ClassNotFoundException, SQLException {
        //配置信息
        //useUnicode=true&characterEncoding=utf-8 解决中文乱码
        String url="jdbc:mysql://localhost:3306/jdbc?useUnicode=true&characterEncoding=utf-8";
        String username = "root";
        String password = "123456";

        //1.加载驱动
        Class.forName("com.mysql.jdbc.Driver");
        //2.连接数据库,代表数据库
        Connection connection = DriverManager.getConnection(url, username, password);

        //3.向数据库发送SQL的对象Statement,PreparedStatement : CRUD
        Statement statement = connection.createStatement();

        //4.编写SQL
        String sql = "select * from users";

        //5.执行查询SQL，返回一个 ResultSet  ： 结果集
        ResultSet rs = statement.executeQuery(sql);

        while (rs.next()){
            System.out.println("id="+rs.getObject("id"));
            System.out.println("name="+rs.getObject("name"));
            System.out.println("password="+rs.getObject("password"));
            System.out.println("email="+rs.getObject("email"));
            System.out.println("birthday="+rs.getObject("birthday"));
        }

        //6.关闭连接，释放资源（一定要做） 先开后关
        rs.close();
        statement.close();
        connection.close();
    }
}

```



**预编译SQL**

```java
public class TestJDBC2 {
    public static void main(String[] args) throws Exception {
        //配置信息
        //useUnicode=true&characterEncoding=utf-8 解决中文乱码
        String url="jdbc:mysql://localhost:3306/jdbc?useUnicode=true&characterEncoding=utf-8";
        String username = "root";
        String password = "123456";

        //1.加载驱动
        Class.forName("com.mysql.jdbc.Driver");
        //2.连接数据库,代表数据库
        Connection connection = DriverManager.getConnection(url, username, password);

        //3.编写SQL
        String sql = "insert into  users(id, name, password, email, birthday) values (?,?,?,?,?);";

        //4.预编译
        PreparedStatement preparedStatement = connection.prepareStatement(sql);

        preparedStatement.setInt(1,2);//给第一个占位符？ 的值赋值为1；
        preparedStatement.setString(2,"狂神说Java");//给第二个占位符？ 的值赋值为狂神说Java；
        preparedStatement.setString(3,"123456");//给第三个占位符？ 的值赋值为123456；
        preparedStatement.setString(4,"24736743@qq.com");//给第四个占位符？ 的值赋值为1；
        preparedStatement.setDate(5,new Date(new java.util.Date().getTime()));//给第五个占位符？ 的值赋值为new Date(new java.util.Date().getTime())；

        //5.执行SQL
        int i = preparedStatement.executeUpdate();

        if (i>0){
            System.out.println("插入成功@");
        }

        //6.关闭连接，释放资源（一定要做） 先开后关
        preparedStatement.close();
        connection.close();
    }
}

```



**事务**

要么都成功，要么都失败！

ACID原则：保证数据的安全。

```java
开启事务
事务提交  commit()
事务回滚  rollback()
关闭事务

转账：
A:1000
B:1000
    
A(900)   --100-->   B(1100) 
```



**Junit单元测试**

依赖

```xml
<!--单元测试-->
<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.12</version>
</dependency>
```

简单使用

@Test注解只有在方法上有效，只要加了这个注解的方法，就可以直接运行！

```java
@Test
public void test(){
    System.out.println("Hello");
}
```

![1568442261610](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568442261610.png)

失败的时候是红色：

![1568442289597](https://cdn.jsdelivr.net/gh/oddfar/static/img/JavaWeb.assets/1568442289597.png)



**搭建一个环境**

```sql
CREATE TABLE account(
   id INT PRIMARY KEY AUTO_INCREMENT,
   `name` VARCHAR(40),
   money FLOAT
);

INSERT INTO account(`name`,money) VALUES('A',1000);
INSERT INTO account(`name`,money) VALUES('B',1000);
INSERT INTO account(`name`,money) VALUES('C',1000);
```

```java
    @Test
    public void test() {
        //配置信息
        //useUnicode=true&characterEncoding=utf-8 解决中文乱码
        String url="jdbc:mysql://localhost:3306/jdbc?useUnicode=true&characterEncoding=utf-8";
        String username = "root";
        String password = "123456";

        Connection connection = null;

        //1.加载驱动
        try {
            Class.forName("com.mysql.jdbc.Driver");
            //2.连接数据库,代表数据库
             connection = DriverManager.getConnection(url, username, password);

            //3.通知数据库开启事务,false 开启
            connection.setAutoCommit(false);

            String sql = "update account set money = money-100 where name = 'A'";
            connection.prepareStatement(sql).executeUpdate();

            //制造错误
            //int i = 1/0;

            String sql2 = "update account set money = money+100 where name = 'B'";
            connection.prepareStatement(sql2).executeUpdate();

            connection.commit();//以上两条SQL都执行成功了，就提交事务！
            System.out.println("success");
        } catch (Exception e) {
            try {
                //如果出现异常，就通知数据库回滚事务
                connection.rollback();
            } catch (SQLException e1) {
                e1.printStackTrace();
            }
            e.printStackTrace();
        }finally {
            try {
                connection.close();
            } catch (SQLException e) {
                e.printStackTrace();
            }
        }
    }
```

## 15、数据库连接池

**概念：其实就是一个容器(集合)，存放数据库连接的容器。**
当系统初始化好后，容器被创建，容器中会申请一些连接对象，当用户来访问数据库时，从容器中获取连接对象，用户访问完之后，会将连接对象归还给容器。
**好处：**

1. 节约资源
2. 用户访问高效

**实现：**
标准接口：`DataSource   javax.sql`包下的

1. 方法：

>获取连接：`getConnection()`
>归还连接：`Connection.close()`。
>如果连接对象Connection是从连接池中获取的，那么调用`Connection.close()`方法，则不会再关闭连接了。而是归还连接

2. 一般我们不去实现它，有数据库厂商来实现

>1. C3P0：数据库连接池技术
>2. Druid：数据库连接池实现技术，由阿里巴巴提供的


**C3P0：数据库连接池技术**

- 步骤：

1. 导入jar包 (两个) c3p0-0.9.5.2.jar mchange-commons-java-0.2.12.jar ，
   *不要忘记导入数据库驱动 `jar` 包*
2. 定义配置文件：

>名称： `c3p0.properties` 或者 `c3p0-config.xml`
>路径：直接将文件放在src目录下即可。

3. 创建核心对象 数据库连接池对象 `ComboPooledDataSource()`
4. 获取连接：`getConnection()`

- 代码：

```java
//1.创建数据库连接池对象
DataSource ds  = new ComboPooledDataSource();
//2. 获取连接对象
Connection conn = ds.getConnection();
```

**Druid：数据库连接池实现技术，由阿里巴巴提供的**

- 步骤：

1. 导入jar包 `druid-1.0.9.jar`
2. 定义配置文件：
   * 是`properties`形式的*
   * 可以叫任意名称，可以放在任意目录下*
3. 加载配置文件。`Properties`
4. 获取数据库连接池对象：通过工厂来来获取  `DruidDataSourceFactory()`
5. 获取连接：`getConnection()`

- 代码：

```
//3.加载配置文件
Properties pro = new Properties();
InputStream is = DruidDemo.class.getClassLoader().getResourceAsStream("druid.properties");
pro.load(is);
//4.获取连接池对象
DataSource ds = DruidDataSourceFactory.createDataSource(pro);
//5.获取连接
Connection conn = ds.getConnection();
```

**定义工具类**

1. 定义一个类 JDBCUtils
2. 提供静态代码块加载配置文件，初始化连接池对象
3. 提供方法

> 1. 获取连接方法：通过数据库连接池获取连接
> 2. 释放资源
> 3. 获取连接池的方法


**代码：**

```Java
public class JDBCUtils {

    //1.定义成员变量 DataSource
    private static DataSource ds ;

    static{
        try {
            //1.加载配置文件
            Properties pro = new Properties();
            pro.load(JDBCUtils.class.getClassLoader().getResourceAsStream("druid.properties"));
            //2.获取DataSource
            ds = DruidDataSourceFactory.createDataSource(pro);
        } catch (IOException e) {
            e.printStackTrace();
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    /**
     * 获取连接
     */
    public static Connection getConnection() throws SQLException {
        return ds.getConnection();
    }

    /**
     * 释放资源
     */
    public static void close(Statement stmt,Connection conn){
			       /* if(stmt != null){
			            try {
			                stmt.close();
			            } catch (SQLException e) {
			                e.printStackTrace();
			            }
			        }
			
			        if(conn != null){
			            try {
			                conn.close();//归还连接
			            } catch (SQLException e) {
			                e.printStackTrace();
			            }
			        }*/

        close(null,stmt,conn);
    }


    public static void close(ResultSet rs , Statement stmt, Connection conn){
        
        if(rs != null){
            try {
                rs.close();
            } catch (SQLException e) {
                e.printStackTrace();
            }
        }
        if(stmt != null){
            try {
                stmt.close();
            } catch (SQLException e) {
                e.printStackTrace();
            }
        }

        if(conn != null){
            try {
                conn.close();//归还连接
            } catch (SQLException e) {
                e.printStackTrace();
            }
        }
    }

    /**
     * 获取连接池方法
     */

    public static DataSource getDataSource(){
        return  ds;
    }
}
```




