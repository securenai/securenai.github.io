---
title: Spring MVC 介紹
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

### 範例
現在建立一個最基本的 Spring MVC Web 專案，在 Eclipse 新增一個 Dynamic Web Project，建立好的專案下有一個目錄叫作 WebContent，裡面有 WEB-INF 的目錄，在 WEB-INF 之下可以需要新增一個 .xml 檔，名字取為 `web.xml` (名稱必須為 web.xml)

步驟 : 1> [NEW] -->

為了要匯入 Spring MVC 相關的 jar 檔，建議將專案 configure 成 Maven Project，接下來就可以在 Pom.xml 裡加上 Spring MVC 所需要的 Dependency，要使用 Spring Web 以及要 Servlet 的支援，就必須加入以下兩個 Dependency。

1. <a href="https://mvnrepository.com/artifact/org.springframework/spring-web" target="_blank">spring-web</a>
2. <a href="https://mvnrepository.com/artifact/org.springframework/spring-webmvc" target="_blank">spring-webmvc</a>

`spring-web` 包含了一些很常用的 web 及 servlet 的功能，而 `spring-webmvc` 提供 servlet 環境正常的 MVC 支援，
不過由於 `spring-webmvc` 已經有 `spring-web` 作為它的 dependency 之一了，所以當我們在使用 `spring-webmvc` 時就可以不需要 spring-web，因此其實 dependency 加入 `spring-webmvc` 即可。

```
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-web</artifactId>
    <version>${org.springframework.version}</version>
</dependency>
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-webmvc</artifactId>
    <version>${org.springframework.version}</version>
</dependency>
```