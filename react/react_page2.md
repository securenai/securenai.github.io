---
title: JSX
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
<a href="/react/react_page1/">React 簡介</a> >>
<a href="/react/react_page2/" style="color:palevioletred;background-color:papayawhip;">JSX</a> >>
<div class="divider"></div>

### JSX
我們大可以在要寫 React 的地方每次都寫這種 `ReactDOM.render(...);` 的寫法，但會發現不適很方便，JSX是一個解決此問題的方法，JSX 是 javascript 的延伸，可以允許我們用 xml 的語法來建立我們 `ReactDOM.render(...);`的呼叫。
所以原先我們這樣寫.... 托JSX的幫忙 會變成......
但JSX的表示我們的程式並不是先天或是理所當然地可以看懂的，必須要有某種懂JSX語法的工具來幫我們翻譯成React.createElement 的呼叫使瀏覽器可以執行它，也就是需要這個工具幫我們把JSX翻譯成Javascript的code，它叫做[Babel](https://babeljs.io/)，
