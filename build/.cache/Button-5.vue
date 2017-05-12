<template><section><h2 id="button-an-niu"><a class="header-anchor" href="#button-an-niu" aria-hidden="true">¶</a> Button 按钮</h2>
<p>通过按钮触发一个操作/事件</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;a class=\&quot;button is-white\&quot;&gt;White&lt;/a&gt;\n&lt;a class=\&quot;button is-light\&quot;&gt;Light&lt;/a&gt;\n&lt;a class=\&quot;button is-dark\&quot;&gt;Dark&lt;/a&gt;\n&lt;a class=\&quot;button is-black\&quot;&gt;Black&lt;/a&gt;\n&lt;a class=\&quot;button is-link\&quot;&gt;Link&lt;/a&gt;\n&lt;br&gt;&lt;br&gt;\n\n&lt;a class=\&quot;button\&quot;&gt;Button&lt;/a&gt;\n&lt;a class=\&quot;button is-primary\&quot;&gt;Primary&lt;/a&gt;\n&lt;a class=\&quot;button is-info\&quot;&gt;Info&lt;/a&gt;\n&lt;a class=\&quot;button is-success\&quot;&gt;Success&lt;/a&gt;\n&lt;a class=\&quot;button is-warning\&quot;&gt;Warning&lt;/a&gt;\n&lt;a class=\&quot;button is-danger\&quot;&gt;Danger&lt;/a&gt;\n&lt;br&gt;&lt;br&gt;\n\n&lt;a class=\&quot;button is-small\&quot;&gt;Small&lt;/a&gt;\n&lt;a class=\&quot;button\&quot;&gt;Normal&lt;/a&gt;\n&lt;a class=\&quot;button is-medium\&quot;&gt;Medium&lt;/a&gt;\n&lt;a class=\&quot;button is-large\&quot;&gt;Large&lt;/a&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><a class="button is-white">White</a>
<a class="button is-light">Light</a>
<a class="button is-dark">Dark</a>
<a class="button is-black">Black</a>
<a class="button is-link">Link</a>
<br><br>

<a class="button">Button</a>
<a class="button is-primary">Primary</a>
<a class="button is-info">Info</a>
<a class="button is-success">Success</a>
<a class="button is-warning">Warning</a>
<a class="button is-danger">Danger</a>
<br><br>

<a class="button is-small">Small</a>
<a class="button">Normal</a>
<a class="button is-medium">Medium</a>
<a class="button is-large">Large</a>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>六种色调 除了default还包括<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></li>
<li>四种大小，除了默认大小还包括<code>small</code> <code>medium</code> <code>large</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-white"</span>&gt;</span>White<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-light"</span>&gt;</span>Light<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-dark"</span>&gt;</span>Dark<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-black"</span>&gt;</span>Black<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-link"</span>&gt;</span>Link<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>Button<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Primary<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>Info<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span>&gt;</span>Success<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span>&gt;</span>Warning<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span>&gt;</span>Danger<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-small"</span>&gt;</span>Small<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>Normal<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-medium"</span>&gt;</span>Medium<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-large"</span>&gt;</span>Large<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 六种色调 除了default还包括`primary` `info` `success` `danger` `warning`
  * 四种大小，除了默认大小还包括`small` `medium` `large`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-white"</span>&gt;</span>White<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-light"</span>&gt;</span>Light<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-dark"</span>&gt;</span>Dark<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-black"</span>&gt;</span>Black<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-link"</span>&gt;</span>Link<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>Button<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Primary<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>Info<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span>&gt;</span>Success<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span>&gt;</span>Warning<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span>&gt;</span>Danger<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-small"</span>&gt;</span>Small<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>Normal<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-medium"</span>&gt;</span>Medium<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-large"</span>&gt;</span>Large<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="bu-tong-style"><a class="header-anchor" href="#bu-tong-style" aria-hidden="true">¶</a> 不同Style</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;a class=\&quot;button is-outlined\&quot;&gt;Outlined&lt;/a&gt;\n&lt;a class=\&quot;button is-primary is-outlined\&quot;&gt;Outlined&lt;/a&gt;\n&lt;a class=\&quot;button is-info is-outlined\&quot;&gt;Outlined&lt;/a&gt;\n&lt;a class=\&quot;button is-success is-outlined\&quot;&gt;Outlined&lt;/a&gt;\n&lt;a class=\&quot;button is-danger is-outlined\&quot;&gt;Outlined&lt;/a&gt;\n&lt;br&gt;&lt;br&gt;\n\n&lt;a class=\&quot;button is-primary is-inverted\&quot;&gt;Inverted&lt;/a&gt;\n&lt;a class=\&quot;button is-info is-inverted\&quot;&gt;Inverted&lt;/a&gt;\n&lt;a class=\&quot;button is-success is-inverted\&quot;&gt;Inverted&lt;/a&gt;\n&lt;a class=\&quot;button is-danger is-inverted\&quot;&gt;Inverted&lt;/a&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;a class=\&quot;button is-danger is-outlined is-fullwidth\&quot;&gt;Outlined&lt;/a&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><a class="button is-outlined">Outlined</a>
