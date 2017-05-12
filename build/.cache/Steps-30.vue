<template><section><h2 id="steps-bu-zou-tiao"><a class="header-anchor" href="#steps-bu-zou-tiao" aria-hidden="true">¶</a> Steps 步骤条</h2>
<p>步骤条，常用于分步操作</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;steps :current=\&quot;0\&quot; type=\&quot;line\&quot; prev-text=\&quot;上一步\&quot; next-text=\&quot;下一步\&quot;&gt;\n  &lt;step title=\&quot;标题\&quot; description=\&quot;举头望明月\&quot;&gt;\n    &lt;p&gt;1.床前明月光，疑是地上霜。举头望明月，低头思故乡&lt;/p&gt;\n  &lt;/step&gt;\n  &lt;step title=\&quot;Eating\&quot; description=\&quot;春晓\&quot;&gt;\n    &lt;p&gt;2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。&lt;/p&gt;\n  &lt;/step&gt;\n  &lt;step title=\&quot;Swimming\&quot; description=\&quot;春夜喜雨\&quot;&gt;\n    &lt;p&gt;3.好雨知时节，当春乃发生。随风潜入夜，润物细无声&lt;/p&gt;\n  &lt;/step&gt;\n&lt;/steps&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><steps :current="0" type="line" prev-text="上一步" next-text="下一步">
  <step title="标题" description="举头望明月">
    <p>1.床前明月光，疑是地上霜。举头望明月，低头思故乡</p>
  </step>
  <step title="Eating" description="春晓">
    <p>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。</p>
  </step>
  <step title="Swimming" description="春夜喜雨">
    <p>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声</p>
  </step>
</steps>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li><code>current</code> 设置当前进行到第几步</li>
<li><code>prev-text / next-text</code> 设置按钮文字</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">steps</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"line"</span> <span class="hljs-attr">prev-text</span>=<span class="hljs-string">"上一步"</span> <span class="hljs-attr">next-text</span>=<span class="hljs-string">"下一步"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"标题"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"举头望明月"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>1.床前明月光，疑是地上霜。举头望明月，低头思故乡<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Eating"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春晓"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Swimming"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春夜喜雨"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">steps</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * `current` 设置当前进行到第几步
  * `prev-text / next-text` 设置按钮文字
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">steps</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"line"</span> <span class="hljs-attr">prev-text</span>=<span class="hljs-string">"上一步"</span> <span class="hljs-attr">next-text</span>=<span class="hljs-string">"下一步"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"标题"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"举头望明月"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>1.床前明月光，疑是地上霜。举头望明月，低头思故乡<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Eating"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春晓"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Swimming"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春夜喜雨"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">steps</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;steps :current=\&quot;0\&quot; type=\&quot;pills\&quot;&gt;\n  &lt;step title=\&quot;标题\&quot; description=\&quot;举头望明月\&quot;&gt;\n    &lt;p&gt;1.床前明月光，疑是地上霜。举头望明月，低头思故乡&lt;/p&gt;\n  &lt;/step&gt;\n  &lt;step title=\&quot;Eating\&quot; description=\&quot;春晓\&quot;&gt;\n    &lt;p&gt;2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。&lt;/p&gt;\n  &lt;/step&gt;\n  &lt;step title=\&quot;Swimming\&quot; description=\&quot;春夜喜雨\&quot;&gt;\n    &lt;p&gt;3.好雨知时节，当春乃发生。随风潜入夜，润物细无声&lt;/p&gt;\n  &lt;/step&gt;\n&lt;/steps&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><steps :current="0" type="pills">
  <step title="标题" description="举头望明月">
    <p>1.床前明月光，疑是地上霜。举头望明月，低头思故乡</p>
  </step>
  <step title="Eating" description="春晓">
    <p>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。</p>
  </step>
  <step title="Swimming" description="春夜喜雨">
    <p>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声</p>
  </step>
</steps>
</div>
                    <div slot="description"><h4 id="ling-yi-chong-yang-shi"><a class="header-anchor" href="#ling-yi-chong-yang-shi" aria-hidden="true">¶</a> 另一种样式</h4>
