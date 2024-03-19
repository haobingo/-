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



# 一、HTML

## 1.1 锚点链接

> 锚点链接是超链接中的一种。锚点的妙处之一在于，`你可以使用它链接到文档中的某个特定位置`。例如，有些网页内容较多，页面过长，用户需要不停的使用浏览器上的滚动条来查看文档中的内容。这时为了增强用户体验，可以在网页中插入锚点链接。

>锚点链接的具体使用场景有 2 种：
>
>- 跳转到`当前页面的指定位置`
>
>- 跳转到`其他页面的指定位置`

### 跳转到当前页面的指定位置

方法一：不过HTML5已经废弃了name属性。

1. 在要跳转到的位置所在的标签中添加了`id`或者`name`属性，并为其赋值；
2. 使用 <a> 标签设置锚点，href 属性值为`#`+`id`或`#`+`name`属性值。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>锚点链接</title>
</head>
<body>
    <p id="content"></p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <a href="#content">回到顶部</a>
</body>
</html>
```

```html
<!DOCTYPE html>
<html>
	<head>
    <meta charset="UTF-8">
    <title>锚点设置</title>
	</head>
	<body>
     <a href="#bottom" name="top">去底部</a>
    <div style="height: 5000px; width: 300px; background-color: #123">这里演示如何跳转到页面头部和底部</div>
    <a href="#top" name="bottom">回到顶部</a>
	</body>
</html>
```




方法二：可以达到同样的效果

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>锚点链接</title>
</head>
<body>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <p>这是页面内容</p>
    <a href="#top">回到顶部</a>
</body>
</html>
```

`#top`，其中`#`表示位置信息，网页的顶端默认是`#top`，所以如果是跳转到浏览器的顶端，不需要写锚点的第一步操作,，也就是说不需要为标签设置 id 属性。

> 注意：href 属性中的 top 也可以省略，不影响正常使用。



### 跳转到其他页面的指定位置

> 使用锚点链接，也可以跳转到其他页面的指定位置。与跳转到当前页面的指定位置相比，它需要在`#`前加上要跳转到的页面的路径。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>index页面</title>
</head>
<body>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <p>index页面</p>
    <h2 id="index">这是h2标题</h2>
</body>
</html>
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>锚点链接</title>
</head>
<body>
    <a href="./index.html#index">跳转到index页面</a>
</body>
</html>
```

在 <a> 标签中，href 属性指向了 index.html 页面中 id 为 index 的标签。点击后，发生相应的跳转。





## 1.2 自定义列表

> 自定义列表不仅仅是一列项目，而是项目及其注释的组合。
>
> 自定义列表以 <dl> 标签开始。每个自定义列表项以 <dt> 开始。每个自定义列表项的定义以 <dd> 开始。

- dl：define list
- dt：define term

```html
<dl>
    <dt>Coffee</dt>
    <dd>- black hot drink</dd>
    <dt>Milk</dt>
    <dd>- white cold drink</dd>
</dl>
```

## 1.3 表格的跨行跨列

> 一般使用<td>元素的colspan属性来实现单元格跨列操作，使用<td>元素的rowspan属性来实现单元格的跨行操作。
>
> colspan属性规定单元格可横跨的列数，所有浏览器都支持colspan属性。其取值为number

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230407082415197.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230407082415197" style="zoom:50%;" />

```html
<table border="1">
  <tr>
    <th colspan="3">物资详情说明</th>
  </tr>
  <tr>
    <td colspan="2" align="center">数量(支)</td>
    <td rowspan="2">重量(吨)</td>
  </tr>
  <tr>
    <td>实发数</td>    
    <td>实收数</td>
  </tr>
  <tr>
    <td>12</td>    
    <td>10</td>
    <td>100.00</td>
  </tr>
</table>
```

## 1.4 视频和音频内容

- 视频---video
- 音频---audio

```html
<video src="" controls autoplay width="" height=""></video>
<audio src="" controls autoplay width="" height=""></audio>
```



## 1.5 页面结构规范

| 元素名  |      描述      |
| :-----: | :------------: |
| header  |    页眉部分    |
| footer  |    页脚部分    |
| section |  一块独立区域  |
| article | 独立的文章内容 |
|  aside  |  侧边栏目录等  |
|   nav   | 导航类辅助内容 |

## 1.6 ifram内联框架

>  iframe标签是一个内联框架，即用来在当前 HTML 页面中嵌入另一个文档的，且所有主流浏览器都支持iframe标签。

> height可以设置框架显示的高度
>
> - width可以设置框架显示的宽度
> - name可以定义框架的名称
> - frameborder用来定义是否需要显示边框，取值为1表示需要边框
> - scrolling用来设置框架是否需要滚动条，取值可以是yes,no,auto
> - src用于设置框架的地址，可以使页面地址，也可以是图片地址
> - align用于设置元素对齐方式，取值可以是left，right，top，middle，bottom

```html
<iframe src="" width="" height="" frameborder="">
    
