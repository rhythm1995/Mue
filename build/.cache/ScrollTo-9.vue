<template><section><h2 id="scrollto-gun-dong-gong-ju"><a class="header-anchor" href="#scrollto-gun-dong-gong-ju" aria-hidden="true">¶</a> ScrollTo 滚动工具</h2>
<p>平滑滚动到指定位置，预设了'滚动到顶部'，本功能基于小巧精悍的 <a href="https://github.com/callmecavs/jump.js">jump.js</a></p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;scroll-to target=\&quot;#t2\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot; id=\&quot;t1\&quot;&gt;t1，滚动到id为 `t2` 的元素&lt;/button&gt;\n&lt;/scroll-to&gt;\n\n&lt;scroll-to :distance=\&quot;500\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;向下滚动500px&lt;/button&gt;\n&lt;/scroll-to&gt;\n\n&lt;div style=\&quot;width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd\&quot;&gt;长div&lt;/div&gt;\n&lt;scroll-to target=\&quot;#t1\&quot;&gt;\n  &lt;button class=\&quot;button is-outlined\&quot; id=\&quot;t2\&quot;&gt;我是t2，滚回到t1&lt;/button&gt;\n&lt;/scroll-to&gt;\n&lt;scroll-to :distance=\&quot;-500\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;向上滚动500px&lt;/button&gt;\n&lt;/scroll-to&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><scroll-to target="#t2">
  <button class="button is-primary" id="t1">t1，滚动到id为 `t2` 的元素</button>
</scroll-to>

<scroll-to :distance="500">
  <button class="button is-primary">向下滚动500px</button>
</scroll-to>

<div style="width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd">长div</div>
<scroll-to target="#t1">
  <button class="button is-outlined" id="t2">我是t2，滚回到t1</button>
</scroll-to>
<scroll-to :distance="-500">
  <button class="button is-primary">向上滚动500px</button>
</scroll-to>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>通过 <code>target</code> 指定目标，target的值可以是任意css的选择器，如 <code>'.target' '#id1'</code></li>
<li>当 <code>target='top'</code> 时，会触发内置的 '返回到顶部',即在页面右下角显示返回顶部的箭头按钮</li>
<li>通过 <code>distance</code> 设置滚动距离(优先级高于target)，正值向下滚动，负值向上滚动</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t2"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t1"</span>&gt;</span>t1，滚动到id为 `t2` 的元素<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>向下滚动500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd"</span>&gt;</span>长div<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-outlined"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t2"</span>&gt;</span>我是t2，滚回到t1<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"-500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>向上滚动500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 通过 `target` 指定目标，target的值可以是任意css的选择器，如 `'.target' '#id1'`
  * 当 `target='top'` 时，会触发内置的 '返回到顶部',即在页面右下角显示返回顶部的箭头按钮
  * 通过 `distance` 设置滚动距离(优先级高于target)，正值向下滚动，负值向上滚动
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t2"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t1"</span>&gt;</span>t1，滚动到id为 `t2` 的元素<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>向下滚动500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 200px;height: 1000px; margin: 10px;border: 1px solid #ddd"</span>&gt;</span>长div<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">target</span>=<span class="hljs-string">"#t1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-outlined"</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"t2"</span>&gt;</span>我是t2，滚回到t1<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">scroll-to</span> <span class="hljs-attr">:distance</span>=<span class="hljs-string">"-500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>向上滚动500px<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">scroll-to</span>&gt;</span>
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
<td>target</td>
<td>目标，target的值可以是任意css的选择器，如 <code>'.target' '#id1'</code>.当 <code>target='top'</code> 时，会触发内置的 '返回到顶部'，即在页面右下角显示返回顶部的箭头按钮</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>duration</td>
<td>滚动时间，单位毫秒</td>
<td>Number</td>
<td>500</td>
</tr>
<tr>
<td>distance</td>
<td>滚动距离(优先级高于target)，正值向下滚动，负值向上滚动</td>
<td>Number</td>
<td>无</td>
</tr>
</tbody>
</table>
<div style="width: 200px;height: 1000px;margin: 10px; "></div>
</section></template>

