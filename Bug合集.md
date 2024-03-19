### 1、找不到依赖项 'e-iceblue:spire.office.free:5.3.1'

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230827174158546.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230827174158546" style="zoom: 33%;" />

==解决方法==

在[maven](https://so.csdn.net/so/search?q=maven&spm=1001.2101.3001.7020)的配置settings.xml文件中添加下列内容

```xml
<mirrors>
	<mirror>
		<id>com.e-iceblue</id>
		<url>http://repo.e-iceblue.cn/repository/maven-public/</url>
	    <mirrorOf>com.e-iceblue</mirrorOf>
	    <name>com.e-iceblue</name>
	</mirror>
</mirrors>	
<repositories>
	<repository>
		<id>com.e-iceblue</id>
		<url>http://repo.e-iceblue.cn/repository/maven-public/</url>
	</repository>
</repositories>
```

### 2、vue项目运行报错Proxy error: Could not proxy request “ UIRL” from “  ” to  “”

**今天在测试反向代理的时候，访问本地接口的时候报错Proxy error: Could not proxy request /miaomiao/cityList from localhost:8080 to http://10.12.0.111:3001.
See https://nodejs.org/api/errors.html#errors_common_system_errors for more information (ECONNREFUSED).**
**首先看编译器报错**
![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/2021030110480443.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)
出现这种问题大致两种原因

1. 是因为代理对象没有开启服务，不能访问到对象服务器
2. 代理规则写错
   我们这里出现此问题的原因是因为我在vue.config.js中把代理地址写错了，本来应该是3000的，我测试反向代理是否成功的时候写成了3001，所以出现了这样的错误、
   ![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210301105258521.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/2021030110494098.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### 3、java: 无法访问org.springframework.boot.SpringApplication
  错误的类文件: 
    类文件具有错误的版本 61.0, 应为 52.0
    请删除该文件或确保该文件位于正确的类路径子目录中。

![image-20230903172014097](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230903172014097.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

[解决无法访问org.springframework.boot.SpringApplication，类文件具有错误的版本xxx, 应为xxx，请删除该文件或确保该文件位于正确的类路径子目录中。-天翼云 (ctyun.cn)](https://www.ctyun.cn/zhishi/p-249214)

## 4、由于打错字

![image-20231004105253844](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231004105253844.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)
