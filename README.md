###网站的架构
- CS：Client Server 客户端和服务端
	移动客户端：Android和iOS
	电脑客户端：windows和linux、Mac OS
	客户端是由客户端工程师开发
	服务端功能：给客户端提供数据 
	应用场景： 京东、淘宝、唯品会
- BS：Browser Server 浏览器和服务端
	浏览器
	服务端功能： 给浏览器提供数据 和 页面
	应用场景： 页游  
![](01.png)
- 将来工作 BS和CS架构都会涉及，但是只需要掌握BS架构 CS就会了

###课程介绍

![](02.png)
###前端课程介绍
1. HTML ： 用来勾勒出页面的结构和内容(骨架)
2. CSS ： 用来美化页面 
3. JavaScript： 让页面呈现动态效果和动态数据的
4. JQuery：用来简化JavaScript代码的

###HTML
	Hyper Text Markup Language：超文本标记语言 
- 什么是超文本：不仅仅是文本，还包括文本的字体颜色，样式 还包括多媒体（图片，音频，视频）
- html学习内容： 学习有哪些固定的标签，还有标签内部有哪些属性和标签和标签之间的嵌套关系

###通过Eclipse创建html文件 
- 新建文件-> other->搜索html 

###html结构

		<!DOCTYPE html>   //文档声明 告诉浏览器使用html的哪个版本来解析页面内容 ，此写法是告诉浏览器用最新的html5的版本解析 
		<html>//所有内容都在html标签内部 除了 文档声明
			<head>//头 ：里面的内容是给浏览器看的 比如使用什么编码 
			</head>
			<body>//体 ：里面的内容是给用户看的 
			</body>
		</html>
####head里面的标签

		<meta charset="UTF-8">：告诉浏览器使用哪种字符集解析

		<title>Insert title here</title> 告诉浏览器 页面标题是什么，title还可以起到优化SEO的作用（让搜索引擎尽快搜索到此页面）
		 keywords的作用：让搜索引擎尽快的找到本页面

###Body内部的标签
####文本标签
		
		1. <h1></h1>.......<h6></h6> 内容标题
		- align：left/center/right  水平对齐方式
		2. <p></p>    段落标签 ，每个段落标签独占一行并且上下会留有空白区域
		3. <hr> 水平分割线
		4. <br> 换行
####列表标签
		
		1. 无序列表：
 
			<ul type="circle"> <!-- u:unordered 无序 l:list 列表 -->
				<li>刘备</li><!--l:list列表 i:item 项  -->
				<li>貂蝉</li>
				<li>孙尚香</li>
				<li>孙悟空</li>
			</ul>


	
