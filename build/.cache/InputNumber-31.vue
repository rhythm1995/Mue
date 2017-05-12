<template><section><h2 id="inputnumber"><a class="header-anchor" href="#inputnumber" aria-hidden="true">¶</a> InputNumber</h2>
<p>用在数字的输入场景中，可使用鼠标和键盘操作</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;input-number :val=\&quot;5\&quot;&gt;&lt;/input-number&gt;\n\n&lt;input-number disabled&gt;&lt;/input-number&gt;\n\n&lt;input-number size=\&quot;small\&quot;&gt;&lt;/input-number&gt;\n\n&lt;input-number mode=\&quot;s\&quot;&gt;&lt;/input-number&gt;\n\n&lt;input-number :max=\&quot;10\&quot; :min=\&quot;-5\&quot; :on-change=\&quot;callback\&quot;&gt;&lt;/input-number&gt;\n\n&lt;input-number mode=\&quot;s\&quot; :on-change=\&quot;callback\&quot;&gt;&lt;/input-number&gt;\n\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      callback(num) {\n        this.$notify.open({\n          content: `现在的数字是${num}`,\n          icon: 'smile-o',\n          placement: 'top-center',\n        });\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><input-number :val="5"></input-number>

<input-number disabled></input-number>

<input-number size="small"></input-number>

<input-number mode="s"></input-number>

<input-number :max="10" :min="-5" :on-change="callback"></input-number>

<input-number mode="s" :on-change="callback"></input-number>



</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>通过 <code>val</code> 设置初始值</li>
<li>通过 <code>disabled</code> 设置禁用状态</li>
<li>设置 <code>size=&quot;small&quot;</code> 显示小尺寸</li>
<li>通过 <code>step</code> 设置步长</li>
<li><code>mode='s'</code> 设置增减按钮放在input的两边</li>
<li>通过 <code>max</code> <code>min</code> 设置范围</li>
<li>通过 <code>on-change</code> 设置回调</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">:val</span>=<span class="hljs-string">"5"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">:max</span>=<span class="hljs-string">"10"</span> <span class="hljs-attr">:min</span>=<span class="hljs-string">"-5"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"callback"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"callback"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      callback(num) {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">`现在的数字是<span class="hljs-subst">${num}</span>`</span>,
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
  #### 基本
  * 通过 `val` 设置初始值
  * 通过 `disabled` 设置禁用状态
  * 设置 `size="small"` 显示小尺寸
  * 通过 `step` 设置步长
  * `mode='s'` 设置增减按钮放在input的两边
  * 通过 `max` `min` 设置范围
  * 通过 `on-change` 设置回调
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">:val</span>=<span class="hljs-string">"5"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">:max</span>=<span class="hljs-string">"10"</span> <span class="hljs-attr">:min</span>=<span class="hljs-string">"-5"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"callback"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">input-number</span> <span class="hljs-attr">mode</span>=<span class="hljs-string">"s"</span> <span class="hljs-attr">:on-change</span>=<span class="hljs-string">"callback"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">input-number</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      callback(num) {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">`现在的数字是<span class="hljs-subst">${num}</span>`</span>,
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
<th>成员</th>
<th>说明</th>
<th>类型</th>
<th>默认值</th>
</tr>
</thead>
<tbody>
<tr>
<td>val</td>
<td>初始值</td>
<td>Number</td>
<td>无</td>
</tr>
<tr>
<td>min</td>
<td>最小值</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>max</td>
<td>最大值</td>
<td>Number</td>
<td>Infinity</td>
</tr>
<tr>
<td>size</td>
<td>标签大小，可选值为<code>small</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>mode</td>
<td>按钮展现方式，当值为<code>s</code>时，按钮放在两边</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>step</td>
<td>步长</td>
<td>Number</td>
<td>1</td>
</tr>
<tr>
<td>disabled</td>
<td>设置禁用状态</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-change</td>
<td>数字改变时的回调</td>
<td>Function(val)</td>
<td>无</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    callback(num) {
      this.$notify.open({
        content: `现在的数字是${num}`,
        icon: 'smile-o',
        placement: 'top-center',
      });
    },
  },
};
</script>