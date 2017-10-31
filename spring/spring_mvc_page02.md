<a href="/spring/">Spring</a> >>
<a href="/spring/spring_page1/">Spring 簡介</a> >>
<a href="/spring/spring_page2/">Spring Container</a> >> <a href="/spring/spring_page3/">Spring Beans</a> >> <a href="/spring/spring_page4/">Dependency Injection</a>

<a href="/spring/spring_mvc_page01/">Spring MVC介紹</a> >> 
<a href="/spring/spring_mvc_page02/" style="color:palevioletred;background-color:papayawhip;">Controllers</a>

<div class="divider"></div>
### Controllers
在 src 目錄下加入一個新的 package 並建立一個 Class 叫作 TestController :

```
package com.example.controller;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;

@Controller
public class TestController{
	@RequestMapping(value="/TestController/test")
	public void test(){
		System.out.println("hi!");
	}
}
```

在 `DispatcherServlet-servlet.xml` 修改成以下程式 : 

```
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xmlns:context="http://www.springframework.org/schema/context"
	xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

	<context:component-scan base-package="com.example.controller" />
	
</beans>
```
在 WebContent 下可以建立一個 index.jsp 檔加入以下程式:
```
<html>
<head>
<title>Insert title here</title>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<script src="https://code.jquery.com/jquery-1.9.1.js"></script>
<script src="https://code.jquery.com/ui/1.10.3/jquery-ui.js"></script> 
<script>
$(document).ready(function(){
	$('#btn').click(function(){
		var json = JSON.stringify($('#input').val());
		$.ajax({
			url:'<%=request.getContextPath()%>/TestController/test.do',
			async : true,
			type : 'post',
			data : {
				"string" : json
			}
		});
	});
});
</script>
</head>

<body>
	<h2>MVC test</h2>
	<input id="input" type="text" />
	<button id="btn">click me</button>
</body>
</html>
```
<!--![Spring](spring_images/springoverview01.png)-->
