---
layout: post
title: Java Web Service
comments: true
description: Java Web Service
keywords: dummy content
published: true
---
### SOAP

SOAP(Single Object Access Protocal) 為兩平台交換資料的標準協定，主要為 XML 的形式，Server 和 Client 之間彼此使用XML 的訊息來互相溝通。一個基本的 web service 架構至少要有兩種元件:

* Client
* Server

![ws_intro_01.png](/assets/images/post_images/ws_intro_01.png)

Client 要能夠與服務供應者(Service provider)溝通的話，Client 就得知道以下資訊:

* 服務供應者的 Server 位於哪裡
* 該 Service 提供了哪些的功能(functions)，以及這些 function 以何種形式回傳
* 溝通的協定為何
* 輸入及輸出的格式是什麼

服務供應者會產出一個標準的 XML file，裡頭包含了以上資訊的條件，如果這個檔案提供給 Client ，Client 就可以與 Web Service 溝通了，此 XML 檔被稱為 WSDL。


### WSDL

WSDL(Web Service Description Language) 為一個描述如何在技術上實作 web service 的詳細資訊 XML 的檔案，更詳細的說就是 URI，port，方法名稱，需要用到的引數以及資料種類等。既然為一個 XML 檔，代表人可以看得懂，電腦也能夠讀，透過 WSDL 檔我們可以知道以下資訊:

* Port / Endpoint –  web service 的 URL
* 輸入/輸出訊息的格式
* 需要遵守的安全協定
* web service 使用了那些協定


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
