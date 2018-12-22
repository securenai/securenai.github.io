---
title: Objects
description: >-
  Automate your task for sending email notification with PowerShell script and
  Windows SMTP Client.
keywords: >-
  software build automation, send email notification, using smtp client in
  powershell, software build notification
tags:
  - javascript
comments: true
published: true
---

<a href="/javascript/">Javascript</a> >>
<a href="/javascript/javascript_intro/">javascript intro</a> >>
<a href="/javascript/javascript_variables/">variables</a> >>
<a href="/javascript/javascript_functions/">functions</a> >>
<a href="/javascript/javascript_objects/" style="color:palevioletred;background-color:papayawhip;">objects</a> >>
<div class="divider"></div>

### Objects

js物件可被視為一群屬性的集合，物件的好處就是透過將許多資料(屬性`properties`跟方法`methods`)打包後供我們方便使用，物件的屬性透過key-value的形式儲存，是為該物件量身打造的屬性，屬性告訴我們有關於該物件的相關資訊。

其實屬性跟方法說穿了就是變數跟函數，只是它們被定義在物件裡面時，習慣把它們稱為屬性跟方法。

### 利用 Object literal 創造物件
Object literal 是創造js object的一種方式，語法如下:
```
var book = { }
```

利用 `var` or `const`(ES6)來宣告一個變數book，並用"{ }"assign給book，目前此為一個空的物件。

接下來要定義該物件的一些屬性properties，就以key-value的形式定義之:
```
var book = { 
  name : 'javascript',
  pages : 600,
  author : 'Alex',
  copies : 250,
  sold : 200
}
```
`name`、`pages`、`author`、`copies`、`sold`都是剛剛定義的屬性，明顯的看得出它們述說者物件book的一些資訊，這就是屬性的意義。

談到語法，屬性的定義遵守key-value的概念，屬性key跟value以冒號隔開，以name的屬性來說:左邊是key，也就是屬性的名稱，叫做name，而右邊就是屬性的value(值)，叫'javascript'，同一個物件不可宣告兩個相同key的屬性，多個屬性時，每個屬性後面須以逗號隔開。

再來要定義該物件的方法(method):
```
var book = { 
  name : 'javascript',
  pages : 600,
  author : 'Alex',
  copies : 250,
  sold : 200,
  checkStock : function(){
    return book.copies - book.sold;
  }
}
```
當我們定義一個leftInstock屬性，而key是一個函數function時，這就會視為物件的方法method，回傳一個結果，function裡面的程式若看不懂沒關係，後面會解釋，目前只需要知道方法精神在於呼叫物件的行為，以此例來說當你呼叫checkStock時，可以得知目前這本書還剩下多少庫存。

所以結論是，物件的精神在於將許多資訊(屬性和方法)包裝在一起，成為一個物件，這些資訊僅為此物件擁有，必須透過該物件才能使用其屬性和方法，有封裝的概念。


> 參考資料(英文) **<a href="https://tylermcginnis.com/imperative-vs-declarative-programming/" target="_blank"> Imperative vs Declarative Programming</a>**


### Variables2
動態式網頁常常有動態產生或移除新的元素、或者部分重新整理的動作，這些動作會導致整個 DOM 的重新產出，比方說當我們在一個有20個項目的 list 裡加了1個項目，整個 list 會被重新產生，包含了那21個項目。
React 則是產生一個虛擬的 DOM 這個 DOM 假設也有一個 list，同樣的狀況下，假設增加了一個 item，React 則是很聰明去跟原來前一版的 DOM 比對，判斷說因為你只有增加一個 item，我在重新 render 時，就只 render 那新增的那個 item。

### Variables3

我們要如何在虛擬 DOM 裡形容一個 DOM 元素呢?
DOM 元素主要由三樣東西組成等
1. 名稱 : 形容該元素是甚麼類型，是 p，還是 a，還是 h1、div....等
2. 屬性 : 一組 key 跟 value 提供更多資訊像是 type、href....等
3. 內容 : 有些元素有，有些沒有，例 : `<p>hello</p>` 

簡單的 Hello World 例子
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Hello World</title>
    <script src="https://unpkg.com/react@latest/dist/react.js"></script>
    <script src="https://unpkg.com/react-dom@latest/dist/react-dom.js"></script>
    <script src="https://unpkg.com/babel-standalone@6.15.0/babel.min.js"></script>
  </head>
  <body>
    <div id="root"></div>
    <script type="text/babel">

      ReactDOM.render(
        <h1>Hello, world!</h1>,
        document.getElementById('root')
      );

    </script>
  </body>
</html>
```

---
<div class="pagenation_center">
  <div  class="pagenation_center_inner">
  |<a class="pagenation_link" href="/javascript/javascript_intro"> 上一頁</a> |
   <a class="pagenation_link" href="/javascript/javascript_functions"> 下一頁 </a> |
  </div>
</div>
