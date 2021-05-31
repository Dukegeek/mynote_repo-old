# 2021/5/27

## html标签 
标记语言，单纯标记

## html头部声明
HTML5与HTML4.1有差异  

## 编码问题
中文网页需要声明utf-8,不然乱码
```
<meta charset="utf-8">
```
***
## 标签复习?
## 本地存储
***
### 标签复习一
#### \<base>\</base>
```
<base\> 标签为页面上的所有链接规定默认地址或默认目标。
通常情况下，浏览器会从当前文档的 URL 中提取相应的元素来填写相对 URL 中的空白。

使用 <base> 标签可以改变这一点。浏览器随后将不再使用当前文档的 URL，而使用指定的基本 URL 来解析所有的相对 URL。这其中包括 <a>、<img>、<link>、<form> 标签中的 URL。
```
#### \<canvas>\</canvas>
canvas只是画布容器，具体的还的是js控制<br/>
#### \<video>\</video>
***
### 新的特殊内容元素(语义化)
- \<article>\</article>
- \<footer>\</footer>
- \<header>\</header>
- \<nav>\</nav>
- \<section>\</section>
***
### 新的表单控件
- \<calendar>\</calendar>
- \<date>\</date>
- \<time>\</time>
- \<email>\</email>
- \<url>\</url>
- \<search>\</search>
***
### 新语义元素
- \<bdi>\</bdi>
