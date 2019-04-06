用<h1/h1>
对HTML网页进行添加标题<br>
标题一共分六个等级<br>
字体和字号依次减小

#在字体的区别上<br>
 <em /em>表示的是对指定文字的斜体表示
而<strong /strong>表示的是对指定文字的加粗
国内的前端程序员更比较倾向于使用<strong /strong>来表示强调</br>
<span /span>没有语义，但是他的作用是为了设置单独的样式。</br>
<q></q>对其他人说的话进行引用
不是为了增加引号而使用，而是为了起加强语气的作用
引用的文本不需要添加双引号，使用该语法可以自动添加


<blackquote/blackquote>      <br>
也是引用别人的文本，但是主要是对长文本的引用。
假如需要引用大量的知名作家的文字，就需要用到<blackquote>

br / 表示对一句话的换行，在需要回车的地方加入<br />
能在HTML语言中充当word文档的回车
另外：<br>
在HTML语言中是没有空格和回车的<br>
要想实现回车和空格的作用，就必要要用到br /

&nbsp;
代表的是HTML语言中的文本空格
要想在文本中输入多个空格，就要反复在文本中使用&nbsp

使用hr能做到文本的分割线<br>
样式大致和知乎的分割线差不多<br>
为了文章看起来整齐美观

<address /address<br>
对公司的地址进行说明和强调<br>

<code /code>  <br>
介绍计算机专业的编程代码时，可以使用code进行插入<br>
注：如果使用的是多行代码，则可以使用pre标签
#
```
<div> </div>
```
用来在网页制作中独立的逻辑部分划分出来
相当于一个容器

div id=""  <br>
为独立的分区起名
<br>
```
<table> </table>
```
整个表格以其开始以其结束
```
<tbody> </tbody>
```
按结构一块一块显示

```
<tr> </tr>
```
表格的一行，有多少对<tr>就有多少行

```
<td> </td>
```
表格的一个单元格，有几对<td>就有几列

```
<th> </th>
```
表格头部的一个单元格，表格表头 <br>
默认为粗体并且居中表示  <br>

表格中列的个数取决于单元格的个数  <br>

```
<table summary="">
```
用来增加表格的可读性 <br>
能更好的读懂内容

```
<caption>
```
用来描述表格内容，在正上方的中间

使用a标签可以实现超链接  <br>
语法为：
```
    <a href="目标网址"  <br> title=“鼠标滑过显示的文本”>链接显示的文本</a>

如何在新建浏览器窗口中打开链接
```
    <a href="目标网址" target="_blank">目标文本 </a>
    
如何使用mailto在网页中链接email地址
![image](http://note.youdao.com/noteshare?id=87f7b8fcf447b877c512422a54184f65)


如何用img为网页插图片：  <br>
```
    <img src="图片地址" alt="下载失败时的替换文本" title = "提示文本">
```    
 如何实现网站与用户的交互? <br>
 使用HTML表单把浏览者的数据传到服务器端 <br>
 语法如下： <br>
 ```
    <form   method="传送方式"   action="服务器文件">
    
```

如何在表单中键入文本输入框，密码输入框 <br>
```
<form>
   <input type="text/password" name="名称" value="文本" />
</form>
```

文本域如何键入多行文本：

语法：
```
<textarea rows="行数" cols="列数">文本</textarea>
```
行数列数这两个属性可以在CSS中用height和weight代替 <br>

HTML中如何使用单选框和复选框 

语法：
```
<input   type="radio/checkbox"   value="值"    name="名称"   checked="checked"/>
```
radio表示单选框，checkbox表示多选框
checked表示默认值
当设备写为checked=“checked时”，该选项被默认选中

注：
在同一个单选目录下的两个name必须完全一致，这样才能起到单选的作用。

如何在网页中使用下拉列表框为页面节省空间

```
<select>  
    <option value="提交值" selected="selected">选项 </option>
</select>
```
提交值上传至服务器，选项用于网页平面内的选择
selected="selected"表示自动选择选项默认值

在select选项中通过设置multiple选项可以进行下拉列表框的多选
语法为：
```
<select muliple="muliple">    </select>
```
在 windows 操作系统下，进行多选时按下Ctrl键同时进行单击

如何使用提交按钮将数据上传至服务器<br>
语法：
```
<input   type="submit"   value="提交">
```
只有当type值设定为submit时，提交按钮才会起作用<br>
value是按钮上显示的文字<br>

如何使用重置按钮重置表单信息：<br>
语法：
```
<input type="reset" value="重置">
```

label标签用于改进鼠标用户的用户体验

语法：
```
<label for="控件id名称">
```
标签的for属性的值应该与相关控件的值一致
