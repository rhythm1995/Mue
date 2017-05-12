<template><section><h2 id="timeline"><a class="header-anchor" href="#timeline" aria-hidden="true">¶</a> Timeline</h2>
<p>Vertical display timeline.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;timeline&gt;\n  &lt;timeline-item date=\&quot;2 minutes ago\&quot; type=\&quot;primary\&quot;&gt;\n    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.\n  &lt;/timeline-item&gt;\n  &lt;timeline-item date=\&quot;Sat, 5 Mar\&quot; type=\&quot;primary\&quot;&gt;\n    &lt;p&gt;adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit&lt;/p&gt;\n  &lt;/timeline-item&gt;\n  &lt;timeline-item date=\&quot;Sun, 11 Feb\&quot; type=\&quot;success\&quot;&gt;\n    Call to customer Jacob and discuss the detail.\n  &lt;/timeline-item&gt;\n&lt;/timeline&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><timeline>
  <timeline-item date="2 minutes ago" type="primary">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  </timeline-item>
  <timeline-item date="Sat, 5 Mar" type="primary">
    <p>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
  </timeline-item>
  <timeline-item date="Sun, 11 Feb" type="success">
    Call to customer Jacob and discuss the detail.
  </timeline-item>
</timeline>
</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Sets date&amp;time by <code>date</code> parameter.</li>
<li>color of node，including <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code>.</li>
<li>Setting content by <code>slot</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Basic
  * Sets date&time by `date` parameter.
  * color of node，including `primary` `info` `success` `danger` `warning`.
  * Setting content by `slot`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;timeline&gt;\n  &lt;timeline-item date=\&quot;2 minutes ago\&quot; icon=\&quot;twitter\&quot; type=\&quot;primary\&quot;&gt;\n    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.\n  &lt;/timeline-item&gt;\n  &lt;timeline-item type=\&quot;primary\&quot; date=\&quot;Sat, 5 Mar\&quot;&gt;\n    &lt;p&gt;adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit&lt;/p&gt;\n    &lt;p&gt;&lt;a href&gt;news center&lt;/a&gt;&lt;/p&gt;\n    &lt;p&gt;&lt;img src=\&quot;https://pek3a.qingstor.com/warehouse1/c1.jpg\&quot;&gt;&lt;/p&gt;\n  &lt;/timeline-item&gt;\n  &lt;timeline-item date=\&quot;Sun, 11 Feb\&quot; icon=\&quot;wechat\&quot; type=\&quot;success\&quot;&gt;\n    Call to customer Jacob and discuss the detail.\n  &lt;/timeline-item&gt;\n&lt;/timeline&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><timeline>
  <timeline-item date="2 minutes ago" icon="twitter" type="primary">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  </timeline-item>
  <timeline-item type="primary" date="Sat, 5 Mar">
    <p>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
    <p><a href="">news center</a></p>
    <p><img src="https://pek3a.qingstor.com/warehouse1/c1.jpg"></p>
  </timeline-item>
  <timeline-item date="Sun, 11 Feb" icon="wechat" type="success">
    Call to customer Jacob and discuss the detail.
  </timeline-item>
</timeline>
</div>
                    <div slot="description"><h4 id="more-settings"><a class="header-anchor" href="#more-settings" aria-hidden="true">¶</a> More settings</h4>
<ul>
<li>Sets icon of timeline-item by <code>icon</code> parameter.</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"twitter"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">href</span>=<span class="hljs-string">""</span>&gt;</span>news center<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">img</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://pek3a.qingstor.com/warehouse1/c1.jpg"</span> /&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"wechat"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### More settings
  * Sets icon of timeline-item by `icon` parameter.
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"twitter"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">href</span>=<span class="hljs-string">""</span>&gt;</span>news center<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">img</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://pek3a.qingstor.com/warehouse1/c1.jpg"</span> /&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"wechat"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="timeline-item"><a class="header-anchor" href="#timeline-item" aria-hidden="true">¶</a> timeline-item</h4>
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
<td>type</td>
<td>color of node，accepted value: <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>date</td>
<td>date string (2 minutes ago, Sun, 11 Feb... etc)</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>icon</td>
<td>icon of timeline item</td>
<td>String</td>
<td>-</td>
</tr>
</tbody>
</table>
</section></template>

