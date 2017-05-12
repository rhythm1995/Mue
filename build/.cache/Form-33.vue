<template><section><h2 id="form-biao-dan"><a class="header-anchor" href="#form-biao-dan" aria-hidden="true">¶</a> Form 表单</h2>
<p>对于表单的样式和布局等展现方面的实现，我们认为原生的HTML元素加CSS足以满足，特别是有了Bulma。所以Blu的Form基本全部依赖于Bulma。对于某些功能性的表单组件如AutoComplete、Select，
Blu会另有封装。</p>
<p>下面介绍一下Form，内容主要来自于 <a href="http://bulma.io/documentation/elements/form/">http://bulma.io/documentation/elements/form/</a></p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;label class=\&quot;label\&quot;&gt;Name&lt;/label&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Text input\&quot;&gt;\n&lt;/p&gt;\n&lt;label class=\&quot;label\&quot;&gt;Username&lt;/label&gt;\n&lt;p class=\&quot;control has-icon has-icon-right\&quot;&gt;\n  &lt;input class=\&quot;input is-success\&quot; type=\&quot;text\&quot; placeholder=\&quot;Text input\&quot; value=\&quot;bulma\&quot;&gt;\n  &lt;i class=\&quot;fa fa-check\&quot;&gt;&lt;/i&gt;\n  &lt;span class=\&quot;help is-success\&quot;&gt;This username is available&lt;/span&gt;\n&lt;/p&gt;\n&lt;label class=\&quot;label\&quot;&gt;Email&lt;/label&gt;\n&lt;p class=\&quot;control has-icon has-icon-right\&quot;&gt;\n  &lt;input class=\&quot;input is-danger\&quot; type=\&quot;text\&quot; placeholder=\&quot;Email input\&quot; value=\&quot;hello@\&quot;&gt;\n  &lt;i class=\&quot;fa fa-warning\&quot;&gt;&lt;/i&gt;\n  &lt;span class=\&quot;help is-danger\&quot;&gt;This email is invalid&lt;/span&gt;\n&lt;/p&gt;\n&lt;label class=\&quot;label\&quot;&gt;Subject&lt;/label&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;span class=\&quot;select\&quot;&gt;\n    &lt;select&gt;\n      &lt;option&gt;Select dropdown&lt;/option&gt;\n      &lt;option&gt;With options&lt;/option&gt;\n    &lt;/select&gt;\n  &lt;/span&gt;\n&lt;/p&gt;\n&lt;label class=\&quot;label\&quot;&gt;Message&lt;/label&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;textarea class=\&quot;textarea\&quot; placeholder=\&quot;Textarea\&quot;&gt;&lt;/textarea&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;label class=\&quot;checkbox\&quot;&gt;\n    &lt;input type=\&quot;checkbox\&quot;&gt;\n    Remember me\n  &lt;/label&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;label class=\&quot;radio\&quot;&gt;\n    &lt;input type=\&quot;radio\&quot; name=\&quot;question\&quot;&gt;\n    Yes\n  &lt;/label&gt;\n  &lt;label class=\&quot;radio\&quot;&gt;\n    &lt;input type=\&quot;radio\&quot; name=\&quot;question\&quot;&gt;\n    No\n  &lt;/label&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Submit&lt;/button&gt;\n  &lt;button class=\&quot;button is-link\&quot;&gt;Cancel&lt;/button&gt;\n&lt;/p&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><label class="label">Name</label>
<p class="control">
  <input class="input" type="text" placeholder="Text input">
</p>
<label class="label">Username</label>
<p class="control has-icon has-icon-right">
  <input class="input is-success" type="text" placeholder="Text input" value="bulma">
  <i class="fa fa-check"></i>
  <span class="help is-success">This username is available</span>
</p>
<label class="label">Email</label>
<p class="control has-icon has-icon-right">
  <input class="input is-danger" type="text" placeholder="Email input" value="hello@">
  <i class="fa fa-warning"></i>
  <span class="help is-danger">This email is invalid</span>