<ul>
<li>目前有两种样式，通过 <code>type</code> 设置</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">steps</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"pills"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"标题"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"举头望明月"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>1.床前明月光，疑是地上霜。举头望明月，低头思故乡<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Eating"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春晓"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Swimming"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春夜喜雨"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">steps</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 另一种样式
  * 目前有两种样式，通过 `type` 设置
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">steps</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"0"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"pills"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"标题"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"举头望明月"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>1.床前明月光，疑是地上霜。举头望明月，低头思故乡<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Eating"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春晓"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Swimming"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春夜喜雨"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">steps</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;steps :current=\&quot;current\&quot; type=\&quot;line\&quot; :show-footer=\&quot;false\&quot;&gt;\n  &lt;step title=\&quot;标题\&quot; description=\&quot;举头望明月\&quot;&gt;\n    &lt;p&gt;1.床前明月光，疑是地上霜。举头望明月，低头思故乡&lt;/p&gt;\n    &lt;p&gt;\n      &lt;button class=\&quot;button is-info\&quot; @click=\&quot;handlePrev\&quot;&gt;上一步&lt;/button&gt;\n      &lt;button class=\&quot;button is-info\&quot; @click=\&quot;handleNext\&quot;&gt;下一步&lt;/button&gt;\n    &lt;/p&gt;\n  &lt;/step&gt;\n  &lt;step title=\&quot;Eating\&quot; description=\&quot;春晓\&quot;&gt;\n    &lt;p&gt;2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。&lt;/p&gt;\n    &lt;p&gt;\n      &lt;button class=\&quot;button is-info\&quot; @click=\&quot;handlePrev\&quot;&gt;上一步&lt;/button&gt;\n      &lt;button class=\&quot;button is-info\&quot; @click=\&quot;handleNext\&quot;&gt;下一步&lt;/button&gt;\n    &lt;/p&gt;\n  &lt;/step&gt;\n  &lt;step title=\&quot;Swimming\&quot; description=\&quot;春夜喜雨\&quot;&gt;\n    &lt;p&gt;3.好雨知时节，当春乃发生。随风潜入夜，润物细无声&lt;/p&gt;\n    &lt;p&gt;\n      &lt;button class=\&quot;button is-info\&quot; @click=\&quot;handlePrev\&quot;&gt;上一步&lt;/button&gt;\n      &lt;button class=\&quot;button is-info\&quot; @click=\&quot;handleNext\&quot;&gt;下一步&lt;/button&gt;\n    &lt;/p&gt;\n  &lt;/step&gt;\n&lt;/steps&gt;\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    data() {\n      return {\n        current: 0,\n      };\n    },\n\n    methods: {\n      handleNext() {\n        this.current &lt;= 3 &amp;&amp; this.current++;\n        this.$notify.open({content: '自定义回调'});\n      },\n      handlePrev() {\n        this.current &gt;= 0 &amp;&amp; this.current--;\n        this.$notify.info({content: '自定义回调'});\n      }\n    }\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><steps :current="current" type="line" :show-footer="false">
  <step title="标题" description="举头望明月">
    <p>1.床前明月光，疑是地上霜。举头望明月，低头思故乡</p>
    <p>
      <button class="button is-info" @click="handlePrev">上一步</button>
      <button class="button is-info" @click="handleNext">下一步</button>
    </p>
  </step>
  <step title="Eating" description="春晓">
    <p>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。</p>
    <p>
      <button class="button is-info" @click="handlePrev">上一步</button>
      <button class="button is-info" @click="handleNext">下一步</button>
    </p>
  </step>
  <step title="Swimming" description="春夜喜雨">
    <p>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声</p>
    <p>
      <button class="button is-info" @click="handlePrev">上一步</button>
      <button class="button is-info" @click="handleNext">下一步</button>
    </p>
  </step>
</steps>


</div>
                    <div slot="description"><h4 id="kong-zhi"><a class="header-anchor" href="#kong-zhi" aria-hidden="true">¶</a> 控制</h4>
