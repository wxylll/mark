#1、在JavaScript中<h></h>里面的表示是一个标题，`<p></p>`里面表示的是一个段落

#2、js对事件的反应：
`<button type="button" onclick="alert（'欢迎！'）">点击</button>`
写完时候，就会发现运行后会出现一个点击的框，点击后会提示“欢迎！”

#3、据说还能用JavaScript插入图片呢233。（我实在是没有看懂）

#4、利用JavaScript改变HTML元素的样式

	<p id="test">
	JavaScript 能改变 HTML 元素的样式。
	</p>
	<script>
	function change(){
		x=document.getElementById("test") // 找到元素
		x.style.color="#ff0000";          // 改变样式
	}
	</script>
	<button type="button" onclick="change()">点击这里</button>
<br>这个情况就是鼠标点击“点击这里”时，将test里面的元素的颜色变成红色

#5、

	<h1>我的第一段 JavaScript</h1>
	<p>请输入数字。如果输入值不是数字，浏览器会弹出提示框。</p>
	<input id="demo" type="text">
	<script>
	function myFunction()
	{
		var x=document.getElementById("demo").value;
		if(isNaN(x)||x.replace(/(^\s*)|(\s*$)/g,"")==""){
		alert("不是数字");
		}
	}
	</script>
	<button type="button" onclick="myFunction()">点击这里</button>
这个是用JavaScript验证输入的是不是数字的一段代码（就是有点没有看懂）

#6、  
 
	<html>
	<body>
	<h1>我的 Web 页面</h1>
	<p id="demo">一个段落</p>
	<button type="button" onclick="myFunction()">尝试一下</button>
	<script>
	function myFunction()
	{
	    document.getElementById("demo").innerHTML="我的第一个 JavaScript 函数";
	}
	</script>
	</body>
	</html>
据说这段代码运行的时候能发生这样的效果：
<br>运行后会出现一个框：点击这里。
<br>点击后“一个段落”就会变成“我的第一个JavaScript函数”</br>
据说`<script>`还能再`<head>`中和外部JavaScript中输入并实现呢

#7、

	<h1>我的第一个页面</h1>
	<p>我的第一个段落。</p>
	<script>
	window.alert(5 + 6);
	</script>
`window.alert`的意思是再点开网页的时候，浏览器会出现一个提示，就是现实“11”


	<h1>我的第一个 Web 页面</h1>
	<p id="demo">我的第一个段落。</p>
	<script>
	document.getElementById("demo").innerHTML="段落已修改。";
	</script>
运行这段代码就会将“我的第一个段落”变更成“段落已修改”


	<h1>我的第一个 Web 页面</h1>
	<p>我的第一个段落。</p>
	<script>
	document.write(Date());
	</script>
运行这段代码屏幕上就会显示现在系统的时间

	<h1>我的第一个 Web 页面</h1>
	<p>我的第一个段落。</p>
	<button onclick="Datenow()">点我</button>
	<script>
	function Datenow() {
	    document.write(Date());
	}
	</script>
运行这段代并点击“点我”，屏幕上的信息就会变成现在系统的时间

	<script>
	a = 5;
	b = 6;
	c = a + b;
	console.log(c);
	</script>
运行这段代码并再浏览器中打开，摁F12，Console（控制台）中就会显示a+b的结果，就是“11”。
<br>由于JavaScript 没有任何打印或者输出的函数。 
<br>JavaScript 显示数据可以通过不同的方式来输出数据：
<br>使用 window.alert() 弹出警告框。
<br>使用 document.write() 方法将内容写到 HTML 文档中。
<br>使用 innerHTML 写入到 HTML 元素。
<br>使用 console.log() 写入到浏览器的控制台。

#8、JavaScript字面量
1）数字(number)字面量
- 

	<p id="demo"></p>
	<script>
	document.getElementById("demo").innerHTML = 123e5;
	</script>
这段代码输出的结果就是12300000，也就是123后面跟5个0，其中e是科学计数法。

    <p id="demo"></p>
    <script>
    document.getElementById("demo").innerHTML = 3.10;
    </script>
上面的代码是输出3.10，而实际输出的是3.1,后面的0自动就消失了。
2）字符串字面量
-

	<p id="demo"></p>
	<script>
	document.getElementById("demo").innerHTML = 'MarkDown Pad';
	</script>
这段代码输出的是"MarkDown Pad"。
<br><font color="pink">****注意：这里面的引号可以是单引号'，也可以是双引号"*。只要前后一致就行。***</font></br>
3）表达式字面量
-
表达式字面量是用于计算的

	<p id="demo"></p>
	<script>
	document.getElementById("demo").innerHTML = 5 * 10;
	</script> 
这段代码输出的结果就是“50”。
JavaScript语言有多种类型的运算符：

	类型|实例|描述
	:- | :- | :-
	赋值，算术和位运算符| =  +  -  *  /|在 JS 运算符中描述
	条件，比较及逻辑运算符| ==  != <  >  |在 JS 比较运算符中描述
[JavaScript中有着大量的关键字符，详情点击](http://www.runoob.com/charsets/ref-html-utf8.html "标题")
#9、JavaScript语句
JavaScript中基本的语句标识符
-
	break
	用于跳出循环。
	catch
	语句块，在 try 语句块执行出错时执行 catch 语句块。
	continue
	跳过循环中的一个迭代。
	do ... while
	执行一个语句块，在条件语句为 true 时继续执行该语句块。
	for
	在条件语句为 true 时，可以将代码块执行指定的次数。 
	for ... in 
	用于遍历数组或者对象的属性（对数组或者对象的属性进行循环操作）。
	function
	定义一个函数
	if ... else
	用于基于不同的条件来执行不同的动作。
	return
	退出函数
	switch
	用于基于不同的条件来执行不同的动作。
	throw
	抛出（生成）错误 。 
	try
	实现错误处理，与 catch 一同使用。 
	var
	声明一个变量。
	while
	当条件语句为 true 时，执行语句块。
JavaScript会忽视语句中多余的空格。
对代码行进行折行
-
您可以在文本字符串中使用反斜杠对代码行进行换行。下面的例子会正确地显示：

	document.write("Hello\
	world!");
屏幕上会显示“Helloworld”，不过，您不能像这样折行：

	document.write \ 
	("Helloworld!");
JavaScript中的代码块是和Java中一样，都是用{}框起来的。
#10、JavaScript注释
和Java中的注释是一样的。单行注释是用“`//`”进行开头
<br>多行注释是以“`/*`”开始，“`*/`”结束
#11、JavaScript变量
这个像极了Java中定义变量的方式

	<script>
	var x=5;
	var y=6;
	var z=x+y;
	document.write(x + "<br>");
	document.write(y + "<br>");
	document.write(z + "<br>");
	</script>
后面的`<br>`代表的是换行，否则的话输出的将是<br>`5611`<br>而不是<br>`5`<br>`6`<br>`11`