</p>
<label class="label">Subject</label>
<p class="control">
  <span class="select">
    <select>
      <option>Select dropdown</option>
      <option>With options</option>
    </select>
  </span>
</p>
<label class="label">Message</label>
<p class="control">
  <textarea class="textarea" placeholder="Textarea"></textarea>
</p>
<p class="control">
  <label class="checkbox">
    <input type="checkbox">
    Remember me
  </label>
</p>
<p class="control">
  <label class="radio">
    <input type="radio" name="question">
    Yes
  </label>
  <label class="radio">
    <input type="radio" name="question">
    No
  </label>
</p>
<p class="control">
  <button class="button is-primary">Submit</button>
  <button class="button is-link">Cancel</button>
</p>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>使用 <code>control</code> 作为元素的容器</li>
<li>使用 <code>.label</code> <code>.input</code> <code>.textarea</code> <code>.select</code> <code>.checkbox</code> <code>.radio</code> <code>.button</code> <code>.help</code> 控制相应表单元素的样式</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Name<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Text input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Username<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon has-icon-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-success"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Text input"</span> <span class="hljs-attr">value</span>=<span class="hljs-string">"bulma"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-check"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"help is-success"</span>&gt;</span>This username is available<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Email<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon has-icon-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-danger"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email input"</span> <span class="hljs-attr">value</span>=<span class="hljs-string">"hello@"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-warning"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"help is-danger"</span>&gt;</span>This email is invalid<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Subject<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>Select dropdown<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>With options<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Message<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">textarea</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"textarea"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Textarea"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">textarea</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"checkbox"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"checkbox"</span>&gt;</span>
    Remember me
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span>&gt;</span>
    Yes
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span>&gt;</span>
    No
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Submit<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-link"</span>&gt;</span>Cancel<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * 使用 `control` 作为元素的容器
  * 使用 `.label` `.input` `.textarea` `.select` `.checkbox` `.radio` `.button` `.help` 控制相应表单元素的样式
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Name<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Text input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Username<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon has-icon-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-success"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Text input"</span> <span class="hljs-attr">value</span>=<span class="hljs-string">"bulma"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-check"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"help is-success"</span>&gt;</span>This username is available<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Email<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon has-icon-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-danger"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email input"</span> <span class="hljs-attr">value</span>=<span class="hljs-string">"hello@"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-warning"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"help is-danger"</span>&gt;</span>This email is invalid<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Subject<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>Select dropdown<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>With options<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Message<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">textarea</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"textarea"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Textarea"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">textarea</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"checkbox"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"checkbox"</span>&gt;</span>
    Remember me
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span>&gt;</span>
    Yes
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span>&gt;</span>
    No
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Submit<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-link"</span>&gt;</span>Cancel<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="color-yan-se"><a class="header-anchor" href="#color-yan-se" aria-hidden="true">¶</a> Color 颜色</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;p class=\&quot;control\&quot;&gt;\n  &lt;input class=\&quot;input is-primary\&quot; type=\&quot;text\&quot; placeholder=\&quot;Primary input\&quot;&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;input class=\&quot;input is-info\&quot; type=\&quot;text\&quot; placeholder=\&quot;Info input\&quot;&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;input class=\&quot;input is-success\&quot; type=\&quot;text\&quot; placeholder=\&quot;Success input\&quot;&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;input class=\&quot;input is-warning\&quot; type=\&quot;text\&quot; placeholder=\&quot;Warning input\&quot;&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;input class=\&quot;input is-danger\&quot; type=\&quot;text\&quot; placeholder=\&quot;Danger input\&quot;&gt;\n&lt;/p&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><p class="control">
  <input class="input is-primary" type="text" placeholder="Primary input">
</p>
<p class="control">
  <input class="input is-info" type="text" placeholder="Info input">
</p>
<p class="control">
  <input class="input is-success" type="text" placeholder="Success input">
</p>
<p class="control">
  <input class="input is-warning" type="text" placeholder="Warning input">
</p>
<p class="control">
  <input class="input is-danger" type="text" placeholder="Danger input">
