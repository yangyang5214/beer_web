- 选择器分组
```html
h1,h2,a{
    color:red
}

body {
    color:blue
}
```
- 继承
```html
<body>

    <h1>111</h1>
    <h2>222</h2>
    <a href="#img">222</a>

    <p>我是一个段落</p>
</body>
```

body 定义了样式，则 p 继承了样式

- 派生选择器

上下文选择器
```html
li strong {
    font-style: italic;
    font-weight: normal;
  }
```

- id 选择器

```
# 选择 id

<div id = pid>
</div>

#pid a{
    font-style: italic;
} 
```
- 类选择器

类选择器 和 派生选择器结合使用
```
. 选择

<p class="p_class">我是一个段落 class</p>

.p_class{
    color:red
}
```

- 属性选择器

````html
<p title="t">title</p>

[title] {
    color: aquamarine;
}
````

- 背景
```html
body {
    color:blue;
    background-color: black;
    background-image: url('bg.jpg');
}
```
- 文本

```html

```

- 字体

- 链接

```html
a:link{
    color: #FF0000
    <!--去掉下划线-->
    text-decoration: ;
}

a:visited{
    color: #00FF00
}

a:active{

}

a:hover{

}
```

- 列表

```html
ul li {
    list-style-image: url('../img/吐司面包.png')
}
```

- 轮廓

```html
outline-width
outline-color
outline-style
```
- 定位

相对定位
```html
设置为相对定位的元素框会偏移某个距离。元素仍然保持其未定位前的形状，它原本所占的空间仍保留。
#box_relative {
  position: relative;
  left: 30px;
  top: 20px;
}
```
绝对定位
```html
设置为绝对定位的元素框从文档流完全删除，并相对于其包含块定位，包含块可能是文档中的另一个元素或者是初始包含块。元素原先在正常文档流中所占的空间会关闭，就好像该元素原来不存在一样。元素定位后生成一个块级框，而不论原来它在正常流中生成何种类型的框。

重点是脱离文档流
#box_relative {
  position: absolute;
  left: 30px;
  top: 20px;
}
```

浮动
```html
也是不在文档流中
#position{
    background-color: red;
    width: 200px;
    height: 400px;
    float: right
}
```

```html
float: left
float: right

clear: both
clear: left
clear: right
```

- 盒子模型
```html
margin
border
padding
content
```

- 对齐

margin
```html
居中
.content{
    width: 200px;
    height: 1500px;
    margin-left: auto;
    margin-right: auto;
    background-color: red
}
```
position
```html
居右
.content{
    width: 200px;
    height: 1500px;
    position: absolute;
    right: 0px;
    background-color: red
}
```

float
```html
居左
.content{
    width: 200px;
    height: 1500px;
    float: left;
    background-color: red
}
```
- 导航栏
- 图片
```html
透明度
opacity : 0
```

- 选择器

元素选择器
```html
h1{
}
```
选择器分组
```html
h1,h2{
}
```
通配符
```html
*{
}
```
类选择器
```html
.div{
}
```
id 选择器
```html
#div{
}
```
多类选择器
```html
.class.class{
}
```
属性选择器
```html
[title]{
}

[title~=title]{
}
```
后代选择器
```html
p li{
}
```
相邻兄弟选择器
```html
相邻兄弟选择器（Adjacent sibling selector）可选择紧接在另一元素后的元素，且二者有相同父元素。

h1 + p{
}
```
- 多列
```html
.content{
    column-count: 3;
}
```
- 瀑布流

