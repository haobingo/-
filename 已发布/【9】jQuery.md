[TOC]

# 一、基本介绍

> 推荐API网站：[jQuery文档](https://jquery.cuishifeng.cn/)

>推荐下载网站：[jQuery下载](https://jquery.com/)

> 推荐在线CDN加速网站：[jQuery CDN加速](https://www.jq22.com/cdn/)和[BOOTCDN加速](https://www.bootcdn.cn/jquery/)

==公式==：`$（selector）. action（）；`

选择器：

- 标签选择器：标签名
- id选择器：# + id名
- 类选择器：.  + 类名

```javascript
<body>
    <a href="#" id="test_js">点我</a>
    <a href="#" id="test_jquery">点我</a>

    <script src="https://cdn.bootcdn.net/ajax/libs/jquery/3.6.3/jquery.min.js"></script>

    <script>

        //使用JavaScript
        var test_js = document.getElementById('test_js');

        //使用jQuery
        $('#test_jquery').click(function(){
            alert('我是jQuery！');
        });
    </script>
</body>
```



# 二、事件举例

> action

|     事件      |   说明    |
| :-----------: | :-------: |
| mousedown（） | 鼠标按下  |
| mousemove（） | 鼠标移动  |
|     pageX     | 获取x坐标 |
|     pageY     | 获取y坐标 |



```javascript
<body>
    <!-- 获取鼠标当前的坐标 -->
  
    <h2>mouse坐标：<span id="mouseMove"></span></h2>
    <div id="divMouse" style="width:500px;height:500px;border:2px solid red">
          <h1>在这里移动鼠标试试</h1>
    </div>

    <script src="https://cdn.bootcdn.net/ajax/libs/jquery/3.6.3/jquery.min.js"></script>
    <script>
        // 当网页元素加载完毕之后，响应事件

        // 简写：$(function(){});
        $(document).ready(function(){
            $('#divMouse').mousemove(function(e){
                $('#mouseMove').text('x:'+e.pageX+';'+'y:'+e.pageY);
            });
        });
    </script>
</body>
```



# 三、操作DOM元素

```javascript
<body>
    <ul id="test_ul">
        <li class="js">JavaScript</li>
        <li id="py">Python</li>
        <li name="jq">jQuery</li>
    </ul>

    <script src="https://cdn.bootcdn.net/ajax/libs/jquery/3.6.3/jquery.min.js"></script>
    <script>

        // innerText();
        $('#test_ul li[name=jq]').text(); // 属性选择器;有参数就取值，没有参数就设置值

        // innerHtml();
        $('#py').html("<li id='py'>新Python</li>");

        // sytle
        $('.js').css({'color':'red','background-color':'green'});//键值对，单个用逗号，多个用冒号

        // 元素的显示与隐藏------------display:none
        $('#py').hide();
        $('#py').show();

        //使用 toggle（）切换显示与隐藏
        $('#py').toggle();
    </script>
</body>
```




---

> ####  **说在最后📝*：*
>
> ​	✍创作不易，如果觉得文章写得还可以的话，就不要吝啬你的 👍 啦~ ✍

---