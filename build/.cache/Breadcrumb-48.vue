<template><section><h2 id="breadcrumb"><a class="header-anchor" href="#breadcrumb" aria-hidden="true">¶</a> Breadcrumb</h2>
<p>A breadcrumb displays the current location within a hierarchy. It allows going back to states higher up in the hierarchy.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;breadcrumb&gt;\n  &lt;breadcrumb-item label=\&quot;Home\&quot; to=\&quot;/#\&quot;&gt;&lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;Component\&quot; to=\&quot;#/components\&quot;&gt;&lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;breadcrumb\&quot; to=\&quot;#/components/breadcrumb\&quot;&gt;&lt;/breadcrumb-item&gt;\n&lt;/breadcrumb&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><breadcrumb>
  <breadcrumb-item label="Home" to="/#"></breadcrumb-item>
  <breadcrumb-item label="Component" to="#/components"></breadcrumb-item>
  <breadcrumb-item label="breadcrumb" to="#/components/breadcrumb"></breadcrumb-item>
</breadcrumb>
</div>
                    <div slot="description"><h4 id="basic-usage"><a class="header-anchor" href="#basic-usage" aria-hidden="true">¶</a> Basic Usage</h4>
<ul>
<li>The simplest use</li>
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
  #### Basic Usage
  * The simplest use
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
                    <div slot="description"><h4 id="separator"><a class="header-anchor" href="#separator" aria-hidden="true">¶</a> Separator</h4>
<ul>
<li>Customized the separator by setting the <code>separator</code> property</li>
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
  #### Separator
  * Customized the separator by setting the `separator` property
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span> <span class="hljs-attr">separator</span>=<span class="hljs-string">"-"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Home"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/#"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Component"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"#/components/breadcrumb"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;breadcrumb&gt;\n  &lt;breadcrumb-item&gt;\n    &lt;router-link to=\&quot;/\&quot; exact&gt;&lt;i class=\&quot;fa fa-home\&quot;&gt;&lt;/i&gt;Home&lt;/router-link&gt;\n  &lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item&gt;\n    &lt;router-link to=\&quot;/components/tag\&quot; exact&gt;&lt;i class=\&quot;fa fa-tag\&quot;&gt;&lt;/i&gt;Tags&lt;/router-link&gt;\n  &lt;/breadcrumb-item&gt;\n  &lt;breadcrumb-item label=\&quot;breadcrumb\&quot;&gt;\n    &lt;select&gt;\n      &lt;option&gt;Please Select&lt;/option&gt;\n      &lt;option&gt;NY&lt;/option&gt;\n      &lt;option&gt;LA&lt;/option&gt;\n    &lt;/select&gt;\n  &lt;/breadcrumb-item&gt;\n&lt;/breadcrumb&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><breadcrumb>
  <breadcrumb-item>
    <router-link to="/" exact=""><i class="fa fa-home"></i>Home</router-link>
  </breadcrumb-item>
  <breadcrumb-item>
    <router-link to="/components/tag" exact=""><i class="fa fa-tag"></i>Tags</router-link>
  </breadcrumb-item>
  <breadcrumb-item label="breadcrumb">
    <select>
      <option>Please Select</option>
      <option>NY</option>
      <option>LA</option>
    </select>
  </breadcrumb-item>
</breadcrumb>
</div>
                    <div slot="description"><h4 id="link"><a class="header-anchor" href="#link" aria-hidden="true">¶</a> link</h4>
<ul>
<li>Sets link address by the <code>to</code> param</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Home<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/tag"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-tag"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Tags<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>Please Select<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>NY<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>LA<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### link
  * Sets link address by the `to` param
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-home"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Home<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">router-link</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/tag"</span> <span class="hljs-attr">exact</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-tag"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>Tags<span class="hljs-tag">&lt;/<span class="hljs-name">router-link</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">breadcrumb-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"breadcrumb"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>Please Select<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>NY<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>LA<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">breadcrumb</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="breadcrumb-2"><a class="header-anchor" href="#breadcrumb-2" aria-hidden="true">¶</a> breadcrumb</h4>
<table>
<thead>
<tr>
<th>Members</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>separator</td>
<td>separator，default: <code>&gt;</code></td>
<td>String</td>
<td><code>&gt;</code></td>
</tr>
</tbody>
</table>
<h4 id="breadcrumb-item"><a class="header-anchor" href="#breadcrumb-item" aria-hidden="true">¶</a> breadcrumb-item</h4>
<table>
<thead>
<tr>
<th>Members</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>to</td>
<td>link address</td>
<td>String</td>
<td>-</td>
</tr>
</tbody>
</table>
</section></template>

