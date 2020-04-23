
<a href="/HTML/">HTML</a> >>
<a href="/HTML/Headings_Paragraphs_Links/">Headings/Paragraphs/Links</a> >>
<a href="/HTML/List/">List</a> >>
<a href="/HTML/Semantic_HTML_1/" style="color:palevioletred;background-color:papayawhip;">Semantic HTML </a> >>
<a href="/HTML/Files_Images/">Files/Images</a> >>
<div class="divider"></div>

> **Semantic HTML**<br/>
  markup that describes the *meaning* of content instead of how it looks.

### In HTML there are some semantic elements that can be used to define different parts of a web page:

* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header" target="_blank">&lt;header&gt;</a>** - header : an element that represents a group of introductory content ,usually contains the site name and main menu etc
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer" target="_blank">&lt;footer&gt;</a>** - footer : an element that typically contains information about the site, copyright data or related links
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/section" target="_blank">&lt;section&gt;</a>** - section : an element that represents standalone sections of content
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/article" target="_blank">&lt;article&gt;</a>** - article : content that can be syndicated
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav" target="_blank">&lt;nav&gt;</a>** - nav : an element that represents a major section of navigation
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/aside" target="_blank">&lt;aside&gt;</a>** - aside : an element that represents a section of content that's indirectly related to the main content of the page
* **<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/main" target="_blank">&lt;main&gt;</a>** - main : an element that represents the main content of the &lt;body&gt; of the page(normally not including &lt;aside&gt; inside &lt;main&gt;)

<div class="divider"></div>

### Example

