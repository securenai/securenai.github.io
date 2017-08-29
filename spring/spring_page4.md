---
title: Dependency Injection
description: >-
  Automate your task for sending email notification with PowerShell script and
  Windows SMTP Client.
keywords: >-
  software build automation, send email notification, using smtp client in
  powershell, software build notification
tags:
  - Spring
comments: true
published: true
---
<a href="/spring/">Spring</a> >>
<a href="/spring/spring_page1/">Spring 簡介</a> >>
<a href="/spring/spring_page2/">Spring Container</a> >> <a href="/spring/spring_page3/">Spring Beans</a> >> <a href="/spring/spring_page4/" style="color:palevioletred;background-color:papayawhip;">Dependency Injection</a>
<div class="divider"></div>

Dependency Injection (DI)(**<a href="https://stackoverflow.com/questions/130794/what-is-dependency-injection?noredirect=1&lq=1" target="_blank">資料參考</a>**) 是一種設計模式，這種設計模式的理念在於希望將程式裡皮此之間的關係或依賴性降到最低(低耦合性)。

```
Animal monkey = new Monkey();
```
一個 Animal Class 如果要用到 Monkey Class 的物件，它可以使用 `new` 的 keyword 來替它產生，但這意味著兩個 Class 的耦合度(依賴性)相對高，假設 Monkey Class 因為什麼原因而消失或是被異動了，那 Animal 是會受到影響的。