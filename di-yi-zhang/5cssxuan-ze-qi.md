# 5 CSS选择器

> **\*关系选择器结构组成如下图**  
> ![](/assets/Css xuazn.png)
>
> ---
>
> ## 5.1基础选择器
>
> **\*基础选择器结构组成如下图**  
> ![](/assets/basic select.png)
>
> ### 5.1.1标签选择器
>
> ```js
> html { background-color: yellow; }
> h1 { color: blue; }
> h2 { color: red; }
> ```
>
> * 如上图标签选择器详解如上图
>
> ### 5.1.2class选择器

```js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS层叠样式表</title>
    <style>
        .tag {
            color: blue;
        }
    </style>
</head>
<body>
    <h1 class="tag">我是标题</h1>
    <div class="tag">我是一个div</div>
</body>
</html>
```

> * 如上图class选择器详解如上图

---

> ### 5.1.3 ID选择器

![](/assets/guanxi.png)

```js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        #title {
            color: blue;
        }
        #block {
            /*文字居中*/
            text-align: center;
            color: red;
        }
    </style>
</head>
<body>
    <h1 id="title">我是标题</h1>
    <div id="block">我是一个div</div>
</body>
</html>
```

> * 注意：id与类选择器的概念相似，只是ID选择器只能被引用一次，而类选择器可以被多次引用。
>
> ---

![](/assets/shuxing.png)

---