<a class="button is-primary is-outlined">Outlined</a>
<a class="button is-info is-outlined">Outlined</a>
<a class="button is-success is-outlined">Outlined</a>
<a class="button is-danger is-outlined">Outlined</a>
<br><br>

<a class="button is-primary is-inverted">Inverted</a>
<a class="button is-info is-inverted">Inverted</a>
<a class="button is-success is-inverted">Inverted</a>
<a class="button is-danger is-inverted">Inverted</a>
<br><br>
<a class="button is-danger is-outlined is-fullwidth">Outlined</a>

</div>
                    <div slot="description"><h4 id="bu-tong-style"><a class="header-anchor" href="#bu-tong-style" aria-hidden="true">¶</a> 不同Style</h4>
<ul>
<li>通过设置 <code>is-outlined</code> 显示边框</li>
<li>Inverted，文字颜色和背景颜色颠倒互换</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-outlined is-fullwidth"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 不同Style
  * 通过设置 `is-outlined` 显示边框
  * Inverted，文字颜色和背景颜色颠倒互换
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-outlined"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-inverted"</span>&gt;</span>Inverted<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-outlined is-fullwidth"</span>&gt;</span>Outlined<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>

</code></pre>
</demo-box>
<h4 id="states-zhuang-tai"><a class="header-anchor" href="#states-zhuang-tai" aria-hidden="true">¶</a> States 状态</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;a class=\&quot;button is-loading\&quot;&gt;Loading&lt;/a&gt;\n&lt;a class=\&quot;button is-primary is-loading\&quot;&gt;Loading&lt;/a&gt;\n&lt;a class=\&quot;button is-info is-loading\&quot;&gt;Loading&lt;/a&gt;\n&lt;a class=\&quot;button is-success is-loading\&quot;&gt;Loading&lt;/a&gt;\n&lt;a class=\&quot;button is-warning is-loading\&quot;&gt;Loading&lt;/a&gt;\n&lt;a class=\&quot;button is-danger is-loading\&quot;&gt;Loading&lt;/a&gt;\n&lt;br&gt;&lt;br&gt;\n\n&lt;a class=\&quot;button is-active\&quot;&gt;Active&lt;/a&gt;\n&lt;a class=\&quot;button is-primary is-active\&quot;&gt;Active&lt;/a&gt;\n&lt;a class=\&quot;button is-info is-active\&quot;&gt;Active&lt;/a&gt;\n&lt;a class=\&quot;button is-success is-active\&quot;&gt;Active&lt;/a&gt;\n&lt;a class=\&quot;button is-warning is-active\&quot;&gt;Active&lt;/a&gt;\n&lt;a class=\&quot;button is-danger is-active\&quot;&gt;Active&lt;/a&gt;\n&lt;br&gt;&lt;br&gt;\n\n&lt;a class=\&quot;button is-disabled\&quot;&gt;Disabled&lt;/a&gt;\n&lt;a class=\&quot;button is-primary is-disabled\&quot;&gt;Disabled&lt;/a&gt;\n&lt;a class=\&quot;button is-info is-disabled\&quot;&gt;Disabled&lt;/a&gt;\n&lt;a class=\&quot;button is-success is-disabled\&quot;&gt;Disabled&lt;/a&gt;\n&lt;a class=\&quot;button is-warning is-disabled\&quot;&gt;Disabled&lt;/a&gt;\n&lt;a class=\&quot;button is-danger is-disabled\&quot;&gt;Disabled&lt;/a&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><a class="button is-loading">Loading</a>
<a class="button is-primary is-loading">Loading</a>
<a class="button is-info is-loading">Loading</a>
<a class="button is-success is-loading">Loading</a>
<a class="button is-warning is-loading">Loading</a>
<a class="button is-danger is-loading">Loading</a>
<br><br>

