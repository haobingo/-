[TOC]



# 1️⃣ 一、前端简介

## 🚋 1、三要素

- **HTML**

​		结构层，超文本标记语言，决定网页的结构和内容。

- **CSS**

​		表现层，层叠样式表，设定网页的表现样式。

- **JavaScript**

​		行为层，一种弱类型的脚本语言，其源码不需要经过编译，而是由浏览器解释运行，用于控制网页的行为，严格区分大小写，但是并不适合处理高并发的工作。

## 🎈  2、CSS预处理器

CSS预处理器定义了一种新的语言，其基本思想是，用一种专门的编程语言，为CSS增加一些编程特性，将CSS作为目标生成文件，然后开发者就只要使用这种语言进行编码工作。通俗地说，==CSS预处理器用一种专门的编程语言，进行Web页面样式设计，然后再编译成正常的CSS文件，以供项目使用==。CSS预处理器为CSS增加了一些编程的特性，无需考虑浏览器的兼容性问题，例如，你可以在CSS中使用变量、简单地逻辑程序和函数等等在编程语言中的一些基本特性，可以让你的CSS更加简洁、适应性更强、可读性更佳、更易于代码的维护等诸多好处。



# 2️⃣ 二、简单使用

## 🚋 1、引入JavaScript

```javascript
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script>
        //这里可以写JS代码
    </script>

       <!--也可以外部引入-->
    <script src="./js.js"></script>
</head>
<body>

    <script>
        //这里也可以写
    </script>
</body>
</html>
```

## 🎈  2、弹窗——alert（）

```javascript
<script>
    alert("Hello World!");
</script>
```

## 🌈 3、调试——console.log()

> 类似 Java 中的打印,console.log() 就是在浏览器的控制台打印



```javascript
<script>
    console.log("Hello World!");
</script>
```



# 3️⃣ 三、数据类型总括

==JavaScript是一种弱类型的编程语言==

## 🚋 1、分类

|       类型        |                          举例/说明                           |                 特点                 |
| :---------------: | :----------------------------------------------------------: | :----------------------------------: |
|      number       |                    12、12.34、-12、1.12e3                    |          JS不区分小数和整数          |
|        NaN        |           不是一个数，与所有的数值包括自己都不相等           |      使用 isNaN() 方法进行判断       |
|     Infinity      |             表示无限大的数，超出计算机的计算范围             |                                      |
|      字符串       |                       ’abc‘  、 “abc”                        |    JS中使用单双引号并没有太大区别    |
| 布尔值（boolean） |                        true 、 false                         |                                      |
|    逻辑运算符     |                与、或、 非 、短路与、 短路或                 |                                      |
|    比较运算符     | = 、 == （类型可以不一样，值一样） 、 ===（绝对等于，类型和值都必须一样） |                                      |
|     undefined     |                            未定义                            |  取数组下标越界后就会出现 undefined  |
|       数组        |          var  arr  = [123,'abc',true,null,[1,2,3]];          |             用中括号定义             |
|       对象        | var person = { "name" : "haobing", "age" : 18, "job" : "student", "home" : "jiangxi"}; | 用大括号定义，不同属性之间用逗号隔开 |



## 🎈  2、严格检查模式

> 在 JS 代码的第一行加上  ==' use strict ';==    可以防止JavaScript的随意性导致产生的一些问题

建议：`局部有变量都使用 let 定义`



# 4️⃣ 四、数据类型详解

> JavaScript中所有的键都是字符串，值是任意对象。

## 🚋 1、字符串

==JS 字符串不可变==

```javascript
<body>
    <script>
        //转义字符   使用 \ + ...(包括Unicode字符、Ascall字符)
        console.log('hello\nworld');

        //多行字符
        var msg =  
        `hello
        world
        我是
        JavaScript`;

        //模板字符串  使用  `${变量名}`
        let name = "张三";
        let age = 18;
        let msg2 = `你好，我叫${name},今年${age}岁了！`;
        console.log(msg2);

        //常用方法
        var msg3 = "abcABC";
        msg3[3];//获取指定下标的字符值，通过下标取值
        msg3.toUpperCase();//转大写
        msg3.toLowerCase();//转小写
        msg3.length;//获取字符串的长度
        msg3.indexOf('C');//获取指定字符的下标
        msg3.substring(1,4);//截取字符串，取左不取右
    </script>
</body>
```



