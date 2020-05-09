
<a href="/CSS/">CSS</a> >>
<a href="/CSS/Headings_Paragraphs_Links/">Headings/Paragraphs/Links</a> >>
<a href="/CSS/flexbox/" style="color:palevioletred;background-color:papayawhip;">List</a> >>
<a href="/CSS/???/">???</a> >>
<a href="/CSS/???/">???</a> >>
<div class="divider"></div>

### 關於 FlexBox...

利用css 的 float、inline-block、position:absolute 等方式有時無法完全滿足現代許多網頁的複雜 RWD 版面設計/配置，而且他們最原先
的設計也並非為了該目的而生，flexible box layout 提供了一些 css 的屬性讓我們可以有彈性的設置網頁的版面。

<div class="divider"></div>

### FlexBox 的重要元素

**Flex containers**

1. Sets the context for the flexbox layout

2. Contains flex items, the actual elements you layout using flexbox

3. Can be any block-level or inline element

**Flex items**

1. Every direct child of a flex container

2. There can be any number of flex items in the flex container

![CSS](CSS_images/flexbox_container_example.png)

**Flexbox Axes**

1. Main axis

2. Cross Axis

![CSS](CSS_images/flexbox_container_axis1.png)

![CSS](CSS_images/flexbox_container_axis2.png)


```
<!DOCTYPE CSS>
<CSS>
<head>
</head>
<body>
   <ul>
     <li>item1</li>
     <li>item2</li>
     <li>item3</li>
     <li>item4</li>
   </ul>
</body>
</CSS>
```
結果 : 
<CSS>
<head>
</head>
<body>
   <ul>
     <li>item1</li>
     <li>item2</li>
     <li>item3</li>
     <li>item4</li>
   </ul>
</body>
</CSS>

<div class="divider"></div>

### &lt;ol&gt;

```
<!DOCTYPE CSS>
<CSS>
<head>
</head>
<body>
   <ol>
     <li>item1</li>
     <li>item2</li>
     <li>item3</li>
     <li>item4</li>
   </ol>
</body>
</CSS>
```
結果 : 
<CSS>
<head>
</head>
<body>
   <ol>
     1.item1<br>
     2.item2<br>
     3.item3<br>
     4.item4<br>
   </ol>
</body>
</CSS>

<div class="divider"></div>
參考資料:

1: **<a href="https://css-tricks.com/snippets/css/a-guide-to-flexbox/" target="_blank">A Complete Guide to Flexbox</a>**

2: **<a href="https://scotch.io/tutorials/a-visual-guide-to-css3-flexbox-properties" target="_blank">A Visual Guide to CSS3 Flexbox Properties</a>**

3: **<a href="https://demos.scotch.io/visual-guide-to-css3-flexbox-flexbox-playground/demos/" target="_blank">Flexbox Playground</a>**

4: **<a href="https://caniuse.com/#search=flexbox" target="_blank">Flexbox - latest browser support</a>**

