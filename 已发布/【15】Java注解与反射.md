[TOC]

# ⭐️写在前面的话⭐️
> 📒博客主页： [程序员好冰](https://blog.csdn.net/m0_67689541?spm=1011.2124.3001.5343)
> 🎉欢迎 【点赞👍 关注🔎 收藏⭐️ 留言📝】
> 📌本文由 程序员好冰 原创，CSDN 首发！
> 📆入站时间： 🌴2022 年 07 月 13 日🌴
> ✉️ 是非不入松风耳，花落花开只读书。
> 💭推荐书籍：📚《Java编程思想》，📚《Java 核心技术卷》
> 💬参考在线编程网站：🌐[牛客网](https://www.nowcoder.com/)🌐[力扣](https://leetcode.cn/)
> 🍭<strong><font color = orange> 作者水平很有限，如果发现错误，一定要及时告知作者哦！感谢感谢！</font></strong>🍭

--- ---



# 1、什么是注解？

>  **Java 注解用于为 Java 代码提供元数据。作为元数据，注解不直接影响你的代码执行，但也有一些类型的注解实际上可以用于这一目的。Java 注解是从 Java5 开始添加到 Java 的。**

将上面的话再翻译一下，如下：
（1）元数据在开发中的作用就是做数据约束和标准定义，可以将其理解成代码的规范标准（代码的模板）；
（2）代码的模板（元数据）不直接影响代码的执行，它只是帮助我们来更快捷的开发；

综上，注解是一种元数据，可以将它理解为注释、解释，它为我们在代码中添加信息提供了一种形式化的方法，它用于帮助我们更快捷的写代码。

## 注解的分类

一般常用的注解可以分为三类：

**1、Java自带的标准注解**
包括@Override、@Deprecated、@SuppressWarnings等，使用这些注解后编译器就会进行检查。

**2、元注解**
元注解是用于定义注解的注解，包括@Retention、@Target、@Inherited、@Documented、@Repeatable 等。
元注解也是Java自带的标准注解，只不过用于修饰注解，比较特殊。

**3、自定义注解**
用户可以根据自己的需求定义注解。



## 常用的Java注解

> 1、@Deprecated – 所标注内容不再被建议使用；
> 2、@Override – 只能标注方法，表示该方法覆盖父类中的方法；
> 3、@Documented --所标注内容可以出现在javadoc中；
> **4、@Inherited – 只能被用来标注“Annotation类型”，它所标注的Annotation具有继承性；**
> **5、@Retention – 只能被用来标注“Annotation类型”，而且它被用来指定Annotation的RetentionPolicy属性；**
> **6、@Target – 只能被用来标注“Annotation类型”，而且它被用来指定Annotation的ElementType属性；**
> 7、@SuppressWarnings – 所标注内容产生的警告，编译器会对这些警告`保持静默`；
> **8、@interface – 用于定义一个注解；**

其中，4、5、6、8多用于自定义注解，读者着重记一下。

# 2、元注解

## @Target

Target的英文意思是目标，这也很容易理解，使用@Target元注解表示我们的==注解作用的范围==就比较具体了，可以是类，方法，方法参数变量等，同样也是通过枚举类ElementType表达作用类型：

- @Target(ElementType.TYPE) 作用接口、类、枚举、注解
- @Target(ElementType.FIELD) 作用属性字段、枚举的常量
- @Target(ElementType.METHOD) 作用方法
- @Target(ElementType.PARAMETER) 作用方法参数
- @Target(ElementType.CONSTRUCTOR) 作用构造函数
- @Target(ElementType.LOCAL_VARIABLE)作用局部变量
- @Target(ElementType.ANNOTATION_TYPE)作用于注解（@Retention注解中就使用该属性）
- @Target(ElementType.PACKAGE) 作用于包
- @Target(ElementType.TYPE_PARAMETER) 作用于类型泛型，即泛型方法、泛型类、泛型接口 （jdk1.8加入）
- @Target(ElementType.TYPE_USE) 类型使用.可以用于标注任意类型除了 class （jdk1.8加入）

一般比较常用的是ElementType.TYPE类型，如下：

```java
@Retention(RetentionPolicy.RUNTIME)
@Target(ElementType.TYPE)
public @interface MyTestAnnotation {

}
```

## @Retention

Retention英文意思有保留、保持的意思，它表示注解存在阶段是保留在源码（编译期），字节码（类加载）或者运行期（JVM中运行）。

在@Retention注解中使用枚举RetentionPolicy来表示===注解保留时期===：

- @Retention(RetentionPolicy.SOURCE)，注解仅存在于源码中，在class字节码文件中不包含
- @Retention(RetentionPolicy.CLASS)， 默认的保留策略，注解会在class字节码文件中存在，但运行时无法获得
- @Retention(RetentionPolicy.==RUNTIME==)， 注解会在class字节码文件中存在，在运行时可以通过反射获取到

> RUNTIME > CLASS > SOURCE

如果我们是自定义注解，则通过前面分析，我们自定义注解如果只存着源码中或者字节码文件中就无法发挥作用，而在运行期间能获取到注解才能实现我们目的，所以自定义注解中肯定是使用 @Retention(RetentionPolicy.RUNTIME)，如下：

```java
@Retention(RetentionPolicy.RUNTIME)
public @interface MyTestAnnotation {

}
```

## @Documented

Document的英文意思是文档。它的作用是能够将注解中的元素包含到==Javadoc==中去。

## @Inherited

Inherited的英文意思是==继承==，但是这个继承和我们平时理解的继承大同小异，一个被@Inherited注解了的注解修饰了一个父类，如果他的子类没有被其他注解修饰，则它的子类也继承了父类的注解。

# 3、自定义注解

### @Override注解的基本格式

![image-20230827111823374](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230827111823374.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



> public @interface 注解名{ 定义内容 }



```java
import java.lang.annotation.*;

public class test {
    @MyAnnotation
    public void test(){

    }
}

@Target(value = ElementType.METHOD)
@Retention(value = RetentionPolicy.RUNTIME)
@Documented
@Inherited
@interface  MyAnnotation{

}
```



# 4、什么是反射？

> 1、Java反射机制的核心是在程序运行时动态加载类并获取类的详细信息，从而操作类或对象的属性和方法。本质是JVM得到class对象之后，**再通过class对象进行反编译，从而获取对象的各种信息。**
>
> 2、Java属于先编译再运行的语言，程序中对象的类型在编译期就确定下来了，而当程序在运行时可能需要动态加载某些类，这些类因为之前用不到，所以没有被加载到JVM。通过反射，可以在运行时动态地创建对象并调用其属性，**不需要提前在编译期知道运行的对象是谁。**

## 什么时候需要用到反射？

- 我们编译时知道类或对象的具体信息，此时直接对类和对象进行操作即可，无需使用反射（reflection）
- 如果编译不知道类或对象的具体信息，此时应该如何做呢？这时就要用到 **反射** 来实现。比如类的名称放在XML文件中，属性和属性值放在XML文件中，需要在运行时读取XML文件，动态获取类的信息

## 反射的应用场合

- 在编译时根本无法知道该对象或类可能属于哪些类，程序只依靠运行时信息来发现该对象和类的真实信息
- 比如：**log4j，Servlet、SSM框架技术**都用到了**反射机制**

```xml
比如：log4j
   log4j.appender.stdout=org.apache.log4j.ConsoleAppender
   log4j.appender.logfile.layout=org.apache.log4j.PatternLayout
比如：Servlet
  <servlet>
        <servlet-name>HelloServlet</servlet-name>
        <servlet-class>servlet.HelloServlet</servlet-class>
    </servlet>
 比如 SSM
  <bean id="tm"  
  class="org..jdbc.datasource.DataSourceTransactionManager">
    <property name="dataSource" ref="dataSource"/>
   </bean>
```

# 5、反射的原理

下图是类的正常加载过程、反射原理与class对象：

Class对象的由来是将.class文件读入内存，并为之创建一个Class对象。

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/v2-12ed9f48c94e5e2a3c63b2ed9bc964b9_1440w.webp?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



# 6、反射机制的优缺点

**1、优点：**

在运行时获得类的各种内容，进行反编译，对于Java这种先编译再运行的语言，能够让我们很方便的创建灵活的代码，这些代码可以在运行时装配，无需在组件之间进行源代码的链接，更加容易实现面向对象。

**2、缺点：**

（1）反射会消耗一定的系统资源，因此，如果不需要动态地创建一个对象，那么就不需要用反射；

（2）反射调用方法时可以忽略权限检查，因此可能会破坏封装性而导致安全问题。



# 7、得到 Class 的三种方式

```java
//1、通过对象调用 getClass() 方法来获取,通常应用在：比如你传过来一个 Object
//  类型的对象，而我不知道你具体是什么类，用这种方法
　　Person p1 = new Person();
　　Class c1 = p1.getClass();

//2、直接通过 类名.class 的方式得到,该方法最为安全可靠，程序性能更高
//  这说明任何一个类都有一个隐含的静态成员变量 class
　　Class c2 = Person.class;

//3、通过 Class 对象的 forName() 静态方法来获取，用的最多，
//   但可能抛出 ClassNotFoundException 异常
　　Class c3 = Class.forName("com.ys.reflex.Person");
```

> 灵活使用反射能让我们代码更加灵活，这里比如JDBC原生代码注册驱动，hibernate 的实体类，Spring 的 AOP等等都有反射的实现。但是凡事都有两面性，反射也会消耗系统的性能，增加复杂性等，合理使用才是真！





---

> <strong> 🚀<font color = orange>先看后赞，养成习惯！</font>🚀</strong>
>
> <strong> 🚀<font color = red> 先看后赞，养成习惯！</font>🚀</strong>

> **🎈觉得文章写得不错的老铁们，点赞评论关注走一波！谢谢啦！🎈**

---



