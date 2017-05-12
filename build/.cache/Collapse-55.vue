<template><section><h2 id="collapse"><a class="header-anchor" href="#collapse" aria-hidden="true">¶</a> Collapse</h2>
<p>A content area which can be collapsed and expanded.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;collapse accordion&gt;\n  &lt;collapse-item title=\&quot;Collapsible Group Item #1\&quot;&gt;Lorem ipsum dolor sit amet, consectetur\n    adipiscing elit lorem ipsum dolor sit amet,\n    consectetur adipiscing elit&lt;/collapse-item&gt;\n  &lt;collapse-item title=\&quot;Collapsible Group Item #2\&quot; actived&gt;Lorem ipsum dolor sit amet, consectetur\n    adipiscing elit lorem ipsum dolor sit amet,\n    consectetur adipiscing elit&lt;/collapse-item&gt;\n  &lt;collapse-item title=\&quot;Collapsible Group Item #3\&quot;&gt;Lorem ipsum dolor sit amet, consectetur\n    adipiscing elit lorem ipsum dolor sit amet,\n    consectetur adipiscing elit&lt;/collapse-item&gt;\n&lt;/collapse&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><collapse accordion="">
  <collapse-item title="Collapsible Group Item #1">Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit</collapse-item>
  <collapse-item title="Collapsible Group Item #2" actived="">Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit</collapse-item>
  <collapse-item title="Collapsible Group Item #3">Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit</collapse-item>
</collapse>

</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Accordion mode, only one panel can be expanded at a time.</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">collapse</span> <span class="hljs-attr">accordion</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #1"</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #2"</span> <span class="hljs-attr">actived</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #3"</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">collapse</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Basic
  * Accordion mode, only one panel can be expanded at a time.
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">collapse</span> <span class="hljs-attr">accordion</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #1"</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #2"</span> <span class="hljs-attr">actived</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #3"</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">collapse</span>&gt;</span>

</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;collapse&gt;\n  &lt;collapse-item title=\&quot;Collapsible Group Item #1\&quot;&gt;\n    Lorem ipsum dolor sit amet, consectetur adipiscing elit lorem ipsum dolor sit amet,\n    consectetur adipiscing elit&lt;/collapse-item&gt;\n  &lt;collapse-item title=\&quot;Collapsible Group Item #2\&quot; actived&gt;\n    &lt;collapse&gt;\n      &lt;collapse-item title=\&quot;Sub Collapse #1\&quot;&gt;Sub Collapse #1&lt;/collapse-item&gt;\n      &lt;collapse-item title=\&quot;Sub Collapse #2\&quot;&gt;Sub Collapse #2&lt;/collapse-item&gt;\n    &lt;/collapse&gt;\n  &lt;/collapse-item&gt;\n  &lt;collapse-item title=\&quot;Collapsible Group Item #3\&quot; actived&gt;Lorem ipsum dolor sit amet, consectetur\n    adipiscing elit lorem ipsum dolor sit amet,\n    consectetur adipiscing elit&lt;/collapse-item&gt;\n&lt;/collapse&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><collapse>
  <collapse-item title="Collapsible Group Item #1">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit</collapse-item>
  <collapse-item title="Collapsible Group Item #2" actived="">
    <collapse>
      <collapse-item title="Sub Collapse #1">Sub Collapse #1</collapse-item>
      <collapse-item title="Sub Collapse #2">Sub Collapse #2</collapse-item>
    </collapse>
  </collapse-item>
  <collapse-item title="Collapsible Group Item #3" actived="">Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit</collapse-item>
</collapse>
</div>
                    <div slot="description"><h4 id="advanced"><a class="header-anchor" href="#advanced" aria-hidden="true">¶</a> Advanced</h4>
<ul>
<li>open multiple panels</li>
<li>Collapse is nested inside the Collapse</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">collapse</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #1"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #2"</span> <span class="hljs-attr">actived</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">collapse</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Sub Collapse #1"</span>&gt;</span>Sub Collapse #1<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Sub Collapse #2"</span>&gt;</span>Sub Collapse #2<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">collapse</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #3"</span> <span class="hljs-attr">actived</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">collapse</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Advanced
  * open multiple panels
  * Collapse is nested inside the Collapse
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">collapse</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #1"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #2"</span> <span class="hljs-attr">actived</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">collapse</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Sub Collapse #1"</span>&gt;</span>Sub Collapse #1<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Sub Collapse #2"</span>&gt;</span>Sub Collapse #2<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">collapse</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">collapse-item</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Collapsible Group Item #3"</span> <span class="hljs-attr">actived</span>&gt;</span>Lorem ipsum dolor sit amet, consectetur
    adipiscing elit lorem ipsum dolor sit amet,
    consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">collapse-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">collapse</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="collapse-2"><a class="header-anchor" href="#collapse-2" aria-hidden="true">¶</a> Collapse</h4>
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
<td>accordion</td>
<td>Accordion mode, only one panel can be expanded at a time</td>
<td>Boolean</td>
<td>false</td>
</tr>
</tbody>
</table>
<h4 id="collapseitem"><a class="header-anchor" href="#collapseitem" aria-hidden="true">¶</a> CollapseItem</h4>
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
<td>title</td>
<td>title of the panel</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>actived</td>
<td>whether the panel is active</td>
<td>Boolean</td>
<td>false</td>
</tr>
</tbody>
</table>
</section></template>

