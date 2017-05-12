<template><section><h2 id="radio-dan-xuan-kuang"><a class="header-anchor" href="#radio-dan-xuan-kuang" aria-hidden="true">¶</a> Radio 单选框</h2>
<p>单选框</p>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;radio&gt;Radio&lt;/radio&gt;\n\n&lt;br&gt;&lt;br&gt;\n&lt;radio v-model=\&quot;radio1\&quot; val=\&quot;test\&quot;&gt;v-model绑定&lt;/radio&gt; {{ radio1 }}\n\n&lt;br&gt;&lt;br&gt;\n&lt;radio v-model=\&quot;radio1\&quot; val=\&quot;test\&quot; disabled&gt;Radio(disabled)&lt;/radio&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><radio>Radio</radio>

<br><br>
<radio v-model="radio1" val="test">v-model绑定</radio> {{ radio1 }}

<br><br>
<radio v-model="radio1" val="test" disabled>Radio(disabled)</radio>

</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>tag有四种大小，除了默认大小还包括<code>small</code> <code>medium</code> <code>large</code>,通过<code>size</code>来设置</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">radio</span>&gt;</span>Radio<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"radio1"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"test"</span>&gt;</span>v-model绑定<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span> <span>{{</span> radio1 <span>}}</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"radio1"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"test"</span> <span class="hljs-attr">disabled</span>&gt;</span>Radio(disabled)<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 基本
  * tag有四种大小，除了默认大小还包括`small` `medium` `large`,通过`size`来设置
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">radio</span>&gt;</span>Radio<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"radio1"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"test"</span>&gt;</span>v-model绑定<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span> <span>{{</span> radio1 <span>}}</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"radio1"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"test"</span> <span class="hljs-attr">disabled</span>&gt;</span>Radio(disabled)<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>

</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;radio-group v-model=\&quot;group1\&quot;&gt;\n  &lt;radio val=\&quot;Kobe\&quot;&gt;Kobe&lt;/radio&gt;\n  &lt;radio val=\&quot;James\&quot; disabled&gt;James&lt;/radio&gt;\n  &lt;radio val=\&quot;Wade\&quot;&gt;Wade&lt;/radio&gt;\n&lt;/radio-group&gt;\n&lt;div&gt;{{ group1 }}&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><radio-group v-model="group1">
  <radio val="Kobe">Kobe</radio>
  <radio val="James" disabled>James</radio>
  <radio val="Wade">Wade</radio>
</radio-group>
<div>{{ group1 }}</div>
</div>
                    <div slot="description"><h4 id="radio-group"><a class="header-anchor" href="#radio-group" aria-hidden="true">¶</a> radio-group</h4>
<ul>
<li>一组互斥的 Radio 配合使用</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">radio-group</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"group1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Kobe"</span>&gt;</span>Kobe<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"James"</span> <span class="hljs-attr">disabled</span>&gt;</span>James<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Wade"</span>&gt;</span>Wade<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">radio-group</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span>&gt;</span><span>{{</span> group1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### radio-group
  * 一组互斥的 Radio 配合使用
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">radio-group</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"group1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Kobe"</span>&gt;</span>Kobe<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"James"</span> <span class="hljs-attr">disabled</span>&gt;</span>James<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Wade"</span>&gt;</span>Wade<span class="hljs-tag">&lt;/<span class="hljs-name">radio</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">radio-group</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span>&gt;</span><span>{{</span> group1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;radio-group v-model=\&quot;group1\&quot;&gt;\n  &lt;radio-button val=\&quot;Kobe\&quot; icon=\&quot;dribbble\&quot;&gt;Kobe&lt;/radio-button&gt;\n  &lt;radio-button val=\&quot;James\&quot; icon=\&quot;chrome\&quot;&gt;James&lt;/radio-button&gt;\n  &lt;radio-button val=\&quot;Wade\&quot;&gt;Wade&lt;/radio-button&gt;\n&lt;/radio-group&gt;\n&lt;div&gt;{{ group1 }}&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><radio-group v-model="group1">
  <radio-button val="Kobe" icon="dribbble">Kobe</radio-button>
  <radio-button val="James" icon="chrome">James</radio-button>
  <radio-button val="Wade">Wade</radio-button>
</radio-group>
<div>{{ group1 }}</div>
</div>
                    <div slot="description"><h4 id="radio-button"><a class="header-anchor" href="#radio-button" aria-hidden="true">¶</a> radio-button</h4>
<ul>
<li>按钮样式的单选组</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">radio-group</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"group1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio-button</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Kobe"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"dribbble"</span>&gt;</span>Kobe<span class="hljs-tag">&lt;/<span class="hljs-name">radio-button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio-button</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"James"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"chrome"</span>&gt;</span>James<span class="hljs-tag">&lt;/<span class="hljs-name">radio-button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio-button</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Wade"</span>&gt;</span>Wade<span class="hljs-tag">&lt;/<span class="hljs-name">radio-button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">radio-group</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span>&gt;</span><span>{{</span> group1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### radio-button
  * 按钮样式的单选组
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">radio-group</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"group1"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio-button</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Kobe"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"dribbble"</span>&gt;</span>Kobe<span class="hljs-tag">&lt;/<span class="hljs-name">radio-button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio-button</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"James"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"chrome"</span>&gt;</span>James<span class="hljs-tag">&lt;/<span class="hljs-name">radio-button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">radio-button</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Wade"</span>&gt;</span>Wade<span class="hljs-tag">&lt;/<span class="hljs-name">radio-button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">radio-group</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span>&gt;</span><span>{{</span> group1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="radio"><a class="header-anchor" href="#radio" aria-hidden="true">¶</a> radio</h4>
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
<td>name</td>
<td>绑定的原生checkbox的name</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>val</td>
<td>checkbox的value值</td>
<td>String, Number, Boolean</td>
<td>无</td>
</tr>
<tr>
<td>disabled</td>
<td>是否禁用</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>checked</td>
<td>是否已选</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-change</td>
<td>值变化时的回调</td>
<td>Function</td>
<td>无</td>
</tr>
</tbody>
</table>
<h4 id="radio-button"><a class="header-anchor" href="#radio-button" aria-hidden="true">¶</a> radio-button</h4>
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
<td>name</td>
<td>绑定的原生checkbox的name</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>val</td>
<td>checkbox的value值</td>
<td>String, Number, Boolean</td>
<td>无</td>
</tr>
<tr>
<td>icon</td>
<td>按钮上的icon</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>disabled</td>
<td>是否禁用</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>checked</td>
<td>是否已选</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-change</td>
<td>值变化时的回调</td>
<td>Function</td>
<td>无</td>
</tr>
</tbody>
</table>
<h4 id="radio-group"><a class="header-anchor" href="#radio-group" aria-hidden="true">¶</a> radio-group</h4>
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
<td>value</td>
<td>指定选中的选项</td>
<td>Array</td>
<td>无</td>
</tr>
<tr>
<td>on-change</td>
<td>值变化时的回调</td>
<td>Function</td>
<td>无</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  data() {
    return {
      radio1: 'test',
      group1: '',
    };
  },
};
</script>