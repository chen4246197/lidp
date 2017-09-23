# 4.CSS

## 4.1CSS语法基础：层叠样式表Cascading Style Sheet

> 为了提升html编辑的拓展功能，**了更好的渲染HTML元素而引入的**,讲页面内容与形式（标签属性）进行拓展分离，丰富Html表格、各种功能而做的拓展.  
> 就像面向对象思想一样，将他的标签的内容单独封装起来进行拓展，通过`<link>`标签进行接口连接。
>
> * **网页标准化设计的趋势**使css得到更广泛浏览器厂商的支持。
> * **网页现在的新标准是W3C**目前的模式是html+css+javascript即如下图
> * _html是网页的结构_ 就是盖房子先要把结构建出来
> * _CSS是网页的样式_ CSS来装饰
> * _javascript是行为_最后精装修 
>
> ![](/assets/css主要组成.png)

## 4.2 **CSS代码的结构：**

> \*每条声明由一个属性和一个值组成，属性和值用冒号（“ : ”）分开，多条声明用分号（“ ; ”）分开

![](/assets/css_selector.gif)

## 4.3引入样式方式

![](/assets/yinru.png)

> ### 4.3.1行内样式（内联样式）
>
> ```js
>  <p style="color:blue;margin-left:20px;">This is a paragraph.</p>
> ```
>
> 如上图显示出如何改变**段落的颜色**和**左外边距**

### 4.3.2 内部样式（嵌入式）

```js
<style>
    body {
        /*设置背景颜色*/
        background-color: yellow;
    }

    h1 {
        /*设置字体颜色*/
        color: blue;
        /*设置字体大小*/
        font-size: 30px;
    }
</style>
```

> * 如上图**HTML文档头部定义多个style元素，实现多个样式表**

### 4.3.3外部样式（外链式）

```js
index{
style="color:blue;margin-left:20px;
}
```

```js
<head>
    <meta charset="UTF-8">
    <title>CSS层叠样式表</title>
    /*引入外部的层叠样式表，href指向的是需要加载样式表的.css文件*/
    <link rel="stylesheet" href="css/index.css">
</head>
```

> * 作用如下
>   * **对于较大规模的网站**将CSS样式定义独立成一个一个的文档，可有效地提高效率，并有利于对网站风格的维护。
>   * 而无需更改HTML文档，可以改变样式表。
>   * 可以根据介质有选择的加载样式表。

## 4.4优先级
***
![](/assets/youxianji2.png)
***
![](/assets/youxianji.png)

> * 如上图总结：**谁离body得近，谁优先级高！**
* 有个例外的情况，就是如果外部样式放在内部样式的后面，则外部样式将覆盖内部样式.
> * 同一组属性设置中标有**“!important”**规则的优先级最大；示例如下：
>
> ```js
> <html>
>   <head>
>     <style type="text/css">
>      #redP p{
>         /*两个color属性在同一组*/
>         color:#00f !important; /* 优先级最大 */
>         color:#f00;
>      }
>     </style>
>   </head>
>   <body>
>      <div id="redP">
>        <p>color</p>
>        <p>color</p>
>      </div>
>   </body>
> </html>
> ```



