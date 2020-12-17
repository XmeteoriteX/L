# JS学习

## 基础结构

1. ###### <!DOCTYPE html>:文档类型声明，表示该文件为 HTML5文件。<!DOCTYPE> 声明必须是 HTML 文档的第一行，位于 <html> 标签之前

2. <html></html>标签对：<html>标签位于HTML文档的最前面，用来标识HTML文档的开始；</html>标签位于HTML文档的最后面，用来标识HTML 文档的结束；这两个标签对成对存在，中间的部分是文档的头部和主题。

3. <head></head>标签对：标签包含有关HTML文档的信息，可以包含一些辅助性标签。如<title></title>，<link /><meta />，<style></style>，<script></script>等，但是浏览器除了会在标题栏显示<title>元素的内容外，不会向用户显示head元素内的其他任何内容。

4. <body></body>标签对：它是HTML文档的主体部分，在此标签中可以包含<p><h1><br>等众多标签，<body>标签出现在</head>标签之后，且必须在闭标签</html>之前闭合。

## head

1. `head`标签为双标签，有尾标签，`<head></head>`。
2. `head`标签表示头部标签,通常用来嵌套`meta`、`title`、`style`等标签。
3. `<title>`标签：在<title>和</title>标签之间的文字内容是网页的标题信息，它会出现在浏览器的标题栏中。网页的title标签用于告诉用户和搜索引擎这个网页的主要内容是什么，搜索引擎可以通过网页标题，迅速的判断出网页的主题。每个网页的内容都是不同的，每个网页都应该有一个独一无二的title。
4. `<meta charset="UTF-8">`设置当前文件字符编码
5. `style`标签：双标签中设置当前文件样式

例如title标签：

```HTML
<head>
    <title>hello world</title>
</head>
```

```HTML
span {
color:blue;
    }
```

### 其他标签

1. span标签

2. ###### 使用<hx>标签为网页增加标题如markdown

3. ######  使用<div>标签自定义块 页面上相互关联的一组元素

4. header footer section 对应头部 底部以及定义区段 aside 侧边栏

5. br 换行 &nbsp 空格 hr 水平线标签

6. ul li 无序列表 ol li 有序列表

#### img标签

####   格式

```HTML
<img src="图片地址" alt="下载失败时的替换文本" title = "提示文本">
```

#### 

1. src：标识图像的位置；

2. alt：指定图像的描述性文本，当图像不可见时（下载不成功时），可看到该属性指定的文本；

3. title：提供在图像可见时对图像的描述(鼠标滑过图片时显示的文本)；

4. 图像可以是GIF，PNG，JPEG格式的图像文件。

   

   ### a 标签 网页添加超链接

```HTML
<a  href="目标网址"  title="鼠标滑过显示的文本">链接显示的文本</a>
```

a标签中的target属性  

```HTML
<a href="www.baidu.com" target="_blank"(新窗口打开) target="_self"(当前页面打开)>百度</a>
```

创建表格的四个元素：table、tr、th、td

1、<table>…</table>：整个表格以<table>标记开始、</table>标记结束。

2、<tr>…</tr>：表格的一行，所以有几对tr 表格就有几行。

3、<td>…</td>：表格的一个单元格，一行中包含几对<td>...</td>，说明一行中就有几列。

4、<th>…</th>：表格的头部的一个单元格，表格表头。

5、表格中列的个数，取决于一行中数据单元格的个数。

6、border属性可以为表格添加边框，属性值为数字。

**注意：**

1、table标签用来定义整个表格，为双标签，必须有结束标签。

2、table标签里面可以放caption标签和tr标签。

3、caption标签用来定义表格的标题。

4、tr标签用来设置表格的行，tr里面只能放th或者td标签，一组tr标签代表一行。

5、th用来设置表格的标题，会加粗居中显示。也就是th标签中的文本默认为粗体并且居中显示。

6、td同来设置表格的列，一组td标签代表一列。

7、table表格在没有添加border属性之前, 在浏览器中显示是没有表格线的。

## 使用thead、tbody、tfoot定义表格

<img src="https://img.mukewang.com/5e91834a000161cc06140254.jpg" alt="img" style="zoom:30%;" />

1、`<thead>` 标签定义表格的表头。该标签用于组合 HTML 表格的表头内容。

2、`<tbody>…</tbody>`：如果不加<thead><tbody><tfooter> , table表格加载完后才显示。加上这些表格结构， tbody包含行的内容下载完优先显示，不必等待表格结束后在显示，同时如果表格很长，用tbody分段，可以一部分一部分地显示。（通俗理解table 可以按结构一块块的显示，不在等整个表格加载完后显示。）

3、`<tfoot>` 元素用于对 HTML 表格中的表注（页脚）内容进行分组。

4、thead、tfoot 以及 tbody 元素使您有能力对表格中的行进行分组。当您创建某个表格时，您也许希望拥有一个标题行，一些带有数据的行，以及位于底部的一个总计行。这种划分使浏览器有能力支持独立于表格标题和页脚的表格正文滚动。当长的表格被打印时，表格的表头和页脚可被打印在包含表格数据的每张页面上。

form 创建表单 语法：

1.**<form> ：**<form>标签是成对出现的，以<form>开始，以</form>结束。

2.**action** **：**浏览者输入的数据被传送到的地方,比如一个PHP页面(save.php)。

3.**method** **：** 数据传送的方式（get/post）。‘

**注意:**

**1、所有表单控件（文本框、文本域、按钮、单选框、复选框等）都必须放在 <form></form> 标签之间（否则用户输入的信息可提交不到服务器上哦！）。**

**2、method : post/get 的区别这一部分内容属于后端程序员考虑的问题。感兴趣的小伙伴可以查看本小节的 wiki，里面有详细介绍。**

```html
<form   method="传送方式"   action="服务器文件">
<form    method="post"   action="save.php">
        <label for="username">用户名:</label>
        <input type="text" name="username" />
        <label for="pass">密码:</label>
        <input type="password" name="pass" />
</form>
```

输入输出

```HTML
<form>
   <input type="text/password" name="名称" value="文本" />
</form>
```

```HTML
<form>
  姓名：
  <input type="text" name="myName">
  <br/>
  密码：
  <input type="password" name="pass">
</form>
```

<img src="http://img.mukewang.com/52e4e9be000152ca05250275.jpg" alt="img" style="zoom:66%;" />



placeholder 占位符<img src="https://img.mukewang.com/5e918efa0001a01204260146.jpg" alt="img" style="zoom:50%;" />

```
  <input type="text" placeholder="请输入关键字">
```

数字输入框 

```
<input type="number">
```

url输入框（输入时需要以http://或者https://开头）

```
<input type="url">
```

email 同理 

#### 使用<textarea>标签创建文本域

**语法**：

```
<textarea  rows="行数" cols="列数">文本</textarea>
```

1、<textarea>标签是成对出现的，以<textarea>开始，以</textarea>结束。

2、cols ：多行输入域的列数。

3、rows ：多行输入域的行数。

4、在<textarea></textarea>标签之间可以输入默认值。

举例：

```HTML
<form  method="post" action="save.php">
        <label>联系我们</label>
        <textarea cols="50" rows="10" >在这里输入内容...</textarea>
</form>
```

#### label标签

语法：

```html
<label for="控件id名称">
```

例子：

```html
<form
  <label for="email">输入你的邮箱地址</label>
  <input type="email" id="email" placeholder="Enter email">
</form>
```

### 单选复选框框

```
语法：
<input   type="radio/checkbox"   value="值"    name="名称"   checked="checked"/>
```

1、**type:**

  当 **type="radio"** 时，控件为**单选框**

  当 **type="checkbox"** 时，控件为**复选框**

2、**value：**提交数据到服务器的值（后台程序PHP使用）

3、**name：**为控件命名，以备后台程序 ASP、PHP 使用

4、**checked：**当设置 checked="checked" 时，该选项被默认选中

## 使用select、option标签创建下拉菜单

```html
<form>
        <select>
            <option value="看书">看书</option>
            <option value="旅游" selected="selected ">旅游</option>
            <option value="运动">运动</option>
            <option value="购物">购物</option>
        </select>
    </form>
```

注意 双标签 select里面只能放option 设置selected="selected"属性，则该选项就被默认选中。

#### 提交/重置按钮

**语法**：

```HTML
<input   type="submit"   value="提交">
<input   type="reset"   value="充值">
```

type：只有当type值设置为submit/reset时，按钮才有提交/重置作用

value：按钮上显示的文字

# CSS 层叠样式表 (Cascading Style Sheets)”

 css 样式由**选择符**和**声明**组成，而**声明**又由**属性**和**值**组成

