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


### el
當看到 Vue Instance 裡有定義 `el` 這樣的東西，表示這個 el 目前指到你網頁的哪一個 template，假設說 el 對應到一個 id 為 element 的元素，
如果你有在你的 html 網頁中給予某一個元素該 element 的 Id，那這個 Vue 的實例裡被定義出的所有物件和行為都會去與該元素進行同步的變化。


### data
data 為該 Vue Instance 底下物件的被賦予的屬性，當需要用到時，可拿這些屬性提供給你的 template，網頁就會識別出該資料屬性並正確的表示它所代表的值。

範例:

如果我的 html 網頁有一個 div 元素，id 是 element，我的 {% raw %}{{title}}{% endraw %} 就會被 data 裡所定義的 title : "abc" 給取代。

Vue template
```
<div id="element">
    <h1>{% raw %}{{title}}{% endraw %}</h1>
</div>
```

Vue Instance
```
new Vue({
   el: '#element',
   data: {
     title: "abc"
  }
});
```

