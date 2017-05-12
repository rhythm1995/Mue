<template><section><h2 id="checkbox-fu-xuan-kuang"><a class="header-anchor" href="#checkbox-fu-xuan-kuang" aria-hidden="true">¶</a> Checkbox 复选框</h2>
<p>复选框</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;checkbox val=\&quot;john\&quot;&gt;Checkbox&lt;/checkbox&gt;\n\n&lt;br&gt;&lt;br&gt;\n&lt;checkbox v-model=\&quot;checkedNames\&quot; val=\&quot;Jackie\&quot; checked&gt;Jackie Chan&lt;/checkbox&gt;\n{{ checkedNames }}\n\n&lt;br&gt;&lt;br&gt;\n&lt;checkbox label=\&quot;Checkbox\&quot; val=\&quot;john\&quot; disabled&gt;Checkbox&lt;/checkbox&gt;\n\n&lt;br&gt;&lt;br&gt;\n&lt;checkbox label=\&quot;Checkbox\&quot; val=\&quot;john\&quot; @change=\&quot;changeFunc\&quot;&gt;Checkbox&lt;/checkbox&gt;\n\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        checkedNames: '',\n      };\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><checkbox val="john">Checkbox</checkbox>

<br><br>
<checkbox v-model="checkedNames" val="Jackie" checked>Jackie Chan</checkbox>
{{ checkedNames }}

<br><br>
<checkbox label="Checkbox" val="john" disabled>Checkbox</checkbox>

<br><br>
<checkbox label="Checkbox" val="john" @change="changeFunc">Checkbox</checkbox>



</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>可通过 <code>v-model</code> 绑定数据</li>
<li>通过 <code>disabled</code> 设置禁用状态</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"john"</span>&gt;</span>Checkbox<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"checkedNames"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Jackie"</span> <span class="hljs-attr">checked</span>&gt;</span>Jackie Chan<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
<span>{{</span> checkedNames <span>}}</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Checkbox"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"john"</span> <span class="hljs-attr">disabled</span>&gt;</span>Checkbox<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Checkbox"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"john"</span> <span class="hljs-attr">@change</span>=<span class="hljs-string">"changeFunc"</span>&gt;</span>Checkbox<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">checkedNames</span>: <span class="hljs-string">''</span>,
      };
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 基本
  * 可通过 `v-model` 绑定数据
  * 通过 `disabled` 设置禁用状态
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"john"</span>&gt;</span>Checkbox<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"checkedNames"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Jackie"</span> <span class="hljs-attr">checked</span>&gt;</span>Jackie Chan<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
<span>{{</span> checkedNames <span>}}</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Checkbox"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"john"</span> <span class="hljs-attr">disabled</span>&gt;</span>Checkbox<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Checkbox"</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"john"</span> <span class="hljs-attr">@change</span>=<span class="hljs-string">"changeFunc"</span>&gt;</span>Checkbox<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">checkedNames</span>: <span class="hljs-string">''</span>,
      };
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;checkbox-group v-model=\&quot;groupVal\&quot;&gt;\n  &lt;checkbox val=\&quot;Kobe\&quot;&gt;Kobe&lt;/checkbox&gt;\n  &lt;checkbox val=\&quot;James\&quot;&gt;James&lt;/checkbox&gt;\n  &lt;checkbox val=\&quot;Wade\&quot;&gt;Wade&lt;/checkbox&gt;\n&lt;/checkbox-group&gt;\n{{ groupVal }}\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        groupVal: ['Kobe'],\n      };\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><checkbox-group v-model="groupVal">
  <checkbox val="Kobe">Kobe</checkbox>
  <checkbox val="James">James</checkbox>
  <checkbox val="Wade">Wade</checkbox>
</checkbox-group>
{{ groupVal }}


</div>
                    <div slot="description"><h4 id="checkbox-group"><a class="header-anchor" href="#checkbox-group" aria-hidden="true">¶</a> checkbox-group</h4>
<ul>
<li>绑定数据到同一数组</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">checkbox-group</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"groupVal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Kobe"</span>&gt;</span>Kobe<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"James"</span>&gt;</span>James<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Wade"</span>&gt;</span>Wade<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox-group</span>&gt;</span>
<span>{{</span> groupVal <span>}}</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">groupVal</span>: [<span class="hljs-string">'Kobe'</span>],
      };
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### checkbox-group
  * 绑定数据到同一数组
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">checkbox-group</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"groupVal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Kobe"</span>&gt;</span>Kobe<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"James"</span>&gt;</span>James<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">checkbox</span> <span class="hljs-attr">val</span>=<span class="hljs-string">"Wade"</span>&gt;</span>Wade<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">checkbox-group</span>&gt;</span>
<span>{{</span> groupVal <span>}}</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">groupVal</span>: [<span class="hljs-string">'Kobe'</span>],
      };
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="checkbox"><a class="header-anchor" href="#checkbox" aria-hidden="true">¶</a> checkbox</h4>
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
<td>change</td>
<td>值变化时的回调</td>
<td>Function</td>
<td>无</td>
</tr>
</tbody>
</table>
<h4 id="checkbox-group"><a class="header-anchor" href="#checkbox-group" aria-hidden="true">¶</a> checkbox-group</h4>
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
<td>change</td>
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
      checkedNames: '',
      groupVal: ['Kobe'],
    };
  },
  watch: {
    checked(val) {
      console.log(val);
    }
  },
  methods: {
    changeFunc(p) {
      console.log(p);
    },
  },
};
</script>