![img](http://img.mukewang.com/52fde5c30001b0fe03030117.jpg)

当有多条声明时，中间可以英文分号“;”分隔，如下所示：

```html
p{
   font-size:12px;
   color:red;
}
```



```html
<style type="text/css">
    span {
        color:blue;
    }
</style>
```

分为  内联式、嵌入式和外部式三种

优先级：内联式 > 嵌入式 > 外部式

嵌入式>外部式有一个前提：嵌入式css样式的位置一定在外部式的后面。总结来说，就是`--就近原则（离被设置元素越近优先级别越高）`。

### 内联式

把css代码直接写在现有的HTML标签中，如下面代码：

```html
<p style="color:red">这里文字是红色。</p>
<p style="color:red;font-size:12px">这里文字是红色。</p>
```

### 嵌入式

嵌入式css样式必须写在<style></style>之间，并且一般情况下嵌入式css样式写在<head></head>之间。

```html
<head>
    <meta charset="UTF-8">
    <title>嵌入式css样式</title>
    <style type="text/css">
    span {
       		color:red;
		}
</style>
</head>
```

### 外部式

外部式css样式(也可称为外联式)就是把css代码写一个单独的外部文件中，这个css样式文件以“`.css`”为扩展名，在<head>内**<u>（不是在<style>标签内）</u>**使用<link>标签将css样式文件链接到HTML文件内，如下面代码：

```html
<link href="base.css" rel="stylesheet" type="text/css" />
```

注意：

1、css样式文件名称以有意义的英文字母命名，如 main.css。

2、rel="stylesheet" type="text/css" 是固定写法不可修改。

3、<link>标签位置一般写在<head>标签之内。

### 注释

html中

```
<!--注释语句-->
```

css中

```
/*注释语句*/
```

# 选择器！！！！

### 标签选择器

```html
p{font-size:12px;line-height:1.6em;}
```

### 类选择器

类选择器在css样式编码中是最常用到的，如右侧代码编辑器中的代码:可以实现为“胆小如鼠”、“勇气”字体设置为红色。

语法：

```
.类选器名称{css样式代码;}
```

注意：

1、**英文圆点开头**

2、其中**类选器名称**可以任意起名（但不要起中文噢）

使用方法：

第一步：使用合适的标签把要修饰的内容标记起来，如下：

```
<span>胆小如鼠</span>
```

第二步：使用class="类选择器名称"为标签设置一个类，如下：

```
<span class="stress">胆小如鼠</span>
```

第三步：设置类选器css样式，如下：

```
.stress{color:red;}/*类前面要加入一个英文圆点*/
```

```html
.stress {
        color:green;
    }
```

###   ID选择器

**ID选择器只能在文档中使用一次**。

**可以使用类选择器词列表方法为一个元素同时设置多个样式。**我们可以为一个元素同时设多个样式，但只可以用类选择器的方法实现，ID选择器是不可以的（**不能使用 ID 词列表）。**

1、使用ID选择器，必须给标签添加上id属性，为标签设置id="ID名称"，而不是class="类名称"。

2、ID选择符的前面是井号**（#）**号，而不是英文圆点**（.）**。

3、id属性的值既为当前标签的id，尽量见名思意，语义化。

```html
#stress {
        color: red;
    }
<span id="stress">胆小如鼠</span>
```

### **子选择器**

即大于符号(>),用于选择指定标签元素的**第一代子元素。**如右侧代码编辑器中的代码：

```
.food>li{border:1px solid red;}
```

这行代码会使class名为food下的子元素li（水果、蔬菜）加入红色实线边框。

### 后代选择器

**包含选择器**，即加入空格,用于选择指定标签元素下的**后辈元素。**如右侧代码编辑器中的代码：

```
.first  span{color:red;}
```

子选择器（child selector）仅是指它的直接后代，或者你可以理解为作用于子元素的第一代后代。而后代选择器是作用于所有子后代元素。后代选择器通过空格来进行选择，而子选择器是通过“>”进行选择。

总结：**>**作用于元素的第一代后代，**空格**作用于元素的所有后代。

### 通用选择器

通用选择器是功能最强大的选择器，它使用一个（*）号指定，它的作用是匹配html中所有标签元素，如下使用下面代码使用html中任意标签元素字体颜色全部设置为红色：

```html
* {
	color:red;
  }
```

### 伪类选择器

它允许给html不存在的标签（标签的某种状态）设置样式，比如说我们给html中一个标签元素的鼠标滑过的状态来设置字体颜色：

```
a:hover{color:red;}
```

上面一行代码就是为 a 标签鼠标滑过的状态设置字体颜色变红。

**关于伪选择符：**

  关于伪类选择符，到目前为止，可以兼容所有浏览器的“伪类选择符”就是 a 标签上使用 :hover 了（其实伪类选择符还有很多，尤其是 css3 中，但是因为不能兼容所有浏览器，本教程只是讲了这一种最常用的）。其实 :hover 可以放在任意的标签上，比如说 p:hover，但是它们的兼容性也是很不好的，所以现在比较常用的还是 a:hover 的组合。

###  分组选择器

当你想为html中多个标签元素设置同一个样式时，可以使用分组选择符（，），如下代码为右侧代码编辑器中的h1、span标签同时设置字体颜色为红色：

```
h1,span{color:red;}
```

它相当于下面两行代码：

```
h1{color:red;}
span{color:red;}
```

# 继承

继承是一种规则，它允许样式不仅应用于某个特定html标签元素，而且应用于其后代。比如下面代码：如某种颜色应用于p标签，这个颜色设置不仅应用p标签，还应用于p标签中的所有子元素文本，这里子元素为span标签。

```
p{color:red;}

<p>三年级时，我还是一个<span>胆小如鼠</span>的小女孩。</p>
```

可见右侧结果窗口中p中的文本与span中的文本都设置为了红色。但注意有一些css样式是不具有继承性的。如border:1px solid red;

```
p{border:1px solid red;}

<p>三年级时，我还是一个<span>胆小如鼠</span>的小女孩。</p>
```

在上面例子中它代码的作用只是给p标签设置了边框为1像素、红色、实心边框线，而对于子元素span是没用起到作用的。

<img src="C:\Users\XWZ\AppData\Roaming\Typora\typora-user-images\image-20201202214332849.png" alt="image-20201202214332849" style="zoom:33%;" />

### 选择器优先级

1、如果一个元素使用了多个选择器,则会按照选择器的优先级来给定样式。

2、选择器的优先级依次是: 内联样式 > id选择器 > 类选择器 > 标签选择器 > 通配符选择器

# 权值计算-特殊性

**标签的权值为1，类选择符的权值为10，ID选择符的权值最高为100。**例如下面的代码：

```html
p{color:red;} /*权值为1*/
p span{color:green;} /*权值为1+1=2*/
.warning{color:white;} /*权值为10*/
p span.warning{color:purple;} /*权值为1+1+10=12*/
#footer .note p{color:yellow;} /*权值为100+10+1=111*/
```

**注意：还有一个权值比较特殊--继承也有权值但很低，有的文献提出它只有0.1，所以可以理解为继承的权值最低。**

## 选择器最高层级!important

如下代码：

```
p{color:red!important;}
p{color:green;}
<p class="first">三年级时，我还是一个<span>胆小如鼠</span>的小女孩。</p>
```

这时 p 段落中的文本会显示的red红色。

**注意：!important要写在分号的前面**

这里注意当网页制作者不设置css样式时，浏览器会按照自己的一套样式来显示网页。并且用户也可以在浏览器中设置自己习惯的样式，比如有的用户习惯把字号设置为大一些，使其查看网页的文本更加清楚。这时注意样式优先级为：**浏览器默认的样式 < 网页制作者样式 < 用户自己设置的样式**，但记住!important优先级样式是个例外，权值高于用户自己设置的样式。

# 使用font-family设置字体系列

我们可以使用css样式为网页中的文字设置字体、字号、颜色等样式属性。下面我们来看一个例子，下面代码实现：为网页中的文字设置字体为宋体。

```
body{font-family:"宋体";}
```

这里注意不要设置不常用的字体，因为如果用户本地电脑上如果没有安装你设置的字体，就会显示浏览器默认的字体。（因为用户是否可以看到你设置的字体样式取决于用户本地电脑上是否安装你设置的字体。）
现在一般网页喜欢设置“微软雅黑”，如下代码：

```
body{font-family:"Microsoft Yahei";}
```

或

```
body{font-family:"微软雅黑";}
```

注意：第一种方法比第二种方法兼容性更好一些。

因为这种字体即美观又可以在客户端安全的显示出来（用户本地一般都是默认安装的）。

## font-weight加粗

```
p span{font-weight:bold;}
```

## font-style设置字体样式

1、font-style可以设置字体样式，并且有种3设置方式。

2、正常字体为normal,也是font-style的默认值。

3、italic为设置字体为斜体，用于字体本身就有倾斜的样式。

4、oblique为设置倾斜的字体，强制将字体倾斜。

```html
p{
         font-style:italic;
 } 
```

## 使用color设置字体颜色

1、color属性可以设置字体颜色。

2、color的值有3种设置方式：

- 英文命令颜色

```
p{color:red;}
```

- RGB颜色

这个与 photoshop 中的 RGB 颜色是一致的，由 R(red)、G(green)、B(blue) 三种颜色的比例来配色。

```
p{color:rgb(133,45,200);}
```

每一项的值可以是 0~255 之间的整数，也可以是 0%~100% 的百分数。如：

```
p{color:rgb(20%,33%,25%);}
```

- 十六进制颜色

这种颜色设置方法是现在比较普遍使用的方法，其原理其实也是 RGB 设置，但是其每一项的值由 0-255 变成了十六进制 00-ff。

```
p{color:#00ffff;}
```

## font样式的简写方式

网页中的字体css样式代码也有他自己的缩写方式，下面是给网页设置字体的代码：

```
body{
    font-style:italic;
    font-weight:bold; 
    font-size:12px; 
    line-height:1.5em; 
    font-family:"宋体",sans-serif;
}
```

这么多行的代码其实可以缩写为一句：

```
body{
    font:italic  bold  12px/1.5em  "宋体",sans-serif;
}
```

注意：

1、使用这一简写方式你至少要指定 font-size 和 font-family 属性，其他的属性(如 font-weight、font-style、font-variant、line-height)如未指定将自动使用默认值。

2、在缩写时 font-size 与 line-height 中间要加入“/”斜扛。

一般情况下因为对于中文网站，英文还是比较少的，所以下面缩写代码比较常用：

```
body{
    font:12px/1.5em  "宋体",sans-serif;
}
```

只是有字号、行间距、中文字体、英文字体设置。

## 使用text-decoration添加文本修饰

1、text-decoration可以设置添加到文本的修饰。

2、text-decoration默认值为none, 定义标准的文本。

3、text-decoration的值为underline为定义文本下的一条线。

4、text-decoration的值为overline为定义文本上的一条线。

5、text-decoration的值为line-through为定义穿过文本的一条线，一般用于商品折扣价。

## text-indent为文本添加首行缩进

```html
   p{
    text-indent:2em;
    }
```

注意：2em的意思就是文字的2倍大小。

## line-height为文字设置行间间距

## letter/word-spacing增加或减少字符间的空白

**中文字间隔、字母间隔设置：**

如果想在网页排版中设置**文字间隔**或者**字母间隔**就可以使用   **letter-spacing** 来实现，如下面代码：

```
h1{
    letter-spacing:50px;
}
...
<h1>了不起的盖茨比</h1>
```

注意：这个样式使用在英文单词时，是设置字母与字母之间的间距。

**单词间距设置**：

如果我想设置英文单词之间的间距呢？可以使用 **word-spacing** 来实现。如下代码：

```
h1{
    word-spacing:50px;
}
...
<h1>welcome to imooc!</h1>
```

##  text-align设置文本对齐方式

为**块状元素**中的文本、图片设置居中样式

```
h1{
    text-align:center;
}
<h1>了不起的盖茨比</h1>
```

center		left		right

## background设置背景

# 长度值

长度单位总结一下，目前比较常用到px（像素）、em、% 百分比，要注意其实这三种单位都是相对单位。

**1、像素**

像素为什么是相对单位呢？因为像素指的是显示器上的小点（CSS规范中假设“90像素=1英寸”）。实际情况是浏览器会使用显示器的实际像素值有关，在目前大多数的设计者都倾向于使用像素（px）作为单位。

**2、em**

就是本元素给定字体的 font-size 值，如果元素的 font-size 为 14px ，那么 1em = 14px；如果 font-size 为 18px，那么 1em = 18px。如下代码：

```
p{font-size:12px;text-indent:2em;}
```

上面代码就是可以实现段落首行缩进 24px（也就是两个字体大小的距离）。

**下面注意一个特殊情况：**

但当给 font-size 设置单位为 em 时，此时计算的标准以 p 的父元素的 font-size 为基础。如下代码：

html:

```
<p>以这个<span>例子</span>为例。</p>
```

css:

```
p{font-size:14px}
span{font-size:0.8em;}
```

结果 span 中的字体“例子”字体大小就为 11.2px（14 * 0.8 = 11.2px）。

**3、百分比**

```
p{font-size:12px;line-height:130%}
```

设置行高（行间距）为字体的130%（12 * 1.3 = 15.6px）。

# 元素分类

在讲解CSS布局之前，我们需要提前知道一些知识，在CSS中，html中的标签元素大体被分为三种不同的类型：**块状元素**、**内联元素(又叫行内元素)**和**内联块状元素**。

```html
常用的块状元素有：

<div>、<p>、<h1>...<h6>、<ol>、<ul>、<dl>、<table>、<address>、<blockquote> 、<form>

常用的内联元素有：

<a>、<span>、<br>、<i>、<em>、<strong>、<label>、<q>、<var>、<cite>、<code>

常用的内联块状元素有：

<img>、<input>
```

## 块级元素

什么是块级元素？在html中<div>、 <p>、<h1>、<form>、<ul> 和 <li>就是块级元素。设置`display:block`就是将元素显示为块级元素。如下代码就是将**内联元素a**转换为**块状元素**，从而使a元素具有**块状元素**特点。

```
a{display:block;}
```

**块级元素特点：**

1、每个块级元素都从新的一行开始，并且其后的元素也另起一行。（真霸道，一个块级元素独占一行）

2、元素的高度、宽度、行高以及顶和底边距都可设置。

3、元素宽度在不设置的情况下，是它本身父容器的100%（和父元素的宽度一致），除非设定一个宽度。

## 内联元素

在html中，<span>、<a>、<label>、 <strong> 和<em>就是典型的**内联元素**（**行内元素**）（inline）元素。当然**块状元素**也可以通过代码`display:inline`将元素设置为**内联元素**。如下代码就是将**块状元素div**转换为**内联元素**，从而使 div 元素具有**内联元素**特点。

```
 div{
     display:inline;
 }

......

<div>我要变成内联元素</div>
```

**内联元素特点：**

1、和其他元素都在一行上；

2、元素的高度、宽度及顶部和底部边距**不可**设置；

3、元素的宽度就是它包含的文字或图片的宽度，不可改变。

##  内联块状元素

**内联块状元素（**inline-block**）**就是同时具备内联元素、块状元素的特点，代码`display:inline-block`就是将元素设置为内联块状元素。(css2.1新增)，<img>、<input>标签就是这种内联块状标签。

inline-block 元素特点：

1、和其他元素都在一行上；

2、元素的高度、宽度、行高以及顶和底边距都可设置。

## none不占据位置

```
   p{
	display: none;
	}
```

# 盒子模型

盒模型内的内容可以是文字，图片，标签等等。视频应该也可以,盒子与盒子内的内容之间的距离用 **padding** 表示,两个盒模型之间的距离用 margin 表示,盒模型的边框用 border 表示.内填充，外边距，边框都有四个方向**top,left right,buttom.

块级元素标签具备盒子模型的特点.css内定义的宽（width）和高（height），指的是填充以里的内容范围。 

因此一个元素实际宽度（盒子的宽度）= 

左边界(margin)+左边框(border)+左填充(padding)+内容宽度(width)+右填充(padding)+右边框(border)+右边界(padding)

![img](http://img.mukewang.com/539fbb3a0001304305570259.jpg)

元素的高度也是同理。

比如：

css代码：

```
div{
    width:200px;
    padding:20px;
    border:1px solid red;
    margin:10px;    
}
```

html代码：

```
<body>
   <div>文本内容</div>
</body>
```

元素的实际长度为：10px+1px+20px+200px+20px+1px+10px=262px。在chrome浏览器下可查看元素盒模型，如下图：

[![img](http://img.mukewang.com/543b4cae0001b34304300350.jpg)

## 使用border为盒子添加边框 以及边框样式

盒子模型的边框就是围绕着内容及补白的线，这条线你可以设置它的粗细、样式和颜色(边框三个属性)。

如下面代码为 div 来设置边框粗细为 2px、样式为实心的、颜色为红色的边框：

```
div{
    border:2px  solid  red;
}
```

上面是 border 代码的缩写形式，可以分开写：

```
div{
    border-width:2px;
    border-style:solid;
    border-color:red;
}
```

**注意：**

1、border-style（边框样式）常见样式有：

dashed（虚线）| dotted（点线）| solid（实线）。


2、border-color（边框颜色）中的颜色可设置为十六进制颜色，如:

```
border-color:#888;//前面的井号不要忘掉。
```


3、border-width（边框宽度）中的宽度也可以设置为：

thin | medium | thick（但不是很常用），最常还是用像素（px）。

## 设置单方向边框

```
div{border-bottom:1px solid red;}
```

## 使用border-radius设置圆角

元素边框的圆角效果可以使用border-radius属性来设置。圆角可分为左上、右上、右下、左下。如下代码：

```
 div{border-radius: 20px 10px 15px 30px;}
```

效果：

<img src="https://img.mukewang.com/5e95770b0001576e05910345.jpg" alt="img" style="zoom: 50%;" />

也可以分开写：

```
div{
    border-top-left-radius: 20px;
   border-top-right-radius: 10px;
   border-bottom-right-radius: 15px;
   border-bottom-left-radius: 30px;
}
```

如果四个圆角都为10px;可以这么写：

```
div{ border-radius:10px;}
```

如果左上角和右下角圆角效果一样为10px，右上角和左下角圆角一样为20px，可以这么写：

```
div{ border-radius:10px 20px;}
```

需要特别注意的：一个正方形，当设置圆角效果值为元素宽度一半时，显示效果为圆形。例如：

```
 div {
        width: 200px;
        height: 200px;
        border: 5px solid red;
        border-radius: 100px;
    }
```

效果：

<img src="https://img1.mukewang.com/5e957ad10001740003340337.jpg" alt="img" style="zoom:50%;" />

## 使用padding为盒子设置内边距（填充）

元素内容与边框之间是可以设置距离的，称之为“内边距（填充）”。填充也可分为上、右、下、左(顺时针)。如下代码：

```
div{padding:20px 10px 15px 30px;}
```

效果：

![img](https://img.mukewang.com/5e95733a0001dead04210227.jpg)

顺序一定不要搞混。可以分开写上面代码：

```
div{
   padding-top:20px;
   padding-right:10px;
   padding-bottom:15px;
   padding-left:30px;
}
```

如果上、右、下、左的填充都为10px;可以这么写

```
div{padding:10px;}
```

如果上下填充一样为10px，左右一样为20px，可以这么写：

```
div{padding:10px 20px;}
```

 

## 使用margin为盒子设置外边距（边界）

元素与其它元素之间的距离可以使用边界（margin）来设置。边界也是可分为上、右、下、左。如下代码：

```
div{margin:20px 10px 15px 30px;}
```

效果：

![img](https://img4.mukewang.com/5e95747a0001a39505090231.jpg)

也可以分开写：

```
div{
   margin-top:20px;
   margin-right:10px;
   margin-bottom:15px;
   margin-left:30px;
}
```

如果上右下左的边界都为10px;可以这么写：

```
div{ margin:10px;}
```

如果上下边界一样为10px，左右一样为20px，可以这么写：

```
div{ margin:10px 20px;}
```

总结一下：padding和margin的区别，padding在边框里，margin在边框外

# CSS3的布局 - css布局模型

清楚了CSS3 盒模型的基本概念、 盒模型类型， 我们就可以深入探讨网页布局的基本模型了。布局模型与盒模型一样都是 CSS3 最基本、 最核心的概念。 但布局模型是建立在盒模型基础之上，又不同于我们常说的 CSS3 布局样式或 CSS3 布局模板。如果说布局模型是本，那么 CSS3 布局模板就是末了，是外在的表现形式。 
CSS3包含3种基本的布局模型，用英文概括为：Flow、Layer 和 Float。
在网页中，元素有三种布局模型：
1、流动模型（Flow）
2、浮动模型 (Float)
3、层模型（Layer）

## 流动模型

，流动（Flow）是默认的网页布局模式。也就是说网页在默认状态下的 HTML 网页元素都是根据流动模型来分布网页内容的。

流动布局模型具有2个比较典型的特征：

第一点，**块状元素**都会在所处的**包含元素内**自上而下按顺序垂直延伸分布，因为在默认状态下，块状元素的宽度都为**100%**。实际上，块状元素都会以行的形式占据位置。如右侧代码编辑器中三个块状元素标签(div，h1，p)宽度显示为100%。

```html
<body>
    <div id="box2">box2</div>
    <!--块状元素，由于没有设置宽度，宽度默认显示为100%-->
    <h1>标题</h1>
    <!--块状元素，由于没有设置宽度，宽度默认显示为100%-->
    <p>文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段文本段。</p>
    <!--块状元素，由于没有设置宽度，宽度默认显示为100%-->
    <div id="box1">box1</div>
    <!--块状元素，由于设置了width:300px，宽度显示为300px-->
</body>
```

<img src="C:\Users\XWZ\AppData\Roaming\Typora\typora-user-images\image-20201203171655654.png" alt="image-20201203171655654" style="zoom:50%;" />

第二点，在流动模型下，**内联元素**都会在所处的包含元素内从左到右水平分布显示。（内联元素可不像块状元素这么霸道独占一行）

右侧代码编辑器中内联元素标签a、span、em、strong都是内联元素。

## 浮动模型

块状元素这么霸道都是独占一行，如果现在我们想让两个块状元素并排显示，怎么办呢？不要着急，设置元素浮动就可以实现这一愿望。

任何元素在默认情况下是不能浮动的，但可以用 CSS 定义为浮动，如 div、p、table、img 等元素都可以被定义为浮动。如下代码可以实现两个 div 元素一行显示。

```
div{
    width:200px;
    height:200px;
    border:2px red solid;
    float:left;
}
<div id="div1"></div>
<div id="div2"></div>
```

效果图

[![img](http://img.mukewang.com/540e62c60001c56a06760417.jpg)](http://img.mukewang.com/540e62c60001c56a06760417.jpg)

当然你也可以同时设置两个元素右浮动也可以实现一行显示。

```
div{
    width:200px;
    height:200px;
    border:2px red solid;
    float:right;
}
```

效果图

[![img](http://img.mukewang.com/540e632b0001f5f506760417.jpg)](http://img.mukewang.com/540e632b0001f5f506760417.jpg)

又有小伙伴问了，设置两个元素一左一右可以实现一行显示吗？当然可以：

```
div{
    width:200px;
    height:200px;
    border:2px red solid;
}
#div1{float:left;}
#div2{float:right;}
```

效果图

[![img](http://img.mukewang.com/540e63b50001f6a206760417.jpg)](http://img.mukewang.com/540e63b50001f6a206760417.jpg)

##  层模型和定位

层布局模型就像是图像软件PhotoShop中非常流行的图层编辑功能一样，每个图层能够精确定位操作，但在网页设计领域，由于网页大小的活动性，层布局没能受到热捧。但是在网页上局部使用层布局还是有其方便之处的。下面我们来学习一下html中的层布局。

如何让html元素在网页中精确定位，就像图像软件PhotoShop中的图层一样可以对每个图层能够精确定位操作。CSS定义了一组定位（positioning）属性来支持层布局模型。

层模型有三种形式：

1、**绝对定位**(position: absolute)

2、**相对定位**(position: relative)

3、**固定定位**(position: fixed)

### 绝对定位

如果想为元素设置层模型中的绝对定位，需要设置**position:absolute**(表示绝对定位)，这条语句的作用将元素从文档流中拖出来，然后使用left、right、top、bottom属性相对于其最接近的一个具有定位属性的父包含块进行绝对定位。如果不存在这样的包含块，则相对于body元素，即相对于**浏览器窗口**。

如下面代码可以实现div元素相对于浏览器窗口向右移动100px，向下移动50px。

```
div{
    width:200px;
    height:200px;
    border:2px red solid;
    position:absolute;
    left:100px;
    top:50px;
}
<div id="div1"></div>
```

效果如下：

![img](http://img.mukewang.com/53a00b130001e86707360547.jpg)

### 相对定位

如果想为元素设置层模型中的相对定位，需要设置position:relative（表示相对定位），它通过left、right、top、bottom属性确定元素在**正常文档流中**的偏移位置。相对定位完成的过程是首先按static(float)方式生成一个元素(并且元素像层一样浮动了起来)，然后相对于**以前的位置移动，**移动的方向和幅度由left、right、top、bottom属性确定，偏移前的位置保留不动。

如下代码实现相对于以前位置向下移动50px，向右移动100px;

```
#div1{
    width:200px;
    height:200px;
    border:2px red solid;
    position:relative;
    left:100px;
    top:50px;
}

<div id="div1"></div>
```


效果图：

![img](http://img.mukewang.com/53a00d2b00015c4b06190509.jpg)

什么叫做“偏移前的位置保留不动”呢？

大家可以做一个实验，在右侧代码编辑器的19行div标签的后面加入一个span标签，在标并在span标签中写入一些文字。如下代码：

```
<body>
    <div id="div1"></div><span>偏移前的位置还保留不动，覆盖不了前面的div没有偏移前的位置</span>
</body>
```

效果图：

[![img](http://img.mukewang.com/541a4bfc0001abef05940489.jpg)](http://img.mukewang.com/541a4bfc0001abef05940489.jpg)

从效果图中可以明显的看出，虽然div元素相对于以前的位置产生了偏移，但是div元素以前的位置还是保留着，所以后面的span元素是显示在了div元素以前位置的后面。

###  固定定位

fixed：表示固定定位，与absolute定位类型类似，但它的相对移动的坐标是视图（**屏幕内的网页窗口**）本身。由于视图本身是固定的，它不会随浏览器窗口的滚动条滚动而变化，除非你在屏幕中移动浏览器窗口的屏幕位置，或改变浏览器窗口的显示大小，因此固定定位的元素会始终位于浏览器窗口内视图的某个位置，不会受文档流动影响，这与background-attachment:fixed;属性功能相同。以下代码可以实现相对于**浏览器视图**向右移动100px，向下移动50px。并且拖动滚动条时位置固定不变。

```
#div1{
    width:200px;
    height:200px;
    border:2px red solid;
    position:fixed;
    left:100px;
    top:50px;
}
<p>文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本文本。</p>
....
```

##  Relative与Absolute组合使用



使用position:relative下面规范

1、参照定位的元素必须是相对定位元素的前辈元素：

```
<div id="box1"><!--参照定位的元素-->
    <div id="box2">相对参照元素进行定位</div><!--相对定位元素-->
</div>
```

从上面代码可以看出box1是box2的父元素（父元素当然也是前辈元素了）。

2、参照定位的元素必须加入position:relative;

```
#box1{
    width:200px;
    height:200px;
    position:relative;        
}
```

3、定位元素加入position:absolute，便可以使用top、bottom、left、right来进行偏移定位了。

```
#box2{
    position:absolute;
    top:20px;
    left:30px;         
}
```

这样box2就可以相对于父元素box1定位了（这里注意参照物就可以不是浏览器了，而可以自由设置了）。

## 弹性盒模型之flex属性

```html
 .box {
        background: blue;
        display: flex;
    }

    .box div {
        width: 200px;
        height: 200px;
    }

    .box1 {
        background: red;
    }

    .box2 {
        background: orange;
    }

    .box3 {
        background: green;
    }
```

1、设置display: flex属性可以把块级元素在一排显示。

2、flex需要添加在父元素上，改变子元素的排列顺序。

3、默认为从左往右依次排列,且和父元素左边没有间隙。

<img src="C:\Users\XWZ\AppData\Roaming\Typora\typora-user-images\image-20201203192851306.png" alt="image-20201203192851306" style="zoom:50%;" />

## 使用justify-content属性设置横轴排列方式

```css
 justify-content: flex-start | flex-end | center | space-between | space-around;
```

`flex-start`：交叉轴的起点对齐

```
 .box {
        background: blue;
        display: flex;
        justify-content: flex-start;
    }
```

实现效果：

[![img](https://img.mukewang.com/5e959b080001a38d25340322.jpg)](https://img.mukewang.com/5e959b080001a38d25340322.jpg)

`flex-end`：右对齐

```
 .box {
        background: blue;
        display: flex;
        justify-content: flex-end;
    }
```

实现效果：

[![img](https://img1.mukewang.com/5e959b8b0001d43b25420308.jpg)](https://img1.mukewang.com/5e959b8b0001d43b25420308.jpg)

`center`： 居中

```
 .box {
        background: blue;
        display: flex;
        justify-content: center;
    }
```

实现效果：

[![img](https://img2.mukewang.com/5e959bdd0001ad2125300303.jpg)](https://img2.mukewang.com/5e959bdd0001ad2125300303.jpg)

`space-between`：两端对齐，项目之间的间隔都相等。

```
 .box {
        background: blue;
        display: flex;
        justify-content: space-between;
    }
```

实现效果：

[![img](https://img2.mukewang.com/5e959c6400017b1c25530313.jpg)](https://img2.mukewang.com/5e959c6400017b1c25530313.jpg)

`space-around`：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。

```
.box {
        background: blue;
        display: flex;
        justify-content: space-around;
    }
```

实现效果：

[![img](https://img2.mukewang.com/5e959caf000113b125370303.jpg)](https://img2.mukewang.com/5e959caf000113b125370303.jpg)

## 使用align-items属性设置纵轴排列方式

```
        align-items: flex-start;
    }
```

实现效果：

[![img](https://img3.mukewang.com/5e95a3720001140325381051.jpg)](https://img3.mukewang.com/5e95a3720001140325381051.jpg)

`flex-end`：交叉轴的终点对齐

```
 .box {
        height: 700px;
        background: blue;
        display: flex;
        align-items: flex-end;
    }
```

实现效果：

[![img](https://img2.mukewang.com/5e95a3ca0001550a25381056.jpg)](https://img2.mukewang.com/5e95a3ca0001550a25381056.jpg)

`center`： 交叉轴的中点对齐

```
.box {
        height: 700px;
        background: blue;
        display: flex;
        align-items: center;
    }
```

实现效果：

[![img](https://img3.mukewang.com/5e9667880001796c25371056.jpg)](https://img3.mukewang.com/5e9667880001796c25371056.jpg)

`baseline`：项目的第一行文字的基线对齐。

```
.box {
        height: 700px;
        background: blue;
        display: flex;
        align-items: baseline;
    }
```

三个盒子中设置不同的字体大小，可以参考右侧编辑器中的代码进行测试。

实现效果：

[![img](https://img3.mukewang.com/5e9668ff0001f8f125341053.jpg)](https://img3.mukewang.com/5e9668ff0001f8f125341053.jpg)

`stretch（默认值）`：如果项目未设置高度或设为auto，将占满整个容器的高度。

```
 .box {
        height: 300px;
        background: blue;
        display: flex;
        align-items: stretch;
    }

    .box div {
        /*不设置高度，元素在垂直方向上铺满父容器*/
        width: 200px;
    }
```

实现效果：

[![img](https://img2.mukewang.com/5e9669ef00017e0e25390453.jpg)](https://img2.mukewang.com/5e9669ef00017e0e25390453.jpg)

## 给子元素设置flex占比

1、给子元素设置flex属性,可以设置子元素相对于父元素的占比。

2、flex属性的值只能是正整数,表示占比多少。

3、给子元素设置了flex之后,其宽度属性会失效。

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <title>flex占比</title>
    <style type="text/css">
    .box {
        height: 300px;
        background: blue;
        display: flex;
    }

    .box div {
        width: 200px;
        height: 200px;
    }

    .box1 {
        flex: 1;
        background: red;
    }

    .box2 {
        flex: 3;
        background: orange;
    }

    .box3 {
        flex: 2;
        background: green;
    }
    </style>
</head>

<body>
    <div class="box">
        <div class="box1">flex:1</div>
        <div class="box2">flex:3</div>
        <div class="box3">flex:2</div>
    </div>
</body>

</html>
```

## 水平居中设置-行内元素

我们在实际工作中常会遇到需要设置水平居中的场景，比如为了美观，文章的标题一般都是水平居中显示的。

这里我们又得分两种情况：[行内元素](http://www.imooc.com/code/2049) 还是 [块状元素](http://www.imooc.com/code/2048) ，块状元素里面又分为定宽块状元素，以及不定宽块状元素。今天我们先来了解一下行内元素怎么进行水平居中？

如果被设置元素为文本、图片等行内元素时，水平居中是通过给**父元素**设置 `text-align:center` 来实现的。(父元素和子元素：如下面的html代码中，div是“我想要在父容器中水平居中显示”这个文本的父元素。反之这个文本是div的子元素 )如下代码：

html代码：

```html
<body>
  <div class="txtCenter">我想要在父容器中水平居中显示。</div>
</body>
```

css代码：

```html
<style>
  .txtCenter{
    text-align:center;
  }
</style>
```

## 水平居中设置-定宽块状元素

当被设置元素为 [块状元素](http://www.imooc.com/code/2048) 时用 text-align：center 就不起作用了，这时也分两种情况：**定宽**块状元素和**不定宽**块状元素。

这一小节我们先来讲一讲定宽块状元素。(定宽块状元素：块状元素的宽度width为固定值。)

满足定宽和块状两个条件的元素是可以通过设置“左右margin”值为“auto”来实现居中的。我们来看个例子就是设置 div 这个块状元素水平居中：

html代码：

```
<body>
  <div>我是定宽块状元素，哈哈，我要水平居中显示。</div>
</body>
```

css代码：

```
<style>
div{
    border:1px solid red;/*为了显示居中效果明显为 div 设置了边框*/
    
    width:200px;/*定宽*/
    margin:20px auto;/* margin-left 与 margin-right 设置为 auto */
}

</style>
```

也可以写成：

```
margin-left:auto;
margin-right:auto;
```

注意：元素的“上下 margin” 是可以随意设置的

## 实现盒子水平垂直居中

、利用父元素设置相对定位,子元素设置绝对定位,那么子元素就是相对于父元素定位的特性。

2、子元素设置上和左偏移的值都为50%，是元素的左上角在父元素中心点的位置。效果：

[![img](https://img2.mukewang.com/5e967c3d0001fbbf25600616.jpg)](https://img2.mukewang.com/5e967c3d0001fbbf25600616.jpg)

3、然后再用margin给上和左都给负的自身宽高的一半,就能达到垂直水平居中的效果。

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>已知宽高实现盒子水平垂直居中</title>
    <style type="text/css">
    .box {
        border: 1px solid #00ee00;
        height: 300px;
        position:relative;

    }

    .box1 {
         position:absolute;
        width: 200px;
        height: 200px;
        border: 1px solid red;
       
        top:50%;
        left:50%;
        margin:-100px 0 0 -100px;
    }
    </style>
</head>

<body>
    <div class="box">
        <div class="box1"></div>
    </div>
</body>

</html>
```

1、利用父元素设置相对定位,子元素设置绝对定位,那么子元素就是相对于父元素定位的特性。

2、子元素设置上和左偏移的值都为50%。

3、然后再用css3属性translate位移,给上和左都位移-50%距离，就能达到垂直水平居中的效果。

```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>宽高不定实现盒子水平垂直居中</title>
    <style type="text/css">
    .box {
        border: 1px solid #00ee00;
        height: 300px;
        position: relative;
    }

    .box1 {
        border: 1px solid red;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    </style>
</head>

<body>
    <div class="box">
        <div class="box1">
            慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网慕课网
        </div>
    </div>
</body>

</html>
```

# JS正式学习

### typeof输出数据类型

### parseInt方法用于将字符串转为整数。

如果字符串头部有空格，空格会被自动去除。字符串转为整数的时候，是一个个字符依次转换，如果遇到不能转为数字的字符，就不再进行下去，返回已经转好的部分。

### parseFloat方法用于将一个字符串转为浮点数。

会自动过滤字符串前导的空格`parseFloat`会将空字符串转为`NaN`。

这些特点使得`parseFloat`的转换结果不同于`Number`函数。

### isNaN方法可以用来判断一个值是否为`NaN`。

`isNaN`只对数值有效，如果传入其他值，会被先转成数值。比如，传入字符串的时候，字符串会被先转成`NaN`，所以最后返回`true`，这一点要特别引起注意。也就是说，`isNaN`为`true`的值，有可能不是`NaN`，而是一个字符串。

### isFinite方法返回一个布尔值，表示某个值是否为正常的数值。

除了`Infinity`、`-Infinity`、`NaN`和`undefined`这几个值会返回`false`，`isFinite`对于其他的数值都会返回`true`。

字符串默认只能写在一行内，分成多行将会报错。

```js
'a
b
c'
// SyntaxError: Unexpected token ILLEGAL
```

上面代码将一个字符串分成三行，JavaScript 就会报错。

如果长字符串必须分成多行，可以在每一行的尾部使用反斜杠。

```js
var longString = 'Long \
long \
long \
string';

longString
// "Long long long string"
```

反斜杠的后面必须是换行符，而不能有其他字符（比如空格），否则会报错。

### 连接运算符（`+`）

可以连接多个单行字符串，将长字符串拆成多行书写，输出的时候也是单行。

```js
var longString = 'Long '
  + 'long '
  + 'long '
  + 'string';
```

如果想输出多行字符串，有一种利用多行注释的变通方法。

```javascript
(function () { /*
line 1
line 2
line 3
*/}).toString().split('\n').slice(1, -1).join('\n')
// "line 1
// line 2
// line 3"
```

上面的例子中，输出的字符串就是多行。

## 反斜杠

反斜杠还有三种特殊用法。

（1）`\HHH`

反斜杠后面紧跟三个八进制数（`000`到`377`），代表一个字符。`HHH`对应该字符的 Unicode 码点，比如`\251`表示版权符号。显然，这种方法只能输出256种字符。

（2）`\xHH`

`\x`后面紧跟两个十六进制数（`00`到`FF`），代表一个字符。`HH`对应该字符的 Unicode 码点，比如`\xA9`表示版权符号。这种方法也只能输出256种字符。

（3）`\uXXXX`

`\u`后面紧跟四个十六进制数（`0000`到`FFFF`），代表一个字符。`XXXX`对应该字符的 Unicode 码点，比如`\u00A9`表示版权符号。

如果在非特殊字符前面使用反斜杠，则反斜杠会被省略。

```js
'\a'
// "a"
```

上面代码中，`a`是一个正常字符，前面加反斜杠没有特殊含义，反斜杠会被自动省略。

如果字符串的正常内容之中，需要包含反斜杠，则反斜杠前面需要再加一个反斜杠，用来对自身转义。

```js
"Prev \\ Next"
// "Prev \ Next"
```

## 字符串与数组

字符串可以被视为字符数组，因此可以使用数组的方括号运算符，用来返回某个位置的字符（位置编号从0开始）。

```js
var s = 'hello';
s[0] // "h"
s[1] // "e"
s[4] // "o"

// 直接对字符串使用方括号运算符
'hello'[1] // "e"
```

如果方括号中的数字超过字符串的长度，或者方括号中根本不是数字，则返回`undefined`。

```js
'abc'[3] // undefined
'abc'[-1] // undefined
'abc'['x'] // undefined
```

但是，字符串与数组的相似性仅此而已。实际上，无法改变字符串之中的单个字符。

字符串可以被视为字符数组，因此可以使用数组的方括号运算符，用来返回某个位置的字符（位置编号从0开始）。

```js
var s = 'hello';
s[0] // "h"
s[1] // "e"
s[4] // "o"

// 直接对字符串使用方括号运算符
'hello'[1] // "e"
```

如果方括号中的数字超过字符串的长度，或者方括号中根本不是数字，则返回`undefined`。

```js
'abc'[3] // undefined
'abc'[-1] // undefined
'abc'['x'] // undefined
```

### length属性返回字符串的长度，该属性也是无法改变的。

## Base64 转码

有时，文本里面包含一些不可打印的符号，比如 ASCII 码0到31的符号都无法打印出来，这时可以使用 Base64 编码，将它们转成可以打印的字符。另一个场景是，有时需要以文本格式传递二进制数据，那么也可以使用 Base64 编码。

所谓 Base64 就是一种编码方法，可以将任意值转成 0～9、A～Z、a-z、`+`和`/`这64个字符组成的可打印字符。使用它的主要目的，不是为了加密，而是为了不出现特殊字符，简化程序的处理。

 JavaScript 原生提供两个 Base64 相关的方法。

btoa()`：任意值转为 Base64 编码

atob()：Base64 编码转为原来的值

## 对象

对象（object）是 JavaScript 语言的核心概念，也是最重要的数据类型。

什么是对象？简单说，对象就是一组“键值对”（key-value）的集合，是一种无序的复合数据集合。

```js
var obj = {
  foo: 'Hello',
  bar: 'World'
};
```

上面代码中，大括号就定义了一个对象，它被赋值给变量`obj`，所以变量`obj`就指向一个对象。该对象内部包含两个键值对（又称为两个“成员”），第一个键值对是`foo: 'Hello'`，其中`foo`是“键名”（成员的名称），字符串`Hello`是“键值”（成员的值）。键名与键值之间用冒号分隔。第二个键值对是`bar: 'World'`，`bar`是键名，`World`是键值。两个键值对之间用**逗号分隔**。

## 属性读取

读取对象的属性，有两种方法，一种是使用点运算符，还有一种是使用方括号运算符。

```js
var obj = {
  p: 'Hello World'
};

obj.p // "Hello World"
obj['p'] // "Hello World"
```

上面代码分别采用点运算符和方括号运算符，读取属性`p`。

请注意，如果使用方括号运算符，键名必须放在引号里面，否则会被当作变量处理。

```js
var foo = 'bar';

var obj = {
  foo: 1,
  bar: 2
};

obj.foo  // 1
obj[foo]  // 2
```

上面代码中，引用对象`obj`的`foo`属性时，如果使用点运算符，`foo`就是字符串；如果使用方括号运算符，但是不使用引号，那么`foo`就是一个变量，指向字符串`bar`。

方括号运算符内部还可以使用表达式。

```js
obj['hello' + ' world']
obj[3 + 3]
```

数字键可以不加引号，因为会自动转成字符串。

```js
var obj = {
  0.7: 'Hello World'
};

obj['0.7'] // "Hello World"
obj[0.7] // "Hello World"
```

上面代码中，对象`obj`的数字键`0.7`，加不加引号都可以，因为会被自动转为字符串。

注意，数值键名不能使用点运算符（因为会被当成小数点），只能使用方括号运算符。

```js
var obj = {
  123: 'hello world'
};

obj.123 // 报错
obj[123] // "hello world"
```

上面代码的第一个表达式，对数值键名`123`使用点运算符，结果报错。第二个表达式使用方括号运算符，结果就是正确的。

## 属性的赋值

点运算符和方括号运算符，不仅可以用来读取值，还可以用来赋值。

```js
var obj = {};

obj.foo = 'Hello';
obj['bar'] = 'World';
```

上面代码中，分别使用点运算符和方括号运算符，对属性赋值。

JavaScript 允许属性的“后绑定”，也就是说，你可以在任意时刻新增属性，没必要在定义对象的时候，就定义好属性。

```js
var obj = { p: 1 };

// 等价于

var obj = {};
obj.p = 1;
```

### 属性的查看

查看一个对象本身的所有属性，可以使用`Object.keys`方法。

```js
var obj = {
  key1: 1,
  key2: 2
};

Object.keys(obj);
// ['key1', 'key2']
```

### 属性的删除：delete 命令

`delete`命令用于删除对象的属性，删除成功后返回`true`。

```js
var obj = { p: 1 };
Object.keys(obj) // ["p"]

delete obj.p // true
obj.p // undefined
Object.keys(obj) // []
```

上面代码中，`delete`命令删除对象`obj`的`p`属性。删除后，再读取`p`属性就会返回`undefined`，而且`Object.keys`方法的返回值也不再包括该属性。

注意，删除一个不存在的属性，`delete`不报错，而且返回`true`。

```js
var obj = {};
delete obj.p // true
```

上面代码中，对象`obj`并没有`p`属性，但是`delete`命令照样返回`true`。因此，不能根据`delete`命令的结果，认定某个属性是存在的。

只有一种情况，`delete`命令会返回`false`，那就是该属性存在，且不得删除。

```js
var obj = Object.defineProperty({}, 'p', {
  value: 123,
  configurable: false
});

obj.p // 123
delete obj.p // false
```

上面代码之中，对象`obj`的`p`属性是不能删除的，所以`delete`命令返回`false`（关于`Object.defineProperty`方法的介绍，请看《标准库》的 Object 对象一章）。

另外，需要注意的是，`delete`命令只能删除对象本身的属性，无法删除继承的属性（关于继承参见《面向对象编程》章节）。

```
var obj = {};
delete obj.toString // true
obj.toString // function toString() { [native code] }
```

上面代码中，`toString`是对象`obj`继承的属性，虽然`delete`命令返回`true`，但该属性并没有被删除，依然存在。这个例子还说明，即使`delete`返回`true`，该属性依然可能读取到值。

### 属性是否存在：in 运算符

`in`运算符用于检查对象是否包含某个属性（注意，检查的是键名，不是键值），如果包含就返回`true`，否则返回`false`。它的左边是一个字符串，表示属性名，右边是一个对象。

```js
var obj = { p: 1 };
'p' in obj // true
'toString' in obj // true
```

`in`运算符的一个问题是，它不能识别哪些属性是对象自身的，哪些属性是继承的。就像上面代码中，对象`obj`本身并没有`toString`属性，但是`in`运算符会返回`true`，因为这个属性是继承的。

这时，可以使用对象的`hasOwnProperty`方法判断一下，是否为对象自身的属性。

```js
var obj = {};
if ('toString' in obj) {
  console.log(obj.hasOwnProperty('toString')) // false
}
```

### 属性的遍历：for...in 循环

`for...in`循环用来遍历一个对象的全部属性。

```js
var obj = {a: 1, b: 2, c: 3};

for (var i in obj) {
  console.log('键名：', i);
  console.log('键值：', obj[i]);
}
// 键名： a
// 键值： 1
// 键名： b
// 键值： 2
// 键名： c
// 键值： 3
```

`for...in`循环有两个使用注意点。

- 它遍历的是对象所有可遍历（enumerable）的属性，会跳过不可遍历的属性。
- 它不仅遍历对象自身的属性，还遍历继承的属性。

举例来说，对象都继承了`toString`属性，但是`for...in`循环不会遍历到这个属性。

```js
var obj = {};

// toString 属性是存在的
obj.toString // toString() { [native code] }

for (var p in obj) {
  console.log(p);
} // 没有任何输出
```

上面代码中，对象`obj`继承了`toString`属性，该属性不会被`for...in`循环遍历到，因为它默认是“不可遍历”的。关于对象属性的可遍历性，参见《标准库》章节中 Object 一章的介绍。

如果继承的属性是可遍历的，那么就会被`for...in`循环遍历到。但是，一般情况下，都是只想遍历对象自身的属性，所以使用`for...in`的时候，应该结合使用`hasOwnProperty`方法，在循环内部判断一下，某个属性是否为对象自身的属性。

```js
var person = { name: '老张' };

for (var key in person) {
  if (person.hasOwnProperty(key)) {
    console.log(key);
  }
}
// name
```

## with 语句

`with`语句的格式如下：

```js
with (对象) {
  语句;
}
```

它的作用是操作同一个对象的多个属性时，提供一些书写的方便。

```js
// 例一
var obj = {
  p1: 1,
  p2: 2,
};
with (obj) {
  p1 = 4;
  p2 = 5;
}
// 等同于
obj.p1 = 4;
obj.p2 = 5;

// 例二
with (document.links[0]){
  console.log(href);
  console.log(title);
  console.log(style);
}
// 等同于
console.log(document.links[0].href);
console.log(document.links[0].title);
console.log(document.links[0].style);
```

注意，如果`with`区块内部有变量的赋值操作，必须是当前对象已经存在的属性，否则会创造一个当前作用域的全局变量。

```js
var obj = {};
with (obj) {
  p1 = 4;
  p2 = 5;
}

obj.p1 // undefined
p1 // 4
```

上面代码中，对象`obj`并没有`p1`属性，对`p1`赋值等于创造了一个全局变量`p1`。正确的写法应该是，先定义对象`obj`的属性`p1`，然后在`with`区块内操作它。

这是因为`with`区块没有改变作用域，它的内部依然是当前作用域。这造成了`with`语句的一个很大的弊病，就是绑定对象不明确。

```js
with (obj) {
  console.log(x);
}
```

单纯从上面的代码块，根本无法判断`x`到底是全局变量，还是对象`obj`的一个属性。这非常不利于代码的除错和模块化，编译器也无法对这段代码进行优化，只能留到运行时判断，这就拖慢了运行速度。因此，建议不要使用`with`语句，可以考虑用一个临时变量代替`with`。

```js
with(obj1.obj2.obj3) {
  console.log(p1 + p2);
}

// 可以写成
var temp = obj1.obj2.obj3;
console.log(temp.p1 + temp.p2);
```

## 概述

### 函数的声明

JavaScript 有三种声明函数的方法。

**（1）function 命令**

`function`命令声明的代码区块，就是一个函数。`function`命令后面是函数名，函数名后面是一对圆括号，里面是传入函数的参数。函数体放在大括号里面。

```javascript
function print(s) {
  console.log(s);
}
```

上面的代码命名了一个`print`函数，以后使用`print()`这种形式，就可以调用相应的代码。这叫做函数的声明（Function Declaration）。

**（2）函数表达式**

除了用`function`命令声明函数，还可以采用变量赋值的写法。

```javascript
var print = function(s) {
  console.log(s);
};
```

这种写法将一个匿名函数赋值给变量。这时，这个匿名函数又称函数表达式（Function Expression），因为赋值语句的等号右侧只能放表达式。

采用函数表达式声明函数时，`function`命令后面不带有函数名。如果加上函数名，该函数名只在函数体内部有效，在函数体外部无效。

```
var print = function x(){
  console.log(typeof x);
};

x
// ReferenceError: x is not defined

print()
// function
```

上面代码在函数表达式中，加入了函数名`x`。这个`x`只在函数体内部可用，指代函数表达式本身，其他地方都不可用。这种写法的用处有两个，一是可以在函数体内部调用自身，二是方便除错（除错工具显示函数调用栈时，将显示函数名，而不再显示这里是一个匿名函数）。因此，下面的形式声明函数也非常常见。

```
var f = function f() {};
```

需要注意的是，函数的表达式需要在语句的结尾加上分号，表示语句结束。而函数的声明在结尾的大括号后面不用加分号。总的来说，这两种声明函数的方式，差别很细微，可以近似认为是等价的。

**（3）Function 构造函数**

第三种声明函数的方式是`Function`构造函数。

```
var add = new Function(
  'x',
  'y',
  'return x + y'
);

// 等同于
function add(x, y) {
  return x + y;
}
```

上面代码中，`Function`构造函数接受三个参数，除了最后一个参数是`add`函数的“函数体”，其他参数都是`add`函数的参数。

你可以传递任意数量的参数给`Function`构造函数，只有最后一个参数会被当做函数体，如果只有一个参数，该参数就是函数体。

```
var foo = new Function(
  'return "hello world";'
);

// 等同于
function foo() {
  return 'hello world';
}
```

`Function`构造函数可以不使用`new`命令，返回结果完全一样。

总的来说，这种声明函数的方式非常不直观，几乎无人使用。

### 函数的重复声明

如果同一个函数被多次声明，后面的声明就会覆盖前面的声明。

```
function f() {
  console.log(1);
}
f() // 2

function f() {
  console.log(2);
}
f() // 2
```

上面代码中，后一次的函数声明覆盖了前面一次。而且，由于函数名的提升（参见下文），前一次声明在任何时候都是无效的，这一点要特别注意。

### 圆括号运算符，return 语句和递归

调用函数时，要使用圆括号运算符。圆括号之中，可以加入函数的参数。

```
function add(x, y) {
  return x + y;
}

add(1, 1) // 2
```

上面代码中，函数名后面紧跟一对圆括号，就会调用这个函数。

函数体内部的`return`语句，表示返回。JavaScript 引擎遇到`return`语句，就直接返回`return`后面的那个表达式的值，后面即使还有语句，也不会得到执行。也就是说，`return`语句所带的那个表达式，就是函数的返回值。`return`语句不是必需的，如果没有的话，该函数就不返回任何值，或者说返回`undefined`。

函数可以调用自身，这就是递归（recursion）。下面就是通过递归，计算斐波那契数列的代码。

```
function fib(num) {
  if (num === 0) return 0;
  if (num === 1) return 1;
  return fib(num - 2) + fib(num - 1);
}

fib(6) // 8
```

上面代码中，`fib`函数内部又调用了`fib`，计算得到斐波那契数列的第6个元素是8。

### 第一等公民

JavaScript 语言将函数看作一种值，与其它值（数值、字符串、布尔值等等）地位相同。凡是可以使用值的地方，就能使用函数。比如，可以把函数赋值给变量和对象的属性，也可以当作参数传入其他函数，或者作为函数的结果返回。函数只是一个可以执行的值，此外并无特殊之处。

由于函数与其他数据类型地位平等，所以在 JavaScript 语言中又称函数为第一等公民。

```
function add(x, y) {
  return x + y;
}

// 将函数赋值给一个变量
var operator = add;

// 将函数作为参数和返回值
function a(op){
  return op;
}
a(add)(1, 1)
// 2
```

### 函数名的提升

JavaScript 引擎将函数名视同变量名，所以采用`function`命令声明函数时，整个函数会像变量声明一样，被提升到代码头部。所以，下面的代码不会报错。

```
f();

function f() {}
```

表面上，上面代码好像在声明之前就调用了函数`f`。但是实际上，由于“变量提升”，函数`f`被提升到了代码头部，也就是在调用之前已经声明了。但是，如果采用赋值语句定义函数，JavaScript 就会报错。

```
f();
var f = function (){};
// TypeError: undefined is not a function
```

上面的代码等同于下面的形式。

```
var f;
f();
f = function () {};
```

上面代码第二行，调用`f`的时候，`f`只是被声明了，还没有被赋值，等于`undefined`，所以会报错。

注意，如果像下面例子那样，采用`function`命令和`var`赋值语句声明同一个函数，由于存在函数提升，最后会采用`var`赋值语句的定义。

```
var f = function () {
  console.log('1');
}

function f() {
  console.log('2');
}

f() // 1
```

上面例子中，表面上后面声明的函数`f`，应该覆盖前面的`var`赋值语句，但是由于存在函数提升，实际上正好反过来。

## 函数的属性和方法

### name 属性

函数的`name`属性返回函数的名字。

```
function f1() {}
f1.name // "f1"
```

如果是通过变量赋值定义的函数，那么`name`属性返回变量名。

```
var f2 = function () {};
f2.name // "f2"
```

但是，上面这种情况，只有在变量的值是一个匿名函数时才是如此。如果变量的值是一个具名函数，那么`name`属性返回`function`关键字之后的那个函数名。

```
var f3 = function myName() {};
f3.name // 'myName'
```

上面代码中，`f3.name`返回函数表达式的名字。注意，真正的函数名还是`f3`，而`myName`这个名字只在函数体内部可用。

`name`属性的一个用处，就是获取参数函数的名字。

```
var myFunc = function () {};

function test(f) {
  console.log(f.name);
}

test(myFunc) // myFunc
```

上面代码中，函数`test`内部通过`name`属性，就可以知道传入的参数是什么函数。

### length 属性

函数的`length`属性返回函数预期传入的参数个数，即函数定义之中的参数个数。

```
function f(a, b) {}
f.length // 2
```

上面代码定义了空函数`f`，它的`length`属性就是定义时的参数个数。不管调用时输入了多少个参数，`length`属性始终等于2。

`length`属性提供了一种机制，判断定义时和调用时参数的差异，以便实现面向对象编程的“方法重载”（overload）。

### toString()

函数的`toString()`方法返回一个字符串，内容是函数的源码。

```
function f() {
  a();
  b();
  c();
}

f.toString()
// function f() {
//  a();
//  b();
//  c();
// }
```

上面示例中，函数`f`的`toString()`方法返回了`f`的源码，包含换行符在内。

对于那些原生的函数，`toString()`方法返回`function (){[native code]}`。

```
Math.sqrt.toString()
// "function sqrt() { [native code] }"
```

上面代码中，`Math.sqrt()`是 JavaScript 引擎提供的原生函数，`toString()`方法就返回原生代码的提示。

函数内部的注释也可以返回。

```
function f() {/*
  这是一个
  多行注释
*/}

f.toString()
// "function f(){/*
//   这是一个
//   多行注释
// */}"
```

利用这一点，可以变相实现多行字符串。

```
var multiline = function (fn) {
  var arr = fn.toString().split('\n');
  return arr.slice(1, arr.length - 1).join('\n');
};

function f() {/*
  这是一个
  多行注释
*/}

multiline(f);
// " 这是一个
//   多行注释"
```

上面示例中，函数`f`内部有一个多行注释，`toString()`方法拿到`f`的源码后，去掉首尾两行，就得到了一个多行字符串。

## 函数作用域

### 定义

作用域（scope）指的是变量存在的范围。在 ES5 的规范中，JavaScript 只有两种作用域：一种是全局作用域，变量在整个程序中一直存在，所有地方都可以读取；另一种是函数作用域，变量只在函数内部存在。ES6 又新增了块级作用域，本教程不涉及。

对于顶层函数来说，函数外部声明的变量就是全局变量（global variable），它可以在函数内部读取。

```
var v = 1;

function f() {
  console.log(v);
}

f()
// 1
```

上面的代码表明，函数`f`内部可以读取全局变量`v`。

在函数内部定义的变量，外部无法读取，称为“局部变量”（local variable）。

```
function f(){
  var v = 1;
}

v // ReferenceError: v is not defined
```

上面代码中，变量`v`在函数内部定义，所以是一个局部变量，函数之外就无法读取。

函数内部定义的变量，会在该作用域内覆盖同名全局变量。

```
var v = 1;

function f(){
  var v = 2;
  console.log(v);
}

f() // 2
v // 1
```

上面代码中，变量`v`同时在函数的外部和内部有定义。结果，在函数内部定义，局部变量`v`覆盖了全局变量`v`。

注意，对于`var`命令来说，局部变量只能在函数内部声明，在其他区块中声明，一律都是全局变量。

```
if (true) {
  var x = 5;
}
console.log(x);  // 5
```

上面代码中，变量`x`在条件判断区块之中声明，结果就是一个全局变量，可以在区块之外读取。

### 函数内部的变量提升

与全局作用域一样，函数作用域内部也会产生“变量提升”现象。`var`命令声明的变量，不管在什么位置，变量声明都会被提升到函数体的头部。

```
function foo(x) {
  if (x > 100) {
    var tmp = x - 100;
  }
}

// 等同于
function foo(x) {
  var tmp;
  if (x > 100) {
    tmp = x - 100;
  };
}
```

### 函数本身的作用域

函数本身也是一个值，也有自己的作用域。它的作用域与变量一样，就是其声明时所在的作用域，与其运行时所在的作用域无关。

```
var a = 1;
var x = function () {
  console.log(a);
};

function f() {
  var a = 2;
  x();
}

f() // 1
```

上面代码中，函数`x`是在函数`f`的外部声明的，所以它的作用域绑定外层，内部变量`a`不会到函数`f`体内取值，所以输出`1`，而不是`2`。

总之，函数执行时所在的作用域，是定义时的作用域，而不是调用时所在的作用域。

很容易犯错的一点是，如果函数`A`调用函数`B`，却没考虑到函数`B`不会引用函数`A`的内部变量。

```
var x = function () {
  console.log(a);
};

function y(f) {
  var a = 2;
  f();
}

y(x)
// ReferenceError: a is not defined
```

上面代码将函数`x`作为参数，传入函数`y`。但是，函数`x`是在函数`y`体外声明的，作用域绑定外层，因此找不到函数`y`的内部变量`a`，导致报错。

同样的，函数体内部声明的函数，作用域绑定函数体内部。

```
function foo() {
  var x = 1;
  function bar() {
    console.log(x);
  }
  return bar;
}

var x = 2;
var f = foo();
f() // 1
```

上面代码中，函数`foo`内部声明了一个函数`bar`，`bar`的作用域绑定`foo`。当我们在`foo`外部取出`bar`执行时，变量`x`指向的是`foo`内部的`x`，而不是`foo`外部的`x`。正是这种机制，构成了下文要讲解的“闭包”现象。

## 参数

### 概述

函数运行的时候，有时需要提供外部数据，不同的外部数据会得到不同的结果，这种外部数据就叫参数。

```
function square(x) {
  return x * x;
}

square(2) // 4
square(3) // 9
```

上式的`x`就是`square`函数的参数。每次运行的时候，需要提供这个值，否则得不到结果。

### 参数的省略

函数参数不是必需的，JavaScript 允许省略参数。

```
function f(a, b) {
  return a;
}

f(1, 2, 3) // 1
f(1) // 1
f() // undefined

f.length // 2
```

上面代码的函数`f`定义了两个参数，但是运行时无论提供多少个参数（或者不提供参数），JavaScript 都不会报错。省略的参数的值就变为`undefined`。需要注意的是，函数的`length`属性与实际传入的参数个数无关，只反映函数预期传入的参数个数。

但是，没有办法只省略靠前的参数，而保留靠后的参数。如果一定要省略靠前的参数，只有显式传入`undefined`。

```
function f(a, b) {
  return a;
}

f( , 1) // SyntaxError: Unexpected token ,(…)
f(undefined, 1) // undefined
```

上面代码中，如果省略第一个参数，就会报错。

### 传递方式

函数参数如果是原始类型的值（数值、字符串、布尔值），传递方式是传值传递（passes by value）。这意味着，在函数体内修改参数值，不会影响到函数外部。

```
var p = 2;

function f(p) {
  p = 3;
}
f(p);

p // 2
```

上面代码中，变量`p`是一个原始类型的值，传入函数`f`的方式是传值传递。因此，在函数内部，`p`的值是原始值的拷贝，无论怎么修改，都不会影响到原始值。

但是，如果函数参数是复合类型的值（数组、对象、其他函数），传递方式是传址传递（pass by reference）。也就是说，传入函数的原始值的地址，因此在函数内部修改参数，将会影响到原始值。

```
var obj = { p: 1 };

function f(o) {
  o.p = 2;
}
f(obj);

obj.p // 2
```

上面代码中，传入函数`f`的是参数对象`obj`的地址。因此，在函数内部修改`obj`的属性`p`，会影响到原始值。

注意，如果函数内部修改的，不是参数对象的某个属性，而是替换掉整个参数，这时不会影响到原始值。

```
var obj = [1, 2, 3];

function f(o) {
  o = [2, 3, 4];
}
f(obj);

obj // [1, 2, 3]
```

上面代码中，在函数`f()`内部，参数对象`obj`被整个替换成另一个值。这时不会影响到原始值。这是因为，形式参数（`o`）的值实际是参数`obj`的地址，重新对`o`赋值导致`o`指向另一个地址，保存在原地址上的值当然不受影响。

### 同名参数

如果有同名的参数，则取最后出现的那个值。

```
function f(a, a) {
  console.log(a);
}

f(1, 2) // 2
```

上面代码中，函数`f()`有两个参数，且参数名都是`a`。取值的时候，以后面的`a`为准，即使后面的`a`没有值或被省略，也是以其为准。

```
function f(a, a) {
  console.log(a);
}

f(1) // undefined
```

调用函数`f()`的时候，没有提供第二个参数，`a`的取值就变成了`undefined`。这时，如果要获得第一个`a`的值，可以使用`arguments`对象。

```
function f(a, a) {
  console.log(arguments[0]);
}

f(1) // 1
```

### arguments 对象

**（1）定义**

由于 JavaScript 允许函数有不定数目的参数，所以需要一种机制，可以在函数体内部读取所有参数。这就是`arguments`对象的由来。

`arguments`对象包含了函数运行时的所有参数，`arguments[0]`就是第一个参数，`arguments[1]`就是第二个参数，以此类推。这个对象只有在函数体内部，才可以使用。

```
var f = function (one) {
  console.log(arguments[0]);
  console.log(arguments[1]);
  console.log(arguments[2]);
}

f(1, 2, 3)
// 1
// 2
// 3
```

正常模式下，`arguments`对象可以在运行时修改。

```
var f = function(a, b) {
  arguments[0] = 3;
  arguments[1] = 2;
  return a + b;
}

f(1, 1) // 5
```

上面代码中，函数`f()`调用时传入的参数，在函数内部被修改成`3`和`2`。

严格模式下，`arguments`对象与函数参数不具有联动关系。也就是说，修改`arguments`对象不会影响到实际的函数参数。

```
var f = function(a, b) {
  'use strict'; // 开启严格模式
  arguments[0] = 3;
  arguments[1] = 2;
  return a + b;
}

f(1, 1) // 2
```

上面代码中，函数体内是严格模式，这时修改`arguments`对象，不会影响到真实参数`a`和`b`。

通过`arguments`对象的`length`属性，可以判断函数调用时到底带几个参数。

```
function f() {
  return arguments.length;
}

f(1, 2, 3) // 3
f(1) // 1
f() // 0
```

**（2）与数组的关系**

需要注意的是，虽然`arguments`很像数组，但它是一个对象。数组专有的方法（比如`slice`和`forEach`），不能在`arguments`对象上直接使用。

如果要让`arguments`对象使用数组方法，真正的解决方法是将`arguments`转为真正的数组。下面是两种常用的转换方法：`slice`方法和逐一填入新数组。

```
var args = Array.prototype.slice.call(arguments);

// 或者
var args = [];
for (var i = 0; i < arguments.length; i++) {
  args.push(arguments[i]);
}
```

**（3）callee 属性**

`arguments`对象带有一个`callee`属性，返回它所对应的原函数。

```
var f = function () {
  console.log(arguments.callee === f);
}

f() // true
```

可以通过`arguments.callee`，达到调用函数自身的目的。这个属性在严格模式里面是禁用的，因此不建议使用。

## 函数的其他知识点

### 闭包

闭包（closure）是 JavaScript 语言的一个难点，也是它的特色，很多高级应用都要依靠闭包实现。

理解闭包，首先必须理解变量作用域。前面提到，JavaScript 有两种作用域：全局作用域和函数作用域。函数内部可以直接读取全局变量。

```
var n = 999;

function f1() {
  console.log(n);
}
f1() // 999
```

上面代码中，函数`f1`可以读取全局变量`n`。

但是，正常情况下，函数外部无法读取函数内部声明的变量。

```
function f1() {
  var n = 999;
}

console.log(n)
// Uncaught ReferenceError: n is not defined(
```

上面代码中，函数`f1`内部声明的变量`n`，函数外是无法读取的。

如果出于种种原因，需要得到函数内的局部变量。正常情况下，这是办不到的，只有通过变通方法才能实现。那就是在函数的内部，再定义一个函数。

```
function f1() {
  var n = 999;
  function f2() {
　　console.log(n); // 999
  }
}
```

上面代码中，函数`f2`就在函数`f1`内部，这时`f1`内部的所有局部变量，对`f2`都是可见的。但是反过来就不行，`f2`内部的局部变量，对`f1`就是不可见的。这就是 JavaScript 语言特有的"链式作用域"结构（chain scope），子对象会一级一级地向上寻找所有父对象的变量。所以，父对象的所有变量，对子对象都是可见的，反之则不成立。

既然`f2`可以读取`f1`的局部变量，那么只要把`f2`作为返回值，我们不就可以在`f1`外部读取它的内部变量了吗！

```
function f1() {
  var n = 999;
  function f2() {
    console.log(n);
  }
  return f2;
}

var result = f1();
result(); // 999
```

上面代码中，函数`f1`的返回值就是函数`f2`，由于`f2`可以读取`f1`的内部变量，所以就可以在外部获得`f1`的内部变量了。

闭包就是函数`f2`，即能够读取其他函数内部变量的函数。由于在 JavaScript 语言中，只有函数内部的子函数才能读取内部变量，因此可以把闭包简单理解成“定义在一个函数内部的函数”。闭包最大的特点，就是它可以“记住”诞生的环境，比如`f2`记住了它诞生的环境`f1`，所以从`f2`可以得到`f1`的内部变量。在本质上，闭包就是将函数内部和函数外部连接起来的一座桥梁。

闭包的最大用处有两个，一个是可以读取外层函数内部的变量，另一个就是让这些变量始终保持在内存中，即闭包可以使得它诞生环境一直存在。请看下面的例子，闭包使得内部变量记住上一次调用时的运算结果。

```
function createIncrementor(start) {
  return function () {
    return start++;
  };
}

var inc = createIncrementor(5);

inc() // 5
inc() // 6
inc() // 7
```

上面代码中，`start`是函数`createIncrementor`的内部变量。通过闭包，`start`的状态被保留了，每一次调用都是在上一次调用的基础上进行计算。从中可以看到，闭包`inc`使得函数`createIncrementor`的内部环境，一直存在。所以，闭包可以看作是函数内部作用域的一个接口。

为什么闭包能够返回外层函数的内部变量？原因是闭包（上例的`inc`）用到了外层变量（`start`），导致外层函数（`createIncrementor`）不能从内存释放。只要闭包没有被垃圾回收机制清除，外层函数提供的运行环境也不会被清除，它的内部变量就始终保存着当前值，供闭包读取。

闭包的另一个用处，是封装对象的私有属性和私有方法。

```
function Person(name) {
  var _age;
  function setAge(n) {
    _age = n;
  }
  function getAge() {
    return _age;
  }

  return {
    name: name,
    getAge: getAge,
    setAge: setAge
  };
}

var p1 = Person('张三');
p1.setAge(25);
p1.getAge() // 25
```

上面代码中，函数`Person`的内部变量`_age`，通过闭包`getAge`和`setAge`，变成了返回对象`p1`的私有变量。

注意，外层函数每次运行，都会生成一个新的闭包，而这个闭包又会保留外层函数的内部变量，所以内存消耗很大。因此不能滥用闭包，否则会造成网页的性能问题。

### 立即调用的函数表达式（IIFE）

根据 JavaScript 的语法，圆括号`()`跟在函数名之后，表示调用该函数。比如，`print()`就表示调用`print`函数。

有时，我们需要在定义函数之后，立即调用该函数。这时，你不能在函数的定义之后加上圆括号，这会产生语法错误。

```
function(){ /* code */ }();
// SyntaxError: Unexpected token (
```

产生这个错误的原因是，`function`这个关键字即可以当作语句，也可以当作表达式。

```
// 语句
function f() {}

// 表达式
var f = function f() {}
```

当作表达式时，函数可以定义后直接加圆括号调用。

```
var f = function f(){ return 1}();
f // 1
```

上面的代码中，函数定义后直接加圆括号调用，没有报错。原因就是`function`作为表达式，引擎就把函数定义当作一个值。这种情况下，就不会报错。

为了避免解析的歧义，JavaScript 规定，如果`function`关键字出现在行首，一律解释成语句。因此，引擎看到行首是`function`关键字之后，认为这一段都是函数的定义，不应该以圆括号结尾，所以就报错了。

函数定义后立即调用的解决方法，就是不要让`function`出现在行首，让引擎将其理解成一个表达式。最简单的处理，就是将其放在一个圆括号里面。

```
(function(){ /* code */ }());
// 或者
(function(){ /* code */ })();
```

上面两种写法都是以圆括号开头，引擎就会认为后面跟的是一个表达式，而不是函数定义语句，所以就避免了错误。这就叫做“立即调用的函数表达式”（Immediately-Invoked Function Expression），简称 IIFE。

注意，上面两种写法最后的分号都是必须的。如果省略分号，遇到连着两个 IIFE，可能就会报错。

```
// 报错
(function(){ /* code */ }())
(function(){ /* code */ }())
```

上面代码的两行之间没有分号，JavaScript 会将它们连在一起解释，将第二行解释为第一行的参数。

推而广之，任何让解释器以表达式来处理函数定义的方法，都能产生同样的效果，比如下面三种写法。

```
var i = function(){ return 10; }();
true && function(){ /* code */ }();
0, function(){ /* code */ }();
```

甚至像下面这样写，也是可以的。

```
!function () { /* code */ }();
~function () { /* code */ }();
-function () { /* code */ }();
+function () { /* code */ }();
```

通常情况下，只对匿名函数使用这种“立即执行的函数表达式”。它的目的有两个：一是不必为函数命名，避免了污染全局变量；二是 IIFE 内部形成了一个单独的作用域，可以封装一些外部无法读取的私有变量。

```
// 写法一
var tmp = newData;
processData(tmp);
storeData(tmp);

// 写法二
(function () {
  var tmp = newData;
  processData(tmp);
  storeData(tmp);
}());
```

上面代码中，写法二比写法一更好，因为完全避免了污染全局变量。

## eval 命令

### 基本用法

`eval`命令接受一个字符串作为参数，并将这个字符串当作语句执行。

```
eval('var a = 1;');
a // 1
```

上面代码将字符串当作语句运行，生成了变量`a`。

如果参数字符串无法当作语句运行，那么就会报错。

```
eval('3x') // Uncaught SyntaxError: Invalid or unexpected token
```

放在`eval`中的字符串，应该有独自存在的意义，不能用来与`eval`以外的命令配合使用。举例来说，下面的代码将会报错。

```
eval('return;'); // Uncaught SyntaxError: Illegal return statement
```

上面代码会报错，因为`return`不能单独使用，必须在函数中使用。

如果`eval`的参数不是字符串，那么会原样返回。

```
eval(123) // 123
```

`eval`没有自己的作用域，都在当前作用域内执行，因此可能会修改当前作用域的变量的值，造成安全问题。

```
var a = 1;
eval('a = 2');

a // 2
```

上面代码中，`eval`命令修改了外部变量`a`的值。由于这个原因，`eval`有安全风险。

为了防止这种风险，JavaScript 规定，如果使用严格模式，`eval`内部声明的变量，不会影响到外部作用域。

```
(function f() {
  'use strict';
  eval('var foo = 123');
  console.log(foo);  // ReferenceError: foo is not defined
})()
```

上面代码中，函数`f`内部是严格模式，这时`eval`内部声明的`foo`变量，就不会影响到外部。

不过，即使在严格模式下，`eval`依然可以读写当前作用域的变量。

```
(function f() {
  'use strict';
  var foo = 1;
  eval('foo = 2');
  console.log(foo);  // 2
})()
```

上面代码中，严格模式下，`eval`内部还是改写了外部变量，可见安全风险依然存在。

总之，`eval`的本质是在当前作用域之中，注入代码。由于安全风险和不利于 JavaScript 引擎优化执行速度，所以一般不推荐使用。通常情况下，`eval`最常见的场合是解析 JSON 数据的字符串，不过正确的做法应该是使用原生的`JSON.parse`方法。

### eval 的别名调用

前面说过`eval`不利于引擎优化执行速度。更麻烦的是，还有下面这种情况，引擎在静态代码分析的阶段，根本无法分辨执行的是`eval`。

```
var m = eval;
m('var x = 1');
x // 1
```

上面代码中，变量`m`是`eval`的别名。静态代码分析阶段，引擎分辨不出`m('var x = 1')`执行的是`eval`命令。

为了保证`eval`的别名不影响代码优化，JavaScript 的标准规定，凡是使用别名执行`eval`，`eval`内部一律是全局作用域。

```
var a = 1;

function f() {
  var a = 2;
  var e = eval;
  e('console.log(a)');
}

f() // 1
```

上面代码中，`eval`是别名调用，所以即使它是在函数中，它的作用域还是全局作用域，因此输出的`a`为全局变量。这样的话，引擎就能确认`e()`不会对当前的函数作用域产生影响，优化的时候就可以把这一行排除掉。

`eval`的别名调用的形式五花八门，只要不是直接调用，都属于别名调用，因为引擎只能分辨`eval()`这一种形式是直接调用。

```
eval.call(null, '...')
window.eval('...')
(1, eval)('...')
(eval, eval)('...')
```

上面这些形式都是`eval`的别名调用，作用域都是全局作用域。







