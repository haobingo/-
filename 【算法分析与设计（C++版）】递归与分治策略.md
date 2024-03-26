[TOC]

# ⭐️写在前面的话⭐️

> CSDN主页：[程序员好冰](https://blog.csdn.net/m0_67689541?spm=1000.2115.3001.5343)
>
> 目前在学习：数字图像处理、算法设计与分析
>
> 技术栈：SpringBoot开发、小程序开发
>
> 推荐书籍：《编译原理》、《软件工程》
>
> 博客网站：暂无
>
> ==旅途的意义亦在旅途中。==
>
> 🎉欢迎 【点赞👍 关注🔎 收藏⭐️ 留言📝】
> 📌本文由 程序员好冰 原创，CSDN 首发！
> 📆入站时间： 🌴2022 年 07 月 13 日🌴
>
> 🍭<strong><font color = red> 作者水平很有限，如果发现错误，一定要及时告知作者哦！感谢感谢！</font></strong>🍭



# 先导知识

分段函数、数学归纳法

# 一、是什么？

> 百度百科搜一下，本质,特点，优缺点。

## 递归

`百度`

```xml
To iterate is human,to recurse divine.	             
					---L.Peter Deutsch
```

递归，在数学与计算机科学中，是指在方法的定义中使用方法自身。

也就是说，递归算法是一种直接或者间接调用自身方法的算法。

简言之：***在定义自身的同时又出现自身的直接或间接调用。***

递归函数的 **两要素**：1. 边界条件 2. 递归方程

`优点`

递归算法解题通常显得很简洁，

`缺点`

递归算法解题的**运行效率较低**。在递归调用的过程当中==系统为每一层的返回点、局部量等开辟了栈来存储==。

递归次数过多容易造成栈溢出等，所以一般**不提倡用递归算法**设计程序。

## 分治

`百度`

在计算机科学中，分治法是一种很重要的算法。分治算法，字面上的解释是“**分而治之**”，分治算法主要是三点：

1. 将一个复杂的问题分成两个或更多的相同或相似的子问题，再把子问题分成更小的子问题—-**“分”**
2. 将最后子问题可以简单的直接求解—-**“治”**
3. 将所有子问题的解合并起来就是原问题打得解—-**“合”**

这三点是分治算法的主要特点，只要是符合这三个特点的问题都可以使用分治算法进行解决(==注意用词==，是”用”, 至于好不好就是另外一回事了)

`优点`

分治算法的特点使得它很容易实现并行计算。因为子问题之间相互独立，可以同时对多个子问题进行处理，从而加速整体求解过程。同时，治算法的结构相对清晰明了，易于理解和实现。通常可以通过递归或迭代的方式编写代码，使得算法的实现较为简洁。

`缺点`

分治算法通常需要额外的存储空间来存储子问题的解，以及在递归过程中所需要的中间变量。这可能导致算法的空间复杂度较高。

有些问题的合并过程可能比较复杂，需要额外的计算和处理，这可能会增加算法的复杂度和实现难度。

# 二、为什么有这个？（历史）

> 怎么来的？没有这个东西之前用的是什么？使用场景？

早期的计算机语言如**LISP**就广泛使用了**递归算法**

 递归的思想部分地源自**数学归纳法**。

数学归纳法通过证明基本情况成立，并证明如果对于某个整数*n*成立，那么对于*n*+1也成立，从而推断对于所有自然数都成立。这种自然的推广思想在递归算法中也有所体现，即将问题不断化简为更小的同类问题直到基本情况。

 **分治算法**的术语在20世纪50年代开始出现。

美国计算机科学家约翰·冯·诺伊曼（John von Neumann）在他的工作中使用了"**divide and conquer**"（分而治之）这个术语，指代一种将复杂问题分解为更简单的子问题来解决的方法。

古希腊数学家欧几里德提出的**辗转相除法**就是一种分治思想的应用，用于求解最大公约数问题。

# 三、具体的应用

> 能够解决什么问题？举例案例进行巩固,需要真正掌握的有哪些？分析时间复杂度，空间复杂度？图解、伪代码。

## 0、递归算法伪代码

```c++
type digui(int n,...){
    if(中止条件){
        return ;
    }
    return digui(n-1,...)...;//递归方程
}
```

## 1、阶乘函数

>当n=0时，n! =1；
>
>当n>0时，n! =n(n-1).

推荐博客：[递归算法1——简单递归之求n的阶乘_递归求n的阶乘-CSDN博客](https://blog.csdn.net/baidu_36669549/article/details/104130503)

==回推==

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20200201101339444.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

==递推==

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20200201101346316.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```c++
int factorial(int n){
    if(n==0){
        return 1;
    }
    return n*factorial(n-1);
}
```

`时间复杂度`：

- 在最坏情况下，函数会递归调用n次，直到n减小到0为止。
- 每次递归调用都会执行一次乘法操作（n * factorial(n-1)）和一次减法操作（n-1）。
- 因此，时间复杂度可以表示为**O(n)**，即线性时间复杂度。

`空间复杂度`：

- 由于函数是递归实现的，每次递归调用都会将当前函数的局部变量、参数和返回地址等信息保存在栈内存中。
- 递归调用n次，因此栈的深度为n。
- 所以，空间复杂度可以表示为**O(n)**，即线性空间复杂度。

## 2、斐波那契数列

> 1,1,2,3,5,8,13,21,34,55,...
>
> 当n>1时，这个数列的第n项的值是它前面两项之和。

![image-20240325081531815](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20240325081531815.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20240325081503350](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20240325081503350.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```c++
int fibonacci(int n){
    if(n<=1){
        return 1;
    }
    return fibonacci(n-1)+fibonacci(n-2);
}
```

**非递归方式定义**

![斐波那契数列c语言_斐波那契数列通项公式与黄金分割率-CSDN博客](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/2d34bf23c1679b42f8b3b73221dbe27d.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

`时间复杂度`：

时间复杂度方面，由于每次调用`fibonacci(n-1)`和`fibonacci(n-2)`都会产生新的递归调用，这导致了指数级的时间增长。具体来说，对于每一个n值，都会产生两个新的n-1和n-2的递归调用，直到基本情况n=1或n=2被满足。因此，这个算法的时间复杂度是**O(2^n)** 。

`空间复杂度`：

空间复杂度方面，虽然每次递归调用都会占用栈空间，但是由于每次递归调用都只涉及到局部变量（即`n-1`和`n-2`），并且在递归返回时这些局部变量会被销毁，所以整体的空间复杂度是**O(1)** 。

## 3、Ackerman双递归函数

参考阅读：

[思维的有限边界：阿克曼函数](https://zhuanlan.zhihu.com/p/93644792)

[Ackermann函数（阿克曼函数）的递归、非递归（手动栈模拟）](https://blog.csdn.net/qq_26119041/article/details/111941618)

Ackerman 函数。并非一切[递归函数](https://so.csdn.net/so/search?q=递归函数&spm=1001.2101.3001.7020)都能用非递归方式定义。

**当一个函数及它的一个变量由函数自身定义**时，称这个函数是双递归函数。

Ackerman 函数 A(n,m)有两个独立的整型变量m≥0 和n≥0，其定义如下：

![image-20240325091509547](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20240325091509547.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**注意**：我们这里  m 和 n 互换了位置，但是最终的结果不变。

参考量定义**递归方程**（当存在两个自变量时，应当先确定一个，然后再去研究关于另一个自变量的函数变化）：

![image-20240325085712045](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20240325085712045.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**边界条件**：当m < 0 且 n < 0 时跳出函数

```c++
int ackerman(int m, int n) {
    if (m == 0) {
        return n + 1;
    } else if (m > 0 && n == 0) {
        return ackerman(m - 1, 1);
    } else if (m > 0 && n > 0) {
        return ackerman(m-1, ackerman(m,n-1));
    }
}
```

`时间复杂度`

由于Ackerman函数的递归调用会不断地产生新的函数调用，导致计算时间随着参数m和n的增加而指数级增长。特别是在递归深度较大时，即使是在计算较小的参数值时，也会非常耗时。因此，这个算法的时间复杂度是**指数级**的，具体来说，是(**O(2^{(m+n)})**)，因为每次递归调用都会使问题规模减小到原来的1/2（在某些情况下），但同时也会增加递归深度，这导致了指数级的时间复杂度。

`空间复杂度`

由于每次递归调用都会占用栈空间，并且递归深度可以达到非常大，所以空间复杂度也是指数级的，即(**O(2^{(m+n)})**)。这是因为随着递归深度的增加，需要更多的栈空间来存储中间结果。

## 4、排列问题

> 从n个不同元素中任取m（m≤n）个元素，按照一定的顺序排列起来，叫做从n个不同元素中取出m个元素的一个排列。
>
> 当m=n时所有的排列情况叫**全排列**。
>
> **全排列的含义就是一个序列所有的排序可能性**
>
> N个元素进行全排列后的排列数量为==N！==个。

参考阅读：

[递归全排列问题（两种方法 Java实现）](https://blog.csdn.net/qq_29339467/article/details/106257953)

[全排列问题（图文详解）](https://blog.csdn.net/ThinPikachu/article/details/105514367)

[全排列算法讲解](https://blog.csdn.net/m0_56069910/article/details/130541706)

![C#算法之全排列递归算法实例讲解 / 张生荣](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20170410093109333.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



特点总结：

- 对于给定的序列，刚开始时我们知道序列的第一个元素，剩余的序列元素此时又可以看成是一个全排列的例子；

- 我们可以对剩余的序列进行与开始相同的操作，直到中只一个元素为止。这样我们就获得了所有的可能性。

`下面是我的书写推导`：

![结果2](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/%E7%BB%93%E6%9E%9C2.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 递归不去重的情况

```c++
#include <iostream>

using namespace std;
int count = 0;

void permute(string str,int left,int right){
    if(left == right){//左标记到达右标记，只有一种方式可选，故打印
        cout<<str<<endl;
        count++;
    }else{
        for(int i=left;i<=right;i++){
            swap(str[left],str[i]);
            permute(str,left+1,right);
            swap(str[left],str[i]);
        }
    }
}

int main() {
    string str = "12345";
    int size = str.size();
    permute(str,0,size-1);
    cout<<"共"<<count<<"种"<<endl;
    return 0;
}
```

`时间复杂度`

- 在这个算法中，使用了递归来生成字符串的全排列。
- 对于每个位置，有 n 种可能的选择，其中 n 是字符串的长度。因此，总的时间复杂度可以表示为 O(n!)，即阶乘级别的复杂度。
- 在递归调用中，每次递归都会减少一个位置的选择范围，直到所有位置都确定下来。因此，时间复杂度是 **O(n!)**。

`空间复杂度`

- 算法中并没有使用额外的数据结构，主要的空间消耗是递归调用时的函数调用栈。
- 递归调用的层数取决于字符串的长度 n，因此空间复杂度可以表示为 **O(n)**，即线性级别的复杂度。

需要注意的是，阶乘级别的时间复杂度在输入规模较大时会非常高，因此在实际应用中需要谨慎使用。

##  5、整数划分问题

> **题目描述**
>
> 整数划分问题是将一个正整数n拆成一组数连加并等于n的形式，且这组数中的最大加数不大于n。
> 即：n=n1+n2+…+nk;
> n1>=n2>=n3…>=nk
> 如整数的6划分为:
> 6
> 5 + 1
> 4 + 2, 4 + 1 + 1
> 3 + 3, 3 + 2 + 1, 3 + 1 + 1 + 1
> 2 + 2 + 2, 2 + 2 + 1 + 1, 2 + 1 + 1 + 1 + 1
> 1 + 1 + 1 + 1 + 1 + 1共11种。
>
> 补充：正整数的这种操作称为正整数的划分，正整数的不同划分个数称为正整数n的划分数，记为p(n)。例如：p(6)=11;

推荐视频：[整数划分问题](https://www.bilibili.com/video/BV1QN4y1p7hK/?spm_id_from=333.337.search-card.all.click&vd_source=9beb96d6b8d54789ae03a969dbb82622)

推导：

==q（n，m）表示用不大于m的数组成n的所有可能的个数。==

![【算法】整数划分问题_整数划分问题 将正整数 n 表示成一系列正整数之和,称之为一个划分。-CSDN博客](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20200415092135953.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**当m>n时**

举例：q(3,5),用不大于5的数来组成3，其实只有1，2，3，这几种选择，4，5不能选。故`q(n,m)=q(n,n)`;

**当m=n时**

举例：q(3,3)，用不大于3的数来组成3，首先提出3，3可以直接组成3，其次就是用不大于2的数组成3，即：q(3,2)。故`q(n,m)=q(n,n)=1+q(n,n-1)`；

**当m<n时**

举例：q(5,3)，用不大于3的数来组成5，首先考虑必须不包含3的情况，即用不大于2的数来组成5，即：q(5,2),其次考虑必须包含3的情况，即5-3后剩下2，即q(2,3)  （`注：这里又跳转到m>n的情况`）。故`q(n,m)=q(n,m-1)+q(n-m,m)`。

**当m=1时，同时也是递归的边界条件**

举例：q(5,1) 用不大于1的数来组成5，当然只有`一种情况`，就是 1+1+1+1+1 = 5。

**当n=1时，同时也是递归的边界条件**

举例：q(1,5)用不大于5的数来组成1，`注：这里又跳转到m>n的情况`,q(1,1)，用不大于1的数来组成1，当然也只有`一种情况`。

递归式：

![整数划分问题——递归_整数划分 递归-CSDN博客](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20200503160301528.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```c++
int q(int n,int m){
    if(n<1||m<1){
        return 0;//负数返回0
    }
    if(n==1||m==1){
        return 1;//递归的边界条件
    }
    if(n<m){
        return q(n,n);
    }
    if(n==m){
        return 1+q(n,n-1);
    }
    if(n>m){
        return q(n,m-1)+q(n-m,m);
    }
    return 0;
}
```

`时间复杂度`

- 在函数中，有一些条件语句和递归调用，我们来看每一部分的时间复杂度：
  - 条件语句 `if(n<1||m<1)` 和 `if(n==1||m==1)` 只需常数时间内判断条件，时间复杂度为 O(1)。
  - 条件语句 `if(n<m)` 和 `if(n==m)` 中的递归调用 `q(n,n)` 和 `q(n,n-1)`，分别进行了 n 次和 n-1 次的递归调用，时间复杂度为 O(n)。
  - 条件语句 `if(n>m)` 中的递归调用 `q(n,m-1)` 和 `q(n-m,m)`，可能进行的递归调用次数取决于 n 和 m 的大小关系，但是总体来说，这部分的时间复杂度为 O(2^n)，因为每次递归调用都可能导致两个更小的子问题。
- 综合考虑，函数的时间复杂度为 **O(2^n)**。

`空间复杂度`

- 函数中除了递归调用外，并没有使用额外的空间，递归调用时会有一些函数调用栈的空间占用，但是这个空间占用量与递归调用次数相关，随着递归层级的增加而增加，因此空间复杂度可以用递归调用的最大层级来表示，即为 **O(n)。**

## 6、汉诺塔问题

推荐文章：[一文带你吃透汉诺塔和其变形题](https://zhuanlan.zhihu.com/p/435052098)

**汉诺塔问题**是一个经典的问题。汉诺塔（Hanoi Tower），又称河内塔，源于印度一个古老传说。大梵天创造世界的时候做了三根金刚石柱子，在一根柱子上从下往上按照大小顺序摞着64片黄金圆盘。

大梵天命令婆罗门把圆盘从下面开始按大小顺序重新摆放在另一根柱子上。并且规定，任何时候，在小圆盘上都不能放大圆盘，且在三根柱子之间一次只能移动一个圆盘。

问应该如何操作？(三根柱子分别为A,B,C)

**提示：**两个盘子，你会怎么做？

A —— B；A——C；B——C。

<img src="https://pic2.zhimg.com/v2-9fb2a450ba5a1a2dd425fdd3714a49a9_b.webp" stylt="zoom:100%"/>

```c++
void hanoi(int n,char 'A',char 'B',char 'C'){//参数说明：阶数，源点，借助点，目标点
    if(n>0){
        hanoi(n-1,'A','C','B');
        move('A','C');
        hanoi(n-1,'C','A','B');
    }
}
```

按照课本上的例子：A是源，B是目标，C是辅助塔。

- 我们从只有一个盘子的时候开始研究。很简单，直接把红色的盘子移到B上就可以了。

<img src="https://pic2.zhimg.com/v2-757bf1f710e7ccd1631139ebb5584629_b.webp" stylt="zoom:100%"/>

- 来研究两个盘子的情况

<img src="https://pic2.zhimg.com/v2-89651ea20997ea398e90998a9acaa8b9_b.webp" stylt="zoom:100%"/>

- 再来看三个盘子的情况

<img src="https://pic2.zhimg.com/v2-a49bb6ef1a48317c9de2477e26fa8935_b.webp" stylt="zoom:100%"/>

## 0、分治算法伪代码

```c++




```

## 1、二分搜索技术





## 2、大整数的乘法





## 3、Strassen矩阵乘法





## 4、棋盘覆盖





## 5、合并排序（归并排序）

![java递归算法（一）——详解以及几个经典示例_java递归简单例子-CSDN博客](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20181205220604400.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 6、快速排序





## 7、线性时间选择





## 8、最接近点对问题





## 9、循环赛日程表
















---

>  ==**<font color=red>🚀 先看后赞，养成习惯！🚀</font>**==
>
> ==**<font color=red>🚀 先看后赞，养成习惯！🚀</font>**==

> <font color=red>**🎈觉得文章写得不错的老铁们，点赞评论关注走一波！谢谢啦！🎈**</font>

---



