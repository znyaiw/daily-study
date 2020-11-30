# HTML及其结构

HTML()，超文本标记语言，被用来语义化的定义以及描述一个具有良好结构的Web页面的内容。
HTML文档由HTML元素构成，HTML元素由标签名以及尖括号组成的标签来表示：一些标签作为内容
直接写在页面中，另外的一些用来规定文档的文本信息，还有一些可能包含其他的一些标签作为子标签。
浏览器不会显示这些标签，而是将标签视作对页面内容的解释。

## 基础HTML文档

```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>HTML标题</title>
	</head>
	<body>
		HTML内容
	</body>
</html>
```

### <!DOCTYPE>

声明文档类型。文档类型声明类似于链接，规定了HTML页面必须遵从的良好规则，能自动检测错误和其他有用的东西。
```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```
现在只需要声明：`<!DOCTYPE html>`。

### <html></html>

HTML文档的根元素，包裹整个完整的页面。

### <head></head>

head标签包含在HTML页面中但不想在页面中显示的内容，包括搜索结果中出现的关键字和页面描述、CSS样式、字符集声明等等。

### <meta charset="utf-8">

设置文档使用的utf-8字符集编码。

### <title></title>

设置页面标题，出现在浏览器标签上，标记/收藏页面时可用来描述页面。

### <body></body>

包含所有显示在页面上的内容，包括文本、图片、音频和游戏等等。

## 特殊字符

在HTML中，字符`<`, `>`, `"`, `'`和`&`是特殊字符，是HTML语法的一部分，必须使用字符引用来表示字符的特殊编码，以符号`&`开始，`;`结束。
```
原义字符		等价字符引用
<				&lt;
>				&gt;
"				&quot;
'				&apos;
&				&amp;
```

## 注释

注释是被浏览器忽略，而且对用户也不可见，目的是为了描述代码如何工作和不同部分的代码做了什么等。

语法：`<!-- 注释内容 -->`

## 文档结构

```
- 页眉		<header></header>
- 导航栏	<nav></nav>
- 主内容	<main></main>
- 侧边栏	<aside></aside>
- 页脚		<footer></footer>
```