## 🎈  2、数组

==JS 中的数组可以包含任意的数据类型，数组的长度和内容均可以改变==

```javascript
<body>
    <script>
        //数组中可以包含任意数据类型
        var arr = [1,2,3,null,true,[1,2,3]];

        arr.indexOf(true);//获取指定元素的下标，字符串 "1" 和 数字 1 是不同的
        arr.slice(1,4);//截取数组的一部分，返回一个新的数组，类似 substring()，取左不取右

        //追加元素  ————返回操作后，数组的长度
        arr.unshift('a');//头部追加   
        arr.push('b');//尾部追加

        //弹出元素  ————返回操作后，弹出的元素
        arr.shift();//头部弹出
        arr.pop();//尾部弹出

        //排序
        arr.sort();

        //元素翻转
        arr.reverse();

        //拼接数组  ————返回拼接好后的新数组，原来的数组不会被修改
        arr.concat([1,2,3]);

        //连接符
        arr.join("-");//打印拼接数组，使用特定的字符串拼接

        //填充数组
        arr.fill(1);
    </script>
</body>
```



## 🌈 3、对象

==核心：若干个键值对==

> JavaScript中所有的键都是字符串，值是任意对象

```javascript
<body>
    <script>
        //使用关键字 new 对象，使用大括号声明
        var person = {
            "name" : "张三",//属性之间使用逗号隔开
            "age" : 18,
            "email" : "12345678@qq.com",
            "score" : 100
        }

        //判断某个属性是否是这个对象自身所拥有的
        person.hasOwnProperty("name");

        //可以直接更改对象的属性，并且使用一个不存在的对象属性，浏览器只是报 undefined 
        person.name = "李四";

        //动态删减属性
        delete person.score;

        //动态添加属性，直接赋值
        person.habit = "sleep";

        //判断某个属性是否在这个对象中，包括继承过来的属性    xxx  in  xxx
        "toString" in person;
        "name" in person;

        //JavaScript中所有的键都是字符串，值是任意对象
        person['age'];
    </script>
</body>
```



# 5️⃣ 五、分支与循环

```javascript
<body>
    <script>

        let a = 5;

        //if 判断
        if(a>5){
            alert('大于5');
        }else if(a<5){
            alert('小于5');
        }else{
            alert('等于5');
        }

        //while 循环
        while(a<=10){
            alert(a);
            a++;
        }

        //do while 循环
        do{
            alert(a);
            a++;
        }while(a<=10);

        //for 循环
        for(let i = 0 ; i <100 ; i++){
            console.log(i);
        }

        //数组循环            
        
        /*
            Java中的增强 for：  
                for(Type str : el){}
        */
        var arr = [1,2,3,4,5];

        for(let b in arr){   //------->  let index  in  arr  使用 in 取的是下标
            console.log(arr[b]);
        }

        for(let c of arr){   //------->  let value  of  arr  使用 of 取的是值
            console.log(c);
        }

        //forEach循环
        arr.forEach(function(e){  //同样可以遍历数组中的所有值
            console.log(e);
        });
    </script>
</body>
```



# 6️⃣ 六、Map 和 Set 集合

> 可以将学生的名字和成绩映射起来

## 🚋 1、Map

==类似Python中的字典==

```javascript
<body>
    <script>

        //Map 的声明
        var map = new Map([['Tom',100],['Jack',80],['Rose',60]]);

        //取值
        map.get('Tom');

        //设置值   参数:  (Key , Value)
        map.set('Kitty',85);
        map.set('Tom',99);  //修改值

        //删除值
        map.delete('Tom');
 
    </script>
</body>
```

## 🎈  2、Set

==指无序不重复的集合==

```javascript
<body>
    <script>

        //Set 的声明   Set可以去重
        var set = new Set([1,2,2,2,3]);

        //添加不重复的值
        set.add(5);

        //删除值
        set.delete(1);

        //判断是否包含某个元素
        set.has(5);

    </script>
</body>
```



