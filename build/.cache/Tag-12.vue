<template><section><h2 id="tag-biao-qian"><a class="header-anchor" href="#tag-biao-qian" aria-hidden="true">¶</a> Tag 标签</h2>
<p>对不同事物的属性或维度进行标记和分类的小标签</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;tag type=\&quot;primary\&quot;&gt;Tag Primary&lt;/tag&gt;\n&lt;tag type=\&quot;info\&quot;&gt;Tag Info&lt;/tag&gt;\n&lt;tag type=\&quot;success\&quot;&gt;Tag Success&lt;/tag&gt;\n&lt;tag type=\&quot;danger\&quot;&gt;Tag Danger&lt;/tag&gt;\n&lt;tag type=\&quot;warning\&quot;&gt;Tag Warning&lt;/tag&gt;\n&lt;tag type=\&quot;primary\&quot; color=\&quot;#f50\&quot; :closable=\&quot;true\&quot;&gt;Tag Color&lt;/tag&gt;\n&lt;br&gt;&lt;br&gt;\n&lt;tag type=\&quot;primary\&quot; rounded&gt;Tag Primary&lt;/tag&gt;\n&lt;tag type=\&quot;info\&quot; rounded&gt;Tag Info&lt;/tag&gt;\n&lt;tag type=\&quot;success\&quot; rounded&gt;Tag Success&lt;/tag&gt;\n&lt;tag type=\&quot;danger\&quot; rounded&gt;Tag Danger&lt;/tag&gt;\n&lt;tag type=\&quot;warning\&quot; rounded&gt;Tag Warning&lt;/tag&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><tag type="primary">Tag Primary</tag>
<tag type="info">Tag Info</tag>
<tag type="success">Tag Success</tag>
<tag type="danger">Tag Danger</tag>
<tag type="warning">Tag Warning</tag>
<tag type="primary" color="#f50" :closable="true">Tag Color</tag>
<br><br>
<tag type="primary" rounded="">Tag Primary</tag>
<tag type="info" rounded="">Tag Info</tag>
<tag type="success" rounded="">Tag Success</tag>
<tag type="danger" rounded="">Tag Danger</tag>
<tag type="warning" rounded="">Tag Warning</tag>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>默认有五种主题颜色的tag，包括<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code>，通过<code>type</code>来设置</li>
<li>也可以通过设置<code>color</code>直接设置颜色(color的优先级高于type)</li>
<li>设置rounded，tag显示为圆弧形</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Tag Primary<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span>&gt;</span>Tag Info<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>Tag Success<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span>&gt;</span>Tag Danger<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span>&gt;</span>Tag Warning<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">color</span>=<span class="hljs-string">"#f50"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag Color<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Primary<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Info<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Success<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Danger<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Warning<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 默认有五种主题颜色的tag，包括`primary` `info` `success` `danger` `warning`，通过`type`来设置
  * 也可以通过设置`color`直接设置颜色(color的优先级高于type)
  * 设置rounded，tag显示为圆弧形
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Tag Primary<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span>&gt;</span>Tag Info<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>Tag Success<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span>&gt;</span>Tag Danger<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span>&gt;</span>Tag Warning<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">color</span>=<span class="hljs-string">"#f50"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag Color<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Primary<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Info<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Success<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Danger<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">rounded</span>&gt;</span>Tag Warning<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;tag type=\&quot;primary\&quot;&gt;Size default&lt;/tag&gt;\n&lt;tag type=\&quot;info\&quot; size=\&quot;small\&quot;&gt;Size small&lt;/tag&gt;\n&lt;tag type=\&quot;success\&quot; size=\&quot;medium\&quot;&gt;Tag medium&lt;/tag&gt;\n&lt;tag type=\&quot;warning\&quot; size=\&quot;large\&quot;&gt;Tag large&lt;/tag&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><tag type="primary">Size default</tag>
<tag type="info" size="small">Size small</tag>
<tag type="success" size="medium">Tag medium</tag>
<tag type="warning" size="large">Tag large</tag>
</div>
                    <div slot="description"><h4 id="she-zhi-da-xiao"><a class="header-anchor" href="#she-zhi-da-xiao" aria-hidden="true">¶</a> 设置大小</h4>
<ul>
<li>tag有四种大小，除了默认大小还包括<code>small</code> <code>medium</code> <code>large</code>,通过<code>size</code>来设置</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Size default<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span>Size small<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"medium"</span>&gt;</span>Tag medium<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"large"</span>&gt;</span>Tag large<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 设置大小
  * tag有四种大小，除了默认大小还包括`small` `medium` `large`,通过`size`来设置
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Size default<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span>Size small<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"medium"</span>&gt;</span>Tag medium<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"large"</span>&gt;</span>Tag large<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;tag type=\&quot;primary\&quot; :closable=\&quot;true\&quot;&gt;Tag with close button&lt;/tag&gt;\n&lt;tag type=\&quot;warning\&quot; size=\&quot;medium\&quot; :closable=\&quot;true\&quot; :on-close=\&quot;close\&quot;&gt;Close with callback&lt;/tag&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      close() {\n        this.$notify.open({\n          type: 'success',\n          title: 'Tag close callback',\n        });\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><tag type="primary" :closable="true">Tag with close button</tag>
<tag type="warning" size="medium" :closable="true" :on-close="close">Close with callback</tag>

</div>
                    <div slot="description"><h4 id="guan-bi-he-hui-diao"><a class="header-anchor" href="#guan-bi-he-hui-diao" aria-hidden="true">¶</a> 关闭和回调</h4>
<ul>
<li>可通过设置closable实现可关闭，on-close设置关闭时的回调函数</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag with close button<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"medium"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:on-close</span>=<span class="hljs-string">"close"</span>&gt;</span>Close with callback<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      close() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
          <span class="hljs-attr">title</span>: <span class="hljs-string">'Tag close callback'</span>,
        });
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 关闭和回调
  * 可通过设置closable实现可关闭，on-close设置关闭时的回调函数
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag with close button<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"medium"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:on-close</span>=<span class="hljs-string">"close"</span>&gt;</span>Close with callback<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      close() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
          <span class="hljs-attr">title</span>: <span class="hljs-string">'Tag close callback'</span>,
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
<td>type</td>
<td>主题颜色，可选值为<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>color</td>
<td>背景色,如#87d087</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>size</td>
<td>标签大小，可选值为<code>small</code> <code>medium</code> <code>large</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>rounded</td>
<td>是否圆弧形</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>closable</td>
<td>标签是否可关闭</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-close</td>
<td>标签关闭时的回调</td>
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
          title: 'Tag close callback',
        });
      },
    },
  };
</script>