**目录：**

- [中小团队技术选型](#%E4%B8%AD%E5%B0%8F%E5%9B%A2%E9%98%9F%E6%8A%80%E6%9C%AF%E9%80%89%E5%9E%8B)
    - [发布/部署](#%E5%8F%91%E5%B8%83%E9%83%A8%E7%BD%B2)
    - [docker](#docker)
    - [配置中心](#%E9%85%8D%E7%BD%AE%E4%B8%AD%E5%BF%83)
    - [SQL自动审核工具](#sql%E8%87%AA%E5%8A%A8%E5%AE%A1%E6%A0%B8%E5%B7%A5%E5%85%B7)
- [Java](#java)
    - [awesome](#awesome)
    - [源码学习](#%E6%BA%90%E7%A0%81%E5%AD%A6%E4%B9%A0)
    - [学习案例](#%E5%AD%A6%E4%B9%A0%E6%A1%88%E4%BE%8B)
    - [开发手册](#%E5%BC%80%E5%8F%91%E6%89%8B%E5%86%8C)
    - [Lib](#lib)
    - [框架](#%E6%A1%86%E6%9E%B6)
    - [tools-监控](#tools-%E7%9B%91%E6%8E%A7)
    - [JVM](#jvm)
- [前端](#%E5%89%8D%E7%AB%AF)
- [数据库](#%E6%95%B0%E6%8D%AE%E5%BA%93)
- [AI算法](#ai%E7%AE%97%E6%B3%95)
- [22待整理](#22%E5%BE%85%E6%95%B4%E7%90%86)

==================================================




## 中小团队技术选型

#### 发布/部署

- [中小团队技术选型](#%E4%B8%AD%E5%B0%8F%E5%9B%A2%E9%98%9F%E6%8A%80%E6%9C%AF%E9%80%89%E5%9E%8B)
    - [发布/部署](#%E5%8F%91%E5%B8%83%E9%83%A8%E7%BD%B2)
    - [docker](#docker)
    - [配置中心](#%E9%85%8D%E7%BD%AE%E4%B8%AD%E5%BF%83)
    - [SQL自动审核工具](#sql%E8%87%AA%E5%8A%A8%E5%AE%A1%E6%A0%B8%E5%B7%A5%E5%85%B7)
- [Java](#java)
    - [awesome](#awesome)
    - [源码学习](#%E6%BA%90%E7%A0%81%E5%AD%A6%E4%B9%A0)
    - [学习案例](#%E5%AD%A6%E4%B9%A0%E6%A1%88%E4%BE%8B)
    - [开发手册](#%E5%BC%80%E5%8F%91%E6%89%8B%E5%86%8C)
    - [Lib](#lib)
    - [框架](#%E6%A1%86%E6%9E%B6)
    - [tools-监控](#tools-%E7%9B%91%E6%8E%A7)
    - [JVM](#jvm)
- [前端](#%E5%89%8D%E7%AB%AF)
- [数据库](#%E6%95%B0%E6%8D%AE%E5%BA%93)
- [AI算法](#ai%E7%AE%97%E6%B3%95)
- [22待整理](#22%E5%BE%85%E6%95%B4%E7%90%86)

#### docker

> ----------运维咖啡吧
> https://mp.weixin.qq.com/s/xnBehfSlZ3J02xb0GFuGDw
背景介绍
那年公司快速成长，频繁上线新项目，每上线一个项目，就需要新申请一批机器，初始化，部署依赖的服务环境，一个脚本行天下
那年项目发展如火如荼，A项目流量暴增马上给A扩机器，B项目上线新功能又要扩容B，上线新项目没资源了，就先下线处于流量低峰的C项目主机
每天日夜加班，疲于奔命
那年得知了Docker能拯救我于水火，遂决定为了荣誉（发际线）而战。
为了快速落地以及尽量降低引入Docker对整个CICD流程的影响，用最小的改动把Docker加入到了我们上线的流程中，流程变化参考下图
![](https://mmbiz.qpic.cn/mmbiz_png/s0ib4cHvBPB92uq5ibUINQYLbx46O7j6RkVO4I3VtTPqnmBeOM4T9CDz4iaT9GGBvF9hKTNicllfxR3ibXlZibhXA4aA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

#### 配置中心

> ----------中小团队落地配置中心详解 - 云+社区 - 腾讯云
> https://cloud.tencent.com/developer/article/1380942

#### SQL自动审核工具

> 【Inception-SQL自动审核工具】
> 
> ----------中小团队快速构建SQL自动审核系统：：运维咖啡吧
> https://mp.weixin.qq.com/s?__biz=MzU5MDY1MzcyOQ==&mid=2247483715&idx=1&sn=0afbe6ae23c9b052b70d11cf441775ca&scene=21#wechat_redirect
SQL审核与执行，作为DBA日常工作中相当重要的一环，一直以来我们都是通过人工的方式来处理，效率低且质量没办法保证。为了规范操作，提高效率，我们决定引入目前市面上非常流行的SQL自动审核工具Inception。
>
>github：https://github.com/mysql-inception/inception
官方文档：http://mysql-inception.github.io/inception-document
Inception是一个开源的Mysql自动化工具，具有SQL审核、执行、回滚等实用的功能，由国内大神基于mysql源码开发，可以很明确的，详细的，准确的审核Mysql的SQL语句，工作模式与Mysql完全相同，可以直接使用mysql客户端来连接。但遗憾的是2年前已停止更新，不过兼容大部分的mysql版本，仍然是开源SQL审核工具的翘楚。




==================================================

## Java

#### awesome

> 【JavaGuide: Java学习+面试指南】
> 
> ----------Snailclimb/JavaGuide: 【Java学习+面试指南】 一份涵盖大部分Java程序员所需要掌握的核心知识。
> https://github.com/Snailclimb/JavaGuide
【Java学习+面试指南】 一份涵盖大部分Java程序员所需要掌握的核心知识。 https://github.com/Snailclimb/JavaGuide


> 【awesome-java】
> 
> ----------akullpp/awesome-java: A curated list of awesome frameworks, libraries and software for the Java programming language.
> https://github.com/akullpp/awesome-java
作者将JAVA中那些最常用的第三方库按照分类整理成了一个列表。包含Ancients(古老，但常用的)，Bean Mapping，Build，Bytecode Manipulation，Code Analysis，Command-line Argument Parsers，Configuration，Continuous Integration，CSV，Database等等，简直是一本jiava第三方库大全，如果你对项目中应该使用哪一个库不确定，或希望选择几个库来做比较，都可以到awesome-java上进行参考。



+ [weiweifan/Big-Data-Resources](https://github.com/weiweifan/Big-Data-Resources): 大数据/数据挖掘/推荐系统/机器学习相关资源
+ [onurakpolat/awesome-bigdata](https://github.com/onurakpolat/awesome-bigdata): A curated list of awesome big data frameworks, ressources and other awesomeness.
+ [bulutyazilim/awesome-datascience](https://github.com/bulutyazilim/awesome-datascience)：An awesome Data Science repository to learn and apply for real world problems.
+ [MaximAbramchuck/awesome-interview-questions: A curated awesome list of lists of interview questions. Feel free to contribute!](https://github.com/MaximAbramchuck/awesome-interview-questions)

+ [Search · topic:awesome](https://github.com/search?q=topic%3Aawesome&type=Repositories)
+ [sindresorhus/awesome](https://github.com/sindresorhus/awesome): Curated list of awesome lists(6w star+)
+ [lyfeyaj/awesome-resources](https://github.com/lyfeyaj/awesome-resources): Awesome resources for coding and learning: open source projects, websites, books e.g.


#### 源码学习

> + [芋道源码 —— 纯源码解析博客(愿半生编码，如一生老友！)](http://www.iocoder.cn/)




#### 学习案例

https://github.com/JeffLi1993/springboot-learning-example
spring boot 实践学习案例，是 spring boot 初学者及核心技术巩固的最佳实践。

> 【99-Problems】
> 
> ----------shekhargulati/99-problems: This is an adaptation of the Ninety-Nine Prolog Problems written by Werner Hett.
> https://github.com/shekhargulati/99-problems
99-Problems是一个很有意思的GitHub项目，它对三种不同的语言Java 8,Scala和Haskell分别提出了99个问题，让你通过使用特定语言编程来提供一个最优的解决方案。
这些问题分为不同的难度等级，用*表示，一个星号表示在15分钟内解决，2个星号可能需要30-69分钟，而最难的3个星号，则需要更长时间（90分钟左右），如果你能在限定的时间内使用JAVA8的特性解决所有的问题，那说明你对JAVA8的掌握程度已经非常牢固了。如果你没办法解决所有问题也没关系，你可以查看作者提供的代码示例，这也是你学习JAVA8很好的途径。

#### 开发手册

> 阿里开发规范

> 唯品会Java开发手册，结合唯品会的内部经验，参考《阿里巴巴Java开发手册》《Clean Code》、《Effective Java》等重磅资料进行了大幅定制，包含核心基础类库VJKit ，问题排查工具VJMap 和 VJTop 三部分。
https://github.com/vipshop/vjtools


#### Lib

> ----------GitHub 上那些值得一试的 Java 开源库 - arthur.dy.lee的专栏 - CSDN博客
> https://blog.csdn.net/paincupid/article/details/51923284
Strmen-java是一个字符串处理工具，你可以通过maven将它引入到项目中。除了Java本身的字符串处理方式外，我们还可以使用Apache Common Langs里的StringUtils来简化String的操作。但以上两种方式对于我们日常编程中最容易碰到的字符串处理来说，仍然显得有些不足。Strmen-java为我们提供了一个非常完整且强大的解决方案，使用它可以解决几乎所有字符串处理场景。


> NullAway 是 Uber 开源的一款帮助你清除 Java 代码中的 NullPointerException（NPE）的工具，快速且实用。NullAway 类似于 Kotlin 和 Swift 语言中的基于类型的可空性检查，能显着提高开发人员的生产力，同时也满足高要求的安全检查需求。
https://github.com/uber/NullAway


#### 框架

> Nacos是一个易于使用的平台，旨在实现动态服务发现，配置和服务管理。它可以帮助开发者轻松构建云本机应用程序和微服务平台。
https://github.com/alibaba/nacos


#### tools-监控

> 【Automon-JAVA监控工具】
> 
> ----------stevensouza/automon: Automon combines the power of AOP (AspectJ) with monitoring or logging tools you already use to declaratively monitor your Java code, the JDK, and 3rd party libraries.
> https://github.com/stevensouza/automon
Automon是一个非常灵活的JAVA监控工具，它结合了AOP(AspectJ)以及JDK和其他依赖库的功能特性，以声明方式去监控你的Java代码。它可以与JAMon，JavaSimon，Yammer Metrics，StatsD和像 perf4j,log4j,sl4j这样的logging库结合使用。
Automon最常被用于跟踪**Java方法的调用时长，异常次数**等信息，并在你选择的工具中显示监控结果。它并不自己进行任何监控动作，但却很好地扮演了“我应该监控什么”以及“我如何进行监控”这两者之间中间人的角色。而且它的安装也非常简单，只需要简单进行配置便可使用。


> 【Gumshoe - Java程序检测】
> 
> ----------GitHub 上那些值得一试的 Java 开源库 - arthur.dy.lee的专栏 - CSDN博客
> https://blog.csdn.net/paincupid/article/details/51923284
Gumshoe - Java程序检测
Gumshoe是一个JAVA程序检测工具，它能帮助你跟踪程序的负载和性能。它能通过度量TCP,UDP,CPU使用等信息，帮助你分析出资源的使用情况 ，同时它也提供了Java程序中调用栈的分析功能，比如提供某个方法调用的次数，频度等信息。




> 【LeakCanary - 内存泄漏监控】
> 
> ----------GitHub 上那些值得一试的 Java 开源库 - arthur.dy.lee的专栏 - CSDN博客
> https://blog.csdn.net/paincupid/article/details/51923284
LeakCanary - 内存泄漏监控
内存泄漏一直是令Java程序员苦恼的问题，因为在你开发阶段很难察觉内存泄漏问题，而一旦到了生产环境，则可能因为它而造成严重的后果。LeakCanary是一个内存泄漏检查工具，只需要像下面这样简单加入LeakCanary，它便能全程监控你的应用，并在出现内存泄漏时给你发出警告。LeakCanary同时支持Android和Java，下面是在Android应用中使用的例子。




#### JVM


> 【JarsLink (原名 Titan ) -基于 Java 的**模块化**开发框架】
> 
>https://github.com/alibaba/jarslink Star 21058
JarsLink (原名 Titan ) 是一个基于 Java 的模块化开发框架，它提供在运行时动态加载模块（一个 Jar 包）、卸载模块和模块间调用的 API。目前蚂蚁金服微贷事业部几个系统和几十个模块已经使用JarsLink框架。

> 【Swiss Java Knife(**SJK**) - JAVA工具集】
> 
> ----------aragozin/jvm-tools: Small set of tools for JVM troublshooting, monitoring and profiling.
> https://github.com/aragozin/jvm-tools
SJK（Java瑞士军刀）是一个用于JVM监控、排错以及调优的工具集。它是一个命令行工具，但使用起来非常方便，你可以用它来**查询JVM中线程的CPU使用，GC实时信息**，以及基本调优选项。也可以结合MBean以JSON格式导出所有你需要的信息。


> bytecodeviewer是一款简单易用功能强大的反编译软件。
> 它是一款基于图形界面的Java反编译器，Java字节码编辑器，APK编辑器，Dex编辑器，APK反编译器，DEX反编译器。不仅如此，它还是一款Hex查看器，代码搜索器和代码调试器。除此之外，它还具备Smali和Baksmali等汇编器的相关功能。


> Graal 是一个用 Java 编写的新的 JVM 即时编译器，集成到 HotSpot 虚拟机，侧重性能和语言互操作性。Graal 为 Java 代码提供性能优势，这得益于方法内联、流转对象分配和推理执行等新技术，从而可以实现高性能的脚本语言引擎。
https://github.com/oracle/graal


=======================================================



## 前端

> SmartTable 是一套数据源使用 Ajax 获取数据，并展现成表格与图像的形式，并且支持下载（思路源于talkingdata）的智能表格。开源引入：Bootstrap 3.0，Bootstrap respond (IE解决方案)，Jquery 11.02，dataTables，echarts，table2CSV

=======================================================


## 数据库

> 【Inception-SQL自动审核工具】
> 
> ----------中小团队快速构建SQL自动审核系统：：运维咖啡吧
> https://mp.weixin.qq.com/s?__biz=MzU5MDY1MzcyOQ==&mid=2247483715&idx=1&sn=0afbe6ae23c9b052b70d11cf441775ca&scene=21#wechat_redirect
SQL审核与执行，作为DBA日常工作中相当重要的一环，一直以来我们都是通过人工的方式来处理，效率低且质量没办法保证。为了规范操作，提高效率，我们决定引入目前市面上非常流行的SQL自动审核工具Inception。
>
>github：https://github.com/mysql-inception/inception
官方文档：http://mysql-inception.github.io/inception-document
Inception是一个开源的Mysql自动化工具，具有SQL审核、执行、回滚等实用的功能，由国内大神基于mysql源码开发，可以很明确的，详细的，准确的审核Mysql的SQL语句，工作模式与Mysql完全相同，可以直接使用mysql客户端来连接。但遗憾的是2年前已停止更新，不过兼容大部分的mysql版本，仍然是开源SQL审核工具的翘楚。



> quicksql（360）

> Data Transfer Project 旨在创建一个开源的服务到服务数据可移植平台，以便其网站用户和其他人可以轻松将数据从一个平台迁移到另一个平台。它提供了一个通用框架和生态系统，可接受服务提供商的贡献，以实现数据无缝传输到服务之间。
https://github.com/google/data-transfer-project


> 【Tablesaw - “大数据”】
> 
> ----------GitHub 上那些值得一试的 Java 开源库 - arthur.dy.lee的专栏 - CSDN博客
> https://blog.csdn.net/paincupid/article/details/51923284
Tablesaw - “大数据”
谈到大数据，我们想到的总是Hodoop加上集群部署，但有没有一种更小巧的方式，能让我们在单机上方便地实现大数据的那些功能呢？Tablesaw给我们提供了一种基于内存的高性能大数据解决方案。你可以使用它的API方便地从RDBMS或是CSV中导入数据，然后利用Tablesaw提供的接口对数据进行排序、筛选、分组、map/reduce等操作。
根据文档给出的说明，你将可以在22秒内将500,000,000行（每行4个字段）的数据文件加载到10G的内存中。而查询速度更是达到仅需1-2ms。


==========================================================

## AI算法
。。https://github.com/hankcs/HanLP Star 6273
HanLP是由一系列模型与算法组成的Java工具包，目标是普及自然语言处理在生产环境中的应用。HanLP具备功能完善、性能高效、架构清晰、语料时新、可自定义的特点。在提供丰富功能的同时，HanLP内部模块坚持低耦合、模型坚持惰性加载、服务坚持静态提供、词典坚持明文发布，使用非常方便，同时自带一些语料处理工具，帮助用户训练自己的模型。



=======================================================



## 22待整理

==============================================

//整理到opensource分类，2019-1-25 13:58:19
。。https://github.com/cachecats/coderiver


coderiver 中文名 河码，是一个为程序员和设计师提供项目协作的平台，类似程序员客栈，但主要目的是方便各细分领域人才之间技术交流，共同成长，多人协作完成项目。暂不涉及金钱交易。


。。https://github.com/kdn251/interviews Star 30614


Java工程师面试指南，里面涵盖几乎所有软件工程师面试时会碰到的问题以及答案。


。。Spring Cloud Alibaba 致力于提供微服务开发的一站式解决方案。此项目包含开发分布式应用微服务的必需组件，方便开发者通过 Spring Cloud 编程模型轻松使用这些组件来开发分布式应用服务。通过它，只需要添加一些注解和少量配置，就可以将 Spring Cloud 应用接入阿里微服务解决方案，通过阿里中间件来迅速搭建分布式应用系统。
。。一个小商城。litemall = Spring Boot后端 + Vue管理员前端 + 微信小程序用户前端，由于没有上线，只能在微信开发工具中测试运行
。。https://github.com/crossoverJie/JCSprout Star 17084
这是一个还处于萌芽阶段的 Java 核心知识库。分为常用集合、Java多线程、JVM、分布式相关、常用框架等内容
。。https://github.com/Snailclimb/JavaGuide Star 14726
这是一份Java学习指南，涵盖大部分Java程序员所需要掌握的核心知识

。。https://github.com/iluwatar/java-design-patterns Star 42081
Design patterns 是程序员在设计应用程序或系统时可用来解决常见问题的最佳实践手册。
。。https://github.com/macrozheng/mall Star 3249
mall项目是一套电商系统，包括前台商城系统及后台管理系统，基于SpringBoot+MyBatis实现。 
。。https://github.com/b3log/symphony Star 8931
一款用 Java 实现的现代化社区（论坛/BBS/社交网络/博客）平台。分为社区版和商业版
。。https://github.com/eugenp/tutorials Star 10447
该项目是一系列小而专注的教程，每个教程都涵盖一个明确的开发领域。大多数教程项目都专注于Spring Framework（和Spring Security）。以下技术是重点：core Java，Jackson，HttpClient，Guava。
。。Arthas旨在帮助开发人员解决Java应用程序的生产问题，无需修改代码或重新启动服务器。有了Arthas，你就可以在不重新启动JVM或需要额外的代码更改的情况下实时地对问题进行故障排除。


==============================================
