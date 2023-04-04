[TOC]



#杂

## Git使用

[Java线上环境安装说明](http://47.97.82.68:8080/49th/Java线上环境安装说明.html?ws=none&cf=off#git的使用)

## 开发编程规约

[Java开发编程规约](http://47.97.82.68:8080/49th/Java开发编程规约.html)

## 命名规范

### 类和接口的命名规则

> 单个单词/多个单词
>
> 单个单词：首字母大写
>
> 多个单词：每个单词首字母大写（驼峰命名）

### 变量和方法的命名规则

> 单个单词：全部小写
>
> 多个单词：第一个单词首字母小写，从第二个单词开始每个单词首字母大写，如：danZiupan

### 常量的命名规则

> 单个：所有字母全部大写，如MAX，MIN
>
> 多个：如上，单词之间以下划线分隔，如MAX_VALUE



## 一些快捷键

> * 开发中写强转的快捷方式:
>                   1.在要强转数据后面加".cast"回车
>                   2.alt + 回车 报错的地方
> * 对于表达式的处理,可以考虑接收,也可以考虑直接输出
>               都可以使用相应的快捷键
>               如果想要直接输出,可以用".sout"/".soutv"回车
>               如果想要用变量接收,可以用两种方式:
>                   1.".var"回车
>                   2.快捷键ctrl+alt+V
>               注意事项:
>               为了写代码更有效率,并且写出更安全的代码
>               推荐在写有"="的等式,赋值语句时,从右往左写
>               右边写完,自动生成左边,不要手写从左往右



## 关于sourcetree



## JavaSE经典面试题

> 1. ==和equals比较的区别？
> 2. 为什么重写 equals 还要重写 hashcode？
> 3. 为啥有时会出现 4.0 - 3.6 = 0.40000001 这种现象？
> 4. final 关键字的作用
> 5. 介绍 Java 的集合类
> 6. ArrayList 和 LinkedList 的区别
>
> 



---





# 语法基础

## [**初识Java**](http://47.97.82.68:8080/49th/SE01/V1/01_初识Java.html?ws=none&cf=off)

### Java运行原理

![image-20230227102556416](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230227102556416.png)

####问题：解释执行？

> **解释执行是指将编译好的字节码一行一行地翻译为机器码执行**

解释执行和编译执行的区别（[Java解释执行和编译执行 - 九·思 - 博客园 (cnblogs.com)](https://www.cnblogs.com/lingz/p/9394238.html)）：

> ```
> 解释执行：将编译好的字节码一行一行地翻译为机器码执行。
> 
> 编译执行：以方法为单位，将字节码一次性翻译为机器码后执行。
> ```



### Java语言的特点

- 跨平台

- 面向对象

- 解释型

  高级语言计算机本身是不认识的（只认识二进制），因此需要一个工具将高级语言转化为二进制语言

  1.编译型语言：用这种语言写出的代码，会一次性通过编译器的编译转化为目标代码（二进制文件 如.exe），然后依次在操作系统上运行。

  2.解释型语言：转化一句，执行一句

  Java程序执行过程：.java --> .class --> java虚拟机（jvm）

- 健壮性

- 动态性

- 分布性 

  java.net库是专门用于网络通信的

- 高效性

- 多线程

- 结构中立（字节码）

- 开源

- 跨平台性

  跨平台性的实现原理：**Java程序是在Java虚拟机（jvm）上运行**，而非直接运行于操作系统

![image-20230129000742615](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129000742615.png)

注意：**jvm不跨平台**

java之所以能跨平台就是以jvm不跨平台为代价，每一种操作系统都对应一种jvm

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129001142084.png" alt="image-20230129001142084" style="zoom:67%;" />

## [**Java开发环境基础配置**](http://47.97.82.68:8080/49th/SE01/V1/02_Java开发环境基础配置.html?ws=none&cf=off)

### 线上环境安装

http://47.97.82.68:8080/49th/Java%E7%BA%BF%E4%B8%8A%E7%8E%AF%E5%A2%83%E5%AE%89%E8%A3%85%E8%AF%B4%E6%98%8E.html?ws=none&cf=off#git%E7%9A%84%E4%BD%BF%E7%94%A8



### JDK和JRE

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129001512524.png" alt="image-20230129001512524" style="zoom:60%;" />

#### 其他术语

![image-20230214225524770](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230214225524770.png)

#### 什么是javac和javap



### Java程序运行原理

![image-20230129002223059](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129002223059.png)





### Path和Classpath环境变量

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129110348017.png" alt="image-20230129110348017" style="zoom:50%;" />

相关博客：

[(85条消息) 通俗易懂解析环境变量及其配置_StandByMeQuan的博客-CSDN博客_大白话说环境变量](https://blog.csdn.net/qq_37872792/article/details/80642985)

[(85条消息) 为什么要配环境变量？path用来干什么？_向着自由的博客-CSDN博客_配置环境变量path的目的是什么](https://blog.csdn.net/Pre_waist_L/article/details/79696507)



### java文件编写的注意事项

- 在Java文件中只能定义一个public修饰的类，且被public修饰的类名必须和文件名相同



### IDEA使用

---

#### 创建项目

>  关于IDEA的Project
>
> **Project，即工程。它是IDEA进行项目结构管理的顶层概念 ，IDEA中进行Java开发必须要在一个Project中进行。**
>
> IDEA的 Project 具有以下特点：
>
> 1. **Project只是项目管理的顶层概念，不是物理存在于操作系统上的结构。**（这一点随后你就会明白）
>
> 2. 在操作系统层面来看，创建一个project实际上就是新建了一个文件夹。
>
> 3. 从IDEA软件层面来说，创建一个project就是创建了一个独立的工作空间。
>
> ​	当然，想要完全理解 **Project** 在IDEA中的涵义，还需要自己多多使用，多多体悟。

> **在IDEA中创建Project遵循以下步骤：**
>
> 1. 打开 File--->New--->Project或者Create New Project（反正就是要新建Project）
>
> 2. 弹窗界面中，首先会要求选择JDK版本，**请选择版本Java8**，还可以选择模板，但JavaSE部分无需选择模板，直接下一步：
>
>    
>
>    图 19. 新建Project
>
>    ![新建Project](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202202241407742.png?align=center)
>
>    
>
>    **注：这里选择的JDK版本是你装在本地的JDK，具体来说需要直接选择整个JDK目录，参考下图：**
>
>    
>
>    图 20. IDEA选择JDK目录
>
>    ![IDEA选择JDK目录](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202202241410853.png?align=center)
>
>    
>
>    1. 下一步来到给Project起名，这里稍微谈一下Project的命名：
>
>    
>
>    图 21. 新建Project—命名
>
>    ![新建Project—命名](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202202241411909.png?align=center)
>
>    
>
>    关于Project的命名问题：工程的命名格式没有固定的限制，一般具有**"见名知意"**的作用即可，也就是说工程的名字需要指出该Project的意义。
>
>    根据日常工作的普遍规律，给出几条起名的限制：
>
>    1. **工程名尽量使用正确的英语单词，如无特殊需求不要使用中文或者拼音。**
>    2. **多个单词之间建议使用下划线或者横杠连接。**
>
>    举个例子，比如我新建一个工程用于做作业，而我是Java38th的，所以我可以将Project命名为**Java38th-homework**，这样就是一个不错的命名。**当然实际开发中，可以根据公司领导的安排决定，领导喜欢叫啥都行。**
>
> 3. 新建project其它需要注意的地方：
>
>    1. **除了起名字外，Location的含义是工程存放的硬盘位置，建议单独找一个空间存放，不要直接存在默认位置。**
>    2. 其余设置都默认即可，不需要改动，点击 **Finish** 即可。
>    3. 创建完成，可以选择在当前窗口打开Project，还是在新窗口，这个自由选择即可。
>
> 这里强烈建议大家专门找一个硬盘区域用来放`idea-project`。做人要经常收拾房间，做程序员也要把自己的硬盘内容管理的井井有序。**不要直接使用默认路径（C盘或根目录），默认名（untitled）创建Project！**

> **IDEA中所有Java源代码都必须放在src目录下，才能执行。** 如下图所示：
>
> 
>
> 图 23. src目录
>
> ![src目录](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202202241407887.png?align=center)
>
> 
>
> 注：简单来说，src是英语单词"source"的缩写，代指"源代码"，这个缩写以后将会经常看到和使用。
>
> **就JavaSE阶段的学习进度而言，所有的代码都需要写在src目录下，也只有放在src目录下的代码，才可以被执行。**
>
> 知道**"src目录"**后，我们按以下步骤进行操作：
>
> 右键单击src目录，选择**New ----> Java Class**新建一个类，然后按照之前一样写main方法，具体代码如下：
>
> 代码块 2. hello world案例
>
> ```java
> //文件 HelloWorld.java中
> public class HelloWorld {
> public static void main(String[] args) {
> System.out.println("Hello World");
> }
> }
> ```
>
> 
>
> **在IDEA这种集成开发环境中，已经集成了cmd窗口控制台的作用，点击main方法左边的Run，启动main方法即可看到代码执行结果！**
>
> **最后虽然已经强调过了，但是这里还是要强调几点：**
>
> 1. public修饰类的类名必须和文件名保持一致，一个Java文件中只有一个public修饰的类，但非public类可以有多个。
>
>    **比如下面Java代码是允许的：**
>
>    代码块 3. 一个Java文件定义多个类
>
>    ```java
>     //文件 HelloWorld.java中
>    public class HelloWorld {
>     }
>    class A{}
>     class B{}
>    class C{}
>    ```
>
>    
>
>    **注：public修饰class的含义，什么是public，它的作用是什么等相关问题，我们放在后面再讲。**
>
> 2. main方法是程序的入口方法，只有存在main方法的Java类可以启动，执行其中的代码。
>
>    注：关于方法的概念，我们会在后面探讨。
>
> 3. 如果Java Class都**直接**放在src目录下，是不允许有同名的class的，包括public修饰的class和非public修饰的class！**这就好比同一个文件夹下，不允许有同名文件一样。****（这里牵扯到一个包的概念，后面会详细讲解）**
>
> ------
>
> 以上，IDEA的基本使用就结束了，下面我们讲一个比较重要的概念——Module。

####文件构成

> [IDEA | IDEA项目结构认识 - 茶哩哩 - 博客园 (cnblogs.com)](https://www.cnblogs.com/martin-1/p/14772209.html)
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129114758009.png" alt="image-20230129114758009" style="zoom:80%;" />
>
> 如何区分项目文件夹和项目?
>
> - 项目文件夹是用于储存一个个项目
> - 项目`根目录` 下 有 配置文件
>
> IDEA中的`Project`和Eclipse中的`Workspace`是类似的，相当于文件夹目录
>
> `Eclipse`中有`Workspace(工作空间)`和`Project(工程)`的概念
>
> `IDEA`中只有`Project(工程)` 和 `Module(模块)`的概念
>
> **只需要知道「新建立一个IDEA java项目」是实际是 建立 `Module` 即可**
>



#####**module和project的关系：**

[(78条消息) IntelliJ IDEA 中 Project 和 Module 的概念及区别_CG国斌的博客-CSDN博客_idea project module](https://blog.csdn.net/qq_35246620/article/details/65448689)

在 IntelliJ IDEA 中Project是最顶级的结构单元，然后就是Module，**一个Project可以有多个Module**。目前，主流的大型项目结构基本都是多Module的结构，这类项目一般是按功能划分的，比如：user-core-module、user-facade-module和user-hessian-module等等，模块之间彼此可以相互依赖。通过这些Module的命名可以看出，它们都是处于同一个项目中的模块，彼此之间是有着不可分割的业务关系。因此，我们可以大致总结出：一个Project是由一个或多个Module组成

- 当为单`Module`项目的时候，这个单独的`Module`实际上就是一个`Project`；
- 当为多`Module`项目的时候，多个模块处于同一个`Project`之中，此时彼此之间具有互相依赖的关联关系。



IDEA项目结构:

<img src="https://img2020.cnblogs.com/blog/1890468/202105/1890468-20210515175921640-1530178724.png" alt="img" style="zoom:67%;" />



> 通过在IDEA种创建两种结构Project和Module，不难发现实际上两者没有本质区别。
>
> 总得来说：**Project是概念上的顶层结构，Module是IDEA的基本单元。** 
>
> 1. IDEA中的Project不是一个独立的概念，新建一个Project的实质是创建了一个独立的Module，并且这个module的名字和project名字一样。
> 2. 一个Project可以有多个module
> 3. 主流的大型项目结构基本都是多Module的，这类项目一般是按功能划分模块，模块之间彼此可以相互依赖。
>
> **两个注意事项：**
>
> 1. **在JavaSE阶段，没有必要创建多Module的Project。即便创建了，多个module之间实际也不会相互依赖。**
> 2. 每个Project用独立的窗口打开，而不是堆在一个窗口中。



 #### module创建

如果想在当前项目中创建一个平行关系的module，需要确保创建的文件路径和当前项目中的其他module是平行的

这样多个module之间相互独立，又同属于一个项目文件夹                                                                                                                                                                                                

> 关于IDEA的module   :
>
> Project只是IDEA进行项目管理的**顶层概念**，而不是真实存在的基本单元。谁是IDEA进行Java项目开发的基本单元呢？
>
> **Module！**
>
> 实际上：
>
> **每创建一个Project，默认就会创建一个Module，并且该Module的名字和Project相同！**
>
> **每创建一个Project，默认就会创建一个Module，并且该Module的名字和Project相同！**
>
> **每创建一个Project，默认就会创建一个Module，并且该Module的名字和Project相同！**
>
> 当然，在IDEA中要想创建Module，必须在一个Project的基础上才能够完成创建。
>
> 从操作系统层面上看，每个Module也是一个独立的文件夹！

> 在IDEA中创建Module遵循以下步骤：
>
> 1. **右键任何一个Project--->New--->Module（创建Module必须在Project基础上进行）**
>
> 2. 接下来步骤大致和创建Project相同（因为创建Project本质也是新建了一个Module）
>
>    1. 选择选择JDK版本（**选择Java8**）
>    2. 无需选择模板，直接下一步
>
> 3. Module的命名，规则和Project类似，不再赘述。
>
> 4. 创建Module时，在选择路径时，可以注意一下层级关系：
>
>    
>
>    图 24. Module之间的关系
>
>    ![Module之间的关系](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202202241512636.png?align=center)
>
>    
>
>    1. **如果你希望第二个Module和第一个Module是同级关系，目录路径上要体现同级。**
>    2. **如果你希望第二个Module和第一个Module是上下级关系，目录路径上要体现上下级。**
>
> 5. 上述设置完成后，其它设置保持默认即可。最后点击**Finish**，即完成创建Module。
>
> 至此，IDEA当中的项目管理结构你基本已经知道了，可以开始写代码了！





#### 导入外部项目

[第2天-25 导入外部项目步骤_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV15f4y1R7eM?p=67&vd_source=6d1909c0a76203ae4ee4729da314f213)



#### Debug



###包的概念

---

在IDEA当中写Java代码，存在包的概念。**Java当中的包有点类似于操作系统中的文件夹，但又不同于文件夹。**

包是一个非常基础的概念，下面来讲解一下。

> 包的概念：
>
> - 类似于操作系统以文件夹来管理文件，Java以包来管理类，方便组织和维护
> - 并且类似于操作系统，可以避免无法重名的问题，这样即使不同包之间有相同命名的类，也不会冲突，在团队合作中很有帮助
>



####包的创建

> 在IDEA的工程（module）下，可以：
>
> **右键src目录 --> new --> package**来创建包（这里不再配图，因为比较简单）。
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230227113301550.png" alt="image-20230227113301550" style="zoom:33%;" />
>
> 注意：
>
> 1. 如果直接输入一个字符串就是创建一级包名。
> 2. 如果想要创建多级包，**那么每级包名之间用"."隔开。**
> 3. 包名的字符串并不是任意给出的，具体的规范参考文档：[包名的命名规范](http://47.97.82.68:8080/49th/SE01/V1/05_Java变量概述与使用.html?ws=none#具体规范)。



#### 包的命名规则

> 为了保证包名的唯一，以域名反转的形式来命名包
>
> 如baidu.com，经过反转就是com.baidu
>
> ![image-20230129142952848](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129142952848.png)
>
> 
>
> 
>
> 包又可以分为单级包和多级包：
>
> 单级包：以小写字母作为包名
>
> 多级包：以域名反转的形式作为包名，单词全部小写
>



####包的作用

Java中的包（package）主要有两个作用：

1. **用来区分同名Java类，同包中不能有两个同名的Java class。**（一个文件夹中也不允许有两个同名文件）
2. 所谓的包，在操作系统中，就是一个文件夹。
3. 包还可以用来划分**访问权限**。（面向对象详细讲，这里先略过）

> 之前在写"Hello World"案例时，已经强调过一个概念了：
>
> **一个Java文件中，只能有一个public修饰的类，并且该public class的类名必须和Java文件的名字保持一致。**
>
> 所以，一个Java文件下，实际上可以定义多个非public修饰的类，那么**这些非public类和public类是什么关系呢？**
>
> 是同包的关系！
>
> 所以下面的类结构是不允许的！
>
> 图 25. **同包下不允许同名类**
>
> <img src="https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202205301819687.png?align=center" alt="同包下不允许同名类" style="zoom:33%;" />
>
> 
>
> **Demo.java下有一个public class Demo，还有一个非public class A是不允许的！**因为同包下已经存在一个public class A了！



## [**IDEA常用操作和软件推荐**](http://47.97.82.68:8080/49th/SE01/V1/03_IDEA常用操作和软件推荐.html?ws=none&cf=off)

### IDEA常用操作

####导入和打开IDEA项目

> **对于已有的IDEA工程（例如老师每天传的代码）是可以直接用IDEA打开的，逐个点击其中的Java文件查看代码是很低效的！**
>
> 点击IDEA左上角，**File ---> Open ---> 选择目标工程文件**，IDEA工程在选择打开时是有特殊图标的，如下图：
>
> 
>
> 图 1. 可以打开的idea工程
>
> ![image-20230218160216233](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230218160216233.png)
>
> 
>
> **普通文件夹是没有这个黑色的小格子的，这是IDEA工程的标记！打开后，就可以正常查看Project中的代码，并且能够运行。**
>
> 如果代码不能运行，可以找同学研究一下或者直接提问老师。



##### 打开最近的Project

> 很多时候，我们需要打开之前已经打开过的Project，做法参考下面：
>
> 点击IDEA左上角，**File ---> Open Recent** ，即可选择打开最近的工程。如下图：
>
> 
>
> 图 2. 打开最近的Project
>
> ![打开最近的Project](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202201221509299.png?align=center)
>
> 当然这个操作，只能打开你已经打开过的Project，如果想要打开还未打开过的Project，请参考上一条。



##### 文件的重命名和删除

> 如果有文件重命名和删除的需求，可以右键某个文件或者文件夹，参考以下图片，进行相关操作，也可以记下相关快捷键。
>
> 
>
> 图 3. IDEA-删除和重命名
>
> <img src="https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202111091607826.png?align=center" alt="IDEA-删除和重命名" style="zoom: 50%;" />
>
> 
>
> 快捷键即重命名：**Shift + F6**  、删除：**Delete**

##### 包路径折叠与打开

> 在开发中，在src目录创建一个多级包目录来写代码是非常常见的，如下图所示：
>
> 
>
> 图 4. 多级包目录
>
> <img src="https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202201221553782.png?align=center" alt="多级包目录" style="zoom:50%;" />
>
> 
>
> 这就是一个具有**多级包目录**的Module，stage1。
>
> 实际开发中，这种**多级包目录**也是非常常见的，像上图中，是完全打开多级包目录，当然你也可以选择折叠其中的空包。
>
> 按照下图点击图中的螺丝图标：
>
> 
>
> 图 5. 折叠包目录按钮
>
> ![折叠包目录按钮](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202201221601089.png?align=center)
>
> 
>
> 在打开的菜单中，点击：
>
> 
>
> 图 6. 折叠多级包目录
>
> <img src="https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202201221602446.png?align=center" alt="折叠多级包目录" style="zoom:33%;" />
>
> 
>
> 这样就可以折叠多级空包目录，效果如下：
>
> 
>
> 图 7. 折叠多级空包目录效果图
>
> <img src="https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202201221603935.png?align=center" alt="折叠多级空包目录效果图" style="zoom:33%;" />
>
> 
>
> **这个选项菜单中的其它按钮，你也可以试一试效果，总之多摸索摸索，熟悉了就好了。**



#### IDEA必要设置

#### IDEA设置杂项

#### IDEA插件

#### IDEA快捷键

> main方法：psvm
>
> 输出：sout
>
> **格式化代码 ：Ctrl+Alt+L**

### 常用优秀软件



## Java语法基本概念

---

### 程序的概念

> 程序是指令的合集，但是并不是什么指令都能够被计算机识别，而是存在一定规范或者说语法的。Java程序指的是通过Java语言编写的，符合Java语法的，能够被计算机识别和执行的指令合集。在Java的规范中，Java程序的指令合集（代码）必须遵循：
>
> 1. 首先新建一个Java文件。
> 2. 在文件中创建类（class），所有代码都必须写在类中。
> 3. Java程序要想启动，必须有main方法，**main方法是Java程序的入口方法**。
> 4. 所有需要执行的代码（指令），都必须 **直接或间接** 的写在main方法中。
> 5. 任何要执行的代码（指令），都必须遵守Java语法规范。
>
> 相信很多同学已经发现了，一旦写出了不遵守上述规范或者不符合Java语法的代码：
>
> Java的源文件就不能通过`javac`命令编译生成class字节码文件了，称之为 **"编译失败"** 。
>
> 在IDEA中写代码时，会表现为：语法错误处出现红色波浪线，点击会显示错误信息。这时启动main方法（如果有的话）就会报错，并在控制台打印编译失败的信息。（这里具体的图我就不贴了，你都可以自己尝试一下。）



### 关键字和保留字

#### 关键字

> > 什么是关键字（keyword）？关键字有什么特点？
> >
> > 关键字的定义是：关键字是被Java语法赋予特定含义的单词。
> >
> > 关键字的特点是：**关键字都是合法的单词，而且单词字母必须全部小写。** 
> >
> > **总得来说，关键字是Java语法中具有特定、特殊含义的小写形式英文单词。**
>
> > 关键字有什么作用？
> >
> > 其实上述定义已经说明了它的作用，关键字在Java语法中都有特定的含义，**它对编译器具有特殊意义，能够影响编译！**具体来说，关键字往往都用来表示一种程序的结构或者修饰一些程序的结构等等。当然更具体的含义，要针对不同的关键字来说明。
> >
> > 这里举一个非常常见的案例：
> >
> > class是最常见的关键字之一，它用来表示当前代码中定义了一个类（这样的程序结构）。

##### 修饰符

> > 在Java中，关键字总体可分为两大类：修饰符和非修饰符。修饰符是典型的关键字，如它的名字一样，修饰符是用来修饰"别人"的单词。比如用来修饰一个类，修饰一个方法等等的关键字都是修饰符。
> >
> > 修饰符（modifier）总体上还可以再分两类：
> >
> > 1. **访问权限修饰符**，例如：
> >    1. **private**
> >    2. 缺省的默认权限**（什么关键字都不写）**
> >    3. **protected**
> >    4. **public**
> > 2. **非访问权限修饰符**，例如：
> >    1. final
> >    2. abstract
> >    3. static
> >    4. ...
>
> > 注：访问权限修饰符，其它修饰符，等到**面向对象**知识点时会详谈，这里大家可以先留个印象即可！
> >
> > 没有太大必要死记上述概念，简单了解即可，等用多了自然而然就熟练了。

##### 非修饰符

> 非修饰符实际上远比修饰符更多，非修饰符往往用来表示程序结构，表示要在程序中定义XXX等，就比如上面说的class就属于这个分类当中。当然还有一些其它的非修饰符，等到我们学到的时候再详细说。



#### 保留字





#### 注释

---

> ##### 单行注释
>
> //
>
> ##### 多行注释
>
> /* */
>
> ##### 文档注释
>
> /** 注释内容 */	
>







#### 进制

---

所谓x进制就是逢x进1



##### 不同进制中间转换



##### 不同进制数的Java表示

1. 二进制（binary）：0，1，满二进一。以0b或0B开头。
2. 十进制（decimal）：0-9，满10进1.
3. 八进制（octal）：0-7，满8进1.以数字0开头表示。
4. 十六进制（hex）：0-9和A-F，满16进1。以0x或0X开头表示。注意：A-F不区分大小写。比如 0X12AB=0x12ab。

```java
public class decimal {
    public static void main(String[] args){
        System.out.println("二进制："+0b110);
        System.out.println("八进制："+011);
        System.out.println("十六进制："+0x11);
    }
}

二进制：6
八进制：9
十六进制：17
```



##### 负数如何表示



####变量

---

变量的值其实就是存储在一个内存空间中的值

##### 数据类型

<img src="https://img-blog.csdnimg.cn/20190211164317916.jpg#pic_center" alt="数据类型分类" style="zoom:80%;" />

格式：数据类型 变量名 = 变量值

内存管理系统根据变量的类型为变量分配存储空间，分配的空间只能用来储存该类型数据。

因此，通过定义不同类型的变量，可以在内存中储存整数、小数或者字符。

Java 的两大数据类型:

- 内置数据类型

- 引用数据类型

  

内置数据类型：



##### 数据类型的转化

java编译器禁止把大类型的值赋值给小类型，反过来就可以

但事实上jvm要求参与运算的值必须是相同类型，如int+byte时，jvm会先把byte读取出来并转化为int类型（小的类型转化为大的类型）再进行运算，这里就涉及到数据类型的转化规则：

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129164135752.png" alt="image-20230129164135752" style="zoom:50%;" />



##### 面试题

```java
byte b1 = 1,b2 = 2,b;
b = b1 + b2;
b = 1+2;
Q：哪句会编译失败？为什么？
A：
    第一句会报错，看上面那张图，两个byte类型的数据参与运算会首先转化为int的类型，并且因为是变量，和常量不同，是会变化的，编译器为了保险起见，就会报错。
    第二句：1和2是字面型常量，而字面型常量的值是固定的，可以理解为编译器可以直接得知对应的值并计算一下看看会不会超出范围，而byte类型可表示的输指范围是-128~127，所以不会报错，而如果b2的值改为200，则超出可表示范围，就会报错。
```

🔺具体分析：[(78条消息) Java千问：Java语言中为byte和short类型变量赋值为啥会报错？_穆哥学堂的博客-CSDN博客](https://blog.csdn.net/shalimu/article/details/103662342#:~:text=如果编译器认为所,就会报语法错误。)



##### 变量的作用域

![image-20230129191322899](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129191322899.png)



####运算符

---

##### 算术运算符

- 加法运算符：

- 除法运算符：

  当参与/运算的两个操作数都是整数时，表示整数除法；否则，表示浮点数除法，如：

  ```java
  15/2 = 7
  15.0/2 = 7.5
  ```

- 自增自减运算符：

  **1、自增（++）自减（--）运算符**是一种特殊的算术运算符，在算术运算符中需要两个操作数来进行运算，而自增自减运算符是一个操作数。

  **2、前缀自增自减法(++a,--a):** 先进行自增或者自减运算，再进行表达式运算。

  **3、后缀自增自减法(a++,a--):** 先进行表达式运算，再进行自增或者自减运算 实例：



#####赋值运算符



#####比较运算符



##### instanceof 运算符

该运算符用于操作对象实例，检查该对象是否是一个特定类型（类类型或接口类型）。

instanceof运算符使用格式如下：

```java
( Object reference variable ) instanceof  (class/interface type)
```

如果运算符左侧变量所指的对象，是操作符右侧类或接口(class/interface)的一个对象，那么结果为真。

下面是一个例子：

```java
String name = "James";
boolean result = name instanceof String; // 由于 name 是 String 类型，所以返回真
```

如果被比较的对象兼容于右侧类型，该运算符仍然返回 true。

看下面的例子：

```java
class Vehicle {}
 
public class Car extends Vehicle {
   public static void main(String[] args){
      Vehicle a = new Car();
      boolean result =  a instanceof Car;
      System.out.println( result);
   }
}
```

以上实例编译运行结果如下：

```
true
```



##### 逻辑运算符

下表列出了逻辑运算符的基本运算，假设布尔变量A为真，变量B为假

| 操作符 | 描述                                                         | 例子                |
| :----- | :----------------------------------------------------------- | :------------------ |
| &&     | 称为逻辑与运算符。当且仅当两个操作数都为真，条件才为真。     | （A && B）为假。    |
| \| \|  | 称为逻辑或操作符。如果任何两个操作数任何一个为真，条件为真。 | （A \| \| B）为真。 |
| ！     | 称为逻辑非运算符。用来反转操作数的逻辑状态。如果条件为true，则逻辑非运算符将得到false。 | ！（A && B）为真。  |

下面的简单示例程序演示了逻辑运算符。复制并粘贴下面的Java程序并保存为Test.java文件，然后编译并运行这个程序：

```java
public class Test {
  public static void main(String[] args) {
     boolean a = true;
     boolean b = false;
     System.out.println("a && b = " + (a&&b));
     System.out.println("a || b = " + (a||b) );
     System.out.println("!(a && b) = " + !(a && b));
  }
}
```

以上实例编译运行结果如下：

```java
a && b = false
a || b = true
!(a && b) = true
```

单与和双与的区别：

[(78条消息) Java-逻辑运算符与短路运算符_武梓龙_Arvin的博客-CSDN博客_短路与运算符是哪个](https://blog.csdn.net/weixin_45490198/article/details/124966369)



#####异或运算符

^：**相同为false，不同为true**

eg.

true ^ true = false

false ^ flase = false

true ^ false = true

 

##### 位运算符

Java定义了位运算符，应用于整数类型(int)，长整型(long)，短整型(short)，字符型(char)，和字节型(byte)等类型。

位运算符作用在所有的位上，并且按位运算。假设a = 60，b = 13;它们的二进制格式表示将如下：

```java
A = 0011 1100
B = 0000 1101
-----------------
A&B = 0000 1100
A | B = 0011 1101
A ^ B = 0011 0001
~A= 1100 0011
```

下表列出了位运算符的基本运算，假设整数变量 A 的值为 60 和变量 B 的值为 13：

| 操作符 | 描述                                                         | 例子                           |
| :----- | :----------------------------------------------------------- | :----------------------------- |
| ＆     | 如果相对应位都是1，则结果为1，否则为0                        | （A＆B），得到12，即0000 1100  |
| \|     | 如果相对应位都是 0，则结果为 0，否则为 1                     | （A \| B）得到61，即 0011 1101 |
| ^      | 如果相对应位值相同，则结果为0，否则为1                       | （A ^ B）得到49，即 0011 0001  |
| 〜     | 按位取反运算符翻转操作数的每一位，即0变成1，1变成0。         | （〜A）得到-61，即1100 0011    |
| <<     | 按位左移运算符。左操作数按位左移右操作数指定的位数。         | A << 2得到240，即 1111 0000    |
| >>     | 按位右移运算符。左操作数按位右移右操作数指定的位数。         | A >> 2得到15即 1111            |
| >>>    | 按位右移补零操作符。左操作数的值按右操作数指定的位数右移，移动得到的空位以零填充（**即不含符号位的右移**）。 | A>>>2得到15即0000 1111         |

关于异或^:

1.一个数和它自己异或，a ^ a = 0

2.0和任何一个数异或都等于这个数，0 ^ a = a



######面试题

1.请用最有效率的方式写出计算2*8的结果

​	![image-20230130000233949](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230130000233949.png)

如果直接用乘法运算符，计算机如a = 2,b = 8,a*b,计算机既要拿到a对应内存中的数据，又要拿到b对应内存中的数据，效率并不高，而位运算可以更快速地计算出结果

2.请自己实现两个整数变量的交换

方法一：定义中间变量tmp（开发中最常用）

```java
int a = 2;
        int b = 10;

        //方法一
        int tmp = 0;
        tmp = a;
        a =b;
        b = tmp;
        System.out.println("a:"+a);
        System.out.println("b:"+b);
```

方法二：

```java
//方法二
        a = a + b;
        b = a - b;
        a = a - b;
        System.out.println("a:"+a);
        System.out.println("b:"+b);
```

方法三：

```java
//方法三
a = a ^ b;
b = a ^ b;//相当于a^(b^b)
a = a ^ b;//相当于(a^a)^b
System.out.println("a:"+a);
System.out.println("b:"+b);
```

方法四：

```java
//方法四
a = (a+b) - (b = a);
System.out.println("a:"+a);
System.out.println("b:"+b);
```

​	

#####三目运算符

> 格式：**关系表达式？表达式1：表达式2**
>
> 如果关系表达式结果为true，运算后的结果是表达式1，如果为false，结果是表达式2
>
> 实例：
>
> 1.判断相等
>
> ```java
> Scanner sc = new Scanner(System.in);
> int a = sc.nextInt();
> int b = sc.nextInt();
> 
> String s = a == b ? "相等":"不相等";
> System.out.println(s);
> ```
>
> 2.三数取大
>
> ```java
> //三数取大
> 
> //形式一
> Scanner sc = new Scanner(System.in);
> int a = sc.nextInt();
> int b = sc.nextInt();
> int c = sc.nextInt();
> int tmp = a > b ? a:b;
> int result = c > tmp ? c:tmp;
> System.out.println(result);
> 
> //形式二
> Scanner sc = new Scanner(System.in);
> int a = sc.nextInt();
> int b = sc.nextInt();
> int c = sc.nextInt();
> int result = c > (a > b ? a:b) ? c:(a > b ? a:b);
> System.out.println(result);
> ```
>



## 输入与输出

---

### 键盘录入数据

如何使用？

1.导入对应包

```java
import java.util.Scanner;
```

2.创建对象

```java
//构造一个与“标准输入流”System.in关联的Scanner对象
Scanner sc = new Scanner(System.in);
```

3.读取键盘输入数据

```java
//读取整数
int x = sc.nextInt();

//读取字符串（中间可能包含空格）
String x = sc.nextLine();

//若指向读取一个单词（以空格作为分隔符）
String x = sc.next();
```

其他方法：

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230214231317615.png" alt="image-20230214231317615" style="zoom:50%;" />

4.用完之后关闭对象

```java
sc.close();
```



###Scanner补充

---



#### 关于跳过键盘录入的情况：

```java
package com.cskaoyan.javase.basic._5scanner;

import java.util.Scanner;

/**
 * Scanner使用细节
 * 如果存在多种数据类型的数据输入,一定要注意,很容易出现跳过键盘录入的情况
 *
 *
 * @since 11:36
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo2 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        // 请键盘接收一个int整数
        System.out.println("请键盘录入一个int整数:");
        int num = sc.nextInt();


        // 请键盘接收一个String字符串
        System.out.println("请键盘录入一个String字符串:");
        String str = sc.nextLine();

        System.out.println("num = " + num);
        System.out.println("str = " + str);
        // 这里键盘接收的是一个长度为0的字符串,是一个绝对空字符串,什么都没有的字符串
        /*
            在计算机的编码设定中,ASCII码表中,编码值为0的字符就是一个绝对空字符
            这个字符表示什么都没有
         */
        System.out.println(str.length());

        String str2 = "";
        System.out.println(str2.length());
    }
}

```

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230228130531732.png" alt="image-20230228130531732" style="zoom:50%;" />

> 原因：
>
> Scanner的使用问题，**next()、nextInt()等一系列方法**和nextLine()的区别：
>
> 1. **next()、nextInt()等一系列方法**
>    1. next()之类的一系列方法遇见第一个有效字符（非空格，非换行符，非制表符）时，开始扫描
>    2. 当遇见第一个分隔符或结束符(空格、换行符或者制表符)时，结束扫描，获取扫描到的内容
>    3. 即获得第一个扫描到的不含空格、换行符的单个字符串
> 2. **nextLine()方法**
>    1. 从方法名上就可以看出来，这个方法是获取一行的内容作为一个字符串被接收
>    2. 该方法不会因为空格或制表符号而结束扫描
>    3. 只会因为回车（换行）而结束扫描

> 由于nextLine()方法碰到换行才结束扫描的特性，所以使用有如下问题：
>
> 当使用Scanner接收数值类型后又使用nextLine()方法接收字符串时，例如以下代码：
>
> 代码块 4. 混用两种Scanner方法
>
> ```
> Scanner sc = new Scanner(System.in);
> ```
>
> ```
> sc.nextInt();
> ```
>
> ```
> sc.nextLine();
> ```
>
> 
>
> 输入数值后回车，会导致程序并不会等待并接收一个字符串，而是直接结束键盘录入。究其原因在于，nextLine()方法碰到回车就结束扫描，所以**该方法此时接收的实际上是一个（绝对）空字符串。**
>
> 解决的办法有很多种：
>
> 1. 可以使用不同的Scanner对象接收，这样肯定不存在冲突问题
>
> 2. 在接收int数据的后面加一个不接收数据的nextLine用来接收回车
>
> 3. 用next()方法接收字符串，但是需要注意该方法以分隔符结束，不再是接收一行了
>
> 4. 可以统一用字符串接收数值类型，接收完毕后再进行类型转换。（具体怎么做，可以自行百度一下）
>
>    > 例如转换成int类型（传入一个字符串，转换成int接收即可）
>    >
>    > Integer.parseInt()

解决办法：

```java
package com.cskaoyan.javase.basic._5scanner;

import java.util.Scanner;

/**
 * 怎么解决Scanner在混合录入多种数据类型,尤其是需要混合录入String,int等数据类型时发生的跳过录入的情况?
 * 建议在这种情况下,键盘录入仅使用同一个方法nextLine
 * 把所有的数据类型都当成字符串来接收,然后再把字符串转换成各种需要的数据类型
 * 这时不会出现任何跳过录入的情况
 *
 * @since 11:42
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo3 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        // 请键盘接收一个int整数,为了避免跳过录入,选择nextline方法
        System.out.println("请键盘录入一个int整数:");
        String numStr = sc.nextLine();
        // String --> int ?
        /*
            String myString = "1234";
            int foo = Integer.parseInt(myString);
         */
        int num = Integer.parseInt(numStr);


        // 请键盘接收一个String字符串
        System.out.println("请键盘录入一个String字符串:");
        String str = sc.nextLine();

        System.out.println("num = " + num);
        System.out.println("str = " + str);

    }
}

```

其他如str转double：double doubleType = Double.parseDouble(doubleStr);、



### 格式化输出

![image-20230214231707399](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230214231707399.png)







## [**Java变量概述与使用**](http://47.97.82.68:8080/49th/SE01/V1/05_Java变量概述与使用.html?ws=none&cf=off)

---

### 概述

> 「 **该节的内容都与Java变量有关，都非常重要。下面提供思维导图，为大致的知识网络**」
>
> 
>
> 图 1. Java变量-思维导图
>
> ![Java变量-思维导图](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202112220949859.png?align=center)
>
> 
>
> 思维导图可以帮助组织知识体系，但是我给出的思维导图细节部分并没有给出，大家可以在复习时自行补全。



### 数据类型

#### 什么是数据类型？

数据类型=数据+操作

#### 数据类型的分类

从大的分类角度来说，Java实际上只有两种数据类型：

1. **基本数据类型**
2. **引用数据类型**

---

##### 基本数据类型

###### 整型

###### 浮点型



###### 数值基本数据类型的取值范围（重要）

「 **基本数据类型中的整型和浮点型都是表示纯粹的数值的，所以它们能够表示的数值范围我们必须要知道！**」

字符型char虽然表示字符，但实际上也仍然是存储字符的编码值，所以char类型也存在一个取值范围。

整型的取值范围是很容易得到的，通过数值位的长度n**（数值位 = 总位数 -1）**可以直接算出最大值是2n -1，最小值则是-2n 。

浮点型的取值范围并不是一个普通的区间，严格来说它很复杂，下面表格给出的取值范围只是一个大概值，并不十分准确。如果你想了解最准确的浮点型取值范围，还是请查看 [补充知识点_IEEE754标准](http://47.97.82.68:8080/49th/SE01/V1/09_补充_IEEE754标准.html?ws=none) 学习。

###### 

表 1. Java数值类型的取值范围

| 基本数据类型 | 字节长度 | 大小（位） | 最小值 | 最大值 | 取值范围                                                  |
| ------------ | -------- | ---------- | ------ | ------ | --------------------------------------------------------- |
| **byte**     | 1字节    | 8bit       | -2^7   | 2^7-1  | -128 ~ 127                                                |
| **short**    | 2字节    | 16bit      | -2^15  | 2^15-1 | -32768 ~ 32767                                            |
| **int**      | 4字节    | 32bit      | -2^31  | 2^31-1 | -2147483648 ~ 2147483647（21亿出头）                      |
| **long**     | 8字节    | 64bit      | -2^63  | 2^63-1 | -9223372036854774808 ~ 9223372036854774807（大概922亿亿） |
| **float**    | 4字节    | 32bit      | -      | -      | 大约  ±3.403E38（有效位数7~8位）                          |
| **double**   | 8字节    | 64bit      | -      | -      | 大约  ±1.798E308（有效数字16~17位）                       |
| **char**     | 2字节    | 16bit      | 0      | 2^16-1 | 0 ~ 65535，编码值必须是一个正整数                         |

### 标识符

就跟父母给孩子起名字也不是乱起的一样，标识符在命名时，也有自己的独特规范，称之为"标识符命名规范"。 **一名合格的Java程序员，应该从写好标识符的命名规范开始。**



#### 约定俗成的规范

> **在符合语法的前提下，标识符还有一套约定俗成的命名规则。**
>
> 详细内容可以参考 [王道Java开发编程规约](http://47.97.82.68:8080/49th/Java开发编程规约.html) ，我们后面会详细讲解该文档。
>
> **首先，需要遵循以下几个原则（非常重要）：**
>
> 1. 标识符字符串尽量使用合法的英文单词（少数特殊情况可以用拼音）
> 2. 标识符字符串尽量只使用英文字母和阿拉伯数字。
> 3. **不要**使用“$”美元符号，其在命名中有特殊含义，建议程序员不要主动使用它。
> 4. **尽量不要**使用“_”下划线，其在命名中也有特殊含义，除开特殊场景不要使用它。
> 5. "$"或者“_”即便出现，也严禁作为开头结尾！



> 不同结构的标识符,遵循的驼峰命名规范是不同的,具体来说是:
>
> 1.**类名**,应该**大驼峰**
>
> 2.**方法名**,变量名,应该**小驼峰**
>
> 3.**包名**,应该全部使用**小写字母**,不要出现大写,包名的名词不要使用复数形式,一律用**单数**(不要加s)
>
> 在公司当中,包名,往往都会以反转公司域名开头
>
> 比如: com.baidu.xxx  com.cskaoyan.xxx



### 变量的使用

---

#### 变量

> **变量初始化**
>
> **![image-20230227091009727](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230227091009727.png)**
>
> 注释：
>
> ![image-20230227091529751](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230227091529751.png)



#####关于Java中获取数据类型📕

> 参考：[(87条消息) Java中获取数据的类型_Dream_飞翔的博客-CSDN博客](https://blog.csdn.net/qq_48455576/article/details/119818558)
>
> 不同于python，Java中没有相应的内置函数来返回数据的类型，只能自己定义方法来获取数据的类型
>
> ```java
> public class GetType {	
> 	public static String getType(Object obj) {
> 		/**
> 		 *  1. 通过反射获取传来参数的JavaClass对象
> 		 *  2. 获取到JavaClass对象的类型名称
> 		 *  3. 将参数的类型名称返回
> 		 */
> 		return obj.getClass().getTypeName();
> 	}
> }
> ```
>
> 方法：
>
> * .getclass():
>
>   
>
> * .getTyperName():



##### 变量使用的细节问题

String类

> String类是JDK源码中提供的一个固有类，也是源码中最常被使用的类型，是最常见的Java引用数据类型。
>
> 关于String类的详细内容，我们留到后续再去讲解。这里，我们仅简单了解一下String类。
>
> String的意思是字符串，所以在Java当中，String类型是用来表示字符串的。**Java代码中，所有用双引号直接引起来的内容，都是String类的一个实例，比如"hello world!"。**
>
> 一个String类型局部变量的声明、初始化语法是下面形式：
>
> 1
>
> ```
> String str = "hello world!";
> ```
>
> 当然，你直接使用输出语句在控制台输出字符串，也是使用了Java的String类。
>
> 除此之外，在当前这个阶段，还希望大家能够了解的一个知识点是：如何判断两个String字符串变量的**内容一致**呢？
>
> 比如给你两个字符串变量：
>
> 代码块 13. 两个字符串变量
>
> 1
>
> ```
> String s1 = "hello";
> ```
>
> 2
>
> ```
> String s2 = "hello";
> ```
>
> 
>
> s1和s2的内容是一致的，如何判断呢？这里，我直接给出具体做法，大家可以记忆一下，这些内容在后续再详细学习：
>
> 1
>
> ```
> s1.equals(s2);
> ```
>
> 以上结构，用于判断两个字符串变量s1和s2的内容是否一致。它会返回一个布尔类型值，如果一致返回true，否则返回false。
>
> 当然，对于s1和s2，它们equals比较的结果是：
>
> > true

> 切记：
>
> **比较两个字符串的内容是否一致，不能使用“==”号！**
>
> 而是使用equals方法！





---



###常量的使用

在Java中，利用关键字final指示常量。

分为：

> 字面值常量：
>
> - 整型常量：
>
>   Java 的整型常量值主要有如下 3 种形式。
>
>   - 十进制数形式：如 54、-67、0，这种**默认类型是int**
>   - 八进制数形式：Java 中的八进制常数的表示**以 0 开头**，如 0125 表示十进制数 85，-013 表示十进制数 -11。
>   - 十六进制数形式：Java 中的十六进制常数的表示以 0x 或 0X 开头，如 0x100 表示十进制数 256，-0x16 表示十进制数 -22。
>
>   整型（int）常量默认在内存中占 32 位，是具有整数类型的值，当运算过程中所需值超过 32 位长度时，可以把它表示为长整型（long）数值。长整型类型则要在数字后面加 L 或 1， 如 697L，表示一个长整型数，它在内存中占 64 位。
>
> ```java
> // 在代码中直接写一个整数,不用任何特殊格式,它就是一个十进制的整数
>         int a = 10;
>         // a = 100;
> 
>         // 如果想要表示二进制数,这个数要以0b开头
>         int a2 = 0b10;
>         System.out.println(a2);
> 
>         // 如果想要表示八进制,这个数用0开头
>         // Octal integer '01'
>         int a3 = 0100;
>         System.out.println(a3);
> 
>         // 如果想要表示十六进制,这个数用0X开头
>         int a4 = 0x123;
>         System.out.println(a4);
> 
>         String str = null;
>         //int a5 = null;
> ```
>
> 
>
> 
>
> - 字符串常量：
>
>   Java 的字符型常量值是用单引号引起来的一个字符，如 'e'、E'。需要注意的是，Java 字符串常量值中的单引号和双引号不可混用。双引号用来表示字符串，像 "11"、"d" 等都是表示单个字符的字符串。
>
>   除了以上所述形式的字符常量值之外，Java 还允许使用一种特殊形式的字符常量值来表示一些难以用一般字符表示的字符，这种特殊形式的字符是以开头的字符序列，称为转义字符。
>
> 
>
> - 布尔常量：
>
> ​		只有两个值：true和false
>
> 
>
> - 空常量：
>
> ​		空常量是引用数据类型独有的一种取值，只有null一个。（后面会讲，这里先记一下）
>
> ​		**基本数据类型不能用空常量赋值.**
>
> ​		报错信息：Incompatible types. Found: 'null', required: 'int'

> **自定义常量**：
>
> 
>
> ##### 解释字面量、常量和变量之间的区别
>
> 字面量是指由字母，数字等构成的[字符串](https://so.csdn.net/so/search?q=字符串&spm=1001.2101.3001.7020)或者数值，它只能作为右值出现，所谓右值是指等号右边的值，如：int a=123这里的a为左值，123为右值。
>
> 常量和变量都属于变量，只不过常量是赋过值后不能再改变的变量，而普通的变量可以再进行赋值操作。
>
> 在Java中通俗的说：int i = 1;把整数1赋值给int型变量i，整数1就是[Java](http://lib.csdn.net/base/javase)字面量，
> 同样，String s = "abc";中的abc也是字面量。
>
> 
>
> ##### 关于默认值的知识点
>
> 1.
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129193304773.png" alt="image-20230129193304773" style="zoom:67%;" />
>
> Q：用字面常量去给long型变量赋值时，明明没有超出long的范围，为什么报错？
>
> A：因为字面常量默认是int类型，而这么多个8已经超出int的类型了，如何解决？
>
> ​	  通过在整数字面量后面加L来声明
>
> 2.再如：
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230129222804932.png" alt="image-20230129222804932" style="zoom:67%;" />
>
> 原因如上，默认类型是double
>
> 通过后面加F解决

#### 常量使用的细节问题

> Java当中的整数字面值常量，默认当作int处理。
> * 假如你想使用字面值整数定义一个**long**类型变量，那么该字面值常量的后面应该加上一个"L"区分（禁止使用小写"l"）。
> * Java当中的小数字面值常量，默认当作double处理。假如你想使用字面值小数定义一个float类型变量，那么该字面值常量的后面应该加上一个"F"或"f"区分。

---



### 基本数据类型的数据类型转换

---

#### 自动类型转换

自动类型转换,自动指的是"编译器自动完成这个类型转换",这一次转换不需要程序员做任何额外操作就可以直接完成.

#### 强制类型转换

强制类型转换,这时编译器不会自动完成这个类型转换,而是需要程序员写额外的代码(强转的语法)来完成这个类型转换.

强转的语法: 强转后的数据类型 变量名 = (强转后的数据类型)被强转的变量/常量;

> ```java
> package com.cskaoyan.javase.basic._3variable.detail;
> 
> /**
>  * 基本数据类型的类型转换
>  * Java中变量的数据类型由某一种转换为另一种，我们将这个过程叫做数据类型转换。
>  * 数据类型有固定的语法条件,不是随便转换的
>  *
>  * 数据类型的转换又可以分为两类：
>  *      1.自动类型转换,自动指的是"编译器自动完成这个类型转换",这一次转换不需要程序员做任何额外操作就可以直接完成.
>  *
>  *      2.强制类型转换,这时编译器不会自动完成这个类型转换,而是需要程序员写额外的代码(强转的语法)来完成这个类型转换.
>  *      强转的语法:
>  *      强转后的数据类型 变量名 = (强转后的数据类型)被强转的变量/常量;
>  *
>  * 基本数据类型能够完成类型转换的前提:
>  * 只能发生在数值类型之间,也就是说boolean不参与基本数据类型的类型转换
>  *
>  * 基本数据类型的自动类型转换
>  *      条件: 取值范围小的数据类型 --> 取值范围大的数据类型
>  *      注意事项:
>  *      基本数据类型的自动类型转换自动完成,自动发生,那么它有没有什么风险呢?
>  *      大取值范围数据类型装小取值范围数据类型的变量,是可以装的下的,风险是比较小的,所以可以自动完成
>  *      但风险小,不意味着没有风险
>  *      这个风险主要来源于浮点数,因为浮点数有有效数字的限制,会出现精度丢失的情况
>  *
>  * 基本数据类型的强制类型转换
>  *      条件: 取值范围大的数据类型 --> 取值范围小的数据类型
>  *      大到小是有很大概率出现数据溢出(装不下)的,这时导致数据失真(数据和之前完全不同的,这就和精度不同了)
>  *      所以基本数据类型的强制类型转换是有很大风险的,既然有风险,编译器说,我不做,你自己做,风险由程序员承担
>  *      所以强转必须程序员手动写特定语法完成,编译器不会自动完成
>  *
>  *      注意:
>  *      强转是存在风险的,不要随便做强转
>  *      在开发中,强转大多数用于小数取整
>  *
>  * 引申(扩展):
>  * Java的引用数据类型也同样具备类型转换的能力,同样分为两大类:
>  *      1.引用数据类型的自动类型转换,编译器自动完成,不需要写额外代码
>  *      2.引用数据类型的强制类型转换,需要写额外代码完成
>  * 注:
>  *      引用数据类型的类型转换非常常用,这是后面学习的重点.
>  *
>  * @since 10:00
>  * @author wuguidong@cskaoyan.onaliyun.com
>  */
> public class Demo4 {
>     public static void main(String[] args) {
>         // int --> long 自动类型转换
>         long a = 100;
> 
>         // long --> float 自动类型转换
>         float b = a;
> 
>         // float --> double 自动类型转换
>         double c = b;
> 
>         int num = 123456789;
>         // 自动类型转换丢失了精度
>         float num2 = num;
>         System.out.println(num2);
> 
>         double num3 = num;
>         System.out.println(num3);
> 
>         // double --> float 大到小是强转,必须程序员手动完成
>         /*
>             开发中写强转的快捷方式:
>                 1.在要强转数据后面加".cast"回车
>                 2.alt + 回车 报错的地方
>          */
>         float d = ((float) 0.1);
>         float d2 = (float) 0.2;
> 
>         System.out.println(((int) 10.1));
>     }
> }
> 
> ```
>
> 开发中写强转的快捷方式:
>                 1.在要强转数据后面加".cast"回车
>                 2.alt + 回车 报错的地方

---



#### 表达式类型提升

1.如果表达式中仅存在**byte,short,char**变量参与运算,表达式结果直接提升到**int**,而不是最大的数据类型

​	因为byte、char、short都太小，byte+byte也很容易超出范围

🔺特别提醒,注意事项:

**表达式的类型提升仅在表达式中存在任意变量(或者小数常量)参与运算时才生效**

**如果表达式中全部都是整型常量,则不符合这个规则**

```java
package com.cskaoyan.javase.basic._3variable.detail;

/**
 * 表达式的类型提升
 * 给出一个表达式,表达式中存在(多个)变量参与运算,这些变量的数据类型可以不同,那么结果的数据类型是什么呢?
 * 这里就遵循表达式的类型提升语法
 *
 * 当表达式中存在多个变量参与运算时,表达式的结果数据类型是取值范围最大的那个数据类型
 * 两个特殊的规则:
 *      1.如果表达式中仅存在byte,short,char变量参与运算,表达式结果直接提升到int,而不是最大的数据类型
 *      2.String可以用"+"表示字符串拼接运算,如果表达式中存在任意String参与拼接运算,那么结果一定是String
 *
 * 特别提醒,注意事项:
 *      表达式的类型提升仅在表达式中存在任意变量(或者小数常量)参与运算时才生效
 *      如果表达式中全部都是整型常量,则不符合这个规则
 *
 * @since 10:41
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo5 {
    public static void main(String[] args) {
        int a = 10;
        byte b = 10;
        /*
            对于表达式的处理,可以考虑接收,也可以考虑直接输出
            都可以使用相应的快捷键
            如果想要直接输出,可以用".sout"/".soutv"回车
            如果想要用变量接收,可以用两种方式:
                1.".var"回车
                2.快捷键ctrl+alt+V
            注意事项:
            为了写代码更有效率,并且写出更安全的代码
            推荐在写有"="的等式,赋值语句时,从右往左写
            右边写完,自动生成左边,不要手写从左往右
         */
        System.out.println("a + b = " + a + b);
        int num = a + b;
        int num2 = a + b;

        float c = 0.1f;
        float v = a + b + c;

        double d = 0.1;
        double v1 = a + b + c + d;


        char var1 = 'a';
        byte var2 = 10;
        int i = var1 + var2;


        String s = a + b + c + d + "abc";
    }
}

```

```java
package com.cskaoyan.javase.basic._3variable.detail;

/**
 * 当表达式中全部都是整型常量时,它的运算不遵循表达式提升
 * 这是整型常量的特殊性
 * 编译器是很"聪明"的：
 *      1.对于整数字面值常量（包括常量的运算）而言，因为它的值一定不会发生变化，而且整型数据值的位数十分容易判断，所以编译器能够自动判断整型常量是否在接收数据类型的范围内。
 *      2.体现在语法上就是：将一个整型字面值（包括常量的运算）赋值给整型时，如果该常量在整型数据类型的取值范围内，是可以赋值成功的。
 *
 *
 *
 * @since 10:52
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo6 {
    public static void main(String[] args) {
        // int --> byte 大到小按理说是强转,但实际上这里自动完成
        byte a = 10;

        char b = 65535;
        // char c = 65536;

        // byte c = 100 + 100;
        byte c = 20;
        byte d = 10 + 20;
        // byte + byte = int
        byte e = (byte) (a + c);
    }
}

```



---



# 控制流程

---

## 控制流程结构

---

###块作用域

![image-20230214232009374](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230214232009374.png)



##选择结构

---

### 条件语句

即if语句



## 循环结构

---



### 循环

即while语句

注意：while循环语句是在最开始检测循环条件，所以有可能一次都不执行，如果要至少执行一次，使用do/while语句，如：

![image-20230214233432325](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230214233432325.png)

### 确定循环(for循环)

即for循环

![image-20230214233722223](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230214233722223.png)

### 多重选择：switch循环

![image-20230214233939816](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230214233939816.png)



### 中断控制流程的语句

---

#### break

> **概述：**
>
> break意为"打断，中断"，是常用的循环控制关键字。
>
> **使用场景：**
>
> break并不仅仅能用在循环中，它在switch中也可以使用，break就有了两个使用场景：
>
> 1. switch语句中某个case分支，用于结束整个switch。
> 2. 循环语句中。
>
> 注意：除开上面两种语境不能使用break，编译不通过
>
> **语义/作用：**
>
> 针对break的使用场景不同，作用也是不同的：
>
> 1. 在switch中使用，表示结束当前switch语句。
> 2. 在循环中使用，表示结束当前循环。
>
>  **注意：若有嵌套循环，表示结束当前层次的循环，和外层没有关系。**
>
> 

> 那么如果我就有多层嵌套循环，需要结束外层循环呢？
>
> 这时就需要使用标签（label）了，语法如下：
>
>  ```java
>  label:for(){
>   label2:for(){
>       label3:for(){
>           //break label
>       }
>   }
>  }
>  ```
>
> 使用注意事项：
>
> 1. 标签是用来标注某个层次的循环的，所以它应该加在for或者while关键字的头上。
> 2. 标签名可以看成是一个变量名，建议小驼峰式书写。
> 3. 使用标签标注循环层次时，不要忘记**" : "** 
> 4. 当break后面跟标签表示结束标签层次循环时，无需加" : "冒号。



![image-20230215001232244](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230215001232244.png)

![image-20230215001242709](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230215001242709.png)



#### continue

> **continue不同于break，它只能在循环中使用，无法在循环外使用，如果使用，会编译报错。**
>
> **continue在循环表示结束当前次的循环，转而继续执行后面的循环。**注意它不是结束整个循环，而是跳出当前层的当前次循环，进行当前层的下一次循环。如果有嵌套循环，同样可以使用标签，用法和break一致，不再赘述。

---



# 方法



## 方法的基本使用

> ### 语法
>
> ```java
> [修饰符列表] 返回值类型 方法名 (形式参数列表){
>   // 方法体
> }
> ```
>
> 在具体了解每个部分的语义之前，我们需要了解 **两个非常重要的概念：** 
>
> 1. **[修饰符列表] 返回值类型 方法名 (形式参数列表)** 合起来称之 **方法的声明**（也叫**方法头**）
> 2. **方法名 (形式参数列表)** 合起来称之为 **方法的签名**

> 1. **修饰符列表**：修饰符列表不是必须的，可以为空不写，现在默认为**public static**（具体含义面向对象讲）
> 2. **返回值类型**：方法可能会有结果，这个结果就是返回值，返回值的数据类型称之为**返回值类型**
>    1. 返回值类型可以是基本数据类型，也可以是引用数据类型（例如String）
>       - 此时表示方法拥有返回值，必须显式的指出该返回值，否则编译报错
>       - 在方法体中用`return`关键字指示返回值，格式为`return + 返回值`
>       - return后的返回值的数据类型，要和方法声明中的返回值类型保持一致**（或者兼容）**
>       - 方法执行到return语句时，表示方法执行完毕。
>    2. 方法完全可以没有结果，也就是没有返回值，但是方法必须要有返回值类型，用关键字**void**标记。
>       - 使用void标记的方法，没有返回值，自然也无需指出返回值
>       - ❗**void方法没有返回值，但它有返回值类型，void本身就是一种返回值类型。**
> 3. **方法名**：给方法起个名字，调用方法时用的，方法名的命名需要遵守规范
>    1. 必须是合法的标识符
>    2. **方法名最好`见名知意`**
>    3. 方法名最好是动词
>    4. **方法名遵循首字母小写，其他单词的首字母大写的`小驼峰命名法`**



## 方法的重载

> ```java
> 
> package com.cskaoyan.javase.overload._0introduction;
> 
> /**
>  * 方法重载的定义:
>  * 方法重载允许一个类中，多个方法拥有相同的名字。
>  * 方法重载是有限制条件的,方法名既然相同了,调用方法时如何区分方法呢?
>  *
>  * 方法的定义语法:
>  * [修饰符列表] 返回值类型 方法名(形参列表){
>  *     // 方法体
>  * }
>  * 方法的签名: 方法名(形参列表)
>  * 作用是: 在同一类当中,方法的签名可以唯一的确定一个方法
>  *
>  * 方法的重载要求方法名相同,这时还要保证方法不同,那么形参列表形参列表就必须不同
>  *
>  * 什么叫做形参列表不同呢?
>  *      1.形参的个数不同
>  *      2.在形参个数相同的情况下,形参的数据类型不同
>  *      3.在形参个数相同,数据类型也相同的情况下,形参的顺序不同
>  * 以上三点,满足其一或者满足多条都可以构成方法的重载!
>  *
>  * 注意:
>  * 方法的重载有且仅有上述三种情况构成,其余情况一律不构成方法的重载!
>  * 比如:
>  *      1.[修饰符列表] 返回值类型 都不影响方法重载
>  *      2.形参名不同不能构成方法的重载
>  *
>  * @since 09:51
>  * @author wuguidong@cskaoyan.onaliyun.com
>  */
> public class NewDemo {
> 
>     // 无参方法
>     public static void test() {
>     }
>     // public static int test(){
>     //     return 1;
>     // }
>     // void test(){}
>     // 方法的重复
>     // public static void test(){}
> 
>     public static void test(int a) {
>     }
>     // public static void test(int b) {
>     // }
> 
>     public static void test(double a) {
>     }
> 
>     public static void test(int a, double b) {
>     }
> 
>     public static void test(double a, int b) {
>     }
> 
> }
> 
> ```

> **关于就近原则**
>
> ```java
> package com.cskaoyan.javase.overload._1detail;
> 
> /**
>  * 在同一个类中,在很多方法中，唯一地找到一个方法，需要明确什么？
>  * 要想唯一确定一个方法，必须明确方法的名字和形参列表
>  * 而这俩合起来就称之为"方法的签名"，这就是方法签名唯一确定方法的由来。
>  * 方法重载导致方法名是一样的,所以这时只需要区分不同的形参列表就足够确定方法了
>  *
>  * 由于方法在调用时,实参数据类型自动类型转换到形参,该实参就允许传入方法
>  * 所以在方法重载时,就有可能出现一次方法调用,多个方法匹配的情况
>  *
>  * 这时就要遵循Java设计原则的"就近原则"(重要)
>  * 就近原则: 当代码中出现多个可以匹配的场景时,那么只要找到一条原则/逻辑,判断出谁更近,那么就匹配它
>  * 所以就近原则最重要的就是要搞清楚，究竟什么是“最近的”！ 找出这样的一条判断原则,判断最近.
>  *
>  * 注意事项:
>  * 就近原则也不是万能的,当就近原则失效时,多个场景都能匹配就无法确定匹配谁了,这时就会编译报错
>  *
>  * @since 09:59
>  * @author wuguidong@cskaoyan.onaliyun.com
>  */
> public class Demo {
>     public static void main(String[] args) {
>         // test(10);
>         // test(10L);
>         // test(10F);
>         // test(0.1);
> 
>         // Ambiguous method call: both 'Demo.method(int, double)' and 'Demo.method(double, int)' match
>         // method(1, 1);
>     }
> 
>     public static void method(int a, double b) {
>     }
> 
>     public static void method(double a, int b) {
>     }
> 
>     public static void test(int a) {
>     }
> 
>     public static void test(double a) {
>     }
> 
>     public static void test(float a) {
>     }
> }
> 
> ```
>
> 方法的重载使用场景:
>
> 1.写工具类,有一系列相似功能的方法,区别在于需要参数的数据类型不同时
>
> 使用方法重载
>
> 2.JDK源码中存在大量方法重载
>
> 3.(最常见)面向对象语法中的构造器



## **Junit单元测试**

什么是Junit单元测试？

简单来说，**Junit可以在同一个类中实现多个main方法的效果，它是非常好的测试工具。**在JavaSE阶段可以用来测试各种demo或者idea。

> 如何使用
>
> Junit如何使用?
>
> 1. 直接在要测试的方法上方，写注解(annotation) `@Test`
>
> 2. 直接写注解肯定会报错，这是因为没有导包，但是`@Test`注解的导包比较特殊。需要直接 Alt + 回车 依照下图完成依赖导入并导包。
>
>    
>
>    图 1. 导入依赖图
>
>    ![导入依赖图](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202112290204711.png?align=center)
>
>    
>
> 3. 导入依赖后，在注解`@Test`下方直接写代码：
>
> ```java
> public void 方法名(){
>     //方法体
> }
> ```
>
> 1. 注解。注解（annotation）是和class同等级别的数据类型，同样是引用数据类型（你完全可以把注解看成一个类）
> 2. 我们在给Scanner导包时，直接快捷键`Alt + 回车`完成，并不需要像导入`@Test`这么麻烦。这是因为Scanner是JDK中原有的类，可以直接导包使用。而**Test注解并不是JDK中原本自带的注解，是第三方开发出来的工具包中的注解**。 所以在导包之前还需要**导入依赖**。
> 3. **导入依赖：是指将非JDK当中的，第三方工具包中的内容，导入当前Project的过程。导入依赖后，在当前Project下就可以使用该依赖中的类和方法等完成开发。**
> 4. `Junit`这个第三方工具包比较特殊，它是IDEA开发工具下会自带的工具包，只需要使用`Alt + 回车`就能自动完成**依赖导入**。（正常情况下，普通三方工具包就需要手动添加了，当然后面我们还会自动管理和添加依赖的方式。）
> 5. **导入依赖后，只是能够使用工具包，还需要使用导包语句完成导包，这样才可以使用该注解。**

> 注意事项：
>
> 1. Junit单元测试的格式上：
>    1. **public void 是固定格式**，不可修改，修改会报错。
>    2. 并且测试方法正常情况下，不能添加形参，必须是空参方法。（因为没人调用啊）
> 2. 做单元测试的类中，不要写main方法，没有太大意义。

> ```java
> package javase.day03;
> 
> import org.junit.Test;
> 
> public class JunitTest {
>     public static void main(String[] args) {
> 
>     }
> 
>     //使用junit测试
>     @Test
>     public void test()
>     {
>         System.out.print("hello world！");
>     }
> }
> 
> ```
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230301173028566.png" alt="image-20230301173028566" style="zoom:33%;" />

### 关于全限定类名

> 不要在一个叫做Test类中使用`@Test`注解。如果你非要使用，也不是不行，只是需要使用**"全限定类名"**。
>
> ------
>
> 在Test类中，使用注解`@Test`时，会默认将类Test当成注解使用，这是一种就近原则。但实际上，Junit单元测试中的注解Test是属于包`org.junit.Test`下的，由于就近原则就会报错。那么怎么办呢？
>
> 正常情况下，我们使用类/注解时，无需指出包名，但现在已经不正常了，就需要明确包了。我们把`包名 + 类名`这种可以唯一确定一个类的类名书写形式，称之为 **全限定类名**。它的作用就是唯一的、准确的定位一个类。
>
> 如：
>
> ```java
> package com.cskaoyan.javase.junit._1basic;
> 
> /**
>  * 在Test类之下使用Junit单元测试
>  * 注解是和class同等级别的数据类型,它等价于class
>  * 所以注解Test和类Test是重复的,有冲突的
>  * 当在一个Test class下面使用注解Test时,由于就近原则,会直接把类Test当成注解Test使用,这显然是不可能的
>  * 也就是说我们实际需要的是org.junit包下的注解Test
>  * 但实际上得到的是类class Test
>  *
>  * 知道原因后,如何解决这个问题呢?(我就想要在Test类中使用Junit)
>  * 简单类名: 单单写出一个类的名字,不添加任何其它信息,比如Demo,Student...
>  *      简单类名不可以唯一确定类
>  * 全限定类名(全类名): 包名 + 简单类名,比如com.cskaoyan.Demo类
>  *      由于同包下绝不可能出现同名类,所以全限定类名可以唯一的确定一个类
>  *
>  * 用全限定类名去使用注解Test,而不是简单类名
>  * 使用以下结构:
>  * \@org.junit.Test
>  *
>  * 全限定类名在绝大多数情况下都是比较长的,所以尽量不要用全限定类名,除非迫不得已
>  *
>  * @since 10:48
>  * @author wuguidong@cskaoyan.onaliyun.com
>  */
> public class Test {
>     @org.junit.Test
>     public void test() {
>         System.out.println("hello wrold!");
>     }
> }
> 
> ```



### 关于在Junit中使用键盘录入

一般情况下，Junit下是不能使用Scanner的

解决办法：[Java JUnit测试实现控制台输入的正确姿势 - 腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1870330)

---



# 数组

---

## 数组的基本概念

**数组是一种在内存中需要一片连续空间，连续存储数据的数据结构。**



### 数组的数据结构及优缺点

优点：随机访问

> 思考一个问题：数组是有下标的，那这个下标有什么作用呢？数组作为一种典型的数据结构，它的优点是什么呢？
>
> 答：数组的下标可以允许数组在访问元素时，直接通过下标访问对应元素，这就是数组的**随机访问**。

> **随机访问**：指的是在访问第n个元素时，无需经过其它元素，直接可以定位访问它。
>
> **非随机访问**：指的是访向第n个元素时，需要先访问前（n-1）个元素，然后才能访问第n个元素。

> 很明显，随机访问的效率要比非随机访问高很多，从时间复杂度（**时间复杂度是指执行算法所需要的计算工作量**）上来说：
>
> 1. 随机访问是常数级别的访问效率，即O(1)
> 2. 非随机访问的访问效率是O(n)
>
> 随机访问（也叫随机存取）是数组的最主要、最显著的特点，也是它最重要的优点，**使用数组大多都是图它快**。

<blockquote class="v-q green em"><p d-id="vk-pg-49" d-pg-idx="49"></p><p d-id="vk-pg-50" d-pg-idx="50"><span>任何事物都不可能只有优点和好处，没有缺点。那么数组有什么缺点呢？</span><span style="color:red;background:yellow"><strong><span>换句话说，数组为了实现随机访问这样的一个优点，数组付出了什么代价呢？</span></strong></span></p><p d-id="vk-pg-51" d-pg-idx="51"><strong><span>数组的随机访问实现方式是：根据数组的首地址和下标，通过寻址公式直接计算出对应的内存地址，最终找出数据。</span></strong><span>要想使用这种方式实现随机访问，显然数组对数据结构和数组中的元素都是有要求的：</span></p><ol start=""><li d-id="vk-pg-52" d-pg-idx="52"><font color="red"><strong><span>存储结构必须是连续的（有序），这样才能连续计算。</span></strong></font></li><li d-id="vk-pg-53" d-pg-idx="53"><font color="red"><strong><span>存储的元素必须数据类型相同，这样每个存储单元的地址偏移量都是相同的。</span></strong></font></li></ol><p d-id="vk-pg-54" d-pg-idx="54"><span>进一步推导可以得出：</span></p><ol start=""><li d-id="vk-pg-55" d-pg-idx="55"><span>数组对内存空间的要求很高，必须划分出一片</span><strong><span>独立的、连续的</span></strong><span>内存空间给一个数组用以存储元素。</span></li><li d-id="vk-pg-56" d-pg-idx="56"><span>一个数组的内存空间是固定的，一旦创建某个数组，除非销毁它，否则它的存储空间不能改变，</span><span style="color:red;background:yellow"><strong><span>即数组创建后就长度不可变，这是数组最显著的一个缺点。</span></strong></span></li><li d-id="vk-pg-57" d-pg-idx="57"><span>同一个数组中必须存储相同数据类型的元素，这也是数组的一个限制。</span></li></ol></blockquote>

> 这里做一个总结：
>
> 首先数组是用一段连续的内存空间，来存储一组具有相同类型的数据的结构。
>
> 它的优点是：随机访问（存取），访问n位置的元素，无需经过前面(n-1)个元素，访问效率非常高。时间复杂度是常数级别 O(1)
>
> 它的缺点主要是：**数组一旦创建其长度就固定了，就绝不可能更改了。**这是数组最大的缺点！除此之外，数组还会限制存储其中元素的数据类型，这也是一个不小的限制。

> 数组固然效率高优点很突出，但它的缺点同样非常明显，同样非常突出。这导致在实际开发中，我们**几乎不可能直接使用数组，这是因为数组的长度实在是难以确定：**
>
> 1. 如果给出的长度过长，会导致空间浪费。
> 2. 如果给出的长度过短，那数组根本不可用。
>
> 如何解决上面的困境呢？
>
> 假设这样一个场景：教室可以容纳100名学生，此时教室有80人可以坐得下，但很快又要再来30名学生，教室肯定坐不下了，怎么办呢？
>
> 难道把教室的墙拆掉扩建？显然不可能也不需要。此时，**只需要找一个更大的教室然后让原先的学生以及新同学都去新教室就可以了。**
>
> 这其实就对应着**“数组扩容”**的思想来解决数组长度不可变的缺点：
>
> 数组不可能真的在原本基础上增长长度，那就新建一个更长的数组，然后将原数组的元素拷贝到新数组当中。
>
> **这种通过“数组元素拷贝”方式实现的“数组扩容”，使得“新容器”能够使用下标访问效率高，且一定程度上规避了数组长度不可变的缺点。这种设计就是Java集合容器当中的——ArrayList，在实际开发中，大多数需要使用数组容器的场景都会使用它。**



## 数组的基本使用



#### 声明

格式：`数据类型[] 数组名;`



#### 初始化

声明完成一个数组后，该数组仍然不能使用，还缺少一个初始化（initialization）的过程，类似变量初始化（赋值）

对于变量而言，初始化是在内存中开辟空间并赋值的过程，对于数组而言，也是类似的过程。

数组要开辟一片连续的空间用来存放数据，然后进行元素赋值，即：

1. 我们要告诉需要开辟多少内存空间**（数组有多长）**
2. 数组中的元素要明确它的值**（没有值，数组的存储单元也没有意义）**

为了完成上述两个要求，数组的初始化就有了以下两种方式。

##### 静态初始化

> 静态初始化指的是：
>
> > 由程序员显式的，指定数组中每个元素的初始值，数组的长度由系统决定（实际上也是由程序员给出的）
>
> 和数组的声明写在一起，语法格式就是：
>
> ```java
> 数据类型[] 数组名 = new 数据类型[]{元素1,元素2,元素3...};
> ```
>
> 静态初始化有简写的形式，可以省略new关键字，如下：
>
> ```java
> 数据类型[] 数组名 = {元素1,元素2,元素3...};
> ```
>
>  **注：简化的形式必须跟在声明之后，不能单独使用！** 下列写法就是错误的：
>
> ```java
> 数组名 = {元素1,元素2,元素3...};
> ```
>
> 



##### 动态初始化



## **JVM内存模型**

---



### JVM运行时数据区域

程序在运行期间，需要处理很多数据，JVM中有专门的区域来存放这些数据，这片区域称之为**JVM的运行时数据区域**。

在这片区域中，变量显然不可能是杂乱无章的随意存放的， **而是被JVM分区管理的：** 这些区域各有各的用途，创建时间，销毁时间等特点皆有不同，与之相对应的，不同区域中存放的变量的生命周期、特点和使用方式也会随之产生差异。

**理解JVM运行时内存是学习Java的基本，这个东西并不底层，需要每位同学都掌握。**

**理解JVM运行时内存，能够加深我们对Java中的很多现象的理解。**



### JVM运行时内存模型图

> 为了描述JVM运行时内存空间，Java的开发者在《Java虚拟机规范》中指出：JVM （运行时数据区）内存共分为：
>
> 1. JVM栈
> 2. 堆
> 3. 方法区
> 4. 程序计数器
> 5. 本地方法栈
>
> 这五大区域，示意图如下：
>
> 
>
> 图 1. JVM运行时内存模型
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230301192727445.png" alt="image-20230301192727445" style="zoom:50%;" />
>
> 
>
> **为了方便简化交流，以后我们统一称呼JVM运行时内存模型为JVM内存模型。** 下面详细解释一下各个区域的用途.



#### JVM栈（栈）

<blockquote class="v-q green em"><p d-id="vk-pg-19" d-pg-idx="19"></p><p d-id="vk-pg-20" d-pg-idx="20"><span>我们要明确的是，Java程序当中的方法调用是需要耗费资源的：</span></p><ol start=""><li d-id="vk-pg-21" d-pg-idx="21"><span>方法中的局部变量需要开辟空间存储。</span></li><li d-id="vk-pg-22" d-pg-idx="22"><span>方法执行过程中所产生的局部变量也需要空间存储。</span></li><li d-id="vk-pg-23" d-pg-idx="23"><span>方法执行完毕后返回值也需要存储。</span></li><li d-id="vk-pg-24" d-pg-idx="24"><span>...</span></li></ol><p d-id="vk-pg-25" d-pg-idx="25"><span>总之，Java方法的执行是需要在JVM内存当中进行的，是需要耗费资源的。笼统得说，</span><span style="color:red;background:yellow"><strong><span>JVM栈（以后简称栈，stack），描述的是Java的（普通）方法执行时的所占内存的内存模型。</span></strong></span></p><p d-id="vk-pg-26" d-pg-idx="26"><span>注：普通方法指的是由Java代码书写实现的方法。比如JDK源码中的方法，比如我们自己自定义的方法等。</span></p></blockquote>

> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230301193114901.png" alt="image-20230301193114901" style="zoom: 50%;" />
>
> 栈这种数据结构的最大特点是：**先进后出**
>
> 我们把**进栈、出栈的基础单元称之为“栈帧”（frame）**。如果是JVM栈，描述的是方法的执行过程，那么进出栈的基本单元就是“方法栈帧”。
>
> 了解JVM栈的相关概念后，Java（普通）方法的执行，在JVM内存中，就可以做以下描述：
>
> 1. 每当Java程序执行一个方法，都会在栈上分配一块只属于该方法的内存区域，称之为**方法的栈帧**。
> 2. 方法调用实际上是将该方法的栈帧压入栈中，这个过程称之为**方法进栈**。
> 3. 方法进栈的同时局部变量开辟内存空间存储值，局部变量生效。
> 4. 方法调用完毕后，方法的栈帧随之出栈销毁，称之为**方法出栈**。



#### 堆

> 堆（heap）：堆是JVM内存中最大的一片区域，因为所有代码中“new”出来的东西，都存储在堆上。
>
> 我们把这些“new”出来的东西，称之为**对象（Object）**或者**实例（Instance）**。
>
> **所以这里，解释一下new关键字的语义就是：new关键字表示在堆上开辟空间，创建一个新的、独立的对象。**



#### 方法区



#### 本地方法栈



#### 总结

> **很明显，在JVM内存模型中，相对比较重要的，和程序的执行联系更紧密的是：堆和JVM栈。**
>
> 堆内存用来存储对象，由于Java是面向对象语言，Java面向对象程序中将会有非常多的对象，所以：
>
> 1. **堆内存主要决定了Java程序的数据如何存储的问题。**
> 2. **JVM栈用来表示方法的执行流程，它决定了程序如何执行，或者说如何处理数据。**



### 引用数据类型

#### 堆和栈中内容的区别



![image-20230302151332640](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230302151332640.png)





## **数组操作中的异常**

### 概念

```java
package com.cskaoyan.java.array._3exception;

/**
 * 首先第一个问题，什么是异常？
 * 异常，指的是程序运行时出现的不正常的情况。
 *      程序必须正常启动后,才会产生异常
 *      程序未启动报错属于编译报错
 * 一旦程序出现异常，JVM会把这个异常信息封装成一个对象（也就是异常对象）
 * 然后在默认情况(不处理异常的情况)下JVM就会终止程序执行，并在控制台打印这个异常信息。
 *
 * 异常对象的主要作用是描述程序运行出现不正常情况时各种信息，主要包括：
 *      1.异常的名称，问题的描述
 *      2.产生问题的代码行数（位置）
 *
 * 最后，还需要注意的就是：
 * 由于Java代码最终是逐行解释执行的，所以产生异常之前的代码是可以正常执行的。在默认情况下，程序产生异常会导致程序在异常行终止执行，所以异常行之后的代码就不会执行了。
 *
 * 思考:
 * 在默认情况下,程序最多产生几个异常呢?
 * 很明显,最多只有一个异常产生
 *
 * @since 15:38
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    public static void main(String[] args) {
        System.out.println("6666666666666");
        // 代码一旦产生异常,从该行开始就终止程序执行(默认情况下,没有处理异常时)
        System.out.println(10 / 0);
        System.out.println("77777777777777");
        System.out.println(10 / 0);
        System.out.println(10 / 0);
    }
}

```



### 数组下标越界异常

```java
package com.cskaoyan.java.array._3exception;

/**
 * 数组下标越界异常（ArrayIndexOutOfBoundsException），用来描述访问了某个数组的一个不存在（不合法）的下标时的问题。
 *
 * 注意事项：
 * 这是一个单独针对数组操作的异常，从名字就能看出来。
 * 这个异常在数组操作中很常见，尤其是在循环当中，当你误判了循环的变量是非常容易下标越界的。
 *
 * @since 15:44
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo2 {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3};
        System.out.println(arr[0]);
        System.out.println(arr[1]);
        System.out.println(arr[2]);
        // Array index is out of bounds
        // System.out.println(arr[3]);

        for (int i = 0; i < 5; i++) {
            System.out.println(arr[i]);
        }
    }
}

```



### 空指针异常

```java
package com.cskaoyan.java.array._3exception;


/**
 * 空指针异常（NullPointerException）
 * 用来描述通过一个指向null的引用访问、操作对象时的问题。当引用数据类型的引用指向了null（空常量）时，表示引用是没有指向任何对象，这时如果还想通过引用操作堆上对象，就会产生空指针异常（因为没有任何对象可供操作）
 *
 * (重点)注意事项:
 *
 * 1.空指针异常针对所有引用数据类型，不仅仅是数组操作。
 *
 * 2.空指针异常（NullPointerException），简称NPE，是Java之中最负盛名的异常，没有之一。
 * 以后大家会天天和引用数据类型打交道，也会每天和空指针异常打交道。
 * 空指针异常在多数情况下是有害的，会导致程序意外终止，避免空指针异常是Java程序员的必修课之一。(Java8当中提供了新语法,让Java程序员优雅得避免空指针异常)
 *      常见的、最简单朴实的规避手段就是通过if进行判断，判断出引用不会指向null后再使用引用操作对象。
 *
 * 最后再提一点：
 * 我们在开发时，要明确知道程序中的引用哪里会指向null，哪里完全不会指向null，对于：
 *      1.那些逻辑上，可能会指向null的引用，要在使用前慎重判断。如果等于null，需要做出相应处理（反正不能访问对象），判断不为null之后才能使用该引用访问对象。
 *      更多情况下
 *      2.那些逻辑上，完全不可能等于null的引用，就不应该做判断了。一旦程序抛出空指针异常，要去排查为什么引用会等于null，然后修正程序以避免引用等于null。
 *
 *
 * @since 15:52
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo3 {
    public static void main(String[] args) {

        // System.out.println(arr.length);
        // String str = null;
        // if (str != null) {
        //     // 不等于null的引用再去操作对象
        //     System.out.println(str.length());
        // }
        int[] arr = null;
        // 这里产生一个空指针异常
        // System.out.println(arr[0]);
        int[] arr2 = new int[0];
        System.out.println(arr2[0]);
    }
}

```



### 数组长度为0和数组是null以及数组未初始化，有啥区别？

```java
package com.cskaoyan.java.array._3exception;

/**
 * 数组长度为0和数组是null以及数组未初始化，有啥区别？
 *
 * 数组未初始化： 这个数组完全是不可用的，没有初始化的数组毫无意义，一旦使用会编译报错。
 * 数组长度为0和数组为null都是可以使用的，可以认为是经过初始化的，但它们都不是正常数组：
 *
 * 长度为0的数组，只在内存中存在对象的结构但没有存储单元，不能存储任何数据。它的操作中：
 * 直接打印数组名可以获取数组对象的地址。
 * 不能访问任何数组下标，否则都会抛出数组下标越界异常。
 * 输出数组的长度为0
 * 数组为null，表示数组的引用指向了null，无法对数组对象执行任何操作。
 *
 * 直接打印数组名得到一个null字符串。（null是一个字面值常量，所以可以直接打印输出它，此时没有操作对象，不会产生空指针异常）
 * 不能访问任何数组下标，也不能打印数组长度，都会报空指针异常。
 *
 * @since 16:02
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Exercise {
    public static void main(String[] args) {
        // 局部变量数组未初始化时,完全不可用,不能执行任何操作
        int[] arr;

        // 数组长度为0以及数组为null都表示数组经过了初始化,都是可以用的
        int[] arr2 = new int[0];
        System.out.println(arr2.length);
        // 长度为0的数组不能访问任何元素,因为它没有
        // System.out.println(arr2[0]);
        // System.out.println(arr2);

        // 引用指向null,不能执行任何对对象的操作
        int[] arr3 = null;
        // 打印引用不算操作对象,是可行的
        System.out.println(arr3);
        // System.out.println(arr3.length);
        // System.out.println(arr3[0]);
    }
}

```



## 方法的传参问题（重要）

> 方法的传参问题(重要)
>
> 什么是方法的传参问题?
>
> 在调用方法时,有些时候需要向方法传递实参，实参传递给方法后,有可能在方法内部去修改它
>
> 那么在方法内部修改完传递进方法的实参后,会被原先的实参变量本身带来什么影响呢?
>
> 这就是方法的传参问题



 **先记住结论：java只有值传递，不存在引用传递**

> ```java
> /**
>  * 方法的传参问题(重要)
>  * 什么是方法的传参问题?
>  *      在调用方法时,有些时候需要向方法传递实参
>  *      实参传递给方法后,有可能在方法内部去修改它
>  *      那么在方法内部修改完传递进方法的实参后,会被原先的实参变量本身带来什么影响呢?
>  *      这就是方法的传参问题
>  *
>  * 在具体讲方法的传参问题之前,我们了解两种Java中可能的传参方式:
>  *      1.值传递,指的是方法得到的并不是实参变量本身,而是这个实参变量的拷贝
>  *          如果Java采取值传递,那么方法就不可以修改实参变量本身,因为方法内部修改的是实参变量的拷贝
>  *
>  *      2.引用传递,指的是方法就直接得到了实参变量本身(得到地址)
>  *          如果Java采取引用传递,那么方法就可以修改实参变量本身,因为方法就直接得到了实参变量本身.
>  *
>  * 我们可以写代码验证Java究竟是值传递还是引用传递:
>  *      1.我们通过一个将int数值变为原先2倍但没有生效的方法,可以得知,至少对于Java基本数据类型
>  *          Java是值传递的
>  *
>  *      2.我们通过一个将int数组元素变为原先2倍生效的方法,得出,Java对于引用数据类型
>  *          是引用传递的
>  *
>  * 实际上上述结论是完全错误的,Java只有值传递,Java没有任何引用传递.
>  *
>  * 为什么Java只有值传递呢?
>  * 因为任何时候Java的方法都只能得到实参变量的拷贝,而不可能得到实参变量本身
>  * 这其实是必然的,因为方法调用必然是在另一个方法中调用
>  * 传入方法的实参变量,都是局部变量
>  * 如果局部变量能够传递给另一个方法,那局部变量就不是局部变量了
>  * 所以一个方法在调用其它方法时,传递给其他方法的实参变量时,其它方法只能得到这个变量的拷贝
>  *
>  * 知道Java值传递后,对我们定义方法,调用方法有什么影响呢?
>  *      1.对于Java基本数据类型的实参变量,任何方法都不可能修改该实参变量本身的取值
>  *
>  *
>  *      2.对于Java引用数据类型实参变量传入的引用,引用也是一个局部变量,任何方法不可能修改实参变量这个引用本身
>  *
>  *      以上也就是说, 方法不可能修改其它方法内部的局部变量
>  *
>  *      3.(最重要的)
>  *      虽然Java值传递,导致方法仅得到实参变量的拷贝
>  *      但引用的拷贝和原先引用仍然指向同一个对象
>  *      在方法内部使用引用的拷贝,仍然可以修改对象中元素的取值
>  *      对象的状态: 对象中属性,元素的取值
>  *      我们把这个现象称之为"方法可以改变对象的状态"
>  *
> 
> ```
>
> 例一：
>
> ```java
> // 该方法将传入方法的实参数据变为了原先的2倍
>     public static void doubleIntValue(int num) {
>         // 传入的只是实参变量的拷贝
>         //所以实参变量本身并不会有什么变化！
>         num *= 2;
>         System.out.println("在方法内部num的取值:" + num);
>     }
> 
> ```
>
> 例二：
>
> ```java
> // 该方法将数组中的元素变为原先的2倍
>     public static void doubleEleIntArr(int[] arr) {
>         for (int i = 0; i < arr.length; i++) {
>             arr[i] *= 2;
>         }
>     }
> ```
>
> 调用这个方法会发现，传入方法的实参变量（数组）确实在方法调用完毕之后发生了变化，和例一不同，但这并不能说明java就是引用传递，事实上还是值传递，因为传入方法的实参变量事实上是一个引用，引用存储的是对象的地址，那么即便是拷贝，指向的地址仍旧没有变，相当于同一个对象同时拥有两个指向它的引用，其中一个是方法中的引用，通过这个引用对对象进行修改之后，即便这个拷贝的引用被销毁，对象也已经发生改变了。
>
> 例三：
>
> ```java
> public static void main(String[] args) {
>         int[] arr1 = {666, 666, 666};
>         int[] arr2 = {777, 777, 777};
>         System.out.println("交换之前arr1 = " + arr1);
>         System.out.println("交换之前arr2 = " + arr2);
>         /*
>             如果Java是值传递的,那么方法内部交换的就是引用的拷贝,而不是引用本身,于是交换失败
>             但如果Java是引用传递的,那么方法内部交换的就是引用本身,于是交换成功
>             实际上这个交换失败了,说明Java引用数据类型也属于值传递
>             Java没有任何引用传递,Java只有值传递
>          */
>         swapReference(arr1, arr2);
>         System.out.println("交换之后arr1 = " + arr1);
>         System.out.println("交换之后arr2 = " + arr2);
>     }
> 
>     
>     // 该方法的目的是交换两个引用
>     public static void swapReference(int[] arr1, int[] arr2) {
>         int[] temp = arr1;
>         arr1 = arr2;
>         arr2 = temp;
>         System.out.println("交换方法之中arr1 = " + arr1);
>         System.out.println("交换方法之中arr2 = " + arr2);
>     }
> ```
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230303140456162.png" alt="image-20230303140456162" style="zoom:67%;" />
>
> 这个例子再次证明Java是值传递而不是引用传递

<blockquote class="v-q green em"><p d-id="vk-pg-61" d-pg-idx="61"></p><blockquote><p d-id="vk-pg-62" d-pg-idx="62"><span>总结：Java方法对方法参数能做什么？</span></p></blockquote><ol start=""><li><p d-id="vk-pg-63" d-pg-idx="63"><span>任何Java方法，都不可能修改另外一个方法中的局部变量，包括:</span></p><ol start=""><li d-id="vk-pg-64" d-pg-idx="64"><span style="color:red;background:yellow"><strong><span>其它方法中的基本数据类型变量</span></strong></span></li><li d-id="vk-pg-65" d-pg-idx="65"><span style="color:red;background:yellow"><strong><span>其它方法中的引用数据类型的引用</span></strong></span></li></ol><p d-id="vk-pg-66" d-pg-idx="66"><span>可以想象，如果上述修改能够成立，就违背了局部变量的设计原则。</span></p></li><li d-id="vk-pg-67" d-pg-idx="67"><span style="color:red;background:yellow"><strong><span>（重点）Java方法可以修改对象的状态，因为方法得到的是引用的拷贝，拷贝引用仍然指向原先引用指向的对象。</span></strong></span></li></ol></blockquote>

长风说：

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230303140823287.png" alt="image-20230303140823287" style="zoom:67%;" />



---



# 面向对象基础



## 重新认识引用数据类型

> 我们第一次认识和了解**引用数据类型**是在数组这一章节，我们通过JVM内存模型图和数组的初始化过程，知道：
>
> 1. 一个引用数据类型变量，分为两个部分：
>    1. 在栈上创建引用，它是一个局部变量。
>    2. 在堆上开辟空间，创建对象。
> 2. **栈上的引用通过存储堆上对象的地址和对象产生联系。**
> 3. 对象是引用数据类型的实质，但**我们只能通过栈上引用间接访问堆上对象。**
>
> ------
>
> 现在，我们已经学习过**对象与类**的知识点了，是时候进一步或者换一个角度去了解引用数据类型了。

> 像数组那样理解引用数据类型，虽然看到了引用数据类型的实质，但也把基本数据类型和引用数据类型完全割裂了。
> 
> 这两种数据类型当然不可能是完全没有关系的了！
> 
> 所以，我们需要让它们重新产生联系起来！
>
> 先回顾一下，在Java基础语法部分，我们给出的数据类型的概念/定义：
> 
> 数据类型： **表示的是一组数据的集合，和基于该数据集合的一组合法操作。**
> 
> 这个定义套在基本数据类型上，实在再合适不过了。
> 
> 比如**int类型**，它的取值范围是固定的，有限的，能够做的操作（加减乘除等）也是被限制的。
> 
> 那么这个定义能不能套在引用数据类型中呢？能否用数据类型的概念来统一基本数据类型和引用数据类型呢？
>
> 接下来我们需要分析一下，这个问题。
> 
> 在上一节类的定义中，类中的成员包括：
> 
> 1. 成员变量
> 2. 成员方法
> 
> 成员变量本质上就是数据，成员方法本质上就是操作，那么假设做以下类比：
> 
> 1. 数据的集合： 类中成员变量的集合
> 2. 操作的集合： 类中成员方法的集合
> 
> 于是，就可以做出以下总结：
> 
> 1. **一个类的定义，实际上就是定义了一种全新的数据类型，一种自定义的数据类型。**
> 2. **这种完全不同于基本数据类型的数据类型，我们称之为"引用数据类型"。**
> 
> 注：当然引用数据类型不仅仅包括类，但大体上上述说法是没问题的。

### 类加载

> 当我们在程序中使用一个基本数据类型时，由于基本数据类型是JVM当中已经预先定义好的（所以基本数据类型叫"内置数据类型"），JVM可以清楚的知道这个基本数据类型变量在内存中的存储方式（占用空间大小、结构等等），JVM能够正常开辟空间，正常给变量初始化赋值。

> 但是**类这种引用数据类型**，并不是内置数据类型，而是我们自定义的数据类型。
>
> 现在我们要根据一个类来创建它的对象，要让JVM帮助我们开辟空间创建引用和对象，JVM怎么知道到底要创建什么呢？难道它未卜先知吗？
>
> 显然是不可能的，某个类在一开始并不被JVM**"认识"**——它不知道类中有什么，必然不可能做任何操作。
>
> 所以在对某个类做任何操作之前，都需要让JVM来**"认识"**这个类型。
>
> 在Java中，把JVM**"认识"**一个类的过程，称之为**类加载（Class loading）**。

> 关于类加载：
>
> 1. 类加载的具体过程，我们后面会详细学习。这里我们先不用了解它的详细过程。
> 2. 类加载是通过把某个类的**二进制字节码文件（class文件）**通过I/O流的形式，读取进JVM内存中的方法区实现的。
> 3. 通过读取二进制字节码文件，并加载进JVM内存。这是JVM了解这个类型的过程。
> 4. 类加载之后，就可以做很多类型相关的操作了。
> 5. 类加载要在创建对象之前进行，换句话说**创建一个类的对象必然触发该类的类加载！**



## this关键字

注意事项：

1. this指向当前对象的隐含传参，必须是在普通成员方法中，加static的方法中，没有该this传参。**（所以static方法不能直接访问类的成员，需要先创建对象才能访问。）**

​			因为static方法不属于对象，而是属于类！

> ​			<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230305215059948.png" alt="image-20230305215059948" style="zoom:50%;" />

2. 既然this指向当前对象，那么不同的this指向的对象必然不同。



## 构造方法

### 语法

> 构造方法也是方法，但属于一种特殊的方法，具有以下特点：
>
> 1. 语法结构和一般方法不同，如下：
>
>    ```java
>    [访问权限修饰符] 类名(形参列表){
>      // 构造方法体
>    }
>    ```
>
>    注：
>
>    * 访问权限修饰符我们还没有学习，这里我们默认它是**public**修饰的。
>
>    * 类名的位置必须和当前类的类名完全一致。**（类名是大驼峰的，这里也要大驼峰）**
>
>    * 形参列表可以为空，称之为无参构造方法，简称**无参构造**。当然也可以有参数，是为**有参构造**。
>
> 2. 构造方法没有返回值，也不需要写返回值类型。（你也写不了！）
>
> 3. 构造方法体，和一般方法类似，可以写语句。具体后面详细说明。



### 构造器的作用

**在Java中使用new关键字创建某类的对象，必然调用该类的构造方法。但构造器的作用不是创建对象，而是在new对象的过程中用来给成员变量赋值的。构造器的作用是赋值！**

说明：

1. **new对象的过程，由JVM负责自动去调用该类的构造方法，构造方法的调用方式和普通方法是不同的。**
2. 创建对象的整个过程都由JVM负责完成，和构造器没有必然联系。new创建对象过程中，会伴随着构造器的执行。但不是构造器的执行就是创建对象，这个逻辑要理清楚。

### 构造器的使用

> 构造器不是给程序员去调用的，但是程序员可以指示JVM在创建对象时，用哪个构造器给成员变量赋值！
>
> 具体的方式是：
>
> ```java
> new 类名(实参列表);
> ```
>
> **通过实参列表的不同，来判断调用哪个构造器。这实际也是方法重载的应用！**

#### 课上代码

```java
package com.cskaoyan.javase.oop1._6constructor._0introduction;

/**
 * 创建一个教师类，有课程和年龄两个属性，行为是可以上课。
 * 现在我们需要创建以下对象：
 * 18岁的Java老师对象
 * 28岁的C++老师对象
 * 30岁的Python老师对象
 * ...
 * 按照之前我们的做法，需要先创建出对象，再进行成员变量的赋值。
 * 这样做如果只有一个两个对象还好，如果需要创建很多对象，就有点过于麻烦了。
 * 对象的属性，能不能"出厂"的时候就设定好呢？
 * 有这种需求时，就需要，构造方法（constructor，也叫构造器）来完成了。
 *
 * 1.构造方法的语法:
 * 构造方法属于特殊的方法,它的语法和普通方法是完全不一样的,参考以下格式:
 * [访问权限修饰符] 类名(形参列表){
 *   // 构造方法体
 * }
 * 解释:
 *      1.访问权限修饰符没学,现在先默认是public,当然完全可以空着不写
 *      2.普通方法在"类名"的位置一般写返回值类型和方法名
 *          构造方法没有返回值类型,也没有返回值,也不能使用return关键字
 *          语法结构中的"类名"可以认为是构造方法的名字,也就是说构造方法名和类名保持一致
 *          类名是大驼峰的,于是构造器的名字也是大驼峰的,需要和类名保持完全一致
 *      3.形参列表是普通方法一样,如果形参列表为空,就是一个空参构造器,也叫无参构造器
 *      4.构造方法的方法体类似于成员方法的方法体,因为它们都隐含了this传参,都可以使用this关键字
 *          this关键字指向当前对象
 *
 * 2.(重点)构造器的作用
 *      构造器的作用是创建对象,这是典型的错误观点
 *      构造器的作用不是创建对象,在new对象的过程中,创建对象是JVM所做的事情,构造器不负责创建对象
 *      实际上.
 *      构造器的作用是在new对象的过程中,被JVM自动调用,用来给对象的成员变量赋值
 *      所以构造器的作用是赋值,给成员变量赋值
 *
 *      解释:
 *          a.构造器不是由程序员手动去调用的一个方法,而是在new对象过程中由JVM自动去调用的
 *              构造器也没有办法,像普通方法一样去调用
 *
 *          b.(重点)虽然我们不能直接手动调用构造器,但是在JVM调用构造器时,我们可以指明JVM调用哪个构造器
 *              当然JVM调用构造器的作用是赋值
 *              语法:
 *              new 类名(实参列表);
 *              根据传入实参列表的不同,会调用不同的构造器(方法的重载)
 *
 * 3.构造器的定义
 *      a.对于一个类来说,如果类中没有提供任何一个构造器
 *      那么Java编译器在编译这个类的代码时,会自动加上一个无参构造器
 *      称之为该类的"默认无参构造"
 *      默认无参的格式是:
 *      [访问权限修饰符] 类名(){}
 *
 *      b.默认无参显然是没有办法给成员变量赋值
 *          那么如果想要实现赋值,就需要类中的有参构造器
 *          有参构造器,一般都按照下列格式定义(标准格式):
 *          构造器中是有this传参的,可以访问同类中的成员变量和成员方法
 *          [访问权限修饰符] 类名(数据类型 成员变量名1, 数据类型 成员变量名2 ...){
 *              this.成员变量名1 = 成员变量名1;
 *              this.成员变量名2 = 成员变量名2;
 *              ...
 *          }
 *
 *     c.同一个类当中,不同的构造器之间是方法的重载关系,这也是方法重载最常见的场景.
 *
 * 以上就是构造器的基本使用了
 *
 * @since 10:56
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    public static void main(String[] args) {
        // 18岁的Java老师对象
        Teacher t1 = new Teacher();
        t1.course = "Java";
        t1.age = 18;
        t1.teach();
        // 28岁的C++老师对象
        Teacher t2 = new Teacher();
        t2.course = "C++";
        t2.age = 28;
        t2.teach();
        // 30岁的Python老师对象
        Teacher t3 = new Teacher();
        t3.course = "Python";
        t3.age = 30;
        t3.teach();
        System.out.println("--------------------");
        Teacher t4 = new Teacher(18);
        System.out.println(t4.age);
        System.out.println("--------------------");
        Teacher t5 = new Teacher(48, "物理");
        t5.teach();
    }
}

class Teacher {
    int age;
    String course;

    public void teach() {
        System.out.println(age + "的老师,正在讲" + course);
    }

    // 默认无参构造器
    public Teacher() {
    }

    // 定义一个构造器,给age赋值
    public Teacher(int age) {
        this.age = age;
    }

    // 定义一个构造器,给age和course赋值
    public Teacher(int age, String course) {
        this.age = age;
        this.course = course;
    }
}

```



> 注意：
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230307141531035.png" alt="image-20230307141531035" style="zoom:67%;" />



## 代码块

### 静态代码块

#### 作用

静态代码块在类中的作用

**随着类加载的过程而执行，静态代码块可以看成是一个在类加载过程中，会自动调用的静态方法！用于给静态成员变量赋值！**

> 这里还是想再强调一下：**一般的静态成员方法是调用才会执行，并不是类加载过程中就会自动调用执行它！**
>
> **想要一段语句，能够在类加载过程中自动被调用，需要使用静态代码块，而不是静态方法！！**

#### 实践用途

> 静态代码块在实际开发中，并不常见。根据它的一些特点，可以总结一下它的使用场景
>
> 1. **复杂的静态成员变量的赋值。**
>
>    JavaEE中加载JDBC驱动（最经典的），也可能是最常见的。
>
> 2. **如果有一段代码，在类的全局，从始至终，只运行一次，可以写到静态代码块中。**（依赖于类加载只有一次的原理）
>
>    比如一些初类的始化工作，就可以放在静态代码块中完成。
>
>    最常见的就是类System的初始化，源码如下：
>
>    
>
>    图 1. System类源码
>
>    ![System类源码](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202203201845289.png?align=center)
>
>    
>
>    System类的初始化，依赖于本地方法**registerNatives()**的执行。

#### 注意事项

> 一些细节问题（重要）

1. 静态代码块可以近似看成一个，**在类加载时期自动调用的静态成员方法**，所以不能在里面访问非静态。（没有对象）

   > 包括this关键字，和后面学习的super关键字，都不能使用。
   >
   > 这意味**虽然构造代码块可以给静态成员变量赋值，但静态代码块不能给成员变量赋值。**
   >
   > **说白了，还是要搞清楚，谁先谁后执行的问题！**

2. 当需要使用复杂的代码给静态成员变量赋值时，可以使用静态代码块。

   > 但如果仅仅是简单的赋值，直接显式赋值即可。
   >
   > 总得来说，静态代码块用得不多。

3. **静态代码块也经常被用来测试类加载的顺序（重要）**

   > 一个类的静态代码块如果没有被执行，说明它没有被完全类加载。

#### 课上代码

```java
package com.cskaoyan.javase.oop1._12block._2static._0introduction;

/**
 * 静态代码块
 * 语法:
 * 就是比构造代码块多了一个static修饰,都是定义在成员位置
 * //成员位置
 * static{
 *   // 局部位置
 * }
 * //成员位置
 * 静态代码块当中定义的变量是局部变量,不要误以为其中定义的变量是静态变量
 *
 * 作用:
 * 在类加载的过程中,静态代码块会被自动执行,可以认为静态代码块是一个在类加载过程中自动被调用的静态方法,它的作用是给静态成员变量赋值
 *
 * 总结一下在类加载过程中,给静态成员变量赋值的手段:
 *      1.默认初始化,具有默认值
 *      2.显式赋值
 *      3.静态代码块赋值
 * 以上赋值,默认初始化永远最先执行,显式赋值和静态代码块赋值按照代码的书写顺序从上到下执行
 *
 * 原理:
 * 静态代码块之所以体现这样的执行特点,是由类加载的机制来保证的
 * 在类加载的最后一步,JVM会自动封装一个方法("clinit方法"),该方法的内容包括:
 *      1.静态成员方法的显式赋值
 *      2.静态代码块代码
 * 该方法封装代码时,按照代码的书写顺序从上到下封装
 * 随后JVM会执行这个方法
 * 该方法的执行是类加载的最后一步,该方法执行完毕,实际上类加载就结束了
 * 这个过程,实际上整体都是为了静态成员变量的赋值
 *
 * @since 10:13
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    public static void main(String[] args) {
        System.out.println(A.num);
    }
}

class A {

    static int num = 10;

    // 静态代码块
    static {
        num = 20;
    }
}
```



### 类加载详细过程（重要！）

首先我们来看一个代码案例：

```java
public class Demo{
static Demo d = new Demo();
}
```

在以上代码中，**"static Demo d = new Demo();"**语句需要在类加载时期，创建Demo类的对象。

那么问题就来了：Demo类加载都没有进行完毕，为什么能够创建Demo类的对象呢？ 创建对象不应该在类加载完成之后进行吗？

要想明白这些问题，就需要大致来看一下类加载的各个步骤的执行。



首先，一个类从被加载到JVM内存中开始，到卸载出内存为止，**一个类的生命周期**包括：

![image-20230307190552861](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230307190552861.png)

一共是：

1. **加载**（Loading）

2. **验证**（Verification）

3. **准备**(Preparation)

4. **解析**(Resolution)

5. **初始化**(Initialization)

6. **使用**(Using) 

7. **卸载**(Unloading)

   注：其中，验证、准备和解析可以统称为**连接(Linking)**。

一个类在JVM中的生命周期，共有七个阶段。

其中**"加载 --> 连接 ---> 初始化"**这三个步骤，即一个类的类加载过程。

这三步主要做：

1. **加载**主要是做将class字节码文件读取进JVM内存的操作。

2. 在**连接**过程中：

   1. **验证**，主要目的是为了确保class文件的字节流中包含的信息符合当前JVM的要求，不会影响JVM的安全。

   2. **准备**，主要目的是进行静态成员变量的默认初始化，设置初始值。

      这样，就**保证了静态成员变量的默认初始化，永远最先进行。**

      > 准备阶段是正式为类变量分配内存并设置类变量初始值的阶段，这些内存都将在方法区中进行分配。这个阶段中有两个容易产生混淆的概念需要强调一下，首先是这时候进行内存分配的仅包括类变量（被static修饰的变量），而不包括实例变量，实例变量将会在对象实例化时随着对象一起分配在Java堆中。其次是这里所说的初始值“通常情况”下是数据类型的零值，假设一个类变量的定义为：
      >
      > ```java
      > public static int value = 123;
      > ```
      >
      > 那么变量value在准备阶段过后的初始值为0而不是123，因为这时候尚未开始执行任何Java方法，而把value赋值为123的putstatic指令是程序被编译后，存放于类构造器<clinit>()方法之中，所以把value赋值为123的动作将在初始化阶段才会被执行。

      

   3. 解析，主要目的是将符号引用替换为直接引用。（不理解算了，目前不需要详细了解）

3. **初始化**是类加载的最后一个步骤。主要目的是执行**和static相关的内容**，包括：

   > 执行静态成员变量的显式赋值。
   >
   > 执行静态代码块。

> ​			<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230307192243816.png" alt="image-20230307192243816" style="zoom:150%;" />

以上，关于类加载各步骤，大致的作用，我们就了解了。

所以这里要重新认识一个概念：**类加载的时机**

类加载的时机，说得更准确一点，应该是**类初始化的时机**。**当然，想要初始化一个类，必然要先进行加载和连接。**

> Java中把一个类必须要进行初始化的场景称之为**类初始化的时机**，目前已经学习过的有：
>
> 1. 启动某个类的main方法，一定要初始化这个类。
> 2. new某个类的对象时，一定要初始化这个类。
> 3. 访问某个类的静态成员（包括变量和方法）时，一定要初始化这个类。

再回到上述案例中，通过启动main方法，JVM需要**初始化**类Demo，在进行Demo类初始化时，需要创建Demo类对象。

这种语法既然不报错，说明：

1. **类初始化步骤完成之前，这个类就可以创建对象了。创建对象，不依赖于完成类加载（初始化）。**

2. **某个类一旦开始进行初始化，就不会再重复进行一次初始化了！**

   > main方法启动已经使JVM开始初始化类Demo了，
   >
   > 即便初始化过程需要创建Demo对象，也不会又一次开始初始化类Demo了。直接创建对象即可。

我知道你有点晕，不妨，我们来看个案例，练习一下。

#### 案例1：(debug)一下

```java
package com.cskaoyan.javase.oop1._12block._2static._2exercise;
/**
 * 读程序题
 *
 * @since 10:51
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    static {
        System.out.println("Demo类开始初始化步骤了!");
    }
    static Cat cat = new Cat();
    static {
        System.out.println("Demo类结束初始化步骤了!");
    }
    Dog dog = new Dog();
    public static void main(String[] args) {
        System.out.println("hello world!");
        Demo d = new Demo();
    }
    public Demo() {
        System.out.println("demo");
    }
}

class Cat {
    static {
        System.out.println("Cat类开始初始化步骤了!");
    }
    static Dog dog = new Dog();
    static {
        System.out.println("Cat类结束初始化步骤了!");
    }
    public Cat() {
        System.out.println("cat");
    }
}
class Dog {
    static {
        System.out.println("Dog类开始初始化步骤了!");
    }
    // 在Dog类的类加载过程中,需要new创建Demo对象,这是一个什么样的操作呢?
    static Demo demo = new Demo();
    static {
        System.out.println("Dog类结束初始化步骤了!");
    }

    public Dog() {
        System.out.println("dog");
    }
}

```



#### 案例2：(debug)一下

```java
package com.cskaoyan.javase.oop1._12block._2static._2exercise;

/**
 * 读程序题
 * 在一般的,普遍的情况下,考虑类加载在前,new对象在后
 * 如果一个类中存在静态代码块,构造代码块,构造器的结构
 * 在new该类的对象时,它们的执行顺序是什么样的?
 *      1.静态代码块
 *      2.构造代码块
 *      3.构造器
 *
 * 但是本案例就不符合以上原则,因为它不是普通的场景
 * 因为在本案例中,在类初始化的过程中,需要new创建自身对象
 * 而且静态成员变量的显式赋值,在静态代码块的上面
 * 所以本案例中,以上结构的执行顺序是:
 *      1.构造代码块
 *      2.构造器
 *      3.静态代码块
 */

public class TestStaticDemo {
    public static void main(String[] args) {
        staticMethod();
    }

    // 静态成员变量的显式赋值需要new创建自身对象
    static TestStaticDemo ts = new TestStaticDemo();

    static {
        System.out.println("静态代码块");
    }

    {
        System.out.println("构造代码块");
    }

    public TestStaticDemo() {
        System.out.println("无参构造器");
        // 因为成员变量的显式赋值会先于构造器执行,所以a = 666
        // 而b是静态成员变量,此时它的显式赋值还没有轮到,所以b只有默认值,b=0
        System.out.println("a=" + a + ",b=" + b);
    }

    public static void staticMethod() {
        System.out.println("静态成员方法");
    }

    int a = 666;
    static int b = 777;

    static TestStaticDemo ts2 = new TestStaticDemo();
}

```

> 为啥类加载还没完成就可以new对象了？
>
> 结论：
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230307201021771.png" alt="image-20230307201021771" style="zoom:33%;" />
>
> ![image-20230307201056100](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230307201056100.png)
>
> 初始化负责执行和static相关的内容，包括：
>
> > 执行静态成员变量的显式赋值。
> >
> > 执行静态代码块。
>
> 当在初始化之前就可以new对象了

## 访问权限修饰符

### 访问级别

Java的访问权限的级别，是依赖**包（package）**来实现的。

Java的访问权限级别共分为以下四个级别，访问权限从严格到宽松顺序为：

1. 只能在同类中能够访问，私有的，外界一律不能访问。
2. 同一包中的子类或者其它类能够访问，同包中都可以使用。
3. 不同包的子类能够访问。
4. 不同包的其他类能够访问。

上述四种访问权限级别，分别对应三个关键字和一个缺省：

1. 私有的访问权限，对应关键字：**private**

2. 同包中能访问，对应**缺省**，表示在访问权限修饰符的位置空出来，什么都不写。

   比如，定义类的成员变量时：

   ```java
   String name;
   ```

   这就是一个缺省的访问权限，表示同包中都可以访问。

   这种访问权限一般称之为"默认的访问权限"、“缺省的访问权限”以及“包私有的访问权限”。

3. 不同包的子类能够访问，也就是受保护的访问权限。对应关键字： **protected**

4. 不同包的其他类都能访问，相当于没有控制权限，大家都能用，公共的访问权限。对应关键字： **public**

**注：当然宽松的访问权限总是包含严格的，比如public修饰，表示不同包都能用，自然同包或自身类中也能随便用了。**



## 问题（待解决）

### 1.Java中为什么不能用private protect修饰外部类

* 为什么不能用private？

> [(89条消息) Java中为什么不能用private protect修饰类_苦心僧的博客-CSDN博客](https://blog.csdn.net/qq_45736483/article/details/106475476)		
>
> 对于顶级类(外部类)来说，只有两种修饰符：public和默认(default)。因为外部类的上一单元是包，所以外部类只有两个作用域：同包，任何位置。因此，只需要两种控制权限：包控制权限和公开访问权限，也就对应两种控制修饰符：public和默认(default)。
>
> 如果类使用了private修饰符，说明是个内部类。内部类的上一级是外部类，那么对应的有四种访问控制修饰符：本类(private)，同包(default)，父子类(protected)，任何位置(public)。当一个内部类使用了private修饰后，只能在该类的外部类内部使用。
>
> 上面这些都是平时使用司空见惯的，但是为什么是这种情况呢？
>
> 可以想一下，一个java项目是不可能在一个class里面完成的。mvc模式中，是把类分为三层，一层层调用类。如果定义为私有的和受保护的就无法调用。换句话说，对于一个java文件，要么就是自己单独运行，要么就是被其他程序作为库调用，如果一个java文件的类被private修饰，那么是不是其他的程序或是类是无法使用它的，那么他作为一个单独的文件就没啥用了。如果它作为单个文件运行，类加载怎么找到它呢，因为它对外不可见。同时，也失去了类的存在意义。因此，类只有public和默认修饰符。

* 为什么不能用protected？

> ![image-20230312214436920](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230312214436920.png)
>



# 封装



# 继承

## 引用数据类型的类型转换

## 继承的限制

```java
package com.cskaoyan.javase.oop2._1extends._5limit;

import com.cskaoyan.javase.oop2._1extends._5limit.a.A;

/**
 * 继承的限制
 * 在前面，继承的定义中，我们说子类会继承父类的所有成员，那么思考以下问题：
 *      1.子类继承父类的成员,那么父类的私有成员(以及子类没有权限的成员)能不能继承?
 *          可以继承的,只不过是由于没有访问权限,导致子类没有办法直接访问罢了
 *          可以通过getter方法进行间接的访问
 *      2.父类的静态成员能不能继承?
 *          普通成员是属于对象的,被子类继承后,创建子类对象,该被继承的成员就属于子类对象了,这才是继承
 *          而静态成员属于类,虽然子类类名也可以使用父类的静态成员
 *              但这不是继承,而是子类和父类共用了父类的静态成员
 *          静态成员属于类,它没有继承的概念,该属于谁就属于谁,它不会被继承.
 *
 *      3.父类的构造器能不能继承?
 *          不能继承的
 *
 * @since 10:10
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    public static void main(String[] args) {
        ASon as = new ASon();
        System.out.println(as.getNum());
        System.out.println(as.getNum2());

        System.out.println("-------------------");
        System.out.println(B.num);
        B.num = 20;
        System.out.println(BSon.num);
    }
}
class B{
    static int num = 10;
}
class BSon extends B{
    static int num = 100;
}

class ASon extends A {

}
```

## 子类对象的初始化

### 基础

```java
package com.cskaoyan.javase.oop2._1extends._7init._1basic;

/**
 * 我们通过一个引例，练习并讲解这个问题：
 * 创建一个Person类，有name属性和eat方法。
 * 创建一个Star类，有stageName属性和sing方法。
 * Star类要继承Person类。
 * 创建Star这个子类对象，通过画图/运行代码等研究子类对象初始化的过程。
 *
 * 现在程序运行,需要创建子类Star的对象,new对象,需要先考虑类加载
 * 所以Star类是必然需要类加载的
 * 但是Star还有父类Person
 * 子类继承父类,会得到父类的成员,那么继承到底继承了父类什么成员呢?
 * 所以为了解决这个问题,父类也必然是需要类加载的
 *
 * 既然要类加载父类,那么类加载的顺序是什么样的?
 * 是"先父后子"的
 * 先进行父类类型的类加载,然后再进行子类的类加载
 *
 * 在子类对象初始化时,创建子类对象,触发子类类加载,会优先类加载父类
 * 而且是从最顶层父类开始向下进行类加载
 * 子类的类加载的触发方式可以是任意方式,也就是说只要触发子类的类加载,那么就一定会优先类加载父类
 * 这也是一种类加载的时机,总结类加载时机如下:
 *      1.new对象
 *      2.启动main方法
 *      3.访问类的静态成员
 *      4.触发子类类加载,优先类加载它的父类
 *
 * 有了继承以后,new子类对象,在堆上会创建几个对象呢?
 * 只会创建一个子类对象本身,不会创建任何父类对象,只有一个对象
 *
 * 这个子类对象当中,是有进一步的内存区域划分的:
 * 子类对象中会专门开辟一片独立的区域，用来存储父类的成员变量，而子类自身的成员仍会存储在自身对象当中。
 * 这样子类对象就被划分为了两个区域：
 *      1.自身成员的区域，自身对象的区域，该区域用隐含this引用指向。
 *      2.父类成员的区域，该区域用super关键字指向。
 *          super关键字用于指向子类对象当中,装父类成员的区域
 *
 * this指向当前对象,其实就是子类对象本身,this指向的是一个对象
 * 而super指向子类对象中装父类成员的区域,super指向的是子类对象中的一片区域,没有指向一个对象
 *      但是super指向的内存区域非常类似于一个父类对象
 *      所以可以近似的认为super指向父类对象
 *
 *
 * (最重要)子类对象创建完毕后,开始考虑给父子类的成员变量赋值
 * 首先对于父子类成员变量的默认初始化,我们不需要考虑,因为它们永远是最先执行的
 * 任何其它的赋值手段一定在默认值的基础上进行
 * 除了默认初始化,还有:
 *      1.显式赋值
 *      2.构造代码块赋值
 *      3.构造器赋值
 * 以上三种方式的赋值,它们的赋值顺序是什么呢?
 * 我们已经知道,在同一个类当中,显式赋值和构造代码块赋值按照代码的书写顺序从上到下执行
 * 而构造器赋值最后执行
 * 现在有了继承,有了父类和子类,一共至少两个类
 * 那么它们在各自的父子类之间,是先给父类成员变量赋值,还是先给子类?
 * 很明显是"先父后子"的
 * 先给父类的成员变量赋值,再给子类的成员变量赋值
 *
 * 为什么有这样的先父后子的执行顺序呢?如何保证呢?
 * 只需要保证父类的构造器先于子类的所有赋值手段执行就可以了
 * 只需要保证父类的构造器先于子类的构造器执行就可以了
 * 而实际上也确实是这样的
 * 在子类对象初始化的过程中,父类的构造器永远会先于子类构造器执行
 *
 * 为了保证以上执行顺序,在Java当中子类初始化的方式有两种:
 *      1.子类对象的隐式初始化
 *      (重点)
 *      在一个Java类中的任何一个构造器中
 *      如果构造器的第一行没有明确的使用this/super表示调用其它构造器,那么该构造器的第一行就隐含了
 *      super();
 *      表示去调用父类的无参构造器
 *      this在构造器中可以表示调用子类自身构造器
 *      super在构造器中可以表示调用子类的父类构造器
 *
 *      2.子类对象的显式初始化
 *         子类对象的隐式初始化只能自动调用父类的无参构造器
 *         无参构造器无法给父类成员变量赋值
 *         所以可以在子类构造器的第一行使用语法:
 *         super(实参列表);
 *         明确的指示调用父类的某个构造器
 *         来完成父类成员变量的赋值
 *
 * @since 11:31
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    public static void main(String[] args) {
        // Star s = new Star();
        // System.out.println(s.stageName);
        Star s = new Star("李四");
        System.out.println(s.name);
        System.out.println(s.stageName);
    }
}

class Person {
    String name = "张三";
    // static {
    //     System.out.println("Person类加载了!");
    // }

    {
        System.out.println("Person的构造器执行了!");
    }

    public Person() {
    }

    public Person(String name) {
        this.name = name;
    }

    public void eat() {
        System.out.println("人要吃饭!");
    }
}

class Star extends Person {
    String stageName = name + "的狗!";
    // static {
    //     System.out.println("Star类加载了!");
    // }

    {
        System.out.println("Star的构造器执行了!");
    }

    public Star() {
        // 表示去调用父类的无参构造器
        // super();
    }

    public Star(String name) {
        // 调用父类的单参name构造器
        super(name);
    }

    public void sing() {
        System.out.println("练习两年半,唱了一首爱的供养!");
    }
}
```



### super关键字和this关键字的区别

```java
package com.cskaoyan.javase.oop2._1extends._7init._3super;

/**
 * super关键字 vs this关键字
 * 首先这两个关键字都是和子类对象相关的,所以它们都是可以在类的非静态上下文使用的
 * 可以在:
 *      1.成员方法
 *      2.构造器
 *      3.构造代码块
 * 注意:
 *      1.在成员方法,构造代码块中,this表示指向当前子类对象,super指向子类对象中父类成员的区域
 *          可以近似看成super指向父类对象
 *      2.在构造器中,除了有上述指向对象的用途外,还可以用来表示调用不同的构造器
 *          其中this表示调用子类自身的构造器
 *          super表示调用父类的构造器
 *      3.一般情形下,在表示调用父子类成员时,this的范围要更广,super仅能用于访问父类成员
 *          但是在特殊情况下,父子类出现同名成员时,可以用super访问父类成员以区分
 *
 * this和super必然是不同的:
 *      1.(最根本的区别)this指向当前对象,this是一个引用
 *          super可以认为并不是一个引用,它并不是真的指向一个对象,指向的是子类对象中父类成员的区域
 *          this是可以直接输出的,super并不能直接输出
 *
 *      2.super和this在表示访问父子类成员时,this毕竟是自己访问自己,所以this不受权限限制
 *          super毕竟是访问父类,所以受权限限制
 *
 * 最后在表示调用构造器时,this和super很相似
 *      它们都必须要争抢构造器代码的第一行,所以它们是不可能同时存在的,只能同时存在一个
 *      也必然是有一个:
 *      如果写了就有一个
 *      如果不写,就默认是super();
 *
 * @since 14:51
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
}

class Father {
    private int num = 10;

    public Father() {
    }

    public Father(int num) {
        this.num = num;
    }
}

class Son extends Father {
    // 父子类出现同名成员变量
    int num = 100;
    int num2 = 20;

    public void test(int num) {
        System.out.println(num);
        System.out.println(this.num);
        // super.访问受权限限制
        // System.out.println(super.num);
    }

    public Son() {
        // super();
    }

    public Son(int num) {
        // super();
        this.num = num;
    }

    public Son(int num, int num1) {
        super(num);
        this.num = num1;
    }
}
```



## 继承中的属性隐藏

```java
package com.cskaoyan.javase.oop2._1extends._8hidden;

import org.junit.Test;

/**
 * 什么是属性的隐藏?
 * 当父子类出现同名成员变量时,创建子类引用指向子类对象,用这个子类引用访问同名成员变量
 * 得到的结果是子类中的结果
 * 而这时想要访问父类中的同名成员变量,可以在父类中提供Getter方法
 * 然后使用子类引用调用该方法访问父类同名成员
 * 这个现象就是"属性的隐藏"
 *
 * "属性的隐藏"归根到底是"对象名.成员变量"的访问机制决定的
 * 父子类同名成员变量,想要访问,除了Getter方法,还可以使用super关键字
 *
 * (重点)下面的重点是研究"对象名.成员变量名"的访问机制
 * 从两个角度研究:
 *      1.研究"对象名.成员变量名"的访问范围
 *      2."对象名.成员变量名"的访问结果
 *
 * 研究的手段,要区分不同形式的"对象名",得到一个"对象名"目前有以下几种手段:
 *      1.子类引用指向子类对象
 *      2.父类引用指向父类对象
 *      3.父类引用指向子类对象
 *
 * 首先研究"对象名.成员变量名"的访问范围:
 *      1.子类引用指向子类对象
 *          访问范围是 父类 + 子类
 *
 *      2.父类引用指向父类对象
 *          访问范围是 父类
 *
 *      3.父类引用指向子类对象
 *          访问范围是 父类
 *
 * 综上所属,"对象名.成员变量名"的访问范围是依赖于引用决定的:
 *      1.如果引用是一个父类类型,那么访问范围就只有父类
 *      2.如果引用是一个子类类型,那么访问范围就是父类 + 子类
 *
 *  原理:
 *      1."访问范围"实际上是一个编译上的概念,编译器决定是否能够访问,如果可以访问编译器就通过编译,否则就编译报错
 *      2.创建引用的过程就是一个声明的过程,声明的目的是告诉编译器当前这个变量的数据类型
 *      也就是说引用指向对象,引用是什么类型,编译器就认为这个引用数据类型变量是什么类型
 *
 *      3.基于以上两点以及我们得出的结论
 *      我们可以做以下推论:
 *      编译器在根据引用的数据类型决定该引用能够访问成员的范围时,
 *      会优先从本类(引用的数据类型)中找是否存在该成员
 *      如果没找到,就去父类中找(因为继承了父类)
 *      直到找到Object,如果都没有该成员
 *      那么就会报错
 *
 *      注意,不能去子类中找,只能向上找父类
 *
 * 接下来研究"对象名.成员变量名"的访问结果:
 *      1.子类引用指向子类对象
 *          结果都是子类中的结果(如果是继承父类的独有成员变量,结果是父类)
 *
 *      2.父类引用指向父类对象
 *          结果都是父类中的结果
 *
 *      3.父类引用指向子类对象
 *          结果都是父类中的结果
 *
 * 以上总结,
 * "对象名.成员变量名"的访问结果是依赖于引用的数据类型来决定的
 *
 * 综合对象名点访问成员变量的范围和结果，发现：
 * 都是根据引用的数据类型来决定的，无需考虑是何种对象。
 *
 * @since 15:54
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    @Test
    public void test() {
        Son s = new Son();
        System.out.println(s.num);
        System.out.println(s.getNum());
        s.superAccessFatherNum();
    }

    @Test
    public void test2() {
        // 1.子类引用指向子类对象
        Son s = new Son();
        System.out.println(s.num);
        System.out.println(s.fatherNum);
        System.out.println(s.sonNum);

        // 2.父类引用指向父类对象
        Father f = new Father();
        System.out.println(f.fatherNum);
        System.out.println(f.num);

        // 3.父类引用指向子类对象
        Father fs = new Son();
        System.out.println(fs.num);
        System.out.println(fs.fatherNum);
        // fs.sonNum
    }

    @Test
    public void test3() {
        // 1.子类引用指向子类对象
        Son s = new Son();
        System.out.println(s.num);
        System.out.println(s.fatherNum);
        System.out.println(s.sonNum);

        // 2.父类引用指向父类对象
        Father f = new Father();
        System.out.println(f.fatherNum);
        System.out.println(f.num);

        // 3.父类引用指向子类对象
        System.out.println("-------------");
        Father fs = new Son();
        System.out.println(fs.num);
        // 100
        System.out.println(fs.fatherNum);
    }

}

class Father {
    int num = 10;
    int fatherNum = 100;

    public int getNum() {
        return num;
    }
}

class Son extends Father {
    int num = 20;
    int sonNum = 200;

    public void superAccessFatherNum() {
        System.out.println(super.num);
    }
}
```



### 总结

综合对象名点访问成员变量的范围和结果，发现：**都是根据引用的数据类型来决定的，无需考虑是何种对象。**

注意事项：

1. 父子类中的同名成员变量它们各自有存储的区域，父类的同名成员变量被子类同名成员变量隐藏了，称之为"属性的隐藏"。

   但我们仍然可以通过父类中的Getter方法，或者通过super去访问到父类中同名成员变量，当然它们都受访问权限限制。

2. 静态成员变量在父子类中也存在同名的情况，但是它们不是覆盖也不是隐藏，而是互相独立的两个静态成员变量。

   对于下列代码：

   ```java
   class Person {
       static String nationality;
   }
   
   
   class Student extends Person {
       static String nationality;
   }
   ```

   Person类和Student类的静态成员变量`国籍`分别属于两个类本身，没有所谓继承关系。

   而如果是下列代码：

   ```java
   class Person {
       static String nationality;
   }
   
   class Student extends Person {
   }
   ```

   Person类和Student类都可以使用Person类的静态成员变量`国籍`，是共用的关系。



## 继承中的方法覆盖

### 关于super限定

> super是Java提供的一个关键字，super用于限定该对象调用它从父类继承得到的实例
>
> 变量或方法。正如this不能出现在static修饰的方法中一样，super也不能出现在static修饰的
>
> 方法中。static修饰的方法是属于类的，该方法的调用者可能是一个类，而不是对象，因
>
> 而super限定也就失去了意义。



> #### 问题：重载和重写的区别？
>
> 其实把重载和重写放在一起比较本身没有太大
>
> 的意义，因为重载主要发生在同一个类的多个同名方法之间，而重写发生在子类和父类的
>
> 同名方法之间。它们之间的联系很少，除二者都是发生在方法之间，并要求方法名相同之
>
> 外，没有太大的相似之处。当然，父类方法和子类方法之间也可能发生重载，因为子类会
>
> 获得父类方法，如果子类定义了一个与父类方法有相同的方法名，但参数列表不同的方
>
> 法，就会形成父类方法和子类方法的重载。



# 面向对象设计

## 抽象类



## 接口【问题】

> 什么时候应该使用接口？
>
> [何时使用抽象类？何时使用接口？ - 简书 (jianshu.com)](https://www.jianshu.com/p/28e3b4d61945)
>
> 在Java中接口存在意义是什么? (语言层面设计)
> // 接口是用来定义规范的.
>
> 在Java中接口和接口之间的继承是为了什么?  (语言层面设计)
> // 定义/规范  的  增强

## 内部类（**语法定义了一个类，包括成员内部类、静态内部类和局部内部类**）

在内部类课程当中，我们统一规定：

1. 像CPU这种，定义在别的类的内部的类，我们称之为内部类。（inner）
2. 像Computer这种，包裹内部类的，我们称之为外围类。（enclosed）
3. Demo这种类我们称之为外部类。（outside）

> 内部类怎么学?把什么当成重点?
>  内部类在Java中更倾向于是一种优秀合理的设计,它在很多地方都不是必须使用的,但是使用它会更加合理
>
> 在集合体系的设计中,内部类是非常常见
>
> 在大家日常的开发中,内部类也不是"非用不可",大多数的场景都是可以不用,因为你不需要那么优秀的设计
>
> 所以在目前这个阶段,可以不理解内部类,可以不太会用内部类,但是一定要看得懂内部类语法
>
> 因为在源码当中内部类很常见
>
> 对于以下五种内部类(对象):
>
> 1. 成员内部类,静态内部类,了解语法为主,不要求会使用,会看懂它的语法就够了
>
> 2. 局部内部类,实际开发中很少见,了解语法为主,不要求会使用,会看懂它的语法就够了
>
> 3. (重点)
>
>     Lambda表达式和匿名内部类,它们是特殊的局部内部类,它们非常重要,日常开发中很常见,尤其是Lambda表达式，因为使用它们的目的不是优秀的设计,而是单纯为了简化优化代码,使得代码更加优雅



### 成员内部类

```java
package com.cskaoyan.javase.oop3._2inner._1member._0introduction;

/**
 * 成员内部类是最普通的内部类,它直接定义在另一个类的成员位置
 * 语法：
 * //外围类
 * [访问权限修饰符] class EnclosedClazz{
 * //成员内部类
 *   [访问权限修饰符] class InnerClazz{
 *  }
 * }
 * 成员内部类的自身特点
 * 主要从以下几个角度分析：
 *      1.成员内部类首先仍然是一个类,它的命名,仍然和普通类命名是一样的
 *      2.访问权限修饰符,四种访问级别皆可,尤其是可以私有化
 *      3.(最重点)成员内部类的自身特点,在所有内部类当中,成员内部类有什么特殊的地方呢?
 *          在内部类的设计体系中,成员内部类被设计为完全依赖于外围类而存在的一种内部类
 *          -->
 *          成员内部类对象必须完全依赖于外围类对象而存在
 *          -->
 *          成员内部类对象必须持有外围类对象的引用作为自身的成员变量
 *          -->
 *          (重点)
 *          要想得到一个成员内部类对象,必须先创建外围类对象,然后在外围类对象的基础上才能创建成员内部类对象
 *
 *      4.(重点)成员特点
 *          成员内部类也是类,但是它的和普通类不同
 *          成员内部类当中没有静态声明,包括:
 *              a.静态成员变量,静态成员方法
 *              b.静态代码块
 *          但是可以定义使用字面值常量赋值的全局常量
 *
 *      5.继承和实现
 *          可以继承,可以实现
 *          可以继承外部类,也可以继承内部类
 *          可以实现外部接口,也可以实现内部接口
 *
 * 思考题:
 *      在有权限的前提下,在其他类当中,能不能去继承一个成员内部类呢?
 *      可以(大家课下可以研究一下)
 *
 * @since 10:27
 * @author wuguidong@cskaoyan.onaliyun.com
 */
```

#### 访问

成员内部类的访问特点，主要从以下几个角度研究：



**1.(重点)成员内部类内部访问外围类成员**

> 访问的位置有哪些?
>
> 主要指的是非静态上下文,包括:
>
> 成员方法,构造器,构造代码块
>
> 由于以上结构当中,都已经存在了外围类对象
>
> 所以可以直接访问外围类成员
>
> 如果出现同名,那就用"外围类类名.this"指向外围类对象区分



**2.(重点)外围类访问成员内部类成员**

访问的位置有哪些?

> 外围类是一个普通类,所以访问位置要考虑
>
> 成员方法等非静态上下文以及静态上下文

这时是**不会直接存在成员内部类对象的**,要想访问成员内部类成员,需要自己new一个成员内部类对象

怎么new?

> 成员内部类对象会强依赖于外围类对象,需要在外围类对象的基础上,去new成员内部类对象
>
> 语法:
>
> **成员内部类类名 对象名 = 外围类对象.new 成员内部类类名(实参);**
>
> 有了对象以后,该怎么访问就怎么访问,不受权限限制



3.(了解)外部类访问成员内部类成员

a.外部类当中要想访问成员内部类成员,需要什么权限呢?

> 需要外围类权限,成员内部类权限,成员内部类成员权限
>
> 以上三个权限缺一不可

b.外部类的静态上下文和非静态访问,有区别吗?

> 没有区别,反正都没有外围类对象
>
> 所以想要访问,都需要先创建外围类对象,再创建成员内部类对象
>
> 语法:
>
> **外围类类名.成员内部类类名 对象名 =  new 外围类类名(实参列表).new 成员内部类类名(实参列表);**



4.(了解)成员内部类访问外部类成员

可以访问,但是全程都受权限限制





## 内部类对象（**语法直接创建了一个对象，包括匿名内部类和Lambda表达式**）





# Java常用API

## **Object类**



## **String类**

### String类自身特点

#### 字符串常量池

##### 字符串常量池的作用（重点）

> String对象和Java程序当中的所有对象一样，它的创建和使用都是需要耗费资源的。
>
> 但String对象比较独特的地方在于——Java程序中，String对象无论是数量还是使用频率都远不是一般对象可以比拟的。
>
> 思考一下，这么多String对象如果频繁创建，频繁销毁，对Java程序的性能影响将会非常大。
>
> 所以JVM对String对象在堆上的使用有特殊的处理：
>
> **JVM为了提高性能和减少内存的开销，在创建字符串String对象的时候进行了一些优化——使用字符串常量池。**
>
> 所以字符串常量池的使用目的和作用就是为了提升Java程序的性能，减少JVM内存开销。
>
> 那么字符串常量池究竟是如何工作的，它是如何优化频繁使用String对象的性能呢？



##### 常量字符串对象唯一

> 首先我们看一段代码：
>
> ```java
> String s1 = "hello";
> String s2 = "hello";
> System.out.println(s1 == s2);
> ```
>
> 上述代码输出的结果是：
>
> > true
>
> 这说明：s1和s2两个引用指向的”hello“对象是堆上的同一个对象，而其中的原因就是因为字符串常量池，上述代码的执行，在JVM当中可以做以下描述：
>
> 1. 当代码执行到**”第一次用字符串字面值常量'hello'，赋值引用's1'的语句“**时，**会在堆上创建"hello"字符串常量对象，然后将该对象的地址存入字符串常量池中。**
> 2. 字符串常量池的本质是一个哈希表，在堆上创建的常量字符串对象的地址都会存入字符串常量池，**字符串常量池中不会存储两个相同内容的字符串对象的地址。**
> 3. 当代码执行到**”第二次使用字符串字面值常量'hello'，赋值引用s2的语句“**时，就不会在堆上创建字符串对象了，而是直接获取字符串常量池中该对象的地址。相当于s1和s2通过字符串常量池共用了同一个String对象！
>
> 这里做一下总结：
>
> 1. 在Java代码中第一次用字符串字面值常量赋值时，会在堆上创建该字面值常量字符串对象。
> 2. 再次使用**相同内容的**字符串字面值常量赋值时，会直接复用堆上对象，而不会新建对象。
>
> 这就是标题中所说的**常量字符串对象唯一**，再**结合String对象的不可变性**，将地址存储在字符串常量池中的字符串对象，完全可以实现复用，大大提升了字符串对象的使用性能。**（必须是不可变对象，才能实现这样的复用）**

> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230315090144972.png" alt="image-20230315090144972" style="zoom:50%;" />
>
> 总之，String对象不可变加上字符串常量池的应用，实现了对**”Java常量字符串对象“**的复用。



### String类API

#### 字符串比较大小

> String类中，存在两个用于比较字符串大小的方法，即**String比较大小**的功能。
>
> ```java
> // String类的比较功能
> int compareTo(String str)
> int compareToIgnoreCase(String str)
> ```
>
> 既然是比较大小，这里最重要的就是要理解何为**字符串的大小**，字符串比较大小的规则是什么。
>
> 字符串由多个字符组成，要想理解字符串比较大小的规则，首先要了解一下字符比较大小的规则。

#### 自然排序

> String类的**比较功能**，实际上是要分成两类的：
>
> 1. 我们最早的接触的equals和equalsIgnoreCase这两个方法，用于比较字符串是否内容相同。equals注重比较字符串是否相等，注重比较字符串内容是否一样，**它只有相等的概念，没有大小的概念。**
> 2. 第二类就是上面学习的compareTo的两个方法。compareTo专注于比较字符串的大小，**它有大小的概念，当然也有相等的概念。**
>
> 所以，为什么String中在equals比较相等之外，还需要compareTo方法来比较大小呢？
>
> **因为排序，有了大小，才有了排序。String类的compareTo方法，其目的就是为了实现排序。**

##### 什么是自然排序

> **注意：**String类的**compareTo**方法并不是该类自定义的一个方法，而是重写自String类实现的接口**Comparable**中的compareTo抽象方法。
>
> 某个类实现Comparable接口后，重写compareTo方法，该方法就表示一个比较该类对象大小的比较规则，然后就可以通过以下方法，实现对该类对象的容器的排序：
>
> 1. 如果是对象数组容器，那么使用```Arrays.sort(数组容器)；```                                                                        方法来实现数组容器中，对象的**从小到大**排序。
> 2. 如果是集合容器，那么使用```Collections.sort(集合容器);```                                                                       方法来实现集合容器中，对象的**从小到大**排序。
>
> **Arrays.sort()方法**或**Collections.sort()方法**会自动两两比较容器中的元素（重写的compareTo方法就表示比较大小的规则），然后在原先的容器上按照从小到大进行排序，排序方法没有返回值的（当然也不需要返回值）。
>
> **这种让某个类实现Comparable接口，重写compareTo方法表示排序规则，然后实现对象容器中元素从小到大的排序方式，称之为"自然排序"，其中的compareTo方法被称为该类的自然比较方法。**
>
> String类的自然排序代码案例（基于数组）：
>
> ```java
> String[] arr = {"abc", "bcd", "aaa", "bbb", "ccc", "a", "yyy"};
> Arrays.sort(arr);
> System.out.println(Arrays.toString(arr));
> ```
>
> 输出结果：
>
> > [a, aaa, abc, bbb, bcd, ccc, yyy]
>
> 这就是String类的自然排序。

##### Comparable接口

> 所有类都可以通过实现Comparable接口来最终实现自然排序，当然也包括我们自定义的类。
>
> 这里给出一个**自定义Student类**实现Comparable接口，并重写compareTo方法的案例。**其中compareTo方法表示作为自然比较方法，它用于表示排序的规则，只要懂得重写该方法，基本就学会了自然排序。**
>
> 案例：
>
> ```java
> package com.cskyan.javase.string._5comparable;
> 
> import com.sun.xml.internal.ws.api.ha.StickyFeature;
> 
> import java.util.Arrays;
> 
> /**
>  * String类中，存在两个用于比较字符串大小的方法，即String比较大小的功能。
>  * // String类的比较功能
>  * int compareTo(String str)
>  * int compareToIgnoreCase(String str)
>  * 既然是比较大小，这里最重要的就是要理解何为字符串的大小，字符串比较大小的规则是什么。
>  * 字符串由多个字符组成，要想理解字符串比较大小的规则，首先要了解一下字符比较大小的规则。
>  *
>  * compareTo方法不是String类自定义的,而是它实现接口java.lang.Comparable重写的抽象方法
>  * 单个字符比较大小的规则: 字符的编码值越大,字符就越大,"字典顺序"
>  * 字符串比较大小的规则就是compareTo方法的实现:
>  *      1.遍历两个String对象的字符,然后返回第一个不相同字符的编码值差
>  *      2.如果遍历比较完毕对应位置的字符,字符都相同,那么就返回它们的长度之差
>  * 怎么判断字符串的大小呢?
>  * (String s1).compareTo(String s2)
>  * 这个方法就直接看成s1 - s2
>  * 所以:
>  * 如果方法返回大于0的数，则认为方法调用者字符串s1大于方法形参字符串s2。
>  * 如果方法返回小于0的数，则认为方法调用者字符串s1小于方法形参字符串s2。
>  * 如果方法的返回值就是0，则认为方法调用者字符串s1等于方法形参字符串s2。
>  *
>  *
>  * 一个类通过实现Comparable接口,重写抽象方法compareTo表示比较大小的规则,于是就可以对该类型的对象容器进行排序
>  * 这种排序就称之为自然排序
>  * 自然排序依赖于以下方法:
>  *      1.如果容器是数组,用Arrays.sort(对象数组);
>  *      2.如果容器是集合,用Collections.sort(集合容器);
>  * 自然排序依赖于其中的compareTo方法表示的比较规则
>  * 将对象按照从小到大的顺序进行排序
>  *
>  * Comparable接口实现自然排序局限性很大:
>  *      1.需要修改代码,排序规则绑定类
>  *      2.在设计上equals方法对compareTo方法是存在影响:
>  *          如果equals方法认为相等，compareTo方法也应该返回0，它们在排序时处在相同的位置。
>  *          如果equals方法认为不相等，compareTo方法应该返回非0，它们在排序时必须处在不同的位置。
>  *          要实现以上两点,必须要求两个方法同时重写,而且重写的依据是一样的
>  *          这显然也是很麻烦的
>  *
>  * @since 09:31
>  * @author wuguidong@cskaoyan.onaliyun.com
>  */
> public class Demo {
>     public static void main(String[] args) {
>         String s1 = "abc";
>         String s2 = "aac";
>         // 1
>         System.out.println(s1.compareTo(s2));
>         String s3 = "b";
>         // -1
>         System.out.println(s1.compareTo(s3));
>         String s4 = "abcd";
>         // -1
>         System.out.println(s1.compareTo(s4));
>         String s5 = "abc";
>         // 0
>         System.out.println(s1.compareTo(s5));
> 
>         String[] strs = {s1, s2, s3, s4, s5};
>         System.out.println(Arrays.toString(strs));
>         Arrays.sort(strs);
>         System.out.println(Arrays.toString(strs));
> 
>         Student[] stus = new Student[10];
>         stus[0] = new Student(18, 500);
>         stus[1] = new Student(28, 200);
>         stus[2] = new Student(38, 400);
>         stus[3] = new Student(8, 300);
>         stus[4] = new Student(17, 300);
>         stus[5] = new Student(17, 360);
>         stus[6] = new Student(17, 379);
>         stus[7] = new Student(17, 370);
>         stus[8] = new Student(17, 500);
>         stus[9] = new Student(17, 600);
>         // System.out.println(Arrays.toString(stus));
>         for (Student s : stus) {
>             System.out.println(s);
>         }
>         System.out.println("---------------------");
>         Arrays.sort(stus);
>         // System.out.println(Arrays.toString(stus));
>         for (Student s : stus) {
>             System.out.println(s);
>         }
>     }
> }
> 
> class Student implements Comparable<Student> {
>     int age;
>     double score;
> 
>     public Student(int age, double score) {
>         this.age = age;
>         this.score = score;
>     }
> 
>     @Override
>     public String toString() {
>         return "Student{" +
>                 "age=" + age +
>                 ", score=" + score +
>                 '}';
>     }
> 
>     // 该方法表示比较的规则
>     @Override
>     public int compareTo(Student s) {
>         // 大小的规则看成this - s
>         // 规则一: 按照年龄从小到大排序
>         // 站在this的角度,这个规则就意味着年龄越大,排序越在后面,那就是对象越大,方法就越应该返回一个正数
>         // return age - s.age;
> 
>         // 规则二: 按照成绩从大到小排序
>         // 站在this的角度,这个规则意味着成绩越高,排序越靠前,对象就越小,方法就越要返回一个负数
>         // return (int) (s.score - score);
> 
>         // 规则三: 首先按照年龄从小到大排序,如果年龄一样按照成绩从大到小排序
>         // 在年龄不相同的情况下,按照年龄排
>         if (age != s.age) {
>             return age - s.age;
>         }
>         // 代码运行到这里,说明年龄是一样的,它们按照成绩排
>         return (int) (s.score - score);
>     }
> }
> ```

###### 缺点：



> **局限性**
>
> 让一个类实现Comparable接口，从而实现自然排序，局限性是很大的：
>
> 1. 首先，实现Comparable接口会将排序规则直接和类绑定，灵活性大大降低，一个类无法同时拥有多种排序规则。
> 2. 其次，实现自然排序，需要修改源代码，这在很多时候是做不到的。（公司中的代码不是你想改就能改的。）
>
> Comparable接口除了灵活性欠佳，实际上还有一个非常大的、在设计类时的麻烦：
>
> 在设计上equals方法对compareTo方法是存在影响:
>
> 如果equals方法认为相等，compareTo方法也应该返回0，它们在排序时处在相同的位置。
>
> 如果equals方法认为不相等，compareTo方法应该返回非0，它们在排序时必须处在不同的位置。
>
> 



##### Comparator自定义比较器排序

> 假如仅仅只是实现对象容器的自然排序，那么用匿名内部类或者**Lambda表达式**去使用带Comparator比较器的sort方法会比较好。
>
> 具体方法如下：
>
> ```java
> Arrays.sort(arr,Comparator)
> Collections.sort(collection,Comparator)
> ```
>
> Comparator接口中的**compare(Objetc o1,Object o2)**方法表示一种比较和排序的规则，并且这个规则可以在调用排序方法时灵活的传入，这样排序的规则和对象本身就隔离开了。相比较于Comparable接口实现的排序，显然这种方式要更加自由和灵活，实际开发中也会更推荐使用！
>
> **compare(Objetc o1,Object o2)**方法在表示对象大小和排序规则时，可以看成o1 - o2：
>
> 1. 方法返回负数，表示o1小于o2，排序时o1处在前列。
> 2. 方法返回正数，表示o1大于o2，排序时o2小，处在前列。
> 3. 方法返回0，表示o1等于o2，排序时按照原本的位置直接放在一起，不改变这两个对象之前的相对位置。
>
> 很明显，compare方法在表示排序规则时和compareTo方法一致，不再赘述。
>
> > **注意**❗
> >
> > Comparator接口中看起来有两个抽象方法compare和equals，但实际上只需要实现抽象方法compare就可以了，该接口仍然是一个功能接口。
> >
> > **这是因为任何类都继承Object，都可以把Object类的equals方法实现作为抽象方法equals的实现！**
> >
> > <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322171802351.png" alt="image-20230322171802351" style="zoom: 50%;" />



###### 举例

```java
package com.cskyan.javase.string._6comparator;

import org.junit.Test;
import sun.management.Agent;

import java.util.Arrays;
import java.util.Comparator;

/**
 * 基于java.util包下的功能接口Comparator实现的自然排序,更加灵活,是开发中更常用的方式
 * 其中的抽象方法:
 * int compare(T o1, T o2);
 * 是强制子类实现的
 *
 * compare方法就表示自然排序容器中两个对象比较大小的规则,这个规则可以看成o1 - o2:
 *      1.方法返回负数，表示o1小于o2，排序时o1处在前列。
 *      2.方法返回正数，表示o1大于o2，排序时o2小，处在前列。
 *      3.方法返回0，表示o1等于o2，排序时按照原本的位置直接放在一起，不改变这两个对象之前的相对位置。
 *
 * 为什么要使用Comparator接口呢?它的优势是什么呢?
 * 此时实现自然排序使用的方法是,带比较器的自然排序方法:
 * Arrays.sort(arr,Comparator)
 * Collections.sort(collection,Comparator)
 * 此时方法需要传入一个Comparator接口的实现类对象,这个实现类对象的传入,实际上是传入了一个比较的规则
 * 于是比较的规则本身就和类分开了,这样灵活性大大提升了
 *
 * @since 10:08
 * @author wuguidong@cskaoyan.onaliyun.com
 */
public class Demo {
    static Student[] stus = new Student[10];

    static {
        stus[0] = new Student(18, 500, "张三");
        stus[1] = new Student(28, 200, "张三丰");
        stus[2] = new Student(17, 400, "张四");
        stus[3] = new Student(8, 300, "易烊千玺");
        stus[4] = new Student(17, 300, "小黑子");
        stus[5] = new Student(17, 360, "李明");
        stus[6] = new Student(17, 379, "真");
        stus[7] = new Student(10, 370, "杨超越");
        stus[8] = new Student(19, 500, "雪豹");
        stus[9] = new Student(17, 600, "芝士雪豹吖");
    }

    // 方式一
    @Test
    public void test() {
        // 排序规则1: 按照名字的长度,从长到短排序
        for (Student s : stus) {
            System.out.println(s);
        }
        System.out.println("---------------------");
        Arrays.sort(stus, new SortRuler());
        for (Student s : stus) {
            System.out.println(s);
        }
    }


    // 方式二
    @Test
    public void test2() {
        // 排序规则2: 按照分数从低往高排序
        // 使用匿名内部类对象
        for (Student s : stus) {
            System.out.println(s);
        }
        System.out.println("---------------------");
        Arrays.sort(stus, new Comparator<Student>() {
            @Override
            public int compare(Student o1, Student o2) {
                return (int) (o1.score - o2.score);
            }
        });
        for (Student s : stus) {
            System.out.println(s);
        }
    }

    // 方式三
    @Test
    public void test3() {
        // 排序规则3: 按照年龄从大到小排序
        for (Student s : stus) {
            System.out.println(s);
        }
        Arrays.sort(stus, (s1, s2) -> s2.age - s1.age);
        System.out.println("----------------");
        for (Student s : stus) {
            System.out.println(s);
        }
    }

    // 方式四
    @Test
    public void test4() {
        // 排序规则4: 首先按照年龄从小到大排序,对于年龄一样的,按照名字的长度从短到长排序
        // 如果名字的长度也一样的,按照分数从高到低排序
        for (Student s : stus) {
            System.out.println(s);
        }
        System.out.println("---------------------");
        // Arrays.sort(stus, (s1, s2) -> compare(s1, s2));
        Arrays.sort(stus, Demo::compare);
        for (Student s : stus) {
            System.out.println(s);
        }
    }


    // 引用函数
    private static int compare(Student s1, Student s2) {
        if (s1.age != s2.age) {
            return s1.age - s2.age;
        }
        // age一样,比较名字长度
        if (s1.name.length() != s2.name.length()) {
            return s1.name.length() - s2.name.length();
        }
        // age和name长度都一样,比较分数
        return (int) (s2.score - s1.score);
    }
}

// 朴素的方式,手写实现类
class SortRuler implements Comparator<Student> {
    @Override
    public int compare(Student o1, Student o2) {
        // 排序规则1: 按照名字的长度,从长到短排序
        // 站在o1的角度,此时名字越长就越排在前面,说明对象越小,于是该方法就越要返回负数
        return o2.name.length() - o1.name.length();
    }
}

class Student {
    int age;
    double score;
    String name;

    public Student(int age, double score, String name) {
        this.age = age;
        this.score = score;
        this.name = name;
    }

    @Override
    public String toString() {
        return "Student{" +
                "age=" + age +
                ", score=" + score +
                ", name='" + name + '\'' +
                '}';
    }
}
```







##### 自然排序 Vs 比较器排序

> 稍微使用一下两种排序方式，不难发现：
>
> 1. Comparator自定义比较器排序，更加灵活，不需要考虑其它因素，仅考虑排序。在实际开发中，仅对容器做排序时，比较器会更常用。
> 2. 自然排序更多是为了配合整个集合体系**（Collection）**使用的，集合体系中很多方法的使用都需要这个类实现自然排序。使用自然排序，虽然前期需要精密的设计，但设计完毕后，使用就会很方便，相信大家后面学到集合就会有所体会了。

# Java文件处理

## File类

## IO流

> 理解**Java**的**IO**流
>
> 

### 字节流

### 字符流



### 其他流

#### 对象流（序列化和反序列化）

> 在前面，我们已经学过可以对Java基本数据类型的二进制数据进行操作的**数据流**，也学过可以将Java所有数据类型转换成一个字符串进行打印的**打印流**。
>
> 那么对于一个对象（引用数据类型的对象）的二进制数据难道不能进行直接操作吗？
>
> 答案当然是肯定，Java中也提供了相应的**对象流**来进行Java对象的二进制数据操作。当然我们普遍把这个操作的过程，称之为序列化和反序列化：
>
> 1. 序列化，将堆中的对象二进制数据，直接输出写入到外存中进行持久化保存。
> 2. 反序列化，将外存中对象的二进制数据，读取进JVM内存，在堆上新建这个对象。
>
> 注意事项：
>
> 1. **序列化和反序列化的目的是为了持久化保存和使用某个对象。**
> 2. **反序列化可以认为是一种新的、独特的创建对象的方式，但实际开发中不会频繁使用。**
>
> **对象流是本小节学习的重点。**

##### ObjectOutputStream

> java.io.ObjectOutputStream类是对象输出流，但普遍我们把它称呼为**序列化流**，因为它的作用就是完成序列化，就是将一个Java程序中对象二进制数据持久化保存到外存（文件）中。
>
> **它的继承关系是：**
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322174524766.png" alt="image-20230322174524766" style="zoom:67%;" />
>
> **它的构造方法如下：**
>
> ObjectOutputStream类构造方法
>
> | 构造方法                             | 解释说明                                          |
> | ------------------------------------ | ------------------------------------------------- |
> | ObjectOutputStream(OutputStream out) | 创建写入指定 OutputStream 的 ObjectOutputStream。 |
>
> **常用的成员方法如下：**
>
> | 返回值类型 | 成员方法                | 解释说明                                      |
> | ---------- | ----------------------- | --------------------------------------------- |
> | void       | writeObject(Object obj) | 将指定的对象写入 ObjectOutputStream序列化流。 |
>
> 上述内容看完后，你可能已经跃跃欲试想要开始进行对象的序列化操作了吧？但是不要着急，为了能够确定序列化的操作成功了，我们还需要学习一下反序列操作。



##### ObjectInputStream

> java.io.ObjectInputStream类是**反序化流**，可以对以前使用 ObjectOutputStream 写入的对象二进制数据进行反序列化还原一个对象。
>
> **它的继承关系如下图所示：**
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322174837856.png" alt="image-20230322174837856" style="zoom:50%;" />
>
> **它的构造方法如下：**
>
> ###### 
>
> 表 11. ObjectInputStream类构造方法
>
> | 构造方法                          | 解释说明                                          |
> | --------------------------------- | ------------------------------------------------- |
> | ObjectInputStream(InputStream in) | 创建从指定 InputStream 读取的 ObjectInputStream。 |
>
> **常用的成员方法如下：**
>
> ###### 
>
> 表 12. ObjectInputStream成员方法
>
> | 返回值类型 | 成员方法     | 解释说明                                |
> | ---------- | ------------ | --------------------------------------- |
> | Object     | readObject() | 从ObjectInputStream中读取还原一个对象。 |
>
> 以上学完后，完事具备，我们开始进行序列化和反序列化操作。

**序列化就是写到外存，反序列化就是重新写入内存**



##### 举例

> 首先定义一个Student类：
>
> ```java
> class Student{
>  private String name;
>  private int id;
>  private double score;
> 
>  @Override
>  public String toString() {
>      final StringBuffer sb = new StringBuffer("Student{");
>      sb.append("name='").append(name).append('\'');
>      sb.append(", id=").append(id);
>      sb.append(", score=").append(score);
>      sb.append('}');
>      return sb.toString();
>  }
> 
>  public Student(String name, int id, double score) {
>      this.name = name;
>      this.id = id;
>      this.score = score;
>  }
> 
>  public void study(){
>      System.out.println("as个优秀的学生,学习使我快乐!");
>  }
> }
> ```
>
> 若直接进行序列化操作，参考以下代码：
>
> ```java
> Student s = new Student("张三", 1, 100);
> // 创建序列化流对象
> ObjectOutputStream objOut = new ObjectOutputStream(new FileOutputStream("a.txt"));
> objOut.writeObject(s);
> // 关闭流
> objOut.close();
> ```
>
> 运行代码，抛出异常：java.io.**NotSerializableException**
>
> 这是因为：
>
> **某个类的对象若想进行序列化操作，必须实现接口java.io.Serializable，该接口是一个空接口，是一个标记接口。实现该接口的类意味着对象能够进行序列化/反序列化操作。这一点和之前clone方法的Cloneable接口是一致的。**
>
> 如：<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322185729802.png" alt="image-20230322185729802" style="zoom:50%;" />
>
> 让Student类实现空接口java.io.Serializable后，再以上执行序列化操作，操作成功了。思考一下，打开"a.txt"文件，能够看得懂吗？
>
> 当然是看不懂的，因为这是将一个对象的二进制数据写入一个文本文件。（某些数据是看得懂）
>
> 为了验证序列化的成功，需要进行反序列化，参考以下代码：
>
> ```java
> ObjectInputStream objIn = new ObjectInputStream(new FileInputStream("a.txt"));
> Object oSeria = objIn.readObject();
> Student sSeria = (Student) oSeria;
> sSeria.study();
> // 关闭流
> objIn.close();
> ```
>
> 很容易验证，这个对象又被还原了。以上就是一次完整的基于文件的序列化/反序列化的过程。
>
> 不要着急，还不算完。现在在上述序列化已完成的前提下，给Student类新增一个成员，然后仅进行反序列化操作（a.txt中已经存储了原有的序列化对象）
>
> ```java
> private String gender;
> ```
>
> 这时进行反序列化能够成功吗？
>
> 答案是否定的，运行代码，抛出异常**java.io.InvalidClassException**
>
> 这是因为：
>
> 反序列化在运行过程中，会验证一个序列化ID——serialVersionUID，如果序列化结果存储的ID和该类的ID不一致，就会运行错误，抛出异常InvalidClassException。
>
> 而一个类如果不显式的使用下列方式定义一个序列化ID：
>
> ```private static final long serialVersionUID = -9073063791266399291L;```
>
> 那么这个序列化ID就是通过"该类的各个方面进行计算得出的"，也就是说修改了这个类的源码都可能改变这个序列化ID。并且序列化ID的默认计算还要受编译器版本等外部运行环境的影响。
>
> **总之，我们在给一个类进行序列化操作之前，必须像上面一样显式定义序列化ID。**
>
> 于是，我们总结对一个类的对象做序列化操作的步骤：
>
> 1. 让该类实现空接口java.io.Serializable
>
> 2. 在该类中，显式的明确定义序列化ID。**（IDEA有自动生成功能，建议使用）**
>
>    [(91条消息) IntelliJ Idea -- 自动生成序列化 UUID_idea uuid_兮家小二的博客-CSDN博客](https://blog.csdn.net/qq_41463655/article/details/100022451)
>
>    **AIT + Enter** 生成uid

##### 其他注意事项

序列化和反序列化过程中的注意事项：

1.在绝大多数情况下,在做序列化操作时,直接将多个对象全部存入一个文件中,然后再按照顺序读出来,是没有问题的

但是在少部分场景下,这种操作会带来一定的风险

建议有这种需求时,存容器(数组,集合)对象,而不是直接存元素对象

2.被transient关键字修饰的成员变量,表示在序列化操作时,不能被持久化保存

在这种情况下,序列化一个对象,就不会保存该成员变量的取值

会直接保存它的默认值

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322190331799.png" alt="image-20230322190331799" style="zoom: 50%;" />



# Java多线程

### 面试题：什么是守护线程，有什么用？

## 一、代码实现多线程

### 1. 线程的创建和启动

#### 1.1 方式一：继承Thread类创建线程类

> **Thread是啥？**
>
> Java具有面向对象的语言特性，类似于IO流当中我们操作输入输出流时创建的相关对象，Java程序中操作线程也同样需要创建**”线程对象“**。
>
> 在Java的设计体系中，用**java.lang.Thread类**来描述一个Java程序中的线程，同时基于Thread类来实现Java多线程是一个最基本的、最简单的方式

> **基本步骤：**
>
> 1. 新建一个类A，让该类继承**java.lang.Thread类**。
> 2. 重写该类A继承自父类的**run方法**。
> 3. 创建该类A的对象**（注：直接使用Thread类的无参构造）**，调用**start方法**启动这个线程。







##### 面试问题：

1.能不能直接创建Thread对象来新建线程？

> 答：可以，但没必要。
>
> Java程序中，基于Thread类来表示一个线程有两种方式：
>
> 1. Thread类自身对象
> 2. Thread类的子类对象
>
> 但Thread类自身的run方法没有任何内容，这就意味着直接创建Thread对象，这个线程不能执行任何任务，这个线程是没有任何意义的。
>
> 可以看一下Thread源码里的run方法，啥都没干：
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322132150213.png" alt="image-20230322132150213" style="zoom:80%;" />
>
> ![image-20230322132132049](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322132132049.png)
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322132202501.png" alt="image-20230322132202501" style="zoom:67%;" />
>
> 

> **启动main方法时发生了什么？**
>
> ```java
> 演示代码：
> public class Demo {
> public static void main(String[] args) {
>   new ThreadA().start();
> }
> }
> class ThreadA extends Thread {
> @Override
> public void run() {
>   for (int i = 0; i < 60; i++) {
>       System.out.println(getName() + "这是第" + (i + 1) + "次说我喜欢你！");
>       try {
>           Thread.sleep(2000);
>       } catch (InterruptedException e) {
>           e.printStackTrace();
>       }
>   }
> }
> }
> ```
>
> 可以这样来描述上述代码的执行：
>
> 1. 启动main方法就是运行一个Java程序，也就是在操作系统中启动了一个**Java进程**。而Java程序是执行于JVM当中的，所以一个Java进程，实际上是一个**JVM的进程**。
> 2. main方法是程序的入口方法，main方法的执行代表了这个Java进程中的一条执行路径，也就是一个**线程**。我们一般称呼main方法执行的线程是**“主线程”**，其它线程为**“子线程”**。**main方法执行意味着主线程启动，主线程是一个Java进程执行中的一条主要路径。**
> 3. 在main方法中又开启了一个线程，这个线程是主线程当中新建的子线程。**子线程的开启意味着该Java进程中开辟了一条新的执行路径，这条新的执行路径和原先的主路径可以“并发执行”。**
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230322132753911.png" alt="image-20230322132753911" style="zoom:67%;" />
>
> **三个结论：**
>
> 1. 主线程和子线程并发执行，是两条相对独立的执行路径，互相不会阻塞。
> 2. **主线程执行完毕后，需要等待子线程执行完毕进程才会结束。**
> 3. 主线程当中可以启动多个子线程，子线程当中又可以继续启动子线程，它们的执行仍然符合上述规律。

#### 1.2 方式二：基于Runable接口新建一个线程



#### 1.3 方式三：基于Callable接口新建一个线程





## 2.❗线程的生命周期【面试点】



## 3.控制线程（API）

### 面试题：sleep()方法和yield()方法的区别

> 关于sleep()方法和yield()方法的区别如下。
>
> ➢ sleep()方法暂停当前线程后，会给其他线程执行机会，不会理会其他线程的优先
>
> 级；但yield()方法只会给优先级相同，或优先级更高的线程执行机会。
>
> ➢ **sleep()方法会将线程转入阻塞状态，直到经过阻塞时间才会转入就绪状态；而**
>
> **yield()不会将线程转入阻塞状态，它只是强制当前线程进入就绪状态。因此完全有**
>
> **可能某个线程被yield()方法暂停之后，立即再次获得处理器资源被执行。**
>
> ➢ sleep()方法声明抛出了InterruptedException异常，所以调用sleep()方法时要么捕捉
>
> 该异常，要么显式声明抛出该异常；而yield()方法则没有声明抛出任何异常。
>
> ➢ sleep()方法比yield()方法有更好的可移植性，通常不建议使用yield()方法来控制并发线程的执行。

## 多线程数据安全问题

### 面试题：StringBuffer vs StringBuilder

> StringBuffer vs StringBuilder
> * StringBuffer是线程的安全,它的所有成员方法都是用synchronized关键字修饰的同步方法,共用同一把锁this,任何方法执行的操作都是原子操作,保证了数据安全
> * 但是同步锁的使用,也会降低性能,所以StringBuffer仅推荐在多线程环境下使用,如果不是多线程,就不要使用
> * StringBuilder虽然不是线程安全的,但是单线程环境下,它的效率更高.但多线程环境下,请不要使用
> * 安全要比效率重要



## 线程间通信

### 面试题：

> 1.为什么wait,notify系列的方法不直接放在Thread类当中,而是要在放在Object类当中?
>
> **因为该系列方法需要锁对象来调用,而锁对象可以是任意对象,所以必须把这些方法放在Object类中**

> ❗2.wait() vs sleep()   [看起来都会让线程处在阻塞的状态,但它们的区别很明显]
>
> (比较重要的一个面试题)
>
> * 所属类的不同：
>
>   wait 是Object类的成员方法
>
>   sleep 是Thread类的静态成员方法
>   
>
> * 使用条件的不同：
>
>   **wait 必须在同步区域,使用锁对象来调用**
>
>   sleep 没有限制,想用就用
>   
>
> * 唤醒条件不同：
>
>   wait 必须用同一把锁对象,调用notify方法来唤醒
>
>   sleep 等到休眠时间结束了,就自动唤醒
>   
>
> * **休眠时的表现不同（最核心区别）**
>
>   wait 调用该方法,使得线程等待阻塞,并**立刻释放锁**
>
>   sleep 在休眠时,线程仍然要持有锁对象,**并不会释放锁对象**



## 多线程工具

### 线程池

#### 概念

> 系统启动一个新线程的成本是比较高的，因为它涉及与操作系统交互。在这种情形
>
> 下，使用线程池可以很好地提高性能，尤其是当程序中需要创建大量生存期很短暂的线程
>
> 时，更应该考虑使用线程池。
>
> 与数据库连接池类似的是，线程池在系统启动时即创建大量空闲的线程，程序将一个
>
> Runnable对象或Callable对象传给线程池，线程池就会启动一个空闲的线程来执行它们的
>
> run()或call()方法，当run()或call()方法执行结束后，该线程并不会死亡，而是再次返回线程池中成为空闲状态，等待执行下一个Runnable对象的run()或call()方法。
>
> 
>
> 除此之外，使用线程池可以有效地控制系统中并发线程的数量，当系统中包含大量并发线程时，会导致系统性能剧烈下降，甚至导致JVM崩溃，而线程池的最大线程数参数可以控制系统中并发线程数不超过此数。
>

#### 使用线程池管理线程

> ##### 步骤：
>
> ![image-20230323174156371](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230323174156371.png)
>
> ##### 

> 在JDK5以后，Java提供了线程池的实现，用以下两个类来描述：
>
> 1. **java.util.concurrent.Executors：**工具类，用于生成**线程池对象**。
> 2. **java.util.concurrent.ExecutorService：**一个接口，**是全体线程池类型的父类**，它用于指代线程池对象。
>
> 说明：
>
> **Executors**是一个工具类，用来产生线程池，而**ExecutorService**是所有线程池类型的父类，用来接收创建的线程池用的
>
> 如：
>
> ```java
> ExecutorService service = Executors.newCachedThreadPool();
> ```
>
> 

##### 1.1 创建线程池对象

> Executors工具类底下包含包含如下三个**静态**工厂方法来创建线程池：
>
> ```java
> // 特点:
> // 1.创建一个线程数量会自动扩容的线程池
> // 2.每当需要执行一个新任务时，有活跃的线程就使用该线程，否则就新建一条线程。
> // 3.使用完毕后的线程会回归线程池，如果这个线程在60秒之后依旧空闲，那么就会被移除
> ExecutorService newCachedThreadPool()
> 
> // 特点:
> // 1.线程数量固定为指定初始值
> // 2.维护一个无界队列（暂存已提交的来不及执行的任务）
> // 3.按照任务的提交顺序，将任务执行完毕  
> // 这种方式创建线程池是最常用的方式
> ExecutorService newFixedThreadPool(int nThreads)
> 
> // 特点:
> // 1.线程数量固定为1个
> // 2.维护了一个无界队列（暂存已提交的来不及执行的任务）
> // 3.按照任务的提交顺序，将任务执行完毕
> ExecutorService newSingleThreadExecutor()
> ```
>
> 使用以上方法就可以得到一个具有相应特点的线程池对象。
>
> 三个方法均返回一个**ExecutorService对象**，该对象代表一个线程池，它**可以执行Runnable对象或Callable对象所代表的线程**

##### 1.2 向线程池提交任务

> 光有一个线程池对象还不够，还需要向线程池提交任务，这个线程池才可以正常的执行多线程任务。
>
> ExecutorService代表尽快执行线程的线程池（只要线程池中有空闲线程，就立即执行线程任务），程序只要将一个Runnable对象或Callable对象（代表线程任务）提交给该线程池，该线程池就会尽快执行该任务。
>
> 向线程池提交方法主要依赖于接口**java.util.concurrent.ExecutorService**当中的两个submit方法：
>
> *  Future<?> submit(Runnable task)：将一个Runnable对象提交给指定的线程池，线程池将在有空闲线程时执行Runnable对象代表的任务。其中**Future对象代表Runnable任务的返回值**——但**run()方法没有返回值，所以Future对象将在run()方法执行结束后返回null**。但可以调用Future的isDone()、isCancelled()方法来获得Runnable对象的执行状态。
> * <T>Future<T>submit(Callable<T>task)：将一个Callable对象提交给指定的线程池，线程池将在有空闲线程时执行Callable对象代表的任务。其中Future代表Callable对象里call()方法的返回值。

###### **1.2.1 向线程池提交Runnable任务**

> ```java
> public class Demo {
>  public static void main(String[] args) {
>      //使用static ExecutorService newFixedThreadPool(int 个数)方法
>      //返回值是一个线程池对象es
>      //这个线程池对象里有2个线程
>      ExecutorService es = Executors.newFixedThreadPool(2);
> 
>      // 接下来调用线程池的方法：submit,需要一个Runnable类对象task
>      // 选择使用匿名对象
>      // 每调用一次submit方法，就会使用一个新的线程
>      es.submit(new ThreadPoolRunnable());
>      es.submit(new ThreadPoolRunnable());
>      // 如果超过了线程的数量，那么系统会等先执行的线程回到线程池中
>      // 然后再用这个回来的线程继续执行task任务
>      es.submit(new ThreadPoolRunnable());
>  }
> }
> 
> class ThreadPoolRunnable implements Runnable {
>  @Override
>  public void run() {
>      System.out.println(Thread.currentThread().getName() + "线程执行了一个任务!");
>  }
> }
> ```

###### 1.2.2 向线程池提交Callable任务

> ```java
> public class Demo2 {
>  public static void main(String[] args) {
>      // 创建线程池对象
>      ExecutorService pool = Executors.newCachedThreadPool();
>      // 向线程池提交任务
>      // submit(Callable task)
>      pool.submit(new MyCallableTask());
>  }
> }
> 
> class MyCallableTask implements Callable<String> {
>  @Override
>  public String call() throws Exception {
>      for (int i = 0; i < 10; i++) {
>          System.out.println(i);
>      }
>      return "哈哈哈哈";
>  }
> }
> ```
>
> 实现Callable接口，重写call方法实际上和实现Runnable接口，重写run方法是大差不差的一回事。其中的方法都是表示线程要执行的任务。



##### 1.3 Future 接口

> **java.util.concurrent.ExecutorService**当中的两个submit方法：
>
> ```java
> Future<?> submit(Runnable task)
> Future<T> submit(Callable<T> task)
> ```
>
> 它们都是有返回值的，返回值一个Future。
>
> Future接口用于表示线程执行完毕后结果，也就是线程执行任务后方法给出的返回值。所以很明显：
>
> 1. Runnable类型的任务没有返回值，获取Runnable类型任务执行完毕的结果，会得到一个null。所以Runnable类型的任务没必要处理返回值Future。
> 2. Callable类型的任务是有返回值的，获取就是call方法的返回值。
>
> 对于Callable类型的任务的call方法返回值，如何进行获取呢？依赖于Future下的一个成员方法：
>
> ```
> V get()  
> ```
>
> 该方法具有等待的特性，假如线程需要执行一段时间才能给出返回值，那么该方法就会一直等待线程给出返回值。
>
> 举例：
>
> ```java
> Future<?> result = threadPool.submit(new RunnableTask(10));
>         System.out.println(result.get());
> ```

##### 1.4 关闭线程池

> 线程池执行完毕任务后，整个程序并没有立刻终止，而是处在执行状态。
>
> 这是因为：
>
> **线程池会持续等待进行任务提交，除非关闭线程池。**
>
> 这里就提供两种关闭线程池的手段：
>
> ```java
> // 执行完任务列表中所有已提交的任务，关闭线程池，不再接受新任务。
> void shutdown()        
> // 如果任务已经提交到了线程池并且已经有线程在执行了,那就继续执行完这些任务,而那些只提交任务还未开始执行的任务,就不再执行了
> List<Runnable>shutdownNow()        
> ```
>
> 

### ❗❗面试题

**1.多线程有几种实现方案，分别是哪几种？**

> 三种。
>
> 第一种是直接创建继承Thread类的子类对象
>
> 另一种是创建实现Runnable接口的子类对象，然后通过new Thread(Runable) 来创建指定具体功能任务的线程。
>
> 第三种是创建实现Callable接口的子类对象，然后仍然通过new Thread(Runable)来创建指定具体功能任务的线程。
>
> 除了上述三种实现方案以后，Java还支持向线程池提交任务的方式实现多线程。

**2.基于Runnable接口和Callable接口实现的多线程，有啥区别？**

> 主要的区别在于Callable接口实现的任务有返回值，而Runnable没有返回值。
>
> 这个返回值可以通过Future接口下的get方法来获取。

**3.有几种方式实现线程同步，分别是什么？**

> 一共有三种方式。
>
> 第一种是同步代码块
>
> 第二种是静态/同步方法，同步方法和同步代码块本质上是一回事。
>
> 第三种是上锁，上Lock锁，基于Lock的实现类ReentrantLock来实现，一种更灵活的锁，可以通过API手动加锁、释放锁。

**4.启动一个线程是run()还是start()？它们的区别是什么？**

> start()启动线程
>
> 线程在主线程中调用start()方法启动线程，启动后JVM会自动让该线程调用run()方法。
>
> 而run()方法就是一共普通的成员方法，直接调用它就是调用了一共成员方法罢了。

**5.sleep()和wait()方法的区别**

> sleep()定义在Thread类中，是静态方法。
>
> 作用是让线程进入休眠阻塞状态，但不会释放锁。休眠时间到期后，会进入就绪状态抢夺时间片（CPU执行权）。
>
> wait()定义在Object类中，作用是让线程进入等待阻塞状态，且会立即释放锁资源。接下来就需要被notify()唤醒，才能退出等待状态，进入就绪状态开始抢夺时间片。

**6.为什么wait()、notify()、notifyAll()等方法都定义在Object类中而不是定义在Thread类中？**

> 因为调用这些方法的是锁对象，而锁对象可以是任意类型，所以定义在Object类中。





# Java网络编程

## Java的基本网络支持

> Java为网络支持提供了java.net包，该包下的URL和URLConnection等类提供了以编程
>
> 方式访问Web服务的功能，而URLDecoder和URLEncoder则提供了普通字符串和
>
> application/x-www-form-urlencoded MIME字符串相互转换的静态方法。

### 使用**InetAddress**

```java
// Java提供了InetAddress类来代表IP地址

        // InetAddress类还提供了一个getLocalHost()方法来获取本机IP地址对应的InetAddress实例
        System.out.println(InetAddress.getLocalHost());

        // String getHostName()：获取此IP地址的主机名
        System.out.println(InetAddress.getLocalHost().getHostName());

        // String getHostAddress()：返回该InetAddress实例对应的IP地址字符串（以字符串形式）。
        System.out.println(InetAddress.getLocalHost().getHostAddress());

```

InetAddress类本身并没有提供太多功能，它代表一个IP地址对象，是网络通信的基础。

### 

### 使用**URLDecoder**和**URLEncoder**

> URLDecoder和URLEncoder用于完成普通字符串和application/x-www-form-urlencodedMIME字符串之间的相互转换。可能有读者觉得后一个字符串非常专业，以为又是什么特别高深的知识，其实不是。
>
> 在介绍application/x-www-form-urlencoded MIME字符串之前，先使用www.google.com.hk搜索关键字“疯狂java”，将看到如图17.3所示的界面。
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230323221414478.png" alt="image-20230323221414478" style="zoom:50%;" />
>
> 图**17.3** 搜索关键字包含中文
>
> 从图17.3中可以看出，当关键字包含中文时，这些关键字就会变成如图17.3所示的“乱码”—实际上这不是乱码，这就是所谓的application/x-www-form-urlencoded MIME字符串。
>
> 当URL地址里包含非西欧字符的字符串时，系统会将这些非西欧字符串转换成如图17.3所示的特殊字符串。编程过程中可能涉及普通字符串和这种特殊字符串的相关转换，这就需要使用URLDecoder和URLEncoder类。
>
> ➢ **URLDecoder类**包含一个decode(String s, String enc)静态方法，它可以将看上去是乱码的特殊字符串转换成普通字符串。
>
> ➢ **URLEncoder类**包含一个encode(String s, String enc)静态方法，它可以将普通字符串转换成application/x-www-form-urlencoded MIME字符串。
>
> 下面程序示范了如何将图17.3所示地址栏中的“乱码”转换成普通字符串，并示范了如何将普通字符串转换成application/x-www-form-urlencoded MIME字符串。
>
> ![image-20230323232403762](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230323232403762.png)
>
> 

 

**URL**、**URLConnection**和**URLPermission**



## 基于**UDP**协议的网络编程

> UDP协议和TCP协议简单对比如下。
>
> ➢ TCP协议：可靠，传输大小无限制，但是需要连接建立时间，差错控制开销大。
>
> ➢ UDP协议：不可靠，差错控制开销较小，传输大小限制在64KB以下，不需要建立连接。

> UDP是一种面向无连接的协议，因此在通信时发送端和接收端不用建立连接。数据是以数据包的形式传输的。
>
> 我们把UDP网络编程理解成货运公司在两个码头间发送、接收货物一样，在传输的过程中首先需要创建两个“码头”，其次还需要用集装箱把货物装起来然后在进行传输。
>
> 上面句子的含义就是：
>
> 1. 需要创建接收端和发送端两个Socket（码头）
> 2. 需要将数据封装成数据包再进行传输（集装箱）

### DatagramPacket

> 发送和接收的数据也需要使用“集装箱”进行打包，为此Java提供了一个**java.net.DatagramPacket类**来充当这个集装箱的角色，用于封装UDP通信中发送或者接收的数据。
>
> 在创建发送端和接收端的DatagramPacket对象时，使用的构造方法有所不同：
>
> 1. 接收端的构造方法只需要接收一个字节数组来存放接收到的数据。
> 2. 发送端的构造方法不但要接收存放了发送数据的字节数组，还需要指定发送端IP地址和端口号。
>
> 接下来根据API文档的内容，对DatagramPacket的构造方法进行逐一详细地讲解。
>
> ```java
> // 构造 DatagramPacket，用来接收长度为length的包，在缓冲区中指定了偏移量。
> DatagramPacket(byte[] buf, int offset, int length) 
> // 构造 DatagramPacket，用来接收长度为length的数据包。
> DatagramPacket(byte[] buf, int length) 
> ```
>
> 使用该构造方法在创建DatagramPacket对象时，指定了封装数据的字节数组和数据的大小，没有指定IP地址和端口号。
>
> 很明显，这样的对象只能用于接收端，不能用于发送端。
>
> **因为发送端一定要明确指出数据的目的地(IP地址和端口号)，而接收端不需要明确知道数据的来源，只需要接收到数据即可。**
>
> **再来看一下发送端的数据包创建对象的方式：**
>
> ```java
> // 构造数据报包，用来将长度为length偏移量为offset的包发送到指定主机上的指定端口号。
> DatagramPacket(byte[] buf,  int offset, int length, InetAddress address, int port)        
> // 构造数据报包，用来将长度为length的包发送到指定主机上的指定端口号。
> DatagramPacket(byte[] buf, int length, InetAddress address, int port) 
> ```
>
> 使用该构造方法在创建DatagramPacket对象时，不仅指定了封装数据的字节数组和数据的大小，还指定了数据包的目标IP地址（addr）和端口号（port）。
>
> 在表示IP时，该构造器需要传入一个**java.net.InetAddress**对象，一般使用以下方法获取该对象：
>
> ```java
> // 获取一个表示本地主机的InetAddress对象
> InetAddress address = InetAddress.getLocalHost();
> // 获取一个指定ip地址的InetAddress对象
> InetAddress address2 = InetAddress.getByName("ip地址");
> ```
>
> **该对象用于发送端，因为在发送数据时必须指定接收端的IP地址和端口号，就好像发送货物的集装箱上面必须标明接收人的地址一样。**
>
> 上面讲解的是发送端和接收端创建各自数据包的形式，下面对DatagramPacket类中的常用方法做一下了解，即对数据包能够做以下操作：
>
> ```java
> // 返回数据缓冲区，即数据包封装的字节数据
> byte[] getData()
> // 返回将要发送或接收到的数据的长度。
> int getLength()         
> // 返回将要发送或接收到的数据的偏移量。
> int getOffset()        
>     
> // 获取数据包（要发送到的或者发送者）的IP地址
> //当程序准备发送此数据报时，该方法返回此数据报的目标机器的IP地址；当程序刚接收到一个数据报时，该方法返回该数据报的发送主机的IP地址。
> InetAddress getAddress() 
> // 获取数据包（要发送到的或者发送者）的端口号
> // 当程序准备发送此数据报时，该方法返回此数据报的目标机器的端口；当程序刚接收到一个数据报时，该方法返回该数据报的发送主机的端口。
> int getPort() 
> // 获取数据包（要发送到的或者发送者）的IP地址和端口号
> // 当程序准备发送此数据报时，该方法返回此数据报的目标SocketAddress；当程序刚接收到一个数据报时，该方法返回该数据报的发送主机的SocketAddress。
> SocketAddress getSocketAddress()
> ```
>
> > **关于SocketAddress类：**
> >
> > getSocketAddress()方法的返回值是一个~~SocketAddress对象~~（其实是InetSocketAddress类的对象），该对象实际上就是一个IP地址和一个端口号。也就是说，SocketAddress对象封装了一个InetAddress对象和一个代表端口的整数，所以使用SocketAddress对象可以同时代表IP地址和端口。
> >
> > `SocketAddress` 类，这个类代表一个套接字地址 (`socket address`)，一个套接字地址是由 IP 地址和端口号组成。 `SocketAddress` 是一个抽象类，而它的唯一子类就是 `InetSocketAddress` 类。  `InetSocketAddress` 其实是在 `InetAddress` 的基础上加了一个端口号。

### DatagramSocket

> ava.net.DatagramPacket对象数据包的作用就如同是“集装箱”，可以将发送端或者接收端的数据封装起来。
>
> **然而运输货物只有“集装箱”是不够的，还需要有码头。**
>
> 在程序中需要实现通信只有DatagramPacket数据包也同样不行，为此JDK中提供的一个**java.net.DatagramSocket类**。DatagramSocket类的作用就类似于码头，使用这个类的实例对象就可以发送和接收DatagramPacket数据包。
>
> 在创建发送端和接收端的DatagramSocket对象时，使用的构造方法也有所不同，下面对DatagramSocket类中常用的构造方法进行讲解。
>
> **构造函数**：
>
> ```java
> // ip:本机IP 端口：随机分配一个可用端口
> DatagramSocket()
> // ip:主机IP 端口：参数指定
> DatagramSocket(int port)
> // 指定IP和端口
> DatagramSocket(int port,InetAddress laddr)
> ```
>
> 这三个构造器，你能想明白它们创建的对象是接收端还是发送端的“码头”吗？
>
> **发送端的“集装箱”DatagramPacket构造器中指定了IP地址和端口号，所以发送端的“码头”可以不直接指出这两个参数（当然也可以指出），而接收端的“集装箱”DatagramPacket构造器中没有指定任何IP地址和端口号，所以接收端的“码头”必须指出这两个参数。**
>
> 于是：
>
> 1. **上述三个构造器都可以作为发送端的DatagramSocket创建对象。**
> 2. **只有DatagramSocket(int port)和DatagramSocket(int port,InetAddress laddr)能用于创建接收端的DatagramSocket对象。**接收端的DatagramSocket必须给出明确的IP地址和端口号，用于监听发送端的数据发送。

> **上面我们讲解了DatagramSocket的构造方法，接下来对DatagramSocket类中的常用方法进行详细地讲解。**
>
> 核心就是两个成员方法：
>
> ```java
> // 从此套接字接收数据报包。
> void  receive(DatagramPacket p)
> // 从此套接字发送数据报包。
> void  send(DatagramPacket p)        
> ```
>
> 







## 基于**TCP**协议的网络编程

> TCP/IP通信协议是一种可靠的网络协议，它在通信的两端各建立一个Socket，从而在通信的两端之间形成网络虚拟链路。一旦建立了虚拟的网络链路，两端的程序就可以通过虚拟链路进行通信。Java对基于TCP协议的网络通信提供了良好的封装，Java使用Socket对象来代表两端的通信端口，并通过Socket产生IO流来进行网络通信。

### TCP协议基础

> TCP协议要求传输的双方必须建立连接，所以TCP编程的实现要基于C/S架构，也就是常说的客户端（Client）/服务端（Server）结构。
>
> UDP是一种无连接的传输方式，所以UDP只有发送端和接收端，不区分客户端与服务端，计算机之间可以任意地发送数据。
>
> **但TCP通信是严格区分客户端与服务端的，在通信时，必须先由客户端去连接服务端才能实现通信，服务端不可以主动连接客户端，并且服务端程序需要事先启动，等待客户端的连接。**
>
> 在Java代码中，**java.net.Socket类**和**java.net.ServerSocket类**分别表示客户端和服务端的套接字，创建它们的对象就表示创建客户端套接字和服务端套接字。
>
> 通信时，首先创建代表服务端的ServerSocket对象，该对象相当于开启一个服务，并等待客户端的连接，然后创建代表客户端的Socket对象向服务端发出连接请求，服务端响应请求，两者建立连接开始通信。
>
> 最后仍然需要关闭资源，客户端一般用完就会关闭，服务端可酌情考虑是否关闭。
>
> > ❗看图17.4，**并没有看出TCP通信的两个通信实体之间有服务器端、客户端之分**，这是因为此图是两个通信实体已经建立虚拟链路之后的示意图。在两个通信实体没有建立虚拟链路之前，必须有一个通信实体先做出“主动姿态”，主动接收来自其他通信实体的连接请求。
> >
> > 【ZIUPAN】：可以理解成，一开始需要有ServerSocket作为服务器端来做出主动姿态接收信息，而当他们建立好了连接之后，其实就是**靠Socket在交流**了。
> >
> > **Java中能接收其他通信实体连接请求的类是ServerSocket，ServerSocket对象用于监听来自客户端的Socket连接，如果没有连接，它将一直处于等待状态。**ServerSocket包含一个监听来自客户端连接请求的方法(accept（）方法)。（见下方文字👇）

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230324134209134.png" alt="image-20230324134209134" style="zoom:50%;" />



### 使用**ServerSocket**创建**TCP**服务器端【有问题】

> 通过前面的描述我们知道，在TCP编程中，首先需要创建、启动服务端进程（套接字）。
>
> JDK的java.net包中提供了一个ServerSocket类，该类实例对象可以实现一个服务端的进程。
>
> **ServerSocket的构造器：**
>
> ```java
> // 创建绑定到特定端口的服务套接字。   
> ServerSocket(int port)    
> 【上面ServerSocket没有指定IP地址，则该ServerSocket将会绑定到本机默认的IP地址。程序中使用30000作为该ServerSocket的端口号，通常推荐使用1024以上的端口，主要是为了避免与其他应用程序的通用端口冲突。】
>    
> //在机器存在多个IP地址的情况下，允许通过localAddr参数来指定将ServerSocket绑定到指定的IP地址。
> ServerSocket(int port, int backlog, InetAddress localAddr)
> ```
>
> **使用该构造方法在创建ServerSocket对象时，就可以将其绑定到一个指定的端口号上，监听这个端口。（接下来客户端就向这个被监听的端口通信）**
>
> 接下来学习一下ServerSocket的常用方法:
>
> ```java
> // 侦听并接收接收来自客户端的请求
> Socket accept()        
> ```
>
> ServerSocket对象负责监听某台计算机的某个指定的端口号，在创建ServerSocket对象后，需要继续调用该对象的accept()方法，接收来自客户端的请求。
>
> 当执行了accept()方法之后，服务端程序会发生**阻塞**。**（accept方法也是一个阻塞方法）**
>
> 直到客户端发出连接请求，accept()方法才会**返回一个Scoket对象**（如果接收到来自客户端的请求时，accept()会返回一个Socket实例，称为clientSocket(类似于中介把客人介绍给前台小姐姐，由她负责之后的业务流程，中介继续去拉拢客人)，如果没有接收到请求，则一直处于阻塞等待状态。）用于和客户端实现通信，程序才能继续向下执行。
>
> **客户端和服务端进行数据交换，必须使用套接字对象Socket中获取的IO流，自身创建IO流对象是不可以用于数据交互的。从这个角度来说，Socket建立了服务端和客户端的传输通道。**

> 当ServerSocket使用完毕后，应使用ServerSocket的close()方法来关闭该ServerSocket。
>
> 在通常情况下，服务器不应该只接收一个客户端请求，而应该不断地接收来自客户端的所有请求，所以Java程序通常会通过循环不断地调用ServerSocket的accept()方法。代码片段如下：
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326100619926.png" alt="image-20230326100619926" style="zoom:67%;" />

### 使用**Socket**实现TCP客户端

> 讲解了ServerSocket对象可以实现服务端程序，但只实现服务端程序还不能完成通信，此时还需要一个客户端程序与之交互，为此JDK提供了一个**java.net.Socket类**，用于实现TCP客户端程序。
>
> **Socket的构造器如下：**
>
> ```java
> // 创建一个流套接字并将其连接到指定主机上的指定端口号。
> Socket(String host,int port)
> ```
>
> 使用该构造方法创建Socket对象时，会根据参数去**连接在指定地址和端口上运行的服务程序**，其中参数host接收的是一个字符串类型的IP地址。
>
> **❗：当客户端、服务器端产生了对应的Socket之后，就得到了如图17.4所示的通信示意图，程序无须再区分服务器端、客户端，而是通过各自的Socket进行通信。**
>
> 
>
> 接下来学习一下Socket的常用方法，如下表所示:
>
> | 返回值类型       | 方法名                 | 功能描述                                                     |
> | ---------------- | ---------------------- | ------------------------------------------------------------ |
> | void             | close()                | 关闭此套接字。关闭此套接字也将会关闭该套接字的 InputStream 和 OutputStream。 如果此套接字有一个与之关联的通道，则关闭该通道。 |
> | **InputStream**  | **getInputStream()**   | 该方法返回一个InputStream类型的输入流对象，如果该对象是由服务端的Socket返回，就用于读取客户端发送的数据，反之，用于读取服务端发送的数据 |
> | **OutputStream** | **getOutputStream()**  | 该方法返回一个OutputStream类型的输出流对象，如果该对象是由服务端的Socket返回，就用于向客户端发送数据，反之，用于向服务端发送数据 |
> | void             | shutdownOutput()       | 禁用此套接字的输出流。相当于关闭一半套接字的功能。           |
> | SocketAddress    | getRemoteSocketAddress | 返回此Socket和服务端连接时自身的IP地址和端口号，如果未连接则返回 null。 |
> | SocketAddress    | getLocalSocketAddress  | 返回此Socket绑定的服务端的IP地址和端口号，如果尚未绑定则返回 null。 |
>
> 在Socket类的常用方法中，**getInputStream()和getOutStream()方法分别用于获取输入流和输出流**。当客户端和服务端建立连接后，数据是以IO流的形式进行交互的，从而实现通信。**客户端和服务端进行数据交换，必须使用套接字对象Socket中获取的IO流，自身创建IO流对象是不可以用于数据交互的。从这个角度来说，Socket建立了服务端和客户端的传输通道。**



### 客户端思路

> 1. 创建客户端的Socket对象，并明确要连接的、服务端的IP地址和端口名。
> 2. 如果连接建立成功，就表明已经建立了数据传输的通道。就可以在该通道中，通过IO流进行数据的读取和写入。该通道称为Socket流，Socket流中既有输出流，也有输入流。
> 3. 通过Socket对象的成员方法，可以获取这两个流getInputStream和getOutputStream
> 4. 通过Socket流中的输入输出流实现数据在客服端——服务端之间的传输。
> 5. 关闭资源
>
> 思路是不难的，但是需要思考一个IO流方向和作用的问题：
>
> 对于客户端自身而言，Socket获取的输入、输出流分别是什么作用？
>
> 这时站在客户端的角度**（把客户端当成内存）**：
>
> 1. 输入流表示从服务端读数据
> 2. 输出流表示将数据写到服务端

### 服务端思路

> 1. 创建服务端的ServerSocket对象，需要指定一个监听的端口来监听是否有客户端进行连接。
> 2. 利用accept方法建立连接，得到Socke对象。
> 3. 服务端没有自己的流用于数据操作，而是从Socket流中获取输入、输出流。
> 4. 通过获取的输入、输出流读取数据或者写入数据
> 5. 酌情考虑是否关闭服务端。
>
> 同样的，对于服务端自身而言，Socket获取的输入、输出流分别是什么作用？
>
> 这时站在服务端的角度**（把服务端当成内存）**：
>
> 1. 输入流表示从客户端读数据
> 2. 输出流表示将数据写到客户端

### 练习

#### 1. v1客户端发送消息,服务端接收并打印

> **服务端**
>
> ```java
> public class Server {
> public static void main(String[] args) throws IOException {
>   // - 创建服务端的ServerSocket套接字对象
>   ServerSocket serverSocket = new ServerSocket(8888);
>   //- 利用accept方法建立连接, 得到客户端的Socket对象
>   Socket socket = serverSocket.accept();
>   //- 从Socket中获取输入输出流
>   // 这里是读取客户端发来的消息,所以是输入流
>   InputStream in = socket.getInputStream();
>   //- 利用输入输出流进行读写操作
>   byte[] bytes = new byte[1024];
>   int readCount = in.read(bytes);
>   String s = new String(bytes, 0, readCount);
> 
> 
>   // 获取连接服务端的客户端Socket的IP地址和端口号
>   SocketAddress remoteSocketAddress = socket.getRemoteSocketAddress();
>   int port = socket.getPort();
>   System.out.println("接收到了来自" + remoteSocketAddress + ":" + port + "消息 " + s);
>   //- close
>   socket.close();
>   serverSocket.close();
> }
> }
> ```
>
> **客户端**
>
> ```java
> public class Client {
> public static void main(String[] args) throws IOException {
>   // - 创建客户端Socket对象
>   Socket socket = new Socket("127.0.0.1", 8888);
>   //- 从Socket中获取输入输出流
>   // 这里是向服务端发送数据,所以是写数据,是输出流
>   OutputStream out = socket.getOutputStream();
>   //- 利用输入输出流进行读写操作
>   out.write("hello tcp".getBytes());
>   //- close
>   socket.close();
> }
> }
> ```
>
> 通过程序不难看出，**一旦使用ServerSocket、Socket建立网络连接之后，程序通过网络通信与普通IO并没有太大的区别**。

#### 2. v2单个客户端多次发送,服务端接收

> 首先客户端需要多次发送，必然有一个循环。服务端可以多次接收，也需要一个循环。可以直接写死循环，也可以像下列代码一样给出一个结束的条件。
>
> **客户端**
>
> ```java
> public class Client {
>  public static void main(String[] args) throws IOException {
>      // 先创建客户端Socket,尝试连接服务端
>      Socket socket = new Socket("127.0.0.1", 8888);
>      // 客户端先动键盘接收输入
>      Scanner sc = new Scanner(System.in);
>      String msg = "";
>      while (!(msg.equals("结束"))) {
>          msg = sc.nextLine();
>          // 获取Socket输出流,向服务端写数据
>          OutputStream out = socket.getOutputStream();
>          out.write(msg.getBytes());
>      }
>  }
> }
> ```
>
> **服务端**
>
> ```java
> public class Server {
>  public static void main(String[] args) throws IOException {
>      // 创建服务端套接字ServerSocket对象
>      ServerSocket serverSocket = new ServerSocket(8888);
>      // 通过accept方法和客户端建立连接,并获取客户端Socket对象
>      Socket socket = serverSocket.accept();
>      // 一直接收客户端消息
>      String msg = "";
>      while (!msg.equals("结束")) {
>          // 通过客户端Socket对象获取输入流,读客户端发来的消息
>          InputStream in = socket.getInputStream();
>          byte[] buf = new byte[1024];
>          int readCount = in.read(buf);
>          msg = new String(buf, 0, readCount);
>          System.out.println("来自" + socket.getRemoteSocketAddress() + "的客户端,发来消息:" + msg);
>      }
>  }
> }
> ```
>
> 



#### 3. v3多个客户端多次发送,服务端接收(多线程处理)

> TCP编程下，服务端和客户端必须建立连接才能通信，而在单线程环境下，ServerSocket的accept方法作为阻塞方法，显然一次只能接收一个客户端进行连接。如果想要实现多台客户端同时连接一个服务端，显然是需要多线程来完成需求的。
>
> **思路也很简单，只需要服务端进程起多个线程处理多台客户端连接就好了，也就是说这时的服务端要变成多线程的，一个线程处理一个客户端连接。**
>
> 
>
> **客户端**
>
> ```java
> public class Client {
>  public static void main(String[] args) throws IOException {
>      // 先创建客户端Socket,尝试连接服务端
>      Socket socket = new Socket("127.0.0.1", 9999);
>      // 客户端先动键盘接收输入
>      Scanner sc = new Scanner(System.in);
>      String msg = "";
>      while (true) {
>          msg = sc.nextLine();
>          // 获取Socket输出流,向服务端写数据
>          OutputStream out = socket.getOutputStream();
>          out.write(msg.getBytes());
>      }
>  }
> }
> ```
>
> **客户端可以启动多个。**
>
> **服务端**：
>
> ```java
> public class Server {
>  public static void main(String[] args) throws IOException {
>      // 创建服务端ServerSocket对象
>      ServerSocket serverSocket = new ServerSocket(9999);
>      // 此处需要处理不确定个数的客户端连接,而且客户端连接可能短暂通信一下立刻就中断了,完美符合线程池的应用场景
>      ExecutorService pool = Executors.newFixedThreadPool(2);
>      while (true) {
>          Socket socket = serverSocket.accept();
>          pool.submit(new ConnectTask(socket));
>      }
>  }
> }
> ```
>
> **连接任务**：
>
> ```java
> public class ConnectTask implements Runnable {
>  private Socket socket;
> 
>  public ConnectTask(Socket socket) {
>      this.socket = socket;
>  }
> 
> 
>  @Override
>  public void run() {
>      while (true) {
>          try {
>              InputStream in = socket.getInputStream();
>              byte[] bytes = new byte[1024];
>              int readCount = in.read(bytes);
>              String msg = new String(bytes, 0, readCount);
>              System.out.println("来自" + socket.getRemoteSocketAddress() + "的客户端,发来消息:" + msg);
>              // }
>          } catch (IOException e) {
>              e.printStackTrace();
>              System.out.println(socket.getRemoteSocketAddress() + "的客户端,已断开连接!");
>              return;
>          }
>      }
>  }
> }
> ```
>
> 

#### 4. 客户端发送信息，服务端接收后返回信息

> 客户端：
>
> ```java
> package javaSE.day25;
> 
> import com.sun.corba.se.impl.orbutil.CorbaResourceUtil;
> 
> import java.io.*;
> import java.net.Socket;
> import java.util.Scanner;
> 
> public class LoginClient {
>     public static void main(String[] args) throws IOException, InterruptedException {
> 
>         // 输入账户和密码
>         Scanner scanner = new Scanner(System.in);
>         System.out.println("请输入用户名：");
>         String username = scanner.nextLine();
> 
>         System.out.println("请输入密码：");
>         String password = scanner.nextLine();
> 
>         // new 一个User对象
>         User user = new User(username, password);
> 
>         Socket socket = new Socket("127.0.0.1", 8878);
>         OutputStream outputStream = socket.getOutputStream();
>         ObjectOutputStream objectOutputStream = new ObjectOutputStream(outputStream);
> 
>         // 把user对象传给服务端
>         objectOutputStream.writeObject(user);
> 
>         // 此时不能关闭Socket,也不能关闭socket当中的输入流,因为它们都有用,于是可以考虑关闭输出流
>         // 输出流一关闭,就不能再向服务端发消息了,此时服务端的read方法就知道,客户端发送消息结束了!!
>         // 关闭socket的输出流,表示已经不再向服务端发送消息了,服务端的read方法可以放心结束read阻塞,继续执行代码
>         socket.shutdownOutput();
> 
>         // 向服务端发送完数据后,等待服务端的响应,也就是使用socket当中的字节输入流
>         InputStream socketIn = socket.getInputStream();
>         InputStreamReader inputStreamReader = new InputStreamReader(socketIn);
>         int readCount = 0;
>         byte[] buf = new byte[1024];
>         System.out.println("返回信息：");
> //        int read = socketIn.read(buf);
> //        System.out.println(new String(buf, 0, read));
>         while ((readCount = socketIn.read(buf))!=-1)
>         {
>             System.out.println(new String(buf, 0, readCount));
>         }
>     }
> }
> 
> ```
>
> 
>
> 服务端：
>
> ```java
> package javaSE.day25;
> 
> import java.io.*;
> import java.net.ServerSocket;
> import java.net.Socket;
> 
> public class LoginServer {
>     public static void main(String[] args) throws IOException, ClassNotFoundException {
>         ServerSocket serverSocket = new ServerSocket(8878);
>         // 利用accept方法建立连接, 得到客户端的Socket对象
>         Socket sockt = serverSocket.accept();
>         System.out.println("客户端已经连接了!");
>         InputStream inputStream = sockt.getInputStream();
>         // 使用包装流读取对象
>         ObjectInputStream in = new ObjectInputStream(inputStream);
>         Object o = in.readObject();
> 
>         // 强转
>         User user = (User)o;
>         OutputStream outputStream = sockt.getOutputStream();
>         OutputStreamWriter outputStreamWriter = new OutputStreamWriter(outputStream);
> 
>         // 判断
>         if (user.username.equals("admin") && user.password.equals("admin")){
> //            outputStream.write("登录成功".getBytes());
>             outputStreamWriter.write("登陆成功");
> //            outputStream.flush();
>           ❗  outputStreamWriter.flush();
>             System.out.println("登陆成功");
>             sockt.shutdownOutput();
>         }
>         else {
>             System.out.println("登陆失败");
>             outputStream.write("登录失败".getBytes());
>             sockt.shutdownOutput();
>         }
>         // 关闭
>         sockt.close();
>         serverSocket.close();
>     }
> }
> 
> ```
>
> ❗为什么写入网络数据时，要调用`flush()`方法。
>
> 如果不调用`flush()`，我们很可能会发现，客户端和服务器都收不到数据，这并不是Java标准库的设计问题，而是我们以流的形式写入数据的时候，并不是一写入就立刻发送到网络，而是先写入内存缓冲区，直到缓冲区满了以后，才会一次性真正发送到网络，这样设计的目的是为了提高传输效率。如果缓冲区的数据很少，而我们又想强制把这些数据发送到网络，就必须调用`flush()`强制把缓冲区数据发送出去。

# **Java注解反射**

## 反射

> 反射是Java高级特性中最为重要的知识点之一，因为它是学习Java框架最重要的前置知识点。
>
> 如果大家记忆力不错的话，我们早在讲解Object类的API时，就曾提到：**反射实际上就是Class类的API应用**。所以从语法上学习反射是不难的，大家不要有学习的压力。
>
> 在反射这个章节，我们核心的知识点主要有：
>
> 1. **类加载机制**（详细探究一下类加载的原理和过程）
> 2. **反射的使用**（Class类API的使用）
> 3. **反射的应用**（一些具体案例）

### 类加载机制

> 首先在这里，我们给出一个明确的类加载的定义：
>
> **Java虚拟机把描述类的数据从.class文件加载到内存，并对数据进行校验、转换解析和初始化，最终形成可以被虚拟机直接使用的Java类型，这个过程被称作虚拟机的类加载机制。**

> 关于Class类：
>
> ![image-20230326170316929](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326170316929.png)

#### 类加载的过程

> 当程序要使用某个类时，如果该类还未被加载到内存中，则JVM会对该类进行**类加载**操作，也叫**类初始化**。
>
> 一个类从被加载到JVM内存中开始，到卸载出内存为止，**一个类的生命周期**包括：
>
> ![image-20230325001829091](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230325001829091.png)
>
> 其中前面的加载、连接（链接）、初始化步骤合起来都是类加载的过程。
>
> 具体的每个步骤都在执行什么操作呢？
>
> 1. 加载：通过**类加载器(ClassLoader)**去加载**字节码文件**，将class文件数据读取进JVM内存(实际上就是IO流的形式读文件)。
>
>    **在加载的过程中，还有一件非常重要的事情就是在堆上创建封装了该类类型信息的Class对象**。
>
>    **也就是说，当程序中使用任何类时，系统都会为之建立一个java.lang.Class对象！**
>
> 2. 连接，连接阶段负责把类的二进制数据合并到JRE中
>
>    类连接又可以分为以下三个小步骤：
>
>    1. **验证**，主要目的是为了确保class文件的字节流中包含的信息符合当前JVM的要求，不会影响JVM的安全。/检验被加载的类是否有正确的内部结构，并和其他类协调一致。
>
>       【ZIUPAN：因为自己也完全可以新建一个.class格式的文件，如果JVM不检查.class文件中的内容就直接加载的话很容易出问题】
>
>       
>
>    2. **准备**，主要目的是为类的静态成员变量分配内存，进行静态成员变量的默认初始化，设置初始值。
>
>       
>
>    3. **解析**，主要目的是将**类的二进制数据中的**符号引用（就是一个普通的常量）替换为直接引用（真实的内存地址）。
>
>       
>
> 3. **初始化**是类加载的最后一个步骤。主要目的是执行和static相关的内容，包括：
>
>    > 执行静态成员变量的显式赋值。
>    >
>    > 执行静态代码块。
>    >
>    > 
>    >
>    > ❗JVM会按这些语句在程序中的排列顺序依次执行它们
>
>    > ❗❗❗对于一个final型的类变量，如果该类变量的值在编译时就可以确定下来，那么这个类变量相当于“**宏变量**”。**Java编译器会在编译时直接把这个类变量出现的地方替换成它的值，因此即使程序使用该静态类变量，也不会导致该类的初始化**。例如下面示例程序的结果。
>    >
>    > ```java
>    > public class FinalQuestion {
>    >     public static void main(String[] args) {
>    >         System.out.println(MyTest.Constant);
>    >     }
>    > 
>    > }
>    > 
>    > class MyTest{
>    >     static
>    >     {
>    >         System.out.println("静态初始化块");
>    >     }
>    >     static final String Constant = "ZIUPAN";
>    > }
>    > 
>    > 输出结果只有ZIUPAN，而没有输出“静态初始化块”
>    > ```
>    >
>    > 上面程序的MyTest类中有一个compileConstant的类变量，该类变量使用了final修饰，而且它的值可以在编译时确定下来，因此compileConstant会被当成“宏变量”处理。程序中所有使用compileConstant的地方都会在编译时被直接替换成它的值——也就是说，上面程序中①号粗体字代码在编译时就会被替换成“ZIUPAN”，所以该代码不会导致初始化MyTest类。
>    >
>    > ![image-20230326172032905](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326172032905.png)





#### 类加载的时机

> 类加载是懒加载，**在Java中把一定触发类加载的代码场景称之为“类加载的时机”**，也就是**类初始化的时机**。意为遇到这些情况，就必须对该类执行初始化的操作。
>
> 目前我们已经学过的类加载的时机有：
>
> 1. 直接使用**java**命令来运行某个主类，也就是启动某个类的main()方法，会先加载这个类。
> 2. 创建类的对象。(首次)
> 3. 访问类的静态成员（首次）
> 4. 触发某个子类的类加载，会优先类加载父类。
>
> 以及我们今天马上就要学习的：反射触发类加载。
>
> **在Java当中，使用反射方式来强制创建某个类或接口对应的java.lang.Class对象，会触发该类的类加载。**

#### 类加载器

> **类加载器（ClassLoader）**负责将.class文件加载到内存中，并为之生成对应类型的Class对象。从分类上来说，Java当中的类加载器由以下三种组成：
>
> 1. Bootstrap ClassLoader 根类加载器
> 2. Extension ClassLoader 扩展类加载器
> 3. System  ClassLoader  系统类加载器
>
> **Bootstrap ClassLoader 根类加载器**，也被称为引导类加载器，负责**Java核心类**的加载，比如Object、String、System等类都需要用该类加载器进行类加载。在JDK中JRE的lib目录下rt.jar文件中的所有类都使用根类加载器进行加载。
>
> **Extension ClassLoader 扩展类加载器**，负责JRE的扩展目录中jar包的加载，也就是JDK那些非核心代码的加载。在JDK中JRE的lib目录下ext目录下的所有jar包都是用扩展类加载器加载。
>
> **Sysetm ClassLoader 系统类加载器（应用类加载器）**，负责在JVM启动时加载来自java命令的class文件，也就是用来加载**自定义类**。
>
> ❗❗**Java类加载器除了根类加载器之外，其他类加载器都是使用Java语言编写的**，所以程序员完全可以开发自己的类加载器，通过使用自定义类加载器，可以完成一些特定的功能。
>
> 类加载器对于目前阶段而言，仅了解就够了，无需再深入挖掘了。





### Java代码的三个执行阶段

> 对于一个Java代码文件而言，当它处于java文件以及class文件的状态时，就把这个状态称之为**“Source源代码阶段”**。
>
> 待到经过类加载器类加载这个类，会把该类的字节码数据读取进内存，在堆上生成一个封装该类类型信息的Class对象。这个Class对象当中，就存储了该类的类型信息，如何存储呢？
>
> 用Field类来描述类中成员变量，用Constructor类来描述类中构造器，用Method类来描述类中成员方法....总之Java万物皆对象。这个阶段，我们称之为**”Class类对象阶段“**。
>
> 当然最终这个类会被new对象，这时就是Java代码的第三个阶段了——**Runtime阶段**。
>
> 这个阶段转换的过程可以参考下图：
>
> 图 2. Java代码的三个执行过程-示意图
>
> ![Java代码的三个执行过程-示意图](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202211021109867.png?align=center&padding=true)
>
> 
>
> 当然为什么要了解这些东西呢？主要是为了后续课程做铺垫。



### 反射

> 首先，第一个问题：什么是反射？反射是一种什么样的技术？
>
> JAVA反射技术是在**运行状态中：**
>
> 1. 对于任意一个类，都能够知道这个类的所有属性和方法（包括私有）
> 2. 对于任意一个对象，都能够调用它的任意一个方法，访问任意一个属性。
>
> 这种动态获取的信息以及动态调用对象的方法的功能称为Java语言的反射机制。
>
> **总之，反射是提供获取运行时类信息的一种技术，或者更通俗一点反射技术就是操作一个类的Class对象。**
>
> 自然，反射技术应用的起点就是获取某个类的Class对象。



#### 获取Class对象

> 获取Class对象是使用反射技术的起点，Class类的实例表示正在运行的Java应用程序的类和接口。
>
> 目前我们一共有三种方式可以用来获取Class对象：
>
> 1. 依赖于Object类的成员方法——getClass方法。
>
>    **该方法必须先创建这个类型的对象,然后才能获取Class对象**
>
>    该方法限制比较大,一般很少使用(可能就是想在不创建该类型的对象的前提下获取class对象)
>
>    
>
> 2. 通过**类名/接口名.class**获取到该类型对象（任意数据类型都具备一个class静态属性获取Class对象）
>
>    
>
> 3. 通过Class类的静态方法（**forName(String clazzName)方法**）：
>
>    ```java
>      Class<?> forName(String className)
>    ```
>
>    **该方法需要传入字符串参数，该字符串参数的值是某个类的全限定类名（必须添加完整包名）。**
>
> 
>
> 上述三种获取Class对象的方式：
>
> 1. 无论哪种方式获取Class对象，只要是同种类型，Class对象必然是唯一的。（因为类加载只有一次）
> 2. 第三种方式是最常用的方式，因为它直接用一个全限定类名字符串指定一个类，更加灵活。尤其是在配合配置文件使用的时候，它的优越性秒杀其它方式。
>
> ❗：
>
> 注意事项:
>
> 1. 无论是何种方式获取Class对象,都不是创建Class对象
>
>    **Class对象都是在类加载过程中的加载阶段由JVM在堆上创建**
>
> 2. 同一种类型的Class对象是唯一的(因为类加载只有一次)，而不同类型的Class对象是不同的
>
> 3. 推荐使用方式三来获取Class对象,它使用起来更加灵活,是最常用的方式
>
> 4. 任意数据类型都具备一个class静态属性获取Class对象
>
>    *      基本数据类型也有Class对象
>
>    *      也就是可以这样写"int.class,double.class"等
>
>    *      但这种写法基本都是为了配合反射中的方法使用的(后面再讲)
>
>
> 5. (了解)
>
>         方式二和方式三触发的类加载是不同的
>
>    方式二触发的类加载不完整,不进行类初始化
>
>    方式三触发完整的类加载
>
> 举例：
>
> ```java
> public class Demo {
>     public static void main(String[] args) throws ClassNotFoundException {
>        Student s = new Student();
>         Class studentClazz = s.getClass();
> 
>         Class studentClazz2 = Student.class;
> 
>         Class studentClazz3 = Class.forName("com.cskaoyan.javase.reflect._1basic.Student");
> 
>         System.out.println(studentClazz == studentClazz2);
>         System.out.println(studentClazz == studentClazz3);
>         System.out.println(studentClazz2 == studentClazz3);
> 
>         // Class teacherClazz = Class.forName("com.cskaoyan.javase.reflect._1basic.Teacher");
>         // false
>         // System.out.println(teacherClazz == studentClazz);
> 
>         // 该种方式不会触发类初始化,是一次不完整的类加载
>         Class teacherClazz = Teacher.class;
>     }
> }
> 
> class Student {
> 
> }
> 
> class Teacher {
>     static {
>         System.out.println("Teacher类执行了类加载的初始化步骤!");
>     }
> }
> 
> 输出结果：
> true
> true
> true
> 
> ```
>
> 

#### 通过反射获得Class对象并从Class对象中获取信息（反射API）

> Class对象可以获得该类里的方法（由Method对象表示）、构造器（由Constructor对象表示）、成员变量（由Field对象表示），这三个类都位于java.lang.reflect包下，并实现了java.lang.reflect.Member接口。程序可以通过Method对象来执行对应的方法，通过Constructor对象来调用对应的构造器创建实例，能通过Field对象直接访问并修改对象的成员变量值。
>
> Class对象封装了类型信息，把类中的成员（构造方法、成员方法、成员变量）都封装成了对应的类进行表示。获取Class对象就可以获取这些类中成员，从而实现各种操作。
>
> 其中：
>
> 1. Class对象的类型信息中**java.lang.reflect.Constructor类**用于描述构造器，且包含和构造器相关的一些操作。
> 2. Class对象的类型信息中**java.lang.reflect.Field类**用于描述成员变量，且包含和成员变量相关的一些操作。
> 3. Class对象的类型信息中**java.lang.reflect.Method类**用于描述成员方法，且包含和成员方法相关的一些操作。
>
> 这三个类都有一个共同的特点是：**都继承了类java.lang.reflect.AccessibleObject。**
>
> 这个类，作为一个父类，给Constructor、Field、Method三个类提供了一个重要成员方法：
>
> ```java
> void setAccessible(boolean flag)
> ```
>
> 当该方法的参数设为true，表示反射在使用（调用方法）对象的过程可以突破Java语言的访问权限检查。**说人话就是该方法参数设置为true后， 即便访问权限是私有，也可以随意访问。**
>
> 这个方法就提供了一种暴力破解权限的手段，但终究破坏了封装性，不是常规手段，不建议使用，仅了解。
>
> 下面我们就来学习一下这些API。

##### 获取构造器(Constructor)

> Class对象的类型信息中**java.lang.reflect.Constructor类**用于描述构造器，且包含和构造器相关的一些操作。
>
> 以下和Constructor相关的方法都是Class类API：
>
> **获取多个Constructor:**
>
> ```java
> // 获取所有的public修饰的构造方法
> Constructor[] getConstructors()
> // 获取所有的构造方法(包含私有的)
> Constructor[] getDeclaredConstructors()
> ```
>
> **获取指定Constructor:**
>
> ```java
> // 获取public修饰的, 指定参数类型所对应的构造方法
> Constructor<T> getConstructor(Class<?>... parameterTypes)
> // 获取指定参数类型所对应的构造方法(包含私有的)
> Constructor<T> getDeclaredConstructor(Class<?>... parameterTypes)
> ```
>
> 注：获取指定类型构造器时，需要给出对应构造器形参数据类型的Class对象，一般直接用"数据类型.class"的形式。基本数据类型也可以使用这种形式。如果是无参构造器，保持空着也是可以的。
>
> 构造器最常用的功能就是**new对象过程中赋值**了，所以Constructor类下提供了一个成员方法实现这一功能：
>
> ```java
> // 传入相应参数，在创建对象过程中赋值，返回值是一个相应对象
> T newInstance(Object... initargs)   
> ```
>
> 注：newInstance的参数可以自由给定，可以有参可以无参。
>
> 参考代码如下：
>
> ```java
> public class Demo {
> public static void main(String[] args) throws ClassNotFoundException, NoSuchMethodException, IllegalAccessException, InvocationTargetException, InstantiationException {
>   // 反射技术的起点
>   // 获取字节码文件对象
>   // 获取所有的构造方法
>   Class<?> personCls = Class.forName("com.cskaoyan.reflect.Person");
>   System.out.println("获取所有的public构造方法--------");
>   // Constructor[] getConstructors()
>   Constructor<?>[] constructors = personCls.getConstructors();
>   for (Constructor constructor : constructors) {
>       System.out.println(constructor);
>   }
> 
>   System.out.println("获取所有的构造方法--------");
>   //Constructor[] getDeclaredConstructors()
>   Constructor<?>[] declaredConstructors = personCls.getDeclaredConstructors();
>   for (Constructor constructor : declaredConstructors) {
>       System.out.println(constructor);
>   }
>   System.out.println("获取指定的public构造方法--------");
> 
>   // Constructor<T> getConstructor(Class<?>... parameterTypes)
>   Constructor<?> constructor = personCls.getConstructor(int.class, String.class);
>   System.out.println(constructor);
>   System.out.println("获取指定的构造方法--------");
> 
>   //Constructor<T> getDeclaredConstructor(Class<?>... parameterTypes)
>   Constructor<?> declaredConstructor = personCls.getDeclaredConstructor(String.class);
>   System.out.println(declaredConstructor);
> 
>   // 利用构造方法对象 实例化对象  newInstance
>   Constructor<?> c1 = personCls.getDeclaredConstructor();
>   System.out.println(c1.newInstance());
> 
>   // 暴力破解方式
>   // 忽略java语法检查 setAccessible(true)
>   declaredConstructor.setAccessible(true);
>   Object o1 = declaredConstructor.newInstance("张三");
>   System.out.println(o1);
> 
>   // 自己试一下：
>   Constructor<?> declaredConstructor1 = personCls.getDeclaredConstructor(int.class, String.class, String.class);
>   Object o = declaredConstructor1.newInstance(18, "ZIUPAN", "男");
>   System.out.println(o);
> }
> }
> ```
>
> person类：
>
> ```java
> public class Person {
> private int age;
> public String name;
> String gender;
> 
> Person() {
> }
> 
> private Person(String name) {
>   this.name = name;
> }
> 
> public Person(int age, String name) {
>   this.age = age;
>   this.name = name;
> }
> 
> public Person(int age, String name, String gender) {
>   this.age = age;
>   this.name = name;
>   this.gender = gender;
> }
> 
> public void eat() {
>   System.out.println("我今天就想吃一个佛跳墙！");
> }
> 
> private void eat(String food) {
>   System.out.println("我今天就想吃一个" + food);
> }
> 
> @Override
> public String toString() {
>   final StringBuffer sb = new StringBuffer("Person{");
>   sb.append("age=").append(age);
>   sb.append(", name='").append(name).append('\'');
>   sb.append(", gender='").append(gender).append('\'');
>   sb.append('}');
>   return sb.toString();
> }
> }
> ```
>
> 输出结果：
>
> ```java
> 获取所有的public构造方法--------
> public javaSE.reflect.Person(int,java.lang.String,java.lang.String)
> public javaSE.reflect.Person(int,java.lang.String)
> 获取所有的构造方法--------
> public javaSE.reflect.Person(int,java.lang.String,java.lang.String)
> public javaSE.reflect.Person(int,java.lang.String)
> private javaSE.reflect.Person(java.lang.String)
> javaSE.reflect.Person()
> 获取指定的public构造方法--------
> public javaSE.reflect.Person(int,java.lang.String)
> 获取指定的构造方法--------
> private javaSE.reflect.Person(java.lang.String)
> Person{age=0, name='null', gender='null'}
> Person{age=0, name='张三', gender='null'}
> Person{age=18, name='ZIUPAN', gender='男'}
> ```
>
> ##### ❗：
>
> > ![image-20230326225725133](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326225725133.png)
> >
> > <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326230006996.png" alt="image-20230326230006996" style="zoom: 50%;" />
> >
> > 另外可以看一下stage8的例子，也差不多
> >
> > 提示：
> >
> > 这种使用配置文件来配置对象，然后由程序根据配置文件来创建对象的方式非常有用，大名鼎鼎的Spring框架就采用这种方式大大简化了Java EE应用的开发。当然，Spring采用的是XML配置文件——毕竟属性文件能配置的信息太有限了，而XML配置文件能配置的信息就丰富多了
> >
> > 其他方法：→Java疯狂讲义P1341

##### 获取成员变量（Field）

> Class对象的类型信息中**java.lang.reflect.Field类**用于描述成员变量，且包含和成员变量相关的一些操作。
>
> 上面一个学完后，这个就是比着葫芦画葫芦了，直接看：
>
> **获取所有Field**
>
> ```java
> // 获取所有public成员变量，包括父类的公共成员变量
> Field[] getFields()
> // 获取本类所有的成员变量（含private），不包含父类的成员变量
> Field[] getDeclaredFields()
> ```
>
> **获取指定成员变量**
>
> ```java
> // 通过成员变量名获取指定的public变量，包含父类的public成员变量
> Field getField(String name)
> // 通过成员变量名获取本类中指定的变量（含private）同样不包含父类
> Field getDeclaredField(String name)
> ```
>
> Field类提供了和成员变量相关的操作，最常见的就是读和写了，也就是下面两个方法：
>
> 通过Field读写对象的成员变量
>
> ```java
> // 在指定对象obj中，将此 Field 对象表示的成员变量设置为指定的新值
> public void set(Object obj, Object value)
> // 返回指定对象obj中，此 Field 对象表示的成员变量的值
> public Object get(Object obj)
> ```
>
> 同样是基于上面的Person类，先获取获取Class对象，再获取构造方法，然后通过构造方法，创建对象，最后再操作成员变量。
>
> ```java
> // 获取所有public成员变量
>         System.out.println("获取所有public成员变量");
>         Field[] fields = personCls.getFields();
>         for (Field field : fields) {
>             System.out.println(field);
>         }
> 
>         System.out.println("--------------------------");
> 
>         // 获取所有的成员变量
>         System.out.println("获取所有的成员变量");
>         Field[] declaredFields = personCls.getDeclaredFields();
>         for (Field declaredField : declaredFields) {
>             System.out.println(declaredField);
>         }
> 
>         System.out.println("--------------------------");
> 
>         // 获取指定的的成员变量
>         System.out.println("获取指定的的成员变量");
>         Field name = personCls.getField("name");
>         System.out.println(name);
>         Field age = personCls.getDeclaredField("age");
>         System.out.println(age);
> 
>         System.out.println("--------------------------");
> 
>         //void set(Object obj, Object value)：赋值，传入对象
>         // 获取构造方法
>         Constructor<?> declaredConstructor2 = personCls.getDeclaredConstructor();
>         Object o2 = declaredConstructor2.newInstance();
>         name.set(o2, "长风");
>         System.out.println(o2);
>         // Object get(Object obj)：获取值，传入对象
>         Object o3 = name.get(o2);
>         System.out.println(o3);
>     }
> ```
>
> 输出结果：
>
> ```java
> 获取所有public成员变量
> public java.lang.String javaSE.reflect.Person.name
> --------------------------
> 获取所有的成员变量
> private int javaSE.reflect.Person.age
> public java.lang.String javaSE.reflect.Person.name
> java.lang.String javaSE.reflect.Person.gender
> --------------------------
> 获取指定的的成员变量
> public java.lang.String javaSE.reflect.Person.name
> private int javaSE.reflect.Person.age
> --------------------------
> Person{age=0, name='长风', gender='null'}
> 长风
> ```

##### 获取成员方法(Method)

> Class对象的类型信息中**java.lang.reflect.Method类**用于描述成员方法，且包含和成员方法相关的一些操作。
>
> 看到这里，套路已经固定了，直接看API：
>
> 获取所有Method:
>
> ```java
> // 所有公共方法，包括本类和父类，乃至于Object类中的方法。
> Method[] getMethods()
> // 获取本类中的所有方法，包括private方法，不包括父类
> Method[] getDeclaredMethods()
> ```
>
> 获取指定的Method:
>
> ```java
> // 获取指定的公共方法，包括父类。若无参数就不需要写参数类型，或者写null
> Method getMethod(String name, Class<?>... parameterTypes)
> // 获取本类中指定的任意方法（包括private），不包括父类
> Method getDeclaredMethod(String name, Class<?>... parameterTypes)
> ```
>
> Method表示方法，最重要的操作就是调用这个方法了。Method当中提供了成员方法**invoke调用方法**：
>
> ```java
> Object invoke(Object obj, Object... args)
>     注：该方法表示用obj对象来调用Method表示的成员方法，args是传入方法的 实参，无参方法可以为空。
> ```
>
> 示例：
>
> ```java
> public class Demo5 {
>  public static void main(String[] args) throws ClassNotFoundException, NoSuchMethodException, IllegalAccessException, InvocationTargetException, InstantiationException {
>      // 获取字节码文件对象
>      Class<?> personCls = Class.forName("com.cskaoyan.reflect.Person");
> 
>      // 获取所有的public的成员方法
>      System.out.println("获取所有的public的成员方法");
>      // Method[] getMethods() 会获取到父类的public的方法
>      Method[] methods = personCls.getMethods();
>      for (Method method : methods) {
>          System.out.println(method);
>      }
> 
>      System.out.println("获取所有的成员方法");
> 
>      //Method[] getDeclaredMethods()
>      Method[] declaredMethods = personCls.getDeclaredMethods();
>      for (Method method : declaredMethods) {
>          System.out.println(method);
>      }
>      System.out.println("获取指定的public的成员方法");
> 
>      // Method getMethod(String name, Class<?>... parameterTypes)
>      Method eatMethod1 = personCls.getMethod("eat");
>      System.out.println(eatMethod1);
>      //Method getDeclaredMethod(String name, Class<?>... parameterTypes)
>      System.out.println("获取指定的成员方法");
> 
>      Method eatMethod2 = personCls.getDeclaredMethod("eat", String.class);
>      System.out.println(eatMethod2);
> 
>      // 对象.方法名()
>      // 调用方法
>      // Object invoke(Object obj, Object... args)
>      // 获取构造方法
>      Constructor<?> declaredConstructor = personCls.getDeclaredConstructor();
>      // 创建对象
>      Object o = declaredConstructor.newInstance();
>      eatMethod1.invoke(o);
>      // 忽略java语法检查
>      eatMethod2.setAccessible(true);
>      eatMethod2.invoke(o, "apple");
>  }
> }
> ```

##### 获取Class对应类上所包含的Annotation

如下几个方法用于访问Class对应类上所包含的Annotation【其他的查阅文档】

> *  getAnnotation(Class<A> annotationClass)：
>
>   尝试获取**该Class对象对应类上存在的、指定类型的Annotation**；如果该类型的注解不存在，则返回null
>
> * getDeclaredAnnotation(Class<A> annotationClass)：
>
>   这是Java 8新增的方法，该方法尝试获取**直接修饰**该Class对象对应类的、指定类型的Annotation；如果该类型的注解不存在，则返回null。
>
> * getDeclaredAnnotations()：
>
>   返回直接修饰该Class对应类的所有Annotation。
>
> 如下：
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326222109675.png" alt="image-20230326222109675" style="zoom:50%;" />



#### 反射应用举例

下面浅谈一下一些应用到反射的场景。

##### 1. 父类引用指向子类对象时欲访问子类成员

> ![image-20230326214216634](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326214216634.png)
>
> > ❗❗如下图，父类引用是无法访问到独属于子类的方法和变量滴
> >
> > **主线程：**
> >
> > <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326214849311.png" alt="image-20230326214849311" style="zoom: 50%;" />
> >
> > **Test类：**
> >
> > <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230326214912686.png" alt="image-20230326214912686" style="zoom:50%;" />

##### 父类中私有成员被子类隐式继承

> 小标题中的结论，我们早就知道了，用反射很容易就能够验证这一点。参考以下代码：
>
> ```java
> ```
>
> 

##### ORM框架(了解)



#### 配置文件(.properties文件)

> 我们这里说的配置文件指的是以“.properties”作为后缀名的一种文件类型。
>
> 你可以用两种方式来新建一个这种类型的文件：
>
> 1. 直接写文件的名字就是“xxx.properties”
> 2. 在IDEA当中也可以按下列方式创建：
>
> 
>
> 图 3. IDEA创建properties配置文件
>
> <img src="https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202302032311323.png?align=center&padding=true" alt="IDEA创建properties配置文件" style="zoom: 67%;" />
>
> 
>
> 这个所谓的配置文件有什么用呢？
>
> 在实际开发种配置文件比如.properties、.xml、.yml等文件。一般用于放配置信息  比如数据库配置信息  比如第三方的服务信息等。
>
> 那这个配置文件怎么用呢？
>
>  JDK中提供了**java.util.Properties类**来表示描述以及操作properties配置文件。properties作为配置文件时，是一种属性键值对的集合，属性的每个键与值都是一个字符串。
>
> 具体来说，properties文件应该按照下列格式去书写：
>
> > ip=127.0.0.1
> >
> > port=8888
> >
> > StudentClassName=com.cskaoyan.javase.Student
>
> **注："="可以作为键值对的连接符，还可以使用":"，但是推荐使用"="。配置文件中也可以写注释，用"#"开头就可以了。**
>
> 把properties配置文件写好后，就可以创建Properties对象，然后通过成员方法来操作这个文件。
>
> 常用构造器就直接无参创建对象就行了。
>
> 常用成员方法：
>
> ```java
> // 从输入流中读取属性列表（键和元素对）。
> void  load(InputStream inStream)        
> // 按简单的面向行的格式从输入字符流中读取属性列表（键和元素对）。
> void  load(Reader reader)       
> // 用指定的键在此属性列表中搜索属性。
> String  getProperty(String key)        
> ```
>
> 如果properties文件就按照上述写法，我们就可以写出以下代码从配置文件中获取信息：
>
> ```java
> public static void main(String[] args) throws IOException {
>     // 第一步：创建Properties对象
>     Properties properties = new Properties();
> 
>     // 第二步：load加载这个配置文件,实际上就是IO流读这个文件
>     // 从属性文件（以输入流表示）中加载key-value对，把加载到的key-value对追加到Properties里
>     properties.load(new FileInputStream("config.properties"));
> 
>     // 第三步：getProperty获取属性值
>     String host = properties.getProperty("ip");
>     String username = properties.getProperty("port");
>     String studentClazzName = properties.getProperty("StudentClassName");
>     System.out.println(host);
>     System.out.println(username);
>     System.out.println(studentClazzName);
> }
> ```
>
> 配合配置文件，Class.forName获取Class对象的灵活性和优越性就非常强大了。到了实际开发中，这种方式也非常常用。
>
> **一个小问题：如果配置文件中有中文，发现取出来的属性键值对乱码咋办？**
>
> 用字符流读就可以了。
>
> 上课例子：
>
> ```java
> package com.cskaoyan.javase.reflect._2properties;
> 
> import java.io.*;
> import java.util.Properties;
> 
> /**
>  * 我们这里说的配置文件指的是以“.properties”作为后缀名的一种文件类型。
>  * 在开发中常见的配置文件有".properties, .yml, .xml"等
>  * 配置文件
>  * 一般用于放配置信息,比如数据库配置信息,比如第三方的服务信息等。
>  * 这些文件中存放了配置信息,那么怎么读出来呢?怎么读到内存中呢?
>  * properties配置文件,配合相应的API,就可以实现配置信息的快捷读取,很方便.
>  *
>  *  JDK中提供了java.util.Properties类来表示描述以及操作properties配置文件。
>  *  properties作为配置文件时，是一种属性键值对的集合，属性的每个键与值都是一个字符串,而且一一对应.
>  *  properties配置文件的书写语法:
>  * 具体来说，properties文件应该按照下列格式去书写：
>  * ip=127.0.0.1
>  * port=8888
>  * StudentClassName=com.cskaoyan.javase.Student
>  * 注："="可以作为键值对的连接符，还可以使用":"，但是推荐使用"="。配置文件中也可以写注释，用"#"开头就可以了。
>  * 配置文件中尽量不要加空格,除非本身就有空格.
>  *
>  * @since 17:29
>  * @author wuguidong@cskaoyan.onaliyun.com
>  */
> public class Demo {
>     public static void main(String[] args) throws IOException {
>         // 创建Properties对象，然后通过成员方法来操作这个文件。
>         // 常用构造器就直接无参创建对象就行了。
>         Properties properties = new Properties();
> 
>         // 常用成员方法
>         // 从字节输入流中读取属性列表（键和元素对）配置文件
>         // 如果配置文件中存在中文,就一定要用字符流,用字节流可能乱码(当然一般来说,配置文件比较少存在中文)
>         // void  load(InputStream inStream)
>         // properties.load(new FileInputStream("a.properties"));
> 
> 
>         // 按简单的面向行的格式从输入字符流中读取属性列表（键和元素对）配置文件
>         // void  load(Reader reader)
>         properties.load(new BufferedReader(new FileReader("a.properties")));
> 
>         // 用指定的键在此属性列表中搜索属性。通过key获取value
>         // String  getProperty(String key)
>         String ip = properties.getProperty("ip");
>         String port = properties.getProperty("port");
>         String studentName = properties.getProperty("studentName");
>         String best = properties.getProperty("best");
> 
>         System.out.println(ip);
>         System.out.println(port);
>         System.out.println(studentName);
> 
>         System.out.println(best);
> 
>     }
> }
> 
> ```
>
> 



#### 

## 注解

> 注解（annotation），在之前的课程中虽然并未详细讲解它，但我们早就使用过它了。比如：
>
> 1. 表示子类重写父类方法的注解：@Override
> 2. 表示Junit单元测试方法的注解：@Test
> 3. 表示过时的类、方法等结构的注解：@Deprecated
> 4. ...

### 注解 VS 注释

> 首先，我们还是来辨析两个概念（虽然之前大概提过）：注解（annotation）和注释（comment）
>
> 注释的作用很简单：注释传递了代码之外的额外信息，是给程序员理解代码看的，不参与编译。注释的语法有固定形式，但内容并没有任何规定，几乎可以直接写在代码的任何位置。
>
> 注解有和注释相似的地方，注解可以理解成代码的一个特殊标签，这些标签也会传递一些代码外的额外信息。但这些标记和额外信息可以在代码编译、类加载、运行时被读取，并执行相应的处理。
>
> 注解和注解相同的地方在于：
>
> **它们都传递了代码外的额外信息。**
>
> 但它们的区别更多：
>
> 1. **注解可以参与编译，但注释显然不可能。**
> 2. **注解有确定的使用范围和使用方式，注释虽然也有语法，但基本想咋写就咋写。**
> 3. **注解是Java引用数据类型的一种，它和class、interface、enum具有同等地位。**

### 注解的定义

> 注解，其实是代码里的特殊标记，这些标记可以在编译、类加载、运行时被读取，并执行相应的处理。通过使用注解，程序开发人员可以在不改变原有逻辑的情况下，在源文件中嵌入一些补充的信息。代码分析工具、开发工具和部署工具可以通过这些补充信息进行验证或者进行部署。
>
> 注解提供了一种为程序元素设置元数据的方法，从某些方面来看，注解就像修饰符一样，可用于修饰包、类、构造器、方法、成员变量、参数、局部变量的声明，这些信息被存储在注解的“name=value”对中

> 注解也属于Java的一种引用数据类型，它在定义时和接口很相似，如下：
>
> ```java
> 访问权限修饰符 @interface 注解名{
>   // 注解体
>   属性类型 属性名();
>   属性类型 属性名();
>   属性类型 属性名();
>   .....
> }
> 
> 如：
>     @interface AnnotationA {
>     // 这里虽然很像接口中定义抽象方法,但实际并不是,这里只是注解体中的注解属性
>     int num();
> 
>     String str();
> 
>     Class clazz();
> 
>     int[] arr();
> }
> ```
>
> 解释：
>
> 1. 注解的访问权限修饰符和class、interface等是一样的。
> 2. 注解名也遵循大驼峰的命名原则。
> 3. 注解中的属性能够定义的类型范围如下：
>    1. 基本数据类型
>    2. java.lang.String
>    3. java.lang.Class
>    4. 枚举enum
>    5. 注解
>    6. 以及上述类型的数组
>
> **注解和接口的关系：**
>
> 注解的定义和接口使用同一个关键字interface，而且注解体的定义也非常类似于接口中的抽象方法。这当然不是巧合，而是因为注解本身就是一种特殊的接口，可以查看**java.lang.Annotation接口**的JDK文档，原文是：
>
> > 所有 Annotation 类型都要扩展的公共接口。注意，手动扩展该公共接口的接口不会定义为 Annotation 类型。还要注意此接口本身不是定义 Annotation 类型。 
>
> **但即便注解类型有上述的特点，在定义注解时，也不能继承其他的注解或接口。**

### 元注解

> 元注解的概念来源于元数据，什么是元数据呢？
>
> 图 1. 元数据的概念
>
> ![元数据的概念](https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202302060451614.png?align=center&padding=true)
>
> 图中框起来的一列数据是什么意思呢？表头的学校就负责解释这一列数据，所以这一列数据都代表某个学生的学校信息。
>
> **像“学校”这样的，用于解释数据的数据，就是元数据。**
>
> 那什么是元注解呢？
>
> **解释和描述注解的注解就是元注解。**
>
> 元注解是解释注解的注解，所以元注解普遍都直接用来修饰注解，写在一个注解的定义语法头上。比如下图：
>
> 图 2. 注解@Override的定义
>
> <img src="https://hixiaodong123.oss-cn-hangzhou.aliyuncs.com/typora/202302060455846.png?align=center&padding=true" alt="注解@Override的定义" style="zoom:50%;" />
>
> 那么元注解的具体含义是什么呢？两个最常见的元注解如下：
>
> **@Retention元注解，作用是定义注解的保留级别，也就是注解的存活范围。分为以下三个级别：**
>
> 1. RetentionPolicy.RUNTIME：表示该注解会由JVM保留，因此运行时环境可以使用它，这样的一个注解才有可能影响代码执行。
> 2. RetentionPolicy.CLASS：表示该注解在编译时由编译器保留，会进入class文件，但在类加载时期会被JVM忽略，不会进入虚拟机，不影响代码执行。**一个注解如果没有显式用元注解@Retention声明保留级别，那么它默认的保留级别就是RetentionPolicy.CLASS。**
> 3. RetentionPolicy.SOURCE：表示该注解仅保留在.java源文件级别中，会被编译器忽略掉。（类似于注释）
>
> **@Target元注解，作用是定义注解可以修饰的目标，如果一个注解没有用该注解标明可修饰的目标，那么就表示该注解可以修饰任意结构，没有限制。**
>
> 该注解的常见取值如下：
>
> 1. 整个类    ElementType.**TYPE**
> 2. 成员变量   ElementType.FIELD
> 3. 构造方法   ElementType.CONSTRUCTOR
> 4. 成员方法   ElementType.METHOD

### 注解的使用（重点）

> 以往我们使用一个类，往往需要创建它的对象。而注解的使用，也有相似的概念，也必须实例化一个注解。
>
> 注解进行实例化使用的方式和语法也很简单，参考如下形式：
>
> ```java
> @注解名(给注解各个属性赋值)
> ```
>
> 注：
>
> 1. "@"可以认为相当于“new”关键字，必不可少。
> 2. 注解相当于给Java代码打上一个标签，所以它必须要修饰Java代码的一个结构。比如修饰一整个类，一整个方法，一个成员变量等等。
> 3. 实例化注解时，必须给注解的各个属性赋值，赋值方式是：属性名 = 属性值。如果是数组类型的注解属性，用"{}"赋值。
> 4. 定义注解属性时也可以通过关键字default设定该属性的默认值，这样在实例化注解时就不需要给定取值了。当然即便有默认值的注解属性，也仍然可以赋值，覆盖默认值。
> 5. 如果注解体当中的注解属性只有1个，并且它就叫value的话，这时可以进行简化赋值。简化赋值可以直接给定值，无需写"属性名 = "了。而如果value属性再上给定default默认值，那么就可以直接不赋值，直接使用一个注解了。
> 6. 如果注解属性是一个引用数据类型，那么不能等于null，也不能new赋值。
>
> 给出一个注解类型使用的代码参考案例：
>
> ```java
> public class Dmeo {
>     public static void main(String[] args) {
>     }
> 
>     @MyAnno4("admin")
>     @MyAnno3(names = {"zs","ls","ww"})
>     @MyAnno2()
>     @MyAnno(name = "zs",age = 20)
>     public static void func() {
>     }
> }
> 
> @interface MyAnno{
>     // 注解体
>     String name();
>     int age();
> }
> 
> @interface MyAnno2{
>     // 设置默认值
>     String role() default "teacher";
> }
> 
> @interface MyAnno3{
>     String[] names();
> }
> 
> @interface MyAnno4{
>     String value();
> }
> ```
>
> 注解的使用看起来是不难的，但这样用到底能起到什么作用呢？这就涉及到注解的作用了：
>
> 注解只是起到一个标签的作用，给代码增加了额外的信息。至于额外的信息能够起到什么作用，这就不是注解本身所能够掌控的了，这时需要注解处理器来完成这个操作。

### 注解处理器

> 注解处理器的意义在于获取注解所描述的额外信息，然后根据这些额外信息进行处理。注解处理器本身可以是一段Java代码，也可以其它的程序。比如IDEA在很多时候就扮演了注解处理器的角色。
>
> **注解和反射之所以要一起讲，是因为注解处理器最常见的实现方式就是——反射。**
>
> **先通过反射获取注解信息，然后针对注解类型，获取注解当中定义的属性**，一个参考代码案例如下：
>
> ```java
> public class Demo {
> public static void main(String[] args) throws Exception {
>   // 获取字节码文件对象
>   Class<?> c = Class.forName("com.cskaoyan.annotation.Demo2");
>   // 获取方法对象
>   Method loginMethod = c.getDeclaredMethod("login");
>   // 判读是否使用了注解
>   /*
>      Class类的成员方法
>      boolean isAnnotationPresent(Class<? extends Annotation> annotationClass)
>      如果指定类型的注释存在于此元素上，则返回 true，否则返回 false
>       */
>   boolean annotationPresent = loginMethod.isAnnotationPresent(Login.class);
>   if (annotationPresent) {
>       // 获取注解实例
>       Login annotation = loginMethod.getAnnotation(Login.class);
>       // 获取属性值
>       String name = annotation.name();
>       String password = annotation.password();
>       System.out.println(name);
>       System.out.println(password);
>   } else {
>       System.out.println("没有使用注解");
>   }
> }
> @Login()
> public static void login() {
> }
> }
> 
> //使用元注解修饰
> @Retention(RetentionPolicy.RUNTIME)
> @Target(ElementType.METHOD)
> @interface Login {
> // 注解体
> String name() default "root";
> 
> 
> String password() default "123456";
> }
> ```
>

### 利用注解+反射来动态创建对象(注解处理器)

> 基本的语法搞明白后，那么我们就结合注解和反射，实现以下注解处理器案例：
>
> ❗❗❗❗❗❗❗❗❗❗❗❗
>
> > 先定义一个Person类，类中有两个成员变量age和name。
> >
> > 然后再定义2个注解，用于修饰成员变量name和age，其中：
> >
> > 1. @AgeLimit  用于限定成员变量age必须处在1-150之间。
> > 2. @NameLimit  用于限定成员变量name的字符串长度不超过4。
> >
> > 然后定义注解处理器，使得不满足条件的Person对象无法创建。
>
> 注解本身的定义非常简单**（要注意使用元注解，设定保留级别和作用位置）**：
>
> 
>
> *注解处理器案例-注解的定义：*
>
> ```java
> @Target(ElementType.FIELD)
> @Retention(RetentionPolicy.RUNTIME)
> @interface AgeLimit {
>     int max() default 150;
>     int min() default 1;
> }
> 
> @Target(ElementType.FIELD)
> @Retention(RetentionPolicy.RUNTIME)
> @interface NameLimit {
>     int value() default 4;
> }
> ```
>
> *Person类：*
>
> ```java
> class Person {
>     @AgeLimit
>     private int age;
>     @NameLimit
>     private String name;
> 
>     // 1.私有化构造器,避免外界直接new对象.外界直接new对象,是没办法控制属性的赋值的
>     private Person(int age, String name) {
>         this.age = age;
>         this.name = name;
>     }
> 
>     @Override
>     public String toString() {
>         final StringBuilder sb = new StringBuilder("Person{");
>         sb.append("age=").append(age);
>         sb.append(", name='").append(name).append('\'');
>         sb.append('}');
>         return sb.toString();
>     }
> }
> ```
>
> 最后注解处理器要实现以下功能：
>
> 1. 给外界创建、制造Person对象（反射创建对象）
> 2. 不符合成员变量取值条件的Person对象，禁止创建，可以抛出异常。
>
> 该注解处理器实际上是一个工厂的设计模式。参考代码如下：
>
> ```java
> public class Test {
>     public static void main(String[] args) throws NoSuchMethodException, IllegalAccessException, NoSuchFieldException, InstantiationException, InvocationTargetException, ClassNotFoundException {
>         System.out.println(PersonInstanceFactory.createPerson(18, "张三"));
>         // System.out.println(PersonInstanceFactory.createPerson(500, "张三丰"));
>         System.out.println(PersonInstanceFactory.createPerson(18, "丁辽是班上学得最好的同学!"));
>     }
> }
> 
> // 2.Person自身不能再new对象,所以可以在外部创建一个"工厂"专门用来生产"Person对象"
> class PersonInstanceFactory {
>     public static Person createPerson(int age, String name) throws ClassNotFoundException, NoSuchFieldException, NoSuchMethodException, IllegalAccessException, InvocationTargetException, InstantiationException {
>         // 3.在工厂内部可以通过反射获取注解的额外信息,然后通过反射创建对象时,就可以给出限制
>         // 获取Person类的Class对象
>         Class<?> personClazz = Class.forName("com.cskaoyan.javase.annotation._3handle.demo2.Person");
>         // 分别获取两个成员变量的Field对象
>         Field ageField = personClazz.getDeclaredField("age");
>         Field nameField = personClazz.getDeclaredField("name");
>         // 分别获取两个Field对象当中的注解信息
>         // 年龄的最大值和最小值
>         int ageMax = 0;
>         int ageMin = 0;
>         if (ageField.isAnnotationPresent(AgeLimit.class)) {
>             AgeLimit ageAnno = ageField.getAnnotation(AgeLimit.class);
>             ageMax = ageAnno.max();
>             ageMin = ageAnno.min();
>         }
>         int nameLen = 0;
>         if (nameField.isAnnotationPresent(NameLimit.class)) {
>             NameLimit nameAnno = nameField.getAnnotation(NameLimit.class);
>             nameLen = nameAnno.maxLen();
>         }
> 
>         // 接下来判断参数是否合法
>         if (age > ageMax || age < ageMin) {
>             // 不合法
>             throw new IllegalArgumentException("传入的age参数不合法!请重新输入!");
>         }
>         if (name.length() > nameLen) {
>             // 不合法
>             throw new IllegalArgumentException("传入的name参数不合法!请重新输入!");
>         }
>         System.out.println("您传入的参数都是合法的,很棒,我帮你创建这个对象!");
>         // 合法就反射创建对象
>         Constructor<?> cons = personClazz.getDeclaredConstructor(int.class, String.class);
>         // 破解私有权限
>         cons.setAccessible(true);
>         // 创建对象
>         return (Person) cons.newInstance(age, name);
>     }
> }
> ```
>
> 以上就是注解搭配反射使用的一个经典注解处理器案例。



# 泛型

## 泛型概述

> 所谓泛型, 就是**参数化类型**, 当我们在写代码时候, 如果最开始不确定某个代码在逻辑设计的时候, 是什么类型;  我们可以选择假定一种类型来代指, 当我们真正使用的时候再指明具体的类型.
>
> Java中的泛型是在JDK1.5时候出现.  

> **泛型的好处**：
> a. 提高了程序的安全性
> b. 将运行期遇到的问题转移到了编译期
> c. 省去了类型强转的麻烦(省去了我们来做类型强转, **实际底层jvm做了类型强转**)

## 泛型的使用

### 泛型类（重要）

> // 所谓泛型类, 就是把泛型定义在类上.
> // 在类型之后使用<>定义泛型
> 格式:  class 类名  <泛型类型1,…>
>
> 举例：
>
> ```java
> // class User <XXXX>  假定了一种叫 XXXX类型 , 注意是假定的
> class User <T>  {
>  String name;
>  T age;
> }
> ```
>
> * 注意一：使用的写法
>
>   * ```java
>     // 1,标准写法 jdk1.5标准写法:  在前后的<>都指明泛型类型
>     User<Integer> zs = new User<Integer>("zs", 18);
>     Integer age = zs.age;
>             
>     // 2, 简化写法  jdk1.7时候简化的写法:  可以省略后面的<>泛型 
>     User<Integer> zs1 = new User<>("zs", 18);
>     Integer age1 = zs1.age;
>             
>     // 3, 如果某个地方需要我们在使用的时候指明泛型, 但是我们没有指明, 那么这个需要被指明的泛型类型默认为Object
>     //   建议(只是建议): 如果某个地方设计了泛型, 建议指明
>     User zs2 = new User("zs", 18);
>     Object age2 = zs2.age;
>     ```
>
> * 注意2:  多泛型问题
>
>   * 虽然从语法上讲, 我们可以在一个泛型类上假设很多泛型类型(语法完全允许); 但是不建议(强烈)超过2个
>
>   * ```java
>     // 我们定义了一个对泛型的泛型类, 那么在使用的时候, 如果要指明泛型类型, 必须都/全部指明
>     User22<String, Integer, Integer> user = new User22<>();
>     user.name = "zs";
>     user.age = 18;
>             
>     // 我们可以在一个泛型类上定义多个泛型, 以逗号分隔
>     // 我们在泛型类上, 定义了某个泛型, 但是没有使用也是允许的
>     class User22 <XXXX, YYY, ZZZ> {
>     XXXX name;
>     YYY age;
>     }
>     ```
>
>   * 即可以不使用，但必须要指明
>
> * 注意3: 泛型的假设写法
>
>   * ```java
>     // 定义泛型的一般写法
>     // T :  Type
>     // E :  Element
>     // K :  Key
>     // V :  Value
>     class User23 <T> {
>     String name;
>     T age;
>     }
>     ```
>
> * 注意4:  泛型必须是引用类型 (实际上是不影响使用的, 拆箱装箱)
>
>   * ```java
>     // 报错, 泛型不允许使用基本类型
>     // User23<int> user231 = new User23<int>();
>             
>     int num = 10;
>     User23<Integer> user23 = new User23<Integer>();
>     user23.age = 18;
>     user23.age = num;
>     ```
>
> * 注意5: 泛型不允许new
>
>   * ```java
>     class User24  <T>{
>     String name;
>     T age;
>             
>     static {
>        // T a; 不要直接把泛型类的定义泛型在静态代码块里面使用
>     }
>     public User24(){
>        this.name = "zs";
>        // this.age = new T(); // 报错
>     }
>     }
>     ```
>
> * 注意6: 泛型类定义的泛型的作用域
>
>   * ```java
>     // 泛型类上定义一个泛型, 它的作用域仅仅局限于自己的类名和类体内
>     class F{
>     // T ft; 报错
>     }
>     class M  <T> extends F{
>     T t;
>     }
>     class S extends M{
>     // T st; 报错
>     }
>     ```
>
> * 注意7: 泛型的父子继承关系
>
>   * ```java
>     class F <T>{
>     T ft;
>     }
>     class S1 extends F{} // S1 有个Object类型的ft
>     class S2 extends F<Integer>{}// S2 有个Integer类型的ft
>     class S3 extends F<String>{} // S3 有个String类型的ft
>     class S4<E> extends F<String>{} // S4 有个String类型的ft
>     class S5<E> extends F<E>{}// S5里面的ft参照于泛型类型E
>     class S6<T> extends F<String>{}// S6有个String类型的ft
>     class S7<T> extends F<T>{} // 等价于S5的写法
>     ```



### 泛型接口

> **泛型接口: 就是把泛型定义在接口上**
>
> ```java
> interface F<T>{
> public T  getFt(T t);
> }
> class S1 implements F{
> @Override
> public Object getFt(Object o) {
>    return null;
> }
> }
> class S2 implements F<String>{
> @Override
> public String getFt(String s) {
>    return null;
> }
> }
> class S3<E> implements F<Integer>{
> @Override
> public Integer getFt(Integer integer) {
>    return null;
> }
> }
> class S4<E> implements F<E>{
> @Override
> public E getFt(E e) {
>    return null;
> }
> }
> class S5<T> implements F<T>{
> @Override
> public T getFt(T t) {
>    return null;
> }
> }
> ```
>
> 

### 泛型方法（了解）

> **泛型方法: 就是把泛型定义在方法上 (比较鸡肋)**
>
> 泛型方法比较特殊，不需要手动指明泛型，它会自动根据方法的调用参数推断出泛型的类型。
>
> ```java
> F f = new F();
> // 对于一个泛型方法, 
> // 不需要手动指明泛型, 它会自动的根据方法的调用参数推断出泛型的类型
> String zs = f.getT("zs");
> Integer t = f.getT(18);
> 
> class F{
> 
> // 这是一个泛型方法: 因为泛型定义在方法上, 要放在返回值之前
> public <T> T getT(T t){
>    return t;
> }
> }
> ```
>
> 

## 泛型的通配（了解）

> **首先泛型不允许类似数组一样协变: 害怕带来数组协变存储数据的类型不匹配问题**
>
> **又想拥有类似数组协变的功效**
>
> ```java
> //        ① 泛型通配符<?>
> //                  用来代指任意类型
> //        ② <? extends E>
> //                向下限定，代指E类型 以及 E的子类型
> //        ③ <? super E>
> //                向上限定，代指E类型  以及  E的父类型
> 
> MyLinkedCollection<?> collection1 = new MyLinkedCollection<String>();
> MyLinkedCollection<? extends F> collection2 = new MyLinkedCollection<F>();
> MyLinkedCollection<? super F> collection3 = new MyLinkedCollection<Object>();
> 
> class F{}
> class S1 extends F{}
> class S2 extends F{}
> ```
>
> 

## 泛型擦除[面试点]

> 什么是泛型擦除: Java的泛型只存在于编译之前, 当编译的时候, 泛型会被擦除成Object( **面试小概率问到** )

# 集合

## 概述

> **什么是集合类？**
>
> 是一系列Jdk实现/提供的Java类; 这些类用来让我们在Java代码逻辑中存储数据, 作为数据容器存在.
> Java集合类的本质: 就是一个Java工具类, 能用来让我们存储数据.

> **Java为什么要有集合类？**
>
> 很多情况下，我们需要对 "一组对象/某些数据" 进行操作。而且很可能事先并不知道到底有多少个对象。为了解决这个问题呢，所以,Java 就创建了一些特殊的JAVA类型用来存储数据, 这些被创建的类型也就是所谓的集合类.(为了解决: 存储更多类型问题, 扩容问题,  数据查找问题, 数据删除问题等等)

> 在Java中的集合类: 分为两块集合体系
>
> 1, **Collection集合体系**: 存储单个数据
>
> 2, **Map集合体系**: 存储key-value数据(键值对)

> 对于一个集合类我们要注意哪些相关的问题？
>
> // 1, 这个集合类的父子关系
> **2, 表现什么数据结构**
> // 3, 底层结构是什么
> // 4, (如果是数组) 扩容机制和初始长度
> // 5, 有序, 重复, null
> // 6, 是否线程安全

❗❗❗❗集合类就是要记！



## Collection

### Collection的特点

> 1. Collection是Collection集合体系的顶级接口
> 2. Collection定义了一个数据容器
> 3. Collection的有些子实现存储数据是有序的, 有些子实现存储数据是无序的
> 4. Collection的有些子实现允许存储重复数据, 有些子实现不允许存储重复数据
> 5. Collection的有些子实现允许存储null, 有些子实现不允许存储null

### Collection的API

> * Collection的**增删改查相关的api**：
>   * boolean add(E e): 添加方法
>   * boolean addAll(Collection<? extends E> c): 添加所有
>   * boolean remove(Object o): 删除某个指定数据
>   * boolean removeAll(Collection<?> c): 删除所有匹配数据
>   * boolean contains(Object o): 查找（判断某个数据是否存在）
>   * boolean containsAll(Collection<?> c): 判断某些数据是否都存在
>   * boolean retainAll(Collection<?> c): 保留所有匹配数据
> * **集合类都具有的辅助方法**：
>   * void clear() : 删除这个容器内部存储的所有数据
>   * boolean equals(Object o): 重写了这个方法, 按照内容进行比较
>   * int hashCode()：
>   * boolean isEmpty(): 判断是否为空
>   * int size():  获取这个容器存储的元素数目
> * 特殊方法：
>   * Object[] toArray() ： 返回包含此 collection 中所有元素的数组。
>   * <T> T[]  toArray(T[] a) ： 返回包含此 collection 中所有元素的数组；返回数组的运行时类型与指定数组的运行时类型相同。
>   * Iterator<E> iterator(): 返回在此 collection 的元素上进行迭代的迭代器。

#### toArray()方法

> 我们很多时候, 需要对集合类(数据容器 )进行数据遍历, 但是Collection没有办法直接遍历(为啥？), 所以Collection定义了一个toArray方法, 把里面存储的数据放到数组中返回, 就可以实现数据遍历。
>
> * 第一个toArray()方法
>   //        Object[] toArray()
>   //        返回包含此 collection 中所有元素的数组。 ( **为什么返回Object[]类型的数组, 是因为没有办法在toArray中根据泛型类型直接创建数组, 所以只能用Object类型的数组来存储数据** )
>
> * 第二个toArray()方法 : 泛型方法
>   //        <T> T[]  toArray(T[] a)
>   //        返回包含此 collection 中所有元素的数组；返回数组的运行时类型与指定数组的运行时类型相同。
>
>   * ❗虽然这是个泛型方法(从泛型语法角度上传任何类型的数组都是可以的), 但是在实际运行的时候, 只有这个数组类型传正确(和存储数据类型匹配), 才能正常运行
>
>   * ❗在使用这个泛型方法的时候, 如果数组足够长(假设 collection存储元素数量为n, 数组长度至少是n), 返回的数据和传进去的参数, 实际上是一个数组 ;   如果我们给定参数数组长度不够长(空间不够容纳所有的collection元素),那么传进去的数组仅作为类型标记, 和返回的数组并不是同一个数组
>
>   * ❗在使用这个泛型方法的时候, 如果数组过长(collection存储元素数量为n, 数组长度大于n), 它会它数组的第n+1个位置置为null, n+1之后的位置不再处理
>
>   * 源码：<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230329171304314.png" alt="image-20230329171304314" style="zoom:50%;" />
>
>   * ```java
>     示例代码：
>     package javaSE.some_importance;
>     import java.util.ArrayList;
>     import java.util.Collection;
>     import java.util.Objects;
>                     
>     public class Test {
>         public static void main(String[] args) {
>             Collection<String> collection = new ArrayList<String>();
>             // 情形一：数组过长
>             collection.add("a");
>             collection.add("b");
>             collection.add("c");
>                     
>             String[] strings = new String[6];
>             strings[3] = "d";
>             strings[4] = "e";
>             strings[5] = "f";
>             String[] strings1 = collection.toArray(strings);
>                     
>             System.out.println(strings==strings1);
>             for (String s : strings1) {
>                 System.out.println(s);
>             }
>                     
>             System.out.println("---------------------");
>                     
>             // 情形二：数组过短
>             String[] strings2 = new String[2];
>             String[] strings3 = collection.toArray(strings2);
>             System.out.println(strings2==strings3);
>             for (String s : strings3) {
>                 System.out.println(s);
>             }
>                             
>             System.out.println("---------------------");
>                             
>         }
>     }
>     ```
>
>   
>
>   toArray()方法本质上返回的是一个新数组，，，

#### iterator()方法

> 在设计Collection代码的时候, toArray()方法虽然能实现对数据的遍历, 但是toArray()需要创建数组复制源Collection数据(从内存和时间效率上讲)效率比较低. 
>
> 👆为什么这么说？可以用一张图来说明：
>
> <img src="E:/projects/idea-projects/gitee-space/java49-course-materials/02-DS_DB/img&classnote/img/集合类/toArray和iterator.png">
>
> toArray()方法在执行过程中就需要遍历，而iterator()不需要!
>
> 
>
> 所以Collection提供了一种"原地"遍历的方式: iterator()方法
>
> **代码示例**：
>
> ```java
> // 代码示例
> Collection<String> collection = new ArrayList<>();
> collection.add("zs");
> collection.add("ls");
> collection.add("wu");
> collection.add("zl");
> 
> Iterator<String> iterator = collection.iterator();
> 
> while (iterator.hasNext()){
> System.out.println(iterator.next());
> }
> ```
>
> 1. iterator本质
>
>    Collection提供了一个toArray方法, 把数据转存到数组中, 然后遍历, 但是效率不高,所以设计了iterator(原地遍历: 不复制数据, 仅维护标记)
>
>    通过Collection的iterator方法产生了一个iterator对象, 这个对象的在内存上的本质就是iterator对象内维护了一些指向源collection对象数据的标记;   
>
> 2. **iterator方法返回一个Iterator类型的对象**, 这个Iterator类型的对象有三个方法:
>
>    // Iterator类型方法:
>    **boolean hasNext()**: 向后是否可以遍历       
>    **E next()** : 向后遍历
>    **void remove()** : 删除刚刚遍历过的元素: (不要在未遍历之前删除, 也不要做连续的删除)()
>
> 3. 遍历/删除数据, 操作的是什么数据? 
>
>    iterator对象内是维护的指向源collection对象数据的标记;  那么我们通过iterator对象来做遍历(遍历或者删除), 实际上是直接遍历(遍历或者删除)原collection对象中的数据
>
>    所以对于iterator的删除操作:
>
>    * 在使用iterator的remove方法时, 不能在未遍历之前删除, 也不能做连续的删除
>    * remove不能在未遍历之前删除, 不能连续的删除:  也就意味着删除使用范围很狭窄(只有一个使用场景: 在遍历的过程, 我们觉得某个遍历数据, 不符合预期,把它删除), iterator主要是用来做遍历的(关注:hasNext, next )



##### 并发修改异常问题

> 先看示例代码：
>
> ```	java
> package com.cskaoyan.www.collection;
> import java.util.ArrayList;
> import java.util.Collection;
> import java.util.Iterator;
> import java.util.Vector;
> 
> public class DemoCollectionApi9 {
>     public static void main(String[] args) {
>         Collection<String> collection = new Vector<>();
>         collection.add("zs");
>         collection.add("ls");
>         collection.add("wu");
>         collection.add("zl");
> 
>         // 如果存在一个zs删除一个ls
> 
>         Iterator<String> iterator = collection.iterator();
> 
>         while (iterator.hasNext()){
>             String next = iterator.next();// ConcurrentModificationException
>             if (next.equals("zs")){
>                 collection.remove("ls");
>             }
>         }
> 
>         // 怎么避免并发修改异常产生:
>         // 在单线程,
>         // 不要在使用Iterator遍历开始和结束之间使用原集合类修改结构的方法直接修改原集合类
>     }
> }
> class Node{
>     String value;
>     Node Next;
>     boolean bool = false;
> 
>     public Node(String value, Node next) {
>         this.value = value;
>         Next = next;
>     }
> }
> 
> ```
>
> 报错信息：
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230329104316758.png" alt="image-20230329104316758" style="zoom:67%;" />
>
> 原因：
>
> 一些Collection的子实现是线程不安全的(加锁会导致运行效率降低), 在使用Iterator遍历的时候, 就会产生线程安全问题, 但是又不希望通过锁来保证线程安全(加锁会导致运行效率降低) ; 
>
> 所以一些集合类就维护了一个标记(标记修改次数的标记), 当源集合数据发生修改, 标记会增加;
> 在iterator对象中为了保证在遍历过程中源集合类数据没有被修改, 会在每次遍历之前检测自己保存的修改次数记录和源集合类是否一样, 如果不一样, 就认为源集合数据被别的线程修改, 抛出并发修改异常. 
> 这是为了多线程遍历数据设计，但是可能导致单线程情况下, 在遍历的过程中如果直接使用源集合类的修改结构的方法, 直接修改源集合数据, iterator对象的修改次数变量并不会同步更新，因此也会抛出并发修改异常 
>
> ❗怎么避免在单线程情况下产生并发修改异常: 
>
> **在遍历之前直接修改源集合数据, 或者在遍历完成之后修改, 不要在遍历中间过程修改**

#### Foreach方法

> Foreach循环:  增强的for循环, 加强的for循环
>
> 是在jdk1.5的时候在Java中出现
>
> 1. 注意一: 
>    // 我们Java中 foreach/增强for/加强for循环,  是依赖于iterator迭代 
>    // 也就意味着, 要使用增强的for循环遍历数据, 就要有iterator方法
>    // 同时也意味着, 如果我们使用foreach循环遍历某个Java容器, 不应该在遍历的过程中, 调用源集合类修改结构的方法直接修改源集合数据(会爆出并发修改异常)
>
>    ```java
>    //         Java的Foreach循环的本质就是iterator迭代
>            for (String s : collection) {
>    //            collection.remove("zs");// 会报错，并发修改异常
>                System.out.println(s);
>            }
>                
>    ```
>
> 2. 注意二:怎么**让自己写的容器具有foreach循环遍历的能力**
>    // 如果我们要使用foreach遍历我们自己设计的数据容器, 应该让我们自己设计的数据容器父子关系上满足是Iterable的子类; 因为Iterable中定义了iterator方法
>
> 3. 仅作了解：
>
>    // 我们知道foreach循环在Java中底层是iterator,  数组也是这样吗?
>    // 在Java中虽然数组也可以使用Foreach循环,但是数组的foreach和iterator方法没有任何关系, Jvm对数据的foreach做了特殊适配, 会编译成 fori循环



## List

回顾接口和接口的继承：

> 在Java中接口存在意义是什么? (语言层面设计)
> // 接口是用来定义规范的.
>
> 在Java中接口和接口之间的继承是为了什么?  (语言层面设计)
> // 定义/规范  的  增强

### List的特点

> // 1, List接口是Collection接口的**子接口**
> // 2, List接口在Collection接口的基础上 表示为一个逻辑结构为'线性表' 的数据容器
> // 3, List的子类存储数据有序
> // 4, List的子类都允许存储重复数据
> // 5, List的子类都允许存储null

### List的api

> api: 从上述逻辑分析, 得到结论, List是在Collection的基础上进行定义增强, 增强定义为一个逻辑结构为线性表的数据容器;  线性表最重要的特点就是数据一个接着一个排列, 也就意味着一个线性表中, 每一个数据都是有固定位序的, 等价于有下标(逻辑上的分析). 所谓在List接口怎么体现是线性表? 怎么体现是在Collection进行定义增加?  就通过增加根据下标操作的方法 来体现是个逻辑结构线性表, 来体现定义增强.
>
> | 变量和类型                               | 方法                                           | 描述                                                         |
> | :--------------------------------------- | :--------------------------------------------- | :----------------------------------------------------------- |
> | 除去原本就有的从Collection中继承来的方法 | 可以参考Collection的api看一下                  |                                                              |
> |                                          |                                                |                                                              |
> | 普通方法：                               |                                                |                                                              |
> | `void`                                   | `add(int index, E element)`                    | 将指定元素插入此列表中的指定位置。                           |
> | `boolean`                                | `add(E e)`                                     | 将指定的元素追加到此列表的末尾。                             |
> | `boolean`                                | `addAll(int index, Collection<? extends E> c)` | 从指定位置开始，将指定集合中的所有元素插入此列表。           |
> | `E`                                      | `remove(int index)`                            | 删除此列表中指定位置的元素，并返回该元素                     |
> | `boolean`                                | `remove(Object o)`                             | 从该列表中删除指定元素的第一个匹配项（如果存在）。           |
> | `E`                                      | `get(int index)`                               | 返回此列表中指定位置的元素。                                 |
> | `int`                                    | `indexOf(Object o)`                            | 返回此列表中第一次出现的指定元素的索引，如果此列表不包含该元素，则返回-1。 |
> | `int`                                    | `lastIndexOf(Object o)`                        | 返回此列表中指定元素最后一次出现的索引，如果此列表不包含该元素，则返回-1。 |
> | `E`                                      | `set(int index, E element)`                    | 用指定的元素替换此列表中指定位置的元素。                     |
> |                                          |                                                |                                                              |
> | 特殊方法：                               |                                                |                                                              |
> | `ListIterator<E>`                        | `listIterator()`                               | 返回此列表中元素的列表迭代器（按适当顺序）。                 |
> | `ListIterator<E>`                        | `listIterator(int index)`                      | 从列表中的指定位置开始，返回列表中元素的列表迭代器（**按正确顺序**）。说人话：listIterator()方法返回的遍历器的初始光标是在下标为0的数据元素之前的，而listIterator(int index)方法就可以指定遍历器的初始光标在哪里，具体看下面代码👇 |
> | `List<E>`                                | `subList(int fromIndex, int toIndex)`          | 返回指定的 `fromIndex` （包含）和 `toIndex` （不包括）之间的此列表部分的**视图**。 |
> |                                          |                                                |                                                              |
> 
> 

> 关于sublist：其实和iterator很像，sublist并不是真的截取了源数据的一部分，而只是维护了指向源数据的标识，因此如果在调用sublist方法之后直接调用原集合的删除方法，同样会引发并发修改异常问题。
>
> **以后凡是见到"视图"方法: 都代表视图方法所从原数据上获得的数据并不是真实的复制获得的,而是维护了一个标记指向原数据 (思想和Iterator基本上是一样的)**
>
> 方法描述里的**视图**该如何理解？
>
> <img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230331220445492.png" alt="image-20230331220445492" style="zoom:30%;" />

#### listIterator()方法

> List还额外提供了一个listIterator()方法，该方法返回一个ListIterator对象，ListIterator接口继承了Iterator接口，提供了专门操作List的方法。
>
> ListIterator接口在Iterator接口基础上增加了如下方法。
>
> | 变量和类型 | 方法            | 描述                                       |
> | :--------- | :-------------- | :----------------------------------------- |
> | `void`     | `add(E e)`      | 将指定的元素插入列表（可选操作）。         |
> | `boolean`  | `hasPrevious()` | 返回该迭代器关联的集合是否还有上一个元素。 |
> | `E`        | `previous()`    | 返回列表中的上一个元素并向后移动光标位置。 |
>
> 拿ListIterator与普通的Iterator进行对比，不难发现ListIterator增加了向前迭代的功能（Iterator只能向后迭代），而且ListIterator还可通过add()方法向List集合中添加元素（Iterator只能删除元素）。
>
> ```java
> /**
>  * List接口的api
>  */
> public class DemoList3 {
>     public static void main(String[] args) {
>         // ListIterator类型:
>         //        boolean hasNext()
>         //        E next()
>         //        void remove()
>         //        boolean hasPrevious(): 向前是否可以遍历: 知道
>         //        E previous(): 向前遍历: 知道
>         //        void add(E e): 添加一个数据到当前遍历位置
>         //        void set(E e): 修改刚刚遍历过的数据位置
>         //        int nextIndex(): 向后遍历的的位置的下标
>         //        int previousIndex(): 向前遍历的位置的下标
>         List<String> list = new ArrayList<>();
>         list.add("zs");
>         list.add("ls");
>         list.add("wu");
>         list.add("zl");
> 
>         //数组下标最后一个应该是siz-1，此时list.listIterator(list.size())刚好使得光标指向最后一个元素之后，这样从后往前遍历就可以全部遍历到了。
>         ListIterator<String> iterator = list.listIterator(list.size());
>         while (iterator.hasPrevious()){
>             String previous = iterator.previous();
>             System.out.println(previous);
>         }
>     }
> }
> 
> ```
>
> 

## ArrayList

### 如何分析一个集合？

> 1. 父子关系
>
> 2. 数据结构表现(未必一定要)
>
> 3. 底层结构
>
> 4. (如果底层结构有数组), 初始长度, 扩容机制
>
> 5. 有序, 重复, null
>
> 6. 是否线程安全

### ArrayList的特点【面试点】

❗面试的时候按顺序答：

> //1, ArrayList是List接口的子实现
> //2, ArrayList数据结构表现为: **线性表**
> //3, ArrayList底层是一个数组
> //4, ArrayList的底层数组的**默认初始长度 10,   默认扩容机制扩为原来的 1.5倍**
> //5, ArrayList存储数据有序
> //6, ArrayList允许存储重复数据
> //7, ArrayList允许存储null
> //8, ArrayList**线程不安全**

### ArrayLIst的构造方法

> | 构造器                                 | 描述                                                         |
> | :------------------------------------- | :----------------------------------------------------------- |
> | `ArrayList()`                          | 构造一个**初始容量为10**的空列表。                           |
> | `ArrayList(int initialCapacity)`       | 构造具有指定初始容量的空列表。                               |
> | `ArrayList(Collection<? extends E> c)` | 构造一个包含指定 collection 的元素的列表，这些元素是按照该 collection 的迭代器返回它们的顺序排列的。 |

### ArrayLIst的api

❗ArrayList作为List接口的直接实现, 它的api基本上完全遵照List接口的定义（为什么不在实现List接口的基础上多定义许多方法？原因是List作为其父接口，本身就是作为一种规范，以及作为一个类别来框住它，假如ArrayList拥有许多List之外的方法，List就无法用来作为ArrayList的类别描述了。）

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230330211856190.png" alt="image-20230330211856190" style="zoom:67%;" />

> 除了父接口的方法之外，比较特殊的api如下：
>
> | 变量和类型 | 方法                              | 描述                                                         |
> | :--------- | :-------------------------------- | :----------------------------------------------------------- |
> | `Object`   | `clone()`                         | 返回此 `ArrayList`实例的浅表副本。                           |
> | `void`     | `ensureCapacity(int minCapacity)` | 如有必要，增加此 `ArrayList`实例的容量，以确保它至少可以容纳由mincapacity参数指定的元素数。 |
> | `void`     | `trimToSize()`                    | 将此 `ArrayList`实例的容量调整为列表的当前大小。             |

> 注意1:
>
> 逻辑上讲, 如果ArrayList的Set方法应该要触发modCount增加, 但是实际jdk实现的时候没有这样做.

> 注意2:
>
> 可选操作: 当设计集合类的时候并不是每一个集合类都在逻辑上应该实现父接口定义的方法, 但是又为了集合类体系的统一性, 必须让某些子类作为某些接口的子实现, 所以在设计集合类接口api的时候, 设计了大量的可选操作api
>
> “可选”指的是什么意思？
>
> 查看collection的源码注释：![image-20230330215714251](C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230330215714251.png)
>
> ​	也就是说，这里的可选不是子类可以不实现的意思（实际上也不可能，因为子类必须实现接口中的方法），而是指在子类的实现方法中可以直接不写任何东西，直接抛出**UnsupportedOperationException**异常！



## Vector

### Vector特点

> 特点：
>
> 1, Vector是List接口的子实现
> 2, Vector数据结构表示为线性表
> 3, Vector底层结构是数组
> 4, Vector的数组的默认初始长度10,  扩容机制: 如果Vector存在大于0的容量增量, 那么Vector在扩容的时候优先扩大增量个长度, 如果没有增量或者增量不大于0默认扩为原来的2倍
> 5, Vector存储数据有序
> 6, Vector允许存储重复数据
> 7, Vector允许存储null
> 8, Vector线程安全
> 9, Vector是jdk1.0的时候出现, ArrayList是jdk1.2时候出现(为了取代Vector)

## stack

> 1, 当我们使用jdk提供的Stack时候, 虽然Stack具有add方法/remove/set...方法, 但是不建议使用, 建议使用Stack的push/pop/peek方法,对栈做增删查
>
> 2, 假如我们真的需要再代码中使用栈这种数据容器, 推荐我们使用Deque接口下的实现, 而非使用Stack
>
> ```java
> Deque<String>  stack2 = new ArrayDeque<>();
> stack2.push("zs");
> stack2.pop();
> stack2.peek();
> ```
>
> 

## LinkedList

### LinkedList的特点

> 1. LinkedList 是List接口的子实现, 同时也是Deque接口的子实现 (主要作为List子实现使用)<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230330211856190.png" alt="image-20230330211856190" style="zoom: 43%;" />
> 2. LinkedList在数据结构上: 可以表示为, 线性表, 队列, 双端队列, 栈

## ArrayDeque

> 

## Map

### Map的特点

> 特点
>
> 1. Map是Map集合体系的顶级接口
> 2. Map是一个存储映射数据(key-value; 键值对)的数据容器
> 3. Map的一些子实现有序, 一些子实现存储数据无序: (指key)
> 4. Map不允许存储重复数据: (这里的重复指的是key重复)
> 5. Map的一些子实现允许存储null, Map的一些子实现不允许存储null: (指key)
>
> 注意: Map没有办法"直接"使用foreach循环遍历数据;   (是因为Map接口不像Collection接口一样,继承了Iterable接口) (可以通过某些方法间接使用)
>
> ```java
> Collection<Map.Entry<String, Integer>> entries = map.entrySet();
>         
> for (Map.Entry<String, Integer> entry : entries) {
>     System.out.println(entry.getKey() + "----" + entry.getValue());
> }
> ```
>
> 
>
> 注意: key-value数据具有自我描述性 (数据本身能描述数据自己)

### Map接口的api

> **map接口定义的增删改查相关的api**：
>
> | 变量和类型 | 方法                                     | 描述                                             |
> | :--------- | :--------------------------------------- | :----------------------------------------------- |
> | `V`        | `put(K key, V value)`                    | 添加（可选操作）。                               |
> | `void`     | `putAll(Map<? extends K,? extends V> m)` | 将指定映射中的所有映射复制到此映射（可选操作）。 |
> | `V`        | `remove(Object key)`                     | 根据Key删除键值对（可选操作）。                  |
> | `boolean`  | `containsKey(Object key)`                | 查找key是否存在                                  |
> | `boolean`  | `containsValue(Object value)`            | 查找value是否存在                                |
> | `V`        | `get(Object key)`                        | 根据key获取key对应value                          |
>
> **集合类都具有的辅助方法**：
>
> | 变量和类型 | 方法               | 描述                                                       |
> | :--------- | :----------------- | :--------------------------------------------------------- |
> | `void`     | `clear()`          | 从此映射中删除所有映射（可选操作）。                       |
> | `int`      | `size()`           | 返回此映射中键 - 值映射的数量。                            |
> | `boolean`  | `equals(Object o)` | **将指定对象与此映射进行比较以获得相等性。**（不懂看文档） |
> | `int`      | `hashCode()`       | 返回此映射的哈希码值。                                     |
> | `boolean`  | `isEmpty()`        | 如果此映射不包含键 - 值映射，则返回 `true` 。              |
>
> **视图方法**：
>
> | 变量和类型            | 方法         | 描述                                                         |
> | :-------------------- | :----------- | :----------------------------------------------------------- |
> | `Set<K>`              | `keySet()`   | 返回此映射中包含的键的[`Set`](https://www.runoob.com/manual/jdk11api/java.base/java/util/Set.html)视图。 |
> | `Collection<V>`       | `values()`   | 返回此映射中包含的值的[`Collection`](https://www.runoob.com/manual/jdk11api/java.base/java/util/Collection.html)视图。 |
> | `Set<Map.Entry<K,V>>` | `entrySet()` | 返回此映射中包含的映射的[`Set`](https://www.runoob.com/manual/jdk11api/java.base/java/util/Set.html)视图。 |

### 关于Map.Entry

> Map.Entry是Map声明的一个内部接口，此接口为泛型，定义为Entry<K,V>。它表示Map中的一个实体（一个key-value对）
>
> 有什么用？因为Map这个类没有继承Iterable接口，当需要遍历时，不能直接通过map.[iterator](https://so.csdn.net/so/search?q=iterator&spm=1001.2101.3001.7020)来遍历，这时候可以用entrySet()方法，将其转化为Map.Entry<K,V>类型的Set视图，接着就可以使用Map.Entry类提供的一个getKey()方法和一个getValue()方法获取想要的键值对信息
>
> 举例：
>
> ```java
> public class entryLearn {
>     public static void main(String[] args) {
>         HashMap<String, Integer> hashMap = new HashMap<>();
>         
>         Set<Map.Entry<String, Integer>> entrySet = hashMap.entrySet();
>         
>         Iterator<Map.Entry<String, Integer>> entryIterator = entrySet.iterator();
>         
>         while (entryIterator.hasNext()) {
>             System.out.println(entryIterator.next().getValue());
>         }
>     }
> }
> 
> ```
>
> 

## HashMap: 非常重要❗

### 为什么要有HashMap？

> HashMap 可以存储一组**键值对**的集合，并**实现快速的查找**
>
> - 为了实现快速查找，HashMap 选择了数组而不是链表。以利用数组的索引实现 O(1) 复杂度的查找效率。
> - 为了利用索引查找，HashMap 引入 Hash 算法, 将 key 映射成数组下标: key -> Index。
> - 引入 Hash 算法又导致了 Hash 冲突。
> - 为了解决 Hash 冲突，HashMap 采用链地址法，在冲突位置转为使用链表存储。
> - 链表存储过多的节点又导致了在链表上节点的查找性能的恶化。
> - 为了优化查找性能，HashMap 在链表长度超过 8 之后转而将链表转变成红黑树，以将 O(n) 复杂度的查找效率提升至 **O(log n)**。
>
> 结论：**HashMap 存在的意义就是实现一种快速的查找并且插入、删除性能都不错的一种 key-value数据结构。**

### HashMap的底层结构

> HashMap的底层结构:  **数组+链表+红黑树**
>
> - 在JDk1.8之前, HashMap是一个单纯的: 数组 + 链表  (没有红黑树)
>
> - 在JDk1.8时候, HashMap的结构, 由数组+链表 -->  **数组+链表+红黑树**【面试答这个】



> 【**面试必问**】HashMap的存储结构：
>
> **HashMap并不是在数组上顺序存储链表/红黑树的，而是通过以下两个a、b步骤计算出存储的下标位置**
>
> <img src="E:\projects\idea-projects\gitee-space\java49-course-materials\02-DS_DB\img&classnote\img\集合类\HashMap的存储结构.png" alt="HashMap的存储结构" style="zoom:150%;" />
>
> **链表多长算过长？ 链表长度超过8达到9就算过长。**
>
> 上面图片里说的int值就是哈希值

> **为什么除了链表还要有树？**
>
> 因为链表并不适合存储大量的数据，假如有许多的数据计算出来的下标都一样，都存在同一个数据元素内，链表就会变得很长，遍历效率就会很低，而如果使用的是树，遍历效率就会高许多（和树的高相关）

> **为什么要是红黑树？**（疑问？）
>
> 因为如果是二叉搜索树，很容易变成稀疏树，若是使用AVL（平衡二叉树），对于高度差又过于严格且难实现，所以使用红黑树。

### HashMap特点

> 1. HashMap是Map接口的子实现
> 2. HashMap的底层结构: 数组 + 链表 + 红黑树
> 3. **底层数组的默认初始长度: 16 ;** 
> 4. **默认扩容机制: 扩为原来的2倍;**  
> 5. **默认的加载因子: 0.75**
> 6. 存储数据无序
> 7. 不允许存储重复的**key** 
> 8. **允许存储null作为key**
> 9. **线程不安全**

> 注意一：**加载因子问题**
>
> ```java
> //在HashMap中, 有一个默认的参数loadFactor = 0.75
> // 加载因子用来控制阈值:
> 阈值 =  加载因子 *  数组长度 
> 12  =    0.75  * 16
> // 当我们在HashMap存储的数据(key-value)个数超过阈值, 就要触发数组扩容
> ❗❗❗❗注意：扩容参照的个数并不是存了几个下标位置，而是数组中存在的结点数
> 举例：当前下标位置存的是一个链表，链表里有两个结点，那就算两个，因此，极端条件下，此时初始数组长度为16，其中只有一个下标位置存了一个红黑树，红黑树的结点总数为12个，尽管数组只用到了一个下标位置，但此时再多一个结点，就会触发数组扩容！
> ```
>
> 注意2: **数组类型**
>
> ```java
> // HashMap的底层创建了一个Node类型的数组, (也就意味着HashMap的数组存储的是结点)
> class Node{
> key,
> value,
> hash, 👈存hash是为了干啥？是为了当数组扩容的时候重新生成下标，因为下标的生成就是hash值和数组长度取余
> next
> }
> ```
>
> 注意3：在HashMap中, **对重复的key的定义**
>
> ```java
> //在HashMap存储数据的时候, 会先对key计算hash值, 取下标, 如果这个下标位置没有存储任何东西, 直接存储一个Node结点(key, value, hash, next);   如果这个下标位置已经存储了内容, 要先和这个下标位置存储的内容, 比较是否重复(key是否重复)
> 
> HashMap怎么判断两个key-value数据的key重复:
> // 如果两个key-value数据的key的hash值一样, hash一样并且 key直接相等或者key之间equals, 对于HashMap来说才是重复的key
> if (p.hash == hash && ((k = p.key) == key || (key != null && key.equals(k))))
>     
> ```
>
> 注意4：
>
> 添加/删除key-value数据：通过计算哈希值计算出下标
>
> 
>
> 注意5: 如果用一个对象充当了key
>
> ```java
> // (在实际的HashMap存储数据的时候, 常常用String作为key) 但是假设我们在HashMap中存储数据的时候用来一个引用类型的对象(非String,比如一个User对象作为key), 一旦数据已经存储到HashMap中了, 就不要通过key的引用直接修改这个key的内部的参数, 因为有可能访问不到.
> 
> 例如：
> public class DemoHashMap2 {
>     public static void main(String[] args) {
>         User zs1 = new User("zs", 18);
>         User zs2 = new User("zs", 18);
> 
>         HashMap<User, Integer> map = new HashMap<>();
>         map.put(zs1, 1);
>         map.put(zs2, 2);
> 
>         zs1.name = "ls";
> 
>         map.remove(zs1);
>         map.remove(zs2);
> 
> //        map.clear();
>         System.out.println(map.size());
>     }
> }
> 
> class User{
>     String name;
>     int age;
> 
>     public User(String name, int age) {
>         this.name = name;
>         this.age = age;
>     }
> 
>     @Override
>     public boolean equals(Object o) {
>         if (this == o) return true;
>         if (o == null || getClass() != o.getClass()) return false;
>         User user = (User) o;
>         return age == user.age &&
>                 Objects.equals(name, user.name);
>     }
> 
>     @Override
>     public int hashCode() {
>         return Objects.hash(name, age);
>     }
> }
> ```
>
> 
>
> 注意6：重复的key覆盖value
>
> ```java
> 如果我们在HashMap中存储了一份数据, 新存储数据的时候, 发现这个数据的key在HashMap中已经存在(key的hash值一样, 并且key直接相等或者相equals), 会选择用这新的key-value的数据的value覆盖已经在HashMap存储的那个重复的key-value数据的value, 并且把旧的value返回出来
> ```
>
> 
>
> 注意7: <span style="color:red">链表转化为红黑树</span>
>
> ```java
> // 链表过长, 就会转化为红黑树, 链表超过8达到9就是过长(算上新添加到这个链表上的key-value数据).
> 
> 示例: 
> for (int binCount = 0; ; ++binCount) {
> if ((e = p.next) == null) {
>     p.next = newNode(hash, key, value, null);
>     if (binCount >= TREEIFY_THRESHOLD - 1) // -1 for 1st
>         treeifyBin(tab, hash); 👈如果此时链表的结点个数>= TREEIFY_THRESHOLD（为8） - 1
>     break;
> }
> if (e.hash == hash &&
>     ((k = e.key) == key || (key != null && key.equals(k))))
>     break;
> p = e;
> }
> ```
>
> 注意8:  在HashMap中, 链表长度超过8,达到9, 一定会转化为红黑树吗?
>
> ```java
> // 不一定
> // 在HashMap中, 如果某个下标位置散列的数据过多构成了链表,  这个长度超过8达到9正常来说是要转化为红黑树的, 但是如果数组的长度是小于64的, 那么它不会从链表转化为红黑树, 而是选择扩容.
> 
> 代码示例: 
> MIN_TREEIFY_CAPACITY = 64
> (n = tab.length) < MIN_TREEIFY_CAPACITY
>     
> 🔴为啥要这样设计？
>     数组太短，缓冲空间太小（16和它的0.75倍12离得太近，如果1024的长度离768还有很多空间）假如现在数组长度为16，马上存储的数据就要到12个了，即将触发扩容，并且其中一个链表的结点马上就要到9个了，一旦扩容，数组边长，数据元素的下标就有可能因此发生变化（因为是hash值与数组长度取余），那么链表就有可能因此重新散列，就不需要转化成红黑树了，假如链表转化成红黑树，那就有可能刚转化成红黑树又立马重新退化为链表，反复横跳，毫无意义
> ```
>
> 注意9:  数组扩容, 某个在原数组的x位置的key-value, 经过重新散列之后的位置问题?
>
> ```java
> // 如果在HashMap的底层数组扩容的时候,  原本在旧数组的x下标位置存储的数据, 要用hash值和新的数组取余数得到在新的数组中存储的位置;  
> 🔴这个新的位置: 要么还在x位置, 要么在  旧数组长度+x位置
> 
> eg:
> 原数组长度16
> 存储在下标8的位置
> // 扩容
> 新数组长度32
> 原本在8 --> 在新数组的 8 or 24 
>     
> 为啥？
> 🔴下标 = hash % 16 = 8  说明 hash为16的倍数+8 ，如果是16的奇数倍，和32取余就是16 + 8
> ```
>
> 注意10:  红黑树转化为链表的问题?
>
> ```java
> // 在HashMap中, 有两种情况, 会导致红黑树转化会链表
> 
> 1, 当删除数据的时候; (删除的数据, 删的并且是红黑树上的结点, 结点变少)
> // 当删除红黑树上结点的时候: 如果这个红黑树上面"根结点" "根的左右结点""根的左结点的左结点"这四个结点只要有一个不在, 那么就代表树的存储的结点数太少了, 就要由红黑树转化为链表
> 
> eg: 
> // root树的根结点
> root == null  || (root.right == null || (rl = root.left) == null || rl.left == null)
> 
> 2, 当扩容的时候. (扩容会导致红黑树拆成两部分,  结点变少)
> // 🔴当扩容的时候, 一个红黑树会被拆成两部分(低位:旧下标位置;  高位: 旧下标位置+旧数组长度),  这两部分要分别看待,  两个位置的任何一个位置只要数据量(key-value数据个数)小于等于6个‼️🐷, 那么这个位置就不能再继续维护红黑树, 要转化回链表.   
> ```
>
> 注意11:  为什么链表转化为红黑树的阈值设置为8, 红黑树转化为链表阈值设置为6
>
> ```java
> 🔴为了给链表和红黑树转化的数据量预留一些缓冲区间,  避免链表和红黑树反复转化.
> ```
>
> 注意12:   给HashMap指定数组的长度
>
> ```java
> // 如果我们在HashMap的构造方法里, 给HashMap传入一个指定长度, 用来指明数组长度, 它会把这个给定长度变成一个大于等于给定值的最小的2的幂值, 作为底层数组长度.
> 
> eg:
> 10 -> 16
> 20 -> 32
> 16 -> 16
> ```
>
> 注意13: 了解
>
> ```java
> // 1, 红黑树怎么存储数据的问题, 先根据hash值比较选择左右方向; 
> 
> // 2, 如果在红黑树中, hash相同, 但是key不相等也不相equals.  HashMap会强制调用key的来自于Object的hashCode获取hash值, 进行得到一个具有"严格大小"的比较结果
> ```
>
> 

### HashMap的构造函数

> | 构造器                                           | 描述                                                         |
> | :----------------------------------------------- | :----------------------------------------------------------- |
> | `HashMap()`                                      | 使用默认初始容量（16）和默认加载因子（0.75）构造一个空 `HashMap` 。 |
> | `HashMap(int initialCapacity)`                   | 使用指定的初始容量和默认加载因子（0.75）构造一个空 `HashMap` 。 |
> | `HashMap(int initialCapacity, float loadFactor)` | 使用指定的初始容量和加载因子构造一个空 `HashMap` 。          |
> | `HashMap(Map<? extends K,? extends V> m)`        | 构造一个映射关系与指定 Map 相同的新 HashMap。                |

### 源码分析

#### 存储结构【仅关心有标识的部分即可】

> ```java
> 1.底层是Node类型的数组：
>  /**
>  * The table, initialized on first use, and resized as
>  * necessary. When allocated, length is always a power of two.
>  * (We also tolerate length zero in some operations to allow
>  * bootstrapping mechanics that are currently not needed.)
>  */
> transient Node<K,V>[] table;
> 
> 2.HashMap的底层创建了一个Node类型的数组, (也就意味着HashMap的数组存储的是结点)
> Node包含四个属性：hash、key、value、next
> static class Node<K,V> implements Map.Entry<K,V> {
>     🔴final int hash;
>     🔴final K key;
>     🔴V value;
>     🔴Node<K,V> next;
>     
> 3.数组的初始化：
> 并没有在构造方法中进行初始化，构造方法中仅初始化了加载因子
>     //构造方法
>     /**
>      * Constructs an empty <tt>HashMap</tt> with the default initial capacity
>      * (16) and the default load factor (0.75).
>      */
>     public HashMap() {
>     	// loadFactor是加载因子/装填因子，用来控制阈值
>     	阈值 =  加载因子 *  数组长度 
> 		12  =    0.75  * 16
> 		// 当我们在HashMap存储的数据(key-value)个数超过阈值, 就要触发数组扩容   
>         //  
>         this.loadFactor = DEFAULT_LOAD_FACTOR; // all other fields defaulted
>     }
>     
> //这个DEFAULT_LOAD_FACTOR是啥？用来给loadFactor初始赋值的
>      /**
>      * The load factor used when none specified in constructor.
>      */
>     static final float DEFAULT_LOAD_FACTOR = 0.75f;
>     // 
>     
>     既然没有在构造方法对数组进行初始化，那么应该猜测，在第一次添加时对其进行初始化
>     👉put方法：
>    /**
>      * Associates the specified value with the specified key in this map.
>      * If the map previously contained a mapping for the key, the old
>      * value is replaced.
>      *
>      * @param key key with which the specified value is to be associated
>      * @param value value to be associated with the specified key
>      * @return the previous value associated with <tt>key</tt>, or
>      *         <tt>null</tt> if there was no mapping for <tt>key</tt>.
>      *         (A <tt>null</tt> return can also indicate that the map
>      *         previously associated <tt>null</tt> with <tt>key</tt>.)
>      */
>     public V put(K key, V value) {
>         return putVal(hash(key), key, value, false, true);
>     }
>     
>     👉其中的putVal方法：分析第一次添加情况
>         /**
>      * Implements Map.put and related methods
>      *
>      * @param hash hash for key
>      * @param key the key
>      * @param value the value to put
>      * @param onlyIfAbsent if true, don't change existing value
>      * @param evict if false, the table is in creation mode.
>      * @return previous value, or null if none
>      */
>     final V putVal(int hash, K key, V value, boolean onlyIfAbsent,
>                    boolean evict) {
>         Node<K,V>[] tab; 
>         Node<K,V> p; 
>         int n, i;  👇第一次添加时，table没有初始化，为null
>         if ((tab = table  👈底层数组（table）) == null || (n = tab.length) == 0)
>             			👇第一次扩容：此时调用了resize方法（用于扩容的）【见下方】
>             n = (tab = resize()).length;
>         if ((p = tab[i = (n - 1) & hash]) == null)
>             tab[i] = newNode(hash, key, value, null);
>         else {
>             Node<K,V> e; K k;
>             if (p.hash == hash &&
>                 ((k = p.key) == key || (key != null && key.equals(k))))
>                 e = p;
>             else if (p instanceof TreeNode)
>                 e = ((TreeNode<K,V>)p).putTreeVal(this, tab, hash, key, value);
>             else {
>                 for (int binCount = 0; ; ++binCount) {
>                     if ((e = p.next) == null) {
>                         p.next = newNode(hash, key, value, null);
>                         if (binCount >= TREEIFY_THRESHOLD - 1) // -1 for 1st
>                             treeifyBin(tab, hash);
>                         break;
>                     }
>                     if (e.hash == hash &&
>                         ((k = e.key) == key || (key != null && key.equals(k))))
>                         break;
>                     p = e;
>                 }
>             }
>             if (e != null) { // existing mapping for key
>                 V oldValue = e.value;
>                 if (!onlyIfAbsent || oldValue == null)
>                     e.value = value;
>                 afterNodeAccess(e);
>                 return oldValue;
>             }
>         }
>         ++modCount;
>         if (++size > threshold)
>             👇当添加数组超过阈值时也会触发扩容
>             resize();
>         afterNodeInsertion(evict);
>         return null;
>     }
>    
>     
> resize()方法-----用于扩容    
>  /**
>      * Initializes or doubles table size.  If null, allocates in
>      * accord with initial capacity target held in field threshold.
>      * Otherwise, because we are using power-of-two expansion, the
>      * elements from each bin must either stay at same index, or move
>      * with a power of two offset in the new table.
>      *
>      * @return the table
>      */
>     final Node<K,V>[] resize() {
>         Node<K,V>[] oldTab = table;
>                       👇oldTab：旧数组长度=0
>         int oldCap = (oldTab == null) ? 0 : oldTab.length;
>               👇旧阈值=0   👇？
>     	int oldThr = threshold;
>     		👇新长度 👇新阈值 
>         int newCap, newThr = 0;
>         if (oldCap > 0) {
>             if (oldCap >= MAXIMUM_CAPACITY) {
>                 threshold = Integer.MAX_VALUE;
>                 return oldTab;
>             }
>             else if ((newCap = oldCap << 1) < MAXIMUM_CAPACITY &&
>                      oldCap >= DEFAULT_INITIAL_CAPACITY)
>                 newThr = oldThr << 1; // double threshold
>         }
>     	
>        else if (oldThr > 0) // initial capacity was placed in threshold
>             newCap = oldThr;
>     	🔴
>         else {               // zero initial threshold signifies using defaults
>             👇新长度      👇这个值为16
>             newCap = DEFAULT_INITIAL_CAPACITY;
>             👇新阈值 = 0.75 * 16 就等于 12了
>             newThr = (int)(DEFAULT_LOAD_FACTOR * DEFAULT_INITIAL_CAPACITY);
>         }
>         if (newThr == 0) {
>             float ft = (float)newCap * loadFactor;
>             newThr = (newCap < MAXIMUM_CAPACITY && ft < (float)MAXIMUM_CAPACITY ?
>                       (int)ft : Integer.MAX_VALUE);
>         }
>     	👇threshold = 12
>         threshold = newThr;
>          
>     				👇定义一个新长度的数组newTab
>     	Node<K,V>[] newTab = (Node<K,V>[])new Node[newCap];
>         
>     	👇：将上面定义的数组赋给table，数组初始化完成！
>     	table = newTab;
>  
>     ---------------------以下代码是用于将旧数组转移到新数组---------------------
>         if (oldTab != null) {
>             for (int j = 0; j < oldCap; ++j) {
>                 Node<K,V> e;
>                 if ((e = oldTab[j]) != null) {
>                     oldTab[j] = null;
>                     if (e.next == null)
>                         newTab[e.hash & (newCap - 1)] = e;
>                     else if (e instanceof TreeNode)
>                         ((TreeNode<K,V>)e).split(this, newTab, j, oldCap);
>                     else { // preserve order
>                         Node<K,V> loHead = null, loTail = null;
>                         Node<K,V> hiHead = null, hiTail = null;
>                         Node<K,V> next;
>                         do {
>                             next = e.next;
>                             if ((e.hash & oldCap) == 0) {
>                                 if (loTail == null)
>                                     loHead = e;
>                                 else
>                                     loTail.next = e;
>                                 loTail = e;
>                             }
>                             else {
>                                 if (hiTail == null)
>                                     hiHead = e;
>                                 else
>                                     hiTail.next = e;
>                                 hiTail = e;
>                             }
>                         } while ((e = next) != null);
>                         if (loTail != null) {
>                             loTail.next = null;
>                             newTab[j] = loHead;
>                         }
>                         if (hiTail != null) {
>                             hiTail.next = null;
>                             newTab[j + oldCap] = hiHead;
>                         }
>                     }
>                 }
>             }
>         }
>         return newTab;
>     }
> ```

#### 扩容机制

> ```java
> final Node<K,V>[] resize() {
>         Node<K,V>[] oldTab = table;
>         int oldCap = (oldTab == null) ? 0 : oldTab.length;
>         int oldThr = threshold;
>         int newCap, newThr = 0;
>         if (oldCap > 0) {
>             if (oldCap >= MAXIMUM_CAPACITY) {
>                 threshold = Integer.MAX_VALUE;
>                 return oldTab;
>             }
>             else if ((newCap = oldCap << 1) < MAXIMUM_CAPACITY &&
>                      oldCap >= DEFAULT_INITIAL_CAPACITY)
>                 newThr = oldThr << 1; // double threshold
>         }
>         else if (oldThr > 0) // initial capacity was placed in threshold
>             newCap = oldThr;
>         else {               // zero initial threshold signifies using defaults
>             newCap = DEFAULT_INITIAL_CAPACITY;
>             newThr = (int)(DEFAULT_LOAD_FACTOR * DEFAULT_INITIAL_CAPACITY);
>         }
>         if (newThr == 0) {
>             float ft = (float)newCap * loadFactor;
>             newThr = (newCap < MAXIMUM_CAPACITY && ft < (float)MAXIMUM_CAPACITY ?
>                       (int)ft : Integer.MAX_VALUE);
>         }
>         threshold = newThr;
>         @SuppressWarnings({"rawtypes","unchecked"})
>             Node<K,V>[] newTab = (Node<K,V>[])new Node[newCap];
>         table = newTab;
>         if (oldTab != null) {
>             for (int j = 0; j < oldCap; ++j) {
>                 Node<K,V> e;
>                 if ((e = oldTab[j]) != null) {
>                     oldTab[j] = null;
>                     if (e.next == null)
>                         newTab[e.hash & (newCap - 1)] = e;
>                     else if (e instanceof TreeNode)
>                         ((TreeNode<K,V>)e).split(this, newTab, j, oldCap);
>                     else { // preserve order
>                         Node<K,V> loHead = null, loTail = null;
>                         Node<K,V> hiHead = null, hiTail = null;
>                         Node<K,V> next;
>                         do {
>                             next = e.next;
>                             if ((e.hash & oldCap) == 0) {
>                                 if (loTail == null)
>                                     loHead = e;
>                                 else
>                                     loTail.next = e;
>                                 loTail = e;
>                             }
>                             else {
>                                 if (hiTail == null)
>                                     hiHead = e;
>                                 else
>                                     hiTail.next = e;
>                                 hiTail = e;
>                             }
>                         } while ((e = next) != null);
>                         if (loTail != null) {
>                             loTail.next = null;
>                             newTab[j] = loHead;
>                         }
>                         if (hiTail != null) {
>                             hiTail.next = null;
>                             newTab[j + oldCap] = hiHead;
>                         }
>                     }
>                 }
>             }
>         }
>         return newTab;
>     }
> ```
>
> 

#### 哈希值的计算

> ```java
> 在HashMap存储数据的时候, 当我们要存储一份key-value数据, 会先把key取出进行计算,得到一个hash值.
> 我们希望最终存储数据的时候, 每一个key-value都尽量散列到不同的位置; 为了保证这个结果, 我们"希望"每一个key的hash值尽量不要相同. (数组下标的选取是通过计算得到的hash值与对数组长度取余得到的，而数组长度是2的幂值，对其取余相当于去当前hash值的低位（即 17%16 等价于 17&15）) 或者更进一步说, 我们"希望"hash值的低位不要相同. 所以我们让key的hashCode参数, 高位和低位混合,得到hash值 (高位不变, 低位是个混合值)(从逻辑上复合概率论上的一个映射的基本思想, 在映射的过程中给更多不确定的条件, 导致映射更随机)
> 
> 
> 
> static final int hash(Object key) {
>         int h;                              👇hash值的计算方式: hash值来源于一个key的                                                   hashCode方法
>         return (key == null) ? 0 : (h = key.hashCode()) ^ (h >>> 16);
>                                    -----------------------------------
>                                        👆为了存储数据的时候每个数据都尽量散列在不同位置，源码并                                          没有直接使用hashcode，而是还对其进行了移位异或，目的                                          是为了使其散列的更均匀【喝前摇一摇】
>     }
> //  异或：同则0异则1
> //  1101010101 1111010110
> //  0000000000 1101010101
> //^
> //  1101010101 0010000011
> hashCode 和 hash一一对应
> ```
>
> > 哈希算法：对于任何一个**文件**【对计算机来说，一切皆是文件】都可以通过计算得到一个哈希值
> >
> > 常见的哈希算法：md5（计算得出128位二进制数作为哈希值）
> >
> > 有没有可能两个不同的文件计算出相同的哈希值？有可能
> >
> > 为什么？因为文件的数量是无穷的，而哈希值的范围是有限的，所以肯定会有重复
> >
> > 

### 🐷总结

#### 一份key-value数据的添加过程

> // 1, 有一份key-value数据, 要添加的HashMap中
> // 2, 取出key 计算 hash值 ((h = key.hashCode()) ^ (h >>> 16);)
> 取移位和异或运算的原因是希望充分散列/尽量不冲突
> // 3, 用计算的hash值和数组长度取模: (n - 1) & hash
> 推出一个隐含的结论, 在取模计算中 只有hash值的低位会起效果
> // 4, 根据上一步计算的下标, 判断这个下标位置是否已经存储了内容, 如果没有存储内容, 直接创建一个结点存储到这个下标位置
> 结点是Node类型, 包含: key,value, hash,next四个参数
> // 5,  根据上一步(第3)计算的下标, 这个下标位置可能已经存储了元素:  先判断是否重复
> hash一样; 并且,  两个key要么直接相等, 要么相equals
> 			p.hash == hash && ((k = p.key) == key || (key != null && key.equals(k)))
> //      5.1 如果key值重复了, 新的key-value的value值覆盖旧值   
> //      5.2 如果key值不重复, 接着按照链表向下比较, 在遍历链表的过程中还是判断链表中的结点是否重复, (重复了, 新值覆盖旧值)
> //          如果在这个链表比较的过程中, 一直不重复, 把这份新的key-value数据,构建一个结点,添加到这个链表的尾部
> // 6, 如果在这个下标位置, 不重复, 添加(构建链表)(5.2步骤), 如果添加一个元素之后, 导致链表出长度(超过8, 达到9), 那么添加完成之后, 这个链表要转化为红黑树
> //         如果转化红黑树的过程中, 发现数组长度小于64, 选择扩容(元素重新按照新长度散列问题), 而非转化为红黑树
>
> // 7, 假设上述步骤添加成功一份key-value数据:  有可能引起扩容 (整体存储的数据超过阈值)
>
> // 8, 上述所有的扩容, 都有可能导致原本数组某个位置如果有红黑树, 红黑树被拆成两部分(低位和高位), 任一位置结点数变少, 又有可能导致红黑树转化为链表 

#### HashMap的遍历

> 底层数组从头向尾遍历，遇到链表或者红黑树就随着结点顺序进行遍历

## LinkedHashMap

### LinkedHashMap的特点

> 1. LinkedHashMap是**HashMap**的子类
> 2. LinkedHashMap底层基本上完全复用了HashMap的结构 --> LinkedHashMap的特点基本上和HashMap一样
> 3. **LinkedHashMap在HashMap的基础上额外定义了一个双向链表, 用以保证迭代顺序 (重要)**
> 4. LinkedHashMap存储数据有序
> 5. LinkedHashMap不允许存储重复数据
> 6. LinkedHashMap允许存储null
> 7. 线程不安全

### LinkedHashMap的构造方法

> ```java
> LinkedHashMap() 
>      构造一个带默认初始容量 (16) 和加载因子 (0.75) 的空插入顺序 LinkedHashMap 实例。 
> LinkedHashMap(int initialCapacity) 
>      构造一个带指定初始容量和默认加载因子 (0.75) 的空插入顺序 LinkedHashMap 实例。 
> LinkedHashMap(int initialCapacity, float loadFactor) 
>      构造一个带指定初始容量和加载因子的空插入顺序 LinkedHashMap 实例。 
> LinkedHashMap(int initialCapacity, float loadFactor, boolean accessOrder) 
>      构造一个带指定初始容量、加载因子和排序模式的空 LinkedHashMap 实例。 
> LinkedHashMap(Map<? extends K,? extends V> m) 
>      构造一个映射关系与指定映射相同的插入顺序 LinkedHashMap 实例。 
> ```
>
> LinkedHashMap可用于LRU

### LinkedHashMap的api

> LinkedHashMap并没有在Map接口的基础上额外定义什么api (甚至底层的方法就直接使用的HashMap定义的方法



## Hashtable【面试点】

> **和HashMap一样，Hashtable 也是一个散列表，它存储的内容是键值对(key-value)映射。**
>
> 🐷为了将Hashtable归到Map中去，强制其实现了Map接口

> 实际工作中几乎用不到，但是面试会问：
>
> **Hashtable和HashMap有什么区别?**
>
> 1. Hashtable是Map接口的子实现
> 2. Hashtable的底层结构: **数组 + 链表   (没有红黑树)**(和HashMap的jdk1.8之前一样)
> 3. Hashtable的默认初始容量11 ,  扩容机制: 2倍+1
> 4. 存储数据**无序**
> 5. 不允许存储重复的key
> 6. 不允许存储null作为**key**;   不允许存储null作为**value**
> 7. **线程安全**
> 8. 是jdk1.0的时候产生   (HashMap是jdk1.2的时候出现)



## Properties

> 1. Java 的 Properties 加载属性文件后是无法保证输出的顺序与文件中一致的，因为 **Properties 是继承自 Hashtable** 的， key/value 都是直接存在 Hashtable 中的，而 Hashtable 是不保证进出顺序的。
> 2. Properties底层结构完全复用的Hashtable的结构



## TreeMap

### TreeMap的特点

> 1. TreeMap是Map接口的子实现
> 2. TreeMap底层是一个红黑树
> 3. TreeMap底层是链表表示红黑树
> 4. TreeMap存储数据**大小有序**
> 5. TreeMap不允许存储重复的key数据 
>    * 对于TreeMap来讲什么叫重复?
>    * **TreeMap对重复的key的判断和hash, equals都没有关系, 而是判断这两个key是否大小一样**
> 6. TreeMap不允许存储null作为key  (**因为null没有办法比较大小**)
> 7. TreeMap线程不安全
>
> ❗❗注意: 在TreeMap底层是红黑树,  所以TreeMap存储数据是要根据key的大小来判断是否重复/判断大小.
> 这也就要求, 我们存储到TreeMap中的数据要根据大小进行存储.
> 所以, 我们存储到TreeMap中的key-value数据的key要能比较大小(实现Comparable的compareTo方法).
> 如果我们不想自己的key-value的key实现自然顺序(实现Comparable的compareTo方法), 也可以在TreeMap的构造方法中传入一个比较器 (Comparator对象)用来比较大小.

### TreeMap的构造方法

> | 构造器                                      | 描述                                                         |
> | :------------------------------------------ | :----------------------------------------------------------- |
> | `TreeMap()`                                 | 使用其键的自然顺序构造一个新的空树图。                       |
> | `TreeMap(Comparator<? super K> comparator)` | 构造一个新的空树图，根据给定的比较器排序。                   |
> | `TreeMap(Map<? extends K,? extends V> m)`   | 构造一个新的树映射，其中包含与给定映射相同的映射，根据其键的 *自然顺序排序* 。 |
> | `TreeMap(SortedMap<K,? extends V> m)`       | 构造一个包含相同映射的新树映射，并使用与指定有序映射相同的顺序。 |



### TreeMap的api

> | 变量和类型       | 方法                  | 描述                                                    |
> | :--------------- | :-------------------- | :------------------------------------------------------ |
> | `Map.Entry<K,V>` | `ceilingEntry(K key)` | 返回大于等于给定值的**键值对**，如果没有则null 。       |
> | `K`              | `ceilingKey(K key)`   | 返回大于等于给定值的key，如果没有这样的键，则 `null` 。 |
> | `Map.Entry<K,V>` | `floorEntry(K key)`   | 返回小于等于给定值的键值对                              |
> | `K`              | `floorKey(K key)`     | 返回小于等于给定值的key                                 |
> | `K`              | `higherKey(K key)`    | 返回大于给定值的key                                     |
> |                  |                       |                                                         |
> |                  |                       |                                                         |
> |                  |                       |                                                         |
> |                  |                       |                                                         |
> |                  |                       |                                                         |



## Set

<img src="C:\Users\ziupa\AppData\Roaming\Typora\typora-user-images\image-20230403201102697.png" alt="image-20230403201102697" style="zoom:67%;" />

### Set的特点

> 1. Set接口是Collection的子接口
> 2. Set接口表示的数据结构为: **集合**【🐷：不要和集合类搞混，集合类是一种存放数据的容器，而这里的集合指的是数学上的集合】
> 3. Set下的子实现底层全部是持有对应的Map下的对象(HashSet -> HashMap; LinkedHashSet -> LinkedHashMap;   TreeSet -> TreeMap)
> 4. Set的一些子实现有序(LinkedHashSet有序, TreeSet大小有序), 有些子实现无序(HashSet)
> 5. Set的子实现全部都不允许存储重复数据 (HashSet/LinkedHashSet: hash值一样之后, 数据要么直接相等,要么相equals)(TreeSet: 大小重复)
> 6. Set有些子实现允许存储null(HashSet/LinkedHashSet) 有些子实现不允许存储null(TreeSet)

### Set的api

> Set接口没有在Collection的基础上额外定义什么api

## HashSet

### HashSet的特点

> 1. HashSet是Set接口的子实现
> 2. HashSet底层持有了一个HashMap对象, 当我们向HashSet中添加数据的时候, 实际这些数据都添加到HashSet对象底层所持有的HashMap的key上去了; 也就意味着HashSet的特点遵照与HashMap的key的特点
> 3. 存储数据无序
> 4. 不允许存储重复的数据(hash值一样之后, 数据要么直接相等,要么相equals)
> 5. 允许存储null
> 6. 线程不安全

### HashSet的构造方法

> ```java
> HashSet() 
>        构造一个新的空 set，其底层 HashMap 实例的默认初始容量是 16，加载因子是 0.75。
> HashSet(int initialCapacity) 
>        构造一个新的空 set，其底层 HashMap 实例具有指定的初始容量和默认的加载因子（0.75）。 
> HashSet(int initialCapacity, float loadFactor) 
>        构造一个新的空 set，其底层 HashMap 实例具有指定的初始容量和指定的加载因子。
> HashSet(Collection<? extends E> c) 
>        构造一个包含指定 collection 中的元素的新 set。 
> ```

### HashSet的api

> HashSet完全和Set接口定义一样: 没有在Collection的基础上额外定义什么api



## LinkedHashSet

### LinkedHashSet的特点

> 1. LinkedHashSet是HashSet的子实现	
> 2. 底层持有了一个LinkedHashMap对象
> 3. 存储数据有序
> 4. 不允许存储重复数据
> 5. 允许存储null
> 6. 线程不安全







## Stream

注意：此流非IO流，一般说流，指的是I/O流，Stream是基于集合的，用来处理集合数据。

###  Stream概述

> 假如我们拥有一个 学生列表
>
> ```java
> public class Person {
>     public enum Address{
>         BJ,
>         SH,
>         WH,
>         SZ
>     }
>     private String name;
>     private int age;
>     private int height;
>     private Address address;
> }
> ```
>
> ```java
> public class StudentList {
>     public List<Person> personList ;
> 
>     public StudentList(){
>         this.personList = new ArrayList<>();
> 
>         personList.add(new Person("aa", 18, 170, Person.Address.BJ));
>         personList.add(new Person("bb", 20, 163, Person.Address.SH));
>         personList.add(new Person("cc", 30, 182, Person.Address.WH));
>         personList.add(new Person("dd", 16, 190, Person.Address.BJ));
>         personList.add(new Person("ee", 15, 210, Person.Address.SH));
>         personList.add(new Person("ff", 17, 160, Person.Address.WH));
>         personList.add(new Person("gg", 18, 169, Person.Address.BJ));
>         personList.add(new Person("hh", 20, 173, Person.Address.WH));
>         personList.add(new Person("ii", 22, 192, Person.Address.SH));
>         personList.add(new Person("jj", 25, 172, Person.Address.SH));
>         personList.add(new Person("kk", 24, 188, Person.Address.BJ));
>         personList.add(new Person("ll", 17, 161, Person.Address.WH));
>         personList.add(new Person("mm", 18, 169, Person.Address.SH));
>         personList.add(new Person("nn", 20, 162, Person.Address.BJ));
>         personList.add(new Person("oo", 22, 166, Person.Address.SH));
>         personList.add(new Person("pp", 24, 176, Person.Address.WH));
>         personList.add(new Person("qq", 22, 173, Person.Address.BJ));
>         personList.add(new Person("rr", 24, 177, Person.Address.BJ));
>         personList.add(new Person("ss", 17, 169, Person.Address.SH));
>         personList.add(new Person("tt", 18, 170, Person.Address.SH));
>         personList.add(new Person("uu", 20, 171, Person.Address.WH));
>         personList.add(new Person("vv", 22, 172, Person.Address.WH));
>         personList.add(new Person("ww", 24, 181, Person.Address.BJ));
>         personList.add(new Person("xx", 18, 188, Person.Address.SH));
>         personList.add(new Person("yy", 20, 183, Person.Address.BJ));
>         personList.add(new Person("zz", 22, 191, Person.Address.WH));
>     }
> }
> ```
>
> 我们要对这个学生列表进行处理:  <span style="color:red">得到来自北京同学, 并且高度最高的三个同学</span>
>
> 应该怎么做
>
> 方式一：
>
> ```java
> 		TreeSet<Person> peoples = new TreeSet<>(new Comparator<Person>() {
>             @Override
>             public int compare(Person o1, Person o2) {
>                 int com = o2.getHeight() - o1.getHeight();
>                 return com;
>             }
>         });
> 
>         for (Person person : personList) {
>             if (person.getAddress() == Person.Address.BJ){
>                 peoples.add(person);
>             }
>         }
> 
>         System.out.println(peoples.first());
>         peoples.pollFirst();
>         System.out.println(peoples.first());
>         peoples.pollFirst();
>         System.out.println(peoples.first());
>         peoples.pollFirst();
> ```
>
> 那么对于上述代码有没有更好的方法(类似于我们对数据库的操作一样)?
>
> 我们可以使用JAVA中Stream流来解决上述问题
>
> ```java
>  List<Person> collect = personList.stream()
>                 .filter(a -> a.getAddress() == Person.Address.BJ)
>                 .sorted(Comparator.comparing(Person::getHeight).reversed())
>                 .limit(3)
>                 .collect(Collectors.toList());
> 
>          System.out.println(collect);
> ```

> * 什么是流？
>
>   * 流是Java API, 它允许我们以声明的方式来处理集合数据, 也就是说我们不再需要编写一个实现来操作要处理的数据, 而是类似于数据库那样通过查询语句来表达.
>
>     Java中集合类数据处理的一种简化方式;
>
>     通俗的讲: 也就是说, Stream流是Java在jdk1,8提供的对集合数据进行优化/简化操作的一种数据处理方式
>
> * 流用来解决什么问题?
>
>   * Stream流一般用来处理Java中的集合类数据, 进以避免在日常代码书写中的对集合数据操作的性能以及代码冗长问题.
>
> * **流的思想是什么?**【重要】
>
>   和Collection操作不同的是Stream操作有`两个基础的特征`：
>
>   * <span style="color:red">`Pipelining`</span>: 中间操作都会返回流对象本身. 这样多个操作可以串联成一个管道， 如同流式风格(ﬂuent style).
>      这样做可以对操作进行优化.
>   * `内部迭代`: 以前对集合遍历都是通过Iterator或者增强for的方式, 显式的在集合外部进行迭代， 这叫做外部迭代.Stream提供了内部迭代的方式，流可以直接调用遍历方法(所谓”内部“，是指这个遍历在语法底层，是不可直接见的).
>
> * 流有哪些优点?
>
>   * Stream流是一个集合元素的`函数模型`，它并不是集合，也不是数据结构，**其本身并不存储任何元素.**（想象一个管道连接一片湖，负责传输水，不生产水，只是大自然的搬运工）
>   * Stream流是在对函数模型进行操作，(在终结触发之前)集合元素并没有真正被处理，只有当终结方法执行的时候，整个模型才会按照指定策略执行操作.
>   * 对集合数据操作的性能优化,解决代码冗长问题.
>
>   

<span style="color:red">怎么使用流?</span>

> 使用一个流的时候，通常包括三个基本步：
>
> 1. 一个数据源, 创建一个流
>
> 2. 多个(0-n)中间操作, 形成一条流水线
>
> 3.  一个终止/终端操作, 执行流水线,并生成结果

### 创建流

> 三种创建方式：
>
> 1. <span style="color:red"> 调用集合类的stream方法,生成一个流</span>(最常用/常见)
>
>    ```java
>    Collection collection = new ArrayList();
>            Stream stream = collection.stream();
>    ```
>
>    
>
> 2. 由值创建
>
>    ```java
>    Stream<String> zs = Stream.of("zs", "ls", "wu", "zl");
>    ```
>
>    
>
> 3. 由数组创建
>
>    ```java
>    String [] strs = {"zs", "ls", "wu"};
>            Stream<String> stream = Arrays.stream(strs);
>    ```
>
>    