</p>
</div>
                    <div slot="description"><h4 id="yan-se"><a class="header-anchor" href="#yan-se" aria-hidden="true">¶</a> 颜色</h4>
<ul>
<li>五种主题颜色 <code>is-primary</code> <code>is-info</code> <code>is-success</code> <code>is-warning</code> <code>is-danger</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-primary"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Primary input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-info"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Info input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-success"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Success input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-warning"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Warning input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-danger"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Danger input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 颜色
  * 五种主题颜色 `is-primary` `is-info` `is-success` `is-warning` `is-danger`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-primary"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Primary input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-info"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Info input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-success"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Success input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-warning"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Warning input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-danger"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Danger input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="size-da-xiao"><a class="header-anchor" href="#size-da-xiao" aria-hidden="true">¶</a> Size 大小</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;p class=\&quot;control has-icon\&quot;&gt;\n  &lt;input class=\&quot;input is-small\&quot; type=\&quot;email\&quot; placeholder=\&quot;Email\&quot;&gt;\n  &lt;i class=\&quot;fa fa-envelope\&quot;&gt;&lt;/i&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control has-icon\&quot;&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;email\&quot; placeholder=\&quot;Email\&quot;&gt;\n  &lt;i class=\&quot;fa fa-envelope\&quot;&gt;&lt;/i&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control has-icon\&quot;&gt;\n  &lt;input class=\&quot;input is-medium\&quot; type=\&quot;email\&quot; placeholder=\&quot;Email\&quot;&gt;\n  &lt;i class=\&quot;fa fa-envelope\&quot;&gt;&lt;/i&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control has-icon\&quot;&gt;\n  &lt;input class=\&quot;input is-large\&quot; type=\&quot;email\&quot; placeholder=\&quot;Email\&quot;&gt;\n  &lt;i class=\&quot;fa fa-envelope\&quot;&gt;&lt;/i&gt;\n&lt;/p&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><p class="control has-icon">
  <input class="input is-small" type="email" placeholder="Email">
  <i class="fa fa-envelope"></i>
</p>
<p class="control has-icon">
  <input class="input" type="email" placeholder="Email">
  <i class="fa fa-envelope"></i>
</p>
<p class="control has-icon">
  <input class="input is-medium" type="email" placeholder="Email">
  <i class="fa fa-envelope"></i>
</p>
<p class="control has-icon">
  <input class="input is-large" type="email" placeholder="Email">
  <i class="fa fa-envelope"></i>
</p>
</div>
                    <div slot="description"><h4 id="chi-cun"><a class="header-anchor" href="#chi-cun" aria-hidden="true">¶</a> 尺寸</h4>
<ul>
<li>针对input和select有效 <code>is-small</code> <code>空</code> <code>is-medium</code> <code>is-large</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-small"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-medium"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-large"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 尺寸
  * 针对input和select有效 `is-small` `空` `is-medium` `is-large`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-small"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-medium"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-large"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="state-zhuang-tai"><a class="header-anchor" href="#state-zhuang-tai" aria-hidden="true">¶</a> State 状态</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;p class=\&quot;control is-loading\&quot;&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Loading input\&quot;&gt;\n&lt;/p&gt;\n\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Disabled input\&quot; disabled&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;textarea class=\&quot;textarea\&quot; placeholder=\&quot;Disabled textarea\&quot; disabled&gt;&lt;/textarea&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;label class=\&quot;checkbox is-disabled\&quot;&gt;\n    &lt;input type=\&quot;checkbox\&quot; disabled&gt;\n    Remember me\n  &lt;/label&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;label class=\&quot;radio is-disabled\&quot;&gt;\n    &lt;input type=\&quot;radio\&quot; name=\&quot;question\&quot; disabled&gt;\n    Yes\n  &lt;/label&gt;\n  &lt;label class=\&quot;radio is-disabled\&quot;&gt;\n    &lt;input type=\&quot;radio\&quot; name=\&quot;question\&quot; disabled&gt;\n    No\n  &lt;/label&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot; disabled&gt;Submit&lt;/button&gt;\n  &lt;button class=\&quot;button\&quot; disabled&gt;Cancel&lt;/button&gt;\n&lt;/p&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><p class="control is-loading">
  <input class="input" type="text" placeholder="Loading input">
