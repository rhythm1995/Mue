<template><section><h2 id="inputnumber"><a class="header-anchor" href="#inputnumber" aria-hidden="true">¶</a> InputNumber</h2>
<p>Enter a number within certain range with the mouse or keyboard.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;input-number&gt;&lt;/input-number&gt;\n\n&lt;input-number disabled&gt;&lt;/input-number&gt;\n\n&lt;input-number size=\&quot;small\&quot;&gt;&lt;/input-number&gt;\n\n&lt;input-number mode=\&quot;s\&quot;&gt;&lt;/input-number&gt;\n\n&lt;input-number :max=\&quot;10\&quot; :min=\&quot;2\&quot;&gt;&lt;/input-number&gt;\n\n&lt;input-number mode=\&quot;s\&quot; :on-change=\&quot;callback\&quot;&gt;&lt;/input-number&gt;\n\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      callback(num) {\n        this.$notify.open({\n          content: `now the number is ${num}`,\n          icon: 'smile-o',\n          placement: 'top-center',\n        });\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><input-number></input-number>

<input-number disabled></input-number>

<input-number size="small"></input-number>

<input-number mode="s"></input-number>

<input-number :max="10" :min="2"></input-number>

<input-number mode="s" :on-change="callback"></input-number>



</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Enable or disable the component by <code>disabled</code></li>
<li>Sets <code>size=&quot;small&quot;</code> to show small size component</li>
<li><code>step</code> - incremental step</li>
<li><code>mode='s'</code> to set increase and decrease buttons on both sides of input</li>
<li>Sets the range by <code>max</code> and <code>min</code></li>
<li>Sets callback by <code>on-change</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">input-number</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">:max</span>=<span class="hljs-string">"10"</span> <span class="hljs-attr">:min</span>=<span class="hljs-string">"2"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"callback"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      callback(num) {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">`now the number is <span class="hljs-subst">${num}</span>`</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
        });
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Basic
  * Enable or disable the component by `disabled`
  * Sets `size="small"` to show small size component
  * `step` - incremental step
  * `mode='s'` to set increase and decrease buttons on both sides of input
  * Sets the range by `max` and `min`
  * Sets callback by `on-change`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">input-number</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">:max</span>=<span class="hljs-string">"10"</span> <span class="hljs-attr">:min</span>=<span class="hljs-string">"2"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"callback"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      callback(num) {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">`now the number is <span class="hljs-subst">${num}</span>`</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
        });
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
<td>val</td>
<td>default value</td>
<td>Number</td>
<td>-</td>
</tr>
<tr>
<td>min</td>
<td>min value</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>max</td>
<td>max value</td>
<td>Number</td>
<td>Infinity</td>
</tr>
<tr>
<td>size</td>
<td>size of the component,it can be <code>small</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>mode</td>
<td>the position of buttons，the increase and decrease buttons will be on both sides of input when value is <code>s</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>step</td>
<td>The number to which the current value is increased or decreased.</td>
<td>Number</td>
<td>1</td>
</tr>
<tr>
<td>disabled</td>
<td>Enable or disable the component</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-change</td>
<td>The callback triggered when the value is changed.</td>
<td>Function(val)</td>
<td>-</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    callback(num) {
      this.$notify.open({
        content: `now the number is ${num}`,
        icon: 'smile-o',
        placement: 'top-center',
      });
    },
  },
};
</script>