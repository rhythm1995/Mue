<template><section><h1>Vue-Blu</h1>
<p>Vue-Blu是基于<a href="http://www.vuejs.org/">Vuejs</a>和<a href="http://bulma.io/">Bulma</a>开发的开源UI组件库。旨在为PC端的前端开发(特别是中后台产品)提供一个快速且灵活的解决方案。</p>
<h2 id="te-xing"><a class="header-anchor" href="#te-xing" aria-hidden="true">¶</a> 特性</h2>
<ul>
<li>基于 npm + webpack + babel 开发，支持 ES2015</li>
<li>全面、灵活且强大的ui组件，API友好</li>
<li>样式基于Bulma框架(Flexbox based)，布局简单、响应式</li>
<li>可定制化</li>
</ul>
<h2 id="an-zhuang"><a class="header-anchor" href="#an-zhuang" aria-hidden="true">¶</a> 安装</h2>
<pre><code class="language-bash">$ npm install vue-blu --save
</code></pre>
<h2 id="kuai-su-kai-shi"><a class="header-anchor" href="#kuai-su-kai-shi" aria-hidden="true">¶</a> 快速开始</h2>
<pre><code>import Vue from 'vue'
import VueBlu from 'vue-blu'
import 'vue-blu/dist/css/vue-blu.min.css'

Vue.use(VueBlu)

</code></pre>
<h2 id="shi-li"><a class="header-anchor" href="#shi-li" aria-hidden="true">¶</a> 示例</h2>
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
<li>默认有五种主题颜色的tag，包括<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code>，通过<code>type</code>来设置</li>
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
  * 默认有五种主题颜色的tag，包括`primary` `info` `success` `danger` `warning`，通过`type`来设置
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span>Tag Primary<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span>&gt;</span>Tag Info<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span>Tag Success<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span>&gt;</span>Tag Danger<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span>&gt;</span>Tag Warning<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">tag</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">color</span>=<span class="hljs-string">"#f50"</span> <span class="hljs-attr">:closable</span>=<span class="hljs-string">"true"</span>&gt;</span>Tag Color<span class="hljs-tag">&lt;/<span class="hljs-name">tag</span>&gt;</span>
</code></pre>
</demo-box>
<h2 id="ban-ben"><a class="header-anchor" href="#ban-ben" aria-hidden="true">¶</a> 版本</h2>
<ul>
<li>0.1.8 beta</li>
</ul>
<h2 id="jian-rong-xing"><a class="header-anchor" href="#jian-rong-xing" aria-hidden="true">¶</a> 兼容性</h2>
<ul>
<li>基于Vuejs2.x</li>
<li>现代浏览器及IE10+</li>
</ul>
<h2 id="xiang-guan-lian-jie"><a class="header-anchor" href="#xiang-guan-lian-jie" aria-hidden="true">¶</a> 相关链接</h2>
<ul>
<li><a href="http://www.vuejs.org">Vuejs官方</a></li>
<li><a href="http://bulma.io/">Bulma官方</a></li>
</ul>
<h2 id="credits"><a class="header-anchor" href="#credits" aria-hidden="true">¶</a> Credits</h2>
<ul>
<li><a href="https://github.com/vuejs/vue">Vue</a></li>
<li><a href="https://github.com/jgthms/bulma">Bulma</a></li>
<li><a href="https://github.com/vue-bulma/vue-admin">vue-admin</a> 最早的想法起源于此</li>
<li><a href="https://github.com/ant-design/ant-design">ant-design</a> 参考借鉴了某些API的设计</li>
<li><a href="http://github.com/elemefe">element-ui</a> 参考了开发文档的组织方式(vue-markdown-loader)</li>
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