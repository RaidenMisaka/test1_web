### 课程回顾
1. html结构

<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title>页面标题</title>
		<meta name="keywords" content="A,B,C">
	</head>
	<body></body>
</html>
2. 文本元素
	<h1-6></h1-6> 内容标题
	<p>段落</p> 
	<hr> 水平分割线
	<br> 换行
3. 列表元素
- 有序   ol  li   属性：type(1 a A i I) start reversed 
- 无序   ul  li  属性: type
- 定义列表   dl  dt dd
- 列表嵌套  可以无限制互相嵌套
4. 分区元素 
- div: 块级分区元素  独占一行
- span： 行内分区元素  共占一行 
5. 元素分类
- 块级元素： 独占一行 div h1-6 p hr 
- 行内元素： 共占一行 span  i和em b和strong s和del  u 
6. 特殊字符
- 空格 ： &nbsp;
- 小于号： &lt;
- 大于号:  &gt;
- 换行: <br>
7. 图片元素 img
- 支持格式： jpg/jpeg png  gif
- 属性：
1. alt：图片不能正常显示的时候显示此文本
2. src：图片的路径 （相对路径和绝对路径）
3. title: 鼠标悬停的时候显示的文本
4. width：宽  可以设置像素200px或百分比50%，如果只设置宽高度会按比例缩放
5. height：高

#### Map 图像地图
- 什么是图像地图： 可以将图片的某个区域作为可点击的链接
- 使用方式：

		<!-- usemap:使用地图 #代表当前页面 -->
		<img alt="" src="../imgs/b.jpg" usemap="#mymap">
		<!-- 为了保证兼容性问题 把name和id都写上  -->
		<map name="mymap" id="mymap">
			<!-- area区域  shape形状 rect矩形 coords坐标-->
			<area shape="rect" coords="0,0,200,200" 
					href="../imgs/2.gif">
			<area shape="circle" coords="663,473,90"
				 href="../imgs/d.jpg">
		</map>
- map中的id和name作用是让图片能够找得到此地图
- area常见属性： shape表示形状 常用有circle和rect
- href：值为一个路径，可以写相对路径和绝对路径，路径可以指向页面，也可以指向文件（浏览器可以打开的文件直接浏览，不能打开的文件则下载）

### 超链接 a标签
- 如果a标签没有添加href属性 就相当于一个文本不是超链接
- href属性和图像地图中的href作用一样
- target="_blank" 开启一个新的页面
- 锚点用法： 需要先创建锚点:<a id="a" name="a"></a>, 然后通过a标签跳转到锚点的位置：<a href="#a">跳转到锚点</a>
- img标签放在a标签内部 则图片就可以被点击了

### 表格 table
- 接触标签有 table tr td
- table的属性：align水平对齐 width宽度 border边框 cellspacing边框和单元格的距离 cellpadding内容和单元格的距离 
- td的属性：colspan跨列  rowspan跨行 align水平对齐
- caption标签
- 分组标签：<thead> <tbody> <tfoot>  没有任何显示效果，提高代码可读性

### 表单
- 表单的作用是收集用户的数据提交到服务端
- 表单中的控件包括： 文本框、密码框、按钮、下拉列表、单选、复选、时间选择、文件选择、文本域
#### 文本框 

		<input type="text" placeholder="占位文本" maxlength="最大字符长度" readonly="只读" >
#### 密码框

		<input type="password" maxlength>

#### 单选

		<input type="radio" checked默认选中>

#### 多选、复选框

		<input type="checkbox" id="aaa">  <label for="aaa">xxx</label>

#### 时间

		<input type="date" >

#### 文件

		<input type="file" >

#### 下拉选

		<select name>
				<option value selected></option>
		<select>

#### 文本域 
	
		<textarea rows="行数" cols="列数"></textarea>

#### 隐藏域

		<input type="hidden">

#### 按钮

		<input type="submit/reset/button" value="按钮标题">



### 课程回顾：

1. 图像地图 <map id name>   

			<map>
				<area shape="rect/circle" coords="" href=""></area>
			</map>
2. 超链接 a   
	属性： target="_blank" 新页面中显示 href同上
- 锚点用法：  <a id name></a>    <a href="#id/name">跳转到</a>
3. 表格
- 标签 table tr td th  thead tbody tfoot  caption:表格的标题
- table属性：border 边框  cellspacing cellpadding  align  width
- td属性：rowspan 行   colspan列
4. 表单
<form action="提交地址" method="get/post">
	<input type="text/password/radio/checkbox/date/file/hidden/submit/reset/button" name id value placeholder maxlength readonly checked >
	<label for="id">
	<select name> <option value selected> 
</form>
