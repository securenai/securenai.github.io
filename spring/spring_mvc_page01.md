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
現在建立一個最基本的 Spring MVC Web 專案，在 Eclipse 新增一個 Dynamic Web Project，建立好的專案下有一個目錄叫作 WebContent，裡面有 WEB-INF 的目錄，在 WEB-INF 之下可以 new 一個 xml 檔，名字取為 web.xml (名稱必須為 web.xml)

為了要匯入 Spring MVC 相關的 jar 檔，建議將專案 configure 成 Maven Project，接下來就可以在 Pom.xml 裡加上 Spring MVC 所需要的 Dependency，

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
