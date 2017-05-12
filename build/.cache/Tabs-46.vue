<template><section><h2 id="tabs"><a class="header-anchor" href="#tabs" aria-hidden="true">¶</a> Tabs</h2>
<p>Tabs make it easy to switch between different views.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
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
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Three styles，<code>boxed</code> <code>toggle</code> and default</li>
<li>Setting content by <code>slot</code></li>
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
  #### Basic
  * Three styles，`boxed` `toggle` and default
  * Setting content by `slot`
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
<h3 id="styles-and-icon"><a class="header-anchor" href="#styles-and-icon" aria-hidden="true">¶</a> Styles and Icon</h3>
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
                    <div slot="description"><h4 id="styles"><a class="header-anchor" href="#styles" aria-hidden="true">¶</a> styles</h4>
<ul>
<li>The tab can be set to take up the whole width</li>
<li>There are 3 sizes of tab: <code>small</code> <code>large</code> and default</li>
<li><code>alignment</code>: <code>right</code> <code>left</code> <code>centered</code></li>
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
  #### styles
  * The tab can be set to take up the whole width
  * There are 3 sizes of tab: `small` `large` and default
  * `alignment`: `right` `left` `centered`
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
<h3 id="layout"><a class="header-anchor" href="#layout" aria-hidden="true">¶</a> Layout</h3>
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
                    <div slot="description"><h4 id="layout"><a class="header-anchor" href="#layout" aria-hidden="true">¶</a> layout</h4>
<ul>
<li>Position of tabs，accepted value: <code>left / right / bottom / top</code></li>
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
  #### layout
  * Position of tabs，accepted value: `left / right / bottom / top`
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
<h3 id="active-disabled-and-callback"><a class="header-anchor" href="#active-disabled-and-callback" aria-hidden="true">¶</a> Active,Disabled and Callback</h3>
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
                    <div slot="description"><h4 id="advanced"><a class="header-anchor" href="#advanced" aria-hidden="true">¶</a> advanced</h4>
<ul>
<li>Sets default actived tabItem's key by <code>active-index</code></li>
<li>TabItem can be disabled</li>
<li>Sets callback when tab is clicked by <code>on-tab-click</code></li>
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
  #### advanced
  * Sets default actived tabItem's key by `active-index`
  * TabItem can be disabled
  * Sets callback when tab is clicked by `on-tab-click`
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
<h4 id="tabs-2"><a class="header-anchor" href="#tabs-2" aria-hidden="true">¶</a> Tabs</h4>
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
<td>different style of tab，accepted value: <code>boxed / toggle</code> and default</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>is-full-width</td>
<td>whether the tab takes up the whole width (100%)</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>layout</td>
<td>Position of tabs，accepted value: <code>left / right / bottom / top</code></td>
<td>String</td>
<td>top</td>
</tr>
<tr>
<td>size</td>
<td>size of tab，accepted value: <code>small / large</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>alignment</td>
<td>alignment accepted value:<code>left / right</code></td>
<td>String</td>
<td>left</td>
</tr>
<tr>
<td>active-index</td>
<td>default actived tabItem's key(count from 0)</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>on-tab-click</td>
<td>Callback when tab is switched</td>
<td>Function</td>
<td>-</td>
</tr>
</tbody>
</table>
<h4 id="tabitem"><a class="header-anchor" href="#tabitem" aria-hidden="true">¶</a> TabItem</h4>
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
<td>icon</td>
<td>icon of tab item</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>label</td>
<td>title of tab item</td>
<td>String(<code>required</code>)</td>
<td>-</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    tabCallback(index) {
      this.$notify.info({
        content: `opening index: ${index + 1} `,
      });
    },
  },
};
</script>