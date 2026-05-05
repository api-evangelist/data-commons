---
title: "Recent improvements to the Resolve API"
url: "https://blog.datacommons.org/2026/02/10/recent-improvements-to-the-resolve-api/"
date: "Tue, 10 Feb 2026 21:20:15 +0000"
author: "Kara Moscoe"
feed_url: "https://blog.datacommons.org/feed/"
---
<p class="wp-block-paragraph">We are pleased to announce some major improvements to the <a href="https://docs.datacommons.org/api/rest/v2/resolve.html">Resolve V2 API</a>, which is used to programmatically look up DCIDs of knowledge graph entities. Up until today, you could only resolve place types and get limited metadata in the response. Now we&#8217;ve added several enhancements that support a much wider range of use cases:</p>



<ul class="wp-block-list">
<li>Support for resolving statistical variables and topics, which you can look up by description</li>



<li>Additional metadata, such as the confidence scores of the candidate results, available for variables and topics</li>



<li>Ability to limit results to either variable or topics exclusively by using the <code>typeOf</code> filter</li>



<li>For Custom Data Commons instances, ability to restrict the results to your own data if desired</li>
</ul>



<h2 class="wp-block-heading">Summary of API changes</h2>



<h3 class="wp-block-heading">New resolve parameters</h3>



<p class="wp-block-paragraph">Two new optional parameters are available for the <code>resolve</code> REST endpoint and <code>resolve.fetch</code> Python method:</p>



<ul class="wp-block-list">
<li><code>resolver</code>, which allows you to choose between places and indicators (variables and topics). If not set, it defaults to places.</li>



<li><code>target</code>, which allows Custom Data instance owners to choose the source of the data among custom, base, or custom+base</li>
</ul>



<p class="wp-block-paragraph"><strong>Examples:</strong></p>



<p class="wp-block-paragraph">REST:&nbsp;</p>


<div class="wp-block-code">
	<div class="cm-editor">
		<div class="cm-scroller">
			
<pre><code><div class="cm-line">https://api.datacommons.org/v2/resolve?key=...&amp;nodes=population&amp;resolver=indicator</div></code></pre>
		</div>
	</div>
</div>


<p class="wp-block-paragraph">  Python:&nbsp;</p>


<div class="wp-block-code">
	<div class="cm-editor">
		<div class="cm-scroller">
			
<pre><code><div class="cm-line">resolve.fetch(node_ids=&quot;population&quot;, resolver=&quot;indicator&quot;)</div></code></pre>
		</div>
	</div>
</div>


<h3 class="wp-block-heading">New Python method</h3>



<p class="wp-block-paragraph">A new Python convenience method, <code>resolve.fetch_indicators</code>, is available. It takes two parameters:</p>



<ul class="wp-block-list">
<li><code>queries </code>(required) </li>



<li><code>target</code> (optional)</li>
</ul>



<p class="wp-block-paragraph">Example:</p>


<div class="wp-block-code">
	<div class="cm-editor">
		<div class="cm-scroller">
			
<pre><code><div class="cm-line">resolve.fetch_indicators(queries=&quot;female population over 50&quot;)</div></code></pre>
		</div>
	</div>
</div>


<h3 class="wp-block-heading">New response metadata</h3>



<p class="wp-block-paragraph">A new metadata object is returned in the response for indicator resolutions, containing two fields:</p>



<ul class="wp-block-list">
<li><code>score</code> – the confidence score of the ranking of the candidate in the results </li>



<li><code>sentence</code> – the candidate&#8217;s description</li>
</ul>



<p class="wp-block-paragraph">Example:</p>


<div class="wp-block-code">
	<div class="cm-editor">
		<div class="cm-scroller">
			
<pre><code><div class="cm-line">&quot;metadata&quot;: {</div><div class="cm-line">   &quot;score&quot;: &quot;0.8982&quot;,</div><div class="cm-line">   &quot;sentence&quot;: &quot;population count&quot;</div><div class="cm-line">},</div></code></pre>
		</div>
	</div>
</div>


<h3 class="wp-block-heading">Default property for places</h3>



<p class="wp-block-paragraph">For simple place resolutions by description, you can omit the <code>property</code> (REST) or <code>expression</code> parameter (Python).</p>



<p class="wp-block-paragraph"> Examples:</p>



<p class="wp-block-paragraph"> REST:</p>


<div class="wp-block-code">
	<div class="cm-editor">
		<div class="cm-scroller">
			
<pre><code><div class="cm-line">https://api.datacommons.org/v2/resolve?key=...&amp;nodes=Georgia</div></code></pre>
		</div>
	</div>
</div>


<p class="wp-block-paragraph">  Python:</p>


<div class="wp-block-code">
	<div class="cm-editor">
		<div class="cm-scroller">
			
<pre><code><div class="cm-line">resolve.fetch(node_ids=&quot;Georgia&quot;)</div></code></pre>
		</div>
	</div>
</div>


<h2 class="wp-block-heading">Documentation and examples</h2>



<p class="wp-block-paragraph">For full details and examples, see the following pages:</p>



<ul class="wp-block-list">
<li>REST: <a href="https://docs.datacommons.org/api/rest/v2/resolve.html">v2/resolve</a></li>



<li>Python: <a href="https://docs.datacommons.org/api/python/v2/resolve.html">resolve</a></li>
</ul>
