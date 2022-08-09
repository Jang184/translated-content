---
title: Document.forms
slug: Web/API/Document/forms
translation_of: Web/API/Document/forms
---
<div>{{APIRef("DOM")}}</div>

<p><code>forms</code> 屬性會回傳一個包含目前頁面中所有 {{HTMLElement("form")}} 元素的集合物件（型別為 {{domxref("HTMLCollection")}}）。</p>

<h2 id="Syntax">語法</h2>

<pre class="syntaxbox"><var>collection</var> = document.forms;</pre>

<h2 id="Example">範例：取得表單資訊</h2>

<pre class="brush:html">&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;

&lt;head&gt;
&lt;title&gt;document.forms example&lt;/title&gt;
&lt;/head&gt;

&lt;body&gt;

&lt;form id="robby"&gt;
  &lt;input type="button" onclick="alert(document.forms[0].id);" value="robby's form" /&gt;
&lt;/form&gt;

&lt;form id="dave"&gt;
  &lt;input type="button" onclick="alert(document.forms[1].id);" value="dave's form" /&gt;
&lt;/form&gt;

&lt;form id="paul"&gt;
  &lt;input type="button" onclick="alert(document.forms[2].id);" value="paul's form" /&gt;
&lt;/form&gt;

&lt;/body&gt;
&lt;/html&gt;
</pre>

<h2 id="範例_2：取得表單內的元素">範例 2：取得表單內的元素</h2>

<pre class="brush: js">var selectForm = document.forms[index];
var selectFormElement = document.forms[index].elements[index];
</pre>

<h2 id="Specifications">規範</h2>

{{Specifications}}

<h2 id="See_Also">參見</h2>

<ul>
 <li>{{domxref("HTMLFormElement")}}</li>
</ul>