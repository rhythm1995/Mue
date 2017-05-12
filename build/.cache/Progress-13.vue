<template><section><h2 id="progressbar-jin-du-tiao"><a class="header-anchor" href="#progressbar-jin-du-tiao" aria-hidden="true">¶</a> ProgressBar 进度条</h2>
<p>为当前工作流程和动作提供实时反馈</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;progress-bar :percent=\&quot;45\&quot; type=\&quot;primary\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;30\&quot; type=\&quot;info\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;50\&quot; type=\&quot;success\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;60\&quot; type=\&quot;danger\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;65\&quot; type=\&quot;warning\&quot;&gt;&lt;/progress-bar&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><progress-bar :percent="45" type="primary"></progress-bar>
<progress-bar :percent="30" type="info"></progress-bar>
<progress-bar :percent="50" type="success"></progress-bar>
<progress-bar :percent="60" type="danger"></progress-bar>
<progress-bar :percent="65" type="warning"></progress-bar>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>默认有五种主题颜色，包括<code>primary</code> <code>info</code> <code>success</code> <code>danger</code> <code>warning</code>，通过<code>type</code>来设置</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"45"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"30"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"60"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"65"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 默认有五种主题颜色，包括`primary` `info` `success` `danger` `warning`，通过`type`来设置
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"45"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"30"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"60"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"65"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"warning"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;progress-bar :percent=\&quot;45\&quot; type=\&quot;primary\&quot; :striped=\&quot;true\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;30\&quot; type=\&quot;info\&quot; :striped=\&quot;true\&quot; :animated=\&quot;true\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;50\&quot; type=\&quot;success\&quot; :showinfo=\&quot;true\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;50\&quot; type=\&quot;success\&quot; size=\&quot;small\&quot; :showinfo=\&quot;true\&quot; :info-inside=\&quot;false\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;60\&quot; type=\&quot;danger\&quot; size=\&quot;large\&quot; :showinfo=\&quot;true\&quot; :format=\&quot;percentFormat\&quot;&gt;&lt;/progress-bar&gt;\n&lt;progress-bar :percent=\&quot;percent\&quot; type=\&quot;info\&quot; :showinfo=\&quot;true\&quot; :striped=\&quot;true\&quot; :animated=\&quot;true\&quot;&gt;&lt;/progress-bar&gt;\n&lt;p class=\&quot;control has-addons\&quot;&gt;\n  &lt;a class=\&quot;button\&quot; @click=\&quot;percentPlus\&quot;&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;&lt;i class=\&quot;fa fa-plus\&quot;&gt;&lt;/i&gt;&lt;/span&gt;\n  &lt;/a&gt;\n  &lt;a class=\&quot;button\&quot; @click=\&quot;percentMinus\&quot;&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;&lt;i class=\&quot;fa fa-minus\&quot;&gt;&lt;/i&gt;&lt;/span&gt;\n  &lt;/a&gt;\n&lt;/p&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        percent: 10,\n      };\n    },\n\n    methods: {\n      percentFormat(val) {\n        return `Completed ${val}%`;\n      },\n      percentPlus() {\n        if (this.percent &lt; 100) {\n          this.percent += 10;\n        }\n      },\n      percentMinus() {\n        if (this.percent &gt; 0) {\n          this.percent -= 10;\n        }\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><progress-bar :percent="45" type="primary" :striped="true"></progress-bar>
<progress-bar :percent="30" type="info" :striped="true" :animated="true"></progress-bar>
<progress-bar :percent="50" type="success" :showinfo="true"></progress-bar>
<progress-bar :percent="50" type="success" size="small" :showinfo="true" :info-inside="false"></progress-bar>
<progress-bar :percent="60" type="danger" size="large" :showinfo="true" :format="percentFormat"></progress-bar>
<progress-bar :percent="percent" type="info" :showinfo="true" :striped="true" :animated="true"></progress-bar>
<p class="control has-addons">
  <a class="button" @click="percentPlus">
    <span class="icon is-small"><i class="fa fa-plus"></i></span>
  </a>
  <a class="button" @click="percentMinus">
    <span class="icon is-small"><i class="fa fa-minus"></i></span>
  </a>
</p>

</div>
                    <div slot="description"><h4 id="geng-duo-she-zhi"><a class="header-anchor" href="#geng-duo-she-zhi" aria-hidden="true">¶</a> 更多设置</h4>
<ul>
<li><code>striped</code> 设置为true，显示彩带样式</li>
<li><code>animated</code> 设置为true，显示动态进度条</li>
<li><code>showinfo</code> 设置为true，显示当前进度数值</li>
<li><code>info-inside</code> 设置为false，进度信息会显示在进度条外</li>
<li>通过<code>size</code>设置progress bar的宽度，除了默认值外有 <code>small</code> <code>medium</code> <code>large</code></li>
<li>通过设置format内容模板函数，自定义信息显示的内容</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"45"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">:striped</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"30"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">:striped</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:info-inside</span>=<span class="hljs-string">"false"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"60"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"large"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:format</span>=<span class="hljs-string">"percentFormat"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"percent"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:striped</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"percentPlus"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-plus"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"percentMinus"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-minus"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">percent</span>: <span class="hljs-number">10</span>,
      };
    },

    <span class="hljs-attr">methods</span>: {
      percentFormat(val) {
        <span class="hljs-keyword">return</span> <span class="hljs-string">`Completed <span class="hljs-subst">${val}</span>%`</span>;
      },
      percentPlus() {
        <span class="hljs-keyword">if</span> (<span class="hljs-keyword">this</span>.percent &lt; <span class="hljs-number">100</span>) {
          <span class="hljs-keyword">this</span>.percent += <span class="hljs-number">10</span>;
        }
      },
      percentMinus() {
        <span class="hljs-keyword">if</span> (<span class="hljs-keyword">this</span>.percent &gt; <span class="hljs-number">0</span>) {
          <span class="hljs-keyword">this</span>.percent -= <span class="hljs-number">10</span>;
        }
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 更多设置
  * `striped` 设置为true，显示彩带样式
  * `animated` 设置为true，显示动态进度条
  * `showinfo` 设置为true，显示当前进度数值
  * `info-inside` 设置为false，进度信息会显示在进度条外
  * 通过`size`设置progress bar的宽度，除了默认值外有 `small` `medium` `large`
  * 通过设置format内容模板函数，自定义信息显示的内容
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"45"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"primary"</span> <span class="hljs-attr">:striped</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"30"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">:striped</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"success"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:info-inside</span>=<span class="hljs-string">"false"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"60"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"danger"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"large"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:format</span>=<span class="hljs-string">"percentFormat"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">progress-bar</span> <span class="hljs-attr">:percent</span>=<span class="hljs-string">"percent"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"info"</span> <span class="hljs-attr">:showinfo</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:striped</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:animated</span>=<span class="hljs-string">"true"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">progress-bar</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"percentPlus"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-plus"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"percentMinus"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-minus"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">percent</span>: <span class="hljs-number">10</span>,
      };
    },

    <span class="hljs-attr">methods</span>: {
      percentFormat(val) {
        <span class="hljs-keyword">return</span> <span class="hljs-string">`Completed <span class="hljs-subst">${val}</span>%`</span>;
      },
      percentPlus() {
        <span class="hljs-keyword">if</span> (<span class="hljs-keyword">this</span>.percent &lt; <span class="hljs-number">100</span>) {
          <span class="hljs-keyword">this</span>.percent += <span class="hljs-number">10</span>;
        }
      },
      percentMinus() {
        <span class="hljs-keyword">if</span> (<span class="hljs-keyword">this</span>.percent &gt; <span class="hljs-number">0</span>) {
          <span class="hljs-keyword">this</span>.percent -= <span class="hljs-number">10</span>;
        }
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
<td>size</td>
<td>大小，可选值为<code>small</code> <code>medium</code> <code>large</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>percent</td>
<td>百分比</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>showinfo</td>
<td>是否显示进度数值</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>info-inside</td>
<td>进度信息的显示是否在进度条内部</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>format</td>
<td>显示信息的模板函数</td>
<td>function(percent)</td>
<td><code>percent =&gt; percent + '%'</code></td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  data() {
    return {
      percent: 10,
    };
  },

  methods: {
    percentFormat(val) {
      return `Completed ${val}%`;
    },
    percentPlus() {
      if (this.percent < 100) {
        this.percent += 10;
      }
    },
    percentMinus() {
      if (this.percent > 0) {
        this.percent -= 10;
      }
    },
  },
};
</script>