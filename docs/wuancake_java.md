# 煎饼计划Java组学习内容 v3.0

## 一、职业介绍

Java是一种广泛使用的计算机编程语言，拥有跨平台、面向对象、泛型编程的特性，广泛应用于企业级Web应用开发和移动应用开发。

Java程序员的薪资水平可参考BOSS直聘：https://www.zhipin.com/c101010100-p100101/

自学 Java 怎么入门？https://www.zhihu.com/question/25255189

Java 初学者，如何学习 Java？：https://www.zhihu.com/question/22407671

## 二、准备工作

进行学习前，你需要安装一些软件。

1.Java环境JDK8：https://caiyun.139.com/w/i/1F5C3NM6213cc 提取码:JfZb

2.开发工具IntelliJ IDEA（社区版即可）：https://www.jetbrains.com/zh-cn/idea/download/

3.数据库MySQL（目前此见相关项目使用5.7）：https://downloads.mysql.com/archives/installer/

4.数据库管理工具（任选其一）

Navicat for MySQL：https://www.navicat.com.cn/download/navicat-for-mysql

HeidiSQL：https://www.heidisql.com/download.php

DBeaver：https://dbeaver.io/download/

## 三、基础阶段

基础阶段主要学习Java SE的语法、集合、XML文件格式和解析、String、面向对象、多线程、泛型、循环分支、Scanner等。

### 1.考核任务

使用 Java+SAX/Dom4j(XML)实现一个简易的登录与注册功能。

需要编写设计文档与思路并提交至 git。编码实现，编码规范参考 Java 官方推荐的。测试使用 Junit 进行单元测试。使用 findbugs 插件检查简单的 bug。

功能要求：能够命令行运行，实现注册、登录、查询用户数量与信息、退出等功能。

进阶要求：本次开发的程序所有数据在内存中，当项目重启时数据无法继承，请结合`XML（或JSON）` + `序列化/反序列化` + `文件IO`将本次运行时的用户数据落盘，项目重启时继承上次运行的数据。 

### 2.学习内容

以下内容不要求全部学完，也不用局限于以下内容，大家选择适合自己的学习方案，能完成考核任务即可，条条大路通罗马。
- 慕课视频有一套完整的学习计划，可参考，前三季为基础知识部分。
- 菜鸟教程提供了编程的基础技术教程，介绍了各种编程语言的基础知识。

慕课Java视频教程：https://www.imooc.com/course/programdetail/pid/31

菜鸟Java文字教程：http://www.runoob.com/java/java-tutorial.html

廖雪峰Java教程：https://www.liaoxuefeng.com/wiki/1252599548343744

在线Java 8 中文版API手册：https://www.matools.com/api/java8

Java核心技术·卷 I：https://book.douban.com/subject/26880667/

Java核心技术·卷 II：https://book.douban.com/subject/27165931/

## 四、进阶阶段

进阶阶段主要学习Java EE相关内容，并学习HTML基础、CSS、JS基础、HTTP协议、Tomcat使用、数据库增删改查、JDBC（MySQL）、JSP（EL/JSTL表达式）、Servlet、会话管理（Cookie/Session）等知识。

完成该阶段考核任务即可进入煎饼计划开发组。

### 1.考核任务

#### 进阶任务1：

使用 JSP+Servlet+MySQL(Tomcat)技术实现一个简易的能实现录与注册功能的网页，包含注册、登录、修改用户信息、查询用户数量与信息、登出等功能。
信息需存储于 MySQL 数据库中，并使用 JDBC 与 c3p0 连接池维护数据库连接。

未登录时禁止查询与修改用户信息

学习这部分时请着重`response` `request` 这两个servlet的内置对象，在后面的开发中用到频率高。

#### 进阶任务2：

仿照`午安计划周报项目`进行开发API接口，功能包括：注册、登录、修改用户信息、查询用户数量与信息等功能，无需开发界面，数据库表请自行设计。

纯接口项目每一次请求都是全新的会话，session将不再适用，请通过token来作为用户身份验证的载体。

技术要求： 
- Spring Boot 或 Spring + spring MVC
- MyBatis
- MySQL
- 允许使用其他的第三方类库或中间件

本任务通过后可进入开发组

### 2.学习内容

