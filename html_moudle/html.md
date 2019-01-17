### 样式
- 内部样式
```html
    <link rel="stylesheet" type="text/css" href="001.css">
```
- 外部样式
```html
    <style type="text/css">
         h2{
             color: yellow;
         }
     </style>
```
- 内联样式
```html
    <h4 style="color: aqua">444</h4>
```

### 回到顶部

```html
    <a name="top" href=""></a>

    ...
    ...
    ...
    
    <a name="top" href="#top">回到顶部</a>
```
### 主题元素

- article

独立内容 
- section

分块或者分段
- nav

导航，侧边导航，页内导航，分页

- aside

定义其所处内容之外的内容

- time

定义日期或时间，或者两者。
- pubdate

time的一个属性

- header

定义文档的页眉（介绍信息） 
- footer

定义文档或节的页脚

-hgroup

对网页或区段（section）的标题进行组合

### 属性

- formaction 

对每个属性覆盖 form 元素的 action 属性。直接在 input 标签声明，不需要再 form 标签

- formmethod 

对每一个表单元素分别指定不同的提交方法

- formenctype

对每一个表单元素分别指定不同的编码方式

- formtarget 

对每一个表单元素提交之后在何处打开所需加载的页面

- autofocus

自动获取鼠标焦点

- required 

如果元素为空白，则不允许提交，显示提示信息

- labels

是把自己与其他标签"绑定"起来

https://www.jianshu.com/p/59b63d07ab04 

**显示联系**
```html
<!--显式联系通过<label>的 "for" 属性和目标标签的 ID 来完成-->
<from>
        <input type="radio" name="yes-no" id="yes">
        <input type="radio" name="yes-no" id="no">
</from> 

<br />

<label for="yes">点击这里也可选择 确定 选项</label> <br />
<label for="no">点击这里也可以选择 取消 选项</label> <br />
```
**隐示联系**

```html
<!--通过标签嵌套完成,如果用户点击 label 元素内的文本，则会切换到控件本身-->
<from>
    <label><input type="radio" name="yes-no">确定</label>
    <label><input type="radio" name="yes-no">取消</label>
</from>
```

- control

在标签内部（lable）放置一个表单元素，并且该标签的control属性来访问该表单元素

```
<body>

    <script>
        function setDefaultValue() {
            var lable = document.getElementById("username")
            var username = lable.control;
            username.value = "111111";
        }
    </script>

    <form>
        <lable id="username">
            <input id="txt" maxlength="6">
        </lable>

        <input type="button" value="设置默认值" onclick="setDefaultValue()">
    </form>


</body>
```
- placeholder

文本框输入之前的提示
```html
<input id="txt" maxlength="6" placeholder="请输入用户名">
```

- list

描述了其可能的值
```html
<input id="myCar" list="cars" />
    <datalist id="cars">
      <option value="BMW">
      <option value="Ford">
      <option value="Volvo">
    </datalist>
```

- autocomplete
autocomplete 属性规定表单是否应该启用自动完成功能。默认是打开的

- pattern

正则表达式验证


-  indeterminate

说明复选框处于尚未明确是否选取状态

三种状态：选中、未选中、不明确


