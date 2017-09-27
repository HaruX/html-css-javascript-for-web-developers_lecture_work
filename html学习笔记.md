HTML学习笔记
===

## 一. 环境搭建
### 安装emmet插件指导：http://www.jianshu.com/p/f44e91bf9dfb

## 二. 开发人员基本素养
### Git的使用 https://git-scm.com/book/en/v2
### 社区资源 https://stackoverflow.com/
https://jsfiddle.net/
https://css-tricks.com/
https://codepen.io/


## 三. HTML
* Annotates content
* Defines document structure
* Right ang wrong syntax

### Anatomy of an HTML Tag
**core of HTML**
1. opening closing tag <p></p> except<br><hr>
2. Now every HTML element can have predefined attributes. So we will learn some of the most common ones as we progress in the course, but here's what you need to know about tag attributes in general. Attribute is a name value pair that is kind of a meta data about the element itself that it's being applied to.
> <p id="myid"></p>


3.  Each attribute has its own rules for the meaning of its value. So for example, id attribute, being assigned as an example, has to be unique within the scope of the entire HTML document. In other words, no other element of any kind in the webpage is allowed to have its id attribute equal to the string myID. 分配为id的id属性必须在整个HTML文档的范围内是唯一的。网页中没有任何其他元素的id属性等于字符串myID。

4.  basic spacing rules.
    * No space is allowed to exist between the opening bracket and the tag name.like  < p> And likewise, space is not allowed between the opening bracket and the foreword slash of the closing tag. like < /p>
    *  you must have at least one space between the tag itself and any of its attributes, and space is allowed everywhere else and is simply ignored.

5.  One more rule, attributes can only be specified on the opening tag, so you can't specify an attribute on the closing tag.

6.  value in quote

Summary
* Anatomy of an HTML tag
  * Opening and closing tag
  * attributes
  * Using double and single quotes
  * How to specify tag without any content <p></p>


### Basic HTML Document structure
* HTML version declaration.
* Our first HTML tags. html, meta, head, title, body
* Top to bottom.

```
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title>Courasera is Cool!</title>
</head>
<body>
Courasera is Cool!
</body>
</html>
```

### HTML Content Models  
 The term content model refers to the full behavior the browser applies to the elements belonging to that content model, and to the nesting rules of those elements. In other words, which elements are allowed to be nested inside which other elements. Prior to HTML5 specification, HTML elements were either **block level or inline elements** 块级或内联元素. HTML5 split these two content models into seven models. So, things got a bit more complicated.
* Block-Level Elements and Inline Elements
  * Render to begin on a new line(by default)渲染开始于新行  
    Render on the same line(by default)
  * May contain inline or other block-level elements
  *
```
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>div and span elements</title>
</head>
<body>
	<div>*** DIV 1:Some content here ***</div>
	<div>*** DIV 2: Following right after div1 ***</div>
	<span>*** SPAN 1:Following right after div 2***</span>
	<div>
		*** DIV 3:Following right after span 1
		<span>*** SPAN 2:INSIDE div 3***</span>
		Continue content of div 3***
	</div>
</body>
</html>
```
furturt learning:https://www.w3.org/TR/html5/dom.html#kinds-of-content


###  Heading Elements (and some new HTML5 semantic elements)
