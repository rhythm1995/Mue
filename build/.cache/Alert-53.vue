<template><section><h2 id="alert"><a class="header-anchor" href="#alert" aria-hidden="true">¶</a> Alert</h2>
<p>Alert message，show information that need to pay attention to.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
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
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>There are 6 types of Alert : <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code> and default，sets it by <code>type</code> parameter</li>
<li>Enable or disable close button by setting <code>closable</code> parameter</li>
<li>Show loading icon when the <code>type='loading'</code></li>
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
  #### Basic
  * There are 6 types of Alert : `primary` `info` `success` `danger` `warning` and default，sets it by `type` parameter
  * Enable or disable close button by setting `closable` parameter
  * Show loading icon when the `type='loading'`
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
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;alert title=\&quot;well done!\&quot; type=\&quot;primary\&quot; icon=\&quot;smile-o\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;well done!\&quot; type=\&quot;warning\&quot; :animated=\&quot;true\&quot; icon=\&quot;meh-o\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&lt;alert title=\&quot;Callback\&quot; type=\&quot;success\&quot; :closable=\&quot;true\&quot; :on-close=\&quot;close\&quot;&gt;\n  Well done! You successfully read this important alert message.\n&lt;/alert&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><alert title="well done!" type="primary" icon="smile-o">
  Well done! You successfully read this important alert message.
</alert>

<alert title="well done!" type="warning" :animated="true" icon="meh-o">
  Well done! You successfully read this important alert message.
</alert>

<alert title="Callback" type="success" :closable="true" :on-close="close">
  Well done! You successfully read this important alert message.
</alert>

</div>
                    <div slot="description"><h4 id="icon-and-callback"><a class="header-anchor" href="#icon-and-callback" aria-hidden="true">¶</a> Icon and Callback</h4>
<ul>
<li>Sets icon by <code>icon</code>，when <code>:animated=&quot;true&quot;</code> the icon can spin</li>
<li>Sets close callback by <code>on-close</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"smile-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"meh-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Callback"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:on-close</span>=<span class="hljs-string">"close"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Icon and Callback
  * Sets icon by `icon`，when `:animated="true"` the icon can spin
  * Sets close callback by `on-close`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"smile-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"well done!"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"meh-o"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">alert</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Callback"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:on-close</span>=<span class="hljs-string">"close"</span>&gt;</span>
  Well done! You successfully read this important alert message.
<span class="hljs-tag">&lt;/<span class="hljs-name">alert</span>&gt;</span>

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
<td>Type of Alert styles，accepted values: <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code> <code>loading</code></td>
<td>String</td>
<td>default</td>
</tr>
<tr>
<td>title</td>
<td>Sets the alert title</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>icon</td>
<td>Sets the alert icon</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>animated</td>
<td>Whether the icon can be animated</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>closable</td>
<td>Whether Alert can be closed</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>on-close</td>
<td>Callback when close Alert</td>
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
          title: 'alert close callback',
        });
      },
    },
  };
</script>