## 🌈 3、Iterable迭代

- 遍历数组

```javascript
var arr = [1,2,3,4,5]
for(let x of arr){
    console.log(x);
}
```

-  遍历Map

```javascript
var map = new Map([['Tom',100],['Jack',80],['Rose',60]]);       
for(let x of map){
    console.log(x);
}
```

- 遍历Set

```javascript
var set = new Set([1,2,2,2,3]);
for(let x of set){
    console.log(x);
}
```

==bug==

在新增值时，用 for...in ...  去下标时，会存在错误，而使用 for... of ....  会修正。



# 7️⃣七、函数

> 将函数放在对象类中就变成了方法

## 🌈1、定义

```javascript
//定义方式一
function 函数名(参数){
    //函数体
}

//定义方式二  ----匿名函数
var 函数名 = function(参数){
    //函数体
}
```

==bug   参数问题： JavaScript可以传递任意个参数，也可以不传递参数==

> 如何解决不存在参数的问题？--------------------手动抛出异常

```javascript
<body>
    <script>
        var fun = function(x){
            if(typeof(x) !== 'number'){//typeof()可以获取变量（参数）的类型
                throw 'Not a Number';
            }

            alert(x);
        }
    </script>
</body>
```

> 如何解决参数存在多个的问题？（浏览器默认只取第一个）---------arguments

```javascript
<body>
    <script>
        var fun = function(x){

            //arguments 代表传递进来的所有参数，实际上是一个数组
            for(let i = 0 ; i <arguments.length;i++ ){
                console.log(arguments[i]);
            } 
            alert(x);  //实际上用到的只有第一个参数
        }

    </script>
</body>
```

存在问题：数组arguments中还包括当前参数

> 如何排除已经存在过的参数？------------------rest   类似Java中的可变长参数

```javascript
<body>
    <script>
        //传统方法
        var fun1 = function(a,b){
            console.log(a);
            console.log(b);
            if(arguments.length>2){
                for(let i = 2 ;i <=arguments.length;i++){
                    console.log(i);
                }
            }
        }

        //使用 rest 改进
        var fun2 = function(a,b,...rest){
            console.log(a);
            console.log(b);
            console.log(rest);
        }
    </script>
</body>

       
```

## 🎈2、变量的作用域

- 在JavaScript中，`var`定义变量实际上是有作用域的，在函数体中声明的，在函数体外不能使用。

```javascript
<body>
    <script>
        function add(){
            var x = 1;
            x++;
        }
        x += 2;//报  Uncaught ReferenceError: x is not defined
    </script>
</body>
```

-  内部函数`可以访问`外部函数的变量，外部函数`不能访问`内部函数的变量。

```javascript
<body>
    <script>
        function add(){//-------------外部函数
            var x = 1;
            x++;
            function add2(){//----------内部函数
                var y = 2;
                console.log(x);//正常运行
            }
            console.log(y);//报  Uncaught ReferenceError: y is not defined
        }
    </script>
</body>
```

-  假设内外函数变量重名，JavaScript会`从内向外查找`，函数查找变量从自身函数开始，内部函数会屏蔽外部函数变量

```javascript
<body>
    <script>
        function add(){//-------------外部函数

            var x = 1;

            function add2(){//----------内部函数

                var x = 2;

                console.log('内部：'+x);
            }
            console.log('外部：'+x);
            add2();
        }
        add();
    </script>
</body>
```

- JavaScript执行引擎，会自动提升 y 的声明，但是不会提升变量 y 的赋值

```javascript
<body>
    <script>
        var x = 'x ' +y;
        console.log(x);//打印 x undefined，说明 y 已经声明，但是没有被赋值
        var y = 'y';

        /*
            等价于 下面
        */

        var y; //执行引擎自动提升了 y 的声明
        var x = 'x '+y;
        console.log(x);
        y = 'y'; //但是不会提升 y 的赋值

    </script>
</body>
```

-  ==养成规范==：所有的变量定义都放在函数的头部，不要乱放，便于代码维护。
-  默认所有的全局变量都会自动绑定在window 对象下

