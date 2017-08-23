---
title: Spring Bean
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
<a href="/spring/spring_page2/" style="color:palevioletred;background-color:papayawhip;">Spring HelloSpring 範例</a> >> <a href="/spring/spring_page3/">Spring Beans</a> >>
<div class="divider"></div>

### 何謂 Spring Bean?

Spring Bean 是物件，這些 Bean 是整個 Spring 應用程式的骨幹，而且被 Spring 的 IOC container 集中管理，這些 Bean 透過我們餵給 Spring container 的設定資料而被建立出來，上一個範例的過程就可以解釋這一點 : 我們先定義了一個 HelloSpring 的物件，然後透過 ApplicationContext(Spring container) 來將 Bean.xml 餵給它處理，有了 Bean.xml 的設定資料，Spring container 便會產生並初始化該 Spring Bean 供我們使用，而這些被 Spring container 建立出來的 Spring Bean 跟一般的 Java Bean 其實大同小異(Spring Bean 也有建構子、getter 和 setter 但它不需要實作 java.io.Serializable.)，甚至可以不用太去在意名詞上的不同，因為說穿了它其實就只是被 Spring container 管理的物件而已。

### 定義 Bean 的屬性

| 屬性                   | 說明                                           |
| -----------------------|-----------------------------------------------|
| class                  | This attribute is mandatory and specifies the |
| name                   | org.springframework.context.ApplicationContext|
|lazy-initialization mode|

