## 计算机基础

#### 什么是计算机

有硬件和软件组成，著名的`冯 若依曼体系结构`：输入设备、输出设备、存储器、运算器和控制器。

#### 计算机语言的发展史

机器语言、汇编语言、高级语言，高级语言中有分为`面向对象`和`面向过程`两大类。

## Java入门学习

#### Java、C与C++之间的对比

| 语言 |                             优点                             |                             缺点                             |
| :--: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|  C   | 贴近硬件，运行极快，效率极高，面向过程，可以直接编译成可执行的文件，运行速度快 | 指针和内存管理繁琐，内存需要手动处理内存，存在内存泄漏问题， |
| C++  |   兼容C，面向对象，可以直接编译成可执行的文件，运行速度快    |                      存在内存泄漏问题，                      |
| Java | 没有指针和内存管理，类型安全，可移植：`Write once , run anywhere`,拥有高质量的类库，有了`Java虚拟机`，不用考虑垃圾回收以及内存泄漏的问题，语法规范 |                  运行速度较慢，并不贴近底层                  |

#### Java分类

JavaSE（Java标准版：桌面）、JavaME（Java移动版：手机）、JavaEE（Java企业版：服务器）

#### Java的特性

简单性、面向对象、可移植性、高性能、分布式、动态性（反射机制）、多线程、安全性（语法规范、没有指针和内存管理）、健壮性（生态完善、拥有异常处理机制）

#### JDK、JRE和JVM

**JDK（Java开发工具：Java development kit）**由 JRE 和一些工具组成

**JRE（Java运行时环境：Java runtime environment）**由 JVM 和一些库函数组成

**JVM（Java虚拟机：Java virtual machine）**跨平台的核心，相当于在操作系统上模拟了一个小巧的CPU，去处理Java相关的东西

#### 安装Java相关的软件以及开发环境

参考博客  ： [https://blog.csdn.net/weixin_47281685/article/details/126022368](https://blog.csdn.net/weixin_47281685/article/details/126022368)

#### Java的编译型和解释型

举个例子:

```
	中国人刘慈欣写了一本中文科幻小说叫《三体》，这时候有一个不懂中文的美国人想要看这本书，就有两个解决方案：
	一是花钱买来一本中文版的《三体》看，这样的话，如果《三体》这本书更新了，或者是修改了，就又要重新买一本中文版来看；
	二是请一个翻译官，随时翻译，美国人读到哪里的时候就翻译到哪里，看一段就翻译一段，而且不怕随时更新。
```

方案一就类似编译型，方案二就类似解释型。

`编译型`（compile）通过编译器编译，对操作系统的要求较低，速度更快，eg：C语言、C++、Java，Java中编译器将java文件（`源文件`）编译成class文件（`字节码文件`），相当于`预编译`，操作：`javac Java文件名`  ——>会生成一个class文件（计算机可识别的字节码文件），运行class文件，操作：`java class文件名`。

<img src="C:\Users\Haobin\AppData\Roaming\Typora\typora-user-images\image-20230116214340074.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230116214340074" style="zoom: 67%;" />

`解释型`速度较慢，比如网页以及一些脚本，边执行边解释，eg：Python、Java、JavaScript，Java在JVM上解释运行。

参考：[什么是编译型语言和解释型语言](https://blog.csdn.net/weixin_43876206/article/details/93328310)

​			[Java偏向于解释型语言](https://blog.csdn.net/weixin_43876206/article/details/93330986)