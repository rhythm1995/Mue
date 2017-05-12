<template><section><h1>Vue-Blu</h1>
<p>Vue-Blu is an UI component library base on <a href="http://www.vuejs.org/">Vuejs</a> and <a href="http://bulma.io/">Bulma</a> For
developing fast and powerful web application</p>
<h2 id="feature"><a class="header-anchor" href="#feature" aria-hidden="true">¶</a> Feature</h2>
<ul>
<li>Provides a work flow which is based on npm + webpack + babel，supporting ES2015</li>
<li>High quality UI components, flexible and friendly apis</li>
<li>Flexbox, Responsive</li>
<li>Customizable</li>
</ul>
<h2 id="install"><a class="header-anchor" href="#install" aria-hidden="true">¶</a> Install</h2>
<pre><code class="language-bash">$ npm install vue-blu --save
</code></pre>
<h2 id="quick-start"><a class="header-anchor" href="#quick-start" aria-hidden="true">¶</a> Quick Start</h2>
<pre><code>import Vue from 'vue'
import VueBlu from 'vue-blu'
import 'vue-blu/dist/css/vue-blu.min.css'

Vue.use(VueBlu)

</code></pre>
<h2 id="demo"><a class="header-anchor" href="#demo" aria-hidden="true">¶</a> Demo</h2>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;tag type=\&quot;primary\&quot;&gt;Tag Primary&lt;/tag&gt;\n&lt;tag type=\&quot;info\&quot;&gt;Tag Info&lt;/tag&gt;\n&lt;tag type=\&quot;success\&quot;&gt;Tag Success&lt;/tag&gt;\n&lt;tag type=\&quot;danger\&quot;&gt;Tag Danger&lt;/tag&gt;\n&lt;tag type=\&quot;warning\&quot;&gt;Tag Warning&lt;/tag&gt;\n&lt;tag type=\&quot;primary\&quot; color=\&quot;#f50\&quot; :closable=\&quot;true\&quot;&gt;Tag Color&lt;/tag&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><tag type="primary">Tag Primary</tag>
<tag type="info">Tag Info</tag>
<tag type="success">Tag Success</tag>
<tag type="danger">Tag Danger</tag>
<tag type="warning">Tag Warning</tag>
<tag type="primary" color="#f50" :closable="true">Tag Color</tag>
</div>
                    <div slot="description"><h4 id="tag"><a class="header-anchor" href="#tag" aria-hidden="true">¶</a> Tag</h4>
<ul>
<li>There are 5 types of Tag, <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Tag Primary<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span>&gt;</span>Tag Info<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>Tag Success<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span>&gt;</span>Tag Danger<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span>&gt;</span>Tag Warning<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">color</span>=<span class="hljs-string">"#f50"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag Color<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Tag
  * There are 5 types of Tag, `primary` `info` `success` `danger` `warning`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Tag Primary<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span>&gt;</span>Tag Info<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>Tag Success<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span>&gt;</span>Tag Danger<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span>&gt;</span>Tag Warning<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">color</span>=<span class="hljs-string">"#f50"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag Color<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</demo-box>
<h2 id="version"><a class="header-anchor" href="#version" aria-hidden="true">¶</a> Version</h2>
<ul>
<li>0.1.7 beta</li>
</ul>
<h2 id="compatibility"><a class="header-anchor" href="#compatibility" aria-hidden="true">¶</a> Compatibility</h2>
<ul>
<li>Vuejs(2.1.x)</li>
<li>Modern browsers and IE10+</li>
</ul>
<h2 id="useful-links"><a class="header-anchor" href="#useful-links" aria-hidden="true">¶</a> Useful Links</h2>
<ul>
<li><a href="http://www.vuejs.org">Vuejs</a></li>
<li><a href="http://bulma.io/">Bulma</a></li>
</ul>
<h2 id="credits"><a class="header-anchor" href="#credits" aria-hidden="true">¶</a> Credits</h2>
<p>Blu is inspired or powered by these people or projects so I want to thank them</p>
<ul>
<li><a href="https://github.com/vuejs/vue">Vue</a> great work</li>
<li><a href="https://github.com/jgthms/bulma">Bulma</a> A modern CSS framework based on Flexbox</li>
<li><a href="https://github.com/vue-bulma/vue-admin">vue-admin</a> for the original idea</li>
<li><a href="https://github.com/ant-design/ant-design">ant-design</a> some api design are referenced from this project</li>
<li><a href="http://github.com/elemefe">element-ui</a> for the vue-markdown-loader</li>
</ul>

</section></template>

<script>
export default {
  methods: {
    onAffix(status) {
      console.log(status);
    },
    toggle() {
      this.isShow = !this.isShow;
    },
    openNotify() {
      this.$notify.open({
        title: '提示信息',
        type: 'success',
        duration: 50000,
      });
    },
    click() {
      console.log(this);
    },
  },
  data() {
    return {
      disabled: true,
      tabShow: true,
      isShow: false,
      percent: 45,
    };
  },
};
</script>