[TOC]

---



# 1️⃣ **一、注释**

## 🚋 **1、单行注释**

```java
public class Main {
    public static void main(String[] args) {
        //单行注释
        System.out.println("Hello world!");
    }
}
```



## 🎈  **2、多行注释**

```java
public class Main {
    public static void main(String[] args) {
        /*
        	多行注释
            多行注释
         */
        System.out.println("Hello world!");
    }
}
```



## 🌈 **3、文档注释**

文档注释通常用于JavaDoc文档的生成，就是生成自己的API文档。

```java
public class Main {
    /**
     * @author Haobin(作者名)
     * @version (版本号)
     * @since (指明需要最早使用的jdk版本)
     * @param args (参数名)
     * @return (返回值情况)
     * @throws (异常抛出情况)
     */
    public static void main(String[] args) {
        System.out.println("Hello world!");
    }
}
```



## ⛱ **4、有趣的代码注释**



```java
/***                              _
 *  _._ _..._ .-',     _.._(`))
 * '-. `     '  /-._.-'    ',/
 *    )         \            '.
 *   / _    _    |             \
 *  |  a    a    /              |
 *  \   .-.                     ;
 *   '-('' ).-'       ,'       ;
 *      '-;           |      .'
 *         \           \    /
 *         | 7  .__  _.-\   \
 *         | |  |  ``/  /`  /
 *        /,_|  |   /,_/   /
 *           /,_/      '`-'
 */
```



---



# 2️⃣ **二、标识符和关键字**

## 🚋 **1、标识符的使用**



> - 大小写敏感
> - 首字母应以字母、$ 或 __ 开始
> - 不建议使用中文
> - 不能使用关键字作文变量名或方法名





## 🎈  **2、Java中的关键字举例**



| public  |      void      |    static     |     long     |   int    |
| :-----: | :------------: | :-----------: | :----------: | :------: |
| private |     const      |  ==assert==   |     else     |  float   |
| protect |      this      |   abstract    |    import    |  double  |
|  enum   |     super      | ==interface== |  ==native==  |   try    |
|  class  |     throws     |     throw     | ==volatile== |  catch   |
|   do    | ==instanceof== | ==transient== |  impliments  |  switch  |
|  while  |      new       |      if       |    final     |  break   |
|   for   |     return     |     short     |   finally    | continue |
| extends |    package     |   ==goto==    | ==strictfp== |   case   |
| default |      char      |    boolean    | synchronized |   byte   |



---





# 3️⃣ **三、数据类型**

## 🚋 **1、Java的数据类型**

Java属于``强类型语言``，在使用的时候要求变量的使用要严格要求符合规定，所有变量都必须先定义后才能使用，保证了语言的安全性。

`弱类型语言`并不要求一定要符合使用的规范，例如：JavaScript，可以将数值类型的变量与字符类型的变量进行操作。如下：

```javascript
<body>
    <script>
        var a = 123;
        var b = " Hello ";
        var c = 'World!';
        var s;
        s = a + b + c;
        console.log(s);
    </script>
</body>
```





## 🎈  **2、Java的数据类型分类**

|    类型     |                             说明                             |
| :---------: | :----------------------------------------------------------: |
|    byte     |         基本类型，范围较小， -128~127，容易发生越界          |
|    short    |                   基本类型，两个字节的范围                   |
|   ==int==   |                      基本类型，默认类型                      |
|    long     | 基本类型，使用是要在数字后面加上 L 进行标识，==eg：1234000L== |
|    float    | 基本类型，使用时要在数字后面加上 F 进行标识，==eg：12.34F==  |
| ==double==  |                      基本类型，默认类型                      |
|    char     |      基本类型，只能够保存2个字节的值，仅一个中文的大小       |
| ==boolean== |           基本类型，布尔类型， true 和 false 两种            |
| ==String==  |            引用类型，属于类的一种，==不是关键字==            |
| BigDecimal  |  引用类型，==数学工具类==，适合进行银行业务的计算，精度较高  |



> Java中的引用类型包括 类 、 接口 和数组 ！！！



## 🌈 **3、类型转换**

==说明==：强制类型转换——类型级别：高到低 （损失精度，或者存在计算溢出）

​			自动类型转换——类型级别：低到高

> ​       低 ------------------------------------------------------------- 高
>
> byte，short，char   ->  int ->  long  ->  float  ->  double



---





# 4️⃣ **四、变量、常量和作用域**

## 🚋 **1、变量**

- 变量命名需要符合规范,小写驼峰命名法；
- 变量的声明：`数据类型  变量名  =   值 ;`
- 命名尽量不使用中文的拼音，应该简明易懂。

## 🎈  **2、常量**

常量在初始化之后，不再允许改变，使用关键字 ==final ==；

`在给常量命名是通常使用全大写的方式！！！`

==说明==：修饰符不存在先后顺序

> static final int  PI     与      final  static  int   PI   等价。

## 🌈 **3、作用域**

- ==局部变量必须初始化==
- 类变量前加上 static 关键字，方便调用

```java
public class Main {

    static int flags =0;//从属于类，类变量
    
    int a ;//从属于对象，实例变量，默认会是对应类型的默认值，0，false，null
    
    public static void main(String[] args) {
        int b;//局部变量，必须初始化
    }
    