<a class="button is-active">Active</a>
<a class="button is-primary is-active">Active</a>
<a class="button is-info is-active">Active</a>
<a class="button is-success is-active">Active</a>
<a class="button is-warning is-active">Active</a>
<a class="button is-danger is-active">Active</a>
<br><br>

<a class="button is-disabled">Disabled</a>
<a class="button is-primary is-disabled">Disabled</a>
<a class="button is-info is-disabled">Disabled</a>
<a class="button is-success is-disabled">Disabled</a>
<a class="button is-warning is-disabled">Disabled</a>
<a class="button is-danger is-disabled">Disabled</a>
</div>
                    <div slot="description"><h4 id="bu-tong-zhuang-tai"><a class="header-anchor" href="#bu-tong-zhuang-tai" aria-hidden="true">¶</a> 不同状态</h4>
<ul>
<li>通过设置 <code>is-loading</code> 显示加载中</li>
<li>通过设置 <code>is-active</code> 显示激活状态</li>
<li>通过设置 <code>is-disabled</code> 禁用</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 不同状态
  * 通过设置 `is-loading` 显示加载中
  * 通过设置 `is-active` 显示激活状态
  * 通过设置 `is-disabled` 禁用
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-loading"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-active"</span>&gt;</span>Active<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-disabled"</span>&gt;</span>Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;a class=\&quot;button\&quot;&gt;\n  &lt;span class=\&quot;icon\&quot;&gt;\n    &lt;i class=\&quot;fa fa-github\&quot;&gt;&lt;/i&gt;\n  &lt;/span&gt;\n  &lt;span&gt;GitHub&lt;/span&gt;\n&lt;/a&gt;\n&lt;a class=\&quot;button is-primary\&quot;&gt;\n  &lt;span class=\&quot;icon\&quot;&gt;\n    &lt;i class=\&quot;fa fa-twitter\&quot;&gt;&lt;/i&gt;\n  &lt;/span&gt;\n  &lt;span&gt;Twitter&lt;/span&gt;\n&lt;/a&gt;\n&lt;a class=\&quot;button is-success\&quot;&gt;\n  &lt;span class=\&quot;icon\&quot;&gt;\n    &lt;i class=\&quot;fa fa-check\&quot;&gt;&lt;/i&gt;\n  &lt;/span&gt;\n  &lt;span&gt;Save&lt;/span&gt;\n&lt;/a&gt;\n&lt;a class=\&quot;button is-danger\&quot;&gt;\n  &lt;span&gt;Delete&lt;/span&gt;\n  &lt;span class=\&quot;icon\&quot;&gt;\n    &lt;i class=\&quot;fa fa-times\&quot;&gt;&lt;/i&gt;\n  &lt;/span&gt;\n&lt;/a&gt;\n&lt;a class=\&quot;button is-danger is-outlined\&quot;&gt;\n  &lt;span class=\&quot;icon\&quot;&gt;&lt;i class=\&quot;fa fa-times\&quot;&gt;&lt;/i&gt;&lt;/span&gt;\n  &lt;span&gt;Delete&lt;/span&gt;\n&lt;/a&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><a class="button">
  <span class="icon">
    <i class="fa fa-github"></i>
  </span>
  <span>GitHub</span>
</a>
<a class="button is-primary">
  <span class="icon">
    <i class="fa fa-twitter"></i>
  </span>
  <span>Twitter</span>