</iframe>
```

## 1.7 表单

### 1.7.1 form标签

> 元素按照一定的格式定义了表单和确定表单行为的属性。当您想要创建一个 HTML 表单时，都必须从这个元素开始，然后把所有内容都放在里面。

- action：属性定义了在提交表单时，应该把所收集的数据送给谁（URL）去处理。
-  属性定义了发送数据的 HTTP 方法（通常是 `get` 或 `post`）。

```html
<form action="" method=""></form>
```

### 1.7.2 原生表单部件

> 主要针对input标签，表单输入元素。

> **`<input>`** 元素用于为基于 Web 的表单创建交互式控件，以便接受来自用户的数据。取决于设备和[用户代理](https://developer.mozilla.org/zh-CN/docs/Glossary/User_agent)不同，表单可以使用各种类型的输入数据和控件。`<input>` 元素是目前是 HTML 中最强大、最复杂的元素之一，因为它有大量的输入类型和属性组合。

==input的一些属性值==

|   属性    |                             说明                             |
| :-------: | :----------------------------------------------------------: |
|   type    |                        指定元素的类型                        |
|   name    | 指定表单元素的名称，以便后端使用，同时可以为type中radio和checkbox进行分组 |
|   value   |                         元素的初始值                         |
|   size    |                    指定表单元素的初始宽度                    |
| maxlength |           type为text或password时，输入的最大字符数           |
|  checked  |         type为radio或checkbox时，指定按钮是否被选中          |



> `<input>` 的工作方式相当程度上取决于 [`type`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/input#type) 属性的值，不同的 type 值会在各自的参考页中进行介绍。如果未指定此属性，则采用的默认类型为 `text`。

==type一些属性值==

<table>
    <thead>
        <tr>
            <th>值</th>
            <th>示例代码</th>
            <th>描述</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>text</td>
            <td><code>&lt;input type&#61;&#34;text&#34;&gt;</code></td>
            <td>默认。定义单行输入字段&#xff0c;用户可在其中输入文本。默认是 20 个字符</td>
        </tr>
        <tr>
            <td>password</td>
            <td><code>&lt;input type&#61;&#34;password&#34;&gt;</code></td>
            <td>定义密码字段。字段中的字符会被遮蔽</td>
        </tr>
        <tr>
            <td>button</td>
            <td><code>&lt;input type&#61;&#34;button&#34;&gt;</code></td>
            <td>定义可点击的按钮&#xff08;大多与 JavaScript 使用来启动脚本&#xff09;</td>
        </tr>
        <tr>
            <td>checkbox</td>
            <td><code>&lt;input type&#61;&#34;checkbox&#34;&gt;</code></td>
            <td>定义复选框</td>
        </tr>
        <tr>
            <td>radio</td>
            <td><code>&lt;input type&#61;&#34;radio&#34;&gt;</code></td>
       	 	<td>定义单选按钮</td></tr><tr><td>submit</td>
        	<td><code>&lt;input type&#61;&#34;submit&#34;&gt;</code></td>
        	<td>定义提交按钮。提交按钮向服务器发送数据</td></tr>
        <tr>
            <td>file</td>
            <td><code>&lt;input type&#61;&#34;file&#34;&gt;</code></td>
            <td>定义输入字段和 “浏览…” 按钮&#xff0c;供文件上传</td>
        </tr>
        <tr>
            <td>hidden</td><td><code>&lt;input type&#61;&#34;hidden&#34;&gt;</code></td><td>定义隐藏输入字段</td></tr><tr><td>image</td><td><code>&lt;input type&#61;&#34;image&#34;&gt;</code></td><td>定义图像作为提交按钮</td></tr><tr><td>reset</td><td><code>&lt;input type&#61;&#34;reset&#34;&gt;</code></td><td>定义重置按钮。重置按钮会将所有表单字段重置为初始值</td></tr><tr><td>email</td><td><code>&lt;input type&#61;&#34;email&#34;&gt;</code></td><td>定义用于 e-mail 地址的文本字段</td></tr><tr><td>url</td><td><code>&lt;input type&#61;&#34;url&#34;&gt;</code></td><td>定义用于 URL 的文本字段</td></tr><tr><td>tel</td><td><code>&lt;input type&#61;&#34;tel&#34;&gt;</code></td><td>定义用于电话号码的文本字段</td></tr><tr><td>number</td><td><code>&lt;input type&#61;&#34;number&#34;&gt;</code></td><td>定义带有 spinner 控件的数字字段</td></tr><tr><td>range</td><td><code>&lt;input type&#61;&#34;range&#34;&gt;</code></td><td>定义带有 slider 控件的数字字段</td></tr><tr><td>search</td><td><code>&lt;input type&#61;&#34;search&#34;&gt;</code></td><td>定义用于搜索的文本字段</td></tr><tr><td>color</td><td><code>&lt;input type&#61;&#34;color&#34;&gt;</code></td><td>定义拾色器</td></tr><tr><td>date</td><td><code>&lt;input type&#61;&#34;date&#34;&gt;</code></td><td>定义日期字段&#xff08;带有 calendar 控件&#xff09;</td></tr><tr><td>datetime</td><td><code>&lt;input type&#61;&#34;datetime&#34;&gt;</code></td><td>定义日期字段&#xff08;带有 calendar 和 time 控件&#xff09;</td></tr><tr><td>datetime-local</td><td><code>&lt;input type&#61;&#34;datetime-local&#34;&gt;</code></td><td>定义日期字段&#xff08;带有 calendar 和 time 控件&#xff09;</td></tr><tr><td>month</td><td><code>&lt;input type&#61;&#34;month&#34;&gt;</code></td><td>定义日期字段的月&#xff08;带有 calendar 控件&#xff09;</td></tr><tr><td>week</td><td><code>&lt;input type&#61;&#34;week&#34;&gt;</code></td><td>定义日期字段的周&#xff08;带有 calendar 控件&#xff09;</td></tr><tr><td>time</td><td><code>&lt;input type&#61;&#34;time&#34;&gt;</code></td><td>定义日期字段的时、分、秒&#xff08;带有 time 控件&#xff09;</td></tr></tbody></table>



**详细说明：**

- <input type="text">：如果一个input没有type属性，那么它会是默认type=“text”。没有什么特别的，就是允许输入文本，简单明了。
- <input type="password">：顾名思义，在用户输入密码的时候建议使用这个属性而非text，使用了这个属性，用户输入的文字将会变成*，我们是看不到的，当然，传给后台会是用户输入的文本。有些手机端上不会一开始就是*，而是会短暂的明文显示用户输入的最后一个字符，然后才是*。
- <input type="button">：一个按钮，表单按钮，和单纯的元素相比，没有使用CSS方便，所以如果你不是想用这个按钮去重置（reset）或者提交（submit），并且为了和传统的表单风格相比配的话，建议你都使用而不是，`再按钮上添加文字，使用value属性` 。
- <input type="checkbox">：复选框，默认是小方格，可以选择多个。
- <input type="radio">：单选框，默认是小圆圈，只能选择一个，`为了达到单选的效果，需要对其进行分组，使用name属性`。
- <input type="submit">：通常被认为是一个提交按钮，当点击此按钮时，提交本表单的数据。
- <input type="file">：这个类型和其他的不同，其他无非是一些选择，或者输入文本，而这个属性，是为了能让用户上传本地文件。
- <input type="hidden">：该属性是用来隐藏掉该表单控件。
- <input type="image">：该属性接受所有<img>，将会像submit一样提交图片，如果想上传图片，照片，不妨使用这个属性。
- <input type="reset">：重置按钮，点了这个按钮，表单的数据全部重置，也就是清空的意思。慎用！

### 1.7.3 下拉框

> select

- 实际上，multiple 和 size 这两个属性只要设置了其中一个，下拉列表就可以显示多项。如果只设置 size，而不设置 multiple，得到的是一个不允许多选但是可以显示多项的下拉列表；
- < select> 标签的 name 属性不显示在页面上，主要用来提交数据；
- < option> 标签的 value 属性也不显示在页面上，主要用来定义提交给服务器的值；
- < option> 标签的 disabled 属性禁用的是列表中的某一项；
- < select >  标签的 disabled 属性禁用的是整个列表。

```html
<form action="http://vip.biancheng.net/login.php" method="post">
    年龄区间： 
    <select name="selectList" multiple>
        <option selected="selected" value="underage">18岁以下</option>
        <option value="teens">18-28岁</option>
        <option selected="selected" value="youth">28-38岁</option>
        <option value="more">38岁以上</option>
    </select>
