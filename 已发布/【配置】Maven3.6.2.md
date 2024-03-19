[TOC]



# Maven3.6.2 安装与环境搭建

## 1、下载安装

### 1.1 官网下载，点击Download

> [官网链接](https://maven.apache.org/)

![image-20230210111006397](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210111006397.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 1.2 在存档中找

![image-20230210111745314](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210111745314.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### 1.3 找到3.6.2版本

![image-20230210111815690](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210111815690.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 1.4 点击

![image-20230210111943113](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210111943113.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### 1.5 选择3.6.2-bin.zip

![image-20230210112024786](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210112024786.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### 1.6 顺便下载一下源码



![image-20230210112315004](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210112315004.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230210112335005](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210112335005.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### 1.7 下载完成后解压即可

## 2、修改镜像

> Maven目录下---->conf------>settings.xml

==镜像==：方便下载使用

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113127034.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230210113127034" style="zoom: 67%;" />



![image-20230210113157537](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113157537.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> [阿里云镜像官网](https://developer.aliyun.com/mirror/)

![image-20230210113551709](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113551709.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 找到Maven

![image-20230210113613119](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113613119.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 直接复制

![image-20230210113752569](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113752569.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 粘贴在这，即可

![image-20230210113925965](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210113925965.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 3、配置环境变量

> 打开系统环境变量

> M2_HOME---------------bin目录
>
> MAVEN_HOME--------bin上一级目录

![image-20230210115203446](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210115203446.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 添加path

![image-20230210115356258](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210115356258.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 查看是否配置成功--------------mvn -version

![image-20230210115524542](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210115524542.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 4、创建本地仓库

> 在Maven目录下创建一个文件夹

![image-20230210120751587](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210120751587.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

> 修改localRepository下的目录

![image-20230210120646176](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230210120646176.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)


---

> ####  **说在最后📝*：*
>
> ​	✍创作不易，如果觉得文章写得还可以的话，就不要吝啬你的 👍 啦~ ✍

---