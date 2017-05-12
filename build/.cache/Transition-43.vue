<template><section><h2 id="transition"><a class="header-anchor" href="#transition" aria-hidden="true">¶</a> Transition</h2>
<p>Base on Animate.css,Blu provides a variety of transition effects when items are inserted, updated, or removed from the DOM</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;fade\&quot;&gt;fade&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;fadeRight\&quot;&gt;fadeRight&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;fadeLeft\&quot;&gt;fadeLeft&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;fadeLeftBig\&quot;&gt;fadeLeftBig&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;fadeUpBig\&quot;&gt;fadeUpBig&lt;/button&gt;\n\n&lt;br&gt;&lt;br&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;rotate\&quot;&gt;rotate&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;rotateDownLeft\&quot;&gt;rotateDownLeft&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;rotateDownRight\&quot;&gt;rotateDownRight&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;rotateUpLeft\&quot;&gt;rotateUpLeft&lt;/button&gt;\n\n&lt;br&gt;&lt;br&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;bounce\&quot;&gt;bounce&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;bounceDown\&quot;&gt;bounceDown&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;bounceLeft\&quot;&gt;bounceLeft&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;bounceRight\&quot;&gt;bounceRight&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;bounceUp\&quot;&gt;bounceUp&lt;/button&gt;\n\n&lt;br&gt;&lt;br&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;slideDown\&quot;&gt;slideDown&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;slideLeft\&quot;&gt;slideLeft&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;slideRight\&quot;&gt;slideRight&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;slideUp\&quot;&gt;slideUp&lt;/button&gt;\n\n&lt;br&gt;&lt;br&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;zoom\&quot;&gt;zoom&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;zoomDown\&quot;&gt;zoomDown&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;zoomLeft\&quot;&gt;zoomLeft&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;zoomRight\&quot;&gt;zoomRight&lt;/button&gt;\n&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;zoomUp\&quot;&gt;zoomUp&lt;/button&gt;\n\n\n\n&quot;,&quot;script&quot;:&quot;\n  export default {\n    methods: {\n      fadeNotify() {\n        this.$notify.open({content: 'fade', transition: 'fade'});\n      },\n      fadeRight() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'fadeRight',\n          content: 'fadeRight...'\n        });\n      },\n      fadeLeft() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'fadeLeft',\n          content: 'fadeLeft...'\n        });\n      },\n      fadeLeftBig() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'fadeLeftBig',\n          content: 'fadeLeftBig...'\n        });\n      },\n      fadeUpBig() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'fadeUpBig',\n          content: 'fadeUpBig...'\n        });\n      },\n      fade() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'fade',\n          content: 'fade...'\n        });\n      },\n\n      rotate() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'rotate',\n          content: 'rotate...'\n        });\n      },\n      rotateDownLeft() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'rotateDownLeft',\n          content: 'rotateDownLeft...'\n        });\n      },\n      rotateDownRight() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'rotateDownRight',\n          content: 'rotateDownRight...'\n        });\n      },\n      rotateUpLeft() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'rotateUpLeft',\n          content: 'rotateUpLeft...'\n        });\n      },\n\n      bounce() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'bounce',\n          content: 'bounce...'\n        });\n      },\n      bounceDown() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'bounceDown',\n          content: 'bounceDown...'\n        });\n      },\n      bounceLeft() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'bounceLeft',\n          content: 'bounceLeft...'\n        });\n      },\n      bounceRight() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'bounceRight',\n          content: 'bounceRight...'\n        });\n      },\n      bounceUp() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'bounceUp',\n          content: 'bounceUp...'\n        });\n      },\n\n      slideDown() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'slideDown',\n          content: 'slideDown...'\n        });\n      },\n      slideLeft() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'slideLeft',\n          content: 'slideLeft...'\n        });\n      },\n      slideRight() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'slideRight',\n          content: 'slideRight...'\n        });\n      },\n      slideUp() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'slideUp',\n          content: 'slideUp...'\n        });\n      },\n\n      zoom() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'zoom',\n          content: 'zoom...'\n        });\n      },\n      zoomDown() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'zoomDown',\n          content: 'zoomDown...'\n        });\n      },\n      zoomLeft() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'zoomLeft',\n          content: 'zoomLeft...'\n        });\n      },\n      zoomRight() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'zoomRight',\n          content: 'zoomRight...'\n        });\n      },\n      zoomUp() {\n        this.$modal.open({\n          autoClose: 3,\n          transition: 'zoomUp',\n          content: 'zoomUp...'\n        });\n      },\n\n\n    },\n  };\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><button class="button is-primary" @click="fade">fade</button>
<button class="button is-primary" @click="fadeRight">fadeRight</button>
<button class="button is-primary" @click="fadeLeft">fadeLeft</button>
<button class="button is-primary" @click="fadeLeftBig">fadeLeftBig</button>
<button class="button is-primary" @click="fadeUpBig">fadeUpBig</button>

