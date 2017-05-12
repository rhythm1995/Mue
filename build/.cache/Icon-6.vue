<template><section><h2 id="icon-tu-biao-ku"><a class="header-anchor" href="#icon-tu-biao-ku" aria-hidden="true">¶</a> Icon 图标库</h2>
<p>Vue-Blu的图标库采用了被广泛使用的 <a href="http://fontawesome.io/">Fontawesome</a>。图标库没有写成Vue组件的形式，通过原生标签即可调用</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;span class=\&quot;icon is-small\&quot;&gt;\n  &lt;i class=\&quot;fa fa-home\&quot;&gt;&lt;/i&gt;\n&lt;/span&gt;\n&lt;span class=\&quot;icon\&quot;&gt;\n  &lt;i class=\&quot;fa fa-home\&quot;&gt;&lt;/i&gt;\n&lt;/span&gt;\n&lt;span class=\&quot;icon is-medium\&quot;&gt;\n  &lt;i class=\&quot;fa fa-home\&quot;&gt;&lt;/i&gt;\n&lt;/span&gt;\n&lt;span class=\&quot;icon is-large\&quot;&gt;\n  &lt;i class=\&quot;fa fa-home\&quot;&gt;&lt;/i&gt;\n&lt;/span&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><span class="icon is-small">
  <i class="fa fa-home"></i>
</span>
<span class="icon">
  <i class="fa fa-home"></i>
</span>
<span class="icon is-medium">
  <i class="fa fa-home"></i>
</span>
<span class="icon is-large">
  <i class="fa fa-home"></i>
</span>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>icon默认有四种大小，除了默认大小还包括<code>small</code> <code>medium</code> <code>large</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-medium"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-large"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * icon默认有四种大小，除了默认大小还包括`small` `medium` `large`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-medium"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-large"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="tu-biao-ku"><a class="header-anchor" href="#tu-biao-ku" aria-hidden="true">¶</a> 图标库</h3>
<p><icons></icons></p>

</section></template>

<script>
export default{

}
</script>