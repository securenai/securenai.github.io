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


React 介紹了另類開發應用程式介面(UI)的方式，它的主要優點是它是`以元件為基礎(Component-Based)`，當我們撰寫我們前端網頁的畫面時，我們會用使用許多 DOM 元素去組合出我們想要的呈現方式，ex:<div><span><h1>....等。在許多情形下我們會有想要重複利用同樣的一個功能像是想在我們的頁面上多次使用一個 form 表單，以往作法可能會重複貼上一樣的 code 把表單內容再做微調。而React的精神在於它會把這個 form 看成是一個獨立的元件，當我們用 React 做出一個元件，其他地方便可以再次拿這個元件使用。

### 宣告式編程(declarative) vs 指令式編程(Imperative)
React的另一個優點是它屬於`宣告式編程(declarative)`，這個意思是我們寫程式時是在形容或宣告我們要的結果，這個概念是相對於`指令式編程(Imperative)`，指令式是指我們去形容要做哪些事、哪些步驟要完成才可達到目標。舉例來說我們要做出一個下拉選單選了某個 option 後，會在另一個 input 出現，這樣的功能，我們就會寫一行一行的 javascript 像是改變變數的值、呼叫 function...等等步驟來完成上述的功能，這就是指令式編程，而當我們在 HTML 檔要加圖片時，會寫一個 img 標籤，瀏覽器就知道我們要顯示圖檔，我們用 img 標籤告訴 browser 我們要的結果是一個圖片，這就是宣告式編程的概念，而React提供了宣告式編程的方式來建立我們的使用者介面。

簡單的 Hello World 例子
```
<!DOCTYPE html>
<html>
<head>
  <script src="http://fb.me/react-0.13.1.js"></script>  
</head>
<body>
  <div id="app"></div>
  <script>
      var HelloMessage = React.createClass({
        displayName: "HelloMessage",
        render: function() {
          return React.createElement("div", null, "Hello World ", null);
        }
      }),mountNode=document.getElementById('app');
    
    React.render(React.createElement(HelloMessage, null), mountNode);
  </script>
</body>
```
### JSX



Since the markdown will output the code block into something like `<pre><code>...</code></pre>`, so I can use pure JavaScript to create the line numbers and inject the HTML code into my `<pre><code>` block.

```js
React.createElement('a': {
 href: "http://example.com.tw"
},"example")
```

```js
(function() {
  var pre = document.getElementsByTagName('pre'),
      pl = pre.length;
  for (var i = 0; i < pl; i++) {
    pre[i].innerHTML = '<span class="line-number"></span>' + pre[i].innerHTML + '<span class="cl"></span>';
    var num = pre[i].innerHTML.split(/\n/).length;
    for (var j = 0; j < (num - 1); j++) {
      var line_num = pre[i].getElementsByTagName('span')[0];
      line_num.innerHTML += '<span>' + (j + 1) + '</span>';
    }
  }
})();
(function() {
  var pre = document.getElementsByTagName('pre'),
      pl = pre.length;
  for (var i = 0; i < pl; i++) {
    pre[i].innerHTML = '<span class="line-number"></span>' + pre[i].innerHTML + '<span class="cl"></span>';
    var num = pre[i].innerHTML.split(/\n/).length;
    for (var j = 0; j < (num - 1); j++) {
      var line_num = pre[i].getElementsByTagName('span')[0];
      line_num.innerHTML += '<span>' + (j + 1) + '</span>';
    }
  }
})();
(function() {
  var pre = document.getElementsByTagName('pre'),
      pl = pre.length;
  for (var i = 0; i < pl; i++) {
    pre[i].innerHTML = '<span class="line-number"></span>' + pre[i].innerHTML + '<span class="cl"></span>';
    var num = pre[i].innerHTML.split(/\n/).length;
    for (var j = 0; j < (num - 1); j++) {
      var line_num = pre[i].getElementsByTagName('span')[0];
      line_num.innerHTML += '<span>' + (j + 1) + '</span>';
    }
  }
})();
(function() {
  var pre = document.getElementsByTagName('pre'),
      pl = pre.length;
  for (var i = 0; i < pl; i++) {
    pre[i].innerHTML = '<span class="line-number"></span>' + pre[i].innerHTML + '<span class="cl"></span>';
    var num = pre[i].innerHTML.split(/\n/).length;
    for (var j = 0; j < (num - 1); j++) {
      var line_num = pre[i].getElementsByTagName('span')[0];
      line_num.innerHTML += '<span>' + (j + 1) + '</span>';
    }
  }
})();
```

<div class="divider"></div>