<br><br>
<button class="button is-primary" @click="rotate">rotate</button>
<button class="button is-primary" @click="rotateDownLeft">rotateDownLeft</button>
<button class="button is-primary" @click="rotateDownRight">rotateDownRight</button>
<button class="button is-primary" @click="rotateUpLeft">rotateUpLeft</button>

<br><br>
<button class="button is-primary" @click="bounce">bounce</button>
<button class="button is-primary" @click="bounceDown">bounceDown</button>
<button class="button is-primary" @click="bounceLeft">bounceLeft</button>
<button class="button is-primary" @click="bounceRight">bounceRight</button>
<button class="button is-primary" @click="bounceUp">bounceUp</button>

<br><br>
<button class="button is-primary" @click="slideDown">slideDown</button>
<button class="button is-primary" @click="slideLeft">slideLeft</button>
<button class="button is-primary" @click="slideRight">slideRight</button>
<button class="button is-primary" @click="slideUp">slideUp</button>

<br><br>
<button class="button is-primary" @click="zoom">zoom</button>
<button class="button is-primary" @click="zoomDown">zoomDown</button>
<button class="button is-primary" @click="zoomLeft">zoomLeft</button>
<button class="button is-primary" @click="zoomRight">zoomRight</button>
<button class="button is-primary" @click="zoomUp">zoomUp</button>



