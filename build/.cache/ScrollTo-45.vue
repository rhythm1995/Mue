<template><section><h2 id="scrollto"><a class="header-anchor" href="#scrollto" aria-hidden="true">¶</a> ScrollTo</h2>
<p>Scroll to a specific position smoothly,base on <a href="https://github.com/callmecavs/jump.js">jump.js</a></p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;scroll-to target=\&quot;#t2\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot; id=\&quot;t1\&quot;&gt;I'm t1，Scroll to `#t2` element&lt;/button&gt;\n&lt;/scroll-to&gt;\n\n&lt;scroll-to :distance=\&quot;500\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Scroll down 500px&lt;/button&gt;\n&lt;/scroll-to&gt;\n\n&lt;div style=\&quot;width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd\&quot;&gt;Long div&lt;/div&gt;\n&lt;scroll-to target=\&quot;#t1\&quot;&gt;\n  &lt;button class=\&quot;button is-outlined\&quot; id=\&quot;t2\&quot;&gt;I'm t2，scroll back to t1&lt;/button&gt;\n&lt;/scroll-to&gt;\n&lt;scroll-to :distance=\&quot;-500\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Scroll up 500px&lt;/button&gt;\n&lt;/scroll-to&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><scroll-to target="#t2">
  <button class="button is-primary" id="t1">I'm t1，Scroll to `#t2` element</button>
</scroll-to>

<scroll-to :distance="500">
  <button class="button is-primary">Scroll down 500px</button>
</scroll-to>

<div style="width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd">Long div</div>
<scroll-to target="#t1">
  <button class="button is-outlined" id="t2">I'm t2，scroll back to t1</button>
</scroll-to>
<scroll-to :distance="-500">
  <button class="button is-primary">Scroll up 500px</button>
</scroll-to>
</div>
                    <div slot="description"><h4 id="basic-usage"><a class="header-anchor" href="#basic-usage" aria-hidden="true">¶</a> Basic usage</h4>
<ul>
<li>Sets <code>target</code> to scroll to an element, by passing a css selector like <code>'.target' '#id1'</code></li>
<li>When setting <code>target='top'</code>, it will trigger the built-in <code>scrollTop</code>(an arrow button shows at the lower right corner of the page)</li>
<li>Scroll from the current position by passing a number of pixels(use <code>distance</code> parameter.positive scroll down,negative scroll up).</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t2"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t1"</span>&gt;</span>I'm t1，Scroll to `#t2` element<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Scroll down 500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd"</span>&gt;</span>Long div<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-outlined"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t2"</span>&gt;</span>I'm t2，scroll back to t1<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"-500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Scroll up 500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Basic usage
  * Sets `target` to scroll to an element, by passing a css selector like `'.target' '#id1'`
  * When setting `target='top'`, it will trigger the built-in `scrollTop`(an arrow button shows at the lower right corner of the page)
  * Scroll from the current position by passing a number of pixels(use `distance` parameter.positive scroll down,negative scroll up).
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t2"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t1"</span>&gt;</span>I'm t1，Scroll to `#t2` element<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Scroll down 500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd"</span>&gt;</span>Long div<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-outlined"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t2"</span>&gt;</span>I'm t2，scroll back to t1<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"-500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Scroll up 500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<table>
<thead>
<tr>
<th>Properties</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>target</td>
<td>target element，can be any css selector，like <code>'.target' '#id1'</code>.When setting <code>target='top'</code>, it will trigger the built-in <code>scrollTop</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>duration</td>
<td>Pass the time the scroll takes, in milliseconds</td>
<td>Number</td>
<td>500</td>
</tr>
<tr>
<td>distance</td>
<td>scroll distance(Higher priority than target,positive scroll down,negative scroll up)</td>
<td>Number</td>
<td>-</td>
</tr>
</tbody>
</table>
<div style="width: 200px;height: 1000px;margin: 10px; "></div>
</section></template>

