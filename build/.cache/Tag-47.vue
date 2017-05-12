<template><section><h2 id="tag"><a class="header-anchor" href="#tag" aria-hidden="true">¶</a> Tag</h2>
<p>Tag for categorizing or markuping.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
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
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>There are 6 types of Alert: <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code> and default. sets it by <code>type</code> parameter.</li>
<li>apply a different background color by <code>color</code> parameter (Higher priority than type)</li>
<li>tag can be rounded</li>
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
  #### Basic
  * There are 6 types of Alert: `primary` `info` `success` `danger` `warning` and default. sets it by `type` parameter.
  * apply a different background color by `color` parameter (Higher priority than type)
  * tag can be rounded
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
                    <div slot="description"><h4 id="sizes"><a class="header-anchor" href="#sizes" aria-hidden="true">¶</a> Sizes</h4>
<ul>
<li>There are 4 sizes of tag: <code>small</code> <code>medium</code> <code>large</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Size default<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span>Size small<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"medium"</span>&gt;</span>Tag medium<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"large"</span>&gt;</span>Tag large<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Sizes
  * There are 4 sizes of tag: `small` `medium` `large`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Size default<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span>Size small<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"medium"</span>&gt;</span>Tag medium<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"large"</span>&gt;</span>Tag large<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;tag type=\&quot;primary\&quot; :closable=\&quot;true\&quot;&gt;Tag with close button&lt;/tag&gt;\n&lt;tag type=\&quot;warning\&quot; size=\&quot;medium\&quot; :closable=\&quot;true\&quot; :on-close=\&quot;close\&quot;&gt;Close with callback&lt;/tag&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      close() {\n        this.$notify.open({\n          type: 'success',\n          content: 'Tag close callback',\n        });\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><tag type="primary" :closable="true">Tag with close button</tag>
<tag type="warning" size="medium" :closable="true" :on-close="close">Close with callback</tag>

</div>
                    <div slot="description"><h4 id="close-and-callback"><a class="header-anchor" href="#close-and-callback" aria-hidden="true">¶</a> Close and Callback</h4>
<ul>
<li>Tag could be closable by set closable property. Closable Tag supports onClose events</li>
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
          <span class="hljs-attr">content</span>: <span class="hljs-string">'Tag close callback'</span>,
        });
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Close and Callback
  * Tag could be closable by set closable property. Closable Tag supports onClose events
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag with close button<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"medium"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:on-close</span>=<span class="hljs-string">"close"</span>&gt;</span>Close with callback<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      close() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'Tag close callback'</span>,
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
<td>type</td>
<td>There are 6 types of Tag: <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code> and default</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>color</td>
<td>The background color of Tag, such as #87d087</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>size</td>
<td>size of tag，accepted values: <code>small</code> <code>medium</code> <code>large</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>rounded</td>
<td>Whether the icon is rounded</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>closable</td>
<td>Tag can be closed.</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-close</td>
<td>Callback when tag was closed</td>
<td>Function</td>
<td>-</td>
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
          content: 'Tag close callback',
        });
      },
    },
  };
</script>