---
title: Network Information API
slug: Web/API/Network_Information_API
translation_of: Web/API/Network_Information_API
---
<p>{{ SeeCompatTable() }}</p>
<p>Network Information API 將提供系統連線的相關資訊，如使用者裝置的現有頻寬，或目前的連線狀態。根據使用者的連線情形，可進一步選擇高解析度或低解析度的內容。此完整的 API 另包含 domxref("Connection") 介面，以及 <a href="/en-US/docs/Web/API/Navigator"><code>Navigator</code></a> 介面的單一屬性 ─ <a href="/en-US/docs/Web/API/Navigator.connection"><code>Navigator.connection</code></a>。</p>
<h2 id="偵測連線變化">偵測連線變化</h2>
<p>此範例將觀察使用者連線的變化。舉例來說，當使用者從高價位連線轉用低價位連線時，就會降低頻寬需求以避免連線費用暴增，並採用類似 Apps 受到警示的方法。</p>
<pre class="brush: js">var connection = navigator.connection || navigator.mozConnection || navigator.webkitConnection;

function updateConnectionStatus() {
  alert("Connection bandwidth: " + connection.bandwidth + " MB/s");
  if (connection.metered) {
    alert("The connection is metered!");
  }
}

connection.addEventListener("change", updateConnectionStatus);
updateConnectionStatus();
</pre>

<h2 id="Specifications">規範</h2>

{{Specifications}}

{{Specifications("api.Navigator.connection")}}

<h2 id="瀏覽器相容性">瀏覽器相容性</h2>

<h3 id="networkinformation">NetworkInformation</h3>

{{Compat}}

<h3 id="navigator.connection">Navigator.connection</h3>

{{Compat("api.Navigator.connection")}}

<h2 id="See_also">See also</h2>
<ul>
  <li><a href="http://dvcs.w3.org/hg/dap/raw-file/tip/network-api/Overview.html">Network Information API Specification</a></li>
  <li><a href="/en/Online_and_offline_events">線上與離線事件</a></li>
  <li>{{domxref("window.navigator.connection")}}</li>
</ul>