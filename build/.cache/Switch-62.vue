<template><section><h2 id="switch"><a class="header-anchor" href="#switch" aria-hidden="true">¶</a> Switch</h2>
<p>Switching Selector.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;\n&lt;b-switch on-text=\&quot;ON\&quot; off-text=\&quot;OFF\&quot; v-model=\&quot;val1\&quot;&gt;&lt;/b-switch&gt;\n{{ val1 }}\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; checked&gt;&lt;/b-switch&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; disabled&gt;&lt;/b-switch&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; on-text=\&quot;on\&quot; off-text=\&quot;off\&quot; size=\&quot;small\&quot;&gt;&lt;/b-switch&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;b-switch type=\&quot;primary\&quot; :on-change=\&quot;onChange\&quot;&gt;&lt;/b-switch&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        val1: true,\n      };\n    },\n    methods: {\n      onChange(val) {\n        const content = val ? 'open' : 'off';\n        this.$notify.info({content});\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component">
<b-switch on-text="ON" off-text="OFF" v-model="val1"></b-switch>
{{ val1 }}
<br><br>
<b-switch type="primary" checked></b-switch>
<br><br>
<b-switch type="primary" disabled></b-switch>
<br><br>
<b-switch type="primary" on-text="on" off-text="off" size="small"></b-switch>
<br><br>
<b-switch type="primary" :on-change="onChange"></b-switch>

</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>support two-way binding by <code>v-model</code></li>
<li>Enable or disable the component by <code>disabled</code></li>
<li>With text</li>
<li>Sets <code>size=&quot;small&quot;</code> to show small size component</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"ON"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"OFF"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"val1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span>{{</span> val1 <span>}}</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">checked</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"on"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"off"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
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
        <span class="hljs-keyword">const</span> content = val ? <span class="hljs-string">'open'</span> : <span class="hljs-string">'off'</span>;
        <span class="hljs-keyword">this</span>.$notify.info({content});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Basic
  * support two-way binding by `v-model`
  * Enable or disable the component by `disabled`
  * With text
  * Sets `size="small"` to show small size component
</summary>
<pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"ON"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"OFF"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"val1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span>{{</span> val1 <span>}}</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">checked</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">b-switch</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">on-text</span>=<span class="hljs-string">"on"</span> <span class="hljs-attr">off-text</span>=<span class="hljs-string">"off"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">b-switch</span>&gt;</span>
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
        <span class="hljs-keyword">const</span> content = val ? <span class="hljs-string">'open'</span> : <span class="hljs-string">'off'</span>;
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
<th>Properties</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>type</td>
<td>color of Switch, it can be one of <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>on-text</td>
<td>text displayed when the checked state is on</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>off-text</td>
<td>text displayed when the checked state is off</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>size</td>
<td>size of the component,it can be <code>small</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>checked</td>
<td>determine whether the <code>Switch</code> is checked</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>disabled</td>
<td>Enable or disable the component</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-change</td>
<td>The callback triggered when the checked state is changing</td>
<td>Function</td>
<td>-</td>
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
      const content = val ? 'open' : 'off';
      this.$notify.info({content});
    },
  },
};
</script>