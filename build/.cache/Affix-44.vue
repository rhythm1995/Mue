<template><section><h2 id="affix"><a class="header-anchor" href="#affix" aria-hidden="true">¶</a> Affix</h2>
<p>Make an element sticky to viewport.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;affix&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Affix top&lt;/button&gt;\n&lt;/affix&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><affix>
  <button class="button is-primary">Affix top</button>
</affix>
</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<p>The simplest usage.</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Affix top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Basic
  The simplest usage.
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Affix top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;affix :offset=\&quot;200\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Stick 200px below the top&lt;/button&gt;\n&lt;/affix&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><affix :offset="200">
  <button class="button is-primary">Stick 200px below the top</button>
</affix>
</div>
                    <div slot="description"><h4 id="define-an-offset"><a class="header-anchor" href="#define-an-offset" aria-hidden="true">¶</a> Define an offset</h4>
<p>You can also position the element below the viewport edge</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"200"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Stick 200px below the top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Define an offset
  You can also position the element below the viewport edge
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"200"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Stick 200px below the top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div id=\&quot;parent\&quot; style=\&quot;height: 120px; text-align: center\&quot;&gt;\n  &lt;affix :offset=\&quot;0\&quot; boundary=\&quot;#parent\&quot;&gt;\n    &lt;button class=\&quot;button is-primary\&quot;&gt;Sticky bound to parent container&lt;/button&gt;\n  &lt;/affix&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div id="parent" style="height: 120px; text-align: center">
  <affix :offset="0" boundary="#parent">
    <button class="button is-primary">Sticky bound to parent container</button>
  </affix>
</div>
</div>
                    <div slot="description"><h4 id="sticky-boundary"><a class="header-anchor" href="#sticky-boundary" aria-hidden="true">¶</a> Sticky boundary</h4>
<p>You can define the boundary of a sticky element by setting the boundary parameter.This keeps the sticky element
within the dimensions of the boundary element</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"parent"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"height: 120px; text-align: center"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">boundary</span>=<span class="hljs-string">"#parent"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Sticky bound to parent container<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Sticky boundary
  You can define the boundary of a sticky element by setting the boundary parameter.This keeps the sticky element
  within the dimensions of the boundary element
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"parent"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"height: 120px; text-align: center"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">boundary</span>=<span class="hljs-string">"#parent"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Sticky bound to parent container<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div style=\&quot;text-align: right\&quot;&gt;\n  &lt;affix :on-affix=\&quot;onAffixed\&quot;&gt;\n    &lt;button class=\&quot;button is-primary\&quot;&gt;callback&lt;/button&gt;\n  &lt;/affix&gt;\n&lt;/div&gt;\n\n&quot;,&quot;script&quot;:&quot;\nexport default {\n  methods: {\n    onAffixed(status) {\n      this.$notify.open({\n        type: 'success',\n        content: `Sticky state ${status}`,\n      });\n    },\n  },\n};\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div style="text-align: right">
  <affix :on-affix="onAffixed">
    <button class="button is-primary">callback</button>
  </affix>
</div>

</div>
                    <div slot="description"><h4 id="callback"><a class="header-anchor" href="#callback" aria-hidden="true">¶</a> Callback</h4>
<p>Callback with affixed state.</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"text-align: right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:on-affix</span>=<span class="hljs-string">"onAffixed"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>callback<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  <span class="hljs-attr">methods</span>: {
    onAffixed(status) {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">content</span>: <span class="hljs-string">`Sticky state <span class="hljs-subst">${status}</span>`</span>,
      });
    },
  },
};
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Callback
  Callback with affixed state.
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"text-align: right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:on-affix</span>=<span class="hljs-string">"onAffixed"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>callback<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  <span class="hljs-attr">methods</span>: {
    onAffixed(status) {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">content</span>: <span class="hljs-string">`Sticky state <span class="hljs-subst">${status}</span>`</span>,
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
<td>offset</td>
<td>Top offset when affix should be triggered</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>boundary</td>
<td>Set a Css id selector to bind sticky to a specific element.(parent element or parent's parent...)</td>
<td>String(#parent)</td>
<td></td>
</tr>
<tr>
<td>on-affix</td>
<td>Callback when affix state is changed</td>
<td>Function(affixed)</td>
<td>-</td>
</tr>
</tbody>
</table>

</section></template>

<script>
  export default {
    methods: {
      onAffixed(status) {
        this.$notify.open({
          type: 'success',
          title: `回调状态${status}`,
        });
      },
    },
  };
</script>