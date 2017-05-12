<template><section><h2 id="popconfirm-qi-pao-que-ren-kuang"><a class="header-anchor" href="#popconfirm-qi-pao-que-ren-kuang" aria-hidden="true">¶</a> PopConfirm 气泡确认框</h2>
<p>轻量级的确认对话框，基于 Popover 开发</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;pop-confirm content=\&quot;确定删除此条内容？不可恢复\&quot;&gt;\n  &lt;button class=\&quot;button\&quot;&gt;PopConfirm&lt;/button&gt;\n&lt;/pop-confirm&gt;\n\n&lt;pop-confirm content=\&quot;通过审核？\&quot; :show-cancel=\&quot;false\&quot; icon=\&quot;question-circle-o\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Icon Button&lt;/button&gt;\n&lt;/pop-confirm&gt;\n\n&lt;pop-confirm content=\&quot;通过审核？\&quot; icon=\&quot;question-circle-o\&quot; :on-ok=\&quot;ok\&quot; :on-cancel=\&quot;cancel\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Callback&lt;/button&gt;\n&lt;/pop-confirm&gt;\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      ok() {\n        this.$notify.success({content: '删除成功!'});\n      },\n      cancel() {\n        this.$notify.open({content: '取消删除!'});\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><pop-confirm content="确定删除此条内容？不可恢复">
  <button class="button">PopConfirm</button>
</pop-confirm>

<pop-confirm content="通过审核？" :show-cancel="false" icon="question-circle-o">
  <button class="button is-primary">Icon Button</button>
</pop-confirm>

<pop-confirm content="通过审核？" icon="question-circle-o" :on-ok="ok" :on-cancel="cancel">
  <button class="button is-primary">Callback</button>
</pop-confirm>


</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>基于 Popover 开发，除了内容只能是纯文字外，Popover的其他API都支持</li>
<li>支持通过 <code>show-ok</code> <code>show-cancel</code> 隐藏或显示按钮</li>
<li>通过 <code>ok-text</code> <code>cancel-text</code> 自定义按钮文字</li>
<li>通过 <code>on-ok</code> <code>on-cancel</code> 设置对应的回调</li>
<li>通过 <code>icon</code> 设置图标</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"确定删除此条内容？不可恢复"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>PopConfirm<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"通过审核？"</span> <span class="hljs-attr">:show-cancel</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Icon Button<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"通过审核？"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"ok"</span> <span class="hljs-attr">:on-cancel</span>=<span class="hljs-string">"cancel"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Callback<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      ok() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'删除成功!'</span>});
      },
      cancel() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'取消删除!'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 基于 Popover 开发，除了内容只能是纯文字外，Popover的其他API都支持
  * 支持通过 `show-ok` `show-cancel` 隐藏或显示按钮
  * 通过 `ok-text` `cancel-text` 自定义按钮文字
  * 通过 `on-ok` `on-cancel` 设置对应的回调
  * 通过 `icon` 设置图标
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"确定删除此条内容？不可恢复"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>PopConfirm<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"通过审核？"</span> <span class="hljs-attr">:show-cancel</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Icon Button<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"通过审核？"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"ok"</span> <span class="hljs-attr">:on-cancel</span>=<span class="hljs-string">"cancel"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Callback<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      ok() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'删除成功!'</span>});
      },
      cancel() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'取消删除!'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<p>只列出相对 <code>Popover</code> 新增的</p>
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
<td>图标颜色，可选值为<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>icon</td>
<td>图标</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>ok-text</td>
<td>确定按钮的文字</td>
<td>String</td>
<td>OK</td>
</tr>
<tr>
<td>cancel-text</td>
<td>取消按钮的文字</td>
<td>String</td>
<td>Cancel</td>
</tr>
<tr>
<td>on-ok</td>
<td>点击ok后的回调</td>
<td>Function</td>
<td>无</td>
</tr>
<tr>
<td>on-cancel</td>
<td>点击cancel后的回调</td>
<td>Function</td>
<td>无</td>
</tr>
<tr>
<td>show-ok</td>
<td>是否显示ok按钮</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>show-cancel</td>
<td>是否显示cancel按钮</td>
<td>Boolean</td>
<td>true</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    ok() {
      this.$notify.success({content: '删除成功!'});
    },
    cancel() {
      this.$notify.open({content: '取消删除!'});
    },
  },
};
</script>