```
<!DOCTYPE html>
<html>
<head>
</head>
<body>
  <header style="background-color:pink;">
    <h1>News About Covid-19</h1>
    <nav style="background-color:lightcyan;">
      <ul>
        <li>Home</li>
        <li>News</li>
        <li>About</li>
        <li>Contact</li>
      </ul>
    </nav>
   </header>
   <main style="background-color:brown;>
   <section style="background-color:teal;">
     <h2>Recent News</h2>
     <article style="background-color:yellow;">
     <h4>2020-04-22 News update on covid-19</h4>
     <p>On April 22, the Central Epidemic Command Center (CECC) reported that 1,389 additional cases related to coronavirus disease 2019 (COVID-19) were reported on April 21. As of writing, a cumulative total of 56,853 cases have been reported among which COVID-19 has been ruled out in 53,676. Of these reported cases, infection with COVID-19 was laboratory-confirmed in 426 cases (Case #426 confirmed today). Of 426 confirmed cases in Taiwan, 343 are imported and 55 are indigenous while 28 are Navy members on the Dunmu Fleet. Of the confirmed cases, there have been 6 deaths, and 236 patients have been released from isolation, with the remainder remaining hospitalized in isolation.</p>
     </article>
     <article style="background-color:yellow;">
     <h4>2020-04-21 News update on covid-19</h4>
     <p>On April 21, the Central Epidemic Command Center (CECC) reported that 1,853 additional cases related to coronavirus disease 2019 (COVID-19) were reported on April 20. As of writing, a cumulative total of 55,476 cases have been reported among which COVID-19 has been ruled out in 52,150. Of these reported cases, infection with COVID-19 was laboratory-confirmed in 425 cases (Cases #423-425 confirmed today). Of 425 confirmed cases in Taiwan, 343 are imported and 55 are indigenous while 27 are Navy members on the Dunmu (敦睦) Fleet. Of the confirmed cases, there have been 6 deaths, and 217 patients have been released from isolation, with the remainder remaining hospitalized in isolation.</p>
   </article>
   </section>
   <section style="background-color:gray;">
     <h2>About</h2>
     <p>In recent years, with dramatic increases in international exchange and travel and the number of foreign laborers, various communicable diseases have been imported. Facing the threat of emerging diseases and the recurrence of indigenous communicable diseases, the existing policies on disease prevention, quarantine, and surveillance, and the capabilities of laboratory testing and research are considered inadequate to meet the needs of disease control. In coordination with the rapid development in high technology and the trend of internationalization, disease control must be more comprehensive, prompt, effective and international. The goal of the Centers for Disease Control, therefore, is to combat the threat of communicable diseases.</p>
   </section>
   </main>
   <aside style="background-color:blue;">
     <h2>Learn more about COVID-19</h2>
     <ul>
         <li>Introduction</li>
         <li>Known hosts</li>
         <li>Transmission</li>
       </ul>
   </aside>
   <footer style="background-color:green;">
   Copyright © 2019 Taiwan Centers for Disease Control. All rights reserved.
   </footer>
</body>
</html>
```
Result : 
<html>
<head>
</head>
<body>
   <header style="background-color:pink;">
     <h1>News About Covid-19</h1>
     <nav style="background-color:lightcyan;">
       <ul>
         <li>Home</li>
         <li>News</li>
         <li>About</li>
         <li>Contact</li>
       </ul>
     </nav>
   </header>
   <main style="background-color:brown;">
   <section style="background-color:teal;">
     <h2>Recent News</h2>
     <article style="background-color:yellow;">
     <h4>2020-04-22 News update on covid-19</h4>
     <p>On April 22, the Central Epidemic Command Center (CECC) reported that 1,389 additional cases related to coronavirus disease 2019 (COVID-19) were reported on April 21. As of writing, a cumulative total of 56,853 cases have been reported among which COVID-19 has been ruled out in 53,676. Of these reported cases, infection with COVID-19 was laboratory-confirmed in 426 cases (Case #426 confirmed today). Of 426 confirmed cases in Taiwan, 343 are imported and 55 are indigenous while 28 are Navy members on the Dunmu Fleet. Of the confirmed cases, there have been 6 deaths, and 236 patients have been released from isolation, with the remainder remaining hospitalized in isolation.</p>
     </article>
     <article style="background-color:yellow;">
     <h4>2020-04-21 News update on covid-19</h4>
     <p>On April 21, the Central Epidemic Command Center (CECC) reported that 1,853 additional cases related to coronavirus disease 2019 (COVID-19) were reported on April 20. As of writing, a cumulative total of 55,476 cases have been reported among which COVID-19 has been ruled out in 52,150. Of these reported cases, infection with COVID-19 was laboratory-confirmed in 425 cases (Cases #423-425 confirmed today). Of 425 confirmed cases in Taiwan, 343 are imported and 55 are indigenous while 27 are Navy members on the Dunmu (敦睦) Fleet. Of the confirmed cases, there have been 6 deaths, and 217 patients have been released from isolation, with the remainder remaining hospitalized in isolation.</p>
   </article>
   </section>
   <section style="background-color:gray;">
     <h2>About</h2>
     <p>In recent years, with dramatic increases in international exchange and travel and the number of foreign laborers, various communicable diseases have been imported. Facing the threat of emerging diseases and the recurrence of indigenous communicable diseases, the existing policies on disease prevention, quarantine, and surveillance, and the capabilities of laboratory testing and research are considered inadequate to meet the needs of disease control. In coordination with the rapid development in high technology and the trend of internationalization, disease control must be more comprehensive, prompt, effective and international. The goal of the Centers for Disease Control, therefore, is to combat the threat of communicable diseases.</p>
   </section>
   </main>
   <aside style="background-color:blue;">
     <h2>Learn more about COVID-19</h2>
     <ul>
         <li>Introduction</li>
         <li>Known hosts</li>
         <li>Transmission</li>
       </ul>
   </aside>
   <footer style="background-color:green;">
   Copyright © 2019 Taiwan Centers for Disease Control. All rights reserved.
   </footer>
</body>
</html>

<div class="divider"></div>

參考資料:

1: **<a href="https://developer.mozilla.org/en-US/docs/Glossary/Semantics" target="_blank">Semantics – MDN</a>**