​			JavaScript实际上只有一个全局作用域，任何变量（函数也可以视为变量），假设没有在函数作用范围内找到，就会向外查找，直到在全局作用域没有找到（即 window下），报错 `ReferenceError`。

- ==Bug==：由于我们所有的全局变量都会绑定在我们的 window 上，如果不同的 js 文件使用了相同的全局变量就会发生冲突-------------------如何减少冲突？

`将自己的全局变量全部放入自己定义的唯一空间中，降低全局命名冲突的问题，例如：jQuery使用----$(选择器).action();`

```javascript
<body>
    <script>

        var Haobing ={};//唯一的全局变量 放在这

        Haobing.name ='Haobing';       //添加自己的全局变量
        Haobing.add = function(a,b){   //添加自己的全局函数
            return a+b;
        }

    </script>
</body>
```

- 局部变量`let`，一般用于 for 循环中
- 常量`const`，定义一些不能够被修改的变量，通常使用全大写字母声明，为只读变量

## 🧲3、方法

> 函数定义在对象中就称为方法

- 方法的使用

```JavaScript
<body>
    <script>

        var person = {
            name : 'Haobing', //-------属性
            birth : 2000,  //---------属性
            age : function(){  //-------方法
                var now = new Date().getFullYear();
                return now - this.birth;  //this是无法指向的，默认指向调用它的那个对象
            }
        }

        person.age();//-----调用时需要看成是函数的调用，加上括号

    </script>
</body>
```

- ==Bug==：如何解决 this 关键字 无法指向的问题 (即如果将方法函数剥离出去，直接调用剥离后的函数会报错)

```javascript
<body>
    <script>

        function getAge(){
            var now = new Date().getFullYear();
            return now - this.birth;//this 是无法指向的，是默认指向调用它的那个对象的
        }

        var person = {
            name : 'Haobing', //-------属性
            birth : 2000,  //---------属性
            age : getAge   //--------这里不需要加括号
        }

        person.age();//-----调用时需要看成是函数的调用，加上括号，正常运行

        getAge();  //报 NaN ，由于window下没有 this 指的 birth
        
    </script>
</body>
```

`如何解决？`-----------------使用 apply 方法

```javascript
<body>
    <script>

        function getAge(){
            var now = new Date().getFullYear();
            return now - this.birth;//this 是无法指向的，是默认指向调用它的那个对象的
        }

        var person = {
            name : 'Haobing', //-------属性
            birth : 2000,  //---------属性
            age : getAge   //--------这里不需要加括号
        }
        
		//***************解决方案*************************
        getAge.apply(person,[]);//表示 this 指向 person 这个对象，参数为空
        
    </script>
</body>
```



# 8️⃣八、Date日期对象

|                          调用方法                           |     说明     |
| :---------------------------------------------------------: | :----------: |
| var now = new Date();//参数可以传入时间戳，将时间戳转为时间 | 中国标准时间 |
|                     now.getFullYear();                      |     整年     |
|                       now.getMonth();                       | 当前月份 - 1 |
|                       now.getDate();                        |     日期     |
|                        now.getDay();                        |    星期几    |
|                       now.getHours();                       |      时      |
|                      now.getMinutes();                      |      分      |
|                      now.getSeconds();                      |      秒      |
|                       now.getTime();                        |    时间戳    |
|                    now.toLocaleString();                    | 获取当地时间 |



# 9️⃣九、JSON对象

> 轻量级的数据交换格式  

`在JavaScript中一切皆为对象，任何JS支持的类型都可以用JSON来表示`

格式：对象都用 {  }    大括号

​			数组都用 [  ]    中括号

​			所有键值对用   ‘ key'  :  'value ’  ----------均当做字符串，使用双引号

```javascript
<body>
    <script>

        //对象
        var person = {
            name : 'Haobing',
            age : 18,
            job : 'student',
            tags : ['Java','C++','Web']//-----数组
        }

        //将对象转为 JSON 字符串
        var json_person = JSON.stringify(person);

        //将 JSON 字符串转为对象
        var obj_person = JSON.parse(json_person);
    </script>
</body>
```



# 1️⃣0️⃣ 十、面向对象

## 🌈1、面向原型继承（旧）

> 类是对象的抽象，对象是类的具体实例。

