---
title: React 簡介
description: Automate your task for sending email notification with PowerShell script and Windows SMTP Client.
keywords: software build automation, send email notification, using smtp client in powershell, software build notification
tags: [ReactJS]
comments: true
---

React 介紹了另類開發應用程式介面(UI)的方式，它的主要優點是它是`以元件為基礎(Component-Based)`，再來就是

Since the markdown will output the code block into something like `<pre><code>...</code></pre>`, so I can use pure JavaScript to create the line numbers and inject the HTML code into my `<pre><code>` block.

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
```
<div class="divider"></div>