</p>

<p class="control">
  <input class="input" type="text" placeholder="Disabled input" disabled>
</p>
<p class="control">
  <textarea class="textarea" placeholder="Disabled textarea" disabled></textarea>
</p>
<p class="control">
  <label class="checkbox is-disabled">
    <input type="checkbox" disabled>
    Remember me
  </label>
</p>
<p class="control">
  <label class="radio is-disabled">
    <input type="radio" name="question" disabled>
    Yes
  </label>
  <label class="radio is-disabled">
    <input type="radio" name="question" disabled>
    No
  </label>
</p>
<p class="control">
  <button class="button is-primary" disabled>Submit</button>
  <button class="button" disabled>Cancel</button>
</p>

</div>
                    <div slot="description"><h4 id="zhuang-tai"><a class="header-anchor" href="#zhuang-tai" aria-hidden="true">¶</a> 状态</h4>
<ul>
<li>loading 或 disabled <code>is-loading</code> <code>is-disabled</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-loading"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Loading input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Disabled input"</span> <span class="hljs-attr">disabled</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">textarea</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"textarea"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Disabled textarea"</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">textarea</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"checkbox is-disabled"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"checkbox"</span> <span class="hljs-attr">disabled</span>&gt;</span>
    Remember me
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio is-disabled"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span> <span class="hljs-attr">disabled</span>&gt;</span>
    Yes
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio is-disabled"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span> <span class="hljs-attr">disabled</span>&gt;</span>
    No
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">disabled</span>&gt;</span>Submit<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">disabled</span>&gt;</span>Cancel<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 状态
  * loading 或 disabled `is-loading` `is-disabled`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-loading"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Loading input"</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Disabled input"</span> <span class="hljs-attr">disabled</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">textarea</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"textarea"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Disabled textarea"</span> <span class="hljs-attr">disabled</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">textarea</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"checkbox is-disabled"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"checkbox"</span> <span class="hljs-attr">disabled</span>&gt;</span>
    Remember me
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio is-disabled"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span> <span class="hljs-attr">disabled</span>&gt;</span>
    Yes
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"radio is-disabled"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"radio"</span> <span class="hljs-attr">name</span>=<span class="hljs-string">"question"</span> <span class="hljs-attr">disabled</span>&gt;</span>
    No
  <span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">disabled</span>&gt;</span>Submit<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span> <span class="hljs-attr">disabled</span>&gt;</span>Cancel<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

</code></pre>
</demo-box>
<h4 id="icon-pei-he-font-awesome"><a class="header-anchor" href="#icon-pei-he-font-awesome" aria-hidden="true">¶</a> Icon 配合Font Awesome</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;p class=\&quot;control has-icon\&quot;&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;email\&quot; placeholder=\&quot;Email\&quot;&gt;\n  &lt;i class=\&quot;fa fa-envelope\&quot;&gt;&lt;/i&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control has-icon\&quot;&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;password\&quot; placeholder=\&quot;Password\&quot;&gt;\n  &lt;i class=\&quot;fa fa-lock\&quot;&gt;&lt;/i&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control\&quot;&gt;\n  &lt;button class=\&quot;button is-success\&quot;&gt;\n    Login\n  &lt;/button&gt;\n&lt;/p&gt;\n\n&lt;p class=\&quot;control has-icon has-icon-right\&quot;&gt;\n  &lt;input class=\&quot;input is-small\&quot; type=\&quot;email\&quot; placeholder=\&quot;Email\&quot;&gt;\n  &lt;i class=\&quot;fa fa-check\&quot;&gt;&lt;/i&gt;\n&lt;/p&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><p class="control has-icon">
  <input class="input" type="email" placeholder="Email">
  <i class="fa fa-envelope"></i>
