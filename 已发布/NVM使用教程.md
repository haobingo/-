[TOC]

# ⭐️写在前面的话⭐️
> CSDN主页：[程序员好冰](https://blog.csdn.net/m0_67689541?spm=1000.2115.3001.5343)
>
> 目前在学习：操作系统
>
> 技术栈：SpringBoot项目
>
> 推荐书籍：《Java虚拟机》、《Java编程思想》
>
> 博客网站：暂无
>
> ==旅途的意义亦在旅途中。==
>
> 🎉欢迎 【点赞👍 关注🔎 收藏⭐️ 留言📝】
> 📌本文由 程序员好冰 原创，CSDN 首发！
> 📆入站时间： 🌴2022 年 07 月 13 日🌴
>
> 🍭<strong><font color = orange> 作者水平很有限，如果发现错误，一定要及时告知作者哦！感谢感谢！</font></strong>🍭

--- ---



## 1、卸载已经安装的node

**打开控制面板 -> 打开程序和功能 -> 右上角搜索输入node -> 右键卸载**



为了确保彻底删除node在看看你的node安装目录中还有没有node文件夹，有的话一起删除。

再看看C:\Users\用户名 文件夹下有没有`.npmrc`以及`.yarnrc`等等统统删除。再去看看你的环境变量有没有node相关的，有的话也一起删除了。

已经安装了nvm的可以用命令删除指定版本。



 nvm list 查看已经安装的版本

nvm list available 查看网络可以安装的版本

nvm uninstall < version > 卸载制定的版本

![image-20231223151918472](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223151918472.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





现在所有的node都已经删除

![image-20231223151954240](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223151954240.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



顺便删除之前配置好的环境变量：

![image-20231223152405557](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223152405557.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 2、卸载nvm



找到nvm目录下的这个文件，执行以下

![image-20231223152215729](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223152215729.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

环境变量会自动帮你删除

确保已经删除

![image-20231223152531036](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223152531036.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 3、安装nvm

[nvm下载地址](https://github.com/coreybutler/nvm-windows/releases)



![image-20231223152928630](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223152928630.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



运行解压后的可执行文件



![image-20231223153058769](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153058769.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20231223153136180](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153136180.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)







![image-20231223153201099](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153201099.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





用命令符可以查看版本

![image-20231223153238843](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153238843.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





可以看见已经自动添加了环境变量

![image-20231223153320465](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153320465.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





![image-20231223153332062](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153332062.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





## 4、配置路径以及下载源



**找到nvm安装路径 -> 找到 `settings.txt` 文件 -> 配置下载源**



![image-20231223153538853](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153538853.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



```yaml
node_mirror: https://npm.taobao.org/mirrors/node/
npm_mirror: https://npm.taobao.org/mirrors/npm/
```



![image-20231223153657386](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153657386.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





## 5、使用nvm下载node

- 查看可下载的版本     nvm list available



![image-20231223153820938](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153820938.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



- 指定版本进行下载    nvm install 20.5.0



![image-20231223153959985](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223153959985.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



- 使用安装好的node版本      nvm use 20.5.0

![image-20231223154135759](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223154135759.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



- 查看当前的node和npm

![image-20231223154213127](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223154213127.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



- 输入`nvm list` 查看已经安装的node，`*`号表示当前使用的node版本。

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210219095357792.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 6、nvm常用命令

![image-20231223154324579](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223154324579.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 7、全局安装npm、cnpm

安装node的时候，npm其实也已经一起安装了。因为nvm可以管理多个版本的node，如果每次添加一个node版本都要安装一堆的包很麻烦，如果有一个npm可以让各个版本的node共用，就不会这么麻烦了。



- 配置用npm下载包时全局安装的包路径



![image-20231223154906558](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223154906558.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20231223154853968](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223154853968.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 安装全局npm，不同的node都使用这个npm。想更新全局的npm的话首先删除全局路径(就是上一行命令的地址，可以使用npm config ls查看)下的npm，再执行一次这个命令即可

![image-20231223154933198](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223154933198.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



- 在用户变量中添加 `NPM_HOME` = `E:\nvm\npm`，path中添加`%NPM_HOME%`。这里需要注意的是，`%NPM_HOME%`要添加在`%NVM_SYMLINK%`之前，避免npm访问到的是nodejs中自带的npm包管理工具



![image-20231223155002784](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223155002784.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)







![image-20231223155027959](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223155027959.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 8、使用淘宝镜像cnpm

`npm install -g cnpm --registry=https://registry.npm.taobao.org` //使用淘宝镜像cnmp替代npm

`cnpm config get registry` //验证cnpm是否可用





## 9、配置全局的node仓库

在安装node的文件夹下新建两个文件夹；node_cache(缓存文件夹)node_global(全局仓库文件夹)



![image-20231223155612669](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223155612669.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



``` shell
npm config set prefix “D:\dev\nodejs\node_global”

npm config set cache “D:\dev\nodejs\node_cache”
```



![image-20231223155726779](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223155726779.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

在Path环境变量中添加一行

![image-20231223155938974](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231223155938974.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**在【系统变量】新建环境变量 NODE_PATH，值为D:\NVM\node_global\node_modules，其中D:\NVM\node_global\node_modules是上述创建的全局模块安装路径文件夹**

---

> ##### ==🚀 先看后赞，养成习惯！🚀==
>
> ##### ==🚀 先看后赞，养成习惯！🚀==

> <font color=red>**🎈觉得文章写得不错的老铁们，点赞评论关注走一波！谢谢啦！🎈**</font>

---



