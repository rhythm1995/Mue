<template><section><h2 id="pagination-fen-ye"><a class="header-anchor" href="#pagination-fen-ye" aria-hidden="true">¶</a> Pagination 分页</h2>
<p>分页</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;pagination :total=\&quot;50\&quot;&gt;&lt;/pagination&gt;\n&lt;br&gt;\n&lt;pagination :total=\&quot;800\&quot; :current=\&quot;5\&quot;&gt;&lt;/pagination&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><pagination :total="50"></pagination>
<br>
<pagination :total="800" :current="5"></pagination>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>通过 <code>total</code> 设置条目数，自动完成分页</li>
<li><code>current</code> 设置默认打开第几页</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"50"</span> &gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"5"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 通过 `total` 设置条目数，自动完成分页
  * `current` 设置默认打开第几页
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"50"</span> &gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"5"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="xiao-chi-cun-ban"><a class="header-anchor" href="#xiao-chi-cun-ban" aria-hidden="true">¶</a> 小尺寸版</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;pagination :total=\&quot;800\&quot; :current=\&quot;5\&quot; size=\&quot;small\&quot;&gt;&lt;/pagination&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><pagination :total="800" :current="5" size="small"></pagination>
</div>
                    <div slot="description"><h4 id="size"><a class="header-anchor" href="#size" aria-hidden="true">¶</a> Size</h4>
<ul>
<li>通过 <code>size</code> 设置分页大小</li>
<li><code>current</code> 设置默认打开第几页</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"5"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Size
  * 通过 `size` 设置分页大小
  * `current` 设置默认打开第几页
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"5"</span> <span class="hljs-attr">size</span>=<span class="hljs-string">"small"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="she-zhi-xian-shi-xiang-mu-he-shun-xu"><a class="header-anchor" href="#she-zhi-xian-shi-xiang-mu-he-shun-xu" aria-hidden="true">¶</a> 设置显示项目和顺序</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;pagination :total=\&quot;800\&quot; layout=\&quot;total, pager, sizer\&quot;&gt;&lt;/pagination&gt;\n&lt;br&gt;\n&lt;pagination :total=\&quot;800\&quot; layout=\&quot;pager, sizer, total\&quot;&gt;&lt;/pagination&gt;\n&lt;br&gt;\n&lt;pagination :total=\&quot;800\&quot; layout=\&quot;total,pager\&quot;&gt;&lt;/pagination&gt;\n\n&lt;br&gt;\n&lt;pagination :total=\&quot;800\&quot; layout=\&quot;pager\&quot;&gt;&lt;/pagination&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><pagination :total="800" layout="total, pager, sizer"></pagination>
<br>
<pagination :total="800" layout="pager, sizer, total"></pagination>
<br>
<pagination :total="800" layout="total,pager"></pagination>

<br>
<pagination :total="800" layout="pager"></pagination>

</div>
                    <div slot="description"><h4 id="layout"><a class="header-anchor" href="#layout" aria-hidden="true">¶</a> layout</h4>
<ul>
<li>分页分为 <code>total, pager, sizer, jumper</code> 四个元素，可以任意顺序组合排列这四项</li>
<li>如： <code>layout=&quot;total, pager, sizer&quot;</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"total, pager, sizer"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"pager, sizer, total"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"total,pager"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"pager"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### layout
  * 分页分为 `total, pager, sizer, jumper` 四个元素，可以任意顺序组合排列这四项
  * 如： `layout="total, pager, sizer"`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"total, pager, sizer"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"pager, sizer, total"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"total,pager"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">layout</span>=<span class="hljs-string">"pager"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>

</code></pre>
</demo-box>
<h3 id="pei-zhi"><a class="header-anchor" href="#pei-zhi" aria-hidden="true">¶</a> 配置</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;pagination :total=\&quot;800\&quot; :current=\&quot;5\&quot; :size-options=\&quot;[30, 40, 50]\&quot;&gt;&lt;/pagination&gt;\n&lt;br&gt;\n&lt;pagination :total=\&quot;800\&quot; :page-size=\&quot;15\&quot; :size-options=\&quot;[15, 30, 50]\&quot;&gt;&lt;/pagination&gt;\n&lt;br&gt;\n&lt;pagination :total=\&quot;50\&quot; :change=\&quot;pageCb\&quot;&gt;&lt;/pagination&gt;\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      pageCb(page) {\n        this.$notify.open({\n          content: `当前第${page}页`,\n        });\n      },\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><pagination :total="800" :current="5" :size-options="[30, 40, 50]"></pagination>
<br>
<pagination :total="800" :page-size="15" :size-options="[15, 30, 50]"></pagination>
<br>
<pagination :total="50" :change="pageCb"></pagination>

</div>
                    <div slot="description"><h4 id="pei-zhi"><a class="header-anchor" href="#pei-zhi" aria-hidden="true">¶</a> 配置</h4>
<ul>
<li>通过 <code>size-options</code> 设置分页大小选项</li>
<li><code>change</code> 设置分页回调</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"5"</span> <span class="hljs-attr">:size-options</span>=<span class="hljs-string">"[30, 40, 50]"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:page-size</span>=<span class="hljs-string">"15"</span> <span class="hljs-attr">:size-options</span>=<span class="hljs-string">"[15, 30, 50]"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">:change</span>=<span class="hljs-string">"pageCb"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      pageCb(page) {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">`当前第<span class="hljs-subst">${page}</span>页`</span>,
        });
      },
    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 配置
  * 通过 `size-options` 设置分页大小选项
  * `change` 设置分页回调
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"5"</span> <span class="hljs-attr">:size-options</span>=<span class="hljs-string">"[30, 40, 50]"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"800"</span> <span class="hljs-attr">:page-size</span>=<span class="hljs-string">"15"</span> <span class="hljs-attr">:size-options</span>=<span class="hljs-string">"[15, 30, 50]"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">pagination</span> <span class="hljs-attr">:total</span>=<span class="hljs-string">"50"</span> <span class="hljs-attr">:change</span>=<span class="hljs-string">"pageCb"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">pagination</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      pageCb(page) {
        <span class="hljs-keyword">this</span>.$notify.open({
          <span class="hljs-attr">content</span>: <span class="hljs-string">`当前第<span class="hljs-subst">${page}</span>页`</span>,
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
<td>page-size</td>
<td>每页条数</td>
<td>Number</td>
<td>10</td>
</tr>
<tr>
<td>current</td>
<td>当前页数</td>
<td>Number</td>
<td>1</td>
</tr>
<tr>
<td>size</td>
<td>分页是否是迷你型，可选值为<code>small</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>total</td>
<td>数据总数</td>
<td>Number</td>
<td>无</td>
</tr>
<tr>
<td>layout</td>
<td>分页项目及布局</td>
<td>String</td>
<td><code>'total, pager, sizer, jumper'</code></td>
</tr>
<tr>
<td>align</td>
<td>对齐方式，默认居中，可选值 <code>right</code> <code>left</code></td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>change</td>
<td>分页回调</td>
<td>Function(current)</td>
<td>无</td>
</tr>
<tr>
<td>pageSizeChange</td>
<td>每页条数变化后回调</td>
<td>Function(current, pageSize)</td>
<td>无</td>
</tr>
<tr>
<td>size-options</td>
<td>指定每页显示多少条</td>
<td>Array</td>
<td>无</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  methods: {
    pageCb(page) {
      this.$notify.open({
        content: `当前第${page}页`,
      });
    },
  },
};
</script>