</p>
<p class="control has-icon">
  <input class="input" type="password" placeholder="Password">
  <i class="fa fa-lock"></i>
</p>
<p class="control">
  <button class="button is-success">
    Login
  </button>
</p>

<p class="control has-icon has-icon-right">
  <input class="input is-small" type="email" placeholder="Email">
  <i class="fa fa-check"></i>
</p>
</div>
                    <div slot="description"><h4 id="icon"><a class="header-anchor" href="#icon" aria-hidden="true">¶</a> Icon</h4>
<ul>
<li>通过 <code>has-icon</code> 轻松设置icon</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"password"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Password"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-lock"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span>&gt;</span>
    Login
  <span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon has-icon-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-small"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-check"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Icon
  * 通过 `has-icon` 轻松设置icon
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-envelope"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"password"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Password"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-lock"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-success"</span>&gt;</span>
    Login
  <span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-icon has-icon-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-small"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-check"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="addons-biao-dan-zu-he"><a class="header-anchor" href="#addons-biao-dan-zu-he" aria-hidden="true">¶</a> Addons 表单组合</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;p class=\&quot;control has-addons\&quot;&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Find a repository\&quot;&gt;\n  &lt;a class=\&quot;button is-info\&quot;&gt;\n    Search\n  &lt;/a&gt;\n&lt;/p&gt;\n&lt;!-- happy divider line --&gt;\n&lt;p class=\&quot;control has-addons\&quot;&gt;\n  &lt;span class=\&quot;select\&quot;&gt;\n    &lt;select&gt;\n      &lt;option&gt;$&lt;/option&gt;\n      &lt;option&gt;£&lt;/option&gt;\n      &lt;option&gt;€&lt;/option&gt;\n    &lt;/select&gt;\n  &lt;/span&gt;\n  &lt;input class=\&quot;input is-expanded\&quot; type=\&quot;text\&quot; placeholder=\&quot;Amount of money\&quot;&gt;\n  &lt;a class=\&quot;button\&quot;&gt;\n    Transfer\n  &lt;/a&gt;\n&lt;/p&gt;\n\n&lt;p&gt;对齐方式&lt;/p&gt;\n&lt;p class=\&quot;control has-addons has-addons-centered\&quot;&gt;\n  &lt;span class=\&quot;select\&quot;&gt;\n    &lt;select&gt;\n      &lt;option&gt;$&lt;/option&gt;\n      &lt;option&gt;£&lt;/option&gt;\n      &lt;option&gt;€&lt;/option&gt;\n    &lt;/select&gt;\n  &lt;/span&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Amount of money\&quot;&gt;\n  &lt;a class=\&quot;button is-primary\&quot;&gt;\n    Transfer\n  &lt;/a&gt;\n&lt;/p&gt;\n&lt;p class=\&quot;control has-addons has-addons-right\&quot;&gt;\n  &lt;span class=\&quot;select\&quot;&gt;\n    &lt;select&gt;\n      &lt;option&gt;$&lt;/option&gt;\n      &lt;option&gt;£&lt;/option&gt;\n      &lt;option&gt;€&lt;/option&gt;\n    &lt;/select&gt;\n  &lt;/span&gt;\n  &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Amount of money\&quot;&gt;\n  &lt;a class=\&quot;button is-primary\&quot;&gt;\n    Transfer\n  &lt;/a&gt;\n&lt;/p&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><p class="control has-addons">
  <input class="input" type="text" placeholder="Find a repository">
  <a class="button is-info">
    Search
  </a>
</p>
<!-- happy divider line -->
<p class="control has-addons">
  <span class="select">
    <select>
      <option>$</option>
      <option>£</option>
      <option>€</option>
    </select>
  </span>
  <input class="input is-expanded" type="text" placeholder="Amount of money">
  <a class="button">
    Transfer
  </a>
</p>

<p>对齐方式</p>
<p class="control has-addons has-addons-centered">
  <span class="select">
    <select>
      <option>$</option>
      <option>£</option>
      <option>€</option>
    </select>
  </span>
  <input class="input" type="text" placeholder="Amount of money">
  <a class="button is-primary">
    Transfer
  </a>
