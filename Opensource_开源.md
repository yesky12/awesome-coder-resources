**目录：**


- [1）SQL数据库相关(ORM/DBA...)](#1sql%E6%95%B0%E6%8D%AE%E5%BA%93%E7%9B%B8%E5%85%B3ormdba)
  - [数据库客户端](#%E6%95%B0%E6%8D%AE%E5%BA%93%E5%AE%A2%E6%88%B7%E7%AB%AF)
  - [数据库服务器](#%E6%95%B0%E6%8D%AE%E5%BA%93%E6%9C%8D%E5%8A%A1%E5%99%A8)
  - [数据生成(mock)](#%E6%95%B0%E6%8D%AE%E7%94%9F%E6%88%90mock)
  - [DBA(数据库自动化运维平台)](#dba%E6%95%B0%E6%8D%AE%E5%BA%93%E8%87%AA%E5%8A%A8%E5%8C%96%E8%BF%90%E7%BB%B4%E5%B9%B3%E5%8F%B0)
    - [元数据管理](#%E5%85%83%E6%95%B0%E6%8D%AE%E7%AE%A1%E7%90%86)
    - [自助权限申请](#%E8%87%AA%E5%8A%A9%E6%9D%83%E9%99%90%E7%94%B3%E8%AF%B7)
    - [SQL自动审核](#sql%E8%87%AA%E5%8A%A8%E5%AE%A1%E6%A0%B8)
    - [数据库迁移/同步](#%E6%95%B0%E6%8D%AE%E5%BA%93%E8%BF%81%E7%A7%BB%E5%90%8C%E6%AD%A5)
- [2）NoSQL数据库相关(redis/mongoDB/ES...)](#2nosql%E6%95%B0%E6%8D%AE%E5%BA%93%E7%9B%B8%E5%85%B3redismongodbes)
  - [redis](#redis)
    - [客户端](#%E5%AE%A2%E6%88%B7%E7%AB%AF)
      - [Redis 操作工具包](#redis-%E6%93%8D%E4%BD%9C%E5%B7%A5%E5%85%B7%E5%8C%85)
      - [两级缓存框架](#%E4%B8%A4%E7%BA%A7%E7%BC%93%E5%AD%98%E6%A1%86%E6%9E%B6)
    - [服务器](#%E6%9C%8D%E5%8A%A1%E5%99%A8)
    - [运维/监控](#%E8%BF%90%E7%BB%B4%E7%9B%91%E6%8E%A7)
- [3）Java相关](#3java%E7%9B%B8%E5%85%B3)
  - [特别推荐](#%E7%89%B9%E5%88%AB%E6%8E%A8%E8%8D%90)
  - [awesome-java](#awesome-java)
  - [源码学习](#%E6%BA%90%E7%A0%81%E5%AD%A6%E4%B9%A0)
  - [教育培训](#%E6%95%99%E8%82%B2%E5%9F%B9%E8%AE%AD)
  - [开发手册](#%E5%BC%80%E5%8F%91%E6%89%8B%E5%86%8C)
  - [Lib](#lib)
  - [Java数据库开发](#java%E6%95%B0%E6%8D%AE%E5%BA%93%E5%BC%80%E5%8F%91)
    - [ORM](#orm)
      - [MyBatis](#mybatis)
      - [Stream API方式操作数据库](#stream-api%E6%96%B9%E5%BC%8F%E6%93%8D%E4%BD%9C%E6%95%B0%E6%8D%AE%E5%BA%93)
      - [其它ORM框架](#%E5%85%B6%E5%AE%83orm%E6%A1%86%E6%9E%B6)
    - [数据库连接池](#%E6%95%B0%E6%8D%AE%E5%BA%93%E8%BF%9E%E6%8E%A5%E6%B1%A0)
    - [数据库中间件](#%E6%95%B0%E6%8D%AE%E5%BA%93%E4%B8%AD%E9%97%B4%E4%BB%B6)
  - [框架](#%E6%A1%86%E6%9E%B6)
    - [快速开发框架：](#%E5%BF%AB%E9%80%9F%E5%BC%80%E5%8F%91%E6%A1%86%E6%9E%B6)
    - [微服务](#%E5%BE%AE%E6%9C%8D%E5%8A%A1)
  - [tools-代码生成器](#tools-%E4%BB%A3%E7%A0%81%E7%94%9F%E6%88%90%E5%99%A8)
  - [tools-监控](#tools-%E7%9B%91%E6%8E%A7)
  - [JVM](#jvm)
  - [JVM语言](#jvm%E8%AF%AD%E8%A8%80)
    - [Groovy](#groovy)
    - [Kotlin](#kotlin)
    - [Cloujure](#cloujure)
- [运维相关](#%E8%BF%90%E7%BB%B4%E7%9B%B8%E5%85%B3)
    - [Jenkins](#jenkins)
    - [发布/部署](#%E5%8F%91%E5%B8%83%E9%83%A8%E7%BD%B2)
    - [监控](#%E7%9B%91%E6%8E%A7)
    - [docker部署](#docker%E9%83%A8%E7%BD%B2)
    - [配置中心](#%E9%85%8D%E7%BD%AE%E4%B8%AD%E5%BF%83)
- [大数据](#%E5%A4%A7%E6%95%B0%E6%8D%AE)
  - [查询](#%E6%9F%A5%E8%AF%A2)
  - [数据同步](#%E6%95%B0%E6%8D%AE%E5%90%8C%E6%AD%A5)
- [AI算法](#ai%E7%AE%97%E6%B3%95)
- [前端](#%E5%89%8D%E7%AB%AF)
- [中小团队技术选型](#%E4%B8%AD%E5%B0%8F%E5%9B%A2%E9%98%9F%E6%8A%80%E6%9C%AF%E9%80%89%E5%9E%8B)
- [开源网站](#%E5%BC%80%E6%BA%90%E7%BD%91%E7%AB%99)
- [doc文档](#doc%E6%96%87%E6%A1%A3)
- [22待整理](#22%E5%BE%85%E6%95%B4%E7%90%86)

===============================================


## 开源方法论

//
> ----------当当架构部总监张亮：玩转Java开源项目 - 掘金
> https://juejin.im/post/5987e4b26fb9a03c3c14bb57




## awesome汇总




### awesome-list



//
> ----------ramitsurana/awesome-kubernetes: A curated list for awesome kubernetes sources
> https://github.com/ramitsurana/awesome-kubernetes



//
> ----------Awesome_APIs/README-zh.md at master · TonnyL/Awesome_APIs
> https://github.com/TonnyL/Awesome_APIs/blob/master/README-zh.md
这个仓库主要是为开发者收集非常好的 API . 请随意 Star 或 Fork. 有任何评论或者建议? 请让我们知道. 我们欢迎 PR :), 格式参照 awesome 的清单.


//
> ----------hackstoic/golang-open-source-projects: 为互联网IT人打造的中文版awesome-go
> https://github.com/hackstoic/golang-open-source-projects
看过awesome-go项目， 汇总了很多go开源项目。 但是awesome-go收集了太全了， 而且每个项目没有详细描述。 因此我自己根据go语言中文社区提供的资料，还有互联网企业架构设计中的常见组件分类， 共精心挑选了100多个开源项目（项目不限于在github开源的项目）， 分成以下十几个大类。 这个项目可以理解为互联网IT人打造的中文版awesome-go。这个项目初衷是帮助到那些想学习和借鉴优秀golang开源项目， 和在互联网架构设计时期望快速寻找合适轮子的人。





### awesome-Java
//
> ----------crossoverJie/JCSprout: 👨‍🎓 Java Core Sprout : basic, concurrent, algorithm
> https://github.com/crossoverJie/JCSprout
处于萌芽阶段的 Java 核心知识库。

//
> ----------doocs/advanced-java: 😮 互联网 Java 工程师进阶知识完全扫盲
> https://github.com/doocs/advanced-java





//
> ----------jobbole/awesome-java-cn: Java资源大全中文版，包括开发库、开发工具、网站、博客、微信、微博等，由伯乐在线持续更新。
> https://github.com/jobbole/awesome-java-cn
我想很多程序员应该记得 GitHub 上有一个 Awesome - XXX 系列的资源整理。awesome-java 就是 akullpp 发起维护的 Java 资源列表，内容包括：构建工具、数据库、框架、模板、安全、代码分析、日志、第三方库、书籍、Java 站点等等。伯乐在线已经把 awesome-java 资源列表翻成中文后发布于 ImportNew。

Awesome 系列虽然挺全，但基本只对收录的资源做了极为简要的介绍，如果有更详细的中文介绍，对相应开发者的帮助会更大。这也是我们发起这个开源项目的初衷。




//
> ----------aalansehaiyang/technology-talk: 汇总java生态圈常用技术框架、开源中间件，系统架构、项目管理、经典架构案例、数据库、常用三方库、线上运维等知识
> https://github.com/aalansehaiyang/technology-talk
汇总java生态圈常用技术框架、开源中间件，系统架构、项目管理、经典架构案例、数据库、常用三方库、线上运维等知识



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

//
> ----------KotlinBy/awesome-kotlin: A curated list of awesome Kotlin related stuff Inspired by awesome-java.
> https://github.com/KotlinBy/awesome-kotlin





//
> 【list】----------Search · awesome
> https://github.com/search?l=Java&o=desc&q=awesome&s=stars&type=Repositories




//
> ----------Vedenin/useful-java-links: A list of useful Java frameworks, libraries, software and hello worlds examples
> https://github.com/Vedenin/useful-java-links




//
> ----------Blankj/awesome-java-leetcode: LeetCode of algorithms with java solution(updating).
> https://github.com/Blankj/awesome-java-leetcode
我如今是一名 Android Developer，大学的我曾是一名 ACMer，我一直认为数据结构和算法是作为一名程序员必须掌握和善于利用的，为了不让数据结构和算法淡出我的记忆，所以我打算重拾 LeetCode 之 Algorithm，语言选择的是 Java，题库会一点点完善起来，按简单，中等，困难分类，相应难度下按题号排序，源代码在 src 目录中，相关解题都在 note 目录中，想要学习数据结构和算法或打算刷 LeetCode 的小伙伴们欢迎 star 哦。


//
> ----------Java进阶资源汇总 - 阿木侠 - CSDN博客
> https://blog.csdn.net/weixin_36380516/article/details/70196252
Java经过将近**20年**的发展壮大，框架体系已经丰满俱全；从前端到后台到数据库，从智能终端到大数据都能看到Java的身影，个人感觉做后台进要求越来越高，越来越难。
为什么现在Java程序员越来越难做，一是Java框架体系众多，学习成本提高，**每一个细分问题又有很多可选方案**；二是经过移动互联网的洗礼，以前单机单线程那一套行不通了，现在面临的是高并发低延迟，你可能要掌握缓存、分布式、集群、微服务等；物联网时代渐渐到来，将IT行业技能要求推向一个新高度，你的产品要提供7x24小时不间断服务，就像家里的自来水管，打开阀门水不间断流出来。面对成千上万的智能终端上传的海量数据，从数据压缩上传、优化存储、管理、备份防灾、分析利用等方面，要掌握的技能还很多。



+ [weiweifan/Big-Data-Resources](https://github.com/weiweifan/Big-Data-Resources): 大数据/数据挖掘/推荐系统/机器学习相关资源
+ [onurakpolat/awesome-bigdata](https://github.com/onurakpolat/awesome-bigdata): A curated list of awesome big data frameworks, ressources and other awesomeness.
+ [bulutyazilim/awesome-datascience](https://github.com/bulutyazilim/awesome-datascience)：An awesome Data Science repository to learn and apply for real world problems.
+ [MaximAbramchuck/awesome-interview-questions: A curated awesome list of lists of interview questions. Feel free to contribute!](https://github.com/MaximAbramchuck/awesome-interview-questions)

+ [Search · topic:awesome](https://github.com/search?q=topic%3Aawesome&type=Repositories)
+ [sindresorhus/awesome](https://github.com/sindresorhus/awesome): Curated list of awesome lists(6w star+)
+ [lyfeyaj/awesome-resources](https://github.com/lyfeyaj/awesome-resources): Awesome resources for coding and learning: open source projects, websites, books e.g.

//
> ----------graphql-java/awesome-graphql-java: awesome list of graphql-java related projects
> https://github.com/graphql-java/awesome-graphql-java





### awesome-微信开发

//
> ----------opendigg/awesome-github-wechat-weapp: 微信小程序开源项目库汇总
> https://github.com/opendigg/awesome-github-wechat-weapp



//
> ----------justjavac/awesome-wechat-weapp: 微信小程序开发资源汇总 :100:
> https://github.com/justjavac/awesome-wechat-weapp





### awesome-Linux

//
> ----------judasn/Linux-Tutorial: 《Java 程序员眼中的 Linux》
> https://github.com/judasn/Linux-Tutorial


//
> ----------cookieY/bash-step-to-step: bash命令和语法--带你升级打boss
> https://github.com/cookieY/bash-step-to-step

//
> ----------alebcay/awesome-shell: A curated list of awesome command-line frameworks, toolkits, guides and gizmos. Inspired by awesome-php.
> https://github.com/alebcay/awesome-shell

//
> ----------luong-komorebi/Awesome-Linux-Software: A list of awesome applications, software, tools and other materials for Linux distros.
> https://github.com/luong-komorebi/Awesome-Linux-Software





### awesome-数据科学

//
> ----------onurakpolat/awesome-bigdata: A curated list of awesome big data frameworks, ressources and other awesomeness.
> https://github.com/onurakpolat/awesome-bigdata




//
> ----------bulutyazilim/awesome-datascience: An awesome Data Science repository to learn and apply for real world problems.
> https://github.com/bulutyazilim/awesome-datascience

### awesome-算法

//
> ----------apachecn/awesome-algorithm: LeetCode, HackRank, 剑指offer, classic algorithm implementation
> https://github.com/apachecn/awesome-algorithm
LeetCode, HackRank, 剑指offer, classic algorithm implementation

### awesome-book
//
> ----------jobbole/awesome-programming-books: 经典编程书籍大全，涵盖：计算机系统与网络、系统架构、算法与数据结构、前端开发、后端开发、移动开发、数据库、测试、项目与团队、程序员职业修炼、求职面试等
> https://github.com/jobbole/awesome-programming-books





### awesome-前端
//
> ----------jobbole/awesome-javascript-cn: JavaScript 资源大全中文版，内容包括：包管理器、加载器、测试框架、运行器、QA、MVC框架和库、模板引擎等
> https://github.com/jobbole/awesome-javascript-cn



//
> ----------opendigg/awesome-github-vue: Vue相关开源项目库汇总
> https://github.com/opendigg/awesome-github-vue



//
> ----------opendigg/awesome-github-vue: Vue相关开源项目库汇总
> https://github.com/opendigg/awesome-github-vue


//
> ----------JingwenTian/awesome-frontend: A curated list of amazingly awesome frontend libraries, resources and shiny things.
> https://github.com/JingwenTian/awesome-frontend


//
> ----------rohan-paul/Awesome-JavaScript-Interviews: Popular JavaScript / React / Node / Mongo stack Interview questions and their answers. Many of them, I faced in actual interviews over the last few months. And ultimately got my first full-stack Engineer job :)
> https://github.com/rohan-paul/Awesome-JavaScript-Interviews





## 1）SQL数据库相关(ORM/DBA...)




### 数据库客户端

> ----------mysq数据库管理工具navicat基本使用方法 - 师者乐享 - 博客园
> https://www.cnblogs.com/neuedu/p/5876874.html
navicat是mysql数据库的客户端查询管理工具



> ----------DataGrip: 一种工具支持多种数据库
> https://www.jetbrains.com/zh/datagrip/specials/datagrip/datagrip.html?utm_source=baidu&utm_medium=cpc&utm_campaign=cn-bai-br-datagrip-ex-pc&utm_content=datagrip-pure&utm_term=datagrip&gclid=CO6389SJiuACFcd2vAodj1gC_A&gclsrc=ds



> ----------DBeaver免费通用数据库管理器和SQL客户端 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/serge-rider-dbeaver.html
免费的多平台数据库工具，适用于开发人员，SQL程序员，数据库管理员和分析人员。 支持任何具有JDBC驱动程序的数据库（这主要表示ANY数据库）。

> DBeaver 是一个通用的数据库管理工具和 SQL 客户端，
http://blog.51cto.com/12042068/2115077

//
> ----------通过数据库客户端界面工具**DBeaver连接Hive** - 云+社区 - 腾讯云
> https://cloud.tencent.com/developer/article/1176452





### 数据库服务器

> ----------SQLiteToExcel：一个轻量级库用于将SQLite数据库转换为Excel - Java开发社区 | CTOLib码库
> https://www.ctolib.com/SQLite2XL.html

> ----------H2：小型SQL数据库，以可以作为内存数据库使用著称 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/ar-454.html
H2采用Java开发的免费SQL数据库


> Realm是一个用来**替代sqlite**的解决方案，它比sqlite更轻量，同时速度更快，而且使用起来很简单顺手，还跨平台，目前已支持Java，Objective C，Swift，React-Native，Xamarin这五种语言。




### 数据生成(mock)

> ----------基于多数据库的数据生成器 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/ysc-data-generator.html
数据生成器 -- 如果你在从事大数据BI的工作，想对比一下MySQL、GreenPlum、Elasticsearch、Hive、Presto、Impala、Drill、HAWQ、Druid、Pinot、Kylin等不同实现方案之间的表现，那你就需要一份标准的数据进行测试，这个开源项目就是为了生成这样的标准数据。




### DBA(数据库自动化运维平台)

#### 元数据管理

//
> ----------元数据管理的未来趋势——企业级元数据管理（EMM） - xudawenfighting的博客 - CSDN博客
> https://blog.csdn.net/xudawenfighting/article/details/80125648
企业级元数据管理将成为企业信息管理的核心
2011年8月，**Gartner提出了基于企业级元数据管理的信息能力框架(ICF)**，该框架完全独立于使用实例和信息源，不依赖于技术和架构，同时又能考虑到了使用实例的具体细节，解决了之前企业需要根据具体项目、应用和信息类型而开发特定信息管理能力的弊端，避免了由企业信息之间的分裂和脱节引起的不能支持新信息类型问题的出现，逐渐成为企业构建现代信息框架的指导方针，下图是Gartner信息能力框架的详细表示：



//
> ----------数据库自动化运维平台--元数据平台 - 晨夕的博客 - CSDN博客
> https://blog.csdn.net/liuhanran/article/details/70142849#comments
很多DBA可能都用过Excel来维护数据库集群列表，在公司数据库集群规模比较小，用这种方式维护也是很简单方便的。但随着数据实例越来越多达到了上百上千的时候，再用这种方式维护就要崩溃了。所以一旦集群上了规模，每个公司都要开发类似**CMDB的平台来维护集群信息** 。由于本人所在的DBA部门开发资源有限，所以自个也花一个月的时间学习的相关知识，开发了一款MySQL元数据平台，希望能给做平台的朋友一些思路。 本系统主要是内部使用，所以只能展示部分内容。希望大家多多指点。

所涉及的技术点,如下: 
(1)开发语言： python 
(2)框架： Flask 
(3)bootstrap,html,js,css,jquery 
(4)后端存储MySQL

主要功能： 
(1)搜索关业务线下的所有集群实例 
(2)搜索某个端口集群(我们这边一个集群一个端口) 
(3)查看集群概述信息(负责人，归属业务线，用途描述等) 
(4)查看集群实例信息(buffer设置大小 域名 总数据量 所在机房 实例状态等) 
(5)查看集群**库元信息**(库数据量，表数量，字符集，所属项目，归属人等) 
(6)查看**表元信息**(表数据量，行数，索引大小，自增主键使用率等)



#### 自助权限申请

//
> ----------数据库自动化运维平台--自助权限申请 - 晨夕的博客 - CSDN博客
> https://blog.csdn.net/liuhanran/article/details/73289242
客户端程序访问数据库都需要一个**连接数据库**的用户名和密码，这个用户一般是DBA帮RD创建。根据安全级别的不同，每个团队都会有不同的授权方式。我们在用户访问数据库安全方面也制定了一套规则：

(1) 读写账号只能有SELECT，DELETE，UPDATE，INSERT权限。

(2) 用户的白名单IP不能是一个网段，必须是一个IP。

(3) 白名单IP必须是线上的服务器IP，不能是线下测试机IP。

对于白名单IP不能是网段这条规则，可能会给DBA带来很多的工作量。**RD给出几十个IP白名单让DBA授权是常有的事**，并且在手动授权的过程中容易犯错，比如之前就发生过手动授权覆盖已有账号的密码，使得客户端无法连接数据库的故障。

基于以上原因，最近对RD开放了新的运维平台，自助授权申请平台。
![enter image description here](https://img-blog.csdn.net/20170615154216143?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbGl1aGFucmFu/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)
![enter image description here](https://img-blog.csdn.net/20170615163009496?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbGl1aGFucmFu/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)
产生了任务还需要有人审核才行，**审核规则要结合我们的元数据平台**，需要集群负责人审核。
![enter image description here](https://img-blog.csdn.net/20170615164558895?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvbGl1aGFucmFu/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)
总结：
通过平台服务化，使得DBA的工作更有效率，降低重复性工作。﻿﻿

#### SQL自动审核

//
> ----------运维效率之数据迁移自动化 - 云+社区 - 腾讯云
> https://cloud.tencent.com/developer/article/1380939
为什么需要工单？目前的流程都是通过邮件的方式，需求邮件到DBA，DBA执行导数据的操作。自动化的流程理论来说应该从头至尾都无需人工参与，但涉及到数据安全问题，还是需要DBA确认，所以加了工单。同时工单具有状态自助追踪，减少沟通成本等优点，后续也方便统计工单量等指标，以便优化服务与流程。同时为了能够保证工单及时被处理，我们每一步都会增加邮件和IM的通知，给用户最及时的反馈。

数据迁移的工单流程很简单，用户提交工单，DBA进行审核，审核通过系统自动执行迁移操作，审核不通过流程结束。流程图图如下：




//
> ----------基于Inception & Yearning做SQL审核的实践（安装篇） - 简书
> https://www.jianshu.com/p/03e784106003
SQL审核的需求
SQL审核是保证DDL&DML正常使用，不会造成线上事故的重要手段。经研究，来自于去哪儿网的Inception有较大的使用基础，结合一些上层的人机交互系统可以实现SQL审核、执行以及备份和恢复功能。

Inception
Inception是一个自动化运维工具，在Mysql前做一个审核和操作的屏障。跟Inception的交互是程序级别的，即通过Python或其他程序编程实现对Inception的命令调用，并解析结果。

Inception的文档地址：http://mysql-inception.github.io/inception-document/

Yearning
由于Inception是一个基础工具，如果要做SQL审核，系统级的业务操作（提DDL&DML，审核，执行等）还需要一个人机交互的界面，Yearning就是这么一个Python实现的web系统。

Yearning的文档地址：https://cookiey.github.io/Yearning-document/



//
> ----------数据库自动化运维平台--自助DML - 晨夕的博客 - CSDN博客
> https://blog.csdn.net/liuhanran/article/details/70239603
其实很多公司的DBA都是苦逼的，差不多一个DBA要对应几十个甚至上百个开发。半夜爬起来处理故障，上百G的数据动不动搞个迁移,升级等 这些都是很常见的，怪不得很多DBA自嘲”我是搬砖的”。为了使DBA的工作轻松，有效率很多年前各大公司就开始自动化运维平台建设，在这方面我们属于比较晚的了。

今天介绍下最近开发的一个平台，**自助DML**。什么是DML，就是平常执行的增删改查数据库操作。有人有疑问这不是程序访问的操作，为什么还要做一个平台操作这些呢，其实这种操作主要是**开发需要线下修复数据的一种操作，不只是增删改，还有建表，建索引，添加字段等**，这些操作**开发一般会提给DBA协助操作数据库**。可能你会觉得这些活能有多少，其实这种活真不少，我上家公司是电商互联网公司，大概有七八百个实例，每天的这种操作有近百个。处理近百个这种需求，基本上一个人一天就不用干别的了。虽说现在的公司实例少点，但每天的工作量还是很大，关键这种工比较重复，枯燥，没有技术含量，所以迫切需要一个自助的服务平台开放出去来提高工作效率，解放DBA。

其主要功能是审核，审核需要满足几个条件 :  1)操作的集群要有归属业务部门  2)操作库要有归属项目名称和归属人  3)不能自己审核自己提交的任务 4)如果任务提交人跟库归属人不同则需要库归属人审核 5)如果是库归属人提交的任务则需要同部门的另一人审核        (这些条件需要**结合元数据平台**，请参考之前的博客)

 1) 未审核, 没有权限等等都是没有办法执行


> ----------cookieY/Yearning: Mysql web端sql审核平台
> https://github.com/cookieY/Yearning
Mysql web端sql审核平台 http://yearning.io/
> 
> SQL审核
流程化工单
SQL语句检测与执行
SQL回滚
历史审核记录
> 
> 推送
E-mail工单推送
钉钉webhook机器人工单推送
> 
> //用户权限及管理
拼图式权限划分
组合式权限组
支持限制邮箱后缀名的有限注册功能
>
> ![enter image description here](http://yearning.io/img/per.png)
> 
> //DDL
> ![enter image description here](https://guide.yearning.io/images/alter_ddl.png)
> 
> //DML
> ![enter image description here](https://guide.yearning.io/images/sql.png)


//
> ----------cookieY/inception-document: 一个集审核、执行、备份及生成回滚语句于一身的MySQL自动化运维工具之手册部分
> https://github.com/cookieY/inception-document
Inception 是一个集审核、执行、备份及生成回滚语句于一身的MySQL自动化运维工具。由去哪儿网 http://www.qunar.com共享、开源而来。

本项目是 Inception 的手册部分。



> 【Inception-SQL自动审核工具】
> 
> ----------中小团队快速构建SQL自动审核系统：：运维咖啡吧
> https://mp.weixin.qq.com/s?__biz=MzU5MDY1MzcyOQ==&mid=2247483715&idx=1&sn=0afbe6ae23c9b052b70d11cf441775ca&scene=21#wechat_redirect
SQL审核与执行，作为DBA日常工作中相当重要的一环，一直以来我们都是通过人工的方式来处理，效率低且质量没办法保证。为了规范操作，提高效率，我们决定引入目前市面上非常流行的SQL自动审核工具Inception。
>
>github：https://github.com/mysql-inception/inception
官方文档：http://mysql-inception.github.io/inception-document
Inception是一个开源的Mysql自动化工具，具有SQL审核、执行、回滚等实用的功能，由国内大神基于mysql源码开发，可以很明确的，详细的，准确的审核Mysql的SQL语句，工作模式与Mysql完全相同，可以直接使用mysql客户端来连接。但遗憾的是2年前已停止更新，不过兼容大部分的mysql版本，仍然是开源SQL审核工具的翘楚。



> 【Inception-SQL自动审核工具】
> 
> ----------中小团队快速构建SQL自动审核系统：：运维咖啡吧
> https://mp.weixin.qq.com/s?__biz=MzU5MDY1MzcyOQ==&mid=2247483715&idx=1&sn=0afbe6ae23c9b052b70d11cf441775ca&scene=21#wechat_redirect
SQL审核与执行，作为DBA日常工作中相当重要的一环，一直以来我们都是通过人工的方式来处理，效率低且质量没办法保证。为了规范操作，提高效率，我们决定引入目前市面上非常流行的SQL自动审核工具Inception。
>
>github：https://github.com/mysql-inception/inception
官方文档：http://mysql-inception.github.io/inception-document
Inception是一个开源的Mysql自动化工具，具有SQL审核、执行、回滚等实用的功能，由国内大神基于mysql源码开发，可以很明确的，详细的，准确的审核Mysql的SQL语句，工作模式与Mysql完全相同，可以直接使用mysql客户端来连接。但遗憾的是2年前已停止更新，不过兼容大部分的mysql版本，仍然是开源SQL审核工具的翘楚。


> Data Transfer Project 旨在创建一个开源的服务到服务数据可移植平台，以便其网站用户和其他人可以轻松将数据从一个平台迁移到另一个平台。它提供了一个通用框架和生态系统，可接受服务提供商的贡献，以实现数据无缝传输到服务之间。
https://github.com/google/data-transfer-project





#### 数据库迁移/同步

> ----------Flyway：简单的Java数据库迁移工具 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/flyway.html


>【canal：跨机房同步】
> 
> ----------阿里巴巴mysql数据库binlog的增量订阅&消费组件 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/canal.html
早期，阿里巴巴B2B公司因为存在杭州和美国双机房部署，存在跨机房同步的业务需求。不过早期的数据库同步业务，主要是基于trigger的方式获取增量变更，不过从2010年开始，阿里系公司开始逐步的尝试基于数据库的日志解析，获取增量变更进行同步，由此衍生出了增量订阅&消费的业务，从此开启了一段新纪元。


> ----------DataLink是一个满足各种异构数据源之间的实时增量同步，分布式、可扩展的数据交换平台 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/ucarGroup-DataLink.html
> DataLink是这样一个产品：
> 
> 满足各种异构数据源之间的实时增量同步
平台提供统一的基础设施（高可用、动态负载、同步任务管理、插件管理、监控报警、公用业务组件等等），让设计人员专注于同步插件开发，一次投入，长久受益
> 
> 吸收、整合业内经验，在架构模型、设计方法论、功能特性、可运维、易用性上进行全面的升级，在前瞻性和扩展性上下足功夫，满足未来5-10年内的各种同步需求
> 
> DataLink开发时间从2016年12月开始，第一版于2017年5月份上线，在神州优车集团服役到现在，基本上满足了公司所有业务线的同步需求。此次外部开源版本为去除内部依赖后的版本。
> 
> 目前同步规模：
日均数据同步量800G+
涉及272个数据库实例之间的3208个同步映射
60台Worker+2台Manager机器的集群规模







## 2）NoSQL数据库相关(redis/mongoDB/ES...)

### redis


#### 客户端

##### Redis 操作工具包

> ----------jedis：Redis的Java客户端 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/jedis.html

> ----------lettuce - 高级Java Redis客户端，用于线程安全同步，异步和reactive用法 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/lettuce-io-lettuce-core.html

> 【Spring Data Redis】
> 
> ----------它提供了 Spring 应用对 Redis 的简单配置和访问 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/spring-data-redis.html
Spring Data Redis, 是 Spring Data 家族的子项目。它提供了 Spring 应用对 Redis 的简单配置和访问。低级和高级的抽象用于存储，使用户无需考虑考虑基础。

> ----------jedipus 是一个 Redis 3.2 + Java 8 客户端和命令行执行器 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/jedipus.html
jedipus 是一个 Redis 3.2 + Java 8 客户端，用于管理客户端对象池和命令执行。 特点： 1.可使用Consumer<RedisClient> 和Function<RedisClient, R>执行lambda 2.灵活的泛型和初始返回类型会匹配Redis动态的返回类型。

> ----------Redis 操作工具包分装。单点、哨兵、cluster均支持。简单配置即可使用 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/sudo168-redis-helper.html
redisHelper.cmd().set("name", "lisi");


##### 两级缓存框架

> ----------J2Cache: Java **两级缓存框架**，可以让应用支持两级缓存框架 ehcache(Caffeine) + redis 。避免完全使用独立缓存系统所带来的网络IO开销问题
> https://gitee.com/ld/J2Cache
J2Cache 是 OSChina 目前正在使用的两级缓存框架（要求至少 Java 8）。第一级缓存使用内存(同时支持 Ehcache 2.x、Ehcache 3.x 和 Caffeine)，第二级缓存使用 Redis(推荐)/Memcached 。 由于大量的缓存读取会导致 L2 的网络成为整个系统的瓶颈，因此 L1 的目标是降低对 L2 的读取次数。 该缓存框架主要用于集群环境中。单机也可使用，用于避免应用重启导致的缓存冷启动后对后端业务的冲击。




#### 服务器
> ----------**Redisson** - 构建在Redis服务器之上的分布式可扩展Java数据结构 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/redisson.html

> ----------**Redis集群**方案之使用豌豆荚Codis搭建（待实践） - EasonJim - 博客园
> https://www.cnblogs.com/EasonJim/p/7630405.html




#### 运维/监控

//
> ----------redis 一站式管理平台，支持集群创建、管理、监控 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/ngbdf-redis-manager.html




> ----------CacheCloud:搜狐视频的CacheCloud提供一个Redis云管理平台 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/cachecloud.html
CacheCloud提供一个Redis云管理平台：实现多种类型(Redis Standalone、Redis Sentinel、Redis Cluster)自动部署、解决Redis实例碎片化现象、提供完善统计、监控、运维功能、减少运维成本和误操作，提高机器的利用率，提供灵活的伸缩性，提供方便的接入客户端。
> 3. 监控、统计和管理不完善
       一些开源的Redis监控和管理工具，例如：RedisLive(Python)、Redis Commander(Node.js)，Redmon(Ruby)无论从功能的全面性(例如配置管理，支持Redis-Cluster等等)、扩展性很难满足需求。
>
>4. 运维成本
       Redis的使用者需要维护各自的Redis，但是用户可能更加善于使用Redis实现各种功能，但是没有足够的精力和经验维护Redis。Redis的开发人员如同使用MySQL一样，不需要运维Mysql服务器，同样使用Redis服务，不要自己运维Redis，Redis由一些在Redis运维方面更有经验的人来维护（保证高可用，高扩展性），使得开发者更加关注于Redis使用本身。

> ----------基于SpringBoot开发的redis缓存数据图形化管理工具 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/xuebus-redis-admin.html
一个简单好用的redis缓存图形化管理工具，包含redis的5种数据类型的CRUD操作; 由于该系统是在大名鼎鼎的JeeSite基础之上开发的，所有保留了原系统的用户/角色/权限/菜单等模块.





==================================================

## 3）Java相关



### 特别推荐

> 特别推荐：apiJSON，EOVA，CBoard

> 分布式开源程序：mall，zheng



### 源码学习

> + [芋道源码 —— 纯源码解析博客(愿半生编码，如一生老友！)](http://www.iocoder.cn/)


//
> ----------macrozheng/mall: mall项目是一套电商系统，包括前台商城系统及后台管理系统，基于SpringBoot+MyBatis实现。 前台商城系统包含首页门户、商品推荐、商品搜索、商品展示、购物车、订单流程、会员中心、客户服务、帮助中心等模块。 后台管理系统包含商品管理、订单管理、会员管理、促销管理、运营管理、内容管理、统计报表、财务管理、权限管理、设置等模块。
> https://github.com/macrozheng/mall
> http://39.98.190.128/index.html




https://github.com/JeffLi1993/springboot-learning-example
spring boot 实践学习案例，是 spring boot 初学者及核心技术巩固的最佳实践。

> 【99-Problems】
> 
> ----------shekhargulati/99-problems: This is an adaptation of the Ninety-Nine Prolog Problems written by Werner Hett.
> https://github.com/shekhargulati/99-problems
99-Problems是一个很有意思的GitHub项目，它对三种不同的语言Java 8,Scala和Haskell分别提出了99个问题，让你通过使用特定语言编程来提供一个最优的解决方案。
这些问题分为不同的难度等级，用*表示，一个星号表示在15分钟内解决，2个星号可能需要30-69分钟，而最难的3个星号，则需要更长时间（90分钟左右），如果你能在限定的时间内使用JAVA8的特性解决所有的问题，那说明你对JAVA8的掌握程度已经非常牢固了。如果你没办法解决所有问题也没关系，你可以查看作者提供的代码示例，这也是你学习JAVA8很好的途径。


### 教育培训

//
> ----------开发10年，全记在这本Java进阶宝典里了 - 简书
> https://www.jianshu.com/p/428251ede1aa
![enter image description here](https://upload-images.jianshu.io/upload_images/10299630-b467fc172d9be65a.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/840/format/webp)


### 开发手册

> 阿里开发规范

> 唯品会Java开发手册，结合唯品会的内部经验，参考《阿里巴巴Java开发手册》《Clean Code》、《Effective Java》等重磅资料进行了大幅定制，包含核心基础类库VJKit ，问题排查工具VJMap 和 VJTop 三部分。
https://github.com/vipshop/vjtools


### Lib

> ----------GitHub 上那些值得一试的 Java 开源库 - arthur.dy.lee的专栏 - CSDN博客
> https://blog.csdn.net/paincupid/article/details/51923284
Strmen-java是一个字符串处理工具，你可以通过maven将它引入到项目中。除了Java本身的字符串处理方式外，我们还可以使用Apache Common Langs里的StringUtils来简化String的操作。但以上两种方式对于我们日常编程中最容易碰到的字符串处理来说，仍然显得有些不足。Strmen-java为我们提供了一个非常完整且强大的解决方案，使用它可以解决几乎所有字符串处理场景。


> NullAway 是 Uber 开源的一款帮助你清除 Java 代码中的 NullPointerException（NPE）的工具，快速且实用。NullAway 类似于 Kotlin 和 Swift 语言中的基于类型的可空性检查，能显着提高开发人员的生产力，同时也满足高要求的安全检查需求。
https://github.com/uber/NullAway



### Java数据库开发



> 【list】----------数据库相关工具 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/java/categories/java-database.html
数据库相关工具 - **简化**数据库交互的Java相关工具


#### ORM

##### MyBatis


//
> ----------wuhao000/mybatis-xmlless-spring-starter: 使用这个项目，你基本可以不用写Mybatis的xml文件了，它可以自动推断sql（不是生成），既可以完成简单的增删改查，也可以支持复杂的连表查询
> https://github.com/wuhao000/mybatis-xmlless-spring-starter
如果你对于写mapper文件非常厌恶，那么这个项目非常适合你
``` 
【mybatis-xmlless-spring-starter】
----------使用这个项目，你基本可以不用写Mybatis的xml文件了 - Java开发社区 | CTOLib码库
https://www.ctolib.com/wuhao000-mybatis-xmlless-spring-starter.html

sql推断名称与方法名称隔离
在mapper方法上使用@ResolvedName注解，该注解的必选参数name将会代替方法名称作为推断sql的名称，这样可以让方法名称更具语义化

例如

@ResolvedName("findIdAndNameAndAge")
fun findSimpleInfoList(): List<User>

//
指定方法获取的属性集合
使用 @SelectedProperties注解

例如

@SelectedProperties(properties=["id", "name", "age"])
fun findSimpleInfoList(): List<User>

```


> ----------Mybatis 增强工具包 - 只做增强不做改变，简化CRUD操作 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/baomidou-mybatis-plus.html

> ----------Mybatis通用分页插件 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/pagehelper-Mybatis-PageHelper.html


> ----------MyBatisCodeHelper是Intellij下mybatis相关代码自动生成插件 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/MyBatisCodeHelper.html
Intellij下代码自动生成插件 支持生成mybatis的dao接口,mapper xml,和建表sql, 支持直接从接口方法名直接生成sql.

> ----------mybatis 自动生成代码web工具 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/generator-web.html
mybatis文件在线自动生成器-让机械无味的mybatis文件编写工作一去不返 随时随地 - 方便快捷


> ----------MyBatis-CMEU是基于javafx8开发的一款图形界面的Mybatis逆向工程; - Java开发社区 | CTOLib码库
> https://www.ctolib.com/shenzhenMirren-MyBatis-CMEU.html


> ----------perseus：基于 Mybatis + Spring 的读写分离方案 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/chengdedeng-perseus.html



> + ----------扩展mybatis-generator插件;高效率分页查询,自动添加swagger2注解到实体类 - Java开发社区 | CTOLib码库
>https://www.ctolib.com/MisterChangRay-mybatis-generator-plugins.html
```
1. 自动添加swagger2注解到实体类
自动为entity类生成swagger2文档注解，注解内容为数据库comment内容

        <!-- 自动为entity生成swagger2文档-->
        <plugin type="mybatis.generator.plugins.GeneratorSwagger2Doc">
          <property name="apiModelAnnotationPackage" value="io.swagger.annotations.ApiModel" />
          <property name="apiModelPropertyAnnotationPackage" value="io.swagger.annotations.ApiModelProperty" />
        </plugin>
```



##### Stream API方式操作数据库

> ----------Speedment：一个数据库访问库它利用了Java 8 Stream API进行查询 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/speedment.html
Speedment：一个数据库访问库它利用了Java 8 Stream API进行查询


> ----------【Anima】🍶 像 Stream API 那样操作数据库 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/biezhi-anima.html

```
Query
long count = select().from(User.class).count();
// SELECT COUNT(*) FROM users

long count = select().from(User.class).where("age > ?", 15).isNotNull("user_name").count();
// SELECT COUNT(*) FROM users WHERE age > ? AND user_name IS NOT NULL

User user = select().from(User.class).byId(2);
// SELECT * FROM users WHERE id = ?

List<User> users = select().from(User.class).byIds(1, 2, 3);
// SELECT * FROM users WHERE id IN (?, ?, ?)

String name = select().bySQL(String.class, "select user_name from users limit 1").one();

List<String> names = select().bySQL(String.class, "select user_name from users limit ?", 3);

List<User> users = select().from(User.class).all();
// SELECT * FROM users

List<User> users = select().from(User.class).like("user_name", "%o%").all();
// SELECT * FROM users WHERE user_name LIKE ?

```



##### 其它ORM框架

> 【list】----------ORM框架 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/categories/java-orm-pg-2.html


> ----------MyBatis：支持定制化 SQL、存储过程以及高级映射的优秀的持久层框架 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/mybatis-3.html

> ----------jOOQ：构建类型安全的SQL查询 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/jOOQ.html
jOOQ从数据库产生Java代码，并允许您通过其流畅API构建类型安全的SQL查询。




#### 数据库连接池

> ----------Druid是Java语言中最好的数据库连接池。Druid能够提供强大的监控和扩展功能。 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/druid.html




#### 数据库中间件


> ----------| MYCAT官方网站—中国第一开源分布式数据库中间件
> http://www.mycat.io/


> ----------Ctrip DAL是携程框架部开发的数据库访问框架 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/dal.html
Ctrip DAL是携程框架部开发的数据库访问框架，支持代码生成和水平扩展。其由携程技术中心框架部DAL团队开发，历经3年不断打磨，并在长期的实际使用中基于大量的用户反馈不断优化。



> ----------分表分库的新思路——服务层Sharding框架 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/QNJR-GROUP-sharding-method.html
分表分库的新思路——服务层Sharding框架，全SQL、全数据库兼容，ACID特性与原生数据库一致，能实现RR级别读写分离，无SQL解析性能更高






### 框架



#### 快速开发框架：

> JFinal，

> nutz，


#### 微服务

> Nacos是一个易于使用的平台，旨在实现动态服务发现，配置和服务管理。它可以帮助开发者轻松构建云本机应用程序和微服务平台。
https://github.com/alibaba/nacos



### tools-代码生成器

> ----------Spring-generator是基于javafx8开发的图形界面Spring代码生成器 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/EliMirren-Spring-generator.html





### tools-监控

> + MBean

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




### JVM


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



### JVM语言

> ----------Groovy，Clojure和Kotlin都是基于jvm的语言，那他们在实际项目中的运用场景有什么区别？ - 知乎
> https://www.zhihu.com/question/29818569?sort=created

#### Groovy


#### Kotlin

#### Cloujure

> ----------Toucan 一个优雅的高级Clojure库，用于定义应用程序模型并从DB中检索它们 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/toucan.html




=================================================================



## 运维相关


#### Jenkins

>Jenkinsfile Runner - 将**Jenkins管道执行封装为命令行工具**的实验 https://www.ctolib.com/kohsuke-jenkinsfile-runner.html

>初试**Jenkins2.0 Pipeline**持续集成 - 哎_小羊的博客 - CSDN博客https://blog.csdn.net/aixiaoyang168/article/details/72818804
先介绍下什么是Jenkins 2.0，**Jenkins 2.0的精髓是Pipeline as Code**，是帮助Jenkins实现CI到CD转变的重要角色。什么是Pipeline，简单来说，就是一套运行于Jenkins上的工作流框架，将原本独立运行于单个或者多个节点的任务连接起来，实现单个任务难以完成的复杂发布流程。Pipeline的实现方式是一套Groovy DSL，任何发布流程都可以表述为一段Groovy脚本，并且Jenkins支持从代码库直接读取脚本，从而实现了Pipeline as Code的理念。 Pipeline的几个基本概念： Stage: 阶段，一个Pipeline可以划分为若干个Stage，每个Stage代表一组操作。注意，Stage是一个逻辑分组的概念，可以跨多个Node。 Node: 节点，一个Node就是一个Jenkins节点，或者是Master，或者是Agent，是执行Step的具体运行期环境。 Step: 步骤，Step是最基本的操作单元，小到创建一个目录，大到构建一个Docker镜像，由各类Jenkins Plugin提供。 


#### 发布/部署

> ----------walle 2.0 瓦力 | walle 瓦力 - 部署系统
> http://walle-web.io/docs/
walle 让用户代码发布终于可以不只能选择 jenkins！支持各种web代码发布，php、java、python、go等代码的发布、回滚可以通过web来一键完成。walle 一个可自由配置项目，更人性化，高颜值，支持git、多用户、多语言、多项目、多环境同时部署的开源上线部署系统。

#### 监控

//
> ----------使用Nagios打造专业的业务状态监控 - 云+社区 - 腾讯云
> https://cloud.tencent.com/developer/article/1380948

//
> ----------prometheus监控spark on yarn方案（一） - 简书
> https://www.jianshu.com/p/afb308418500





#### docker部署

//
> ----------Jib - 一个能够很方便为Java应用程序构建Docker和OCI容器镜像 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/GoogleContainerTools-jib.html
Jib是一个快速而简单的容器镜像构建工具，它负责处理将应用程序打包到容器镜像中所需的所有步骤。它不需要你编写 Dockerfile或安装 Docker，而且可以直接集成到 Maven和 Gradle中——只需要将插件添加到构建中，就可以立即将 Java应用程序容器化。



> ----------从Jenkins迁移到Jenkins X：一场持续交付之旅：：高效开发运维
> https://mp.weixin.qq.com/s/yq7cBZJiTd_TlafNuX17WA
Jenkins X 是一个高度集成化的 CI/CD 平台，基于 Jenkins 和 Kubernetes 实现，旨在解决微服务体系架构下的云原生应用的持续交付的问题




> ----------探秘varian：优雅的发布部署程序：：运维咖啡吧
> https://mp.weixin.qq.com/s?__biz=MzU5MDY1MzcyOQ==&mid=2247483730&idx=1&sn=435c10f8c1ec6938f80b0e7d814dfdcd&scene=21#wechat_redirect
varian是我们基于Python3编写的一套部署程序，处在整个部署系统的中心，与CMDB、Jenkins、SVN/Git、镜像仓库Harbor、Kubernetes API、通知系统等都有交互，负责将源代码经过一系列的处理后打包成Docker镜像，并发布到各个环境，然后通知相关人员。简化后的varian架构如下：


> ----------Docker环境的持续部署优化实践::运维咖啡吧
> https://mp.weixin.qq.com/s/xnBehfSlZ3J02xb0GFuGDw
背景介绍
那年公司快速成长，频繁上线新项目，每上线一个项目，就需要新申请一批机器，初始化，部署依赖的服务环境，一个脚本行天下
那年项目发展如火如荼，A项目流量暴增马上给A扩机器，B项目上线新功能又要扩容B，上线新项目没资源了，就先下线处于流量低峰的C项目主机
每天日夜加班，疲于奔命
那年得知了Docker能拯救我于水火，遂决定为了荣誉（发际线）而战。
为了快速落地以及尽量降低引入Docker对整个CICD流程的影响，用最小的改动把Docker加入到了我们上线的流程中，流程变化参考下图
![](https://mmbiz.qpic.cn/mmbiz_png/s0ib4cHvBPB92uq5ibUINQYLbx46O7j6RkVO4I3VtTPqnmBeOM4T9CDz4iaT9GGBvF9hKTNicllfxR3ibXlZibhXA4aA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)
>
>//
多环境下配置文件的处理
我们采用了项目代码打包进镜像的镜像管理方案，开发、测试、预发布、生产环境配置文件都不同，所以即便是同一个项目不同的环境都会单独走一遍部署发布流程打包镜像，把不同环境的配置打包到不同的镜像中，这个操作太过繁琐且没有必要，还大大增加了我们的上线时间
>
> 用过k8s的都知道，k8s中有专门管理配置文件的ConfigMap，每个容器可以定义要挂载的配置，在容器启动时自动挂载，以解决打包一次镜像不同环境都能使用的问题，对于没有用到k8s的要如何处理呢？配置中心还是必不可少的，之前一篇文章《中小团队落地配置中心详解》有详细的介绍我们配置中心的方案
>
> 我们处理不同配置的整体思路是，在Docker启动时传入两个环境变量ENVT和PROJ，这两个环境变量用来定义这个容器是属于哪个项目的哪个环境，Docker的启动脚本拿到这两个环境变量后利用confd服务自动去配置中心获取对应的配置，然后更新到本地对应的位置，这样就不需要把配置文件打包进镜像了
> 
> 做到了一次镜像打包多环境共用，上线时也无需再走一次编译打包的流程，只需更新镜像重启容器即可，效率明显提高
>
>//
> 写在最后
**缺少编排的容器是没有灵魂的**，继续推进编排工具的运用将会是2019年工作的重点
实际上我们在Docker改造稳定后，内网开发测试环境部署了一套k8s集群用到现在已经一年多的时间比较稳定
线上用到了多云环境，一部分线上项目已经使用了基于k8s的容器编排，当然还有一部分是我上边介绍的纯Docker环境


#### 配置中心

> ----------中小团队落地配置中心详解 - 云+社区 - 腾讯云
> https://cloud.tencent.com/developer/article/1380942
配置中心选型
选型的原则：**简单，易落地**，不挑平台，不挑语言，**尽量少的依赖**。
对比了Disconf、Apollo等方案，最终选择了**Etcd+Confd**的方案，基本符合上边的原则，且Etcd我们在部署Kubernetes的时候已经有过使用，算是轻车熟路。
> 
> //配置中心架构图:
![配置中心架构图](https://ask.qcloudimg.com/http-save/yehe-2933803/vctroqw9cp.png?imageView2/2/w/1620)




=======================================================

## 大数据

### 查询

> ----------Quicksql：360 开源的更简单，更安全，更快速的跨数据源统一 SQL 查询引擎 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/Qihoo360-Quicksql.html



> 【Tablesaw - “大数据”】
> 
> ----------GitHub 上那些值得一试的 Java 开源库 - arthur.dy.lee的专栏 - CSDN博客
> https://blog.csdn.net/paincupid/article/details/51923284
Tablesaw - “大数据”
谈到大数据，我们想到的总是Hodoop加上集群部署，但有没有一种更小巧的方式，能让我们在单机上方便地实现大数据的那些功能呢？Tablesaw给我们提供了一种基于内存的高性能大数据解决方案。你可以使用它的API方便地从RDBMS或是CSV中导入数据，然后利用Tablesaw提供的接口对数据进行排序、筛选、分组、map/reduce等操作。
根据文档给出的说明，你将可以在22秒内将500,000,000行（每行4个字段）的数据文件加载到10G的内存中。而查询速度更是达到仅需1-2ms。

> ----------Presto：针对大数据的分布式SQL查询引擎 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/presto.html




### 数据同步

> ----------DataX 是阿里巴巴集团内被广泛使用的离线数据同步工具/平台 - Java开发社区 | CTOLib码库
> https://www.ctolib.com/DataX.html
DataX 是阿里巴巴集团内被广泛使用的离线数据同步工具/平台，实现包括 MySQL、Oracle、HDFS、Hive、OceanBase、HBase、OTS、ODPS 等各种异构数据源之间高效的数据同步功能。





==========================================================

## AI算法
。。https://github.com/hankcs/HanLP Star 6273
HanLP是由一系列模型与算法组成的Java工具包，目标是普及自然语言处理在生产环境中的应用。HanLP具备功能完善、性能高效、架构清晰、语料时新、可自定义的特点。在提供丰富功能的同时，HanLP内部模块坚持低耦合、模型坚持惰性加载、服务坚持静态提供、词典坚持明文发布，使用非常方便，同时自带一些语料处理工具，帮助用户训练自己的模型。






=============================================

## 前端

> SmartTable 是一套数据源使用 Ajax 获取数据，并展现成表格与图像的形式，并且支持下载（思路源于talkingdata）的智能表格。开源引入：Bootstrap 3.0，Bootstrap respond (IE解决方案)，Jquery 11.02，dataTables，echarts，table2CSV


=======================================================



## 中小团队技术选型

> ----------小团队构建大网站：中小研发团队架构实践_百度百科
> https://baike.baidu.com/item/%E5%B0%8F%E5%9B%A2%E9%98%9F%E6%9E%84%E5%BB%BA%E5%A4%A7%E7%BD%91%E7%AB%99%EF%BC%9A%E4%B8%AD%E5%B0%8F%E7%A0%94%E5%8F%91%E5%9B%A2%E9%98%9F%E6%9E%B6%E6%9E%84%E5%AE%9E%E8%B7%B5/23232448?fr=aladdin
**《小团队构建大网站：中小研发团队架构实践》**结合作者十几年的工作经验，总结了一套系统又详细、且可落地的中小研发团队架构实践指导方案。



> ----------中小型研发团队架构实践三要点 - 坤少_jkson - CSDN博客
> https://blog.csdn.net/jiangzhexi/article/details/78311302
中小型研发团队很多，而社区在中小型研发团队架构实践方面的探讨却很少。中小型研发团队特别是 50 至 200 人的研发团队，在早期的**业务探索**阶段，更多关注**业务逻辑**，快速迭代以验证商业模式，很少去关注技术架构。这时如果继续按照原有的架构及研发模式，会出现大量的问题，再也无法玩下去了。能不能有一套可直接落地、基于开源、成本低，可快速搭建的中间件及架构升级方案呢？


===============================================


## 开源网站

> ----------CTOLib码库
> https://www.ctolib.com/


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

。。https://github.com/b3log/symphony Star 8931
一款用 Java 实现的现代化社区（论坛/BBS/社交网络/博客）平台。分为社区版和商业版
。。https://github.com/eugenp/tutorials Star 10447
该项目是一系列小而专注的教程，每个教程都涵盖一个明确的开发领域。大多数教程项目都专注于Spring Framework（和Spring Security）。以下技术是重点：core Java，Jackson，HttpClient，Guava。
。。Arthas旨在帮助开发人员解决Java应用程序的生产问题，无需修改代码或重新启动服务器。有了Arthas，你就可以在不重新启动JVM或需要额外的代码更改的情况下实时地对问题进行故障排除。


==============================================