```javascript
<body>
    <script>

        var person = {
            name : 'Haobing',
            age : 18,
            job : 'student',
            run : function(){
                console.log(this.name+' run...');
            }
        }

        var Haobing = {
            name : 'Haobing'
        }

        //Haobing.run(); //TypeError: Haobing.run is not a function

        //原型指向
        Haobing.__proto__ = person;  //表示  Haobing 继承了 person   ---------- Haobing 的原型是 person
        Haobing.run();  //正常运行，打印 Haobing run...
    </script>
</body>
```



## 🎈2、面向class继承（新）

> 在JavaScript中，每个函数都有一个prototype属性，这个属性指向函数的原型对象

```javascript
<body>
    <script>
        function Student(name){
            this.name = name;
        }

        //给Student新增一个方法-------找原型添加（不推荐使用）
        /*
            prototype这个属性指向函数的原型对象
        */
        Student.prototype.hello = function(){
            alert('Hello!');
        }

        //****************************************************
        //****************************************************

        // 定义一个学生的类 ----------(推荐使用)
        class Student2{
            constructor(name){ //--------构造器
                this.name = name;
            }
            hello(){  //----------添加方法
                alert('Hello!');
            }
        }

        var Haobing = new Student2('Haobing');//new 实例对象

        class xiaoStudent2 extends Student2{ //继承，等价于 原型指向父类 __proto__
            hello(){
                alert(this.name+' Hello!');//重写方法
            }
        }
        var Jack = new xiaoStudent2('Jack');

    </script>
</body>
```



# 1️⃣1️⃣十一、操作BOM对象

> BOM：浏览器对象模型

|   对象    |                             作用                             |
| :-------: | :----------------------------------------------------------: |
|  window   | 全局对象，接受所有窗口的属性，eg：alert（）、innerHeight、outerWidth |
| navigator | （不建议使用）封装了浏览器的信息，eg：appName、appVersion、platform |
|  screen   |           电脑屏幕属性（尺寸），eg：width、height            |
| location  | ==重要==，代表当前页面的URL信息，eg：reload（）刷新网页、assign（'绝对网址'）设置新地址、protocol |
| document  | 当前页面内容，eg：title 当前网页网址、getElementById()获取具体的文档树节点、cookie 获取客户端的一些本地信息 |
|  history  |    （不建议使用）历史网页，back（）后退、forward（）前进     |



# 1️⃣2️⃣十二、操作DOM对象

> DOM ：文档对象模型，浏览器网页就是一个DOM树形节点

## 🎈1、获得DOM节点

- `遍历`（获得）

```javascript
<body>

    <div id="father">
        <h1>标签选择器</h1>
        <p id="p1">id选择器</p>
        <p class="p2">class选择器</p>
    </div>

    <script>

        var h1 = document.getElementsByTagName('h1');//标签选择器

        var p1 = document.getElementById('p1');//id选择器

        var p2 = document.getElementsByClassName('p2');//class选择器

        var father = document.getElementById('father');

        var children = document.children;//获取父节点下的所有子节点

        father.firstChild;//获取第一个子节点
        father.lastChild;//获取最后一个子节点

        p1.previousSibling;//上一个节点
        p1.nextSibling;//下一个节点
        
    </script>
</body>
```

-  `更新`

```javascript
<body>
    <div id="father">
        12345
    </div>

    <script>
        var father = document.getElementById('father');

        father.innerText = 'abcde';//修改内容

        father.innerHTML = '<h2>abcde</h2>';//修改超文本

        father.style.color = 'red';//修改样式（颜色）

        father.style.fontSize = '2em';//修改样式（字体）

        father.style.padding = '1.5em';//修改样式（内边距）
    </script>
</body>
```

- ` 删除`

​		==步骤==：先获取父节点，再通过父节点删除自己

```javascript
<body>
    <div id="father">
        <p id="p1">123</p>
        <p id="p2">abc</p>
        <p id="p3">ABC</p>
    </div>

    <script>
        var p1 = document.getElementById('p1');//确定要删除的子节点

        var father = p1.parentElement;//找到该子节点的父节点

        father.removeChild(p1);//删除指定节点

    </script>
</body>
```