</p>
<p class="control has-addons has-addons-right">
  <span class="select">
    <select>
      <option>$</option>
      <option>£</option>
      <option>€</option>
    </select>
  </span>
  <input class="input" type="text" placeholder="Amount of money">
  <a class="button is-primary">
    Transfer
  </a>
</p>
</div>
                    <div slot="description"><h4 id="zu-he"><a class="header-anchor" href="#zu-he" aria-hidden="true">¶</a> 组合</h4>
<ul>
<li>通过 <code>has-addons</code> 设置表单与按钮等元素的组合显示</li>
<li>通过 <code>has-addons-centered</code> <code>has-addons-right</code> 设置对齐</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Find a repository"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>
    Search
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-comment">&lt;!-- happy divider line --&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-expanded"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    Transfer
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>对齐方式<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons has-addons-centered"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    Transfer
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons has-addons-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    Transfer
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 组合
  * 通过 `has-addons` 设置表单与按钮等元素的组合显示
  * 通过 `has-addons-centered` `has-addons-right` 设置对齐
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Find a repository"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>
    Search
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-comment">&lt;!-- happy divider line --&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input is-expanded"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>
    Transfer
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>对齐方式<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons has-addons-centered"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    Transfer
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons has-addons-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    Transfer
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="biao-dan-zu"><a class="header-anchor" href="#biao-dan-zu" aria-hidden="true">¶</a> 表单组</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;control is-grouped\&quot;&gt;\n  &lt;p class=\&quot;control is-expanded\&quot;&gt;\n    &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Find a repository\&quot;&gt;\n  &lt;/p&gt;\n  &lt;p class=\&quot;control\&quot;&gt;\n    &lt;a class=\&quot;button is-info\&quot;&gt;\n      Search\n    &lt;/a&gt;\n  &lt;/p&gt;\n  &lt;p class=\&quot;control has-addons has-addons-right\&quot;&gt;\n  &lt;span class=\&quot;select\&quot;&gt;\n    &lt;select&gt;\n      &lt;option&gt;$&lt;/option&gt;\n      &lt;option&gt;£&lt;/option&gt;\n      &lt;option&gt;€&lt;/option&gt;\n    &lt;/select&gt;\n  &lt;/span&gt;\n    &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Amount of money\&quot;&gt;\n    &lt;a class=\&quot;button is-primary\&quot;&gt;\n      Transfer\n    &lt;/a&gt;\n  &lt;/p&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="control is-grouped">
  <p class="control is-expanded">
    <input class="input" type="text" placeholder="Find a repository">
  </p>
  <p class="control">
    <a class="button is-info">
      Search
    </a>
  </p>
  <p class="control has-addons has-addons-right">
  <span class="select">
    <select>
      <option>$</option>
      <option>£</option>
      <option>€</option>
    </select>
  </span>
    <input class="input" type="text" placeholder="Amount of money">
    <a class="button is-primary">
      Transfer
    </a>
  </p>
</div>
</div>
                    <div slot="description"><h4 id="biao-dan-zu"><a class="header-anchor" href="#biao-dan-zu" aria-hidden="true">¶</a> 表单组</h4>