</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>Sets it by <code>transition</code> component of Vue. such as <code>&lt;transition name=&quot;fade&quot;&gt;...&lt;/transition&gt;</code></li>
<li>Modify the <code>animation-duration</code> of transition by overriding <code>$transition-speed</code>(sass variable)</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fade"</span>&gt;</span>fade<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeRight"</span>&gt;</span>fadeRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeLeft"</span>&gt;</span>fadeLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeLeftBig"</span>&gt;</span>fadeLeftBig<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeUpBig"</span>&gt;</span>fadeUpBig<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotate"</span>&gt;</span>rotate<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotateDownLeft"</span>&gt;</span>rotateDownLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotateDownRight"</span>&gt;</span>rotateDownRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotateUpLeft"</span>&gt;</span>rotateUpLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounce"</span>&gt;</span>bounce<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceDown"</span>&gt;</span>bounceDown<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceLeft"</span>&gt;</span>bounceLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceRight"</span>&gt;</span>bounceRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceUp"</span>&gt;</span>bounceUp<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideDown"</span>&gt;</span>slideDown<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideLeft"</span>&gt;</span>slideLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideRight"</span>&gt;</span>slideRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideUp"</span>&gt;</span>slideUp<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoom"</span>&gt;</span>zoom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomDown"</span>&gt;</span>zoomDown<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomLeft"</span>&gt;</span>zoomLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomRight"</span>&gt;</span>zoomRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomUp"</span>&gt;</span>zoomUp<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      fadeNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'fade'</span>, <span class="hljs-attr">transition</span>: <span class="hljs-string">'fade'</span>});
      },
      fadeRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeRight...'</span>
        });
      },
      fadeLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeLeft...'</span>
        });
      },
      fadeLeftBig() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeLeftBig'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeLeftBig...'</span>
        });
      },
      fadeUpBig() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeUpBig'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeUpBig...'</span>
        });
      },
      fade() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fade'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fade...'</span>
        });
      },

      rotate() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotate'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotate...'</span>
        });
      },
      rotateDownLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotateDownLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotateDownLeft...'</span>
        });
      },
      rotateDownRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotateDownRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotateDownRight...'</span>
        });
      },
      rotateUpLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotateUpLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotateUpLeft...'</span>
        });
      },

      bounce() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounce'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounce...'</span>
        });
      },
      bounceDown() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceDown'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceDown...'</span>
        });
      },
      bounceLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceLeft...'</span>
        });
      },
      bounceRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceRight...'</span>
        });
      },
      bounceUp() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceUp'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceUp...'</span>
        });
      },

      slideDown() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideDown'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideDown...'</span>
        });
      },
      slideLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideLeft...'</span>
        });
      },
      slideRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideRight...'</span>
        });
      },
      slideUp() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideUp'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideUp...'</span>
        });
      },

      zoom() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoom'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoom...'</span>
        });
      },
      zoomDown() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomDown'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomDown...'</span>
        });
      },
      zoomLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomLeft...'</span>
        });
      },
      zoomRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomRight...'</span>
        });
      },
      zoomUp() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomUp'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomUp...'</span>
        });
      },


    },
  };
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Basic
  * Sets it by `transition` component of Vue. such as `<transition name="fade">...</transition>`
  * Modify the `animation-duration` of transition by overriding `$transition-speed`(sass variable)
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fade"</span>&gt;</span>fade<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeRight"</span>&gt;</span>fadeRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeLeft"</span>&gt;</span>fadeLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeLeftBig"</span>&gt;</span>fadeLeftBig<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"fadeUpBig"</span>&gt;</span>fadeUpBig<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotate"</span>&gt;</span>rotate<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotateDownLeft"</span>&gt;</span>rotateDownLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotateDownRight"</span>&gt;</span>rotateDownRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"rotateUpLeft"</span>&gt;</span>rotateUpLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounce"</span>&gt;</span>bounce<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceDown"</span>&gt;</span>bounceDown<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceLeft"</span>&gt;</span>bounceLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceRight"</span>&gt;</span>bounceRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"bounceUp"</span>&gt;</span>bounceUp<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideDown"</span>&gt;</span>slideDown<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideLeft"</span>&gt;</span>slideLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideRight"</span>&gt;</span>slideRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"slideUp"</span>&gt;</span>slideUp<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">br</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoom"</span>&gt;</span>zoom<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomDown"</span>&gt;</span>zoomDown<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomLeft"</span>&gt;</span>zoomLeft<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomRight"</span>&gt;</span>zoomRight<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"zoomUp"</span>&gt;</span>zoomUp<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
  <span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
    <span class="hljs-attr">methods</span>: {
      fadeNotify() {
        <span class="hljs-keyword">this</span>.$notify.open({<span class="hljs-attr">content</span>: <span class="hljs-string">'fade'</span>, <span class="hljs-attr">transition</span>: <span class="hljs-string">'fade'</span>});
      },
      fadeRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeRight...'</span>
        });
      },
      fadeLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeLeft...'</span>
        });
      },
      fadeLeftBig() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeLeftBig'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeLeftBig...'</span>
        });
      },
      fadeUpBig() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fadeUpBig'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fadeUpBig...'</span>
        });
      },
      fade() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'fade'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'fade...'</span>
        });
      },

      rotate() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotate'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotate...'</span>
        });
      },
      rotateDownLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotateDownLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotateDownLeft...'</span>
        });
      },
      rotateDownRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotateDownRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotateDownRight...'</span>
        });
      },
      rotateUpLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'rotateUpLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'rotateUpLeft...'</span>
        });
      },

      bounce() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounce'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounce...'</span>
        });
      },
      bounceDown() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceDown'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceDown...'</span>
        });
      },
      bounceLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceLeft...'</span>
        });
      },
      bounceRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceRight...'</span>
        });
      },
      bounceUp() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'bounceUp'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'bounceUp...'</span>
        });
      },

      slideDown() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideDown'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideDown...'</span>
        });
      },
      slideLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideLeft...'</span>
        });
      },
      slideRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideRight...'</span>
        });
      },
      slideUp() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'slideUp'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'slideUp...'</span>
        });
      },

      zoom() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoom'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoom...'</span>
        });
      },
      zoomDown() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomDown'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomDown...'</span>
        });
      },
      zoomLeft() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomLeft'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomLeft...'</span>
        });
      },
      zoomRight() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomRight'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomRight...'</span>
        });
      },
      zoomUp() {
        <span class="hljs-keyword">this</span>.$modal.open({
          <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
          <span class="hljs-attr">transition</span>: <span class="hljs-string">'zoomUp'</span>,
          <span class="hljs-attr">content</span>: <span class="hljs-string">'zoomUp...'</span>
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
<th>Properties</th>
<th>Description</th>
<th>Type</th>
<th>Default</th>
</tr>
</thead>
<tbody>
<tr>
<td>transition</td>
<td>Accepted Values: <code>bounce</code> <code>bounceDown</code> <code>bounceLeft</code> <code>bounceRight</code> <code>bounceUp</code> <code>fade</code> <code>fadeDown</code> <code>fadeDownBig</code> <code>fadeLeft</code> <code>fadeLeftBig</code> <code>fadeRight</code> <code>fadeRightBig</code> <code>fadeUp</code> <code>fadeUpBig</code> <code>rotate</code> <code>rotateDownLeft</code> <code>rotateDownRight</code> <code>rotateUpLeft</code> <code>rotateUpRight</code> <code>slideDown</code> <code>slideLeft</code> <code>slideRight</code> <code>slideUp</code> <code>zoom</code> <code>zoomDown</code> <code>zoomLeft</code> <code>zoomRight</code> <code>zoomUp</code></td>
<td>String</td>
<td>-</td>
</tr>
</tbody>
</table>
<p>Thanks to <a href="https://github.com/asika32764/vue2-animate">vue2-animate</a></p>

</section></template>

<script>
export default {
  methods: {
    fadeNotify() {
      this.$notify.open({content: 'fade', transition: 'fade'});
    },
    fadeRight() {
      this.$modal.open({
        autoClose: 3,
        transition: 'fadeRight',
        content: 'fadeRight...'
      });
    },
    fadeLeft() {
      this.$modal.open({
        autoClose: 3,
        transition: 'fadeLeft',
        content: 'fadeLeft...'
      });
    },
    fadeLeftBig() {
      this.$modal.open({
        autoClose: 3,
        transition: 'fadeLeftBig',
        content: 'fadeLeftBig...'
      });
    },
    fadeUpBig() {
      this.$modal.open({
        autoClose: 3,
        transition: 'fadeUpBig',
        content: 'fadeUpBig...'
      });
    },
    fade() {
      this.$modal.open({
        autoClose: 3,
        transition: 'fade',
        content: 'fade...'
      });
    },

    rotate() {
      this.$modal.open({
        autoClose: 3,
        transition: 'rotate',
        content: 'rotate...'
      });
    },
    rotateDownLeft() {
      this.$modal.open({
        autoClose: 3,
        transition: 'rotateDownLeft',
        content: 'rotateDownLeft...'
      });
    },
    rotateDownRight() {
      this.$modal.open({
        autoClose: 3,
        transition: 'rotateDownRight',
        content: 'rotateDownRight...'
      });
    },
    rotateUpLeft() {
      this.$modal.open({
        autoClose: 3,
        transition: 'rotateUpLeft',
        content: 'rotateUpLeft...'
      });
    },

    bounce() {
      this.$modal.open({
        autoClose: 3,
        transition: 'bounce',
        content: 'bounce...'
      });
    },
    bounceDown() {
      this.$modal.open({
        autoClose: 3,
        transition: 'bounceDown',
        content: 'bounceDown...'
      });
    },
    bounceLeft() {
      this.$modal.open({
        autoClose: 3,
        transition: 'bounceLeft',
        content: 'bounceLeft...'
      });
    },
    bounceRight() {
      this.$modal.open({
        autoClose: 3,
        transition: 'bounceRight',
        content: 'bounceRight...'
      });
    },
    bounceUp() {
      this.$modal.open({
        autoClose: 3,
        transition: 'bounceUp',
        content: 'bounceUp...'
      });
    },

    slideDown() {
      this.$modal.open({
        autoClose: 3,
        transition: 'slideDown',
        content: 'slideDown...'
      });
    },
    slideLeft() {
      this.$modal.open({
        autoClose: 3,
        transition: 'slideLeft',
        content: 'slideLeft...'
      });
    },
    slideRight() {
      this.$modal.open({
        autoClose: 3,
        transition: 'slideRight',
        content: 'slideRight...'
      });
    },
    slideUp() {
      this.$modal.open({
        autoClose: 3,
        transition: 'slideUp',
        content: 'slideUp...'
      });
    },

    zoom() {
      this.$modal.open({
        autoClose: 3,
        transition: 'zoom',
        content: 'zoom...'
      });
    },
    zoomDown() {
      this.$modal.open({
        autoClose: 3,
        transition: 'zoomDown',
        content: 'zoomDown...'
      });
    },
    zoomLeft() {
      this.$modal.open({
        autoClose: 3,
        transition: 'zoomLeft',
        content: 'zoomLeft...'
      });
    },
    zoomRight() {
      this.$modal.open({
        autoClose: 3,
        transition: 'zoomRight',
        content: 'zoomRight...'
      });
    },
    zoomUp() {
      this.$modal.open({
        autoClose: 3,
        transition: 'zoomUp',
        content: 'zoomUp...'
      });
    },


  },
};
</script>