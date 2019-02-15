**目录：**
- [主题研究](#%E4%B8%BB%E9%A2%98%E7%A0%94%E7%A9%B6)
  - [1）REST API](#1rest-api)
    - [客户端](#%E5%AE%A2%E6%88%B7%E7%AB%AF)
    - [Swagger](#swagger)
    - [测试框架HttpRunner](#%E6%B5%8B%E8%AF%95%E6%A1%86%E6%9E%B6httprunner)
  - [2）JSON](#2json)
    - [服务器开发](#%E6%9C%8D%E5%8A%A1%E5%99%A8%E5%BC%80%E5%8F%91)
    - [工具](#%E5%B7%A5%E5%85%B7)
  - [3）权限管理](#3%E6%9D%83%E9%99%90%E7%AE%A1%E7%90%86)
    - [数据权限](#%E6%95%B0%E6%8D%AE%E6%9D%83%E9%99%90)
    - [开源权限list](#%E5%BC%80%E6%BA%90%E6%9D%83%E9%99%90list)
- [debug线上故障排查/调试经验](#debug%E7%BA%BF%E4%B8%8A%E6%95%85%E9%9A%9C%E6%8E%92%E6%9F%A5%E8%B0%83%E8%AF%95%E7%BB%8F%E9%AA%8C)
  - [List](#list)

    - [工具](#%E5%B7%A5%E5%85%B7)
===================================================



## 主题研究

### 1）REST API

#### 客户端

> Postman

> VSCode插件：REST Client

#### Swagger


> ----------让接口测试成为合格的桥梁——本地搭建 Swagger-UI 环境搭建 · TesterHome
> https://testerhome.com/topics/8168
思路就是借鉴服务端开发使用的Swagger UI，定制化我们自己需求的既可以展示Jmeter执行结果，又能让开发在线调试的页面。
>
>最后在Swagger UI界面可以查看这里的json文件展示的样式：
![](https://testerhome.com/uploads/photo/2017/58b183395d7b395df3adae77d379f893.png!large)



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




#### 测试框架HttpRunner


### 2）JSON

#### 服务器开发

> apiJSON

> GraphQL

> 纯JSON框架

#### 工具

> IDEA插件：JSON转javaBean

> json在线格式化：http://json.cn


### 3）权限管理

#### 数据权限

//
> ----------各功能模块说明 - Yearning_guide
> https://guide.yearning.io/used/
yearning细粒化权限设计理念
在一般的使用过程,用户会有各种不同类型的权限需求，所以权限必须做到细粒度，且以功能来划分最为合理。

Yearning采用多源权限策略，以及多权限配合的设计方案。

首先将提交人和审核人/执行人 通过角色属性区分开来。

然后再通过细粒度的基于功能的权限 对每个用户进行个性化的权限配置。

细粒度可配置的权限如下图（由于查询采用工单形式所以现阶段查询权限已舍弃）:
![enter image description here](https://guide.yearning.io/images/per.png)

细力度权限的每一种权限都具有独立性。所以权限相互独立，互不影响。并且用户可以同时继承不同的权限组，管理员可根据每个用户的实际需求自由组合权限组（多个权限组中重复的权限系统会自动去重)。

所以拼图式的权限划分保证了管理员充分的管理自由性，更能适应不同公司的不同需求。


//
> ----------数据库自动化运维平台--自助权限申请 - 晨夕的博客 - CSDN博客
> https://blog.csdn.net/liuhanran/article/details/73289242
客户端程序访问数据库都需要一个**连接数据库的用户名和密码**，这个用户一般是DBA帮RD创建。根据安全级别的不同，每个团队都会有不同的授权方式。我们在用户访问数据库安全方面也制定了一套规则：

(1) 读写账号只能有SELECT，DELETE，UPDATE，INSERT权限。

(2) 用户的白名单IP不能是一个网段，必须是一个IP。

(3) 白名单IP必须是线上的服务器IP，不能是线下测试机IP。

对于白名单IP不能是网段这条规则，可能会给DBA带来很多的工作量。RD给出几十个IP白名单让DBA授权是常有的事，并且在手动授权的过程中容易犯错，比如之前就发生过手动授权覆盖已有账号的密码，使得客户端无法连接数据库的故障。

基于以上原因，最近对RD开放了新的运维平台，**自助授权申请平台**。




#### 开源权限list
//
> ----------jCasbin：支持 MAC、RBAC、ABAC 多种模型的 Java 权限管理框架 - V2EX
> https://jiasule.v2ex.com/t/446988
jCasbin 是一个用 Java 语言打造的轻量级开源访问控制框架（ https://github.com/casbin/jcasbin ），目前在 GitHub 开源。jCasbin 采用了元模型的设计思想，支持多种经典的访问控制方案，如基于角色的访问控制 RBAC、基于属性的访问控制 ABAC 等。


## debug线上故障排查/调试经验

### List

//
> ----------记一次诡异的故障排查经历 - 云+社区 - 腾讯云
> https://cloud.tencent.com/developer/article/1193722
每一次故障排查都是一笔财富，各种狗血经过不表，解决问题之后的那种满足是不可替代的。



