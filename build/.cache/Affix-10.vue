<template><section><h2 id="affix-gu-ding"><a class="header-anchor" href="#affix-gu-ding" aria-hidden="true">¶</a> Affix 固钉</h2>
<p>将元素钉在固定位置，常用于顶部菜单或者侧边菜单</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;affix&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;固定在顶部&lt;/button&gt;\n&lt;/affix&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><affix>
  <button class="button is-primary">固定在顶部</button>
</affix>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<p>最简单的用法</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>固定在顶部<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  最简单的用法
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>固定在顶部<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;affix :offset=\&quot;200\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;固定距离顶部200px的位置&lt;/button&gt;\n&lt;/affix&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><affix :offset="200">
  <button class="button is-primary">固定距离顶部200px的位置</button>
</affix>
</div>
                    <div slot="description"><h4 id="she-zhi-pian-yi-liang"><a class="header-anchor" href="#she-zhi-pian-yi-liang" aria-hidden="true">¶</a> 设置偏移量</h4>
<p>设置距离顶部达到指定距离时触发</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"200"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>固定距离顶部200px的位置<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 设置偏移量
  设置距离顶部达到指定距离时触发
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"200"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>固定距离顶部200px的位置<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div id=\&quot;parent\&quot; style=\&quot;height: 120px; text-align: center\&quot;&gt;\n  &lt;affix :offset=\&quot;0\&quot; boundary=\&quot;#parent\&quot;&gt;\n    &lt;button class=\&quot;button is-primary\&quot;&gt;在指定容器内浮动&lt;/button&gt;\n  &lt;/affix&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div id="parent" style="height: 120px; text-align: center">
  <affix :offset="0" boundary="#parent">
    <button class="button is-primary">在指定容器内浮动</button>
  </affix>
</div>
</div>
                    <div slot="description"><h4 id="she-zhi-bian-jie-fu-rong-qi"><a class="header-anchor" href="#she-zhi-bian-jie-fu-rong-qi" aria-hidden="true">¶</a> 设置边界父容器</h4>
<p>指定父容器ID后，affix元素会在父容器内浮动，即给浮动元素指定了边界</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"parent"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"height: 120px; text-align: center"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">boundary</span>=<span class="hljs-string">"#parent"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>在指定容器内浮动<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 设置边界父容器
  指定父容器ID后，affix元素会在父容器内浮动，即给浮动元素指定了边界
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">id</span>=<span class="hljs-string">"parent"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"height: 120px; text-align: center"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:offset</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">boundary</span>=<span class="hljs-string">"#parent"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>在指定容器内浮动<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div style=\&quot;text-align: right\&quot;&gt;\n  &lt;affix :on-affix=\&quot;onAffixed\&quot;&gt;\n    &lt;button class=\&quot;button is-primary\&quot;&gt;触发回调&lt;/button&gt;\n  &lt;/affix&gt;\n&lt;/div&gt;\n\n&quot;,&quot;script&quot;:&quot;\nexport default {\n  methods: {\n    onAffixed(status) {\n      this.$notify.open({\n        type: 'success',\n        title: `回调状态${status}`,\n      });\n    },\n  },\n};\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div style="text-align: right">
  <affix :on-affix="onAffixed">
    <button class="button is-primary">触发回调</button>
  </affix>
</div>

</div>
                    <div slot="description"><h4 id="hui-diao-han-shu"><a class="header-anchor" href="#hui-diao-han-shu" aria-hidden="true">¶</a> 回调函数</h4>
<p>可设置固定状态改变时触发的回调函数</p>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"text-align: right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:on-affix</span>=<span class="hljs-string">"onAffixed"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>触发回调<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  <span class="hljs-attr">methods</span>: {
    onAffixed(status) {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">title</span>: <span class="hljs-string">`回调状态<span class="hljs-subst">${status}</span>`</span>,
      });
    },
  },
};
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 回调函数
  可设置固定状态改变时触发的回调函数
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"text-align: right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">affix</span> <span class="hljs-attr">:on-affix</span>=<span class="hljs-string">"onAffixed"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>触发回调<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">affix</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  <span class="hljs-attr">methods</span>: {
    onAffixed(status) {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">title</span>: <span class="hljs-string">`回调状态<span class="hljs-subst">${status}</span>`</span>,
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
<td>offset</td>
<td>距离窗口顶部达到指定偏移量后触发</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>boundary</td>
<td>设置 <code>Affix</code> 的活动范围，值为affix上级元素的id(可以是父元素，也可以是父元素的父元素...)</td>
<td>String(#parent)</td>
<td></td>
</tr>
<tr>
<td>on-affix</td>
<td>固定状态改变时触发的回调函数</td>
<td>Function(affixed)</td>
<td>无</td>
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