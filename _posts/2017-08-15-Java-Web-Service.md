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

![ws_intro_01.png](/assets/images/post_images/ws/ws_intro_01.png)

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

Client 需要以上資訊方能使用 web service，因此只要 web service 提供 WSDL 給 Client，就可以讓 Client 使用 web service 了。

### 利用 eclipse 建立 SOAP web service

開啟 eclipse 建立一個 dynamic web 專案:

步驟 : [new] --> [Dynamic Web Project]

![ws_soapws_01.png](/assets/images/post_images/ws/ws_soapws_01.png)

在該專案下的 src 裡 建立一個 package:(參考如下)

![ws_soapws_02.png](/assets/images/post_images/ws/ws_soapws_02.png)

在 package 下建立一個新的 Class 為 `HelloWorld.java`

```
package com.securenai.webservice;

public class HelloWorld {
	
	public String sayHelloWorld(String name){
		return "Hello World " + name;
	}
}
```
接下來再專案裡 new 一個 web service 的專案

![ws_soapws_03.png](/assets/images/post_images/ws/ws_soapws_03.png)

123

![ws_soapws_04.png](/assets/images/post_images/ws/ws_soapws_04.png)

### 利用 eclipse 建立 JAX-WS web service


