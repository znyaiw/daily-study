# HTML元素与属性

## html
文档根元素。

```
1. 	!DOCTYPE html
	声明文档类型
2.	lang
	设置文档语言
```
> <!DOCTYPE html lang="en">
> !DOCTYPE: 文档类型声明
> lang: 设置文档语言

## head
其内容不会显示在页面中，作用是保存页面的一些元数据。

```
1. 	title
	为文档添加标题。title是一项元数据，用于表示整个HTML文档的标题(而不是文档内容)。

2. 	meta
	元数据，描述数据的数据。
	2.1	charset: 指定文档字符编码。
	2.2 name和content: name指定meta元素的类型，说明该元素包含了什么类型的信息；content指定实际的元数据内容。

3. 	link
	添加自定义引用。
	2.1 rel 引用类型
	2.2 href 引用地址
	2.3 type 引用属性

4. 	script
	放在头部的script在浏览器解析之前加载。
	4.1 type 引用类型
	4.2 src 引用地址
```
> 1. name值
> author: 指定文档作者
> description: 被使用在搜索引擎显示的结果页中
> keywords: 提供关键词给搜索引擎，已被忽略
> property: 提供可使用的特定信息

> 2. 自定义图标
> <link ref="shortcut icon" href="favicon.ico" type="image/x-icon">
> 如果网站使用了内容安全策略(Content Security Policy, CSP)来增加安全性，这个会应用在图标上。如果图标没有被加载，需要确认Content-Security-Policy header的`img-src` directive没有禁止访问图标。

> 3. 引用外部css文件
> <link ref="stylesheet" href="style.css">
> stylesheet: 表明文档的样式表
> href: 样式表文件的路径

> 4. 引用外部script文件
> <script src="script.js"></script>
> script元素看起来像一个空元素，但其实并不是，因此需要一个结束的标记。通常放在文档的尾部，以确保在加载脚本之前浏览器已经解析了HTML内容(如果脚本加载某个不存在的元素，浏览器会报错)。

## body
HTML文档主体内容。

```
1.	标题和段落
	1.1 h1: 在页面加载完毕时显示在页面中，通常只出现一次，用来标记页面内容的标题。
		<h1>主标题</h1>
	1.2 h2: 副标题
		<h2>副标题</h2>
	1.3 h3: 次副标题
		<h3>次副标题</h3>
	1.4 p: 文本段落
		<p>文本段落</p>

2. 	列表
	2.1 无序列表 ul [unordered list]
		<ul><li>...</li>...</ul>
	2.2 有序列表 ol [ordered list]
		<ol><li>...</li>...</ol>
	2.3 嵌套列表
3. 	强调/斜体/粗体/下划线...
	3.1 em: emphasis 标记强调内容，可以被阅读器识别出来，并以不同的语调发出。
	3.2 i: italics 被用来表达传统上用斜体表达的意义。
	3.3 b: bold 被用来表达传统上用粗体表达的意义。
	3.4 u: underline 被用来表达传统上用下划线表达的意义。
```
> 1. 标题
> 每个页面中只使用一次h1，保持标题层次结构，且最好不要超过三级标题。
> 较深的层次结构不便于操作与导航。

> 2. 语义元素与表象元素
> 语义元素: p, h1, h2, h3, em
> 表象元素: i, b, u