    public static void methods(){
        int c;//局部变量，必须初始化
    }
}
```



## ⛱ 4、变量的命名规范

- 所有变量、方法、类名：见名知意；
- 类成员变量：首字母小写和驼峰原则：addMax；
- 局部变量：首字母小写和驼峰原则：
- 常量：全大写，并用下划线分割：MAX_VALUE；
- ==类名：首字母大写和驼峰原则：AddMax；==
- 方法名：首字母小写和驼峰原则。

---





# 5️⃣ **五、基本运算符**

## 🚋 **1、Java中的基本运算符**

|                            运算符                            |                             举例                             |
| :----------------------------------------------------------: | :----------------------------------------------------------: |
|                             a++                              |                        先赋值，后自增                        |
|                             ++a                              |                        先自增，后赋值                        |
|                              %                               |                     取余，取模，得到余数                     |
|                       短路 ：与  、 或                       | a&&b（a为false，b不执行）    、    a \|\|b （a为true，b不执行）  ，会发生短路现象 |
|                        a>b ？a ：  b                         |        三元运算符，a 如果大于 b ,结果为 a ，否则为 b         |
| 位运算    &（与） 、 \|（或） 、 ^（异或）、 ~ （取反） 、>> （右移） 、<< （左移） 、>>> |                  2 << 3 =  16  （在幂上加）                  |
|                                                              |                                                              |



## 🎈  **2、字符串连接符**

`+` 与基本类型的使用

==举例==

```java
public class Main {
    public static void main(String[] args) {
        int a =10;
        int b = 20;
        System.out.println(""+a+b);//结果为  1020  ，转化为了  字符串的拼接
        System.out.println(a+b+"");//结果为  30 ， 进行加法操作
    }
}
```



---



# 6️⃣ 六、 **使用javaDoc生成自己的API文档**

## 🚋 **第一步**   打开Java文件所在位置

![](C:\Users\Haobin\Desktop\images\Snipaste_2023-01-18_22-06-53.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 🎈  **第二步**    在文件路径下打开命令行窗口

![](C:\Users\Haobin\Desktop\images\Snipaste_2023-01-18_22-10-19.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 🌈 **第三步**    在命令行窗口输入相应指令

​			==javadoc -encoding utf-8 -charset utf-8 Main.java==，注意：Main.java 是对应 java 的文件名

![](C:\Users\Haobin\Desktop\images\Snipaste_2023-01-18_22-15-26.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## ⛱ **第四步**    在所生成的文件中查看 index.html ，用浏览器查看API的主页了

![](C:\Users\Haobin\Desktop\images\Snipaste_2023-01-18_22-21-31.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)







![](C:\Users\Haobin\Desktop\images\Snipaste_2023-01-18_22-22-16.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



# 7️⃣ **七、Scanner类的使用**

## 🚋  基本语法

`java.util.Scanner`是Java5的一个新特性，使用Scanner 类来获取用户的输出

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        String s = sc.nextLine();// 可以接收空格，判断回车
        String s1 = sc.next();// 判断空格或是回车
        int i = sc.nextInt();// int 类型
        float f = sc.nextFloat();// float 类型
        
        //凡是属于IO流的类如果不关闭会一直占用资源，要使用close()关闭
        sc.close();
    }
}
```



- ==next（）==：一定要读取到有效字符后才可以结束输入，对于有效字符之前遇到的空白，会自动将其去掉
- ==nextLine()==：可以得到带有空格的字符





# 8️⃣ **八、Java流程控制**

## 🚋 基本流程分类

- ##### 顺序结构 ：一种基本的算法结构，按顺序一次执行

- ##### if 选择结构 

```java
public class Main {
    public static void main(String[] args) {
        if(表达式){
            语句块
            if(表达式){ //——>if 语句可以嵌套使用
                语句块
            }
        }else if(表达式){
            语句块
        }else{
            语句块
        }
    }
}
```



- ##### switch 选择结构  （`尽量在每个case后都加上break语句，防止case穿透`）

```java
public class Main {
    public static void main(String[] args) {
        switch (表达式){
            case 判断值 :
                语句块;
                break;
            case 判断值 :
                语句块;
                break;
            default:
                语句块;
                break;
        }
    }
}
```

- ##### while 循环结构     ——>死循环   while(true){}

  ```java
  public class Main {
      public static void main(String[] args) {
          while(表达式){
              语句块
          }
      }
  }
  ```

- ##### do...while循环  （无论如何，循环体语句都会执行一次）

  ```java
  public class Main {
      public static void main(String[] args) {
          do {
              循环体
          }while(表达式);
      }
  }
  ```

- ##### for 循环   （快捷键：10.fori ）  ——>  死循环  for(  ;  ; ){}

  ```java
  public class Main {
      public static void main(String[] args) {
          for (int i = 0; i < 10; i++) {
              //初始化 ; 布尔表达式;变量更新
              /*
                  其中，int i =0 只执行了一次
                  后执行 i<10  
                  再执行 语句块
                  最后执行 i++
               */
              //添加语句块
          }
      }
  }
  ```

- 增强  for 循环  （Foreach）通常用于数组、集合和容器中

```java
public class Main {
    public static void main(String[] args) {
        int [] a  = {1,2,3,4};
        for (int x :a ){
            System.out.println(x);
        }
    }
}
```

  ==声明语句  int x==：声明新的局部变量，该变量的类型必须与数组元素的类型匹配，其作用域限定在循环语句块中，其中与每一时刻数组元素的值相等；

==表达式  a==:表达式是要访问的数组名，或者是返回值为数组的方法。



# 9️⃣ **九、break 、continue 和 goto**

|    类型     |                             用法                             |
| :---------: | :----------------------------------------------------------: |
| 🚋    break  |           用于强行退出循环，不执行循环中剩余的语句           |
| 🎈  continue | 用于停止执行当前的迭代，然后退回循环的起始处，开始下一次迭代 |
| 🌈      goto | Java中的一个保留字，思想是：若条件A成立，则跳到这里；否则跳到那里， |



---

> ####  **说在最后📝*：*
>
> ​	✍创作不易，如果觉得文章写得还可以的话，就不要吝啬你的 👍 啦~ ✍

---

