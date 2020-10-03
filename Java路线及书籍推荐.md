# Java 直通企业级开发路线及书籍推荐

> https://github.com/hansonwang99/JavaCollection

## Java生态技术体系科普

### Java技术体系

说到 Java，其实是一个很厚重的概念，Sun官方（后来被Oracle收购）所定义的 Java技术体系至少包括以下几个大的组成部分：
1. Java程序设计语言
2. 各种平台上的Java虚拟机（JVM）
3. Java API类库
4. 一系列辅助工具，比如 javac

其中：
* 1+2+3+4 = **JDK**：即Java开发包，是支撑 Java程序开发的最小环境
* 2+3 = **JRE**：即Java运行时环境，是支撑 Java程序运行的最小环境

**JVM（Java Virtual Machine）**即Java虚拟机，Java语言使用 JVM这个魔法神器屏蔽了与具体系统和平台相关的信息，从而使得 Java语言编译的程序只需生成在 Java虚拟机上可运行的目标代码（字节码）即可，JVM会将字节码解释成具体平台的机器指令执行，这就是 Java可以一次编译，到处运行的原因。

这里给出一个关于面试 Java开发时常问的 JVM内存结构相关问题的参考示意图：

![JVM内存结构相关问题的参考示意图](https://i0.hdslb.com/bfs/article/e7631407e674e39c80fb8d6188a4f14b7105b6da.png@1102w_626h.webp)

### Oracle JDK vs OpenJDK

Oracle JDK 和 OpenJDK。

其实二者的核心库是差不多的，大家不必拘泥于此，至于两者区别，结合网上的一些科普文章，可以总结如下：

1. 授权协议不一样
2. OpenJDK 只包含最精简的JDK那一部分
3. OpenJDK 源代码是不完整的，因为 SUN时期的 JDK中一部分源代码因为产权的问题未开放给 Open JDK使用

二者的核心库是差不多的，大家不必过于纠结。而且我们平时学习和开发所常用的是 Oracle JDK，也建议初学者下载这个使用。

### Java技术体系所划分的三大平台

许多0基础的Java学习者可能或多或少听说过 Java SE、Java EE和 Java ME三个概念，但不知道三者之间的区别，以及我们究竟该入手学习哪一个呢？下来面一一认识一下

1. Java SE (Java Platform, Standard Edition)，其以前称为J2SE，主要用来开发传统 C/S架构软件，通俗来讲，即开发电脑桌面应用等
2. Java EE (Java Platform, Enterprise Edition)。这个版本以前被称为J2EE。 企业版是开发和部署可移植、健壮、可伸缩、安全的服务端Java应用，典型的就是企业 Web服务。Java EE是构建于JavaSE之上的，只不过增加了一些更加便捷的企业级应用框架。比如我们现在最常用的Java EE开发框架 Spring家族就属于其范畴。
3. Java ME (Java Platform, Micro Edition)。其是为在移动、嵌入式设备上运行的Java应用提供的平台环境。

而这里推荐 **Java EE** 才是我们应该学习和耕耘的领域。不管是早期的 SSH 框架，还是现如今仍然火热的 SSM框架，甚至于今天更加先进的 Spring Boot 和Spring Cloud等都是Java EE的领域，看到了其繁荣性，我想大家应该无需有后顾之忧了。

### 哪一版JDK用得多，适合于学习

1. JDK版本更新迭代非常之快，官方可下载的版本已经发布到了JDK 11 LTS版，连JDK 12都即将要问世了
2. 但很多技术栈老一点的公司，JDK 1.6甚至都还在使用当中
3. 而 JDK 1.8当下用的还是非常广泛的，我们学习的话装1.8也就够了，出了问题能查到的资料也多

注:  JDK不分 Java SE、Java EE 和 Java ME 的，安装的都是一个东西。

## 书籍推荐

### 《Java编程思想》

细节多，大而全，圣经级别的书。

### 《Java并发编程实战》

企业级开发会涉及到。这本书的原文作者们本来就是Java并发工具专家组的主要成员，所以权威性杠杠滴，但如果学Java并发上来就钻这本书，而这本书又是翻译过来的，确实是有点晦涩了。

### 《深入理解Java虚拟机》

都知道JVM虚拟机对于Java而言极其重要，这本是理解JVM机制比较好的书了。

注: Open JDK

### 《函数式编程思维》

提高代码的信噪比，但不容易重构，难懂。

### 《TCP/IP详解 卷1:协议》

计网的东西乍看起来好像很杂，但抓住分层的思想梳理总结之后其实也还好。就像这本书，表面看起来有点晦涩，但沉下心来完全能看懂。

### 《Spring MVC + MyBatis开发 从入门到项目实践》

快餐级别的书，帮助快速上手。

### 《Spring 技术内幕》

### 《Elasticsearch 服务器开发（第2版）》

版本比较老，但是还比较有指导意义。 NoSQL

### 《Redis入门指南》

快餐书。NoSQL

----

### Java语言

### 《Java核心技术（Core Java）》

这本讲的很全面，书中的代码示例都很好，很适合Java通用学习。

### 《Effective Java》

这本算是进阶书籍了，里面讲的全是Java使用的经验技巧和指导意见，等Java比较熟之后再看看一定会非常有收获的

### 《实战Java高并发程序设计》

这本用来入门学习Java并发编程知识点还是很适合的，基础、全面、能看懂，看完之后心里对于Java并发这一块的东西可以保个底。

## 数据结构和算法

### 《数据结构与算法分析 Java语言描述》

这本书本来它就是国外数据结构与算法分析的经典教材，系统全面且严谨，适合对Java语言比较熟，而且数据结构和算法有些了解的同学。

### 《算法 第4版》

## 计算机网络（TCP/IP协议）

### 《计算机网络：自顶向下方法》

《TCP/IP详解 卷1:协议》看不懂可以先看这个

### 《图解TCP/IP》《图解HTTP》

比上面那本更为简单

## 数据库/SQL

### 《MySQL必知必会》

书不厚，主讲SQL用法，入门不错，也可以当小册子查阅。

### 《高性能MySQL》

上面的用法熟了，学习原理、提升数据库性能，可以读这本，不过书很厚。

## 操作系统

### 《深入理解计算机系统（CSAPP）》

如果说这本是纯讲操作系统的书好像也不尽然，它更像是计组和操作系统的组合。

### 《现代操作系统》

这本也比较系统和全面。

## 设计模式

### 《Head First设计模式》/《大话设计模式》

### 《设计模式：可复用面向对象软件的基础》

## Linux使用/基本Shell编程

当然这里说的基本使用层面的，常见的不管是像《鸟哥的Linux私房菜》这种经典，还是《Linux命令行与shell脚本编程大全》这种大全，都可以做手册来用，书实在太厚了。

## Java后端开发详细学习路线

https://www.bilibili.com/read/cv6013525

![Java后端开发详细学习路线](https://i0.hdslb.com/bfs/article/91b4e4066a32436632dfc58f18b9c78997735d2a.jpg)

## Java企业级开源项目

开源项目是获取项目经验的一个绝好途径。

### Halo

一个优秀的开源博客发布应用（博客系统）。

地址: https://github.com/halo-dev/halo

注意其使用的技术。

### Hutool

Hutool是一个小而全的Java工具类库。

地址: https://github.com/looly/hutool

### Piggy Metrics

Microservice Architecture with Spring Boot, Spring Cloud and Docker

地址: https://github.com/sqshq/piggymetrics

熟悉Spring Cloud落地。

### HanLP

1.X 版本：Java实现

地址: https://github.com/hankcs/HanLP/tree/1.x

2.X 版本：Python实现

面向生产环境的多语种自然语言处理工具包，基于 TensorFlow 2.x，目标是普及落地最前沿的NLP技术。

地址: https://github.com/hankcs/HanLP

### Spring-Boot-In-Action

Code Sheep，对初学者比较友好。

https://www.bilibili.com/read/cv1966843

地址: https://github.com/hansonwang99/Spring-Boot-In-Action

## 开源项目如何运行、读代码

https://www.bilibili.com/video/BV1y4411p74E

不要有畏难心理。

1. 了解项目是干什么的，有没有兴趣学习，有哪些技术点（可以提前拆分了解）。
2. 本地能把项目跑起来
3. 阅读项目源码并调试（可以结合某个运行起来的功能入手，一个组建一个组件弄熟、看报错、看日志、看打印变量）
4. 自己会改东西，加自己的模块。

### 实例Halo

从controller开始看起，是前后端交互的控制入口。不做代码，仅仅是调用。服务在service里。

学习如何在代码设断点**调试**，在前台刷新页面，在后台就能看到传过来的具体参数。

## 开源项目结构、

https://www.bilibili.com/read/cv5236887

## 自学Java开发的学习路线

https://www.bilibili.com/read/cv4184856

### 基础知识

- 编程语言：Java Python C
- 基本算法
- 基本网络知识：TCP/IP  HTTP/HTTPS
- 基本的设计模式

### 工具方面

- 操作系统：linux (CentOS\Ubuntu\Fe..)
- 代码管理：SVN / Git
- 持续集成(CI/CD)：jenkins

- java的项目管理工具：Maven / Gradle 

### 框架方面

#### 应用层框架

- ~~ssh (spring+structs+hibernate)(已过时)~~
- ssm:spring +springmvc+mybatis(流行)
- spring boot

#### 各种中间件

- MQ 消息队列
- RPC 通讯框架 gRPC thrift dubbo springcloud
- elasticsearch 数据库 搜索引擎

#### 数据库

- SQL：MySQL / Postgre SQL
- NoSQL：Redis memcached mongodb elasticsearch

### 架构方面

#### 分布式/微服务架构

- spring cloud
- dubbo
- rpc通信

#### 虚拟化/容器化的技术

- Docker 
- 容器化
- k8s kubernetes

### 关注源码 /性能

- jdk源码以及部分设计思想
- Spring 源码
- JVM细节与排错
- 高并发/高可用