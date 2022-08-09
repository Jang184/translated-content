---
title: 後裔選擇器
slug: Web/CSS/Descendant_combinator
tags:
  - CSS
  - CSS參考
  - Selectors
  - 初學者
  - 選擇器
translation_of: Web/CSS/Descendant_combinator
---
<p>{{CSSRef("Selectors")}}</p>

<h2 id="Summary">簡介</h2>

<p><code>␣</code> 組合符號 (代表空白, 或更精準地說，代表一或多個空白字元) 結合了兩種選擇器，選擇了只有當第二個選擇器的目標為第一個選擇器目標的後裔時的元素，後裔選擇器跟<a href="/en/CSS/Child_selectors">子選擇器</a>相似，但是不要求披對的元素要是嚴格是父子關係。</p>

<h2 id="Syntax">語法</h2>

<pre class="eval">selector1 selector2 { <em>style properties</em> }
</pre>

<h2 id="Example">範例</h2>

<pre class="brush: css">span { background-color: white; }
div span { background-color: DodgerBlue; }
</pre>

<pre class="brush: html">&lt;div&gt;
  &lt;span&gt;Span 1.
    &lt;span&gt;Span 2.&lt;/span&gt;
  &lt;/span&gt;
&lt;/div&gt;
&lt;span&gt;Span 3.&lt;/span&gt;
</pre>

<p>{{ EmbedLiveSample('Example', 200, 50) }}</p>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

{{Compat("css.selectors.descendant")}}