---
title: Vue 簡介
description: >-
  Automate your task for sending email notification with PowerShell script and
  Windows SMTP Client.
keywords: >-
  software build automation, send email notification, using smtp client in
  powershell, software build notification
tags:
  - VueJS
comments: true
published: true
---

<a href="/vue/">Vue</a> >>
<a href="/vue/vue_page1/" style="color:palevioletred;background-color:papayawhip;">Vue 簡介</a> >>
<a href="/vue/vue_page2/">JSX</a> >>
<div class="divider"></div>

### Vue.js

Vue (pronounced /vjuː/, like view) is a progressive framework for building user interfaces. Unlike other monolithic frameworks, Vue is designed from the ground up to be incrementally adoptable. The core library is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects. On the other hand, Vue is also perfectly capable of powering sophisticated Single-Page Applications when used in combination with modern tooling and supporting libraries.

### Vue 物件(Instance)
為Vue應用的根源，以 `new` 這個 keyword 來建立。 可以把一個含有資料的物件或方法傳給這個Vue的物件。一旦交付給Vue物件之後，此物件就可以被Vue的模組(Template)用來展現出你在Vue物件所定義出的行為。

Vue Instance 範例 :
```
new Vue({
   el: '#element',
   data: {
     property1: "abc", 
     property2: 123,
     property3: "Hello, welcome to Vue!" 
  }
});
```

> 參考資料(英文) **<a href="https://tylermcginnis.com/imperative-vs-declarative-programming/" target="_blank"> Vue object</a>**


### Vue 模組化(Template)
一個Vue模組通常由HTML以及資料綁定(data-binding)組成。可藉由該模組定義Vue應該如何呈現你的資料。

Vue Template 範例 :
```
<div id="element">
  <h1>{{ property1 }}</h1>
  <h2>{{ property2 }}</h2>
  <p> {{ property3 }} </p>
</div>
```

### Data Binding

資料綁定通常指應用程式的資料與應用程式的使用者介面(UI)做一個連繫(connection)，Vue會確保我們在Vue instance定義的資料會跟Vue template保持同步的狀態。

以下為簡單的 Hello World 例子來說明Vue如何運作:
```
<!DOCTYPE html>
<html lang="en">
    <head>
	<meta charset="UTF-8" />
	<title>Hello World</title>
	<script src="https://cdn.jsdelivr.net/npm/vue@2.5.16/dist/vue.js"></script>
    </head>
    <body>
	<div id="helloWorld">
	    <h1>{% raw %}{{title}}{% endraw %}</h1>
	</div>
	<script type="text/javascript">
	    var helloWorld = new Vue({
		    el:'#helloWorld',
		    data:{
		        title:"Hello, world!"
		    }
		});
	</script>
    </body>
</html>
```

---
<div class="pagenation_center">
  <div  class="pagenation_center_inner">
  |<a class="pagenation_link" href="react/"> 上一頁</a> |
   <a class="pagenation_link" href="/react/react_page2"> 下一頁 </a> |
  </div>
</div>