</a>
<a class="button is-success">
  <span class="icon">
    <i class="fa fa-check"></i>
  </span>
  <span>Save</span>
</a>
<a class="button is-danger">
  <span>Delete</span>
  <span class="icon">
    <i class="fa fa-times"></i>
  </span>
</a>
<a class="button is-danger is-outlined">
  <span class="icon"><i class="fa fa-times"></i></span>
  <span>Delete</span>
</a>
</div>
                    <div slot="description"><h4 id="icon-tu-biao"><a class="header-anchor" href="#icon-tu-biao" aria-hidden="true">¶</a> Icon 图标</h4>
<ul>
<li>可内嵌图标，具体见下面代码</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-github"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>GitHub<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-twitter"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Twitter<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-check"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Save<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Delete<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-times"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-outlined"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-times"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Delete<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Icon 图标
  * 可内嵌图标，具体见下面代码
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-github"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>GitHub<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-twitter"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Twitter<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-check"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Save<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Delete<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-times"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger is-outlined"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-times"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Delete<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;p class=\&quot;control has-addons\&quot;&gt;\n  &lt;a class=\&quot;button\&quot;&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;\n      &lt;i class=\&quot;fa fa-align-left\&quot;&gt;&lt;/i&gt;\n    &lt;/span&gt;\n    &lt;span&gt;Left&lt;/span&gt;\n  &lt;/a&gt;\n  &lt;a class=\&quot;button\&quot;&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;\n      &lt;i class=\&quot;fa fa-align-center\&quot;&gt;&lt;/i&gt;\n    &lt;/span&gt;\n    &lt;span&gt;Center&lt;/span&gt;\n  &lt;/a&gt;\n  &lt;a class=\&quot;button\&quot;&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;\n      &lt;i class=\&quot;fa fa-align-right\&quot;&gt;&lt;/i&gt;\n    &lt;/span&gt;\n    &lt;span&gt;Right&lt;/span&gt;\n  &lt;/a&gt;\n&lt;/p&gt;\n\n&lt;p class=\&quot;control has-addons\&quot;&gt;\n  &lt;a class=\&quot;button is-primary\&quot;&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;&lt;i class=\&quot;fa fa-angle-left\&quot;&gt;&lt;/i&gt;&lt;/span&gt;\n    &lt;span&gt;Go back&lt;/span&gt;\n  &lt;/a&gt;\n  &lt;a class=\&quot;button is-primary\&quot;&gt;\n    &lt;span&gt;Go Forward&lt;/span&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;&lt;i class=\&quot;fa fa-angle-right\&quot;&gt;&lt;/i&gt;&lt;/span&gt;\n  &lt;/a&gt;\n&lt;/p&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><p class="control has-addons">
  <a class="button">
    <span class="icon is-small">
      <i class="fa fa-align-left"></i>
    </span>
    <span>Left</span>
  </a>
  <a class="button">
    <span class="icon is-small">
      <i class="fa fa-align-center"></i>
    </span>
    <span>Center</span>
  </a>
  <a class="button">
    <span class="icon is-small">
      <i class="fa fa-align-right"></i>
    </span>
    <span>Right</span>
  </a>
</p>

<p class="control has-addons">
  <a class="button is-primary">
    <span class="icon is-small"><i class="fa fa-angle-left"></i></span>
    <span>Go back</span>
  </a>
  <a class="button is-primary">
    <span>Go Forward</span>
    <span class="icon is-small"><i class="fa fa-angle-right"></i></span>
  </a>
</p>
</div>
                    <div slot="description"><h4 id="an-niu-zu"><a class="header-anchor" href="#an-niu-zu" aria-hidden="true">¶</a> 按钮组</h4>
<ul>
<li>按钮可成组显示</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-align-left"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Left<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-align-center"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Center<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-align-right"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Right<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-left"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Go back<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Go Forward<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-right"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 按钮组
  * 按钮可成组显示
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-align-left"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Left<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-align-center"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Center<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-align-right"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Right<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-left"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Go back<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Go Forward<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-right"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</demo-box>
</section></template>

