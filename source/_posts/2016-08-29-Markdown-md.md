---
title: Markdown.md
date: 2016-08-29 13:30:47
tags: Markdown
---
# Markdown 语法说明

## 区块元素

### 段落和换行

前后有一个以上的空行为段落元素，输入两个以上的空格再按回车插入<br />。

### 标题

类Setext形式，用底线的形式。

类atx形式则是在行首插入1到6个\#，对应标题的1到6阶，可以闭合。

### 区块引用

每行前加入\>，或在整个段落第一行加\>，可以嵌套，引用区域也可使用其他的Markdown语法。

### 列表

有序和无序，无序用\*，\+或是\-，有序使用数字接一个英文句点
列表项目内放入引用，\>需要缩进，代码区块的话，该区块要缩进两次，及8个空格或2个制表符。

### 代码区块

缩进4个空格或1个制表符，代码区块里，\&，\<，\>会自动转化成HTML实体，一般的Markdown语法不会被转换。

### 分隔线

一行中三个以上的星号、减号、底线建立一个分隔线。

## 区段元素

### 链接

行内式：

    This is [an example](http://example.com/"Title") inline link.
    [This link](http://example.com) has no title attribute.

参考式：

    This is [an example][id] reference-style link

两个方括号之间可以加入一个空格，接着在文件任意处将标记的链接内容定义出来：

    [id]: http://example.com "Optional title here"

### 强调

用星号和底线作为强调字句的符号，被一个\*或\_包围的字句会被转换为用`<em>`标签包围，两个是用`<strong>`包围。
但是如果你的 * 和 _ 两边都有空白的话，它们就只会被当成普通的符号。

### 代码

标记一小段行内代码用反引号包起来。

### 图片
行内式：

    ![Alt text](path/to/img.jpg)
    ![Alt text](path/to/img.jpg "Optional title")

参考式：

    ![Alt text][id]
    [id]: url/to/image "Optional title attribute"

## 其他
用尖括号包起来的自动连接

    <http://example.com/>
    <address@example.com>

反斜杠，反义字符。