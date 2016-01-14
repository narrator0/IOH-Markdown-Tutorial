# IOH Markdown Tutorial

## Introduction

Markdown 是一種簡便的格式，用以快速編輯美觀的文件。

舉例而言你可以輸入：

```
## This is a _table_

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

```

你就會看到：

## This is a _table_

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

這樣的用語被廣泛使用，如Github, Trello 和 Gitbook，以下將會逐一帶領你學習如何使用這樣的語法編輯自己的文件。在開始本教學之前，你可以先下載MacDown編輯器以供你之後的練習。

> [MacDown 官網](http://macdown.uranusjr.com/)



## Table of Contents

1. [Introduction](#introduction)
2. [Table of Contents](#table-of-contents)
3. [Syntax Guide](#syntax-guide)
4. [Other](#other)
5. [Reference](#reference)

## Syntax Guide

### 段落跟換行

Markdown裡面的換行方式比較特別，假如你輸入：

```
first line
second line
```

你會看到：  

```
first line second line
```

所以他並沒有換行，原因是因為Markdown的換行標準為兩個空白鍵，段落標準為兩個`Enter`鍵，所以你必須在`line`後面再加上兩個空白鍵，你才會看到：  

```
first line  
second line
```

### Headers

在標題方面採用的是階層的方式，在你想要當成標題的文字前面加上1 ~ 6個`#`，就分別代表著第一大標到第六大標，範例如下：

輸入

```
# Header 1
## Header 2
```

得到

# Header 1
## Header 2


### Emphasis

Markdown中提供斜體跟粗體兩種型態，讓你可以強調你想要的字。只要將你想標記的字用一個`*`或`_`夾住，它就會呈現斜體，兩個的話則會變成粗體。

輸入

```
My name is *italic*
My name is **bold**
```

得到

My name is *italic*  
My name is **bold**

### Lists

要條列任何東西在這裡都非常的簡單，如果是數字清單的話可以在你的每一項之前加上`1.`，不用懷疑，都加上`1.`就可以，程式會自動幫你計算它是第幾個；另外，如果你不想用數字的話也可以單純加上`*`或`-`就好。

輸入

```
1. order list 1
2. order list 2
3. order list 3

* unordered list 1
- unordered list 2
* unordered list 3
```

得到

1. order list 1
2. order list 2
3. order list 3

* unordered list 1
- unordered list 2
* unordered list 3

> 也可以在清單中再加入清單，只要層次分清楚，屬於第二層的必須在前面加一個空白鍵。

### Links

連結的部分也有兩種不同的語法，如果你想要在整個網址加上連結的話，只要用`<``>`夾住你想要的連結，它就會直接變成一個連結；另外，如果你想要把連結放在某段你指定的文字上的話，就必須用`[文字](網址)`的格式，如此設定，可以把你想要的網址綁定在指定的文字上。

輸入

```
<http://www.markdown-tutorial.com>
[Markdown Tutorial](http://www.markdown-tutorial.com)
```

得到

<http://www.markdown-tutorial.com>  
[Markdown Tutorial](http://www.markdown-tutorial.com)


### Images

Markdown也可以輕鬆插入圖片，但因為它是純文字檔，所以不能嵌在檔案裡面，所以只能用連結的方式嵌入，語法是`![替代文字](網址)`。這裡要注意的是Markdown語法其實對圖片非常不友善，因為它無法自由設定圖片的長寬，所以必須客製化圖片的大小。

> 替代文字指的是在圖片無法找到的時候，會用一段文字代替。

輸入

```
![Image of Cat](https://pixabay.com/static/uploads/photo/2012/04/12/21/29/cat-30720_960_720.png)
```

得到

![Image of Cat](https://pixabay.com/static/uploads/photo/2012/04/12/21/29/cat-30720_960_720.png)

### Blockquotes

輸入

```
> 一行註解
```

得到

> 一行註解

### Inline Code

Markdown 並不會依照我們的排版顯示文字，所以當我們需要有完全的控制權的時候，可以使用inline code的方式。

輸入

```
 ```
 //          ┌─┐       ┌─┐
 //       ┌──┘ ┴───────┘ ┴──┐
 //       │                 │
 //       │       ───       │
 //       │  ─┬┘       └┬─  │
 //       │                 │
 //       │       ─┴─       │
 //       │                 │
 //       └───┐         ┌───┘
 //           │         │
 //           │         │
 //           │         │
 //           │         └──────────────┐
 //           │                        │
 //           │                        ├─┐
 //           │                        ┌─┘
 //           │                        │
 //           └─┐  ┐  ┌───────┬──┐  ┌──┘
 //             │ ─┤ ─┤       │ ─┤ ─┤
 //             └──┴──┘       └──┴──┘
 ```
```

得到

```
 //          ┌─┐       ┌─┐
 //       ┌──┘ ┴───────┘ ┴──┐
 //       │                 │
 //       │       ───       │
 //       │  ─┬┘       └┬─  │
 //       │                 │
 //       │       ─┴─       │
 //       │                 │
 //       └───┐         ┌───┘
 //           │         │
 //           │         │
 //           │         │
 //           │         └──────────────┐
 //           │                        │
 //           │                        ├─┐
 //           │                        ┌─┘
 //           │                        │
 //           └─┐  ┐  ┌───────┬──┐  ┌──┘
 //             │ ─┤ ─┤       │ ─┤ ─┤
 //             └──┴──┘       └──┴──┘
```

> 本圖原作連結：<https://github.com/Lorex/Bugfree.js>


### Code Blocks

Code blocks的樣式跟 inline code基本上是一樣的，差別在於code block是單行的。

輸入

```
如果以要離開請按下`Command` + `Q`
```

得到

如果以要離開請按下`Command` + `Q`

### Tables

Markdown 中提供一種便捷的方式產生表格，用`|`跟`-`分別代表橫向跟縱向的分隔線。

輸入

```
title1 | title2 | title3
- | - | -
row1 | row2 | row3
- | - | -
row1 | row2 | row3
```

得到

Title1 | Title2 | Title3
------ | ------ | -----
row1   | row2   | row3
------ | ------ | -----
row1   | row2   | row3

## Other

### 跳脫字元

因為語法中很多符號是有特殊意義的，但如果你想要顯示符號本身的話，必須前面加上反斜線`\`，以下是特殊符號的列表：

```
\   反斜線
`   反引號
*   星號
_   底線
{}  大括號
[]  方括號
()  括號
#   井字號
+   加號
-   減號
.   英文句點
!   驚嘆號
```

### Html Support

Markdown 中支援直接使用Html tag，如果想要學習使用Html做出更多效果，可以參考[codecademy](codecademy.com)或是[w3school](http://www.w3schools.com/)。

輸入

```
first line <br> second line <br> third line
```

得到

first line <br> second line <br> third line

## Reference

以下為參考資料：
> <https://github.com/othree/markdown-syntax-zhtw>  
> <https://guides.github.com/features/mastering-markdown/>  
> <http://www.markdown-tutorial.com>



