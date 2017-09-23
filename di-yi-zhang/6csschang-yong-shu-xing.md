#6.CSS常用的属性
> * CSS常见属性如下面三类

![](/assets/CSSchangyongshuxingg.png)
***
##6.1背景属性
> * 背景属性如下面5类

![](/assets/beijingshuxing.png)

###6.1.1background-color 设置元素背景色
```
<style>
    /* 给.box的背景色设置为红色 */
    .box {
        background-color: red;
    }
</style>
```
> * 使用 background-color 属性为元素设置背景色，其默认值是 transparent 也就是“透明”的意思，可使用颜色名称、RGB、RGBA、十六进制数来指定颜色(例如#ffff等)。

##6.1.2background-image背景图片


```
.box {
    background-image: url("img/bg.jpg");
}

```
> * 其默认值是 none，表示背景上没有放置任何图像。

>如果需要设置一个背景图像，必须为这个属性设置一个 URL 值。

##6.1.3background-repeat背景图片




