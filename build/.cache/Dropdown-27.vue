<template><section><h2 id="dropdown-xia-la-cai-dan"><a class="header-anchor" href="#dropdown-xia-la-cai-dan" aria-hidden="true">¶</a> Dropdown 下拉菜单</h2>
<p>下拉菜单</p>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;dropdown&gt;\n  &lt;button class=\&quot;button is-primary\&quot;&gt;Basic Dropdown!&lt;/button&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;menus&gt;\n      &lt;menu-item icon=\&quot;user\&quot;&gt;会员管理&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;ticket\&quot;&gt;工单管理&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;lock\&quot;&gt;修改密码&lt;/menu-item&gt;\n      &lt;div class=\&quot;divider\&quot;&gt;&lt;/div&gt;\n      &lt;menu-item icon&gt;退出&lt;/menu-item&gt;\n    &lt;/menus&gt;\n  &lt;/div&gt;\n&lt;/dropdown&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><dropdown>
  <button class="button is-primary">Basic Dropdown!</button>
  <div slot="content">
    <menus>
      <menu-item icon="user">会员管理</menu-item>
      <menu-item icon="ticket">工单管理</menu-item>
      <menu-item icon="lock">修改密码</menu-item>
      <div class="divider"></div>
      <menu-item icon="">退出</menu-item>
    </menus>
  </div>
</dropdown>
</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>dropdown 组件是和 <code>menu</code> 组件搭配使用的</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Basic Dropdown!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>退出<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 基本
  * dropdown 组件是和 `menu` 组件搭配使用的
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Basic Dropdown!<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>退出<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;dropdown&gt;\n  &lt;a class=\&quot;button is-primary\&quot;&gt;\n    &lt;span&gt;下拉菜单&lt;/span&gt;\n    &lt;span class=\&quot;icon is-small\&quot;&gt;\n    &lt;i class=\&quot;fa fa-angle-down\&quot;&gt;&lt;/i&gt;\n  &lt;/span&gt;\n  &lt;/a&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;menus&gt;\n      &lt;menu-item&gt;会员管理&lt;/menu-item&gt;\n      &lt;menu-item&gt;工单管理&lt;/menu-item&gt;\n      &lt;menu-item&gt;修改密码&lt;/menu-item&gt;\n      &lt;menu-item&gt;\n        &lt;span&gt;用户中心&lt;/span&gt;\n        &lt;menus slot=\&quot;sub\&quot; type=\&quot;float\&quot;&gt;\n          &lt;menu-item icon=\&quot;home\&quot;&gt;Main Nav&lt;/menu-item&gt;\n          &lt;menu-item icon=\&quot;home\&quot;&gt;Sub Nav&lt;/menu-item&gt;\n        &lt;/menus&gt;\n      &lt;/menu-item&gt;\n    &lt;/menus&gt;\n  &lt;/div&gt;\n&lt;/dropdown&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><dropdown>
  <a class="button is-primary">
    <span>下拉菜单</span>
    <span class="icon is-small">
    <i class="fa fa-angle-down"></i>
  </span>
  </a>
  <div slot="content">
    <menus>
      <menu-item>会员管理</menu-item>
      <menu-item>工单管理</menu-item>
      <menu-item>修改密码</menu-item>
      <menu-item>
        <span>用户中心</span>
        <menus slot="sub" type="float">
          <menu-item icon="home">Main Nav</menu-item>
          <menu-item icon="home">Sub Nav</menu-item>
        </menus>
      </menu-item>
    </menus>
  </div>
</dropdown>
</div>
                    <div slot="description"><h4 id="duo-ji-cai-dan"><a class="header-anchor" href="#duo-ji-cai-dan" aria-hidden="true">¶</a> 多级菜单</h4>
<ul>
<li>通过 <code>menu</code> 组件的多级菜单来实现</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>下拉菜单<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>用户中心<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
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
  #### 多级菜单
  * 通过 `menu` 组件的多级菜单来实现
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>下拉菜单<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>用户中心<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
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
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;dropdown trigger=\&quot;hover\&quot;&gt;\n  &lt;a class=\&quot;button is-white\&quot;&gt;\n    &lt;span&gt;下拉菜单&lt;/span&gt;\n      &lt;span class=\&quot;icon is-small\&quot;&gt;\n      &lt;i class=\&quot;fa fa-angle-down\&quot;&gt;&lt;/i&gt;\n    &lt;/span&gt;\n  &lt;/a&gt;\n  &lt;div slot=\&quot;content\&quot;&gt;\n    &lt;menus&gt;\n      &lt;menu-item icon=\&quot;user\&quot;&gt;会员管理&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;ticket\&quot;&gt;工单管理&lt;/menu-item&gt;\n      &lt;menu-item icon=\&quot;lock\&quot;&gt;修改密码&lt;/menu-item&gt;\n      &lt;div class=\&quot;divider\&quot;&gt;&lt;/div&gt;\n      &lt;menu-item icon&gt;退出&lt;/menu-item&gt;\n    &lt;/menus&gt;\n  &lt;/div&gt;\n&lt;/dropdown&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><dropdown trigger="hover">
  <a class="button is-white">
    <span>下拉菜单</span>
      <span class="icon is-small">
      <i class="fa fa-angle-down"></i>
    </span>
  </a>
  <div slot="content">
    <menus>
      <menu-item icon="user">会员管理</menu-item>
      <menu-item icon="ticket">工单管理</menu-item>
      <menu-item icon="lock">修改密码</menu-item>
      <div class="divider"></div>
      <menu-item icon="">退出</menu-item>
    </menus>
  </div>
</dropdown>
</div>
                    <div slot="description"><h4 id="hong-fa-fang-shi"><a class="header-anchor" href="#hong-fa-fang-shi" aria-hidden="true">¶</a> 触发方式</h4>
<ul>
<li>通过 <code>trigger</code> 设置触发方式</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"hover"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-white"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>下拉菜单<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>退出<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 触发方式
  * 通过 `trigger` 设置触发方式
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">dropdown</span> <span class="hljs-attr">trigger</span>=<span class="hljs-string">"hover"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">a</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-white"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>下拉菜单<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">span</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"icon is-small"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">i</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"fa fa-angle-down"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">i</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"content"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"user"</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">""</span>&gt;</span>退出<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">dropdown</span>&gt;</span>
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
<td>trigger</td>
<td>默认 <code>click</code>，可选 <code>hover</code></td>
<td>String</td>
<td>无</td>
</tr>
</tbody>
</table>
</section></template>

