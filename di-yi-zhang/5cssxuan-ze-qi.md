# 5 CSS选择器

**\*关系选择器结构组成如下图**  
![](/assets/Css xuazn.png)

---

## 5.1基础选择器

**\*基础选择器结构组成如下图**  
 ![](/assets/basic select.png)

### 5.1.1标签选择器

> ```js
> html { background-color: yellow; }
> h1 { color: blue; }
> h2 { color: red; }
> ```
>
> * 如上图标签选择器详解如上图

### 5.1.2class选择器

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

### 5.1.3 ID选择器

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

### 5.1.4 通配符选择器

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        * {
            color: red;
        }
    </style>
</head>
<body>
    <h1>我是标题</h1>
    <div>我是一个div标签</div>
    <span>我是一个span标签</span>
</body>
</html>
```

> * 如上图代码即通配符选择器

---

![](/assets/guanxi.png)

## 5.2 关系选择器

### 5.2.1交集选择器

```js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        /*选中"我是一个div标签"的这个标签*/
        div.tag {
            color: blue;
        }
        /*选中"我是一个p标签"的这个标签*/
        p#title {
            font-size: 30px;
        }
    </style>
</head>
<body>
    <h1 class="tag">我是标题</h1>
    <div class="tag">我是一个div标签</div>
    <p id="title">我是一个p标签</p>
</body>
```
> * 交集选择器代码如上图，详解如上图

### 5.2.2并集选择器

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        /*选中符合条件的所有标签*/
        .search, span, #Important {
            color: red;
        }
    </style>
</head>
<body>
    <a class="search" href="#">百度一下</a>
    <h1>我是一个h1标签</h1>
    <span>我是一个span标签</span>
    <div>
        <p>我是一个p标签</p>
        <span>我是一个span标签</span>
        <strong id="Important">我是一个强调标签</strong>
    </div>
    <p>我是一个p标签</p>
</body>
</html>

```
> * 并集选择器代码如上图，详解如上图

### 5.2.3后代选择器


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        /*选中所有div标签中存在的span标签*/
        div span {
            color: red;
        }
    </style>
</head>
<body>
    <div>
        <h1>我是一个h1标签</h1>
        <span>我是一个span标签</span>
        <div>
            <p>我是一个p标签</p>
            <span>我是一个span标签</span>
            <strong>我是一个强调标签</strong>
        </div>
        <p>我是一个p标签</p>
    </div>
</body>
</html>
```
> * 后代选择器代码如上图，详解如上图

### 5.2.4子选择器


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        .tag > span {
            color: red;
        }
    </style>
</head>
<body>
    <div class="tag">
        <h1>我是一个h1标签</h1>
        <span>我是一个span标签</span>
        <div>
            <p>我是一个p标签</p>
            <span>我是一个span标签</span>
            <strong>我是一个强调标签</strong>
        </div>
        <p>我是一个p标签</p>
    </div>
</body>
</html>
```
> * 子选择器代码如上图，详解如上图


---
## 5.3属性选择器





![](/assets/shuxing.png)
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        [class] {
            color: red;
        }
    </style>
</head>
<body>
    <div class="block">我是一个div标签</div>
    <p class="title">我是一个p标签</p>
</body>
</html>
```
> * E[att]选择器代码如上图，详解如上图


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        [class="title"] {
            color: red;
        }
    </style>
</head>
<body>
    <div class="block">我是一个div标签</div>
    <p class="title">我是一个p标签</p>
</body>
</html>
```
> *  E[att="val"]选择器代码如上图，详解如上图


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CSS选择器</title>
    <style>
        [class~="block1"] {
            color: red;
        }
    </style>
</head>
<body>
    <div class="block1 block2">我是一个div标签</div>
</body>
</html>
```
> *  E[att~="val"]选择器代码如上图，详解如上图










---



