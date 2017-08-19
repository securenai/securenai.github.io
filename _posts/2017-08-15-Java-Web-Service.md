---
layout: post
title: Java Web Service
comments: true
description: Java Web Service
keywords: dummy content
published: true
---

開啟 eclipse 建立一個 Maven 專案:

步驟 : [new] --> [other]--> [Maven] --> [Maven Project]

<!--![ws1.png](/assets/images/post_images/ws1.png)-->

archetype 請選擇 maven-archetype-webapp : 

![ws2.png](/assets/images/post_images/ws2.png)

group id : com.securenai.sample [我的例子，您可以自訂]

artifact id : hellows [我的例子，您可以自訂]

建好之後，如果進到 pom.xml 應該會看到這樣 : 

```
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>com.securenai.sample</groupId>
  <artifactId>hellows</artifactId>
  <packaging>war</packaging>
  <version>0.0.1-SNAPSHOT</version>
  <name>hellows Maven Webapp</name>
  <url>http://maven.apache.org</url>
  <dependencies>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>3.8.1</version>
      <scope>test</scope>
    </dependency>
  </dependencies>
  <build>
    <finalName>hellows</finalName>
  </build>
</project>
```
我們開 pom.xml 原因是要準備匯入 webservice 的相關資源工具讓我們直接使用，這樣我們可以專心處理跟業務邏輯有關的程式而不要太去鑽研在 webservice 的底層運作。

# Maven Dependencies

最後的 Pom.xml 的 dependencies 應要包含以下 :
```
<dependencies>
  <dependency>
	<groupId>org.apache.cxf</groupId>
	<artifactId>cxf-rt-frontend-jaxws</artifactId>
	<version>3.0.3</version>
  </dependency>
        
  <dependency>
	<groupId>org.apache.cxf</groupId>
	<artifactId>cxf-rt-transports-http</artifactId>
	<version>3.0.3</version>
  </dependency>
        
  <dependency>
	<groupId>org.springframework</groupId>
	<artifactId>spring-core</artifactId>
	<version>3.2.0.RELEASE</version>
  </dependency>

  <dependency>
	<groupId>org.springframework</groupId>
	<artifactId>spring-context</artifactId>
	<version>3.2.0.RELEASE</version>
  </dependency>

  <dependency>
	<groupId>org.springframework</groupId>
	<artifactId>spring-web</artifactId>
	<version>3.2.0.RELEASE</version>
  </dependency>
</dependencies>
```


