<template><section><h2 id="tooltip-wen-zi-ti-shi"><a class="header-anchor" href="#tooltip-wen-zi-ti-shi" aria-hidden="true">¶</a> Tooltip 文字提示</h2>
<p>简单的文字提示气泡框，常用于鼠标hover时</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;tooltip content=\&quot;Basic Tooltip!\&quot;&gt;\n  &lt;button class=\&quot;button\&quot;&gt;Basic Tooltip&lt;/button&gt;\n&lt;/tooltip&gt;\n\n&lt;tooltip content=\&quot;Tooltip Trigger!\&quot; trigger=\&quot;click\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Click Trigger&lt;/button&gt;\n&lt;/tooltip&gt;\n\n&lt;tooltip content=\&quot;Tooltip Always!\&quot; :always=\&quot;true\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Tooltip Always&lt;/button&gt;\n&lt;/tooltip&gt;\n\n&lt;tooltip content=\&quot;Tooltip Disabled!\&quot; :disabled=\&quot;true\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Tooltip Disabled&lt;/button&gt;\n&lt;/tooltip&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;tooltip content=\&quot;Focus Tooltip！\&quot; trigger=\&quot;focus\&quot;&gt;\n    &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Focus Tooltip！\&quot;&gt;\n  &lt;/tooltip&gt;\n&lt;/p&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><tooltip content="Basic Tooltip!">
  <button class="button">Basic Tooltip</button>
</tooltip>

<tooltip content="Tooltip Trigger!" trigger="click">
  <button class="button is-primary">Click Trigger</button>
</tooltip>

<tooltip content="Tooltip Always!" :always="true">
  <button class="button is-primary">Tooltip Always</button>
</tooltip>

<tooltip content="Tooltip Disabled!" :disabled="true">
  <button class="button is-primary">Tooltip Disabled</button>
</tooltip>
<br><br>
<p class="control">
  <tooltip content="Focus Tooltip！" trigger="focus">
    <input class="input" type="text" placeholder="Focus Tooltip！">
  </tooltip>
