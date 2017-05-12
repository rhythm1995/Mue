<template><section><h2 id="collapse-zhe-die-mian-ban"><a class="header-anchor" href="#collapse-zhe-die-mian-ban" aria-hidden="true">¶</a> Collapse 折叠面板</h2>
<p>可折叠展开的内容区域</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
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
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>通过<code>accordion</code>设置是否同时只能展开一个面板</li>
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
  #### 基本
  * 通过`accordion`设置是否同时只能展开一个面板
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
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>同时打开多个面板</li>
<li>支持嵌套面板</li>
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
  #### 基本
  * 同时打开多个面板
  * 支持嵌套面板
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
<h4 id="collapse"><a class="header-anchor" href="#collapse" aria-hidden="true">¶</a> Collapse</h4>
<table>
<thead>
<tr>
<th>成员</th>
<th>说明</th>
<th>类型</th>
<th>默认值</th>
</tr>
</thead>
<tbody>
<tr>
<td>accordion</td>
<td>手风琴模式，即同时只能展开一个面板</td>
<td>Boolean</td>
<td>false</td>
</tr>
</tbody>
</table>
<h4 id="collapseitem"><a class="header-anchor" href="#collapseitem" aria-hidden="true">¶</a> CollapseItem</h4>
<table>
<thead>
<tr>
<th>成员</th>
<th>说明</th>
<th>类型</th>
<th>默认值</th>
</tr>
</thead>
<tbody>
<tr>
<td>title</td>
<td>面板标题</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>actived</td>
<td>是否展开</td>
<td>Boolean</td>
<td>false</td>
</tr>
</tbody>
</table>
</section></template>

