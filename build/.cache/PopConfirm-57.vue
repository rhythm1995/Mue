<template><section><h2 id="popconfirm"><a class="header-anchor" href="#popconfirm" aria-hidden="true">¶</a> PopConfirm</h2>
<p>A simple and compact confirmation dialog of an action.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;pop-confirm content=\&quot;Are you sure delete this task?？\&quot;&gt;\n  &lt;button class=\&quot;button\&quot;&gt;PopConfirm&lt;/button&gt;\n&lt;/pop-confirm&gt;\n\n&lt;pop-confirm content=\&quot;Are you sure？\&quot; :show-cancel=\&quot;false\&quot; icon=\&quot;question-circle-o\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Icon Button&lt;/button&gt;\n&lt;/pop-confirm&gt;\n\n&lt;pop-confirm content=\&quot;Are you sure？\&quot; icon=\&quot;question-circle-o\&quot; :on-ok=\&quot;ok\&quot; :on-cancel=\&quot;cancel\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Callback&lt;/button&gt;\n&lt;/pop-confirm&gt;\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      ok() {\n        this.$notify.success({content: 'Delete successfully!'});\n      },\n      cancel() {\n        this.$notify.open({content: 'Cancel!'});\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><pop-confirm content="Are you sure delete this task?？">
  <button class="button">PopConfirm</button>
</pop-confirm>

<pop-confirm content="Are you sure？" :show-cancel="false" icon="question-circle-o">
  <button class="button is-primary">Icon Button</button>
</pop-confirm>

<pop-confirm content="Are you sure？" icon="question-circle-o" :on-ok="ok" :on-cancel="cancel">
  <button class="button is-primary">Callback</button>
</pop-confirm>


</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Display or hidden buttons by <code>show-ok</code> and <code>show-cancel</code>.</li>
<li>Customize text of buttons by <code>ok-text</code> and <code>cancel-text</code>.</li>
<li>Sets callback by <code>on-ok</code> and <code>on-cancel</code>.</li>
<li>Support setting icon</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Are you sure delete this task?？"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>PopConfirm<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Are you sure？"</span> <span class="hljs-attr">:show-cancel</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Icon Button<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Are you sure？"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"ok"</span> <span class="hljs-attr">:on-cancel</span>=<span class="hljs-string">"cancel"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Callback<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      ok() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'Delete successfully!'</span>});
      },
      cancel() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'Cancel!'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Basic
  * Display or hidden buttons by `show-ok` and `show-cancel`.
  * Customize text of buttons by `ok-text` and `cancel-text`.
  * Sets callback by `on-ok` and `on-cancel`.
  * Support setting icon
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Are you sure delete this task?？"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>PopConfirm<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Are you sure？"</span> <span class="hljs-attr">:show-cancel</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Icon Button<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">pop-confirm</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Are you sure？"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"question-circle-o"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"ok"</span> <span class="hljs-attr">:on-cancel</span>=<span class="hljs-string">"cancel"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Callback<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">pop-confirm</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      ok() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'Delete successfully!'</span>});
      },
      cancel() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'Cancel!'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<p>PopConfirm is inherited from Popover,Consult <router-link to="/en/components/popover" exact="">Popover's documentation</router-link> to find more APIs.</p>
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
<td>color of icon，accepted value: <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>icon</td>
<td>icon</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>ok-text</td>
<td>text of the confirmation button</td>
<td>String</td>
<td>OK</td>
</tr>
<tr>
<td>cancel-text</td>
<td>text of the cancel button</td>
<td>String</td>
<td>Cancel</td>
</tr>
<tr>
<td>on-ok</td>
<td>callback of confirmation</td>
<td>Function</td>
<td>-</td>
</tr>
<tr>
<td>on-cancel</td>
<td>callback of cancel</td>
<td>Function</td>
<td>-</td>
</tr>
<tr>
<td>show-ok</td>
<td>whether the ok button is visible or not</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>show-cancel</td>
<td>whether the cancel button is visible or not</td>
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
      this.$notify.success({content: 'Delete successfully!'});
    },
    cancel() {
      this.$notify.open({content: 'Cancel!'});
    },
  },
};
</script>