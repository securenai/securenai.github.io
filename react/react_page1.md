---
title: React 簡介
description: >-
  Automate your task for sending email notification with PowerShell script and
  Windows SMTP Client.
keywords: >-
  software build automation, send email notification, using smtp client in
  powershell, software build notification
tags:
  - ReactJS
comments: true
published: true
---

<a href="/react/">React</a> >>
<a href="/react/react_page1/" style="color:lightsalmon;background-color:floralwhite;">React 簡介</a> >>
<a href="/react/react_page2/">JSX</a> >>
<div class="divider"></div>

### React

React 介紹了另類開發應用程式介面(UI)的方式，它的主要優點是它是`以元件為基礎(Component-Based)`，當我們撰寫我們前端網頁的畫面時，我們會用使用許多 DOM 元素去組合出我們想要的呈現方式，ex:<div><span><h1>....等。在許多情形下我們會有想要重複利用同樣的一個功能像是想在我們的頁面上多次使用一個 form 表單，以往作法可能會重複貼上一樣的 code 把表單內容再做微調。而React的精神在於它會把這個 form 看成是一個獨立的元件，當我們用 React 做出一個元件，其他地方便可以再次拿這個元件使用。

### 宣告式編程(declarative) vs 指令式編程(Imperative)
React的另一個優點是它屬於`宣告式編程(declarative)`，這個意思是我們寫程式時是在形容或宣告我們要的結果，這個概念是相對於`指令式編程(Imperative)`，指令式是指我們去形容要做哪些事、哪些步驟要完成才可達到目標。舉例來說我們要做出一個下拉選單選了某個 option 後，會在另一個 input 出現，這樣的功能，我們就會寫一行一行的 javascript 像是改變變數的值、呼叫 function...等等步驟來完成上述的功能，這就是指令式編程，而當我們在 HTML 檔要加圖片時，會寫一個 img 標籤，瀏覽器就知道我們要顯示圖檔，我們用 img 標籤告訴 browser 我們要的結果是一個圖片，這就是宣告式編程的概念，而React提供了宣告式編程的方式來建立我們的使用者介面。

### 虛擬 DOM(Virtual DOM)
動態式網頁常常有動態產生或移除新的元素、或者部分重新整理的動作，這些動作會導致整個 DOM 的重新產出，比方說當我們在一個有20個項目的 list 裡加了1個項目，整個 list 會被重新產生，包含了那21個項目。
React 則是產生一個虛擬的 DOM 這個 DOM 假設也有一個 list，同樣的狀況下，假設增加了一個 item，React 則是很聰明去跟原來前一版的 DOM 比對，判斷說因為你只有增加一個 item，我在重新 render 時，就只 render 那新增的那個 item。

### 如何撰寫虛擬 DOM 元素

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
  |<a class="pagenation_link" href="react/"> 上一頁</a> |
   <a class="pagenation_link" href="/react/react_page2"> 下一頁 </a> |
  </div>
</div>