​	==Bug==：删除多个节点的时候，children 是在时刻变化的，删除节点的时候，尽量不使用下标去删除

```javascript
<body>
    <div id="father">
        <p id="p1">123</p>
        <p id="p2">abc</p>
        <p id="p3">ABC</p>
    </div>

    <script>
        var father = document.getElementById('father');

        father.removeChild(father.children[0]);
        father.removeChild(father.children[1]);//-----------并不能完全删除
        father.removeChild(father.children[2]);
    </script>
</body>
```



- `添加`（添加或插入新节点）

使用 innerHTML直接插入，缺点：会覆盖不为空的DOM节点

==解决方案==

- 追加已经存在的节点
-  创建新节点
- 创建标签节点
- 创建style标签

```javascript
<body>
    <p id="p">0000</p>
    <div id="list">
        <p id="p1">1234</p>
        <p id="p2">abcd</p>
        <p id="p3">ABCD</p>
    </div>

    <script>

        // 追加
        var p = document.getElementById('p');
        var list = document.getElementById('list');
        var p1 = document.getElementById('p1');
        var p2 = document.getElementById('p2');
        var p3 = document.getElementById('p3');
        list.appendChild(p);//追加到list尾部

        // 创建  -----   普通标签
        var newP = document.createElement('p');
        newP.id ='newP';  //等价于  newP.setAttribute('id','newP');
        newP.innerText = 'Hello,newP!'; //等价于 newP.setAttribute('innerText','Hello,newP!');
        list.appendChild(newP);

        // 创建  ------  特殊标签
        var myScript = document.createElement('script');
        myScript.setAttribute('type','text/javascript');  //设置 键 与 值
        list.appendChild(myScript);

        //创建  -------style标签
        var myStyle = document.createElement('style');
        myStyle.setAttribute('type','text/css');
        myStyle.innerHTML = 'body{ background-color : green}';
        document.getElementsByTagName('head')[0].appendChild(myStyle);

        //插入节点
        list.insertBefore(p3,p2);//insertBefor(newNode,targetNode);  新节点插到目标节点之前

        //获取指定节点
        list.children[2];
    </script>
</body>
```

# 1️⃣3️⃣十三、表单

## 🧲1、表单的基本使用

> 表单的基本格式：  

```javascript
<form method="post" action="result.html">
<!-- 表单内容 -->
</form>
```

- `method` 规定如何发送表单数据，常用值：get/post，提交方式；
  - get方式提交，我们可以在URL中看到我们提交的信息，不安全，但是高效；
  - post方式提交，则不会，可以传输大文件，但是后台依然可以看到，需要进行加密。

- `action` 表示向何处发送表单数据，即表单提交的位置，可以是网站，也可以是请求处理地址。

==使用==：简单的表单提交

```javascript
<body>
    <h2>注册</h2>
    <form method="post" action="test2.html">
        <!-- 文本输入框 ：input type="text" -->
        <p>名字：<input type="text" name="username"></p>

        <!-- 密码框：input type="password" 框中内容可以隐藏-->
        <p>密码：<input type="password" name="pwd"></p>

        <p>
            <!-- 提交 -->
            <input type="submit" name="Submit" value="提交">
            <!-- 重置 -->
            <input type="reset" name="Reset" value="重填">
        </p>
    </form>
</body>
```

## 🌈2、表单元素格式

|   属性    |                             说明                             |
| :-------: | :----------------------------------------------------------: |
|   type    | 指定元素的类型，有 text、password、checkbox、radio、submit（提交按钮）、reset(清空表单)、file、hidden、image、button，默认是 text。 |
|   name    | ==必须使用==，指定表单元素的名称，type为radio时，`name值必须都相等`，即分组 |
|   value   |     元素的初始值，type为radio（单选框）时必须指定一个值      |
| maxlength |         type为text或password时，限定输入的最大字符数         |
|  checked  |        type为radio或checkbox时，指定按钮是否是被选中         |
|   size    |            指定表单元素的初始宽度，即文本框的长度            |