<ul>
<li><code>current</code> 设置当前进行到第几步</li>
<li><code>prev-text / next-text</code> 设置按钮文字</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">steps</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"current"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"line"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"标题"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"举头望明月"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>1.床前明月光，疑是地上霜。举头望明月，低头思故乡<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handlePrev"</span>&gt;</span>上一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handleNext"</span>&gt;</span>下一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Eating"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春晓"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handlePrev"</span>&gt;</span>上一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handleNext"</span>&gt;</span>下一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Swimming"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春夜喜雨"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handlePrev"</span>&gt;</span>上一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handleNext"</span>&gt;</span>下一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">steps</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">current</span>: <span class="hljs-number">0</span>,
      };
    },

    <span class="hljs-attr">methods</span>: {
      handleNext() {
        <span class="hljs-keyword">this</span>.current &lt;= <span class="hljs-number">3</span> &amp;&amp; <span class="hljs-keyword">this</span>.current++;
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'自定义回调'</span>});
      },
      handlePrev() {
        <span class="hljs-keyword">this</span>.current &gt;= <span class="hljs-number">0</span> &amp;&amp; <span class="hljs-keyword">this</span>.current--;
        <span class="hljs-keyword">this</span>.$notify.info({<span class="hljs-attr">content</span>: <span class="hljs-string">'自定义回调'</span>});
      }
    }
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 控制
  * `current` 设置当前进行到第几步
  * `prev-text / next-text` 设置按钮文字
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">steps</span> <span class="hljs-attr">:current</span>=<span class="hljs-string">"current"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"line"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"标题"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"举头望明月"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>1.床前明月光，疑是地上霜。举头望明月，低头思故乡<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handlePrev"</span>&gt;</span>上一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handleNext"</span>&gt;</span>下一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Eating"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春晓"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>2.春眠不觉晓，处处闻啼鸟。夜来风雨声，花落知多少。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handlePrev"</span>&gt;</span>上一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handleNext"</span>&gt;</span>下一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">step</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Swimming"</span> <span class="hljs-attr">description</span>=<span class="hljs-string">"春夜喜雨"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>3.好雨知时节，当春乃发生。随风潜入夜，润物细无声<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handlePrev"</span>&gt;</span>上一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"handleNext"</span>&gt;</span>下一步<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">step</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">steps</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    data() {
      <span class="hljs-keyword">return</span> {
        <span class="hljs-attr">current</span>: <span class="hljs-number">0</span>,
      };
    },

    <span class="hljs-attr">methods</span>: {
      handleNext() {
        <span class="hljs-keyword">this</span>.current &lt;= <span class="hljs-number">3</span> &amp;&amp; <span class="hljs-keyword">this</span>.current++;
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'自定义回调'</span>});
      },
      handlePrev() {
        <span class="hljs-keyword">this</span>.current &gt;= <span class="hljs-number">0</span> &amp;&amp; <span class="hljs-keyword">this</span>.current--;
        <span class="hljs-keyword">this</span>.$notify.info({<span class="hljs-attr">content</span>: <span class="hljs-string">'自定义回调'</span>});
      }
    }
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
<td>显示样式，可选值为<code>pills</code> <code>line</code></td>
<td>String</td>
<td><code>pills</code></td>
</tr>
<tr>
<td>current</td>
<td>当前第几步</td>
<td>Number</td>
<td>0</td>
</tr>
<tr>
<td>prevText</td>
<td>上一步的按钮文字</td>
<td>String</td>
<td><code>Prev</code></td>
</tr>
<tr>
<td>nextText</td>
<td>下一步的按钮文字</td>
<td>String</td>
<td><code>Next</code></td>
</tr>
<tr>
<td>on-prev</td>
<td>上一步回调</td>
<td>Function</td>
<td>无</td>
</tr>
<tr>
<td>on-next</td>
<td>下一步回调</td>
<td>Function</td>
<td>无</td>
</tr>
<tr>
<td>show-footer</td>
<td>是否显示footer栏，不显示的话可以通过<code>current</code>自己控制上一步下一步</td>
<td>Boolean</td>
<td>true</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  data() {
    return {
      current: 0,
    };
  },

  methods: {
    handleNext() {
      this.current <= 3 && this.current++;
      this.$notify.open({content: '自定义回调'});
    },
    handlePrev() {
      this.current >= 0 && this.current--;
      this.$notify.info({content: '自定义回调'});
    }
  }
};
</script>