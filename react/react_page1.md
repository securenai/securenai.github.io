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


React 介紹了另類開發應用程式介面(UI)的方式，它的主要優點是它是`以元件為基礎(Component-Based)`，當我們撰寫我們前端網頁的畫面時，我們會用使用許多 DOM 元素去組合出我們想要的呈現方式，ex:<div>、<span>、<h1>....等。在許多情形下我們會有想要重複利用同樣的一個功能像是想在我們的頁面上多次使用一個 form 表單，以往作法可能會重複貼上一樣的 code 把表單內容再做微調。而React的精神在於它會把這個 form 看成是一個獨立的元件，當我們用 React 做出一個元件，其他地方便可以再次拿這個元件使用。

React的另一個優點是它屬於`宣告式編程(declarative)`，這個意思是我們寫程式時是在形容我們要達成的結果，這個概念是相對於`指令式編程(Imperative)`


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
