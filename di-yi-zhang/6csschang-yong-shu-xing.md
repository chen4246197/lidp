# 6.CSS常用的属性

> * CSS常见属性如下面三类

![](/assets/CSSchangyongshuxingg.png)

---

## 6.1背景属性

> * 背景属性如下面5类

![](/assets/beijingshuxing.png)

### 6.1.1 background-color 设置元素背景色

```
<style>
    /* 给.box的背景色设置为红色 */
    .box {
        background-color: red;
    }
</style>
```

> * 使用 background-color 属性为元素设置背景色，其默认值是 transparent 也就是“透明”的意思，可使用颜色名称、RGB、RGBA、十六进制数来指定颜色\(例如\#ffff等\)。

## 6.1.2 background-image背景图片

```
.box {
    background-image: url("img/bg.jpg");
}
```

> * 其默认值是 none，表示背景上没有放置任何图像。
>
> 如果需要设置一个背景图像，必须为这个属性设置一个 URL 值。

## 6.1.3 background-repeat背景图片是否重复

```
.box {
    background-image: url("img/11.jpg");
    /* 设置图片不重复平铺 */
    background-repeat: no-repeat;
}
```

> * 使用 background-repeat 属性设置背景图片是否重复。
>
> repeat 重复（默认值）
>
> repeat-x 图片在横向上平铺
>
> repeat-y 图片在纵向上平铺
>
> no-repeat 不重复平铺

## 6.1.4 background-position背景位置

```
.box {
    background-image: url("img/link.jpg");
    background-repeat: no-repeat;
    /*距离左侧200px 顶部100px*/
    background-position: 200px 100px;
    /*居中对齐*/
    background-position: 50% 50%;
    /*左下角对齐*/
    background-position: left bottom;
}
```

> * 可以使用长度值，如 100px，最后也可以使用百分数值。
>
> 可以使用一些关键字：top、bottom、left、right 和 center，不能超过两个关键字，一个对应水平方向，另一个对 应垂直方向。

## 6.1.5 background-attachment背景关联

```
.box {
    background-image: url("img/link.jpg");
    background-repeat: no-repeat;
    background-position: center center;
    /* 无论滚动条如何滚动，图片都在标签的最中心 */
    background-attachment: fixed;
}
```

> * 如果文档比较长，那么当文档向下滚动时，背景图像也会随之滚动。当文档滚动到超过图像的位置时，图像就会消》&gt; 失，可以通过 background-attachment 属性防止这种滚动。
>   通过这个属性，可以声明图像相对于可视区是固定的（fixed），因此不会受到滚动的影响

## 6.2文本属性

![](/assets/wenbenshuxing.png)

> * **CSS 文本属性**可定义文本的外观。
>
> 通过文本属性，您可以改变文本的颜色、字符间距，对齐文本，装饰文本，对文本进行缩进，等等。

### 6.2.1 color文本的颜色

> * 可使用颜色名称、RGB、RGBA、十六进制数来指定颜色。

### 6.2.2 opacity透明度

> * opacity用来设置透明度，默认值为1，1为不透明，0为完全透明。
>
> `p{ opacity: 0;}` 隐藏一个元素 ，完全不显示，但是会占空间，只是看不到。

### 6.2.3 font字体设置
> 
| font属性名 | 说明 | 参数说明 |
| :---: | :---: | :---: |
| font-family | 字体名称 |例如：Arial，"微软雅黑"，"宋体" |
| font-size | 字体大小 | 例如：18px，2em |
| font-style | 字体风格 | normal(缺省)，italic, oblique|
| font-weight | 字体粗细 | normal(缺省)，bold或数值。 |


```
.title {
    /* 设置字体名字 */
    font-family: "宋体", "微软雅黑", Arial;
    /* 设置字体大小 */
    font-size: 2em;
    /* 设置字体粗细 */
    font-weight: 900;
    /* 设置字体风格 */
    font-style: italic;
}
```
### 6.2.4 text-align字体对齐
> * 文本对齐属性text-align 属性规定元素中的文本的水平对齐方式，只能设置块级元素内文本的水平对齐> 方式。
> 
| text-align选项值 | 描述 |
| :---: | :---: | 
| left | 把文本排列到左边。默认值：由浏览器决定。 |
| right | 把文本排列到右边。 |
| center | 把文本排列到中间 | 
| justify | 实现两端对齐效果 | 

### 6.2.5 text-decoration字体修饰

| text-decoration选项值 | 描述 |
| :---: | :---: | 
| none | **把文本排列到左边。默认值：由浏览器决定。** |
| underline | 定义文本下的一条线。 |
| overline | 定义文本上的一条线。 | 
| line-through |定义穿过文本下的一条线。 | 

> * 实例：去掉a标签的底部线条

```
a {
    text-decoration: none;
}

```

### 6.2.6 text-decoration字间距
> * 设置字与字之间的间距。


```
.title {
     letter-spacing: 10px;
}
```

### 6.2.7 line-height行高


```
.title {
     line-height: 80px;
     text-align: center;
}
```

> * line-height 属性设置行间的距离（行高），属性值可以为数值也可以为百分比。

> line-height妙用：设置文字居上下中展示

### 6.2.8 扩展

```
.title {
     width: 5em;
     height: 1.4em;
     /*设置文本超出文本框时隐藏文本*/
     overflow:hidden;
     /*用略符号来代表被修剪的文本*/
     text-overflow:ellipsis;
     /*设置文本会能换行*/
     white-space:nowrap;
}
```
> * 实现溢出文本eclipsis的解决，让溢出的文字以省略号显示。


### 6.3 列表属性
![](/assets/liebiaoyangshi.png)
> * 列表属性主要针对的是表单（**ul和ol**）类型的列表。

####6.3.1 list-style-type **?**


```
ul{ list-style-type:circle;}
```
> 
 * **list-style-type**
列表样式，类型属性值可以为：
disc (缺省值，黑圆点)
circle (空心圆点) square (小黑方块)
decimal (数字排序)
lower-roman upper-roman 罗马数字
lower-alpha upper-alpha 英文字母
none (无列表项标记)

####6.3.2 list-style-position **?**
> * 设置列表样式位置属性，这个属性有两个值outside和inside

> outside项目符号放在文本以外（默认）

```
ul li{ list-style-position:outside; width:100px; border:1px solid red;}
```
> inside项目符号放在文本以内

```
ul li{ list-style-position:inside; width:100px; border:1px solid red;}
```

#### 6.3.3 list-style-image
> * 列表样式图片属性，只有一个属性url，引导一个图片。


```
ul { list-style-image: url("images/icon.png"); }
```
























