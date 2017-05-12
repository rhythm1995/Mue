<template><section><h2 id="alert-jing-gao-kuang"><a class="header-anchor" href="#alert-jing-gao-kuang" aria-hidden="true">¶</a> Alert 警告框</h2>
<p>警告提示，展现需要关注的信息。</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;alert&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;well done!\&quot; type=\&quot;primary\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;info!\&quot; type=\&quot;info\&quot; :closable=\&quot;true\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;success!\&quot; type=\&quot;success\&quot; :closable=\&quot;true\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n\n&lt;alert title=\&quot;warning!\&quot; type=\&quot;warning\&quot; :closable=\&quot;true\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;danger!\&quot; type=\&quot;danger\&quot; :closable=\&quot;true\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert type=\&quot;loading\&quot;&gt;\n  Loading! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><alert>
  Well done! You successfully read this important alert message.
</alert>

<alert title="well done!" type="primary">
  Well done! You successfully read this important alert message.
</alert>

<alert title="info!" type="info" :closable="true">
  Well done! You successfully read this important alert message.
</alert>

<alert title="success!" type="success" :closable="true">
  Well done! You successfully read this important alert message.
</alert>


<alert title="warning!" type="warning" :closable="true">
  Well done! You successfully read this important alert message.
</alert>

<alert title="danger!" type="danger" :closable="true">
  Well done! You successfully read this important alert message.
</alert>

<alert type="loading">
  Loading! You successfully read this important alert message.
</alert>

</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>默认有五种主题颜色的tag，除了默认色还包括<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code>，可通过<code>type</code>来设置</li>
<li>通过设置<code>closable</code>为true，打开关闭按钮</li>
<li>type为<code>loading</code>时，显示动态载入效果</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">alert</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"info!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"success!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>


<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"warning!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"danger!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"loading"</span>&gt;</span>
  Loading! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 基本
  * 默认有五种主题颜色的tag，除了默认色还包括`primary` `info` `success` `danger` `warning`，可通过`type`来设置
  * 通过设置`closable`为true，打开关闭按钮
  * type为`loading`时，显示动态载入效果
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">alert</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"info!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"success!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>


<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"warning!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"danger!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"loading"</span>&gt;</span>
  Loading! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;alert title=\&quot;well done!\&quot; type=\&quot;primary\&quot; icon=\&quot;smile-o\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;well done!\&quot; type=\&quot;warning\&quot; :animated=\&quot;true\&quot; icon=\&quot;meh-o\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;回调\&quot; type=\&quot;success\&quot; :closable=\&quot;true\&quot; :on-close=\&quot;close\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><alert title="well done!" type="primary" icon="smile-o">
  Well done! You successfully read this important alert message.
</alert>

<alert title="well done!" type="warning" :animated="true" icon="meh-o">
  Well done! You successfully read this important alert message.
</alert>

<alert title="回调" type="success" :closable="true" :on-close="close">
  Well done! You successfully read this important alert message.
</alert>

</div>
                    <div slot="description"><h4 id="tu-biao-he-guan-bi-hui-diao"><a class="header-anchor" href="#tu-biao-he-guan-bi-hui-diao" aria-hidden="true">¶</a> 图标和关闭回调</h4>
<ul>
<li>通过<code>icon</code> 可设置图标，<code>animated</code>设置是否动画</li>
<li><code>on-close</code>设置关闭时的回调</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"smile-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"meh-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"回调"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:on-close</span>=<span class="hljs-string">"close"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 图标和关闭回调
  * 通过`icon` 可设置图标，`animated`设置是否动画
  * `on-close`设置关闭时的回调
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"smile-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"meh-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"回调"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:on-close</span>=<span class="hljs-string">"close"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

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
<td>主题颜色，可选值为<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code> <code>loading</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>title</td>
<td>标题</td>
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
<td>animated</td>
<td>图标是否旋转</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>closable</td>
<td>是否可关闭</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-close</td>
<td>关闭时的回调</td>
<td>Function</td>
<td>无</td>
</tr>
</tbody>
</table>

</section></template>

<script>
  export default {
    methods: {
      close() {
        this.$notify.open({
          type: 'success',
          title: 'alert close callback',
        });
      },
    },
  };
</script>