```javascript
<body>
    <h2>注册</h2>
    <form method="get" action="test2.html">
        <!-- 文本输入框 ：input type="text" -->
        <p>名字：<input type="text" name="username" value="hello" maxlength="10"></p>

        <!-- 密码框：input type="password" 框中内容可以隐藏-->
        <p>密码：<input type="password" name="pwd" size="10em"></p>

        <p>
            <span>性别：</span>
            <!-- 单选框：input type="radio" -->
            <input type="radio" name="sex" value="boy" checked>男
            <input type="radio" name="sex" value="girl">女
        </p>

        <p>
            <span>爱好：</span>
            <!-- 多选框：input type="checkbox" -->
            <input type="checkbox" name="love" value="eat">吃
            <input type="checkbox" name="love" value="sleep" checked>睡
            <input type="checkbox" name="love" value="play">玩
        </p>

         <p>
            <span>按钮：</span>
            <!-- 按钮：input type="button" -->
            <input type="button" name="btn1" value="点击变长">
            <!-- 图片按钮：input type="image" 点击同样可以提交-->
            <input type="image" src="1.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10">
         </p>   

         <!-- 下拉框、列表框 -->
         <p>
            <span>国籍：</span>
            <select name="nation">
                <option value="中国">中国</option>
                <option value="美国" selected>美国</option>
                <option value="日本">日本</option>
                <option value="韩国">韩国</option>
                <option value="朝鲜">朝鲜</option>
            </select>
         </p>

         <!-- 文本域 -->
         <p>
            <span>简介：</span>
            <textarea name="textarea" cols="30" rows="5"></textarea>
         </p>

         <!-- 文件域 -->
         <p>
            <span>文件：</span>
            <input type="file" name="files">
            <input type="button" value="上传" name="upload">
         </p>

         <!-- 邮件验证 -->
         <p>
            <span>邮箱：</span>
            <input type="email" name="email">
         </p>

         <!-- URL验证 -->
         <p>
            <span>URL:</span>
            <input type="url" name="url">
         </p>

         <!-- 数字验证 -->
         <p>
            <span>商品数量:</span>
            <input type="number" name="number" max="999999999999" min="0" step="10">
         </p>

         <!-- 滑块 -->
         <p>
            <span>音量：</span>
            <input type="range" min="0" max="100" name="voice" step="20">
         </p>

         <!-- 搜索框 -->
         <p>
            <span>搜索：</span>
            <input type="search" name="search">
         </p>

        <p>
            <!-- 提交  提交后的信息：/test/test2.html?username=hello654&pwd=432&sex=girl&Submit=提交 -->
            <input type="submit" name="Submit" value="提交">
            <!-- 重置 -->
            <input type="reset" name="Reset" value="重填">
        </p>
    </form>
</body>
```

## 🚦3、表单的应用

- 只读       readonly
- 禁用       disabled
- 隐藏       hidden（但是值还在）
- 默认值    value
- 提高用户体验，增强鼠标可用性

```javascript
<p>
    <label for="mark">点我试试</label>
	<input type="text" id="mark">
</p>
```

## 🛹4、获得和设置表单提交的信息

> 通过JavaScript实现

```javascript
<body>

    <form action="post">
        <p>
            <span>用户名：</span><input type="text" id="username">
        </p>
        
        <!-- 单选框的值，就是定义好的value -->
        <p>
            <span>性别：</span>
            <input type="radio" name="sex" value="man" checked id="boy">男
            <input type="radio" name="sex" value="women" id="girl">女
        </p>

    </form>

    <script>
        //1、获取指定的按钮节点
        var input_text = document.getElementById('username');

        //2、获取值
        input_text.value;//得到输入框所输入的值

        //3、修改值
        input_text.value = 'Hello!';

        // 对于单双选框等固定的值，用boy_raido.value只能获取当前的值
        var boy_raido = document.getElementById('boy');
        var girl_radio = document.getElementById('girl');
        //解决
        boy_raido.checked;//判断是否选中

    </script>
</body>
```

## ⛽5、表单初级验证

==作用==：

- 数据安全性
- 减轻服务器的压力

==使用==：

- placeholder  提示信息
- required    必填属性
- pattern  正则表达式判断

