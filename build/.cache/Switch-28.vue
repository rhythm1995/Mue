<template><section><h2 id="switch-kai-guan"><a class="header-anchor" href="#switch-kai-guan" aria-hidden="true">¶</a> Switch 开关</h2>
<p>Switch 开关</p>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;\n&lt;b-switch on-text=\&quot;开启\&quot; off-text=\&quot;关闭\&quot; v-model=\&quot;val1\&quot;&gt;&lt;/b-switch&gt;\n{{ val1 }}\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; checked&gt;&lt;/b-switch&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; disabled&gt;&lt;/b-switch&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; on-text=\&quot;开\&quot; off-text=\&quot;关\&quot; size=\&quot;small\&quot;&gt;&lt;/b-switch&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; :on-change=\&quot;onChange\&quot;&gt;&lt;/b-switch&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        val1: true,\n      };\n    },\n    methods: {\n      onChange(val) {\n        const content = val ? '开启' : '关闭';\n        this.$notify.info({content});\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component">
<b-switch on-text="开启" off-text="关闭" v-model="val1"></b-switch>
{{ val1 }}
<br><br>
<b-switch type="primary" checked></b-switch>
<br><br>
<b-switch type="primary" disabled></b-switch>
<br><br>
<b-switch type="primary" on-text="开" off-text="关" size="small"></b-switch>
<br><br>
<b-switch type="primary" :on-change="onChange"></b-switch>

</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>可通过 <code>v-model</code> 绑定数据</li>
<li><code>checked=true</code> 默认打开</li>
<li><code>disabled</code> 设置为禁用</li>
<li>通过 <code>on-text</code> <code>off-text</code> 设置开关文字</li>
<li><code>size</code> 设置大小</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"开启"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"关闭"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"val1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span>{{</span> val1 <span>}}</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">checked</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"开"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"关"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"onChange"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">val1</span>: <span class="hljs-literal">true</span>,
      };
    },
    <span class="hljs-attr">methods</span>: {
      onChange(val) {
        <span class="hljs-keyword">const</span> content = val ? <span class="hljs-string">'开启'</span> : <span class="hljs-string">'关闭'</span>;
        <span class="hljs-keyword">this</span>.$notify.info({content});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 可通过 `v-model` 绑定数据
  * `checked=true` 默认打开
  * `disabled` 设置为禁用
  * 通过 `on-text` `off-text` 设置开关文字
  * `size` 设置大小
</summary>
<pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"开启"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"关闭"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"val1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span>{{</span> val1 <span>}}</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">checked</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"开"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"关"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"onChange"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">val1</span>: <span class="hljs-literal">true</span>,
      };
    },
    <span class="hljs-attr">methods</span>: {
      onChange(val) {
        <span class="hljs-keyword">const</span> content = val ? <span class="hljs-string">'开启'</span> : <span class="hljs-string">'关闭'</span>;
        <span class="hljs-keyword">this</span>.$notify.info({content});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
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
<td>type</td>
<td>主题颜色，可选值为<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>on-text</td>
<td>开启时的文字</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>off-text</td>
<td>关闭时的文字</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>size</td>
<td>开关的大小，可选值为<code>small</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>checked</td>
<td>是否开启</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>disabled</td>
<td>是否禁用</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-change</td>
<td>开关切换时的回调</td>
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
      val1: true,
    };
  },
  methods: {
    onChange(val) {
      const content = val ? '开启' : '关闭';
      this.$notify.info({content});
    },
  },
};
</script>