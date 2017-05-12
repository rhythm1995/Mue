<template><section><h2 id="popover"><a class="header-anchor" href="#popover" aria-hidden="true">¶</a> Popover</h2>
<p>The floating card popped by clicking or hovering.</p>
<ul>
<li></li>
</ul>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;popover title=\&quot;Basic Popover\&quot; :always=\&quot;false\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Basic Popover!&lt;/button&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;h4&gt;全面、灵活且强大的ui组件&lt;/h4&gt;\n    &lt;ul&gt;\n      &lt;li&gt;样式基于&lt;strong&gt;Bulma框架&lt;/strong&gt;(Flexbox based)，能够轻松布局并可定制化&lt;/li&gt;\n    &lt;/ul&gt;\n  &lt;/div&gt;\n&lt;/popover&gt;\n\n&lt;popover title=\&quot;Always Popover\&quot; content=\&quot;Duis mollis, est non commodo luctus\&quot; :always=\&quot;true\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Always Popover!&lt;/button&gt;\n&lt;/popover&gt;\n\n&lt;popover title=\&quot;Always Popover\&quot; content=\&quot;Duis mollis, est non commodo luctus\&quot; :disabled=\&quot;true\&quot;&gt;\n  &lt;button class=\&quot;button is-warning\&quot;&gt;Disabled Popover!&lt;/button&gt;\n&lt;/popover&gt;\n\n&lt;popover content=\&quot;No title! Duis mollis, est non commodo luctus\&quot;&gt;\n  &lt;button class=\&quot;button is-info\&quot;&gt;No title!&lt;/button&gt;\n&lt;/popover&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><popover title="Basic Popover" :always="false">
  <button class="button is-primary">Basic Popover!</button>
  <div slot="content">
    <h4>全面、灵活且强大的ui组件</h4>
    <ul>
      <li>样式基于<strong>Bulma框架</strong>(Flexbox based)，能够轻松布局并可定制化</li>
    </ul>
  </div>
</popover>

<popover title="Always Popover" content="Duis mollis, est non commodo luctus" :always="true">
  <button class="button is-primary">Always Popover!</button>
</popover>

<popover title="Always Popover" content="Duis mollis, est non commodo luctus" :disabled="true">
  <button class="button is-warning">Disabled Popover!</button>
</popover>

<popover content="No title! Duis mollis, est non commodo luctus">
  <button class="button is-info">No title!</button>
</popover>

