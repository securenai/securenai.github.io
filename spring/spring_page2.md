---
title: Spring 相關設定
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
首先 Import 一個 Maven project : [New] -> [Project] -> [Maven Project]
![Spring](spring_images/springconfig01.png)

接下來可以利用 Maven 專案的 POM 檔匯入所有 Spring 需要的 jar 檔。目前只是單純的 Java application，這裡
匯入 spring-context 相關的 dependency 即可。

**<a href="https://mvnrepository.com/artifact/org.springframework/spring-context/4.3.9.RELEASE" target="_blank">Home » org.springframework » spring-context » 4.3.9.RELEASE</a>** <--html

