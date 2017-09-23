# 3.文本结构和语法

## 3.1文档结构

```js
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
`
```

## 3.2重要标签属性

### meta:

* Keywords\(关键字\)　keywords用来告诉搜索引擎你网页的关键字是什么

  > `<meta name="keywords" content="武汉JAVA培训,武汉java培训机构,java视频下载,java视频,马士兵,马士兵java视频下载">`
  >
  > ### link标签、script标签
  >
  > * 都是与CSS、JS相关的最常见的用途是链接样式表。

## 3.3基础标题标签

> `<h1>`标签和`<h6>`可定义标题。  
> `<h1>` 定义最大的标题，`<h6>` 定义最小的标题。

```&amp;lt;body&amp;gt;
    <h1>This is heading 1</h1>
    <h2>This is heading 2</h2>
    <h3>This is heading 3</h3>
    <h4>This is heading 4</h4>
</body>
```

| 属性值 | 作用 |
| :--- | :---: |
| left | 左对齐 |
| right | 右对齐 |
| center | 居中对齐 |
| justify | 两端对齐\(需要多行文本才可以看出效果\) |

> 使用align属性让标题居中：
>
> ```
> <body>
>     <h1 align="center">标题</h1>
> </body>
> ```

## 3.4段落标签

> * `<p>`标签定义段落。align是通用属性，块元素都可以使用

```
<body>
    <p>我是一个段落</p>
</body>
```

## 3.5诸多格式标签

> `<b>`文本加粗  
>         `<del>`文本横线描述错误  
>         `<em>`斜体，给SEO强调重要性  
>         `<i>`加粗标签，无SEO强调作用  
>         `<pre>`会保留空格和换行\(如下面代码\)  
>          `<strong>`强调SEO重要性加粗  
>         `<u>`字体下面下划线  
>         `<sup>` 标签和`<sub>` 标签数学平方和下方描述  
>         `<img>`插入图片注意src=“地址” alt=“你下载失败”。title鼠标提示符  
>         width和height宽和高  
>         `<hr>` 标签分割线

```
<body>
    <!--(a-b)²=a²-2ab+b²-->如下代码就是打印平方根的
    (a-b)<sup>2</sup>=a<sup>2</sup>-2ab+b<sup>2</sup>
</body>
```

* `<a>` 标签

  > 可连接URL地址超链接\(也可插图片\)
  >
  > ```
  > 普通的链接：<a href="链接地址">链接文本</a>
  > 图像链接： <a href="http://www.example.com/"><img src="URL" alt="替换文本"></a> 
  > 邮件链接： <a href="mailto:webmaster@example.com">发送e-mail</a>
  > 书签： <a id="tips">
  > 提示部分</a> <a href="#tips">跳到提示部分</a>
  > ```

* `<br>` 标签和`<hr>`标签,如下图

  ```
  <body>
    <span>这是span标签</span><br>
    这不是span标签
  </body>
  ```

  ```&amp;lt;body&amp;gt;
    <p>
    春眠不觉晓，<br/>
      处处闻啼鸟。<br/>
        夜来风雨声，<br/>
          花落知多少。<br/>
    </p>
  </body>
  ```

  ## 3.6 CSS用`<div>`标签和`<span>`标签

  > `<div>`_标签  
  > _`<sapn>`标签