</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Three <code>trigger</code> modes</li>
<li>keep the popover open by setting <code>always=&quot;true&quot;</code></li>
<li>popover can be disabled</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Basic Popover"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Basic Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>全面、灵活且强大的ui组件<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">ul</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span>样式基于<span class="hljs-tag">&lt;<span class="hljs-name">strong</span>&gt;</span>Bulma框架<span class="hljs-tag">&lt;/<span class="hljs-name">strong</span>&gt;</span>(Flexbox based)，能够轻松布局并可定制化<span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">ul</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Always Popover"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Duis mollis, est non commodo luctus"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Always Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Always Popover"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Duis mollis, est non commodo luctus"</span> <span class="hljs-attr">:disabled</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span>&gt;</span>Disabled Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"No title! Duis mollis, est non commodo luctus"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>No title!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Basic
  * Three `trigger` modes
  * keep the popover open by setting `always="true"`
  * popover can be disabled
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Basic Popover"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Basic Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>全面、灵活且强大的ui组件<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">ul</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span>样式基于<span class="hljs-tag">&lt;<span class="hljs-name">strong</span>&gt;</span>Bulma框架<span class="hljs-tag">&lt;/<span class="hljs-name">strong</span>&gt;</span>(Flexbox based)，能够轻松布局并可定制化<span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">ul</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Always Popover"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Duis mollis, est non commodo luctus"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Always Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Always Popover"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Duis mollis, est non commodo luctus"</span> <span class="hljs-attr">:disabled</span>=<span class="hljs-string">"true"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-warning"</span>&gt;</span>Disabled Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"No title! Duis mollis, est non commodo luctus"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>No title!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;popover title=\&quot;Width Popover\&quot; :always=\&quot;false\&quot; :width=\&quot;400\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Width Popover!&lt;/button&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;h4&gt;全面、灵活且强大的ui组件&lt;/h4&gt;\n    &lt;ul&gt;\n      &lt;li&gt;样式基于&lt;strong&gt;Bulma框架&lt;/strong&gt;(Flexbox based)，能够轻松布局并可定制化&lt;/li&gt;\n    &lt;/ul&gt;\n  &lt;/div&gt;\n&lt;/popover&gt;\n\n&lt;popover title=\&quot;free content\&quot; :width=\&quot;500\&quot;&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Free content!&lt;/button&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;img class=\&quot;image\&quot; src=\&quot;https://pek3a.qingstor.com/warehouse1/20161205045719651.jpg\&quot; style=\&quot;float: left;margin-bottom: 8px\&quot; width=\&quot;260\&quot;&gt;\n    &lt;p&gt;这里是亚得里亚海，海龙卷自远处黑暗的云层间从天而降，你来掌镜摄影师Ivan Stulić在克罗地亚一个小岛上拍下了这张照片。\n      “眼前的海龙卷距离左边的船只大概只有50-100米的距离，所幸人员和船只都没事。”他这样说道。&lt;/p&gt;\n  &lt;/div&gt;\n&lt;/popover&gt;\n\n&lt;popover title=\&quot;Always Popover\&quot; content=\&quot;Duis mollis, est non commodo luctus\&quot; trigger=\&quot;hover\&quot;&gt;\n  &lt;button class=\&quot;button is-info\&quot;&gt;Trigger Popover!&lt;/button&gt;\n&lt;/popover&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><popover title="Width Popover" :always="false" :width="400">
  <button class="button is-primary">Width Popover!</button>
  <div slot="content">
    <h4>全面、灵活且强大的ui组件</h4>
    <ul>
      <li>样式基于<strong>Bulma框架</strong>(Flexbox based)，能够轻松布局并可定制化</li>
    </ul>
  </div>
</popover>

<popover title="free content" :width="500">
  <button class="button is-primary">Free content!</button>
  <div slot="content">
    <img class="image" src="https://pek3a.qingstor.com/warehouse1/20161205045719651.jpg" style="float: left;margin-bottom: 8px" width="260">
    <p>这里是亚得里亚海，海龙卷自远处黑暗的云层间从天而降，你来掌镜摄影师Ivan Stulić在克罗地亚一个小岛上拍下了这张照片。
      “眼前的海龙卷距离左边的船只大概只有50-100米的距离，所幸人员和船只都没事。”他这样说道。</p>
  </div>
</popover>

<popover title="Always Popover" content="Duis mollis, est non commodo luctus" trigger="hover">
  <button class="button is-info">Trigger Popover!</button>
</popover>

</div>
                    <div slot="description"><h4 id="width-and-content"><a class="header-anchor" href="#width-and-content" aria-hidden="true">¶</a> Width and Content</h4>
