# HTML 速查列表
***
HTML 速查列表. 你可以打印它，以备日常使用。
***
## HTML 基本文档
```
<!DOCTYPE html>
<html>
<head>
<title>文档标题</title>
</head>
<body> 可见文本... </body>
</html>
```
## 基本标签（Basic Tags）

```
<h1>最大的标题</h1>
 <h2> . . . </h2>
 <h3> . . . </h3>
 <h4> . . . </h4>
 <h5> . . . </h5>
 <h6>最小的标题</h6>
 ````
 ```
 <p>这是一个段落。</p>
 <br> （换行）
 <hr> （水平线）
 <!-- 这是注释 -->
 ```


### 文本格式化（Formatting）

```
<b>粗体文本</b>
 <code>计算机代码</code>
 <em>强调文本</em>
 <i>斜体文本</i>
 <kbd>键盘输入</kbd> 
 <pre>预格式化文本</pre>
 <small>更小的文本</small>
 <strong>重要的文本</strong>
 
 <abbr> （缩写）
 <address> （联系信息）
 <bdo> （文字方向）
 <blockquote> （从另一个源引用的部分）
 <cite> （工作的名称）
 <del> （删除的文本）
 <ins> （插入的文本）
 <sub> （下标文本）
 <sup> （上标文本）
 ```
## 链接（Links）
```
普通的链接：<a href="链接地址">链接文本</a>
图像链接： <a href="http://www.example.com/"><img src="URL" alt="替换文本"></a> 
邮件链接： <a href="mailto:webmaster@example.com">发送e-mail</a>
书签： <a id="tips">
提示部分</a> <a href="#tips">跳到提示部分</a>
```
## 图片（Images）
```
<img src="URL" alt="替换文本" height="42" width="42">
```
## 样式/区块（Styles/Sections）
```
<style type="text/css">
   h1 {color:red;}
   p {color:blue;}
 </style>
 <div>文档中的块级元素</div>
 <span>文档中的内联元素</span>
 ```
## 无序列表
```
<ul>
   <li>项目</li>
   <li>项目</li>
 </ul>
 ```
## 有序列表
```
<ol>
   <li>第一项</li>
   <li>第二项</li>
 </ol>
 ```
## 定义列表
```
<dl>
   <dt>项目 1</dt>
     <dd>描述项目 1</dd>
   <dt>项目 2</dt>
     <dd>描述项目 2</dd>
 </dl>
 ```
## 表格（Tables）
```
<table border="1">
   <tr>
     <th>表格标题</th>
     <th>表格标题</th>
   </tr>
   <tr>
     <td>表格数据</td>
     <td>表格数据</td>
   </tr>
 </table>
 ```
 ***
 # *下面连接作品图片
 ![](/assets/0922日作业.png)
 # *下面连接作品代码
 
 ```
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>用户注册界面</title>
</head>
<body>
<table border="1px" align="left" cellspacing="2" cellpadding="2">
    <h1 height="80" align="left"><b>用户注册界面</b></h1>
    <tr height="35px" align="center">
        <td width="100px" ><b>用户名</b></td>
        <td width="450px" align="left"><label for="username" ></label>
            <input type="text"  placeholder="请输入用户名" id="username" ></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>密码</b></td>
        <td align="left"><label for="password"></label>
            <input type="password" id="password" placeholder="请输入密码"></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>确认密码</b></td>
        <td align="left"><label for="password"></label>
            <input type="password" id="password" placeholder="请重新输入密码"></td</td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>电子邮箱</b></td>
        <td align="left"><label for="password"></label>
            <input type="password" id="password" ></td</td></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>网络昵称</b></td>
        <td align="left"><label for="password"></label>
            <input type="password" id="password" ></td</td></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>性别</b></td>
        <td align="left"><label for="nan">男</label>
            <input type="radio" name="sex" checked id="nan">
            <label for="nv">女</label>
            <input type="radio" name="sex"  id="nv">
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>是否有房</b></td>
        <td align="left"><label for="nan">有</label>
            <input type="radio" name="you" checked id="you">
            <label for="nv">没有</label>
            <input type="radio" name="you"  id="wu"></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>爱好</b></td>
        <td align="left">
            <input type="checkbox" name="柳岩">
            <label for="lyf">范冰冰</label>
            <input type="checkbox" name="angle"  id="ltx">
            <label for="ltx">刘亦菲</label>
            <input type="checkbox" name="nice" id="dmv" >
            <label for="dmv">柳岩</label>
            <input type="checkbox" name="woke" checked id="wh" >
            <label for="wh">佟丽娅红</label>
            <input type="checkbox" name="woke" id="fh" >
        <label for="fh">郭德纲</label></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>户籍</b></td>
        <td align="left"><select name="请选择" id="1" >
            <option value="">--请选择--</option>
        </select></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>课程</b></td>
        <td align="left"><select name="我最喜欢的女明星"  multiple>
            <option value="刘亦菲" selected>计算机体系结构</option>
            <option value="angle">编程语言</option>
            <option value="刘天仙">C++</option>
            <option value="大美女">汇编语言</option>
        </select><br></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>头像</b></td>
        <td align="left"> <input type="file" multiple placeholder="选择文件"></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>个人介绍</b></td>
        <td align="left"><textarea name="我的自我介绍" id="" cols="30" rows="5">
我是textarea的默认值。
    </textarea></td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>验证码</b></td>
        <td align="left"><label for="hhh" ></label>
            <input type="text"  placeholder="请输入验证码"  >8888</td>
    </tr>
    <tr height="35px" align="center">
        <td width="100px"><b>按钮</b></td>
        <td align="left"><input type="submit" value="点我啊！"></td>
    </tr>
    <tr height="30px" align="center" >
        <td colspan="2"   > <input type="checkbox" name="柳岩" checked >
            <label for="lyf" ><b>是否阅读并同意本协议</b></label></td>
    </tr>
    <tr height="35px" align="center">
        <td colspan="2"><img src="img/huawei.jpg" alt="" width="70"></td>
    </tr>
    <tr height="35px" align="center">
        <td align="center" colspan="2"><input type="submit" value="注册新用户">
            &#160<input type="submit" value="重置注册信息"></td>
    </tr>

</table>

</body>
</html>
 ```
 ***
## 框架（Iframe）
```
<iframe src="demo_iframe.htm"></iframe>
```
## 表单（Forms）
```
<form action="demo_form.php" method="post/get">

<input type="text" name="email" size="40" maxlength="50"> 
<input type="password"> 
<input type="checkbox" checked="checked"> 
<input type="radio" checked="checked"> 
<input type="submit" value="Send"> 
<input type="reset"> 
<input type="hidden"> 

<select> 
<option>苹果</option> 
<option selected="selected">香蕉</option> 
<option>樱桃</option> 
</select>

<textarea name="comment" rows="60" cols="20">
</textarea> 
</form>
```
## 实体（Entities）
```
&lt; 等同于 <
 &gt; 等同于 >
&copy; 等同于 ©
```