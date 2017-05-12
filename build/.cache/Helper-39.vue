<template><section><h2 id="helper"><a class="header-anchor" href="#helper" aria-hidden="true">¶</a> Helper</h2>
<p>Vue-Blu's style library uses Bulma -- a new,Flexbox based,modern pure css framework.With a powerful layout feature and
rich style settings.As we can easily write pages with bootstrap,with Bulma will greatly reduce the front end in the style
and layout of the workload.Even,bulma in this respect will do better than bootstrap.Vue-Blu based on bulma, can be said
to have a congenital advantage.Use Blu can not only have a rich Vue components can also use Bulma to bring the layout
and style of convenience.</p>
<p>The following will be related to the basic functions of Bulma, color, etc. to do some introduction.</p>
<h3 id="helpers"><a class="header-anchor" href="#helpers" aria-hidden="true">¶</a> Helpers</h3>
<table>
<thead>
<tr>
<th>Properties</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>is-clearfix</code></td>
<td>Fixes an element's floating children</td>
</tr>
<tr>
<td><code>is-pulled-left</code></td>
<td>Moves an element to the left(float:left)</td>
</tr>
<tr>
<td><code>is-pulled-right</code></td>
<td>Moves an element to the right(float:right)</td>
</tr>
<tr>
<td><code>is-overlay</code></td>
<td>Completely covers the first positioned parent</td>
</tr>
<tr>
<td><code>is-fullwidth</code></td>
<td>Takes up the whole width (100%)</td>
</tr>
<tr>
<td><code>has-text-centered</code></td>
<td>Centers the text</td>
</tr>
<tr>
<td><code>has-text-left</code></td>
<td>Text is left-aligned</td>
</tr>
<tr>
<td><code>has-text-right</code></td>
<td>Text is right-aligned</td>
</tr>
<tr>
<td><code>is-disabled</code></td>
<td>Removes any click event</td>
</tr>
<tr>
<td><code>is-marginless</code></td>
<td>Removes any margin</td>
</tr>
<tr>
<td><code>is-paddingless</code></td>
<td>Removes any padding</td>
</tr>
<tr>
<td><code>is-unselectable</code></td>
<td>Prevents the text from being selectable</td>
</tr>
</tbody>
</table>
<h3 id="colors"><a class="header-anchor" href="#colors" aria-hidden="true">¶</a> Colors</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;p class=\&quot;notification is-primary\&quot;&gt;is-primary&lt;/p&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;p class=\&quot;notification is-info\&quot;&gt;is-info&lt;/p&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;p class=\&quot;notification is-success\&quot;&gt;is-success&lt;/p&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;p class=\&quot;notification is-warning\&quot;&gt;is-warning&lt;/p&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;p class=\&quot;notification is-danger\&quot;&gt;is-danger&lt;/p&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column">
    <p class="notification is-primary">is-primary</p>
  </div>
  <div class="column">
    <p class="notification is-info">is-info</p>
  </div>
  <div class="column">
    <p class="notification is-success">is-success</p>
  </div>
  <div class="column">
    <p class="notification is-warning">is-warning</p>
  </div>
  <div class="column">
    <p class="notification is-danger">is-danger</p>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="colors"><a class="header-anchor" href="#colors" aria-hidden="true">¶</a> Colors</h4>
<ul>
<li>Five primary colors <code>is-primary</code> <code>is-info</code> <code>is-success</code> <code>is-warning</code> <code>is-danger</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-primary"</span>&gt;</span>is-primary<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-info"</span>&gt;</span>is-info<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-success"</span>&gt;</span>is-success<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-warning"</span>&gt;</span>is-warning<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-danger"</span>&gt;</span>is-danger<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Colors
  * Five primary colors `is-primary` `is-info` `is-success` `is-warning` `is-danger`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-primary"</span>&gt;</span>is-primary<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-info"</span>&gt;</span>is-info<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-success"</span>&gt;</span>is-success<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-warning"</span>&gt;</span>is-warning<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"notification is-danger"</span>&gt;</span>is-danger<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="more-detail"><a class="header-anchor" href="#more-detail" aria-hidden="true">¶</a> More detail</h3>
<p><code>Note：</code> For more information: <a href="http://bulma.io/documentation/overview/start/">Bulma Documentation</a></p>
</section></template>