<ul>
<li>set width by <code>width</code></li>
<li><code>slot=&quot;content&quot;</code> to set the content of the popover</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Width Popover"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:width</span>=<span class="hljs-string">"400"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Width Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>全面、灵活且强大的ui组件<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">ul</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span>样式基于<span class="hljs-tag">&lt;<span class="hljs-name">strong</span>&gt;</span>Bulma框架<span class="hljs-tag">&lt;/<span class="hljs-name">strong</span>&gt;</span>(Flexbox based)，能够轻松布局并可定制化<span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">ul</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"free content"</span> <span class="hljs-attr">:width</span>=<span class="hljs-string">"500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Free content!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">img</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"image"</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://pek3a.qingstor.com/warehouse1/20161205045719651.jpg"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"float: left;margin-bottom: 8px"</span> <span class="hljs-attr">width</span>=<span class="hljs-string">"260"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>这里是亚得里亚海，海龙卷自远处黑暗的云层间从天而降，你来掌镜摄影师Ivan Stulić在克罗地亚一个小岛上拍下了这张照片。
      “眼前的海龙卷距离左边的船只大概只有50-100米的距离，所幸人员和船只都没事。”他这样说道。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Always Popover"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Duis mollis, est non commodo luctus"</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"hover"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>Trigger Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Width and Content
  * set width by `width`
  * `slot="content"` to set the content of the popover
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Width Popover"</span> <span class="hljs-attr">:always</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:width</span>=<span class="hljs-string">"400"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Width Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>全面、灵活且强大的ui组件<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">ul</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span>样式基于<span class="hljs-tag">&lt;<span class="hljs-name">strong</span>&gt;</span>Bulma框架<span class="hljs-tag">&lt;/<span class="hljs-name">strong</span>&gt;</span>(Flexbox based)，能够轻松布局并可定制化<span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">ul</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"free content"</span> <span class="hljs-attr">:width</span>=<span class="hljs-string">"500"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Free content!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">img</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"image"</span> <span class="hljs-attr">src</span>=<span class="hljs-string">"https://pek3a.qingstor.com/warehouse1/20161205045719651.jpg"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"float: left;margin-bottom: 8px"</span> <span class="hljs-attr">width</span>=<span class="hljs-string">"260"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>这里是亚得里亚海，海龙卷自远处黑暗的云层间从天而降，你来掌镜摄影师Ivan Stulić在克罗地亚一个小岛上拍下了这张照片。
      “眼前的海龙卷距离左边的船只大概只有50-100米的距离，所幸人员和船只都没事。”他这样说道。<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Always Popover"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Duis mollis, est non commodo luctus"</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"hover"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-info"</span>&gt;</span>Trigger Popover!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;tooltip-placement\&quot;&gt;\n  &lt;div style=\&quot;margin-left: 60px\&quot;&gt;\n    &lt;popover title=\&quot;topLeft\&quot; content=\&quot;popover topLeft popover topLeft!\&quot; placement=\&quot;topLeft\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;topLeft&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover title=\&quot;top\&quot; content=\&quot;popover top!\&quot; placement=\&quot;top\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;top&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover title=\&quot;topRight\&quot; content=\&quot;popover topRight! popover topRight!\&quot; placement=\&quot;topRight\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;topRight&lt;/button&gt;\n    &lt;/popover&gt;\n  &lt;/div&gt;\n\n  &lt;div style=\&quot;width: 60px; float: left\&quot;&gt;\n    &lt;popover title=\&quot;leftTop\&quot; content=\&quot;popover leftTop!\&quot; placement=\&quot;leftTop\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;leftTop&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover title=\&quot;left\&quot; content=\&quot;popover left!\&quot; placement=\&quot;left\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;left&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover title=\&quot;leftBottom\&quot; content=\&quot;popover leftBottom!\&quot; placement=\&quot;leftBottom\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;leftBottom&lt;/button&gt;\n    &lt;/popover&gt;\n  &lt;/div&gt;\n\n  &lt;div style=\&quot;width: 60px; margin-left: 360px\&quot;&gt;\n    &lt;popover title=\&quot;rightTop\&quot; content=\&quot;Basic rightTop!\&quot; placement=\&quot;rightTop\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;rightTop&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover title=\&quot;right\&quot; content=\&quot;popover right!\&quot; placement=\&quot;right\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;right&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover title=\&quot;rightBottom\&quot; content=\&quot;popover rightBottom!\&quot; placement=\&quot;rightBottom\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;rightBottom&lt;/button&gt;\n    &lt;/popover&gt;\n  &lt;/div&gt;\n\n  &lt;div style=\&quot;margin-left: 60px; clear: both\&quot;&gt;\n    &lt;popover content=\&quot;popover bottomLeft! Basic bottomLeft!\&quot; placement=\&quot;bottomLeft\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;bottomLeft&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover content=\&quot;popover bottom!\&quot; placement=\&quot;bottom\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;bottom&lt;/button&gt;\n    &lt;/popover&gt;\n\n    &lt;popover content=\&quot;popover bottomRight! popover bottomRight!\&quot; placement=\&quot;bottomRight\&quot;&gt;\n      &lt;button class=\&quot;button\&quot;&gt;bottomRight&lt;/button&gt;\n    &lt;/popover&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="tooltip-placement">
  <div style="margin-left: 60px">
    <popover title="topLeft" content="popover topLeft popover topLeft!" placement="topLeft">
      <button class="button">topLeft</button>
    </popover>

    <popover title="top" content="popover top!" placement="top">
      <button class="button">top</button>
    </popover>

    <popover title="topRight" content="popover topRight! popover topRight!" placement="topRight">
      <button class="button">topRight</button>
    </popover>
  </div>

  <div style="width: 60px; float: left">
    <popover title="leftTop" content="popover leftTop!" placement="leftTop">
      <button class="button">leftTop</button>
    </popover>

    <popover title="left" content="popover left!" placement="left">
      <button class="button">left</button>
    </popover>

    <popover title="leftBottom" content="popover leftBottom!" placement="leftBottom">
      <button class="button">leftBottom</button>
    </popover>
  </div>

  <div style="width: 60px; margin-left: 360px">
    <popover title="rightTop" content="Basic rightTop!" placement="rightTop">
      <button class="button">rightTop</button>
    </popover>

    <popover title="right" content="popover right!" placement="right">
      <button class="button">right</button>
    </popover>

    <popover title="rightBottom" content="popover rightBottom!" placement="rightBottom">
      <button class="button">rightBottom</button>
    </popover>
  </div>

  <div style="margin-left: 60px; clear: both">
    <popover content="popover bottomLeft! Basic bottomLeft!" placement="bottomLeft">
      <button class="button">bottomLeft</button>
    </popover>

    <popover content="popover bottom!" placement="bottom">
      <button class="button">bottom</button>
    </popover>

    <popover content="popover bottomRight! popover bottomRight!" placement="bottomRight">
      <button class="button">bottomRight</button>
    </popover>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="placement"><a class="header-anchor" href="#placement" aria-hidden="true">¶</a> Placement</h4>
