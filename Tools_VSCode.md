
- [vscode）重要的](#vscode%E9%87%8D%E8%A6%81%E7%9A%84)
- [vscode）22](#vscode22)
- [vscode）list](#vscodelist)
- [vscode）文摘](#vscode%E6%96%87%E6%91%98)



##vscode

#### vscode）重要的
> REST Client 
> SQL Snippets
> Code Runner
> Todo+
> Markdown All in One

#### vscode）22

+ ☐2019-1-25 10:13:22
vscode扩展试用
  > 快捷键
  search:文件打开的扩展,
  gitlens
  git project manager

+ 2019-1-25 17:28:59
>vscode扩展试用，
  ctrl+l快速定位，类似emacs插件，
  打开文件（工程内的文件）

>//已有扩展的试用，记录到github，
文件管理器（打开任意文件），
//，markdown，
//git提交
//todo标记，
//sql扩展
多行tab显示




## REST Client

> ----------REST Client - Visual Studio Marketplace
> https://marketplace.visualstudio.com/items?itemName=humao.rest-client

GET https://example.com/topics/1 HTTP/1.1

//
POST https://example.com/comments HTTP/1.1
content-type: application/json

{
    "name": "sample",
    "time": "Wed, 21 Oct 2015 18:27:50 GMT"
}

> ----------vscode-restclient首页、文档和下载 - VS Code 的 REST 客户端扩展 - 开源中国
> https://www.oschina.net/p/rest-client

//

环境和自定义/系统变量支持

在任何请求位置使用变量

支持环境、文件和请求自定义变量

自动补全和悬停支持环境、文件和请求自定义变量

对请求和文件自定义变量的诊断支持

转到定义并查找仅用于文件自定义变量的所有引用支持

提供**系统动态变量** {{$guid}}、{{$randomInt min max}}、{{$timestamp [offset option]}}、{{$datetime rfc1123|iso8601 [offset option]}} 和 {{$aadToken [new] [public|cn|de|us|ppe] [<domain|tenantId>] [aud:<domain|tenantId>]}}

在设置文件中轻松创建/更新/删除环境和环境变量

支持环境切换

支持共享环境以提供所有环境中可用的变量

//

为后续请求记住 Cookie


============================================================


<!-- list -->
#### vscode）list

。。REST Client 是 VSCode 编辑器的一个扩展，其支持以 .http/.rest 扩展名的文件(HTTP Language)，可在其中以 RFC2616 标准描述 REST API 接口(支持多个请求)，并且支持简单的自定义变量替换。 
感觉可以直接拿来做前后端对接口的文档~

。。vscode插件~Code Runner，， Quokka.js实时执行JavaScript代码(做快速的demo很有用)。Snippets 是一些常用的代码片段，Prettify JSON 格式化JSON

Project Manager 快速切换项目

REST Client 发送REST风格的HTTP请求

Settings Sync VSCode设置同步到Gist

Quokka.js [WallabyJs.quokka-vscode] 是一个调试工具插件，能够根据你正在编写的代码提供实时反馈。它易于配置，并能够预览变量的函数和计算值结果。另外，在使用 JSX 或 TypeScript 项目中，它能够开箱即用。

vscode-faker [deerawan.vscode-faker]  使用流行的 JavaScript 库 – Faker，能够帮你快速的插入用例数据。Faker 可以随机生成姓名、地址、图像、电话号码，或者经典的乱数假文段落，并且每个类别还包含了各种子类别，你可以根据自身的需求来使用这些数据。



#### vscode）文摘
> ----------SQL Snippets - Visual Studio Marketplace
> https://marketplace.visualstudio.com/items?itemName=sadeghpm.sql-snippets

s-s	default select for extending with help query-options
s-sone	select one row by where condition

==========

> ----------VSCode 拓展插件推荐 - zhangzongshan - 博客园
> https://www.cnblogs.com/zzsdream/p/6592429.html

Git Blame 在状态栏显示当前行的Git信息

Git History(git log) 查看git log

GitLens 显示文件最近的commit和作者，显示当前行commit信息

Prettify JSON 格式化JSON

Project Manager 快速切换项目

[a](#)

============================================================



> ----------能让你开发效率翻倍的 VSCode 插件配置（中）_慕课手记
> https://www.imooc.com/article/26032?block_id=tuijian_wz
Code Runner
Code Runner，名副其实的代码运行插件，支持数十种语言，在不离开代码编辑器的前提下通过命令面板可直接执行代码，并查看输出。

> ----------Markdown All in One - Visual Studio Marketplace
> https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one

> ----------Paste JSON as Code - Visual Studio Marketplace
> https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype

Supports TypeScript, Python, Go, Ruby, C#, Java, Swift, Rust, Kotlin, C++, Flow, Objective-C, JavaScript, Elm, and JSON Schema.

============================================================



===========================================================

> ----------Todo+ - Visual Studio Marketplace
> https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-todo-plus

Box: - ❍ ❑ ■ ⬜ □ ☐ ▪ ▫ – — ≡ → › [] [ ]
Done: ✔ ✓ ☑ + [x] [X] [+]
Cancelled: ✘ x X [-]

===========================================================



