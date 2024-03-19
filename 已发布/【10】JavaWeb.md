[TOC]



# 一、基本概念

>  在 Java 中，动态web资源开发的技术统称为JavaWeb

## 1.1 动态Web网站简介

提供给所有人看到的数据始终会发生变化，每个人在不同时间，不同地点看到的信息个不相同

https-------443端口

http---------80端口

常用技术栈：

- Servelt
- JSP
- ASP
- PHP

## 1.2 web应用程序

可以提供浏览器访问的程序，web应用程序编写完毕后，若想提供给外界访问，需要用`Tomcat服务器`统一管理。

- html、css、js
- jsp、servlet
- java程序
- jar包
- 配置文件（properties）

## 1.3 静态web

类似html这样的网页后缀，如果服务器上一直存在这些东西，我们就可以通过网络进行读取。

![](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/静态web流程.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

静态web存在的缺点：

- web页面无法动态更新，只能编写JavaScript实现`伪动态`；

- 无法和数据库交互，`数据无法持久化`（注册、商品信息、用户信息），和用户无法交互；

  

## 1.4 动态web

页面会动态展示

![](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/动态web流程.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

动态web存在的缺点：

- 如果加入服务器的动态web资源出现了错误，我们需要重新编写后台程序再发布，即`停机维护`。

# 二、web服务器

>  C/S：客户端和服务器
>
>  B/S：浏览器和服务器

## 2.1 技术

- ASP：在HTML中嵌入了VB的脚本，ASP+COM,缺点：业务代码多，页面混乱，维护成本高；
- PHP：开发速度快，功能强大，支持跨平台，代码简单，缺点：无法承载大访问量的情况（局限性）；
- JSP/Servlet：sun公司主推的B/S架构，基于Java，可承载三高（高性能、高可用、高并发），语法与ASP相似。

## 2.2 应用服务器

==作用==：处理用户请求和提供用户响应信息。

`IIS`

IIS是指World Wide Web server服务，IIS是一种Web（网页）服务组件，专业的说，IIS可以赋予一部主机电脑一组以上的IP地址，而且还可以有一个以上的域名作为Web网站。

`Tomcat`

Tomcat 是由 Apache 软件基金会下属的 Jakarta 项目开发的一个 Servlet 容器，按照 Sun Microsystems 提供的技术规范开发出来，Tomcat 8 实现了对 Servlet 3.1 和 JavaServer Page 2.3（JSP）的支持，并提供了作为 Web 服务器的一些特有功能，如 Tomcat 管理和控制平台、安全域管理和 Tomcat 附加组件等。==最新版本为9.0==。

![](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/Tomcat在web中的作用.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 2.3 安装 jdk8

[程序员好冰](https://blog.csdn.net/m0_67689541?spm=1011.2266.3001.5343)

# 三、Tomcat

>  [官网链接](https://tomcat.apache.org/)

## 3.1 安装 Tomcat9

[程序员好冰](https://blog.csdn.net/m0_67689541?spm=1011.2266.3001.5343)

## 3.2 文件说明

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209155240737.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209155240737" style="zoom: 33%;" />

- bin ：启动、关闭的脚本文件
- conf ： 配置
- lib ： 依赖的jar包
- logs ： 日志
- temp ： 存放临时文件
- webapps ： 存放网站

## 3.3 启动并使用Tomcat

> Tomcat路径 ------ > bin目录 -------> startup.bat  双击

在浏览器输入：==localhost:8080==

访问测试：http://localhost:8080

localhost(默认主机) 127.0.0.1

默认端口号：8080

- mysql默认端口号：3306
- http默认端口号：80
- https默认端口号：443

## 3.4 关闭Tomcat

> Tomcat路径 ------ > bin目录 -------> shutdown.bat  双击

## 3.5 可能遇到的问题

1. Java环境变量没配置；
2. 闪退问题，需要配置兼容性；
3. 乱码问题，在startup.bat文件中配置。

## 3.6 配置

### 3.6.1 修改测试访问的网页地址

> 在conf目录下打开server.xml  （服务器核心配置文件）

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209160826908.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209160826908" style="zoom:33%;" />

> 修改默认端口号

![image-20230209201502541](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209201502541.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 修改默认主机，如：将 localhost 改为 www. haobing. com 

- 第一步：将Host的name属性修改为 www. haobing. com 

![image-20230209201604371](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209201604371.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 第二步：打开文件：C:\Windows\System32\drivers\etc\hosts  

![image-20230209202219933](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209202219933.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 第三步：添加映射

  ![image-20230209202348957](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209202348957.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 3.6.2 修改测试访问的网页内容

> 在webapps目录下找到 ROOT 打开

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209204234807.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209204234807" style="zoom: 50%;" />

> 保留这个文件夹（WEB-INF），其它都可以修改

![image-20230209204429359](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209204429359.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### 3.6.3 修改存放网页的位置

> Host下的APPBase属性就是网页的根目录

![image-20230209203021614](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209203021614.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> webapps下的每个文件夹名，都是可以访问的

![image-20230209204856693](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209204856693.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 3.7  网站是如何进行访问的？

- 客户端请求网址；
- 先查找客户端本机 host（C:\Windows\System32\drivers\etc\hosts  ） 配置文件下有没有这个域名的映射；
  - 有，直接返回对应的IP地址，结束
  - 没有，继续下一步

- 查找`DNS服务器`
  - 有，返回对应的IP地址，结束
  - 没有，访问出现错误 404



## 3.8 网站应有的结构

```java
---webapps  //Tomcat服务器的web目录、
	-ROOT
	-haobing  //网站的目录名
	-WEB-INF  //存放网站程序
		-web.xml   //网站的配置文件
		-classes  //Java程序
		-lib   //web应用所依赖的jar包
	-index.jsp //默认的首页
	-static
		-css
		-js
		-img
	-...
```

# 四、Http 详解

>  一个简单的请求-响应协议

==它指定了客户端可能发送给服务器什么样的信息以及得到什么样的响应==

默认端口：80

Https：安全，默认端口：443

超文本传输协议，超文本：图片、音乐、视频、定位、地图...，运行在TCP之上

## 4.1 版本

- `http 1.0 `：仅能够一次连接，客户端可以与web服务器连接后，只能获得一个web资源，之后断开连接；
- `http 1.1`：能够进行多次连接，可以获得多个web资源。

## 4.2 Http请求

>  客户端------发请求-----服务器

```java
请求 URL: https://www.baidu.com/
请求方法: GET/POST
状态代码: 200 OK
远程地址: 14.215.177.39:443
引用者策略: strict-origin-when-cross-origin
```

```java
Accept:text/html
Accept-Encoding: gzip
Accept-Language: zh-CN   -------------->语言
Cache-Control: max-age=0
Connection: keep-alive
```

### 4.2.1 请求行

请求行中的请求方式：GET；

请求方式：GET、POST、HEAD、DELETE、PUT、TRACT

- `GET`：一次请求能够携带的参数比较少，大小有限制，会在浏览器的URL地址栏显示数据内容，不安全，但是高效；
- `POST`：一次请求能够携带的参数没有限制，大小没有限制，不会会在浏览器的URL地址栏显示数据内容，安全，但是不高效。

### 4.2.2 消息头

```java
Accept:   -------------->告诉浏览器它支持的数据类型
Accept-Encoding:    -------------->支持哪种编码格式：GBK、UTF-8、GB2312、ISO8859-1
Accept-Language:    -------------->设置语言
Cache-Control:    -------------->缓存控制
Connection:    -------------->告诉浏览器，请求完成是断开还是保持连接
HOST:   -------------->主机
```

## 4.3 Http响应

> 服务器-----响应------客户端

```java
Cache-Control:private    -------------->缓存控制
Connection: keep-alive   --------------->连接，保持连接，说明是http1.1
Content-Encoding: gzip   --------------->编码
Content-Type: text/html; charset=utf-8 ------>类型
```



### 4.3.1 响应体

```java
Accept:   -------------->告诉浏览器它支持的数据类型
Accept-Encoding:    -------------->支持哪种编码格式：GBK、UTF-8、GB2312、ISO8859-1
Accept-Language:    -------------->设置语言
Cache-Control:    -------------->缓存控制
Connection:    -------------->告诉浏览器，请求完成是断开还是保持连接
HOST:   -------------->主机
ReFresh:   -------------->告诉客户端多久刷新一次
Location:   -------------->让网页重新定位
```

### 4.3.2 响应状态码

- `200`：成功
- 3**：请求重定向
- 4**：找不到资源
- 5**：服务器代码错误
- 502：网关错误

# 五、Maven

> [官网链接](https://maven.apache.org/)

>  Maven的核心功能是合理叙述项目间的依赖关系，通俗点讲，就是通过pom.xml文件的配置获取jar包，而不用手动去添加jar包

在JavaWeb开发中，需要手动导入jar包，Maven可以`自动`帮我们导入和配置jar包。

==项目架构管理工具==，核心思想：`约定大于配置`

Maven会规定好你该如何去编写我们的Java代码，必须要按照这个规范来。

## 5.1 安装Maven

> [程序员好冰](https://blog.csdn.net/m0_67689541?spm=1011.2266.3001.5343)

## 5.2 文件说明

![image-20230210112653209](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210112653209.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- bin：执行文件
- boot：启动需要的选项
- conf：配置文件

## 5.3 修改镜像

> Maven目录下---->conf------>settings.xml

==镜像==：方便下载使用

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113127034.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230210113127034" style="zoom: 50%;" />



![image-20230210113157537](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113157537.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> [阿里云镜像官网](https://developer.aliyun.com/mirror/)

![image-20230210113551709](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113551709.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 找到Maven

![image-20230210113613119](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113613119.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 直接复制

![image-20230210113752569](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113752569.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 粘贴在这，即可

![image-20230210113925965](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113925965.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 5.4 配置环境变量

> M2_HOME---------------bin目录
>
> MAVEN_HOME--------bin上一级目录

![image-20230210115203446](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210115203446.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 添加path

![image-20230210115356258](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210115356258.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 查看是否配置成功--------------mvn -version

![image-20230210115524542](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210115524542.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 5.5 创建本地仓库

> 在Maven目录下创建一个文件夹

![image-20230210120751587](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210120751587.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 修改localRepository下的目录

![image-20230210120646176](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210120646176.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 5.6 在IDEA中使用Maven

> 打开全局设置

![image-20230210121855567](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210121855567.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> 设置Maven

![image-20230210121945384](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210121945384.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> 更改：
>
> 1. Maven版本
> 2. settings.xml位置
> 3. 本地仓库位置

![image-20230210122237233](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210122237233.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> Apply

![image-20230210122313712](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210122313712.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 创建新项目

![image-20230210122353742](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210122353742.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20230210122636845](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210122636845.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> 点击创建

![image-20230210122800172](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210122800172.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210122832893](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210122832893.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 查看本地仓库，发现多出来的文件，说明成功

![image-20230210123039045](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210123039045.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 成功！

## 5.7 模板创建和直接创建的对比

> 左边使用模板创建------------------------右边直接创建

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210175523750.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230210175523750" style="zoom:50%;" />



## 5.8 标记文件夹

> ==约定大于配置思想==

> 按照图中打开

![image-20230210212325892](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210212325892.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210212500014](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210212500014.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 照上修改后，对应的文件图标将会改变颜色

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210212638392.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230210212638392" style="zoom: 67%;" />

## 5.9 在IDEA中配置Tomcat

> 编辑配置

![image-20230210213011719](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210213011719.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 找到并选择本地Tomcat

![image-20230210213210963](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210213210963.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> 相关配置

![image-20230210214145800](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214145800.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 配置Tomcat HOME

![image-20230210215331377](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215331377.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210215523383](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215523383.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> 配置Tomcat的安装路径

![image-20230210215616375](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215616375.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 成功，点击OK-----Apply

![image-20230210215721480](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215721480.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)


> ==指定一个文件夹名==

![image-20230210214248602](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214248602.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210214332672](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214332672.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> ==虚拟路径映射==

![image-20230210214745910](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214745910.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)


> 点击运行

> 这里访问到的HelloWorld就是我们默认的==index.jsp==中的内容

![image-20230210215944626](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215944626.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210220006144](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210220006144.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> Tomcat配置成功

## 5.10 Maven侧边栏的说明

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210221445515.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230210221445515" style="zoom: 33%;" />

## 5.11 pom文件分析

```xml
<!--Maven版本和头文件-->
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/maven-v4_0_0.xsd">
  <modelVersion>4.0.0</modelVersion>

<!--  这里就是我们刚才配置的GAV-->
  <groupId>org.example</groupId>
  <artifactId>javaweb-01-maven</artifactId>
<!--  项目的打包方式:
        1.jar-Java应用;
        2.war-JavaWeb应用-->
  <packaging>war</packaging>
<!--  版本-->
  <version>1.0-SNAPSHOT</version>

  <name>javaweb-01-maven Maven Webapp</name>

  <url>https://maven.apache.org</url>
<!--  配置-->
  <properties>
      <!--项目的默认构建编码-->
       <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
       <maven.compiler.source>1.8</maven.compiler.source>
       <maven.compiler.target>1.8</maven.compiler.target>
  </properties>

<!--  项目依赖-->
  <dependencies>
<!--    项目具体依赖的jar包文件-->
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.11</version>
    </dependency>
  </dependencies>
<!--  项目构建的插件-->
  <build>
    <finalName>javaweb-01-maven</finalName>
  </build>
</project>
```

> [Maven的 JAR 包仓库](https://mvnrepository.com/tags/maven)

![image-20230211143702405](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211143702405.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

==Maven的强大之处在于==：它会帮你导入一个JAR包所依赖的其他JAR包

## 5.12 约定大于配置思想的缺点

> Maven由于它的约定大于配置的思想，当我们编写的配置文件不符合规范的时候，将会无法导出或者生效

> 例如：在java目录（本应该放class文件）下，存放xml文件或properties文件

==解决方案==：

> [链接一](https://www.cnblogs.com/yuqiliu/p/12059614.html)
>
> [链接二](https://www.cnblogs.com/pixy/p/4798089.html)

`在build中配置resources，来防止资源导出失败的问题`

```xml
<build>
      <resources>
        <resource>
            <directory>src/main/resources</directory>
            <excludes>
                <exclude>**/*.properties</exclude>
                <exclude>**/*.xml</exclude>
             </excludes>
            <filtering>false</filtering>
        </resource>
        <resource>
            <directory>src/main/java</directory>
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>
            <filtering>false</filtering>
        </resource>
    </resources>
</build>
```

> Maven中的目录树

> Maven中jar包的一些结构体系

![image-20230211123619825](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211123619825.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 5.13 更改webapp版本

> 替换为webapp4.0版本，和Tomcat一致

> 原始版本：webapp2.3

![image-20230211150350752](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211150350752.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 找到：Tomcat安装目录-------webapps-------ROOT-------WEB-INF-------web.xml

![image-20230211150528638](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211150528638.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230211150559155](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211150559155.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

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

> 将上面的内容替换到WEB-INF下的web.xml中，==全部替换==

![image-20230211150654433](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211150654433.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 替换后...

![image-20230211150816502](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211150816502.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

# 六、Servlet

## 6.1 Servlet简介

> [简介链接](http://c.biancheng.net/servlet2/what-is-servlet.html)：Servlet 是 Sun 公司推出的一种基于 Java 的动态网站开发技术。

> 编写 Servlet 代码需要遵循 Java 语法，一个 Servlet 程序其实就是一个按照 Servlet 规范编写的 Java 类。Servlet 程序需要先编译成字节码文件（.class文件），然后再部署到服务器运行。

Sun公司在这些API中提供一个叫Servlet的接口，如果你想开发一个Servlet程序，需要完成两个步骤：

- 编写一个类，实现Servlet接口
- 把开发好的Java类部署到web服务器中

==实现了Servlet接口的Java程序叫做Servlet==

## 6.2 使用Servlet

> 创建一个普通的Maven项目，并将src目录删除

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211160216670.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230211160216670" style="zoom:33%;" />

> 在pom.xml中添加项目依赖

```xml
<dependencies>
    <!-- https://mvnrepository.com/artifact/javax.servlet/javax.servlet-api -->
    <dependency>
        <groupId>javax.servlet</groupId>
        <artifactId>javax.servlet-api</artifactId>
        <version>4.0.1</version>
    </dependency>
    <!-- https://mvnrepository.com/artifact/javax.servlet.jsp/javax.servlet.jsp-api -->
    <dependency>
        <groupId>javax.servlet.jsp</groupId>
        <artifactId>javax.servlet.jsp-api</artifactId>
        <version>2.3.3</version>
    </dependency>
</dependencies>
```

> 找到Maven仓库：maven-repo\javax\servlet，Maven会自动下载如下文件：

![image-20230211160703324](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211160703324.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 创建子模块

![image-20230211161319196](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211161319196.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20230211161516162](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211161516162.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 父子项目

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211161847774.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230211161847774" style="zoom:50%;" />

> 父项目中的pom.xml

![image-20230211161952849](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211161952849.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 子项目中

![image-20230211162051344](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211162051344.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

==父项目中的 JAR 包子项目可以直接使用，反过来不行==-------------`多态`

```java
son extends father {}
```

> 更换web.xml中的webapp版本

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

==编写Servlet程序==

### 6.2.1 编写Java文件

> java---package

![image-20230211162725083](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211162725083.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 包名规范

![image-20230211162941810](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211162941810.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> class文件

![image-20230211163037367](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211163037367.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230211163108181](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211163108181.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



|              树              |                              类                              |
| :--------------------------: | :----------------------------------------------------------: |
|           Servlet            | void service(ServletRequest var1, ServletResponse var2) throws ServletException, IOException; |
|        GenericServlet        | public abstract void service(ServletRequest var1, ServletResponse var2) throws ServletException, IOException; |
|         HttpServlet          | ![image-20230211164530623](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211164530623.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10) |
| HelloServlet（我们创建的类） |                     ==我们需要进行重写==                     |

> 重写doGet（）和doPost（）方法

快捷键：==alt + insert==

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211164756588.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230211164756588" style="zoom:50%;" />

> 由于get或者post只是请求实现的方式不同，因此可以互相调用，业务逻辑都一样

```java
package com.haobin.servlet;

import javax.servlet.ServletException;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.io.PrintWriter;

public class HelloServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        System.out.println("进入doGet方法");
        PrintWriter writer = resp.getWriter();
        writer.print("Hello,Serlvet!");
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        doGet(req, resp);
    }
}
```



### 6.2.2 编写Servlet映射

==为什么需要映射？==

`我们编写的是Java程序，但是要通过浏览器访问，而浏览器需要连接web服务器，所以我们要在web服务器中注册我们编写的Servlet，还需要给它一个浏览器能够访问的路径`

> 在web.xml文件下

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211170008073.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230211170008073" style="zoom:50%;" />



> mapping-----映射

![image-20230211170253491](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211170253491.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 6.2.3 配置Tomcat

> 编辑配置

![image-20230210213011719](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210213011719.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 找到并选择本地Tomcat

![image-20230210213210963](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210213210963.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> 相关配置

![image-20230210214145800](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214145800.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 配置Tomcat HOME

![image-20230210215331377](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215331377.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210215523383](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215523383.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> 配置Tomcat的安装路径

![image-20230210215616375](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215616375.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 成功，点击OK-----Apply

![image-20230210215721480](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215721480.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)


> ==指定一个文件夹名==

![image-20230210214248602](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214248602.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210214332672](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214332672.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> ==虚拟路径映射==

![image-20230210214745910](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210214745910.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)


> 点击运行

> 这里访问到的HelloWorld就是我们默认的==index.jsp==中的内容

![image-20230210215944626](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210215944626.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210220006144](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210220006144.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> Tomcat配置成功

### 6.2.4 运行

> 生成的target文件夹

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211170930431.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230211170930431" style="zoom:50%;" />



> 网页显示

![image-20230211171050812](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211171050812.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20230211171112181](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211171112181.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

`映射请求逻辑`

![image-20230211171413233](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230211171413233.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 6.3 Servlet运行原理

`Servlet是由Web服务器调用的，web服务器在收到浏览器请求之后，会进行如下过程：`

![image-20230227171229506](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230227171229506.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 6.4 Mapping

- 一个Servlet可以指定一个映射路径

```xml
<servlet-mapping>
    <servlet-name>hello</servlet-name>
    <url-pattern>/hello</url-pattern>
</servlet-mapping>
```

- 一个Servlet可以指定多个映射路径

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
```

- 一个Servlet可以指定通用映射路径（*可以包括任何东西，包括为空的情况）

```xml
<servlet-mapping>
    <servlet-name>hello</servlet-name>
    <url-pattern>/hello/*</url-pattern>
</servlet-mapping>
```























































---

> ####  **说在最后📝*：*
>
> ​	✍创作不易，如果觉得文章写得还可以的话，就不要吝啬你的 👍 啦~ ✍

---