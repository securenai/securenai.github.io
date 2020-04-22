
<a href="/HTML/">HTML</a> >>
<a href="/HTML/Headings_Paragraphs_Links/">Headings/Paragraphs/Links</a> >>
<a href="/HTML/List/">List</a> >>
<a href="/HTML/Semantic_HTML_1/" style="color:palevioletred;background-color:papayawhip;">Semantic HTML 1</a> >>
<a href="/HTML/Semantic_HTML_2/">Semantic HTML 2</a> >>
<div class="divider"></div>

### &lt;header&gt;、&lt;footer&gt; and &lt;section&gt;

* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header" target="_blank">&lt;header&gt;</a>** - header
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer" target="_blank">&lt;footer&gt;</a>** - footer
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/section" target="_blank">&lt;section&gt;</a>** - section

<div class="divider"></div>

### &lt;header&gt;、&lt;section&gt;、&lt;footer&gt;

```
<!DOCTYPE html>
<html>
<head>
</head>
<body>
  <header style="background-color:pink;">
    <h1>News About Covid-19</h1>
    <ul>
       <li>Home</li>
       <li>News</li>
       <li>About</li>
       <li>Contact</li>
     </ul>
   </header>
   <section style="background-color:yellow;">
     <p>On April 21, the Central Epidemic Command Center (CECC) reported that 1,853 additional cases related to coronavirus disease 2019 (COVID-19) were reported on April 20. As of writing, a cumulative total of 55,476 cases have been reported among which COVID-19 has been ruled out in 52,150. Of these reported cases, infection with COVID-19 was laboratory-confirmed in 425 cases (Cases #423-425 confirmed today). Of 425 confirmed cases in Taiwan, 343 are imported and 55 are indigenous while 27 are Navy members on the Dunmu (敦睦) Fleet. Of the confirmed cases, there have been 6 deaths, and 217 patients have been released from isolation, with the remainder remaining hospitalized in isolation.</p>
   </section>
   <footer style="background-color:green;">
   ©copy 2020 world health organization
   </footer>
</body>
</html>
```
結果 : 
<html>
<head>
</head>
<body>
   <header style="background-color:pink;">
    <h1>News About Covid-19</h1>
    <ul>
       <li>Home</li>
       <li>News</li>
       <li>About</li>
       <li>Contact</li>
     </ul>
   </header>
   <section style="background-color:gray;">
     <p></p>
   </section>
   <section style="background-color:yellow;">
     <p>On April 21, the Central Epidemic Command Center (CECC) reported that 1,853 additional cases related to coronavirus disease 2019 (COVID-19) were reported on April 20. As of writing, a cumulative total of 55,476 cases have been reported among which COVID-19 has been ruled out in 52,150. Of these reported cases, infection with COVID-19 was laboratory-confirmed in 425 cases (Cases #423-425 confirmed today). Of 425 confirmed cases in Taiwan, 343 are imported and 55 are indigenous while 27 are Navy members on the Dunmu (敦睦) Fleet. Of the confirmed cases, there have been 6 deaths, and 217 patients have been released from isolation, with the remainder remaining hospitalized in isolation.</p>
   </section>
   <footer style="background-color:green;">
   ©copy 2020 world health organization
   </footer>
</body>
</html>

<div class="divider"></div>

參考資料:

1: **<a href="https://developer.mozilla.org/en-US/docs/Glossary/Semantics" target="_blank">Semantics – MDN</a>**
