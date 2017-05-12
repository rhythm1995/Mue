<template><section><h2 id="dropdown"><a class="header-anchor" href="#dropdown" aria-hidden="true">¶</a> Dropdown</h2>
<p>A dropdown list.</p>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;dropdown&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Basic Dropdown!&lt;/button&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;menus&gt;\n      &lt;menu-item icon=\&quot;user\&quot; to=\&quot;/components/menu/submenu2\&quot;&gt;Members&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;ticket\&quot;&gt;Tickets&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;lock\&quot;&gt;Settings&lt;/menu-item&gt;\n      &lt;div class=\&quot;divider\&quot;&gt;&lt;/div&gt;\n      &lt;menu-item icon&gt;Sign out&lt;/menu-item&gt;\n    &lt;/menus&gt;\n  &lt;/div&gt;\n&lt;/dropdown&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><dropdown>
  <button class="button is-primary">Basic Dropdown!</button>
  <div slot="content">
    <menus>
      <menu-item icon="user" to="/components/menu/submenu2">Members</menu-item>
      <menu-item icon="ticket">Tickets</menu-item>
      <menu-item icon="lock">Settings</menu-item>
      <div class="divider"></div>
      <menu-item icon="">Sign out</menu-item>
    </menus>
  </div>
</dropdown>
</div>
                    <div slot="description"><h4 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h4>
<ul>
<li>The dropdown component is used with the menu component,put the dropdown list in <code>slot='content'</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Basic Dropdown!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu2"</span>&gt;</span>Members<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>Tickets<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>Settings<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>Sign out<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Examples
  * The dropdown component is used with the menu component,put the dropdown list in `slot='content'`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Basic Dropdown!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu2"</span>&gt;</span>Members<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>Tickets<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>Settings<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>Sign out<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;dropdown&gt;\n  &lt;a class=\&quot;button is-primary\&quot;&gt;\n    &lt;span&gt;Dropdown Menu&lt;/span&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;\n      &lt;i class=\&quot;fa fa-angle-down\&quot;&gt;&lt;/i&gt;\n    &lt;/span&gt;\n  &lt;/a&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;menus&gt;\n      &lt;menu-item&gt;Members&lt;/menu-item&gt;\n      &lt;menu-item&gt;Tickets&lt;/menu-item&gt;\n      &lt;menu-item&gt;Articles&lt;/menu-item&gt;\n      &lt;menu-item&gt;\n        &lt;span&gt;Settings&lt;/span&gt;\n        &lt;menus slot=\&quot;sub\&quot; type=\&quot;float\&quot;&gt;\n          &lt;menu-item icon=\&quot;home\&quot;&gt;Main Nav&lt;/menu-item&gt;\n          &lt;menu-item icon=\&quot;home\&quot;&gt;Sub Nav&lt;/menu-item&gt;\n        &lt;/menus&gt;\n      &lt;/menu-item&gt;\n    &lt;/menus&gt;\n  &lt;/div&gt;\n&lt;/dropdown&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><dropdown>
  <a class="button is-primary">
    <span>Dropdown Menu</span>
    <span class="icon is-small">
      <i class="fa fa-angle-down"></i>
    </span>
  </a>
  <div slot="content">
    <menus>
      <menu-item>Members</menu-item>
      <menu-item>Tickets</menu-item>
      <menu-item>Articles</menu-item>
      <menu-item>
        <span>Settings</span>
        <menus slot="sub" type="float">
          <menu-item icon="home">Main Nav</menu-item>
          <menu-item icon="home">Sub Nav</menu-item>
        </menus>
      </menu-item>
    </menus>
  </div>
</dropdown>
</div>
                    <div slot="description"><h4 id="multilevel"><a class="header-anchor" href="#multilevel" aria-hidden="true">¶</a> Multilevel</h4>
<ul>
<li>The menu has multiple levels.</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Dropdown Menu<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>Members<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>Tickets<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>Articles<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Settings<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"float"</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Main Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Sub Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Multilevel
  * The menu has multiple levels.
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Dropdown Menu<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>Members<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>Tickets<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>Articles<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Settings<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"float"</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Main Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Sub Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;dropdown trigger=\&quot;hover\&quot;&gt;\n  &lt;a class=\&quot;button is-white\&quot;&gt;\n    &lt;span&gt;Dropdown Menu&lt;/span&gt;\n      &lt;span class=\&quot;icon is-small\&quot;&gt;\n      &lt;i class=\&quot;fa fa-angle-down\&quot;&gt;&lt;/i&gt;\n    &lt;/span&gt;\n  &lt;/a&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;menus&gt;\n      &lt;menu-item icon=\&quot;user\&quot;&gt;Members&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;ticket\&quot;&gt;Tickets&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;lock\&quot;&gt;Settings&lt;/menu-item&gt;\n      &lt;div class=\&quot;divider\&quot;&gt;&lt;/div&gt;\n      &lt;menu-item icon&gt;Sign out&lt;/menu-item&gt;\n    &lt;/menus&gt;\n  &lt;/div&gt;\n&lt;/dropdown&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><dropdown trigger="hover">
  <a class="button is-white">
    <span>Dropdown Menu</span>
      <span class="icon is-small">
      <i class="fa fa-angle-down"></i>
    </span>
  </a>
  <div slot="content">
    <menus>
      <menu-item icon="user">Members</menu-item>
      <menu-item icon="ticket">Tickets</menu-item>
      <menu-item icon="lock">Settings</menu-item>
      <div class="divider"></div>
      <menu-item icon="">Sign out</menu-item>
    </menus>
  </div>
</dropdown>
</div>
                    <div slot="description"><h4 id="trigger-mode"><a class="header-anchor" href="#trigger-mode" aria-hidden="true">¶</a> Trigger Mode</h4>
<ul>
<li>Sets Trigger Mode by <code>trigger</code></li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"hover"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-white"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Dropdown Menu<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span>&gt;</span>Members<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>Tickets<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>Settings<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>Sign out<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Trigger Mode
  * Sets Trigger Mode by `trigger`
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"hover"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-white"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Dropdown Menu<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span>&gt;</span>Members<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>Tickets<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>Settings<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>Sign out<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
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
<td>trigger mode,accepted <code>click</code> <code>hover</code></td>
<td>String</td>
<td><code>click</code></td>
</tr>
</tbody>
</table>
</section></template>

