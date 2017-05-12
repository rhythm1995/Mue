<template><section><h2 id="tabs-biao-qian-ye"><a class="header-anchor" href="#tabs-biao-qian-ye" aria-hidden="true">¶</a> Tabs 标签页</h2>
<p>选项卡切换，常用于内容的收纳和展现</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs type=\&quot;boxed\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs type=\&quot;toggle\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column">
    <tabs>
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>

  <div class="column">
    <tabs type="boxed">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>
</div>

<div class="columns">
  <div class="column">
    <tabs type="toggle">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>三种样式，默认 <code>boxed</code> <code>toggle</code></li>
<li>通过 <code>slot</code> 设置内容</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"boxed"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"toggle"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 三种样式，默认 `boxed` `toggle`
  * 通过 `slot` 设置内容
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"boxed"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"toggle"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="yang-shi-he-tu-biao"><a class="header-anchor" href="#yang-shi-he-tu-biao" aria-hidden="true">¶</a> 样式和图标</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs type=\&quot;toggle\&quot; :is-full-width=\&quot;true\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot; icon=\&quot;image\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot; icon=\&quot;music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot; icon=\&quot;film\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot; icon=\&quot;file-text-o\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&lt;hr&gt;\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs size=\&quot;small\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs alignment=\&quot;centered\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column">
    <tabs type="toggle" :is-full-width="true">
      <tab-item label="Pictures" icon="image">Pictures Tab</tab-item>
      <tab-item label="Music" icon="music">Music Tab</tab-item>
      <tab-item label="Videos" icon="film">Video Tab</tab-item>
      <tab-item label="Documents" icon="file-text-o">Document Tab2</tab-item>
    </tabs>
  </div>
</div>
<hr>
<div class="columns">
  <div class="column">
    <tabs size="small">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>
  <div class="column">
    <tabs alignment="centered">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>
</div>

</div>
                    <div slot="description"><h4 id="yang-shi"><a class="header-anchor" href="#yang-shi" aria-hidden="true">¶</a> 样式</h4>
<ul>
<li>通过 <code>is-full-width</code> 设置是否占满一行</li>
<li>通过 <code>size</code> 设置tab的大小</li>
<li>通过 <code>alignment</code> 设置对齐方式 <code>right</code> <code>left</code> <code>centered</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">:is-full-width</span>=<span class="hljs-string">"true"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"image"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"film"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"file-text-o"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">alignment</span>=<span class="hljs-string">"centered"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 样式
  * 通过 `is-full-width` 设置是否占满一行
  * 通过 `size` 设置tab的大小
  * 通过 `alignment` 设置对齐方式 `right` `left` `centered`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">:is-full-width</span>=<span class="hljs-string">"true"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"image"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"film"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"file-text-o"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">alignment</span>=<span class="hljs-string">"centered"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

</code></pre>
</demo-box>
<h3 id="bu-ju"><a class="header-anchor" href="#bu-ju" aria-hidden="true">¶</a> 布局</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs layout=\&quot;left\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs layout=\&quot;right\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Document\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&lt;hr&gt;\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs layout=\&quot;bottom\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column">
    <tabs layout="left">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>

  <div class="column">
    <tabs layout="right">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Document">Document Tab2</tab-item>
    </tabs>
  </div>
</div>
<hr>
<div class="columns">
  <div class="column">
    <tabs layout="bottom">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>
</div>

</div>
                    <div slot="description"><h4 id="bu-ju"><a class="header-anchor" href="#bu-ju" aria-hidden="true">¶</a> 布局</h4>
<ul>
<li>通过 <code>layout</code> 设置布局，可选值有 <code>left / right / bottom / top</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"right"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Document"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"bottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 布局
  * 通过 `layout` 设置布局，可选值有 `left / right / bottom / top`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"right"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Document"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"bottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