</p>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>通过<code>trigger</code>设置触发方式</li>
<li>设置<code>always</code>为true，tooltip会保持打开状态</li>
<li>设置<code>disabled</code>为true，tooltip会被禁用</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Basic Tooltip!"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>Basic Tooltip<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip Trigger!"</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"click"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Click Trigger<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip Always!"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Tooltip Always<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip Disabled!"</span> <span class="hljs-attr">:disabled</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Tooltip Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Focus Tooltip！"</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"focus"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Focus Tooltip！"</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 通过`trigger`设置触发方式
  * 设置`always`为true，tooltip会保持打开状态
  * 设置`disabled`为true，tooltip会被禁用
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Basic Tooltip!"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>Basic Tooltip<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip Trigger!"</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"click"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Click Trigger<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip Always!"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Tooltip Always<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip Disabled!"</span> <span class="hljs-attr">:disabled</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Tooltip Disabled<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Focus Tooltip！"</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"focus"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Focus Tooltip！"</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;tooltip-placement\&quot;&gt;\n  &lt;div style=\&quot;margin-left: 60px\&quot;&gt;\n    &lt;tooltip content=\&quot;Tooltip topLeft Tooltip topLeft!\&quot; placement=\&quot;topLeft\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;topLeft&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip top!\&quot; placement=\&quot;top\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;top&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip topRight! Tooltip topRight!\&quot; placement=\&quot;topRight\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;topRight&lt;/button&gt;\n    &lt;/tooltip&gt;\n  &lt;/div&gt;\n\n  &lt;div style=\&quot;width: 60px; float: left\&quot;&gt;\n    &lt;tooltip content=\&quot;Tooltip leftTop!\&quot; placement=\&quot;leftTop\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;leftTop&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip left!\&quot; placement=\&quot;left\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;left&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip leftBottom!\&quot; placement=\&quot;leftBottom\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;leftBottom&lt;/button&gt;\n    &lt;/tooltip&gt;\n  &lt;/div&gt;\n\n  &lt;div style=\&quot;width: 60px; margin-left: 360px\&quot;&gt;\n    &lt;tooltip content=\&quot;Basic rightTop!\&quot; placement=\&quot;rightTop\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;rightTop&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip right!\&quot; placement=\&quot;right\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;right&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip rightBottom!\&quot; placement=\&quot;rightBottom\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;rightBottom&lt;/button&gt;\n    &lt;/tooltip&gt;\n  &lt;/div&gt;\n\n  &lt;div style=\&quot;margin-left: 60px; clear: both\&quot;&gt;\n    &lt;tooltip content=\&quot;Tooltip bottomLeft! Basic bottomLeft!\&quot; placement=\&quot;bottomLeft\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;bottomLeft&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip bottom!\&quot; placement=\&quot;bottom\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;bottom&lt;/button&gt;\n    &lt;/tooltip&gt;\n\n    &lt;tooltip content=\&quot;Tooltip bottomRight! Tooltip bottomRight!\&quot; placement=\&quot;bottomRight\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;bottomRight&lt;/button&gt;\n    &lt;/tooltip&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="tooltip-placement">
  <div style="margin-left: 60px">
    <tooltip content="Tooltip topLeft Tooltip topLeft!" placement="topLeft">
      <button class="button">topLeft</button>
    </tooltip>

    <tooltip content="Tooltip top!" placement="top">
      <button class="button">top</button>
    </tooltip>

    <tooltip content="Tooltip topRight! Tooltip topRight!" placement="topRight">
      <button class="button">topRight</button>
    </tooltip>
  </div>

  <div style="width: 60px; float: left">
    <tooltip content="Tooltip leftTop!" placement="leftTop">
      <button class="button">leftTop</button>
    </tooltip>

    <tooltip content="Tooltip left!" placement="left">
      <button class="button">left</button>
    </tooltip>

    <tooltip content="Tooltip leftBottom!" placement="leftBottom">
      <button class="button">leftBottom</button>
    </tooltip>
  </div>

  <div style="width: 60px; margin-left: 360px">
    <tooltip content="Basic rightTop!" placement="rightTop">
      <button class="button">rightTop</button>
    </tooltip>

    <tooltip content="Tooltip right!" placement="right">
      <button class="button">right</button>
    </tooltip>

    <tooltip content="Tooltip rightBottom!" placement="rightBottom">
      <button class="button">rightBottom</button>
    </tooltip>
  </div>

  <div style="margin-left: 60px; clear: both">
    <tooltip content="Tooltip bottomLeft! Basic bottomLeft!" placement="bottomLeft">
      <button class="button">bottomLeft</button>
    </tooltip>

    <tooltip content="Tooltip bottom!" placement="bottom">
      <button class="button">bottom</button>
    </tooltip>

    <tooltip content="Tooltip bottomRight! Tooltip bottomRight!" placement="bottomRight">
      <button class="button">bottomRight</button>
    </tooltip>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="xian-shi-wei-zhi"><a class="header-anchor" href="#xian-shi-wei-zhi" aria-hidden="true">¶</a> 显示位置</h4>
<ul>
<li>tooltip有12个可选位置</li>
<li>tooltip可根据离视图距离自适应位置</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"tooltip-placement"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip topLeft Tooltip topLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip top!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"top"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip topRight! Tooltip topRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; float: left"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip leftTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip left!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>left<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip leftBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; margin-left: 360px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Basic rightTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip right!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>right<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip rightBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px; clear: both"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip bottomLeft! Basic bottomLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip bottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip bottomRight! Tooltip bottomRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 显示位置
  * tooltip有12个可选位置
  * tooltip可根据离视图距离自适应位置
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"tooltip-placement"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip topLeft Tooltip topLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip top!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"top"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip topRight! Tooltip topRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; float: left"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip leftTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip left!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>left<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip leftBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; margin-left: 360px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Basic rightTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip right!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>right<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip rightBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px; clear: both"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip bottomLeft! Basic bottomLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip bottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">tooltip</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Tooltip bottomRight! Tooltip bottomRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">tooltip</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
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
<td>trigger</td>
<td>触发方式</td>
<td>String</td>
<td>hover</td>
</tr>
<tr>
<td>content</td>
<td>内容</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>placement</td>
<td>位置，可选值：<code>top</code> <code>left</code> <code>right</code> <code>bottom</code> <code>topLeft</code> <code>topRight</code> <code>leftTop</code> <code>leftBottom</code> <br> <code>bottomLeft</code> <code>rightTop</code> <code>rightBottom</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>always</td>
<td>是否保持打开状态</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>disabled</td>
<td>是否禁用</td>
<td>Boolean</td>
<td>false</td>
</tr>
</tbody>
</table>

</section></template>
<style>
.tooltip-placement .button{
  width: 120px;
  margin: 5px 0;
}
</style>