```javascript
<body>
    <h2>注册</h2>
    <form method="get" action="test2.html">

        <!-- 使用 placeholder 作为提示信息-->
        <p>
            <span>用户名：</span>
            <input type="text" name="username" placeholder="请输入用户名">
        </p>

        <!-- 使用 required 表示元素内容不能为空 -->
        <p>
            <span>密码：</span>
            <input type="password" name="psd" required>
        </p>

        <!-- 使用pattern，通过正则表达式判断 -->
        <p>
            <span>自定义邮箱：</span>
            <input type="text" name="idy_name" pattern="^[A-Za-z0-9]+$">
        </p>

        <p>
            <input type="submit" value="提交">
        </p>

    </form>
</body>
```



## 📌6、表单提交验证以及MD5加密

> 通过自定义脚本，获取表单内容，并对表单内容进行检查

`MD5工具类`：   

```javascript
 <script src="https://cdn.bootcss.com/blueimp-md5/2.10.0/js/md5.min.js"></script>
```

- 方法一：MD5加密

```javascript
<body>
    <form method="post">
        <h2>注册</h2>
        <p>
            <span>用户名：</span><input type="text" name="username" id="username">
        </p>
        <p>
            <span>密码：</span><input type="password" name="pwd" id="password">
        </p>
        <p>
            <!-- <input type="submit"> -->
            <!-- 绑定事件 onclick 被点击 -->
            <button type="submit" onclick="check()">提交</button>
        </p>
    </form>

    <script src="https://cdn.bootcss.com/blueimp-md5/2.10.0/js/md5.min.js"></script>

    <script>
        function check(){
            var username = document.getElementById('username');
            var pwd = document.getElementById('password');
            console.log(username.value);
            //使用 MD5 算法进行加密
            pwd.value = md5(pwd.value);
            // 结果：
            // username: 3452253
            // pwd: 747eae4eb05a78eaf03094cd9c179412
            //但是用户体验不佳，容易被发现


            console.log(pwd.value); //这里可以直接调出密码
            // pwd.value = '***'; //也是明文的
        }
    </script>
</body>
```

- 方案二：隐藏真实密码

```javascript
<body>
    <form method="post">
        <h2>注册</h2>
        <p>
            <span>用户名：</span><input type="text" name="username" id="username">
        </p>
        <p>
            <span>密码：</span><input type="password" id="input_password">
        </p>

        <!-- 隐藏真实密码 -->
        <input type="hidden" id="md5_password" name="password">

        <p>
            <!-- <input type="submit"> -->
            <!-- 绑定事件 onclick 被点击 -->
            <button type="submit" onclick="check()">提交</button>
        </p>
    </form>

    <script src="https://cdn.bootcss.com/blueimp-md5/2.10.0/js/md5.min.js"></script>

    <script>
        function check(){
            var username = document.getElementById('username');
            var pwd = document.getElementById('input_password');
            var md5pwd = document.getElementById('md5_password');

            md5pwd.value = md5(pwd.value);
        }
    </script>
</body>
```

- 方案三：通过表单绑定提交事件 ——onsubmit

```javascript
<body>
    <form action="https://baidu.com" method="post" onsubmit="return check()">
        <h2>注册</h2>
        <p>
            <span>用户名：</span><input type="text" name="username" id="username">
        </p>
        <p>
            <span>密码：</span><input type="password" id="input_password">
        </p>

        <!-- 隐藏真实密码 -->
        <input type="hidden" id="md5_password" name="password">

        <p>
            <!-- <input type="submit"> -->
            <!-- 绑定事件 onclick 被点击 -->
            <button type="submit">提交</button>
        </p>
    </form>

    <script src="https://cdn.bootcss.com/blueimp-md5/2.10.0/js/md5.min.js"></script>

    <script>
        function check(){
            var username = document.getElementById('username');
            var pwd = document.getElementById('input_password');
            var md5pwd = document.getElementById('md5_pwd');

            md5pwd.value = md5(pwd.value);

        	//可以校验表单内容，true就是通过提交，false就是阻止提交
            return true;
        }
    </script>
</body>
```



---

> ####  **说在最后📝*：*
>
> ​	✍创作不易，如果觉得文章写得还可以的话，就不要吝啬你的 👍 啦~ ✍

---

