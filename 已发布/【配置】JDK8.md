[TOC]

# JDK8的安装与配置

## 1、选择哪个版本的JDK？

目前最新版本为jdk19，但个人认为选择`jdk8`、`jdk11`、`jdk17`这几个长期支持的版本最好；

同时，你的本地版本和服务器的版本最好一致，防止“==本地能跑，服务器不能跑==”。

## 2、官网下载

> [官网链接](https://www.oracle.com/)

#### 2.1 找到导航栏里的Resources下的 Java Downloads

![image-20230209143325209](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209143325209-16759244529511.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

#### 2.2 寻找存档版本 Java archive

![image-20230209143552259](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209143552259-16759245545252.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

#### 2.3 选择jdk8

![image-20230209145059721](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209145059721.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20230209145151566](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209145151566.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

#### 2.4 找到下载好的exe文件，以管理员身份运行

![image-20230209145524621](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209145524621.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



#### 2.5 更改路径，最好是统一放在一个Environments下，之后点击下一步

![image-20230209145815258](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209145815258.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



#### 2.6 修改jre的安装路径，点击下一步

![image-20230209150107486](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209150107486.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



#### 2.7 等待安装

![image-20230209150435022](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209150435022.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



#### 2.8 配置环境变量

##### 2.8.1 找到电脑的高级系统设置

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209150742805.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209150742805" style="zoom: 50%;" />



##### 2.8.2 环境变量

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209150830606.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209150830606" style="zoom: 50%;" />

##### 2.8.3 JAVA_HOME

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209151123292.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209151123292" style="zoom: 50%;" />

##### 2.8.4 找到path变量，双击打开，新建

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209151813931.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209151813931" style="zoom:50%;" />



##### 2.8.5 确定即可

## 3、在项目中引入

##### 3.1 Add JDK

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209152453669.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209152453669" style="zoom:50%;" />

##### 3.2 选择jdk的安装路径，点击OK

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230209152646951.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230209152646951" style="zoom:50%;" />

##### 3.3 即可引入



## 4、注意

==安装多个版本的jdk，上面的变量名应使用不同的==，如：JAVA_HOME、JAVA1.8_HOME、JAVA1.7_HOME。




---

> ####  **说在最后📝*：*
>
> ​	✍创作不易，如果觉得文章写得还可以的话，就不要吝啬你的 👍 啦~ ✍

---