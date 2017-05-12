<template><section><h2 id="timeline-shi-jian-xian"><a class="header-anchor" href="#timeline-shi-jian-xian" aria-hidden="true">¶</a> Timeline 时间线</h2>
<p>垂直按时间展示的信息流</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;timeline&gt;\n  &lt;timeline-item date=\&quot;2 minutes ago\&quot; type=\&quot;primary\&quot;&gt;\n    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.\n  &lt;/timeline-item&gt;\n  &lt;timeline-item date=\&quot;Sat, 5 Mar\&quot; type=\&quot;primary\&quot;&gt;\n    &lt;p&gt;adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit&lt;/p&gt;\n  &lt;/timeline-item&gt;\n  &lt;timeline-item date=\&quot;Sun, 11 Feb\&quot; type=\&quot;success\&quot;&gt;\n    Call to customer Jacob and discuss the detail.\n  &lt;/timeline-item&gt;\n&lt;/timeline&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><timeline>
  <timeline-item date="2 minutes ago" type="primary">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  </timeline-item>
  <timeline-item date="Sat, 5 Mar" type="primary">
    <p>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
  </timeline-item>
  <timeline-item date="Sun, 11 Feb" type="success">
    Call to customer Jacob and discuss the detail.
  </timeline-item>
</timeline>
</div>
                    <div slot="description"><h4 id="ji-chu"><a class="header-anchor" href="#ji-chu" aria-hidden="true">¶</a> 基础</h4>
<ul>
<li>通过<code>date</code>设置时间</li>
<li>默认有五种主题颜色，包括<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code>，通过<code>type</code>来设置</li>
<li><code>timeline-item</code>采用<code>slot</code>接收任意形式的内容</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基础
  * 通过`date`设置时间
  * 默认有五种主题颜色，包括`primary` `info` `success` `danger` `warning`，通过`type`来设置
  * `timeline-item`采用`slot`接收任意形式的内容
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;timeline&gt;\n  &lt;timeline-item date=\&quot;2 minutes ago\&quot; icon=\&quot;twitter\&quot; type=\&quot;primary\&quot;&gt;\n    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.\n  &lt;/timeline-item&gt;\n  &lt;timeline-item type=\&quot;primary\&quot; date=\&quot;Sat, 5 Mar\&quot;&gt;\n    &lt;p&gt;adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit&lt;/p&gt;\n    &lt;p&gt;&lt;a href&gt;news center&lt;/a&gt;&lt;/p&gt;\n    &lt;p&gt;&lt;img src=\&quot;https://pek3a.qingstor.com/warehouse1/c1.jpg\&quot;&gt;&lt;/p&gt;\n  &lt;/timeline-item&gt;\n  &lt;timeline-item date=\&quot;Sun, 11 Feb\&quot; icon=\&quot;wechat\&quot; type=\&quot;success\&quot;&gt;\n    Call to customer Jacob and discuss the detail.\n  &lt;/timeline-item&gt;\n&lt;/timeline&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><timeline>
  <timeline-item date="2 minutes ago" icon="twitter" type="primary">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  </timeline-item>
  <timeline-item type="primary" date="Sat, 5 Mar">
    <p>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
    <p><a href="">news center</a></p>
    <p><img src="https://pek3a.qingstor.com/warehouse1/c1.jpg"></p>
  </timeline-item>
  <timeline-item date="Sun, 11 Feb" icon="wechat" type="success">
    Call to customer Jacob and discuss the detail.
  </timeline-item>
</timeline>
</div>
                    <div slot="description"><h4 id="geng-duo-she-zhi"><a class="header-anchor" href="#geng-duo-she-zhi" aria-hidden="true">¶</a> 更多设置</h4>
<ul>
<li><code>timeline-item</code>可通过<code>icon</code>参数设置图标</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"twitter"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">href</span>=<span class="hljs-string">""</span>&gt;</span>news center<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">img</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://pek3a.qingstor.com/warehouse1/c1.jpg"</span> /&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"wechat"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 更多设置
  * `timeline-item`可通过`icon`参数设置图标
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">timeline</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"2 minutes ago"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"twitter"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante soe aiea ose dos soois.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sat, 5 Mar"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>adipiscing elit lorem ipsum dolor sit amet, consectetur adipiscing elit<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">href</span>=<span class="hljs-string">""</span>&gt;</span>news center<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">img</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://pek3a.qingstor.com/warehouse1/c1.jpg"</span> /&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">timeline-item</span> <span class="hljs-attr">date</span>=<span class="hljs-string">"Sun, 11 Feb"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"wechat"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>
    Call to customer Jacob and discuss the detail.
  <span class="hljs-tag">&lt;/<span class="hljs-name">timeline-item</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">timeline</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="timeline-item"><a class="header-anchor" href="#timeline-item" aria-hidden="true">¶</a> timeline-item</h4>
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
<td>主题颜色，可选值为<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>date</td>
<td>日期时间</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>icon</td>
<td>图标</td>
<td>String</td>
<td>无</td>
</tr>
</tbody>
</table>
</section></template>

