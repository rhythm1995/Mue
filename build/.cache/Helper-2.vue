<template><section><h2 id="helper-bang-zhu-shuo-ming"><a class="header-anchor" href="#helper-bang-zhu-shuo-ming" aria-hidden="true">¶</a> Helper 帮助说明</h2>
<p>Vue-Blu的样式库采用了bulma —— 一套新兴的、基于<strong>Flexbox</strong>、现代化的纯css框架。有着强大的布局功能和丰富的样式设定。就像大家可以在bootstrap上轻松写页面一样，
有了bulma将会大大减轻前端在样式和布局方面的工作量。甚至，bulma在这方面会比bootstrap做的更好。基于bulma构筑的Vue-Blu，可以说有了一个先天的优势。
使用blu不仅可以拥有丰富的Vue组件还可以使用bulma带来的布局和样式上的便利。</p>
<p>基于上面所述，Blu的有些基本组件并没有vue化，而是原生的html、css。其实我们并不主张过度'组件化'，像layout、button之类的元素，原生已经有了足够的表达力，
组件化之后反而会降低效率和灵活性。下面将对bulma的相关基础功能、颜色等做些介绍。</p>
<h3 id="bang-zhu-lei"><a class="header-anchor" href="#bang-zhu-lei" aria-hidden="true">¶</a> 帮助类</h3>
<table>
<thead>
<tr>
<th>成员</th>
<th>说明</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>is-clearfix</code></td>
<td>清除浮动</td>
</tr>
<tr>
<td><code>is-pulled-left</code></td>
<td>左浮动 即float:left</td>
</tr>
<tr>
<td><code>is-pulled-right</code></td>
<td>右浮动 即float:right</td>
</tr>
<tr>
<td><code>is-overlay</code></td>
<td>完全覆盖父层</td>
</tr>
<tr>
<td><code>is-fullwidth</code></td>
<td>占据全部宽度</td>
</tr>
<tr>
<td><code>has-text-centered</code></td>
<td>文字居中</td>
</tr>
<tr>
<td><code>has-text-left</code></td>
<td>文字居左</td>
</tr>
<tr>
<td><code>has-text-right</code></td>
<td>文字居右</td>
</tr>
<tr>
<td><code>is-disabled</code></td>
<td>禁止click事件</td>
</tr>
<tr>
<td><code>is-marginless</code></td>
<td>去除margin</td>
</tr>
<tr>
<td><code>is-paddingless</code></td>
<td>去除padding</td>
</tr>
<tr>
<td><code>is-unselectable</code></td>
<td>禁止文字被选中</td>
</tr>
</tbody>
</table>
<h3 id="yan-se"><a class="header-anchor" href="#yan-se" aria-hidden="true">¶</a> 颜色</h3>
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
                    <div slot="description"><h4 id="zhu-yao-yan-se"><a class="header-anchor" href="#zhu-yao-yan-se" aria-hidden="true">¶</a> 主要颜色</h4>
<ul>
<li>五种主要颜色 <code>is-primary</code> <code>is-info</code> <code>is-success</code> <code>is-warning</code> <code>is-danger</code></li>
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
  #### 主要颜色
  * 五种主要颜色 `is-primary` `is-info` `is-success` `is-warning` `is-danger`
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
<h3 id="geng-duo-shuo-ming"><a class="header-anchor" href="#geng-duo-shuo-ming" aria-hidden="true">¶</a> 更多说明</h3>
<p><code>注：</code> 更多说明请见 <a href="http://bulma.io/documentation/overview/start/">Bulma Documentation</a></p>
</section></template>

