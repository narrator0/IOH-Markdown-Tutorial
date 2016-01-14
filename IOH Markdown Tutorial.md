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

```

### Blockquotes

### Inline Code

### Code Blocks

### Tables

## Other

### 自動連結

### 跳脫字元

### Html Support

## Reference

> 學習資源 <http://www.markdown-tutorial.com>



