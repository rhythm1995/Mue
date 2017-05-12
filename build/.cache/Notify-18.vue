<template><section><h2 id="tong-zhi"><a class="header-anchor" href="#tong-zhi" aria-hidden="true">¶</a> 通知</h2>
<p>全局的消息提示</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;button class=\&quot;button\&quot; @click=\&quot;basicNotify\&quot;&gt;点击我&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;primaryNotify\&quot;&gt;点击我&lt;/button&gt;\n&lt;button class=\&quot;button is-info\&quot; @click=\&quot;infoNotify\&quot;&gt;点击我&lt;/button&gt;\n&lt;button class=\&quot;button is-success\&quot; @click=\&quot;successNotify\&quot;&gt;点击我&lt;/button&gt;\n&lt;button class=\&quot;button is-warning\&quot; @click=\&quot;warningNotify\&quot;&gt;点击我&lt;/button&gt;\n&lt;button class=\&quot;button is-danger\&quot; @click=\&quot;dangerNotify\&quot;&gt;点击我&lt;/button&gt;\n&lt;button class=\&quot;button is-info\&quot; @click=\&quot;loadingNotify\&quot;&gt;Loading&lt;/button&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      basicNotify() {\n        this.$notify.open({content: '您点击了我！',});\n      },\n      primaryNotify() {\n        this.$notify.open({content: '您点击了我！', type: 'primary'});\n      },\n      infoNotify() {\n        this.$notify.info({content: '您点击了我！'});\n      },\n      successNotify() {\n        this.$notify.success({content: '您点击了我！'});\n      },\n      warningNotify() {\n        this.$notify.warning({content: '您点击了我！'});\n      },\n      dangerNotify() {\n        this.$notify.open({content: '您点击了我！', type: 'danger'});\n      },\n      loadingNotify() {\n        this.$notify.open({content: '命令执行中...', type: 'loading'});\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><button class="button" @click="basicNotify">点击我</button>
<button class="button is-primary" @click="primaryNotify">点击我</button>
<button class="button is-info" @click="infoNotify">点击我</button>
<button class="button is-success" @click="successNotify">点击我</button>
<button class="button is-warning" @click="warningNotify">点击我</button>
<button class="button is-danger" @click="dangerNotify">点击我</button>
<button class="button is-info" @click="loadingNotify">Loading</button>

</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>默认有六种类型，除了default还包括<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code>，通过<code>type</code>来设置，也可通过<code>this.$notify.info({...})</code>的形式直接调用</li>
<li>默认 4.5秒 自动关闭</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"basicNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"primaryNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"infoNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"successNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"warningNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"dangerNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"loadingNotify"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      basicNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>,});
      },
      primaryNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'primary'</span>});
      },
      infoNotify() {
        <span class="hljs-keyword">this</span>.$notify.info({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>});
      },
      successNotify() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>});
      },
      warningNotify() {
        <span class="hljs-keyword">this</span>.$notify.warning({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>});
      },
      dangerNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'danger'</span>});
      },
      loadingNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'命令执行中...'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'loading'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 默认有六种类型，除了default还包括`primary` `info` `success` `danger` `warning`，通过`type`来设置，也可通过`this.$notify.info({...})`的形式直接调用
  * 默认 4.5秒 自动关闭
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"basicNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"primaryNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"infoNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"successNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"warningNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"dangerNotify"</span>&gt;</span>点击我<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"loadingNotify"</span>&gt;</span>Loading<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      basicNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>,});
      },
      primaryNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'primary'</span>});
      },
      infoNotify() {
        <span class="hljs-keyword">this</span>.$notify.info({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>});
      },
      successNotify() {
        <span class="hljs-keyword">this</span>.$notify.success({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>});
      },
      warningNotify() {
        <span class="hljs-keyword">this</span>.$notify.warning({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>});
      },
      dangerNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'您点击了我！'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'danger'</span>});
      },
      loadingNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'命令执行中...'</span>, <span class="hljs-attr">type</span>: <span class="hljs-string">'loading'</span>});
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;button class=\&quot;button\&quot; @click=\&quot;durationNotify\&quot;&gt;10秒关闭&lt;/button&gt;\n&lt;button class=\&quot;button\&quot; @click=\&quot;iconNotify\&quot;&gt;自定义icon&lt;/button&gt;\n&lt;button class=\&quot;button\&quot; @click=\&quot;placementNotify\&quot;&gt;top-center弹出&lt;/button&gt;\n&lt;button class=\&quot;button\&quot; @click=\&quot;transitionNotify\&quot;&gt;自定义transition&lt;/button&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      durationNotify() {\n        this.$notify.open({\n          content: '10秒后自动关闭！',\n          duration: 10000,\n        });\n      },\n      iconNotify() {\n        this.$notify.open({\n          content: '自定义图标！',\n          icon: 'smile-o',\n        });\n      },\n      placementNotify() {\n        this.$notify.open({\n          content: '自定义位置！',\n          icon: 'smile-o',\n          placement: 'top-center',\n        });\n      },\n      transitionNotify() {\n        this.$notify.open({\n          content: '自定义transition！',\n          icon: 'smile-o',\n          placement: 'top-center',\n          transition: 'bounce',\n          type: 'danger',\n        });\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><button class="button" @click="durationNotify">10秒关闭</button>
<button class="button" @click="iconNotify">自定义icon</button>
<button class="button" @click="placementNotify">top-center弹出</button>
<button class="button" @click="transitionNotify">自定义transition</button>

</div>
                    <div slot="description"><h4 id="geng-duo-pei-zhi"><a class="header-anchor" href="#geng-duo-pei-zhi" aria-hidden="true">¶</a> 更多配置</h4>
<ul>
<li>通过<code>duration</code>设置自动关闭的倒计时时间</li>
<li>通过<code>icon</code>设置图标</li>
<li>通过<code>closable</code>设置是否可手动关闭</li>
<li>通过<code>placement</code>设置notify的显示位置,支持<code>top-right</code> <code>top-center</code> <code>top-left</code> <code>bottom-right</code> <code>bottom-center</code> <code>bottom-left</code></li>
<li>通过<code>transition</code> 设置过度效果</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"durationNotify"</span>&gt;</span>10秒关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"iconNotify"</span>&gt;</span>自定义icon<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"placementNotify"</span>&gt;</span>top-center弹出<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"transitionNotify"</span>&gt;</span>自定义transition<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
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
          <span class="hljs-attr">content</span>: <span class="hljs-string">'自定义图标！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
        });
      },
      placementNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'自定义位置！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
        });
      },
      transitionNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'自定义transition！'</span>,
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
  #### 更多配置
  * 通过`duration`设置自动关闭的倒计时时间
  * 通过`icon`设置图标
  * 通过`closable`设置是否可手动关闭
  * 通过`placement`设置notify的显示位置,支持`top-right` `top-center` `top-left` `bottom-right` `bottom-center` `bottom-left`
  * 通过`transition` 设置过度效果
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"durationNotify"</span>&gt;</span>10秒关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"iconNotify"</span>&gt;</span>自定义icon<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"placementNotify"</span>&gt;</span>top-center弹出<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"transitionNotify"</span>&gt;</span>自定义transition<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
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
          <span class="hljs-attr">content</span>: <span class="hljs-string">'自定义图标！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
        });
      },
      placementNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'自定义位置！'</span>,
          <span class="hljs-attr">icon</span>: <span class="hljs-string">'smile-o'</span>,
          <span class="hljs-attr">placement</span>: <span class="hljs-string">'top-center'</span>,
        });
      },
      transitionNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">'自定义transition！'</span>,
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
<th>成员</th>
<th>说明</th>
<th>类型</th>
<th>默认值</th>
</tr>
</thead>
<tbody>
<tr>
<td>type</td>
<td>主题颜色，可选值为<code>default</code> <code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code></td>
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
<td>content</td>
<td>内容</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>duration</td>
<td>倒计时关闭的秒数，单位秒</td>
<td>Number</td>
<td>4.5</td>
</tr>
<tr>
<td>icon</td>
<td>图标</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>placement</td>
<td>notify的位置,可选值<code>top-right</code> <code>top-center</code> <code>top-left</code> <code>bottom-right</code> <code>bottom-center</code> <code>bottom-left</code></td>
<td>String</td>
<td>top-right</td>
</tr>
<tr>
<td>closable</td>
<td>是否可关闭</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>transition</td>
<td>过度效果，可选值见 #link</td>
<td>String</td>
<td>无</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    basicNotify() {
      this.$notify.open({content: '您点击了我！',});
    },
    primaryNotify() {
      this.$notify.open({content: '您点击了我！', type: 'primary'});
    },
    infoNotify() {
      this.$notify.info({content: '您点击了我！'});
    },
    successNotify() {
      this.$notify.success({content: '您点击了我！'});
    },
    warningNotify() {
      this.$notify.warning({content: '您点击了我！'});
    },
    dangerNotify() {
      this.$notify.open({content: '您点击了我！', type: 'danger'});
    },
    loadingNotify() {
      this.$notify.open({content: '命令执行中...', type: 'loading'});
    },
    durationNotify() {
      this.$notify.open({
        content: '10秒后自动关闭！',
        duration: 10000,
      });
    },
    iconNotify() {
      this.$notify.open({
        content: '自定义图标！',
        icon: 'smile-o',
      });
    },
    placementNotify() {
      this.$notify.open({
        content: '自定义位置！',
        icon: 'smile-o',
        placement: 'top-center',
      });
    },
    transitionNotify() {
      this.$notify.open({
        content: '自定义transition！',
        icon: 'smile-o',
        placement: 'top-center',
        transition: 'bounce',
        type: 'danger',
      });
    },
  },
};
</script>