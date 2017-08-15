---
title: Spring HelloSpring 範例
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
首先，開啟 Eclpise 然後 Import 一個 Maven project : [New] -> [Project] -> [Maven Project]

Group Id : com.example

Artifact Id : spring

![Spring](spring_images/springconfig01.png)

### 利用 Maven 匯入 Spring Dependencies
接下來可以利用 Maven 專案的 POM 檔匯入所有 Spring 需要的 jar 檔。目前只是單純的 Java application，這裡匯入 spring-context 相關的 dependency 即可。

**<a href="https://mvnrepository.com/artifact/org.springframework/spring-context/4.3.9.RELEASE" target="_blank">spring-context4.3.9.RELEASE</a>**

然後在 Maven 專案的 pom 檔匯入相關資源
```
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-context</artifactId>
    <version>4.3.9.RELEASE</version>
</dependency>
```
![Spring](spring_images/springconfig02.png)
