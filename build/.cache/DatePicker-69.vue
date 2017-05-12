<template><section><h2 id="datepicker"><a class="header-anchor" href="#datepicker" aria-hidden="true">¶</a> DatePicker</h2>
<p>To select or input a date. Base on <a href="https://chmln.github.io/flatpickr/">flatpickr</a></p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;Select Date..\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;Preloading Dates and two-way binding\&quot; :options=\&quot;dateOptions\&quot; v-model=\&quot;date1\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;column is-2\&quot;&gt;{{ date1 }}&lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;enableTime..\&quot; :options=\&quot;{enableTime: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;Format time..\&quot; :options=\&quot;{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;range..\&quot; :options=\&quot;{minDate: new Date(), maxDate: '2017-12-20',}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;datepicker placeholder=\&quot;Button Trigger\&quot; :options=\&quot;{wrap: true, clickOpens: false,}\&quot; class=\&quot;is-grouped\&quot;&gt;&lt;/datepicker&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-3">
    <datepicker placeholder="Select Date.."></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="Preloading Dates and two-way binding" :options="dateOptions" v-model="date1"></datepicker>
  </div>
  <div class="column is-2">{{ date1 }}</div>
</div>

<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="enableTime.." :options="{enableTime: true}"></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-4">
    <datepicker placeholder="Format time.." :options="{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}"></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-4">
    <datepicker placeholder="range.." :options="{minDate: new Date(), maxDate: '2017-12-20',}"></datepicker>
  </div>
</div>

<datepicker placeholder="Button Trigger" :options="{wrap: true, clickOpens: false,}" class="is-grouped"></datepicker>

</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>two-way binding by <code>v-model</code></li>
<li>Make it a datetime picker by setting <code>enableTime</code></li>
<li>Limit the range of available dates with <code>minDate</code> and <code>maxDate</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Select Date.."</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Preloading Dates and two-way binding"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"dateOptions"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"date1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-2"</span>&gt;</span><span>{{</span> date1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"enableTime.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Format time.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"range.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{minDate: new Date(), maxDate: '2017-12-20',}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Button Trigger"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{wrap: true, clickOpens: false,}"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"is-grouped"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Basic
  * two-way binding by `v-model`
  * Make it a datetime picker by setting `enableTime`
  * Limit the range of available dates with `minDate` and `maxDate`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Select Date.."</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Preloading Dates and two-way binding"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"dateOptions"</span> <span class="hljs-attr">v-model</span>=<span class="hljs-string">"date1"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-2"</span>&gt;</span><span>{{</span> date1 <span>}}</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"enableTime.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Format time.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, altInput: true, altFormat: 'F j, Y h:i K'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"range.."</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{minDate: new Date(), maxDate: '2017-12-20',}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Button Trigger"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{wrap: true, clickOpens: false,}"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"is-grouped"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>

</code></pre>
</demo-box>
<h4 id="enabling-or-disabling-dates"><a class="header-anchor" href="#enabling-or-disabling-dates" aria-hidden="true">¶</a> Enabling or Disabling dates</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;disable odd days\&quot; :options=\&quot;disableOddDays\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;7 days from now\&quot; :options=\&quot;enableOddDays\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        disableOddDays: {\n          disable: [\n            function(date){ // disable odd days\n              return date.getDate()%2 &gt; 0;\n            }\n          ]\n        },\n        enableOddDays: {\n          enable: [\n            {\n              from: \&quot;today\&quot;,\n              to: new Date().fp_incr(7) // 7 days from now\n            }\n          ]\n        },\n      };\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component">
<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="disable odd days" :options="disableOddDays"></datepicker>
  </div>
</div>

<div class="columns">
  <div class="column is-3">
    <datepicker placeholder="7 days from now" :options="enableOddDays"></datepicker>
  </div>
</div>



</div>
                    <div slot="description"><h4 id="enable-disable"><a class="header-anchor" href="#enable-disable" aria-hidden="true">¶</a> enable &amp; disable</h4>
<ul>
<li>Disable or enable a date interval, or a specific date(Boolean functions are also supported)</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"disable odd days"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"disableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"7 days from now"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"enableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
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
  #### enable & disable
  * Disable or enable a date interval, or a specific date(Boolean functions are also supported)
</summary>
<pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"disable odd days"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"disableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"7 days from now"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"enableOddDays"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
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
<h4 id="time-picker"><a class="header-anchor" href="#time-picker" aria-hidden="true">¶</a> Time picker</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;enableTime\&quot; :options=\&quot;{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="enableTime" :options="{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="time-picker"><a class="header-anchor" href="#time-picker" aria-hidden="true">¶</a> time picker</h4>
<ul>
<li>Enables time picker by <code>enableTime</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"enableTime"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### time picker
  * Enables time picker by `enableTime`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"enableTime"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{enableTime: true, enableSeconds: true, noCalendar: true, time_24hr: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="selecting-a-range-of-dates"><a class="header-anchor" href="#selecting-a-range-of-dates" aria-hidden="true">¶</a> Selecting a Range of Dates</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;range\&quot; :options=\&quot;{mode: 'range'}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-3">
    <datepicker placeholder="range" :options="{mode: 'range'}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="range"><a class="header-anchor" href="#range" aria-hidden="true">¶</a> range</h4>
<ul>
<li>Set <code>mode: 'range'</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"range"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'range'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### range
  * Set `mode: 'range'`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"range"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'range'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="selecting-multiple-dates"><a class="header-anchor" href="#selecting-multiple-dates" aria-hidden="true">¶</a> Selecting Multiple Dates</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-5\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;multiple\&quot; :options=\&quot;{mode: 'multiple'}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-5">
    <datepicker placeholder="multiple" :options="{mode: 'multiple'}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="multiple"><a class="header-anchor" href="#multiple" aria-hidden="true">¶</a> multiple</h4>
<ul>
<li>Set <code>mode: 'multiple'</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-5"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"multiple"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'multiple'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### multiple
  * Set `mode: 'multiple'`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-5"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"multiple"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{mode: 'multiple'}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="inline-calendar"><a class="header-anchor" href="#inline-calendar" aria-hidden="true">¶</a> Inline Calendar</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;inline mode\&quot; :options=\&quot;{inline: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="inline mode" :options="{inline: true}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="inline"><a class="header-anchor" href="#inline" aria-hidden="true">¶</a> inline</h4>
<ul>
<li>Set <code>inline: true</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"inline mode"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### inline
  * Set `inline: true`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"inline mode"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="show-weeks"><a class="header-anchor" href="#show-weeks" aria-hidden="true">¶</a> Show weeks</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;show weeks\&quot; :options=\&quot;{inline: true, weekNumbers: true}\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="show weeks" :options="{inline: true, weekNumbers: true}"></datepicker>
  </div>
</div>
</div>
                    <div slot="description"><h4 id=""><a class="header-anchor" href="#" aria-hidden="true">¶</a> </h4>
<ul>
<li>Set <code>weekNumbers: true</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"show weeks"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true, weekNumbers: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  ####
  * Set `weekNumbers: true`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"show weeks"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"{inline: true, weekNumbers: true}"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="localization"><a class="header-anchor" href="#localization" aria-hidden="true">¶</a> Localization</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot;&gt;\n  &lt;div class=\&quot;column is-4\&quot;&gt;\n    &lt;datepicker placeholder=\&quot;Localization\&quot; :options=\&quot;localeOption\&quot;&gt;&lt;/datepicker&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n\n\n&quot;,&quot;script&quot;:&quot;\nimport { zh } from 'flatpickr/dist/l10n/zh';\n\nexport default {\n  data() {\n    return {\n      localeOption: {\n        locale: zh,\n      },\n    };\n  },\n};\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns">
  <div class="column is-4">
    <datepicker placeholder="Localization" :options="localeOption"></datepicker>
  </div>
</div>


</div>
                    <div slot="description"><h4 id="l10n"><a class="header-anchor" href="#l10n" aria-hidden="true">¶</a> l10n</h4>
<ul>
<li>Over 25 languages are available.</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Localization"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"localeOption"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
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
  * Over 25 languages are available.
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-4"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">datepicker</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Localization"</span> <span class="hljs-attr">:options</span>=<span class="hljs-string">"localeOption"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">datepicker</span>&gt;</span>
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
<h4 id="more"><a class="header-anchor" href="#more" aria-hidden="true">¶</a> More</h4>
<p><code>Note</code> For more information，Please refer to <a href="https://chmln.github.io/flatpickr/">flatpickr</a></p>
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
<td>options</td>
<td>DatePicker config (<a href="https://chmln.github.io/flatpickr/">Documentation</a> )</td>
<td>Object</td>
<td>-</td>
</tr>
<tr>
<td>name</td>
<td>name of input</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>placeholder</td>
<td>placeholder of the datepicker</td>
<td>String</td>
<td>-</td>
</tr>
</tbody>
</table>

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