---
title: Vue 實例
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
<a href="/vue/vue_page1/">Vue 簡介</a> >>
<a href="/vue/vue_page2/" style="color:palevioletred;background-color:papayawhip;">Vue 實例</a> >>
<a href="/vue/vue_page3/">Vue 模組語法</a> >>
<div class="divider"></div>

### Vue 實例(Instance)

```
var vm = new Vue({
  // options
})
```
變數命名為 vm( ViewModel 簡稱) 跟  MVVM pattern 有些關系，因 Vue 的設計靈感來自它，但這不是重點。

當你宣告了一個 Vue 的實例後，你會在裡面賦予該 Instance 你想要的物件或方法，這些物件跟方法可以達到你想要你網頁呈現的樣貌及行為。

用 `new Vue` 所建立出來的 Instance 視為 root Vue instance，也就是 Vue 的"根"，而根底下所衍伸出來的分支就是你所定義的各種物件和方法。 

> 參考資料(英文) **<a href="https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93viewmodel" target="_blank"> MVVM pattern</a>**


### Data
一個 Vue 模組通常由 HTML 以及資料綁定(data-binding)組成。可藉由該模組定義Vue應該如何呈現你的資料。

Vue Template 範例 :
```
<div id="element">
  <h1>{{ property1 }}</h1>
  <h2>{{ property2 }}</h2>
  <p> {{ property3 }} </p>
</div>
```

### Data Binding

資料綁定通常指應用程式的資料與應用程式的使用者介面(UI)做一個連繫(connection)， Vue 會確保我們在Vue instance 定義的資料會跟 Vue template 保持同步的狀態。

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

