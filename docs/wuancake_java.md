# 午安煎饼计划Java组学习内容 v2.1

## 一、职业介绍

Java是一种广泛使用的计算机编程语言，拥有跨平台、面向对象、泛型编程的特性，广泛应用于企业级Web应用开发和移动应用开发。

Java程序员的薪资水平可参考拉勾网：https://www.lagou.com/zhaopin/Java/

自学 Java 怎么入门？https://www.zhihu.com/question/25255189

Java 初学者，如何学习 Java？：https://www.zhihu.com/question/22407671/answer/145198723

## 二、准备工作

进行学习前，你需要安装一些软件。

Java环境JDK8：http://www.oracle.com/technetwork/cn/java/javase/downloads/jdk8-downloads-2133151-zhs.html

开发工具IntelliJ IDEA：https://www.jetbrains.com/idea/download/ ，也可以选择Spring Tool Suite。

## 三、基础阶段

基础阶段主要学习Java SE的语法、集合、XML文件格式和解析、String、面向对象、多线程、泛型、循环分支、Scanner等。

### 1.考核任务

使用Java+SAX/Dom4j(XML)实现一个简易的登录与注册功能。

需要编写设计文档与思路并提交至git。编码实现，编码规范参考Java官方推荐的。测试使用Junit进行单元测试。使用findbugs插件检查简单的bug。

功能要求：能够命令行运行，实现注册、登录、查询用户数量与信息、退出等功能。

### 2.学习内容

以下内容不要求全部学完，也不用局限于以下内容，大家选择适合自己的学习方案，能完成考核任务即可。

Java入门第一季：http://www.imooc.com/learn/85

Java入门第二季：http://www.imooc.com/learn/124

Java入门第三季：http://www.imooc.com/learn/110

Java 教程：http://www.runoob.com/java/java-tutorial.html

Java 1.6 API 文档官方中文版：http://download.oracle.com/technetwork/java/javase/6/docs/zh/api.zip

Java 1.8 API 文档翻译版：https://blog.fondme.cn/apidoc/jdk-1.8-google/

Java核心技术·卷 I：https://book.douban.com/subject/26880667/

Java核心技术·卷 II：https://book.douban.com/subject/27165931/

## 四、进阶阶段

进阶阶段主要学习Java EE相关内容，并学习HTML基础、CSS、JS基础、HTTP协议、Tomcat使用、数据库增删改查、JDBC（MySQL）、JSP（EL/JSTL表达式）、Servlet、会话管理（Cookie/Session）等知识。

完成该阶段考核任务即可进入煎饼计划开发组。

### 1.考核任务

使用JSP+Servlet+MySQL(Tomcat)技术实现一个简易的能实现录与注册功能的网页，包含注册、登录、修改用户信息、查询用户数量与信息、登出等功能。

信息需存储于MySQL数据库中，并使用JDBC与c3p0连接池维护数据库连接。

### 2.学习内容

1）JavaEE介绍：https://blog.csdn.net/xinxin19881112/article/details/4523274

2）下载所需知识的相关内容：http://pan.baidu.com/s/1i5EFdK5 密码: wuvt

3）前导知识

由于做后端最终需要展示到浏览器上，在一开始学习的时候，做一些demo展示是还是需要一些前端基础才行，要不然无法进行实践。所以在开始前，需要先学习点前端相关的知识。HTML与JavaScript具体需要到什么程度，查看文件分享中的，day2,3,4,5,6,7 从1-26压缩版这个文件夹提取出来的。 

![](https://ws1.sinaimg.cn/large/4079825aly1frrgky441uj20j807ydft.jpg)

4）Web基础

Http协议，服务器容器 tomcat,Servlet,JSP,jdbc等等知识。具体如下：

![](https://ws1.sinaimg.cn/large/4079825aly1frsqydrvj0j20ag0b474q.jpg)

5）Web框架

首先了解下MVC软件架构的含义：https://baike.baidu.com/item/mvc

就从目前来说，一个Web项目使用的框架以及Spring的地位，会有以下几个：

Mybatis: 与数据库做交互的持久层框架，属于半ORM框架，现在比较流行。与MyBatis作用差不多的还有一个Hibernate框架，不过该框架在新起的从0开始的项目中很难在见到使用者了，学习难度远远大于MyBatis。建议先学习MyBatis。

Spring:这里指的是 www.spring.io组织发布的一系列框架中的核心框架。主要指图中的Core: 

![](https://ws1.sinaimg.cn/large/4079825aly1frsr1gknijj20hs08gt8z.jpg)

SpringMVC:在MVC中指的就是C，控制。主要是控制页面间的跳转与值传递。在WEB项目中，页面就是VIEW，可以暂时理解为JSP页面，浏览器看到的部分。与SpringMVC作用差不多的框架有一个Struts2.但是这个框架由于性能，漏洞等原因，在从零开始的新起的项目也基本上被抛弃，而且学习难度在一开始远远难于SpringMVC。所以建议学习SpringMVC.

6）项目框架快速搭建工具SpringBoot：https://projects.spring.io/spring-boot/

7）项目构建工具Maven：https://maven.apache.org/

8）正则表达式30分钟入门教程：http://deerchao.net/tutorials/regex/regex.htm

9）JSON 教程：http://www.runoob.com/json/json-tutorial.html

10）猴子都能懂的Git入门：https://backlog.com/git-tutorial/cn/intro/intro1_1.html

## 五、持续学习

### 1.书籍推荐

Spring in Action: 链接：http://pan.baidu.com/s/1hsBhCI4 密码：4ym4

SpringBoot实战: http://dwz.cn/5WGntPMyBatis手册: http://www.mybatis.org/mybatis-3/zh/index.html

阿里巴巴JAVA开发手册: https://102.alibaba.com/newsInfo.htm?newsId=6

您的设计模式 http://download.csdn.net/detail/meryhuang/9922437

### 2.网站推荐

http://ifeve.com/category/java/

http://www.importnew.com/

https://github.com/upan/cheat-sheet/wiki/%E5%9B%BD%E5%A4%96%E7%A8%8B%E5%BA%8F%E5%91%98%E6%95%B4%E7%90%86%E7%9A%84Java%E8%B5%84%E6%BA%90%E5%A4%A7%E5%85%A8

http://wiki.jikexueyuan.com/list/java/