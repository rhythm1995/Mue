<template><section><h2 id="breadcrumb-mian-bao-xie"><a class="header-anchor" href="#breadcrumb-mian-bao-xie" aria-hidden="true">¶</a> Breadcrumb 面包屑</h2>
<p>在一个带有层次的导航结构中标明当前页面的位置，并可返回上级</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;breadcrumb&gt;\n  &lt;breadcrumb-item label=\&quot;Home\&quot; to=\&quot;/#\&quot;&gt;&lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;Component\&quot; to=\&quot;#/components\&quot;&gt;&lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;breadcrumb\&quot; to=\&quot;#/components/breadcrumb\&quot;&gt;&lt;/breadcrumb-item&gt;\n&lt;/breadcrumb&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><breadcrumb>
  <breadcrumb-item label="Home" to="/#"></breadcrumb-item>
  <breadcrumb-item label="Component" to="#/components"></breadcrumb-item>
  <breadcrumb-item label="breadcrumb" to="#/components/breadcrumb"></breadcrumb-item>
</breadcrumb>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>最基本的用法</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Home"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/#"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Component"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components/breadcrumb"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 最基本的用法
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Home"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/#"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Component"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components/breadcrumb"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;breadcrumb separator=\&quot;-\&quot;&gt;\n  &lt;breadcrumb-item label=\&quot;Home\&quot; to=\&quot;/#\&quot;&gt;&lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;Component\&quot; to=\&quot;#/components\&quot;&gt;&lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;breadcrumb\&quot; to=\&quot;#/components/breadcrumb\&quot;&gt;&lt;/breadcrumb-item&gt;\n&lt;/breadcrumb&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><breadcrumb separator="-">
  <breadcrumb-item label="Home" to="/#"></breadcrumb-item>
  <breadcrumb-item label="Component" to="#/components"></breadcrumb-item>
  <breadcrumb-item label="breadcrumb" to="#/components/breadcrumb"></breadcrumb-item>
</breadcrumb>
</div>
                    <div slot="description"><h4 id="fen-ge-fu"><a class="header-anchor" href="#fen-ge-fu" aria-hidden="true">¶</a> 分隔符</h4>
<ul>
<li>可通过设置<code>separator</code> 自定义分隔符</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span> <span class="hljs-attr">separator</span>=<span class="hljs-string">"-"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Home"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/#"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Component"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components/breadcrumb"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 分隔符
  * 可通过设置`separator` 自定义分隔符
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span> <span class="hljs-attr">separator</span>=<span class="hljs-string">"-"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Home"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/#"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Component"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components/breadcrumb"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;breadcrumb&gt;\n  &lt;breadcrumb-item&gt;\n    &lt;router-link to=\&quot;/\&quot; exact&gt;&lt;i class=\&quot;fa fa-home\&quot;&gt;&lt;/i&gt;Home&lt;/router-link&gt;\n  &lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item&gt;\n    &lt;router-link to=\&quot;/components/tag\&quot; exact&gt;&lt;i class=\&quot;fa fa-tag\&quot;&gt;&lt;/i&gt;Tag标签&lt;/router-link&gt;\n  &lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;breadcrumb\&quot;&gt;\n    &lt;select&gt;\n      &lt;option&gt;请选择&lt;/option&gt;\n      &lt;option&gt;山东省&lt;/option&gt;\n      &lt;option&gt;北京市&lt;/option&gt;\n    &lt;/select&gt;\n  &lt;/breadcrumb-item&gt;\n&lt;/breadcrumb&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><breadcrumb>
  <breadcrumb-item>
    <router-link to="/" exact=""><i class="fa fa-home"></i>Home</router-link>
  </breadcrumb-item>
  <breadcrumb-item>
    <router-link to="/components/tag" exact=""><i class="fa fa-tag"></i>Tag标签</router-link>
  </breadcrumb-item>
  <breadcrumb-item label="breadcrumb">
    <select>
      <option>请选择</option>
      <option>山东省</option>
      <option>北京市</option>
    </select>
  </breadcrumb-item>
</breadcrumb>
</div>
                    <div slot="description"><h4 id="lian-jie-nei-rong"><a class="header-anchor" href="#lian-jie-nei-rong" aria-hidden="true">¶</a> 链接内容</h4>
<ul>
<li>可自定义链接内容</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Home<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/tag"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-tag"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Tag标签<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>请选择<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>山东省<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>北京市<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 链接内容
  * 可自定义链接内容
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Home<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/tag"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-tag"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Tag标签<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>请选择<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>山东省<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>北京市<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="breadcrumb"><a class="header-anchor" href="#breadcrumb" aria-hidden="true">¶</a> breadcrumb</h4>
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
<td>separator</td>
<td>分隔符，默认值<code>&gt;</code></td>
<td>String</td>
<td><code>&gt;</code></td>
</tr>
</tbody>
</table>
<h4 id="breadcrumb-item"><a class="header-anchor" href="#breadcrumb-item" aria-hidden="true">¶</a> breadcrumb-item</h4>
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
<td>to</td>
<td>链接地址，在不设置内容时有效</td>
<td>String</td>
<td>无</td>
</tr>
</tbody>
</table>
</section></template>

