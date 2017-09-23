#6.CSS常用的属性
> * CSS常见属性如下面三类

![](/assets/CSSchangyongshuxingg.png)
***
##6.1背景属性
> * 背景属性如下面5类

![](/assets/beijingshuxing.png)

###6.1.1 background-color 设置元素背景色
```
<style>
    /* 给.box的背景色设置为红色 */
    .box {
        background-color: red;
    }
</style>
```
> * 使用 background-color 属性为元素设置背景色，其默认值是 transparent 也就是“透明”的意思，可使用颜色名称、RGB、RGBA、十六进制数来指定颜色(例如#ffff等)。

##6.1.2 background-image背景图片


```
.box {
    background-image: url("img/bg.jpg");
}

```
> * 其默认值是 none，表示背景上没有放置任何图像。

>如果需要设置一个背景图像，必须为这个属性设置一个 URL 值。

##6.1.3 background-repeat背景图片是否重复


```
.box {
    background-image: url("img/11.jpg");
    /* 设置图片不重复平铺 */
    background-repeat: no-repeat;
}

```
> * 使用 background-repeat 属性设置背景图片是否重复。

>repeat 重复（默认值）

>repeat-x 图片在横向上平铺

>repeat-y 图片在纵向上平铺

>no-repeat 不重复平铺


##6.1.4 background-position背景位置


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

> 可以使用一些关键字：top、bottom、left、right 和 center，不能超过两个关键字，一个对应水平方向，另一个对 应垂直方向。

##6.1.5 background-attachment背景关联


```
.box {
    background-image: url("img/link.jpg");
    background-repeat: no-repeat;
    background-position: center center;
    /* 无论滚动条如何滚动，图片都在标签的最中心 */
    background-attachment: fixed;
}
```
> * 如果文档比较长，那么当文档向下滚动时，背景图像也会随之滚动。当文档滚动到超过图像的位置时，图像就会消》> 失，可以通过 background-attachment 属性防止这种滚动。
> 通过这个属性，可以声明图像相对于可视区是固定的（fixed），因此不会受到滚动的影响












