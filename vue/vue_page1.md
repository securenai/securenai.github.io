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

### Vue
Vue...

> 參考資料(英文) **<a href="https://tylermcginnis.com/imperative-vs-declarative-programming/" target="_blank"> Imperative vs Declarative Programming</a>**


### 虛擬 DOM(Virtual DOM)
動態式網頁常常有動態產生或移除新的元素、或者部分重新整理的動作，這些動作會導致整個 DOM 的重新產出，比方說當我們在一個有20個項目的 list 裡加了1個項目，整個 list 會被重新產生，包含了那21個項目。
React 則是產生一個虛擬的 DOM 這個 DOM 假設也有一個 list，同樣的狀況下，假設增加了一個 item，React 則是很聰明去跟原來前一版的 DOM 比對，判斷說因為你只有增加一個 item，我在重新 render 時，就只 render 那新增的那個 item。

### 如何撰寫虛擬 DOM 元素

我們要如何在虛擬 DOM 裡形容一個 DOM 元素呢?
DOM 元素主要由三樣東西組成等
1. 名稱 : 形容該元素是甚麼類型，是 p，還是 a，還是 h1、div....等
2. 屬性 : 一組 key 跟 value 提供更多資訊像是 type、href....等
3. 內容 : 有些元素有，有些沒有，例 : `<p>hello</p>` 

簡單的 Hello World 例子
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