<ul>
<li>如果你想把 <code>control</code> 容器放在一行， 可以通过在<code>.control</code> 上添加 <code>is-grouped</code>样式实现</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-grouped"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-expanded"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Find a repository"</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>
      Search
    <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons has-addons-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
      Transfer
    <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 表单组
  * 如果你想把 `control` 容器放在一行， 可以通过在`.control` 上添加 `is-grouped`样式实现
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-grouped"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-expanded"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Find a repository"</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>
      Search
    <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control has-addons has-addons-right"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>$<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>£<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>€<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Amount of money"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
      Transfer
    <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h4 id="shui-ping-biao-dan"><a class="header-anchor" href="#shui-ping-biao-dan" aria-hidden="true">¶</a> 水平表单</h4>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;control is-horizontal\&quot;&gt;\n  &lt;div class=\&quot;control-label\&quot;&gt;\n    &lt;label class=\&quot;label\&quot;&gt;From&lt;/label&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;control is-grouped\&quot;&gt;\n    &lt;p class=\&quot;control is-expanded\&quot;&gt;\n      &lt;input class=\&quot;input\&quot; type=\&quot;text\&quot; placeholder=\&quot;Name\&quot;&gt;\n    &lt;/p&gt;\n    &lt;p class=\&quot;control is-expanded\&quot;&gt;\n      &lt;input class=\&quot;input\&quot; type=\&quot;email\&quot; placeholder=\&quot;Email\&quot;&gt;\n    &lt;/p&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&lt;div class=\&quot;control is-horizontal\&quot;&gt;\n  &lt;div class=\&quot;control-label\&quot;&gt;\n    &lt;label class=\&quot;label\&quot;&gt;Subject&lt;/label&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;control\&quot;&gt;\n    &lt;div class=\&quot;select is-fullwidth\&quot;&gt;\n      &lt;select&gt;\n        &lt;option&gt;General enquiry&lt;/option&gt;\n      &lt;/select&gt;\n    &lt;/div&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&lt;div class=\&quot;control is-horizontal\&quot;&gt;\n  &lt;div class=\&quot;control-label\&quot;&gt;\n    &lt;label class=\&quot;label\&quot;&gt;Question&lt;/label&gt;\n  &lt;/div&gt;\n  &lt;div class=\&quot;control\&quot;&gt;\n    &lt;textarea class=\&quot;textarea\&quot; placeholder=\&quot;Explain how we can help you\&quot;&gt;&lt;/textarea&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="control is-horizontal">
  <div class="control-label">
    <label class="label">From</label>
  </div>
  <div class="control is-grouped">
    <p class="control is-expanded">
      <input class="input" type="text" placeholder="Name">
    </p>
    <p class="control is-expanded">
      <input class="input" type="email" placeholder="Email">
    </p>
  </div>
</div>
<div class="control is-horizontal">
  <div class="control-label">
    <label class="label">Subject</label>
  </div>
  <div class="control">
    <div class="select is-fullwidth">
      <select>
        <option>General enquiry</option>
      </select>
    </div>
  </div>
</div>
<div class="control is-horizontal">
  <div class="control-label">
    <label class="label">Question</label>
  </div>
  <div class="control">
    <textarea class="textarea" placeholder="Explain how we can help you"></textarea>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="shui-ping-biao-dan"><a class="header-anchor" href="#shui-ping-biao-dan" aria-hidden="true">¶</a> 水平表单</h4>
<ul>
<li>在 <code>control</code> 容器上添加 <code>is-horizontal</code></li>
<li>使用 <code>control-label</code> 作为label的容器</li>
<li>使用 <code>control</code> 作为表单元素的容器</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-horizontal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control-label"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>From<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-grouped"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-expanded"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Name"</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-expanded"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-horizontal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control-label"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Subject<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select is-fullwidth"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>General enquiry<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-horizontal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control-label"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Question<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">textarea</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"textarea"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Explain how we can help you"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">textarea</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 水平表单
  * 在 `control` 容器上添加 `is-horizontal`
  * 使用 `control-label` 作为label的容器
  * 使用 `control` 作为表单元素的容器
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-horizontal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control-label"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>From<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-grouped"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-expanded"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"text"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Name"</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-expanded"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">input</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"input"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"email"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Email"</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-horizontal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control-label"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Subject<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"select is-fullwidth"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">select</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">option</span>&gt;</span>General enquiry<span class="hljs-tag">&lt;/<span class="hljs-name">option</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">select</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control is-horizontal"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control-label"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">label</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"label"</span>&gt;</span>Question<span class="hljs-tag">&lt;/<span class="hljs-name">label</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"control"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">textarea</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"textarea"</span> <span class="hljs-attr">placeholder</span>=<span class="hljs-string">"Explain how we can help you"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">textarea</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
</section></template>