1）JavaEE介绍：https://blog.csdn.net/xinxin19881112/article/details/4523274

2）下载所需知识的相关内容：https://caiyun.139.com/m/i?014MdMHX7Dl4c 提取码:i1N6

3）前导知识

由于做后端最终需要展示到浏览器上，在一开始学习的时候，做一些demo展示是还是需要一些前端基础才行，要不然无法进行实践。所以在开始前，需要先学习点前端相关的知识。HTML与JavaScript具体需要到什么程度，查看文件分享中的，day2,3,4,5,6,7 从1-26压缩版这个文件夹提取出来的。 

4）Web基础

Http协议，服务器容器 tomcat,Servlet,JSP,jdbc等等知识。具体如下：

```java
day01 java回顾
day02 html教学
day03 JavaScript基础
day04 JavaScript Bom
day05 JavaScript Dom
day06 xml dom解析
day07 xml dom与sax解析
day08 xml约束与tomcat初步
day09 http协议
dayl0 servlet编程
dayll 会话管理
day12 Jsp基础&编程实战
day13 Jsp加强
day14 自定义标签&编程实战
day15 mysql基础
day16 mysql加强
day17 Jdbc基础
day18 Jdbc增强
day19 Jdbc优化
day20 连接池与分页
day21 过滤器
day22 监听器
day23 文件上传与下载&JavaMail邮件开发
day24 项目实战之分组演练I
day25 项目实战之分组演练II
day26 hotel_v1源码
```

5）Web框架

首先了解下MVC软件架构的含义：https://baike.baidu.com/item/mvc

就从目前来说，一个Web项目使用的框架以及Spring的地位，会有以下几个：

Mybatis: 与数据库做交互的持久层框架，属于半ORM框架，现在比较流行。与MyBatis作用差不多的还有一个Hibernate框架，不过该框架在新起的从0开始的项目中很难在见到使用者了，学习难度远远大于MyBatis。建议先学习MyBatis。


Spring：这里指的是 www.spring.io 组织发布的一系列框架中的核心框架。主要指图中的Core: 

![](https://cdn.jsdelivr.net/gh/natianzao/PicGo/img/spring_framework.gif)

SpringMVC：在MVC中指的就是C，控制。主要是控制页面间的跳转与值传递。在WEB项目中，页面就是VIEW，可以暂时理解为JSP页面，浏览器看到的部分。与SpringMVC作用差不多的框架有一个Struts2.但是这个框架由于性能，漏洞等原因，在从零开始的新起的项目也基本上被抛弃，而且学习难度在一开始远远难于SpringMVC。所以建议学习SpringMVC。

6）项目框架快速搭建工具SpringBoot：https://projects.spring.io/spring-boot/

7）项目构建工具Maven：https://maven.apache.org/

8）正则表达式30分钟入门教程：http://deerchao.net/tutorials/regex/regex.htm

9）JSON 教程：http://www.runoob.com/json/json-tutorial.html

10）猴子都能懂的Git入门：https://backlog.com/git-tutorial/cn/intro/intro1_1.html

## 五、持续学习

### 1.书籍推荐

Spring in Action: https://potoyang.gitbook.io/spring-in-action-v5/

SpringBoot实战: https://caiyun.139.com/m/i?015CHwy9ssuOj 提取码:UWbn

MyBatis手册：https://mybatis.org/mybatis-3/zh/

阿里巴巴JAVA开发手册: https://developer.aliyun.com/special/tech-java

您的设计模式：https://caiyun.139.com/m/i?015CHJ107WHZY 提取码:pwF1

### 2.网站推荐

并发编程网：http://ifeve.com/category/java/

ImportNew博客：https://www.weibo.com/importnew

国外程序员整理的Java资源大全：https://github.com/upan/cheat-sheet/wiki/%E5%9B%BD%E5%A4%96%E7%A8%8B%E5%BA%8F%E5%91%98%E6%95%B4%E7%90%86%E7%9A%84Java%E8%B5%84%E6%BA%90%E5%A4%A7%E5%85%A8

极客学院：http://wiki.jikexueyuan.com/list/java/

易百教程：https://www.yiibai.com/html/java/

IDEA使用教程：https://blog.csdn.net/qq_27093465/article/details/77449117
