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



# 一、初识GUI

>  组件：
>
>  - 窗口
>  - 弹窗
>  - 面板
>  - 文本框
>  - 列表框
>  - 按钮
>  - 图片
>  - 监听事件
>  - 鼠标事件
>  - 键盘事件

## 1.1 简介

> GUI的核心技术：Swing、AWT

`图形用户界面`

## 1.2 不流行的原因

- 界面不美观
- 需要jre环境，占用较大空间

## 1.3 为什么要学习？

- 与MVC结构有关，了解监听器
- 可以维护Swing界面
- 可操作性强，可以自己手动编写

# 二、AWT

>  Abstract Windows Tools,==抽象窗口工具==，包含了很多类和接口。

## 2.1 找到awt包所在的位置

- 找到自己电脑JDK的目录

![image-20230315094452359](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315094452359.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 点开与bin同级的jre目录

![image-20230315094602156](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315094602156.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- lib目录，也就是library的意思

![image-20230315094657463](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315094657463.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 找到rt.jar，并用解压软件打开

![image-20230315094748724](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315094748724.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230315094852544](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315094852544.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 依次打开java-----awt

![image-20230315094922181](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315094922181.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20230315094942382](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315094942382.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 2.2 组件的基本分类

![image-20230315161411500](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315161411500.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 2.3 简单使用

### 2.3.1 展示一个窗口

```java
package space.haobin;

import java.awt.*;

public class TestFrame {
    public static void main(String[] args) {
       //new一个Frame对象
        Frame frame = new Frame("我的一个Java图形界面窗口！");

        //需要设置可见性
        frame.setVisible(true);

        //设置窗口大小
        frame.setSize(400,400);

        //设置颜色
        //new Color();
        frame.setBackground(new Color(79, 171, 183));

        //窗口弹出的初始位置,(0,0)点在电脑屏幕的左上角，其中y轴向下为正
        frame.setLocation(200,200);

        //默认窗口是可以拉伸的
        //但是在实际的运用当中，应该不可拉伸
        frame.setResizable(false);

    }
}

```

运行效果：

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315163642939.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230315163642939" style="zoom:33%;" />

==问题==

​		窗口默认不能够被关闭

### 2.3.2 展示多个窗口

```java
package space.haobin;

import java.awt.*;

public class TestFrame {
    public static void main(String[] args) {

        int x= 100;
        int y =100;
        int width=250;
        int height=250;
        
       //new一个Frame对象
        for (int i = 0; i < 10; i++) {
            new MyFrame(x+=20,y+=20,width,height,Color.GRAY);
        }
    }
}

//设置自己使用的窗口样式模板
class MyFrame extends Frame{

    //计数器，统计窗口的个数
    static int id = 0;

    //添加构造器
    public MyFrame(int x,int y,int width,int height,Color color){

        //调用父类Frame中的有参构造
        /* public Frame(String title) throws HeadlessException {
            init(title, null);
        }*/
        super("我的第"+(++id)+"个Frame窗口");

        //可见性
        setVisible(true);

        /*大小和位置可以使用setBounds()方法代替*/
        //setBounds(x,y,width,height);
        //窗口大小
        setSize(width,height);
        //初始位置
        setLocation(x,y);

        //背景颜色
        setBackground(color);
        //大小固定
        setResizable(false);
        
    }
}
```

运行效果：

![image-20230315170300596](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315170300596.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 2.4 Panel面板

> 特点：
>
> - 可以看成是一个空间
> - 不能单独存在
> - 与Frame的区别是：可以内嵌东西

==一般来说，组件应该放在面板Panel上==

### 2.4.1 简单使用

```java
package space.haobin;

import java.awt.*;

public class PanelDemo {
    public static void main(String[] args) {
        Frame frame = new Frame();

        //存在布局的概念
        Panel panel = new Panel();

        /*对于frame*/
        //可以设置布局
        frame.setLayout(null);//默认会使窗口置顶

        frame.setBounds(300,300,500,500);
        frame.setBackground(new Color(104, 150, 155));

        /*对于panel*/
        //panel的坐标参数是相对于frame的
        panel.setBounds(50,50,300,300);

        panel.setBackground(new Color(29, 189, 112));

        //将panel加到frame上
        //frame.add(Component comp)->参数是组件
        //Panel extends Container->继承的是容器
        //Container extends Component->容器的本质也是组件
        frame.add(panel);

        frame.setVisible(true);

    }
}
```

运行效果：

![image-20230315202212237](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315202212237.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 2.5 解决窗口默认无法关闭的问题

`添加窗口关闭事件`，需要对窗口进行操作。

```java
//监听窗口关闭事件 WindowListener--closing
//System.exit(0);
//设计模式：适配器模式

//WindowAdapter implements WindowListener
//WindowAdapter实现了监听窗口的接口
frame.addWindowListener(new WindowAdapter() {
    //重写窗口关闭的时候需要做的事情
    @Override
    public void windowClosing(WindowEvent e) {
        //super.windowClosing(e);
        //退出程序
        /*
            0 表示正常退出
            1 表示异常退出
        */
        System.exit(0);
    }
});
```

## 2.6 布局管理器

### 2.6.1 ==流式布局==

> frame.setLayout(new FlowLayout());

```java
package space.haobin;

import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class FlowLayoutDemo {
    public static void main(String[] args) {
        Frame frame = new Frame();

        //按钮
        Button button1 = new Button("button1");
        Button button2= new Button("button2");
        Button button3 = new Button("button3");

        //设置为流式布局,默认center居中
        /*public FlowLayout() {
            this(CENTER, 5, 5);
        }*/
        frame.setLayout(new FlowLayout());
        frame.setLayout(new FlowLayout(FlowLayout.LEFT));
        //现在是居左，后面的会对前面的造成覆盖


        frame.setSize(200,200);

        //Button extends Component
        //按钮也属于组件
        frame.add(button1);
        frame.add(button2);
        frame.add(button3);

        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });

        frame.setVisible(true);
    }
}
```

运行效果：

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315205334758.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230315205334758" style="zoom:50%;" />

### 2.6.2 ==东西南北中==

```java
package space.haobin;

import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class BorderLayoutDemo {
    public static void main(String[] args) {
        Frame frame = new Frame("BorderLayoutDemo");

        Button east = new Button("EAST");
        Button west = new Button("WEST");
        Button south = new Button("SOUTH");
        Button north = new Button("NORTH");
        Button center = new Button("CENTER");


        // public void add(Component comp, Object constraints);
        //参数:(组件，约束)
        frame.add(east,BorderLayout.EAST);
        frame.add(west,BorderLayout.WEST);
        frame.add(south,BorderLayout.SOUTH);
        frame.add(north,BorderLayout.NORTH);
        frame.add(center,BorderLayout.CENTER);

        frame.setBounds(200,200,500,500);

        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });
        frame.setVisible(true);
    }
}
```

运行效果：

![image-20230315210614303](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230315210614303.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 2.6.3 ==表格布局==

```java
package space.haobin;

import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class GridLayoutDemo {
    public static void main(String[] args) {
        Frame frame = new Frame("GridLayoutDemo");

        Button button1 = new Button("btn1");
        Button button2 = new Button("btn2");
        Button button3 = new Button("btn3");
        Button button4 = new Button("btn3");
        Button button5 = new Button("btn5");
        Button button6 = new Button("btn6");

        //参数:行,列.-------rows,cols
        frame.setLayout(new GridLayout(3,2));

        frame.add(button1);
        frame.add(button2);
        frame.add(button3);
        frame.add(button4);
        frame.add(button5);
        frame.add(button6);

        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });

        frame.setLocation(200,200);

        //Causes this Window to be sized to fit the preferred size
        //pack()是Window的函数,可以调整到一个最合适的大小
        frame.pack();
        frame.setVisible(true);
    }
}
```

运行效果:

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230316160509516.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230316160509516" style="zoom:33%;" />



## 2.7 测试

> 使用嵌套panel、button等实现下面的图

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230316204215696.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230316204215696" style="zoom:50%;" />

### 方法一:

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230316204348808.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230316204348808" style="zoom:50%;" />

代码实现:

```java
package space.haobin;

import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class ComLayoutTest {
    public static void main(String[] args) {
        Frame frame = new Frame("一个复杂的窗口!");
        /*
        有关frame的布局
        */
        frame.setLayout(new GridLayout(1,3));

        /*
        有关panel的布局
         */
        Panel panel_left = new Panel(new GridLayout(2,1));
        Panel panel_center= new Panel(new GridLayout(2,1));
        Panel panel_right = new Panel(new GridLayout(2,1));

        Panel panel_up = new Panel();
        Panel panel_down = new Panel();

        panel_center.add(panel_up,BorderLayout.NORTH);
        panel_center.add(panel_down,BorderLayout.SOUTH);

        frame.add(panel_left,BorderLayout.WEST);
        frame.add(panel_center,BorderLayout.CENTER);
        frame.add(panel_right,BorderLayout.EAST);

        panel_left.add(new Button("1"));
        panel_left.add(new Button("5"));

        panel_up.setLayout(new GridLayout(2,1));
        panel_up.add(new Button("2"));
        panel_up.add(new Button("3"));

        panel_down.setLayout(new GridLayout(2,2));
        panel_down.add(new Button("6"));
        panel_down.add(new Button("7"));
        panel_down.add(new Button("8"));
        panel_down.add(new Button("9"));


        panel_right.add(new Button("4"));
        panel_right.add(new Button("10"));

        frame.setBounds(500,200,600,400);

        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });

        frame.setVisible(true);
    }
}
```

运行效果:

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230316204451662.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230316204451662" style="zoom:33%;" />

### 方法二:

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230316211002160.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230316211002160" style="zoom:50%;" />

代码实现:

```java
package space.haobin;

import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class ComLayoutTest02 {
    public static void main(String[] args) {
        Frame frame = new Frame("一个复杂的窗口!");

        frame.setLayout(new GridLayout(2,1));

        Panel panel_up = new Panel(new GridLayout(1,3));
        Panel panel_up_center = new Panel(new GridLayout(2,1));
        Panel panel_down = new Panel(new GridLayout(1,3));
        Panel panel_down_center = new Panel(new GridLayout(2,2));

        panel_up.add(new Button("1"),BorderLayout.WEST);
        panel_up.add(new Button("4"),BorderLayout.EAST);

        panel_up_center.add(new Button("2"),BorderLayout.NORTH);
        panel_up_center.add(new Button("3"),BorderLayout.SOUTH);
        panel_up.add(panel_up_center,FlowLayout.CENTER);
        
        panel_down.add(new Button("5"),BorderLayout.WEST);
        panel_down.add(new Button("10"),BorderLayout.EAST);

        panel_down_center.add(new Button("6"));
        panel_down_center.add(new Button("7"));
        panel_down_center.add(new Button("8"));
        panel_down_center.add(new Button("9"));
        panel_down.add(panel_down_center,FlowLayout.CENTER);

        frame.add(panel_up);
        frame.add(panel_down);

        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });

        frame.setBounds(200,200,500,500);
        frame.setVisible(true);
    }
}
```

运行效果:

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230316211031021.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230316211031021" style="zoom: 33%;" />

## 2.8 事件监听

> 当某个事件发生的时候，需要做什么反应。

### 2.8.1 使用三种方法达到事件监听的目的

```java
public interface ActionListener extends EventListener {

    /**
     * Invoked when an action occurs.
     */
    public void actionPerformed(ActionEvent e);//只有一个方法
}
```

- 构造一个自己的事件监听类
- 使用匿名内部类
- 使用Lambda表达式

```java
package space.haobin;

import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class ActionDemo {
    public static void main(String[] args) {
        Frame frame = new Frame("事件监听测试.");

        frame.setLayout(new GridLayout(3,1));
        //按下按钮，触发事件
        Button button = new Button("btn1");

        //参数:ActionListener,需要什么事件
        //public void actionPerformed(ActionEvent e);
        //参数需要ActionListener，我们可以自己构造自己的MyActionListener
        MyActionListener myActionListener = new MyActionListener();
        button.addActionListener(myActionListener);

        //匿名内部类的方式
        Button button2 = new Button("btn2");
        button2.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                System.out.println("这是btn2造成的事件响应!");
            }
        });

        //这里只有一个方法，可以使用lambda表达式
        Button button3 = new Button("btn3");
        button3.addActionListener(e-> System.out.println("这是btn3造成的事件响应!"));
        
        frame.add(button);
        frame.add(button2);
        frame.add(button3);
        frame.setBounds(500,200,500,500);
        WindowClosing(frame);
        frame.setVisible(true);

    }
    //自己写一个关闭窗口的方法
    private static void WindowClosing(Frame frame){
        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });
    }
}

//事件监听
class MyActionListener implements ActionListener{
    @Override
    public void actionPerformed(ActionEvent e) {
        //这里可以写事件发生做出的反应
        System.out.println("这是btn1造成的事件响应!");
    }
}
```



### 2.8.2 两个按钮公用一个监听事件

> 可以实现多个按钮只写一个监听类

```java
package space.haobin;

import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class ActionDemo2 {
    public static void main(String[] args) {
        Frame frame = new Frame("两个按钮实现同一监听.");
        frame.setLayout(new GridLayout(2,1));

        //两个按钮实现同一监听：开始监听 and 结束监听
        Button button1 = new Button("start");
        Button button2 = new Button("stop");

        //这里可以显示地定义触发会返回的命令
        //如果不显示定义，则会输出默认label中的值
        button1.setActionCommand("start");
        button2.setActionCommand("stop");

        MyMonitor myMonitor = new MyMonitor();
        button1.addActionListener(myMonitor);
        button2.addActionListener(myMonitor);

        frame.add(button1);
        frame.add(button2);

        frame.setBounds(500,200,500,500);
        frame.addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });
        frame.setVisible(true);
    }
}
class MyMonitor implements ActionListener{
    @Override
    public void actionPerformed(ActionEvent e) {
        //可以从参数e中得到一些数据
        System.out.println("按钮被点击了:msg=>"+e.getActionCommand());
    }
}
```

### 2.8.3 输入框事件监听

> TextField

```java
package space.haobin;

import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class TestFiledDemo {
    public static void main(String[] args) {
        new MyFrame();
    }
}
class MyFrame extends Frame {
    public MyFrame(){
        TextField textField = new TextField();
        add(textField);

        //监听这个文本框输入的文字
        MyActionListener myActionListener = new MyActionListener();
        //按下enter就会触发这个输入框的事件
        textField.addActionListener(myActionListener);

        //设置替换编码
        //每输入一段字符，都会将它转换为 *
        textField.setEchoChar('*');


        setVisible(true);
        setBounds(500,200,500,500);
        addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });
    }
}

class MyActionListener implements ActionListener{
    @Override
    public void actionPerformed(ActionEvent e) {

        /*public Object getSource() {
            return source;
        }*/
        //返回过来的类型是Object类，可以向下转型成任何类，比如：TextField
        TextField source = (TextField) e.getSource();
        //使用getText()方法获得输入的文本
        System.out.println(source.getText());
        //每按下enter，就会将输入框中的文本清空
        source.setText("");
    }
}
```

### 2.8.4 简易计算器

简单写法：（==面向过程写法==）

```java
package space.haobin2;

import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class CalcDemo {
    public static void main(String[] args) {
        new Calculator();
    }
}

class Calculator extends Frame{
    public Calculator(){

        setTitle("Easy Calculator");
        /*3个文本框
        * 1个按钮
        * 1个标签
        * */
        TextField num1 = new TextField(10);
        TextField num2 = new TextField(10);
        TextField num3 = new TextField(20);

        Button button = new Button("=");
        button.addActionListener(new MyCalculatorListener(num1,num2,num3));

        Label label = new Label("+");

        setLayout(new FlowLayout());

        add(num1);
        add(label);
        add(num2);
        add(button);
        add(num3);

        setVisible(true);
        pack();
        setLocation(500,200);
        addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });
    }
}

class MyCalculatorListener implements ActionListener{

    private TextField num1,num2,num3;

    //重载构造方法
    public MyCalculatorListener(TextField num1,TextField num2,TextField num3){
        this.num1=num1;
        this.num2=num2;
        this.num3=num3;
    }

    @Override
    public void actionPerformed(ActionEvent e) {
        //1.获得加数和被加数
        int n1 = Integer.parseInt(num1.getText());
        int n2 = Integer.parseInt(num2.getText());
        //2.经过+法运算后，将该值放到第三个框中
        int n3 =n1+n2;
        num3.setText(Integer.toString(n3));
        //3.清除前两个框
        num1.setText("");
        num2.setText("");
    }
}
```

改进后的写法：（==使用组合，将calculator看成一个整体，一个对象==）

```java
package space.haobin2;

import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class CalcDemo {
    public static void main(String[] args) {
        new Calculator().loadFrame();
    }
}

class Calculator extends Frame{

    TextField num1,num2,num3;

    public void loadFrame(){
        setTitle("Easy Calculator");
        num1 = new TextField(10);
        num2 = new TextField(10);
        num3 = new TextField(20);

        Button button = new Button("=");
        Label label = new Label("+");
        setLayout(new FlowLayout());
        add(num1);
        add(label);
        add(num2);
        add(button);
        add(num3);

        //事件监听
        button.addActionListener(new MyCalculatorListener(this));
        
        addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });

        //布局
        pack();
        setLocation(500,200);
        setVisible(true);
    }
}

class MyCalculatorListener implements ActionListener{

    Calculator calculator = null;

    //重载构造方法
    public MyCalculatorListener(Calculator calculator){
        this.calculator = calculator;
    }

    @Override
    public void actionPerformed(ActionEvent e) {
        //1.获得加数和被加数
        int n1 = Integer.parseInt(calculator.num1.getText());
        int n2 = Integer.parseInt(calculator.num2.getText());
        //2.经过+法运算后，将该值放到第三个框中
        int n3 =n1+n2;
        calculator.num3.setText(Integer.toString(n3));
        //3.清除前两个框
        calculator.num1.setText("");
        calculator.num2.setText("");
    }
}
```

再次改进：（==内部类写法==）

> 内部类最大的好处：可以畅通无阻地访问外部的属性和方法

```java
package space.haobin2;

import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class CalcDemo {
    public static void main(String[] args) {
        new Calculator().loadFrame();
    }
}

class Calculator extends Frame{

    //属性
    TextField num1,num2,num3;

    //方法
    public void loadFrame(){
        setTitle("Easy Calculator");
        num1 = new TextField(10);
        num2 = new TextField(10);
        num3 = new TextField(20);

        Button button = new Button("=");
        Label label = new Label("+");
        setLayout(new FlowLayout());
        add(num1);
        add(label);
        add(num2);
        add(button);
        add(num3);

        //事件监听
        button.addActionListener(new MyCalculatorListener());

        addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });

        //布局
        pack();
        setLocation(500,200);
        setVisible(true);
    }

    //监听器类(内部类)
    private class MyCalculatorListener implements ActionListener{
        
        @Override
        public void actionPerformed(ActionEvent e) {
            //1.获得加数和被加数
            int n1 = Integer.parseInt(num1.getText());
            int n2 = Integer.parseInt(num2.getText());
            //2.经过+法运算后，将该值放到第三个框中
            int n3 =n1+n2;
            num3.setText(Integer.toString(n3));
            //3.清除前两个框
            num1.setText("");
            num2.setText("");
        }
    }
}
```

使用Lambad表达式简化（不推荐）：

```java
package space.haobin2;

import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;
import java.util.EventListener;

public class CalcDemo {
    public static void main(String[] args) {
        new Calculator().loadFrame();
    }
}

class Calculator extends Frame {

    //属性
    TextField num1, num2, num3;

    //方法
    public void loadFrame() {
        setTitle("Easy Calculator");
        num1 = new TextField(10);
        num2 = new TextField(10);
        num3 = new TextField(20);

        Button button = new Button("=");
        Label label = new Label("+");
        setLayout(new FlowLayout());
        add(num1);
        add(label);
        add(num2);
        add(button);
        add(num3);
        
        /*public interface ActionListener extends EventListener {
            public void actionPerformed(ActionEvent e);
        }*/
        
        /*因为ActionListener接口中只需要重写一个方法
        因此可以使用Lambda表达式的方式*/
        
        //事件监听
        button.addActionListener(e -> {
            //1.获得加数和被加数
            int n1 = Integer.parseInt(num1.getText());
            int n2 = Integer.parseInt(num2.getText());
            //2.经过+法运算后，将该值放到第三个框中
            int n3 = n1 + n2;
            num3.setText(Integer.toString(n3));
            //3.清除前两个框
            num1.setText("");
            num2.setText("");
        });

        addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });

        //布局
        pack();
        setLocation(500, 200);
        setVisible(true);
    }
}
```

## 2.9 paint 画笔

>1. 画笔可以设置颜色
>2. 画笔可以画固定大小的图形
>3. 图形可以是空心的，也可以是实心的
>4. 每次使用完画笔之后，都应该将画笔的颜色还原

```java
package space.haobin2;

import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;

public class PaintDemo {
    public static void main(String[] args) {
        new MyPaint().loadFrame();
    }
}

class MyPaint extends Frame{
    //属性

    //方法
    public void loadFrame(){
        setBounds(400,200,600,400);
        setVisible(true);

        addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });
    }

    @Override
    public void paint(Graphics g) {
        //画笔可以设置颜色
        //画笔可以画出固定大小的图形
        g.setColor(Color.red);
        //画空心的图形
        g.drawOval(100,100,100,100);
        //画实心的图形
        g.fillOval(200,200,100,100);
    }
}
```

## 2.10 鼠标监听

> 实现鼠标画画

代码演示：

```java
package space.haobin3;

import java.awt.*;
import java.awt.event.MouseAdapter;
import java.awt.event.MouseEvent;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;
import java.util.ArrayList;
import java.util.Iterator;

public class MouseDemo {
    public static void main(String[] args) {
        new MyFrame("画图");
    }
}

class MyFrame extends Frame {

    //属性
    ArrayList points;

    //方法

    /*画画需要画笔，需要鼠标监听事件监听鼠标当前的位置，需要集合来存储这个点*/

    /*public Frame(String title) throws HeadlessException {
        init(title, null);
    }*/
    public MyFrame(String title) {
        super(title);

        setBounds(500, 200, 600, 500);

        //用集合将点存储起来
        points = new ArrayList<>();

        //针对这个窗口添加鼠标监听事件
        this.addMouseListener(new MyMouseListener());

        setVisible(true);

        addWindowListener(new WindowAdapter() {
            @Override
            public void windowClosing(WindowEvent e) {
                System.exit(0);
            }
        });
    }

    @Override
    public void paint(Graphics g) {
        //监听鼠标的事件

        //使用迭代器遍历这个点
        Iterator iterator = points.iterator();
        while (iterator.hasNext()) {
            Point point = (Point) iterator.next();
            g.setColor(Color.RED);
            g.fillOval(point.x,point.y,10,10);
        }
    }

    //将该点添加到界面上
    public void addPaint(Point point){
        points.add(point);
    }

    //内部类

    /*继承适配器(推荐)*/

    /*
    MouseAdapter implements MouseListener
    */
    private class MyMouseListener extends MouseAdapter {
        @Override
        public void mousePressed(MouseEvent e) {
            MyFrame source = (MyFrame) e.getSource();
            //目的，需要在鼠标点击后在窗口上产生一个点
            source.addPaint(new Point(e.getX(), e.getY()));

            //每次点击一次鼠标都需要重新画一遍
            source.repaint();
        }
    }
}
```

运行演示：

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230318210206560.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230318210206560" style="zoom: 33%;" />

思路分析：

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230318211130732.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230318211130732" style="zoom:50%;" />

==适配器模式的好处==

- 不用适配器，需要重写接口里的所有方法

```java
/*实现接口的方式需要重写所有的方法(不推荐)*/

private class MyMouseListener implements MouseListener{
    @Override
    public void mouseClicked(MouseEvent e) {}
    @Override
    public void mousePressed(MouseEvent e) {}
    @Override
    public void mouseReleased(MouseEvent e) {}
    @Override
    public void mouseEntered(MouseEvent e) {}
    @Override
    public void mouseExited(MouseEvent e) {}
}
```

- 使用适配器，需要哪个方法就重写哪个方法

```java
/*继承适配器(推荐)*/

/*
MouseAdapter implements MouseListener
*/
private class MyMouseListener extends MouseAdapter {
    @Override
    public void mousePressed(MouseEvent e) {
        MyFrame source = (MyFrame) e.getSource();
        //目的，需要在鼠标点击后在窗口上产生一个点
        source.addPaint(new Point(e.getX(), e.getY()));

        //每次点击一次鼠标都需要重新画一遍
        source.repaint();
    }
}
```

## 2.11 窗口监听

```java
package space.haobin04;

import java.awt.*;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;
import java.awt.event.WindowListener;

public class WindowDemo {
    public static void main(String[] args) {
        new WindowFrame("窗口监听");
    }
}
class WindowFrame extends Frame{
    public WindowFrame(String title){
        super(title);
        setVisible(true);
        setBounds(500,200,500,500);
        //写法一:内部类
        //this.addWindowListener(new MyWindowListener());

        //写法二:匿名内部类
        this.addWindowListener(
                new WindowAdapter() {

                    @Override
                    public void windowClosing(WindowEvent e) {
                        System.out.println("窗口正在关闭");
                    }

                    @Override
                    public void windowActivated(WindowEvent e) {
                        System.out.println("窗口被激活");

                        //激活后更换标题
                        WindowFrame source =(WindowFrame) e.getSource();
                        source.setTitle("窗口被激活了");
                    }
                }
        );
    }

    //内部类
    private class MyWindowListener extends WindowAdapter {
        @Override
        public void windowClosing(WindowEvent e) {
            //setVisible(false);//隐藏窗口
            System.exit(0);
        }
    }
}
```

## 2.12 键盘监听

```java
package space.haobin04;

import java.awt.*;
import java.awt.event.KeyAdapter;
import java.awt.event.KeyEvent;

public class KeyListenerDemo {
    public static void main(String[] args) {
        new KeyFrame();
    }
}

class KeyFrame extends Frame{
    public KeyFrame(){
        setBounds(200,200,500,200);
        setVisible(true);

        this.addKeyListener(new KeyAdapter() {
            @Override
            public void keyPressed(KeyEvent e) {
                /* Virtual key codes. */
                int keyCode = e.getKeyCode();
                
                if(keyCode==KeyEvent.VK_UP){
                    System.out.println("你按下了上键");
                }
                if(keyCode==KeyEvent.VK_DOWN){
                    System.out.println("你按下了下键");
                }
            }
        });
    }
}
```



# 三、Swing

## 3.1 JFrame窗体

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;

public class JFrameDemo {
    //init:初始化窗口
    public void init(){
        /*public class JFrame  extends Frame;*/
        JFrame jFrame = new JFrame("这是一个JFrame窗口.");

        //设置颜色(对容器设置颜色)
        Container contentPane = jFrame.getContentPane();
        contentPane.setBackground(Color.GREEN);

        //添加文本
        JLabel jLabel= new JLabel("JLabel添加文字");
        jFrame.add(jLabel);
        //文本居中
        jLabel.setHorizontalAlignment(SwingConstants.CENTER);

        jFrame.setVisible(true);
        jFrame.setBounds(200,200,500,200);
        /*Swing中默认的关闭操作*/
        jFrame.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new JFrameDemo().init();
    }
}
```

## 3.2 JDialog弹窗

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

//主窗口
public class JDialogDemo extends JFrame {

   public JDialogDemo(){
       this.setVisible(true);
       this.setBounds(200,200,500,200);
       this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);

       //获得容器
       Container container = this.getContentPane();

       //设置绝对定位
       container.setLayout(null);

       //通过点击按钮，弹出弹窗
       JButton jButton = new JButton("点击弹出一个对话框");//创建按钮

       jButton.setBounds(30,30,200,50);//绝对定位

       container.add(jButton);

       //监听器
       jButton.addActionListener(new ActionListener() {
           @Override
           public void actionPerformed(ActionEvent e) {
                new MyDialog();
           }
       });
   }

    public static void main(String[] args) {
        new JDialogDemo();
    }
}

//弹窗窗口
/*public class JDialog extends Dialog;*/
class MyDialog extends JDialog{
    public MyDialog(){
        /*弹窗默认存在关闭事件，可以不需要编写*/
        this.setVisible(true);
        
        this.setBounds(250,250,250,250);
        Container container = this.getContentPane();
        container.setLayout(null);
        
        JLabel jLabel = new JLabel("你的第一个弹窗");
        //由于设置了绝对布局，这里的JLabel必须有setBounds才能显示
        jLabel.setBounds(50,50,100,30);
        container.add(jLabel);
    }
}
```

## 3.3 标签

- #### text_label

```java
JLabel jLabel = new JLabel("你的第一个弹窗");
```

- #### icon_label

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;

//Icon也需要重写的方法
/*public interface Icon
{
    void paintIcon(Component c, Graphics g, int x, int y);
    int getIconWidth();
    int getIconHeight();
}*/

/*IconDemo extends JFrame implements Icon*/
//原因:是一个窗口，并且实现Icon
public class IconDemo extends JFrame implements Icon {
    private int width;
    private int height;

    //无参构造
    public IconDemo(){}
    //带参构造
    public IconDemo(int width, int height){
        this.width = width;
        this.height = height;
    }

    public void init(){
        IconDemo iconDemo = new IconDemo(20, 20);
        JLabel jLabel = new JLabel("标签图标测试", iconDemo, SwingConstants.CENTER);
        //必须先获得当前的这个容器，再把这个标签添加到容器中
        Container container = getContentPane();
        container.add(jLabel);
        this.setTitle("这是一个图标测试");
        this.setVisible(true);
        this.setBounds(200,200,500,200);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new IconDemo().init();
    }

    /*组件、画笔、坐标x、y*/
    @Override
    public void paintIcon(Component c, Graphics g, int x, int y) {
        g.fillOval(x,y,this.width,this.height);
    }

    @Override
    public int getIconWidth() {
        return this.width;
    }

    @Override
    public int getIconHeight() {
        return this.height;
    }
}
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328162442338.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328162442338" style="zoom:33%;" />

- #### imageIcon_label

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;
import java.net.URL;

public class imageIconDemo extends JFrame {

    public imageIconDemo(){
        JLabel jLabel = new JLabel("图片标签",SwingConstants.CENTER);
        URL url = imageIconDemo.class.getResource("dog.jpg");
        /*public ImageIcon (URL location)*/
        ImageIcon imageIcon = new ImageIcon(url);
        /*public void setIcon(Icon icon) */
        jLabel.setIcon(imageIcon);
        Container container = getContentPane();
        container.add(jLabel);
        setTitle("图片标签测试");
        setVisible(true);
        setBounds(200,200,450,500);
        setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new imageIconDemo();
    }
}
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328163803798.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328163803798" style="zoom:33%;" />

## 3.4 面板

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;

public class JPanelDemo extends JFrame {
    public JPanelDemo(){
        //获得当前窗口的容器
        /*public Container getContentPane() {
            return getRootPane().getContentPane();
        }*/
        Container container = getContentPane();
        container.setLayout(new GridLayout(2,1,10,10));
        JPanel jPanel1 = new JPanel(new GridLayout(1, 3));
        JPanel jPanel2 = new JPanel(new GridLayout(3, 2));
        JPanel jPanel3 = new JPanel(new GridLayout(4, 1));
        JPanel jPanel4 = new JPanel(new GridLayout(2, 3));

        jPanel1.add(new JButton("1"));
        jPanel1.add(new JButton("1"));
        jPanel1.add(new JButton("1"));
        jPanel2.add(new JButton("2"));
        jPanel2.add(new JButton("2"));
        jPanel2.add(new JButton("2"));
        jPanel2.add(new JButton("2"));
        jPanel2.add(new JButton("2"));
        jPanel2.add(new JButton("2"));
        jPanel3.add(new JButton("3"));
        jPanel3.add(new JButton("3"));
        jPanel3.add(new JButton("3"));
        jPanel3.add(new JButton("3"));
        jPanel4.add(new JButton("4"));
        jPanel4.add(new JButton("4"));
        jPanel4.add(new JButton("4"));
        jPanel4.add(new JButton("4"));
        jPanel4.add(new JButton("4"));
        jPanel4.add(new JButton("4"));

        container.add(jPanel1);
        container.add(jPanel2);
        container.add(jPanel3);
        container.add(jPanel4);

        this.setTitle("面板测试");
        this.setVisible(true);
        this.setBounds(300,200,500,500);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new JPanelDemo();
    }
}
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328165226865.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328165226865" style="zoom:33%;" />

`滚动条实现`

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;

public class JScrollDemo extends JFrame{
    public JScrollDemo(){
        Container container = this.getContentPane();

        //添加文本域
        /*public TextArea(int rows, int columns)*/
        JTextArea JtextArea = new JTextArea(20, 50);
        JtextArea.setText("这里是文本域测试");

        //具有滚动条的面板
        JScrollPane jScrollPane = new JScrollPane(JtextArea);

        container.add(jScrollPane);

        this.setVisible(true);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
        this.setBounds(300,200,500,300);
    }

    public static void main(String[] args) {
        new JScrollDemo();
    }
}
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328170232054.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328170232054" style="zoom:33%;" />



## 3.5 按钮

- 图片按钮

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;
import java.net.URL;

public class JButtonDemo extends JFrame {

    public JButtonDemo(){
        Container container = this.getContentPane();
        URL url = JButtonDemo.class.getResource("dog.jpg");
        /*public ImageIcon (URL location)*/
        //图片变成图标
        Icon imageIcon = new ImageIcon(url);

        //把图标放在按钮上
        JButton Jbutton = new JButton();
        Jbutton.setIcon(imageIcon);

        //设置按钮悬浮提示文本
        /*Registers the text to display in a tool tip.
         The text displays when the cursor lingers over
          the component.*/
        Jbutton.setToolTipText("这是一个图片按钮");
        container.add(Jbutton);
        this.setTitle("这是一个图片按钮");
        this.setVisible(true);
        this.setBounds(300,200,300,500);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new JButtonDemo();
    }
}
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328171504094.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328171504094" style="zoom:33%;" />

- 单选框 

`注意需要进行分组`

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;
import java.net.URL;

public class JButton_RadioDemo extends JFrame {
    public JButton_RadioDemo(){
        Container container = this.getContentPane();

        //初始化单选框
        JRadioButton jRadioButton1 = new JRadioButton("1");
        JRadioButton jRadioButton2 = new JRadioButton("2");
        JRadioButton jRadioButton3 = new JRadioButton("3");

        //由于单选框是只能够选一个值的，因此需要进行分组,一个组中只能选择一个
        ButtonGroup buttonGroup = new ButtonGroup();
        buttonGroup.add(jRadioButton1);
        buttonGroup.add(jRadioButton2);
        buttonGroup.add(jRadioButton3);

        container.add(jRadioButton1,BorderLayout.NORTH);
        container.add(jRadioButton2,BorderLayout.CENTER);
        container.add(jRadioButton3,BorderLayout.SOUTH);

        this.setTitle("这是一个单选框测试");
        this.setVisible(true);
        this.setBounds(300,200,300,300);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new JButton_RadioDemo();
    }
}
```



<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328173829596.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328173829596" style="zoom:33%;" />

- 复选框

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;

public class JButton_CheckBoxDemo extends JFrame {
    public JButton_CheckBoxDemo(){
        Container container = this.getContentPane();

        JCheckBox jCheckBox1 = new JCheckBox("1");
        JCheckBox jCheckBox2 = new JCheckBox("2");
        JCheckBox jCheckBox3 = new JCheckBox("3");

        container.add(jCheckBox1,BorderLayout.NORTH);
        container.add(jCheckBox2,BorderLayout.CENTER);
        container.add(jCheckBox3,BorderLayout.SOUTH);
        this.setTitle("这是一个多选框测试");
        this.setVisible(true);
        this.setBounds(300,200,400,300);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new JButton_CheckBoxDemo();
    }
}
```



<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328174705486.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328174705486" style="zoom:33%;" />



## 3.6 列表

- 下拉框

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;

public class ComboBoxDemo extends JFrame {

    public ComboBoxDemo(){
        Container container = this.getContentPane();

        JComboBox status = new JComboBox();

        status.addItem("香蕉");
        status.addItem("苹果");
        status.addItem("甘蔗");
        status.addItem("西瓜");
        status.addItem("火龙果");
        
        container.add(status);

        this.setTitle("这是一个下拉框测试");
        this.setVisible(true);
        this.setBounds(300,200,400,300);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new ComboBoxDemo();
    }
}
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328180038180.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328180038180" style="zoom:33%;" />

- 列表框



```java
package space.Swing;

import javax.swing.*;
import java.awt.*;
import java.util.Vector;

public class JListDemo extends JFrame {
    public JListDemo() {
        Container container = this.getContentPane();

        //初始化列表的内容
        /*静态*/
        //String[] contents={"1","2","3"};
        //JList jList = new JList(contents);

        /*动态*/
        Vector contents = new Vector();
        JList jList = new JList(contents);
        contents.add("张三");
        contents.add("李四");
        contents.add("王五");

        container.add(jList);

        this.setTitle("列表框测试");
        this.setVisible(true);
        this.setBounds(300, 200, 400, 300);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new JListDemo();
    }
}
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328181019515.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328181019515" style="zoom:33%;" />



`应用场景`：

- 下拉框：单个选项、减少占用的页面空间；
- 列表框：展示信息，一般使用动态扩容（vector）。



## 3.7 文本框

- 文本框

- 密码框

- 文本域

```java
package space.Swing;

import javax.swing.*;
import java.awt.*;

public class TextDemo extends JFrame {

    public TextDemo(){
        Container container = this.getContentPane();

        //1、文本框
        JTextField jTextField = new JTextField("Hello");

        //2、密码框
        JPasswordField jPasswordField = new JPasswordField();
        /* 默认用实心圆点覆盖，可以修改为* */
        jPasswordField.setEchoChar('*');

        //3、文本域
        JTextArea jTextArea = new JTextArea(20, 10);
        jTextArea.setText("这里是文本域测试");

        container.add(jTextField,BorderLayout.NORTH);
        container.add(jPasswordField,BorderLayout.CENTER);
        container.add(jTextArea,BorderLayout.SOUTH);

        this.setTitle("文本框、密码框、文本域测试");
        this.setVisible(true);
        this.setBounds(300,200,500,400);
        this.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new TextDemo();
    }
}
```



<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230328182755799.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230328182755799" style="zoom:33%;" />

# 四、贪吃蛇游戏编写

> 帧的概念：
>
> ​	如果时间片足够小，就是动画，拆开来的每一帧就是静态的图片。

游戏运行展示

![image-20230329180224331](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230329180224331.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

`三部曲`：

1. 定义数据
2. 画到面板上
3. 添加监听事件:键盘监听和事件监听

```java
package space.haobin;

import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.KeyEvent;
import java.awt.event.KeyListener;
import java.net.URL;
import java.util.Random;

/**
 * 游戏的主启动类
 */
public class StartGame {
    public static void main(String[] args) {
        //1
        JFrame jFrame = new JFrame();
        jFrame.setBounds(200,25,900,720);
        jFrame.setResizable(false);//设置窗口大小不可变
        jFrame.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);

        //2
        jFrame.add(new GamePanel());//将面板添加到窗口上

        jFrame.setVisible(true);
    }
}

class Data {
    //页眉
    public static URL headerURL = Data.class.getResource("static/header.png");
    public static ImageIcon header = new ImageIcon(headerURL);
    //蛇的方向
    public static URL upURL = Data.class.getResource("static/up.png");
    public static URL downURL = Data.class.getResource("static/down.png");
    public static URL leftURL = Data.class.getResource("static/left.png");
    public static URL rightURL = Data.class.getResource("static/right.png");
    public static ImageIcon up = new ImageIcon(upURL);
    public static ImageIcon down = new ImageIcon(downURL);
    public static ImageIcon left = new ImageIcon(leftURL);
    public static ImageIcon right = new ImageIcon(rightURL);
    //蛇的身体
    public static URL bodyURL = Data.class.getResource("static/body.png");
    public static ImageIcon body = new ImageIcon(bodyURL);
    //食物
    public static URL foodURL = Data.class.getResource("static/food.png");
    public static ImageIcon food = new ImageIcon(foodURL);
}

/**
 * 游戏的面板
 */
class GamePanel extends JPanel implements KeyListener, ActionListener {
    //6
    //定义蛇的数据结构
    int length;//蛇的长度
    int[] snake_x = new int[600];//蛇的x坐标
    int[] snake_y = new int[500];//蛇的y坐标

    //16
    //食物的坐标
    int food_x;
    int food_y;
    //食物随机产生坐标
    Random random = new Random();

    //21
    //成绩
    int score;


    String director;//记录蛇头的方向

    //9
    //记录当前游戏的状态
    boolean isStart = false;//默认停止

    //19
    //判断游戏失败
    boolean isFail = false;

    //13
    //事件监听，通过固定的事件进行刷新
    //定时器
    /*public Timer(int delay, ActionListener listener)*/
    Timer timer = new Timer(100,this);//delay越小，速度越快



    //8
    //构造器
    public GamePanel() {
        init();

        //12
        //获得焦点和键盘事件
        this.setFocusable(true);
        this.addKeyListener(this);

        timer.start();
    }

    //7
    //初始化方法，游戏的初始化状态
    public void init() {
        length = 3;
        snake_x[0] = 100;
        snake_y[0] = 100;//蛇头的坐标
        snake_x[1] = 75;
        snake_y[1] = 100;//蛇第一个身体的坐标
        snake_x[2] = 50;
        snake_y[2] = 100;//蛇第二个身体的坐标
        director = "R";//默认向右

        //17
        //初始化食物的数据,将食物随机分布在界面上
        food_x=25+25*random.nextInt(34);
        food_y=75+25*random.nextInt(24);

        //22
        score=0;
    }


    //绘制面板，游戏的所有东西都使用这个画笔来画
    @Override
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);//清屏
        this.setBackground(Color.WHITE);//4
        //绘制静态的面板
        //5
        Data.header.paintIcon(this, g, 25, 11);//放置页眉
        g.fillRect(25, 75, 850, 600);//默认游戏界面,默认黑色

        //18
        //绘制食物
        Data.food.paintIcon(this,g,food_x,food_y);

        //8
        //将小蛇画上去，蛇身体使用for循环添加，方向使用if判断
        if (director.equals("R")) {
            Data.right.paintIcon(this, g, snake_x[0], snake_y[0]);//蛇头初始化向右
        }
        if (director.equals("L")) {
            Data.left.paintIcon(this, g, snake_x[0], snake_y[0]);
        }
        if (director.equals("U")) {
            Data.up.paintIcon(this, g, snake_x[0], snake_y[0]);

        }
        if (director.equals("D")) {
            Data.down.paintIcon(this, g, snake_x[0], snake_y[0]);

        }
        for (int i = 1; i < length; i++) {
            Data.body.paintIcon(this, g, snake_x[i], snake_y[i]);
        }

        //10
        //判断游戏状态
        if (isStart == false) {
            g.setColor(Color.WHITE);//设置字体颜色
            g.setFont(new Font("微软雅黑", Font.BOLD, 40));
            g.drawString("按下空格开始游戏", 300, 300);
        }

        if(isFail==true){
            g.setColor(Color.RED);//设置字体颜色
            g.setFont(new Font("微软雅黑", Font.BOLD, 40));
            g.drawString("失败，按下空格重新开始", 300, 300);
        }

        //24
        //绘制积分显示
        g.setColor(Color.WHITE);
        g.setFont(new Font("微软雅黑", Font.BOLD, 18));
        g.drawString("长度"+length,750,35);
        g.drawString("分数"+score,750,50);
    }

    //14
    @Override
    public void actionPerformed(ActionEvent e) {
        if(isStart&&isFail==false){
            //游戏开始，小蛇开始动

            //19
            //检测小蛇吃食物
            if(snake_x[0]==food_x&&snake_y[0]==food_y){
                length++;
                score+=10;
                //重新生成食物
                food_x=25+25*random.nextInt(34);
                food_y=75+25*random.nextInt(24);
            }

            //实现右移
            //控制身体移动
            for(int i =length-1;i>0;i--){
                snake_x[i]=snake_x[i-1];
                snake_y[i]=snake_y[i-1];
            }

            //15
            //控制蛇头移动
            if(director.equals("U")){
                snake_y[0]-=25;
                //边界判断
                if(snake_y[0]<75){
                    snake_y[0]=650;
                }
            }
            if(director.equals("D")){
                snake_y[0]+=25;
                //边界判断
                if(snake_y[0]>650){
                    snake_y[0]=75;
                }
            }
            if(director.equals("L")){
                snake_x[0]-=25;
                //边界判断
                if(snake_x[0]<25){
                    snake_x[0]=850;
                }
            }
            if(director.equals("R")){
                snake_x[0]+=25;
                //边界判断
                if(snake_x[0]>850){
                    snake_x[0]=25;
                }
            }

            //20
            //失败判定，撞到自己
            for(int i=1;i<length;i++){
                if(snake_x[0]==snake_x[i]&&snake_y[0]==snake_y[i]){
                    isFail=true;
                }
            }

            repaint();
        }
        timer.start();
    }

    //11
    //实现键盘监听
    @Override
    public void keyPressed(KeyEvent e) {
        //监听键盘的按压事件
        //获得当前键盘按下的是哪一个
        int keyCode = e.getKeyCode();
        //空格键，游戏开始或者停止
        if (keyCode == KeyEvent.VK_SPACE) {
            if(isFail){
                //重新开始
                isFail=false;
                init();
            }
            if(!isFail){
                isStart = !isStart;
            }
            repaint();
        }


        //16
        //实现小蛇上下左右移动
        if(keyCode==KeyEvent.VK_UP){
            director="U";
        }
        if(keyCode==KeyEvent.VK_DOWN){
            director="D";
        }
        if(keyCode==KeyEvent.VK_LEFT){
            director="L";
        }
        if(keyCode==KeyEvent.VK_RIGHT){
            director="R";
        }

    }
    @Override
    public void keyTyped(KeyEvent e) {

    }
    @Override
    public void keyReleased(KeyEvent e) {

    }
}
```

## 游戏程序需要导的包

```java
import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.KeyEvent;
import java.awt.event.KeyListener;
import java.net.URL;
import java.util.Random;
```

## 编写思路

### 1、主函数编写

```java
public class SnakeGame {
    public static void main(String[] args) {
        JFrame jFrame = new JFrame();
        jFrame.add(new GamePanel());//添加自己的面板置窗口
        jFrame.setTitle("贪吃蛇小游戏");
        jFrame.setResizable(false);
        /*900:36个25*/
        jFrame.setBounds(200,25,900,720);
        jFrame.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);
        jFrame.setVisible(true);
    }
}
```

此时自己的面板是这样的

```java
class GamePanel extends JPanel{
    public  GamePanel(){

    }
}
```

### 2、数据类编写

==调用绘制小蛇及食物的图片资源==

```java
/**
 * 数据类
 */
class Data{
    //页眉图片
    public static URL headerURL = Data.class.getResource("static/header.png");
    public static ImageIcon header = new ImageIcon(headerURL);
    //小蛇
    public static URL upURL = Data.class.getResource("static/up.png");
    public static ImageIcon up = new ImageIcon(upURL);
    
    public static URL downURL = Data.class.getResource("static/down.png");
    public static ImageIcon down = new ImageIcon(downURL);
    
    public static URL leftURL = Data.class.getResource("static/left.png");
    public static ImageIcon left = new ImageIcon(leftURL);
    
    public static URL rightURL = Data.class.getResource("static/right.png");
    public static ImageIcon right = new ImageIcon(rightURL);
    
    public static URL bodyURL = Data.class.getResource("static/body.png");
    public static ImageIcon body = new ImageIcon(bodyURL);
    //食物
    public static URL foodURL = Data.class.getResource("static/food.png");
    public static ImageIcon food = new ImageIcon(foodURL);
}
```



---

> <strong> 🚀<font color = orange>先看后赞，养成习惯！</font>🚀</strong>
>
> <strong> 🚀<font color = red> 先看后赞，养成习惯！</font>🚀</strong>

> **🎈觉得文章写得不错的老铁们，点赞评论关注走一波！谢谢啦！🎈**

---



