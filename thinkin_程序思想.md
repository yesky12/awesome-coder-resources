
**目录：**

- [编程思想](#%E7%BC%96%E7%A8%8B%E6%80%9D%E6%83%B3)
    - [list](#list)
    - [设计思想](#%E8%AE%BE%E8%AE%A1%E6%80%9D%E6%83%B3)
    - [容器思想](#%E5%AE%B9%E5%99%A8%E6%80%9D%E6%83%B3)
    - [Linux思想](#linux%E6%80%9D%E6%83%B3)
        - [纯文本的格式](#%E7%BA%AF%E6%96%87%E6%9C%AC%E7%9A%84%E6%A0%BC%E5%BC%8F)

===============================================

## 编程思想

##### list
//
> ----------GraphQL的前提 - 酷辣虫 - CoLaBug.com
> https://www.colabug.com/4378062.html
即便是现在早已普世的RESTful，真的用在项目里，也依然要搞清楚它**本质的概念（面向资源）**。

殊途同归，**最终都是要先消化业务，抽象模型，再来谈最基本的语法**。

只不过，GQL的schema中为模型里的很多对应概念都提供了对应的元素：edges, nodes。



//
> ----------数据库自动化运维平台--自助权限申请 - 晨夕的博客 - CSDN博客
> https://blog.csdn.net/liuhanran/article/details/73289242
总结：
通过**平台服务化**，使得DBA的工作更有**效率，降低重复性工作**。﻿﻿



//
> ----------运维效率之数据迁移自动化 - 云+社区 - 腾讯云
> https://cloud.tencent.com/developer/article/1380939
为什么需要**工单**？目前的流程都是通过邮件的方式，需求邮件到DBA，DBA执行导数据的操作。**自动化**的流程理论来说应该从头至尾都无需人工参与，但涉及到数据安全问题，还是需要DBA确认，所以加了工单。同时工单具有状态**自助**追踪，减少沟通成本等优点，后续也**方便统计工单量等指标**，以便优化服务与流程。同时为了能够保证工单及时被处理，我们每一步都会增加邮件和IM的通知，给用户最及时的反馈。



>初试**Jenkins2.0 Pipeline**持续集成 - 哎_小羊的博客 - CSDN博客https://blog.csdn.net/aixiaoyang168/article/details/72818804
先介绍下什么是Jenkins 2.0，**Jenkins 2.0的精髓是Pipeline as Code**，是帮助Jenkins实现CI到CD转变的重要角色。什么是Pipeline，简单来说，就是一套运行于Jenkins上的工作流框架，将原本独立运行于单个或者多个节点的任务连接起来，实现单个任务难以完成的复杂发布流程。Pipeline的实现方式是一套**Groovy DSL**，任何发布流程都可以表述为一段Groovy脚本，并且Jenkins支持从代码库直接读取脚本，从而实现了Pipeline as Code的理念。 

> ----------运维咖啡吧
> https://mp.weixin.qq.com/s?__biz=MzU5MDY1MzcyOQ==&mid=2247483730&idx=1&sn=435c10f8c1ec6938f80b0e7d814dfdcd&scene=21#wechat_redirect
>
> + **简单**即是美
> + 适合自己的就是最好的



##### 设计思想

>**动态绑定**优于静态绑定

>隔离变化

> **软件硬件化**，硬件软件化
>     做软件的**主板**



##### 容器思想


> ----------运维咖啡吧
> https://mp.weixin.qq.com/s/xnBehfSlZ3J02xb0GFuGDw
缺少**编排**的容器是没有灵魂的



##### Linux思想

> ----------Linux的哲学思想 - ZhengLiming - 博客园
> https://www.cnblogs.com/ZhengLiming/p/5875049.html
> Linux哲学思想：
> 1、**一切皆文件**；
> 2、小型，单一用途的程序；（**KISS**）
> 3、连接程序，共同完成复杂功能；
> 4、避免令人困惑的用户界面；
> 5、配置数据存储在**文本**中；

==========


####### 纯文本的格式
> ----------Linux 中优秀的**文本化编辑思想**大碰撞（Markdown、LaTeX、MathJax） - 京山游侠 - 博客园
> https://www.cnblogs.com/youxia/p/linux014.html

优秀的思想应该是这样的：

文章就应该存储为**纯文本的格式**，用任何工具都可以阅读和编辑；
该纯文本的内容即要适合人类阅读，也要计算机容易理解；
能正确指定文章各部分的逻辑结构；
内容和显示分离，作者只用考虑文章的内容和逻辑结构，而文章怎么显示得好看是专业的人和工具的事。
这就是我标题中说的“文本化编辑思想”。这种思想在计算机领域由来已久，并逐渐形成一种哲学。比如互联网上广泛使用的 HTML、XML 等，就是把信息储存为纯文本，用任 何工具都可以阅读和编辑，并且能正确地指定内容的逻辑结构，而浏览器和 CSS 则控制文章如何显示。但是，HTML 标签还是太多了，如果没有浏览器，完全靠人工脑补阅读起来还是太困难了。于是，就诞生了 Markdown。

==========

> ----------Todo+ - Visual Studio Marketplace
> https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-todo-plus

Portable: being a **plain text format** you can read and edit it using any editor

==========

