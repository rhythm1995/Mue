<template><section><h2 id="datepicker-ri-qi-shi-jian-xuan-ze-qi"><a class="header-anchor" href="#datepicker-ri-qi-shi-jian-xuan-ze-qi" aria-hidden="true">¶</a> DatePicker 日期时间选择器</h2>
<p>日期时间选择器,基于轻量且强大的 <a href="https://chmln.github.io/flatpickr/">flatpickr</a></p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;Select Date..\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;默认值及数据绑定\&quot; :options=\&quot;dateOptions\&quot; v-model=\&quot;date1\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;column is-2\&quot;&gt;{{ date1 }}&lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;开启时间选择..\&quot; :options=\&quot;{enableTime: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;格式化时间..\&quot; :options=\&quot;{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;设置可选范围..\&quot; :options=\&quot;{minDate: new Date(), maxDate: '2017-12-20',}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;datepicker placeholder=\&quot;按钮选择\&quot; :options=\&quot;{wrap: true, clickOpens: false,}\&quot; class=\&quot;is-grouped\&quot;&gt;&lt;/datepicker&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-3">
    <datepicker placeholder="Select Date.."></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="默认值及数据绑定" :options="dateOptions" v-model="date1"></datepicker>
  </div>
  <div class="column is-2">{{ date1 }}</div>
</div>

<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="开启时间选择.." :options="{enableTime: true}"></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-4">
    <datepicker placeholder="格式化时间.." :options="{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}"></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-4">
    <datepicker placeholder="设置可选范围.." :options="{minDate: new Date(), maxDate: '2017-12-20',}"></datepicker>
  </div>
</div>

<datepicker placeholder="按钮选择" :options="{wrap: true, clickOpens: false,}" class="is-grouped"></datepicker>

</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>可使用 <code>v-model</code> 绑定数据</li>
<li>通过配置项 <code>enableTime</code> 开启时间选择</li>
<li>可通过 <code>minDate</code> <code>maxDate</code> 配置可选时间范围</li>
<li>丰富的格式化选项</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Select Date.."</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"默认值及数据绑定"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"dateOptions"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"date1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-2"</span>&gt;</span><span>{{</span> date1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"开启时间选择.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"格式化时间.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"设置可选范围.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{minDate: new Date(), maxDate: '2017-12-20',}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"按钮选择"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{wrap: true, clickOpens: false,}"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"is-grouped"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 基本
  * 可使用 `v-model` 绑定数据
  * 通过配置项 `enableTime` 开启时间选择
  * 可通过 `minDate` `maxDate` 配置可选时间范围
  * 丰富的格式化选项
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Select Date.."</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"默认值及数据绑定"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"dateOptions"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"date1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-2"</span>&gt;</span><span>{{</span> date1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"开启时间选择.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"格式化时间.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"设置可选范围.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{minDate: new Date(), maxDate: '2017-12-20',}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"按钮选择"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{wrap: true, clickOpens: false,}"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"is-grouped"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>

</code></pre>
</demo-box>
<h4 id="jin-zhi-huo-kai-qi-mou-ge-ri-qi-de-xuan-ze"><a class="header-anchor" href="#jin-zhi-huo-kai-qi-mou-ge-ri-qi-de-xuan-ze" aria-hidden="true">¶</a> 禁止或开启某个日期的选择</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;奇数日期不可选\&quot; :options=\&quot;disableOddDays\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;七日内可选\&quot; :options=\&quot;enableOddDays\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        disableOddDays: {\n          disable: [\n            function(date){ // disable odd days\n              return date.getDate()%2 &gt; 0;\n            }\n          ]\n        },\n        enableOddDays: {\n          enable: [\n            {\n              from: \&quot;today\&quot;,\n              to: new Date().fp_incr(7) // 7 days from now\n            }\n          ]\n        },\n      };\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component">
<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="奇数日期不可选" :options="disableOddDays"></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="七日内可选" :options="enableOddDays"></datepicker>
  </div>
</div>



</div>
                    <div slot="description"><h4 id="jin-zhi-kai-qi"><a class="header-anchor" href="#jin-zhi-kai-qi" aria-hidden="true">¶</a> 禁止 &amp; 开启</h4>
<ul>
<li>可通过配置禁用某些日期的选择(接受函数配置)</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"奇数日期不可选"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"disableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"七日内可选"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"enableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">disableOddDays</span>: {
          <span class="hljs-attr">disable</span>: [
            <span class="hljs-function"><span class="hljs-keyword">function</span>(<span class="hljs-params">date</span>)</span>{ <span class="hljs-comment">// disable odd days</span>
              <span class="hljs-keyword">return</span> date.getDate()%<span class="hljs-number">2</span> &gt; <span class="hljs-number">0</span>;
            }
          ]
        },
        <span class="hljs-attr">enableOddDays</span>: {
          <span class="hljs-attr">enable</span>: [
            {
              <span class="hljs-attr">from</span>: <span class="hljs-string">"today"</span>,
              <span class="hljs-attr">to</span>: <span class="hljs-keyword">new</span> <span class="hljs-built_in">Date</span>().fp_incr(<span class="hljs-number">7</span>) <span class="hljs-comment">// 7 days from now</span>
            }
          ]
        },
      };
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 禁止 & 开启
  * 可通过配置禁用某些日期的选择(接受函数配置)
</summary>
<pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"奇数日期不可选"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"disableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"七日内可选"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"enableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">disableOddDays</span>: {
          <span class="hljs-attr">disable</span>: [
            <span class="hljs-function"><span class="hljs-keyword">function</span>(<span class="hljs-params">date</span>)</span>{ <span class="hljs-comment">// disable odd days</span>
              <span class="hljs-keyword">return</span> date.getDate()%<span class="hljs-number">2</span> &gt; <span class="hljs-number">0</span>;
            }
          ]
        },
        <span class="hljs-attr">enableOddDays</span>: {
          <span class="hljs-attr">enable</span>: [
            {
              <span class="hljs-attr">from</span>: <span class="hljs-string">"today"</span>,
              <span class="hljs-attr">to</span>: <span class="hljs-keyword">new</span> <span class="hljs-built_in">Date</span>().fp_incr(<span class="hljs-number">7</span>) <span class="hljs-comment">// 7 days from now</span>
            }
          ]
        },
      };
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

</code></pre>
</demo-box>
<h4 id="shi-jian-xuan-ze"><a class="header-anchor" href="#shi-jian-xuan-ze" aria-hidden="true">¶</a> 时间选择</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;时间选择\&quot; :options=\&quot;{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="时间选择" :options="{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="shi-jian-xuan-ze"><a class="header-anchor" href="#shi-jian-xuan-ze" aria-hidden="true">¶</a> 时间选择</h4>
<ul>
<li>设置 <code>weekNumbers</code> 为 true</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"时间选择"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 时间选择
  * 设置 `weekNumbers` 为 true
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"时间选择"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="ri-qi-fan-wei"><a class="header-anchor" href="#ri-qi-fan-wei" aria-hidden="true">¶</a> 日期范围</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;范围\&quot; :options=\&quot;{mode: 'range'}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-3">
    <datepicker placeholder="范围" :options="{mode: 'range'}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="fan-wei"><a class="header-anchor" href="#fan-wei" aria-hidden="true">¶</a> 范围</h4>
<ul>
<li>设置<code>mode</code>为range</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"范围"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'range'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 范围
  * 设置`mode`为range
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"范围"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'range'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="tong-shi-xuan-ze-duo-ge-ri-qi"><a class="header-anchor" href="#tong-shi-xuan-ze-duo-ge-ri-qi" aria-hidden="true">¶</a> 同时选择多个日期</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-5\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;多选\&quot; :options=\&quot;{mode: 'multiple'}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-5">
    <datepicker placeholder="多选" :options="{mode: 'multiple'}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="duo-xuan"><a class="header-anchor" href="#duo-xuan" aria-hidden="true">¶</a> 多选</h4>
<ul>
<li>设置 <code>mode</code> 为multiple</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-5"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"多选"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'multiple'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 多选
  * 设置 `mode` 为multiple
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-5"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"多选"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'multiple'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="inline-mo-shi"><a class="header-anchor" href="#inline-mo-shi" aria-hidden="true">¶</a> inline模式</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;inline模式\&quot; :options=\&quot;{inline: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="inline模式" :options="{inline: true}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="inline"><a class="header-anchor" href="#inline" aria-hidden="true">¶</a> inline</h4>
<ul>
<li>设置 <code>inline</code> 为 true</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"inline模式"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### inline
  * 设置 `inline` 为 true
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"inline模式"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="xian-shi-di-ji-zhou"><a class="header-anchor" href="#xian-shi-di-ji-zhou" aria-hidden="true">¶</a> 显示第几周</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;显示周\&quot; :options=\&quot;{inline: true, weekNumbers: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="显示周" :options="{inline: true, weekNumbers: true}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id=""><a class="header-anchor" href="#" aria-hidden="true">¶</a> </h4>
<ul>
<li>设置 <code>weekNumbers</code> 为 true</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"显示周"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true, weekNumbers: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  ####
  * 设置 `weekNumbers` 为 true
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"显示周"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true, weekNumbers: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="guo-ji-hua"><a class="header-anchor" href="#guo-ji-hua" aria-hidden="true">¶</a> 国际化</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;国际化\&quot; :options=\&quot;localeOption\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n\n&quot;,&quot;script&quot;:&quot;\nimport { zh } from 'flatpickr/dist/l10n/zh';\n\nexport default {\n  data() {\n    return {\n      localeOption: {\n        locale: zh,\n      },\n    };\n  },\n};\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="国际化" :options="localeOption"></datepicker>
  </div>
</div>


</div>
                    <div slot="description"><h4 id="l10n"><a class="header-anchor" href="#l10n" aria-hidden="true">¶</a> l10n</h4>
<ul>
<li>通过 <code>locale</code> 设置语言</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"国际化"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"localeOption"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">import</span> { zh } <span class="hljs-keyword">from</span> <span class="hljs-string">'flatpickr/dist/l10n/zh'</span>;

<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  data() {
    <span class="hljs-keyword">return</span> {
      <span class="hljs-attr">localeOption</span>: {
        <span class="hljs-attr">locale</span>: zh,
      },
    };
  },
};
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### l10n
  * 通过 `locale` 设置语言
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"国际化"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"localeOption"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">import</span> { zh } <span class="hljs-keyword">from</span> <span class="hljs-string">'flatpickr/dist/l10n/zh'</span>;

<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  data() {
    <span class="hljs-keyword">return</span> {
      <span class="hljs-attr">localeOption</span>: {
        <span class="hljs-attr">locale</span>: zh,
      },
    };
  },
};
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="geng-duo"><a class="header-anchor" href="#geng-duo" aria-hidden="true">¶</a> 更多</h4>
<p><code>注</code> flatpickr有更详尽的配置说明，请参见 <a href="https://chmln.github.io/flatpickr/">flatpickr</a></p>

</section></template>

<script>
import { zh } from 'flatpickr/dist/l10n/zh';

export default {
  data() {
    return {
      dateOptions: {
      },
      dateOptions2: {
        wrap: true,
        clickOpens: false,
      },
      disableOddDays: {
        disable: [
          function(date){ // disable odd days
            return date.getDate()%2 > 0;
          }
        ]
      },
      enableOddDays: {
        enable: [
          {
            from: "today",
            to: new Date().fp_incr(7) // 7 days from now
          }
        ]
      },
      date1: '2016-10-20',
      localeOption: {
        locale: zh,
      },
    };
  },
};
</script>