<ul>
<li>There are 12 placement options available.</li>
<li>Popover can be adapted to the viewport</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"tooltip-placement"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"topLeft"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover topLeft popover topLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"top"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover top!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"top"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"topRight"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover topRight! popover topRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; float: left"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"leftTop"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover leftTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"left"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover left!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>left<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"leftBottom"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover leftBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; margin-left: 360px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"rightTop"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Basic rightTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"right"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover right!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>right<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"rightBottom"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover rightBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px; clear: both"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover bottomLeft! Basic bottomLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover bottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover bottomRight! popover bottomRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Placement
  * There are 12 placement options available.
  * Popover can be adapted to the viewport
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"tooltip-placement"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"topLeft"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover topLeft popover topLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"top"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover top!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"top"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>top<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"topRight"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover topRight! popover topRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"topRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>topRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; float: left"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"leftTop"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover leftTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"left"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover left!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>left<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"leftBottom"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover leftBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"leftBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>leftBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 60px; margin-left: 360px"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"rightTop"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"Basic rightTop!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightTop"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightTop<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"right"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover right!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>right<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"rightBottom"</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover rightBottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"rightBottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>rightBottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>

  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-left: 60px; clear: both"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover bottomLeft! Basic bottomLeft!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomLeft"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover bottom!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottom"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>

    <span class="hljs-tag">&lt;<span class="hljs-name">popover</span> <span class="hljs-attr">content</span>=<span class="hljs-string">"popover bottomRight! popover bottomRight!"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"bottomRight"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>bottomRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">popover</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
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
<td>trigger</td>
<td>triggering mode: can be hover, focus, or click.</td>
<td>String</td>
<td>hover</td>
</tr>
<tr>
<td>title</td>
<td>title of the Popover</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>content</td>
<td>content of the Popover,can be set by <code>slot</code>，such as <code>&lt;div slot=&quot;content&quot;&gt;...&lt;/div&gt;</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>width</td>
<td>width of the Popover</td>
<td>Number</td>
<td>-</td>
</tr>
<tr>
<td>placement</td>
<td>to set the position, which can be one of：<code>top</code> <code>left</code> <code>right</code> <code>bottom</code> <code>topLeft</code> <code>topRight</code> <code>leftTop</code> <code>leftBottom</code> <code>bottomLeft</code> <code>rightTop</code> <code>rightBottom</code></td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>always</td>
<td>Whether the popover is always open</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>disabled</td>
<td>Disable the popover</td>
<td>Boolean</td>
<td>false</td>
</tr>
</tbody>
</table>
</section></template>

