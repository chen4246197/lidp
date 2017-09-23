# HTML 
## 1.由来：
万维网一个网页（page）就是一个超级媒体文档, 在主页中通常有包括指向其他相关页面或者节点的指针（即超级链接也就是URL  Uniform Resource Locator）过激活它可以使浏览器可以更加方便的获取新的网页，这就是html获取广泛应用的原因，在逻辑上将一些列的页面的集合可以称之为网站（WebSite）,html超级纹板标记语言是为网页创建和链接其他网页而设计的一种标记语言。

## 2. 编辑工具
：适合初学者常见的前端编译集成环境（IDE是"集成开发环境）有WebStorm、HBuilder（国内开发的）、sublime和Dreamweaver

## 3.轻量级语言
    ：记事本、++**sublime Text**++、notepad++

- 4.html或.htm为后缀
    .htm是在win32时代，系统只能识别3位扩展名时使用的，而现在一般都使用.html。
-     以浏览器打开这个文件，即是一个解析的过程。
>
```
<!DOCTYPE html>文档声明，它是Document Type Definition的英文缩写，意思是文档类型定义
<html lang="en">属性
里面可嵌套<title>、<meta>、<link>、<script>、<style>
<head>头部
    <meta charset="UTF-8">有关页面的元信息（meta-information）也是关键字它只可以放在head中
    <title>Title</title>是定义在网页上小标题，是SEO所搜索引擎优化的关键词
</head>
<body>

</body>
</html>
```
## 4.常见的meta

Keywords(关键字)　keywords用来告诉搜索引擎你网页的关键字是什么
```
<meta name="keywords" content="武汉JAVA培训,武汉java培训机构,java视频下载,java视频,马士兵,马士兵java视频下载">
```
- 4.2<link>标签、<script>标签
    都是与CSS、JS相关的最常见的用途是链接样式表。
```
<link rel="stylesheet" type="text/css" href="/html/csstest.css">
<script type="text/javascript" src="/JS/jquery.min.js"></script>
``` 
>
## 5.基础标签
#### 5.1标题标签
<h1> 到 <h6> 标签可定义标题。

<h1> 定义最大的标题，<h6> 定义最小的标题。
<body>
    <h1>This is heading 1</h1>
    <h2>This is heading 2</h2>
    <h3>This is heading 3</h3>
    <h4>This is heading 4</h4>
</body>

align属性值 | 作用
---|---
left | 左对齐
right | 右对齐
center| 居中
justify | 两端对齐(需要多行文本才
```
<body>
    <h1 align="center">标题</h1>
</body>
```
#### 5.2段落标签
```
<body>
    <p>我是一个段落</p>（也可使用align）
</body>
```
#### 5.3诸多格式标签
        <b>文本加粗
        <del>文本横线描述错误
        <em>斜体，给SEO强调重要性
        <i> 加粗标签，无SEO强调作用
        <pre>会保留空格和换行(如下面代码)
```
 <pre>                            
    春眠不觉晓，
      处处闻啼鸟。
        夜来风雨声，
          花落知多少。
    </pre>
```
        <strong>强调SEO重要性加粗
        <u>字体下面下划线
        <sup> 标签和<sub> 标签数学平方和下方描述
```
<body>
    <!--(a-b)²=a²-2ab+b²-->如下代码就是打印平方根的
    (a-b)<sup>2</sup>=a<sup>2</sup>-2ab+b<sup>2</sup>
</body>
```
        <img>网页中插图，注意src=“地址” alt=“你下载失败”。title鼠标提示符
            width和height宽和高
- ####             <a> URL地址超链接(也可插图片)
```
<a target="_blank" href="http://www.baidu.com">百度一下</a>
```
         <br>单行换行  自闭合标签
         <hr>创建一条水平线
         <span>和<div>是CSS来应用
>
#### 5.3列表
#####      5.31 <ul>  <li>无序列表 （如下面代码）
          ul上加type("disc" 默认黑色圆点\"circle" 空心圆点\"square" 方块)属性
```
   <p>知名手机厂商:</p>
    <ul>
        <li>华为</li>
        <li>小米</li>
        <li>三星</li>
        <li>苹果</li>
    </ul>
```
#####     5.32有序列表<ol>  <li>使用数字进行标记，有序列表是有顺序的。
              ol可加type="A" type="a"罗马字母列表 type="I" type="i"  自动升幂 
```
 <ol>
        <li>三星</li>
        <li>苹果</li>
        <li>华为</li>
        <li>小米</li>
    </ol>

```
#####    5.33表格标签
    <table>注意单行如下面代码
```
border="1" align="center" cellpadding="0" cellspacing="0"
```
 #####    5.34表格的表头
    <th>SEO重要，在表格中显示粗体
  #####   5.35<caption>表格的标题
```
 <caption>优秀男演员代表作</caption>
 ```
#####  5.35表格跨行跨列
- colspan跨列（合并列表格）
```
<th colspan="2">手机号</th>
````
##### 5.36rowspan属性实现跨行-（合并行表格）
```
<th rowspan="2">手机号</th>
```
![](http://note.youdao.com/noteshare?id=afa2c3dc3ffe87776a7908f92e2138b9)
![image](http://note.youdao.com/favicon.ico)
>
---
## 5.4表单标签
[](https://pan.baidu.com/s/1eSjFLoI#list/path=%2F)

---
#### 5.41表单标签
    表单使用<form> 标签创建。表单可包含文本字段、复选框、单选框、提交按钮等等。如登录页面等
```
<form action="login.jsp">
```

###### 表单属性
    使用<form> 标签创建。表单可包含文本字段、复选框、单选框、提交按钮等等。
ction="URL"：一个URL地址，指定form表单向何处发送数据。

name="login"：作用是给表单起名，为了便于我们操作。

enctype ="string"：规定在发送表单数据之前，如何对表单数据进行编码。通常在使用文件上传时，我们会enctype="multipart/form-data"，以二进制传输。

method ="get/post"：指定表单以何种方式发送到指定的服务器程序，该属性定义浏览器将表单中的数据提交给服务器处理程序的方式。关于method的取值，最常用的是get和post。


#### 5.42表单域
###### <input>标签
```
<form action="login.jsp">
    性别：男 <input name="sex" checked="checked" type="radio" value="1">
         女 <input name="sex" type="radio" value="2">
 </form>
 ````
 
#### 5.43表单按钮
        input="text" 文本框
        input="password" 密码框
        type="radio" 单选框
        type="checkox" 复选框
        type="file" 文件上传