</code></pre>
</demo-box>
<h3 id="ji-huo-jin-yong-he-hui-diao"><a class="header-anchor" href="#ji-huo-jin-yong-he-hui-diao" aria-hidden="true">¶</a> 激活、禁用和回调</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs :active-index=\&quot;2\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot; disabled&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Document\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&lt;hr&gt;\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column\&quot;&gt;\n    &lt;tabs :on-tab-click=\&quot;tabCallback\&quot;&gt;\n      &lt;tab-item label=\&quot;Pictures\&quot;&gt;Pictures Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Music\&quot;&gt;Music Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Videos\&quot;&gt;Video Tab&lt;/tab-item&gt;\n      &lt;tab-item label=\&quot;Documents\&quot;&gt;Document Tab2&lt;/tab-item&gt;\n    &lt;/tabs&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column">
    <tabs :active-index="2">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>

  <div class="column">
    <tabs>
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music" disabled>Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Document">Document Tab2</tab-item>
    </tabs>
  </div>
</div>
<hr>
<div class="columns">
  <div class="column">
    <tabs :on-tab-click="tabCallback">
      <tab-item label="Pictures">Pictures Tab</tab-item>
      <tab-item label="Music">Music Tab</tab-item>
      <tab-item label="Videos">Video Tab</tab-item>
      <tab-item label="Documents">Document Tab2</tab-item>
    </tabs>
  </div>
</div>

</div>
                    <div slot="description"><h4 id="ji-huo-jin-yong-he-hui-diao"><a class="header-anchor" href="#ji-huo-jin-yong-he-hui-diao" aria-hidden="true">¶</a> 激活、禁用和回调</h4>
<ul>
<li>通过 <code>active-index</code> 设置默认打开第几个选项卡</li>
<li>通过 <code>disabled</code> 禁用某个选项卡</li>
<li>通过 <code>on-tab-click</code> 设置回调</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">:active-index</span>=<span class="hljs-string">"2"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span> <span class="hljs-attr">disabled</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Document"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">:on-tab-click</span>=<span class="hljs-string">"tabCallback"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 激活、禁用和回调
  * 通过 `active-index` 设置默认打开第几个选项卡
  * 通过 `disabled` 禁用某个选项卡
  * 通过 `on-tab-click` 设置回调
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">:active-index</span>=<span class="hljs-string">"2"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span> <span class="hljs-attr">disabled</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Document"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">hr</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tabs</span> <span class="hljs-attr">:on-tab-click</span>=<span class="hljs-string">"tabCallback"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Pictures"</span>&gt;</span>Pictures Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Music"</span>&gt;</span>Music Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Videos"</span>&gt;</span>Video Tab<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">tab-item</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Documents"</span>&gt;</span>Document Tab2<span class="hljs-tag">&lt;/<span class="hljs-name">tab-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tabs</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="tabs"><a class="header-anchor" href="#tabs" aria-hidden="true">¶</a> Tabs</h4>
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
<td>type</td>
<td>tab样式类型，可选值有 <code>boxed / toggle</code> 和默认</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>is-full-width</td>
<td>是否铺满整行</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>layout</td>
<td>布局，可选值有 <code>left / right / bottom / top</code></td>
<td>String</td>
<td>top</td>
</tr>
<tr>
<td>size</td>
<td>tab大小，可选值为<code>small / large</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>alignment</td>
<td>对齐方式 可选值为<code>left / right</code></td>
<td>String</td>
<td>left</td>
</tr>
<tr>
<td>active-index</td>
<td>初始打开tab的index(从0开始计数)</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>on-tab-click</td>
<td>标签切换时的回调</td>
<td>Function</td>
<td>无</td>
</tr>
</tbody>
</table>
<h4 id="tabitem"><a class="header-anchor" href="#tabitem" aria-hidden="true">¶</a> TabItem</h4>
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
<td>icon</td>
<td>图标</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>label</td>
<td>tab标签标题</td>
<td>String(<code>required</code>)</td>
<td>无</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    tabCallback(index) {
      this.$notify.info({
        content: `打开了第 ${index + 1} 个tab`,
      });
    },
  },
};
</script>