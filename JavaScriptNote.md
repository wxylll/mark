在标签中填写 onclick 事件调用函数时，不是 onclick=函数名， 而是 onclick=函数名+()<br>
外部 javascript 文件不使用 <script> 标签，直接写 javascript 代码。<br>
HTML 输出流中使用 document.write，相当于添加在原有html代码中添加一串html代码。而如果在文档加载后使用（如使用函数），会覆盖整个文档。<br>

JavaScript 可以通过不同的方式来输出数据：<br>
使用 <b>window.alert()</b> 弹出警告框。<br>
使用 <b>document.write()</b> 方法将内容写到 HTML 文档中。<br>
使用 <b>innerHTML</b> 写入到 HTML 元素。<br>
使用 <b>console.log()</b> 写入到浏览器的控制台。


<b>document.getElementById("demo") </b>是使用 id 属性来查找 HTML 元素的 JavaScript 代码 。

<b>innerHTML = "段落已修改。" </b>是用于修改元素的 HTML 内容(innerHTML)的 JavaScript 代码。


var 关键字告诉浏览器创建一个新的变量：

JavaScript 关键字必须以<b>字母、下划线（_）或美元符（$）开始。</b>

后续的字符可以是字母、数字、下划线或美元符（数字是不允许作为首字符出现的，以便 JavaScript 可以轻易区分开关键字和数字）。


以下是JavaScript中最重要的保留字
<table>
<tr>
    <td>abstract</td>
    <td>else</td>
    <td>instanceof</td>
    <td>super</td>
</tr>
<tr>
    <td>boolean</td>
    <td>enum</td>
    <td>int</td>
    <td>switch</td>
</tr>
<tr>
    <td>break</td>
    <td>export</td>
    <td>interface</td>
    <td>synchronized</td>
</tr>
<tr>
    <td>byte</td>
    <td>extends</td>
    <td>let</td>
    <td>this</td>
</tr>
<tr>
    <td>case</td>
    <td>false</td>
    <td>long</td>
    <td>throw</td>
</tr>
<tr>
    <td>catch</td>
    <td>final</td>
    <td>native</td>
    <td>throws</td>
</tr>
<tr>
    <td>char</td>
    <td>finally</td>
    <td>new</td>
    <td>transient</td>
</tr>
<tr>
    <td>class</td>
    <td>float</td>
    <td>null</td>
    <td>true</td>
</tr>
<tr>
    <td>const</td>
    <td>for</td>
    <td>package</td>
    <td>try</td>
</tr>
<tr>
    <td>continue</td>
    <td>function</td>
    <td>private</td>
    <td>typeof</td>
</tr>
<tr>
    <td>debugger</td>
    <td>goto</td>
    <td>protected</td>
    <td>var</td>
</tr>
<tr>
    <td>default</td>
    <td>if</td>
    <td>public</td>
    <td>void</td>
</tr>
<tr>
    <td>delete</td>
    <td>implements</td>
    <td>return</td>
    <td>volatile</td>
</tr>
<tr>
    <td>do</td>
    <td>import</td>
    <td>short</td>
    <td>while</td>
</tr>
<tr>
    <td>double</td>
    <td>in</td>
    <td>static</td>
    <td>with</td>
</tr>
</table>

JavaScript对于大小写是敏感的<br>
编写JavaScript语句的时候，需要留意是否关闭了大小写切换<br>

JavaScript的语句标识符：<br>
<table>
<tr>
    <td>语句</td>
    <td>描述</td>
</tr>
<tr>
    <td>break</td>
    <td>用于跳出循环</td>
</tr>
<tr>
    <td>catch</td>
    <td>语句块，在try语句块执行出错时继续执行该语句块。</td>
</tr>
<tr>
    <td>continue</td>
    <td>跳过循环中的一个迭代</td>
</tr>
<tr>
    <td>do...while</td>
    <td>执行一个语句块，在条件语句为true时继续执行该语句块</td>
</tr>
<tr>
    <td>for</td>
    <td>在条件语句为true时，可以将代码块执行指定的次数</td>
</tr>
<tr>
    <td>function</td>
    <td>定义一个函数</td>
</tr>
<tr>
    <td>if...else</td>
    <td>用于基于不同的条件来执行不同的动作</td>
</tr>
<tr>
    <td>return</td>
    <td>退出函数</td>
</tr>
<tr>
    <td>switch</td>
    <td>用于基于不同的条件来执行不同的动作</td>
</tr>
<tr>
    <td>throw</td>
    <td>抛出（生成）错误</td>
</tr>
<tr>
    <td>try</td>
    <td>实现错误处理，与catch一起使用</td>
</tr>
<tr>
    <td>var</td>
    <td>声明一个变量</td>
</tr>
<tr>
    <td>while</td>
    <td>当条件语句为true时，执行语句块</td>
</tr>
</table>

JavaScript会忽略多余的空格<br>
可以在文本字符串中使用反斜杠对代码行进行换行。<br>
<code>document.write("你好 \
世界!");<code>

