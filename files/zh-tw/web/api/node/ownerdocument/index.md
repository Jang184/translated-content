---
title: Node.ownerDocument
slug: Web/API/Node/ownerDocument
translation_of: Web/API/Node/ownerDocument
---
<div>{{APIRef("DOM")}}</div>

<p><code><strong>Node.ownerDocument</strong></code> 唯讀屬性會回傳一個此節點所屬的的頂層 <code>document</code> 物件。</p>

<h2 id="語法">語法</h2>

<pre class="syntaxbox"><var>document</var> = <var>element</var>.ownerDocument
</pre>

<ul>
 <li><code>document</code> is the {{domxref("Document", "document")}} object parent of the current element.</li>
</ul>

<h2 id="範例">範例</h2>

<pre class="brush:js">// given a node "p", get the top-level HTML child
// of the document object

var d = p.ownerDocument;
var html = d.documentElement;
</pre>

<h2 id="備註">備註</h2>

<p>The <code>document</code> object returned by this property is the main object with which all the child nodes in the actual HTML document are created. If this property is used on a node that is itself a document, the result is <code>null</code>.</p>

<h2 id="規範">規範</h2>

{{Specifications}}

<h2 id="瀏覽器相容性">瀏覽器相容性</h2>

{{Compat("api.Node.ownerDocument")}}