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
<a href="/spring/spring_page2/">Spring Container</a> >> <a href="/spring/spring_page3/" style="color:palevioletred;background-color:papayawhip;">Spring Beans</a> >> <a href="/spring/spring_page4/">Dependency Injection</a>
<a href="/spring/spring_mvc_page01/">Spring MVC介紹</a>
<div class="divider"></div>

### 何謂 Spring Bean?

Spring Bean 是物件，這些 Bean 是整個 Spring 應用程式的骨幹，而且被 Spring 的 IOC container 集中管理，這些 Bean 透過我們餵給 Spring container 的設定資料而被建立出來，上一個範例的過程就可以解釋這一點 : 我們先定義了一個 HelloSpring 的物件，然後透過 ApplicationContext(Spring container) 來將 Bean.xml 餵給它處理，有了 Bean.xml 的設定資料，Spring container 便會產生並初始化該 Spring Bean 供我們使用，而這些被 Spring container 建立出來的 Spring Bean 跟一般的 Java Bean 其實大同小異(Spring Bean 也有建構子、getter 和 setter 但它不需要實作 java.io.Serializable.)，甚至可以不用太去在意名詞上的不同，因為說穿了它其實就只是被 Spring container 管理的物件而已。

### 定義 Bean 的屬性

在上一個範例中，我們有在 Bean.xml 裡定義了 Bean 的屬性 :

Bean.xml
```
<?xml version="1.0" encoding="UTF-8"?>

<beans xmlns = "http://www.springframework.org/schema/beans"
   xmlns:xsi = "http://www.w3.org/2001/XMLSchema-instance"
   xsi:schemaLocation = "http://www.springframework.org/schema/beans
   http://www.springframework.org/schema/beans/spring-beans-3.0.xsd">

   <bean id = "helloSpring" class = "com.example.spring.HelloSpring">
      <property name = "message" value = "Hello Spring!"/>
   </bean>

</beans>
```

`id = "helloSpring"` : 此 id 可以自己定義，不過在使用 `context.getBean` 時需要用到這個 id 來認 Bean.xml 所對應的 Bean 設定

`class = "com.example.spring.HelloSpring"` : 此 class 是用來 Mapping 到我們所定義的 POJO Class，需要連 package name 也標示出來。

`property name = "message" value = "Hello Spring!"` : 

| 屬性                   | 說明                                           |
| -----------------------|:----------------------------------------------|
| class                  |強制性的要求指定要以哪個類別建立 Bean             |
| name                   |                                               |
|lazy-initialization mode|

### Bean 設定的種類

Bean 設定的種類主要分為三大種類 : 

1. 以 XML 為 Base 的設定檔
2. 以 Annotation 為 Base 的設定檔
3. 以 Java 為 Base 的設定檔