不能像这样折行：

<code>document.write \ 
("你好世界!");</code>
<br>

JavaScript不会执行注释。<br>
注：
<u>HTML注释符号是以 <-- 开始以 --> 结束的。如果在此注释符号内编写 JavaScript脚本，对于不支持 JavaScript 的浏览器，将会把编写的 JavaScript 脚本作为注释处理。</u>

声明新变量时，可以使用关键词 "new" 来声明其类型：<br>
<code>
var carname=new String;<br>
var x=      new Number;<br>
var y=      new Boolean;<br>
var cars=   new Array;<br>
var person= new Object;
</code>

JavaScript 变量的生命期从它们被声明的时间开始。

局部变量会在函数运行以后被删除。

全局变量会在页面关闭后被删除


字符串方法：
<table>
<tr>
    <td>charAt()</td>
    <td>返回指定索引位置</td>
</tr>
<tr>
    <td>charCodeAt()</td>
    <td>返回指定索引位置字符的unicode值</td>
</tr>
<tr>
    <td>concat()</td>
    <td>连接两个或多个字符串，返回连接后的字符串</td>
</tr>
<tr>
    <td>fromCharCode()</td>
    <td>将Unicode转换为字符串</td>
</tr>
<tr>
    <td>indexOf()</td>
    <td>返回字符串中检索指定字符第一次出现的位置</td>
</tr>
<tr>
    <td>localeCompare()</td>
    <td>用本地的特定顺序来比较两个字符串</td>
</tr>
<tr>
    <td>match()</td>
    <td>找到一个或多个正则表达式的匹配
</tr>
<tr>
    <td>replace()</td>
    <td>替换与正则表达式匹配的字符串</td>
</tr>
<tr>
    <td>search()</td>
    <td>检索与正则表达式匹配的字符串</td>
</tr>
<tr>
    <td>slice()</td>
    <td>提取字符串的片段，并在新的字符串中返回被提取的部分</td>
</tr>
<tr>
    <td>split()</td>
    <td>把字符串分割为子字符串数组</td>
</tr>
<tr>
    <td>substr()</td>
    <td>从起始索引号提取字符串中指定数目的字符</td>
</tr>
<tr>
    <td>sunstring()</td>
    <td>提取字符串中两个指定的索引号之间的字符</td>
</tr>
<tr>
    <td>toLocalLowerCase()</td>
    <td>根据主机的语言环境把字符串转换为小写</td>
</tr>
<tr>
    <td>toLocalUpperCase()</td>
    <td>根据主机的语言环境把字符串转换为大写</td>
</tr>
<tr>
    <td>toString()</td>
    <td>返回字符串对象值</td>
</tr>
<tr>
    <td>trim()</td>
    <td>移除字符串首尾空白</td>
</tr>
<tr>
    <td>valueOf()</td>
    <td>返回某个字符串对象的原始值</td>
</tr>
</table>

反正java里也都学过了，就当打一遍复习了

JavaScript中，变量可以先使用后声明
<br>
JavaScript中，函数及变量的声明都将被提升到函数的<b>最顶部</b>。
<br>
且函数声明总是会被解释器“悄悄的”提升到方法体的最顶部。
<br>
JavaScript只有声明的变量会提升，初始化的不会。
<br>
为了避免这些问题，通常我们在每个作用于开始前声明这些变量，这是正常的JavaScript解析步骤
<br>


##### 严格模式的限制

1.不允许使用未声明的变量
<br>
2.不允许删除变量或对象。
<br>
3.不允许删除函数
<br>
4.不允许变量重名。
<br>
5.不允许使用八进制。
<br>
6.不允许使用转义字符。
<br>
7.不允许对只读属性赋值。
<br>
8.不允许对一个使用getter方法读取的属性进行赋值。
<br>
9.不允许删除一个不允许删除的属性。
<br>
10.变量名不能使用“eval”字符串。
<br>
11.变量名不能使用“argumens”字符串.
<br>
12.不允许使用以下这种语句：
<code><br>
"use strict";<br>
with (Math){x = cos(2)}; // 报错
</code>
<br>


由于一些安全原因，在作用域eval()创建的变量不能被调用。
<br>
禁止this关键字指向全局变量。
<br>


##### 保留关键字
为了向将来JavaScript的新版本过渡，严格模式新增了一些保留关键字：

implements <br>
interface <br>
let <br>
package <br>
private <br>
protected <br>
public <br>
static <br>
yield <br>


**比较运算符常见错误：**

在常规的比较中，数据类型是被忽略的
<br>
<code>
var x = 10;<br>
var y = "10";<br>
if (x == y)
</code>
<br>
在严格的比较运算中，===为恒等运算符，同时检查表达式的值与类型。

##### 字符串分行：

JavaScript中允许我们在字符串中使用断行语句，但是在字符串中直接使用回车换行会报错。在字符串断行需要使用反斜杠。


##### JavaScript表单

HTML表单验证可以通过JavaScript表单来完成。
<br>

