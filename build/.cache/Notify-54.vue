<template><section><h2 id="notify"><a class="header-anchor" href="#notify" aria-hidden="true">¶</a> Notify</h2>
<p>Display global messages as feedbacks to user operations.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;button class=\&quot;button\&quot; @click=\&quot;basicNotify\&quot;&gt;Click me&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;primaryNotify\&quot;&gt;Click me&lt;/button&gt;\n&lt;button class=\&quot;button is-info\&quot; @click=\&quot;infoNotify\&quot;&gt;Click me&lt;/button&gt;\n&lt;button class=\&quot;button is-success\&quot; @click=\&quot;successNotify\&quot;&gt;Click me&lt;/button&gt;\n&lt;button class=\&quot;button is-warning\&quot; @click=\&quot;warningNotify\&quot;&gt;Click me&lt;/button&gt;\n&lt;button class=\&quot;button is-danger\&quot; @click=\&quot;dangerNotify\&quot;&gt;Click me&lt;/button&gt;\n&lt;button class=\&quot;button is-info\&quot; @click=\&quot;loadingNotify\&quot;&gt;Loading&lt;/button&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      basicNotify() {\n        this.$notify.open({content: 'You clicked me!',});\n      },\n      primaryNotify() {\n        this.$notify.open({content: 'You clicked me!', type: 'primary'});\n      },\n      infoNotify() {\n        this.$notify.info({content: 'You clicked me!'});\n      },\n      successNotify() {\n        this.$notify.success({content: 'You clicked me!'});\n      },\n      warningNotify() {\n        this.$notify.warning({content: 'You clicked me!'});\n      },\n      dangerNotify() {\n        this.$notify.open({content: 'You clicked me!', type: 'danger'});\n      },\n      loadingNotify() {\n        this.$notify.open({content: 'Loading...', type: 'loading'});\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><button class="button" @click="basicNotify">Click me</button>
<button class="button is-primary" @click="primaryNotify">Click me</button>
<button class="button is-info" @click="infoNotify">Click me</button>
<button class="button is-success" @click="successNotify">Click me</button>
<button class="button is-warning" @click="warningNotify">Click me</button>
<button class="button is-danger" @click="dangerNotify">Click me</button>
<button class="button is-info" @click="loadingNotify">Loading</button>

</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Six types，<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code> and default</li>
<li>Can be called by <code>this.$notify.info({...})</code>(or <code>this.$notify.success({...})</code> ...)</li>
<li>Auto closed in 4.5s</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"basicNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"primaryNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"infoNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"successNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"warningNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"dangerNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"loadingNotify"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      basicNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>,});
      },
      primaryNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'primary'</span>});
      },
      infoNotify() {
        <span class="hljs-keyword">this</span>.$notify.info({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>});
      },
      successNotify() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>});
      },
      warningNotify() {
        <span class="hljs-keyword">this</span>.$notify.warning({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>});
      },
      dangerNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'danger'</span>});
      },
      loadingNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'Loading...'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'loading'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Basic
  * Six types，`primary` `info` `success` `danger` `warning` and default
  * Can be called by `this.$notify.info({...})`(or `this.$notify.success({...})` ...)
  * Auto closed in 4.5s
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"basicNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"primaryNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"infoNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"successNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"warningNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"dangerNotify"</span>&gt;</span>Click me<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"loadingNotify"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      basicNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>,});
      },
      primaryNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'primary'</span>});
      },
      infoNotify() {
        <span class="hljs-keyword">this</span>.$notify.info({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>});
      },
      successNotify() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>});
      },
      warningNotify() {
        <span class="hljs-keyword">this</span>.$notify.warning({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>});
      },
      dangerNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'You clicked me!'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'danger'</span>});
      },
      loadingNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'Loading...'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'loading'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;button class=\&quot;button\&quot; @click=\&quot;durationNotify\&quot;&gt;auto-close&lt;/button&gt;\n&lt;button class=\&quot;button\&quot; @click=\&quot;iconNotify\&quot;&gt;Icon&lt;/button&gt;\n&lt;button class=\&quot;button\&quot; @click=\&quot;placementNotify\&quot;&gt;top-center&lt;/button&gt;\n&lt;button class=\&quot;button\&quot; @click=\&quot;transitionNotify\&quot;&gt;Transition&lt;/button&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      durationNotify() {\n        this.$notify.open({\n          content: '10秒后自动关闭！',\n          duration: 10000,\n        });\n      },\n      iconNotify() {\n        this.$notify.open({\n          content: 'customize icon！',\n          icon: 'smile-o',\n        });\n      },\n      placementNotify() {\n        this.$notify.open({\n          content: 'customize position！',\n          icon: 'smile-o',\n          placement: 'top-center',\n        });\n      },\n      transitionNotify() {\n        this.$notify.open({\n          content: 'customize transition！',\n          icon: 'smile-o',\n          placement: 'top-center',\n          transition: 'bounce',\n          type: 'danger',\n        });\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><button class="button" @click="durationNotify">auto-close</button>
<button class="button" @click="iconNotify">Icon</button>
<button class="button" @click="placementNotify">top-center</button>
<button class="button" @click="transitionNotify">Transition</button>

</div>
                    <div slot="description"><h4 id="more"><a class="header-anchor" href="#more" aria-hidden="true">¶</a> More</h4>
<ul>
<li>Customize notify display duration by setting <code>duration</code> parameter</li>
<li>Sets icon by <code>icon</code></li>
<li>Enable or disable close button by setting <code>closable</code> parameter</li>
<li>There are 12 placement options available including <code>top-right</code> <code>top-center</code> <code>top-left</code> <code>bottom-right</code> <code>bottom-center</code> <code>bottom-left</code></li>
<li>support <code>transition</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"durationNotify"</span>&gt;</span>auto-close<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"iconNotify"</span>&gt;</span>Icon<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"placementNotify"</span>&gt;</span>top-center<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"transitionNotify"</span>&gt;</span>Transition<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      durationNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'10秒后自动关闭！'</span>,
          <span class="hljs-attr">duration</span>: <span class="hljs-number">10000</span>,
        });
      },
      iconNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'customize icon！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
        });
      },
      placementNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'customize position！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
        });
      },
      transitionNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'customize transition！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounce'</span>,
          <span class="hljs-attr">type</span>: <span class="hljs-string">'danger'</span>,
        });
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### More
  * Customize notify display duration by setting `duration` parameter
  * Sets icon by `icon`
  * Enable or disable close button by setting `closable` parameter
  * There are 12 placement options available including `top-right` `top-center` `top-left` `bottom-right` `bottom-center` `bottom-left`
  * support `transition`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"durationNotify"</span>&gt;</span>auto-close<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"iconNotify"</span>&gt;</span>Icon<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"placementNotify"</span>&gt;</span>top-center<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"transitionNotify"</span>&gt;</span>Transition<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      durationNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'10秒后自动关闭！'</span>,
          <span class="hljs-attr">duration</span>: <span class="hljs-number">10000</span>,
        });
      },
      iconNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'customize icon！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
        });
      },
      placementNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'customize position！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
        });
      },
      transitionNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'customize transition！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounce'</span>,
          <span class="hljs-attr">type</span>: <span class="hljs-string">'danger'</span>,
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
<td>type of notify，one of <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>title</td>
<td>title of notify</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>content</td>
<td>content of notify</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>duration</td>
<td>The duration visibility in seconds</td>
<td>Number</td>
<td>4.5</td>
</tr>
<tr>
<td>icon</td>
<td>icon of notify</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>placement</td>
<td>position of notify,one of<code>top-right</code> <code>top-center</code> <code>top-left</code> <code>bottom-right</code> <code>bottom-center</code> <code>bottom-left</code></td>
<td>String</td>
<td>top-right</td>
</tr>
<tr>
<td>closable</td>
<td>Whether or not the notify can be closed</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>transition</td>
<td>transition effect，accepted value: <router-link to="/en/components/transition" exact="">Transition</router-link></td>
<td>String</td>
<td>-</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    basicNotify() {
      this.$notify.open({content: 'You clicked me!',});
    },
    primaryNotify() {
      this.$notify.open({content: 'You clicked me!', type: 'primary'});
    },
    infoNotify() {
      this.$notify.info({content: 'You clicked me!'});
    },
    successNotify() {
      this.$notify.success({content: 'You clicked me!'});
    },
    warningNotify() {
      this.$notify.warning({content: 'You clicked me!'});
    },
    dangerNotify() {
      this.$notify.open({content: 'You clicked me!', type: 'danger'});
    },
    loadingNotify() {
      this.$notify.open({content: 'Loading...', type: 'loading'});
    },
    durationNotify() {
      this.$notify.open({
        content: 'auto closed in 10s！',
        duration: 10000,
      });
    },
    iconNotify() {
      this.$notify.open({
        content: 'customize icon！',
        icon: 'smile-o',
      });
    },
    placementNotify() {
      this.$notify.open({
        content: 'customize position！',
        icon: 'smile-o',
        placement: 'top-center',
      });
    },
    transitionNotify() {
      this.$notify.open({
        content: 'customize transition！',
        icon: 'smile-o',
        placement: 'top-center',
        transition: 'bounce',
        type: 'danger',
      });
    },
  },
};
</script>