</form>
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230408090457869.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230408090457869" style="zoom:67%;" />



### 1.7.4 文本域

>   <textarea name="文本域名称”value="文本域默认值" rows="行教”cols="列数">   </ textarea>



```html
<form action="#" method="post">
    文本域：<br /><br />
    <textarea id="text1" name="description">默认大小 </textarea><br /><br />
    <textarea id="text2" name="description">使用width属性和height属性设置文本域的宽度为200px，高度为200px。</textarea>
</form>
```



<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230408090839293.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230408090839293" style="zoom:67%;" />





### 1.7.5 文件域 

> ​	**注意1:文件域用来选择文件，还需要一个`上传按钮 `**
>
> **注意2:此处有两个name，上传文件是将文件提交给了文件域对应的files 	并非按钮所对应的upload。也就是说选择文件后value=所上传的文件，上传后files=所上传的文件**

> 参考：[这个文章](https://blog.csdn.net/weixin_44234912/article/details/109380563)

```html
<p>文件域： 	
    <input type="file" name="files"> 	
    <input type="button" value="上传" name="upload"> 	
</p>
```

### 1.7.6 简单验证信息

- 邮箱验证

```html
<p>邮箱:
    <input type="email" name="email">
</p>
```

<p>邮箱:
    <input type="email" name="email">
</p>

- URL验证

```html
<p>URL:
    <input type="email" name="email">
</p>
```

<p>URL:
    <input type="email" name="email">
</p>

- 数字验证

```html
<p>数字:
    <input type="number" name="number" max="100" min="0" step="10">
</p>
```

<p>数字:
    <input type="number" name="number" max="100" min="0" step="10">
</p>

### 1.7.7 滑块

> - max - 规定允许的最大值。
> - min - 规定允许的最小值。
> - step - 规定合法数字间隔。
> - value - 规定默认值。

```html
<p>音量:
    <input type="range" name="音量" id="range" value="20" min="0" max="200" step="1">
</p>
```

<p>音量:
    <input type="range" name="音量" id="range" value="20" min="0" max="200" step="1">
</p>

### 1.7.8 搜索框

```html
<p>
	<input type="search" name="search"> <button type="button">搜索</button>
</p>
```

<p>
	<input type="search" name="search"> <button type="button">搜索</button>
</p>



### 1.7.9 表单应用

|   属性   |  作用  |             说明             |
| :------: | :----: | :--------------------------: |
| readonly |  只读  | 默认value中的值，不允许修改  |
| disabled |  禁用  | 单选框中，禁用男，只能选择女 |
|  hidden  |  隐藏  | 隐藏某个标签，但实际是存在的 |
|  value   | 默认值 |             通用             |

### 1.7.10 增强鼠标可用性

> 当用户将鼠标移至邮箱文字区域，同样可以触发文本框，进行输入。

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230408095952979.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230408095952979" style="zoom:67%;" />

> for 属性规定 label 与哪个表单元素绑定。

>  html中 for属性的作用是关联的作用，一般是和表单中某个控件的id属性一直，表示关联此控件

```html
<p>
    <label for="mark">你点我试试</label>
    <input id="mark">
</p>
```



### 1.7.11 表单初级验证

> 1、可以减轻服务器的压力
>
> 2、为了数据安全性
>
> 3、为了提交性能，减少垃圾数据的提交

- placeholder：很多时候[文本框](https://so.csdn.net/so/search?q=文本框&spm=1001.2101.3001.7020)的`提示信息`可以帮助人们更好更快的进行浏览，我们可以可以placeholder来给用户提示信息，比如我们写一个个签，提示信息为请填写你的个性签名。

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230408102023458.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20230408102023458" style="zoom:67%;" />

- required:很多时候都会有`必填选项`，比如平时在学校填的问卷，我们使用required属性即可判断是否非空。
- pattern:`正则表达式`，我们可以自定义一个验证方式，比如我们需要填写邮箱，不使用html的email，而是使用pattern。

[速查正则表达式](https://www.jb51.net/tools/regexsc.htm)

![image-20230408102251254](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20230408102251254.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```html
<p>
    自定义邮箱：
    <input type="text" name="My_email" pattern="/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$//^[a-z\d]+(\.[a-z\d]+)*@([\da-z](-[\da-z])?)+(\.{1,2}[a-z]+)+$/或\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*">
</p>
```





---

> <strong> 🚀<font color = orange>先看后赞，养成习惯！</font>🚀</strong>
>
> <strong> 🚀<font color = red> 先看后赞，养成习惯！</font>🚀</strong>

> **🎈觉得文章写得不错的老铁们，点赞评论关注走一波！谢谢啦！🎈**

---

、
