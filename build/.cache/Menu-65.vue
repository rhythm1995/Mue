<template><section><h2 id="menu"><a class="header-anchor" href="#menu" aria-hidden="true">¶</a> Menu</h2>
<p>Menu list of Navigation.</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot; style=\&quot;margin-top: 20px; background-color: #f0f0f0;\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;div class=\&quot;menu\&quot;&gt;\n      &lt;menus label=\&quot;Administration\&quot;&gt;\n        &lt;menu-item icon=\&quot;twitter\&quot;&gt;\n          &lt;span&gt;子目录1&lt;/span&gt;\n          &lt;menus slot=\&quot;sub\&quot;&gt;\n            &lt;menu-item :to=\&quot;{ path: '/components/menu/submenu1', query: { userId: 321 }}\&quot; icon=\&quot;qq\&quot; :is-active=\&quot;true\&quot;&gt;子子目录1&lt;/menu-item&gt;\n            &lt;menu-item icon=\&quot;google\&quot;&gt;\n              &lt;span&gt;子子目录2&lt;/span&gt;\n              &lt;menus slot=\&quot;sub\&quot;&gt;\n                &lt;menu-item icon=\&quot;home\&quot;&gt;第三级1&lt;/menu-item&gt;\n                &lt;menu-item icon=\&quot;home\&quot;&gt;第三级2&lt;/menu-item&gt;\n                &lt;menu-item icon=\&quot;home\&quot;&gt;\n                  &lt;span&gt;第三级3&lt;/span&gt;\n                  &lt;menus slot=\&quot;sub\&quot; type=\&quot;float\&quot;&gt;\n                    &lt;menu-item icon=\&quot;home\&quot;&gt;第四级1&lt;/menu-item&gt;\n                  &lt;/menus&gt;\n                &lt;/menu-item&gt;\n              &lt;/menus&gt;\n            &lt;/menu-item&gt;\n          &lt;/menus&gt;\n        &lt;/menu-item&gt;\n        &lt;menu-item icon=\&quot;wechat\&quot; to=\&quot;/components/menu/submenu2\&quot;&gt;子目录2&lt;/menu-item&gt;\n        &lt;div class=\&quot;divider\&quot;&gt;&lt;/div&gt;\n        &lt;menu-item icon=\&quot;facebook\&quot; to=\&quot;/components/menu/submenu3\&quot;&gt;&lt;span&gt;子目录3&lt;/span&gt;&lt;/menu-item&gt;\n      &lt;/menus&gt;\n    &lt;/div&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns" style="margin-top: 20px; background-color: #f0f0f0;">
  <div class="column is-3">
    <div class="menu">
      <menus label="Administration">
        <menu-item icon="twitter">
          <span>子目录1</span>
          <menus slot="sub">
            <menu-item :to="{ path: '/components/menu/submenu1', query: { userId: 321 }}" icon="qq" :is-active="true">子子目录1</menu-item>
            <menu-item icon="google">
              <span>子子目录2</span>
              <menus slot="sub">
                <menu-item icon="home">第三级1</menu-item>
                <menu-item icon="home">第三级2</menu-item>
                <menu-item icon="home">
                  <span>第三级3</span>
                  <menus slot="sub" type="float">
                    <menu-item icon="home">第四级1</menu-item>
                  </menus>
                </menu-item>
              </menus>
            </menu-item>
          </menus>
        </menu-item>
        <menu-item icon="wechat" to="/components/menu/submenu2">子目录2</menu-item>
        <div class="divider"></div>
        <menu-item icon="facebook" to="/components/menu/submenu3"><span>子目录3</span></menu-item>
      </menus>
    </div>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>通过 <code>label</code> 设置菜单组的标签</li>
<li><code>icon</code> 设置菜单项目的图标</li>
<li>设置 <code>to</code> 生成vue-router的链接</li>
<li>设置 <code>click</code> 为菜单项添加点击事件,如果设置了此项 <code>to</code> 参数失效</li>
<li><code>is-active</code> 设置菜单项是否是激活状态</li>
<li>menu 标签可嵌套</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-top: 20px; background-color: #f0f0f0;"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"menu"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Administration"</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"twitter"</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>子目录1<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">:to</span>=<span class="hljs-string">"{ path: '/components/menu/submenu1', query: { userId: 321 <span>}}</span>"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"qq"</span> <span class="hljs-attr">:is-active</span>=<span class="hljs-string">"true"</span>&gt;</span>子子目录1<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"google"</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>子子目录2<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>第三级1<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>第三级2<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>第三级3<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"float"</span>&gt;</span>
                    <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>第四级1<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                  <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
                <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
              <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
            <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
          <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
        <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"wechat"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu2"</span>&gt;</span>子目录2<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"facebook"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu3"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>子目录3<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### Basic
  * 通过 `label` 设置菜单组的标签
  * `icon` 设置菜单项目的图标
  * 设置 `to` 生成vue-router的链接
  * 设置 `click` 为菜单项添加点击事件,如果设置了此项 `to` 参数失效
  * `is-active` 设置菜单项是否是激活状态
  * menu 标签可嵌套
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-top: 20px; background-color: #f0f0f0;"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"menu"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"Administration"</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"twitter"</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>子目录1<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">:to</span>=<span class="hljs-string">"{ path: '/components/menu/submenu1', query: { userId: 321 <span>}}</span>"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"qq"</span> <span class="hljs-attr">:is-active</span>=<span class="hljs-string">"true"</span>&gt;</span>子子目录1<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"google"</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>子子目录2<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>第三级1<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>第三级2<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>第三级3<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"float"</span>&gt;</span>
                    <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>第四级1<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                  <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
                <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
              <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
            <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
          <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
        <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"wechat"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu2"</span>&gt;</span>子目录2<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"facebook"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu3"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>子目录3<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;div class=\&quot;columns\&quot; style=\&quot;margin-top: 20px; background-color: #f0f0f0;\&quot;&gt;\n  &lt;div class=\&quot;column is-3\&quot;&gt;\n    &lt;div class=\&quot;menu is-dark\&quot;&gt;\n      &lt;menus label=\&quot;内容管理\&quot;&gt;\n        &lt;menu-item icon=\&quot;image\&quot;&gt;\n          &lt;span&gt;图片&lt;/span&gt;\n          &lt;menus slot=\&quot;sub\&quot;&gt;\n            &lt;menu-item :to=\&quot;{ path: '/components/menu/submenu1', query: { userId: 321 }}\&quot; icon=\&quot;car\&quot; :is-active=\&quot;true\&quot;&gt;汽车&lt;/menu-item&gt;\n            &lt;menu-item icon=\&quot;slack\&quot;&gt;\n              &lt;span&gt;风景&lt;/span&gt;\n              &lt;menus slot=\&quot;sub\&quot;&gt;\n                &lt;menu-item icon=\&quot;home\&quot;&gt;Picture&lt;/menu-item&gt;\n                &lt;menu-item icon=\&quot;home\&quot;&gt;Content&lt;/menu-item&gt;\n                &lt;menu-item icon=\&quot;home\&quot;&gt;\n                  &lt;span&gt;Nav&lt;/span&gt;\n                  &lt;menus slot=\&quot;sub\&quot; type=\&quot;float\&quot;&gt;\n                    &lt;menu-item icon=\&quot;home\&quot;&gt;Main Nav&lt;/menu-item&gt;\n                    &lt;menu-item icon=\&quot;home\&quot;&gt;Sub Nav&lt;/menu-item&gt;\n                  &lt;/menus&gt;\n                &lt;/menu-item&gt;\n              &lt;/menus&gt;\n            &lt;/menu-item&gt;\n          &lt;/menus&gt;\n        &lt;/menu-item&gt;\n        &lt;menu-item icon=\&quot;music\&quot; to=\&quot;/components/menu/submenu2\&quot;&gt;音乐&lt;/menu-item&gt;\n        &lt;menu-item icon=\&quot;file-text-o\&quot; to=\&quot;/components/menu/submenu4\&quot;&gt;&lt;span&gt;文章&lt;/span&gt;&lt;/menu-item&gt;\n        &lt;menu-item icon=\&quot;film\&quot; to=\&quot;/components/menu/submenu3\&quot;&gt;&lt;span&gt;视频&lt;/span&gt;&lt;/menu-item&gt;\n      &lt;/menus&gt;\n      &lt;menus label=\&quot;系统设置\&quot;&gt;\n        &lt;menu-item icon=\&quot;users\&quot;&gt;会员管理&lt;/menu-item&gt;\n        &lt;menu-item icon=\&quot;ticket\&quot;&gt;工单管理&lt;/menu-item&gt;\n        &lt;menu-item icon=\&quot;lock\&quot;&gt;修改密码&lt;/menu-item&gt;\n        &lt;div class=\&quot;divider\&quot;&gt;&lt;/div&gt;\n        &lt;menu-item icon=\&quot;sign-out\&quot;&gt;退出登录&lt;/menu-item&gt;\n      &lt;/menus&gt;\n    &lt;/div&gt;\n  &lt;/div&gt;\n&lt;/div&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><div class="columns" style="margin-top: 20px; background-color: #f0f0f0;">
  <div class="column is-3">
    <div class="menu is-dark">
      <menus label="内容管理">
        <menu-item icon="image">
          <span>图片</span>
          <menus slot="sub">
            <menu-item :to="{ path: '/components/menu/submenu1', query: { userId: 321 }}" icon="car" :is-active="true">汽车</menu-item>
            <menu-item icon="slack">
              <span>风景</span>
              <menus slot="sub">
                <menu-item icon="home">Picture</menu-item>
                <menu-item icon="home">Content</menu-item>
                <menu-item icon="home">
                  <span>Nav</span>
                  <menus slot="sub" type="float">
                    <menu-item icon="home">Main Nav</menu-item>
                    <menu-item icon="home">Sub Nav</menu-item>
                  </menus>
                </menu-item>
              </menus>
            </menu-item>
          </menus>
        </menu-item>
        <menu-item icon="music" to="/components/menu/submenu2">音乐</menu-item>
        <menu-item icon="file-text-o" to="/components/menu/submenu4"><span>文章</span></menu-item>
        <menu-item icon="film" to="/components/menu/submenu3"><span>视频</span></menu-item>
      </menus>
      <menus label="系统设置">
        <menu-item icon="users">会员管理</menu-item>
        <menu-item icon="ticket">工单管理</menu-item>
        <menu-item icon="lock">修改密码</menu-item>
        <div class="divider"></div>
        <menu-item icon="sign-out">退出登录</menu-item>
      </menus>
    </div>
  </div>
</div>
</div>
                    <div slot="description"><h4 id="wan-zheng-shi-li"><a class="header-anchor" href="#wan-zheng-shi-li" aria-hidden="true">¶</a> 完整示例</h4>
<ul>
<li><code>is-dark</code> 设置黑色主题</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-top: 20px; background-color: #f0f0f0;"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"menu is-dark"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"内容管理"</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"image"</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>图片<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">:to</span>=<span class="hljs-string">"{ path: '/components/menu/submenu1', query: { userId: 321 <span>}}</span>"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"car"</span> <span class="hljs-attr">:is-active</span>=<span class="hljs-string">"true"</span>&gt;</span>汽车<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"slack"</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>风景<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Picture<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Content<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Nav<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"float"</span>&gt;</span>
                    <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Main Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                    <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Sub Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                  <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
                <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
              <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
            <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
          <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
        <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"music"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu2"</span>&gt;</span>音乐<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"file-text-o"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu4"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>文章<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"film"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu3"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>视频<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"系统设置"</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"users"</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"sign-out"</span>&gt;</span>退出登录<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 完整示例
  * `is-dark` 设置黑色主题
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"margin-top: 20px; background-color: #f0f0f0;"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"column is-3"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"menu is-dark"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"内容管理"</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"image"</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>图片<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
          <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">:to</span>=<span class="hljs-string">"{ path: '/components/menu/submenu1', query: { userId: 321 <span>}}</span>"</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"car"</span> <span class="hljs-attr">:is-active</span>=<span class="hljs-string">"true"</span>&gt;</span>汽车<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
            <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"slack"</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>风景<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
              <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Picture<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Content<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>Nav<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span>
                  <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"sub"</span> <span class="hljs-attr">type</span>=<span class="hljs-string">"float"</span>&gt;</span>
                    <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Main Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                    <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"home"</span>&gt;</span>Sub Nav<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
                  <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
                <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
              <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
            <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
          <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
        <span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"music"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu2"</span>&gt;</span>音乐<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"file-text-o"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu4"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>文章<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"film"</span> <span class="hljs-attr">to</span>=<span class="hljs-string">"/components/menu/submenu3"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">span</span>&gt;</span>视频<span class="hljs-tag">&lt;/<span class="hljs-name">span</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">menus</span> <span class="hljs-attr">label</span>=<span class="hljs-string">"系统设置"</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"users"</span>&gt;</span>会员管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"ticket"</span>&gt;</span>工单管理<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"lock"</span>&gt;</span>修改密码<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"divider"</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">menu-item</span> <span class="hljs-attr">icon</span>=<span class="hljs-string">"sign-out"</span>&gt;</span>退出登录<span class="hljs-tag">&lt;/<span class="hljs-name">menu-item</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">menus</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<h4 id="menus"><a class="header-anchor" href="#menus" aria-hidden="true">¶</a> menus</h4>
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
<td>label</td>
<td>String</td>
<td>菜单集合的标签</td>
<td>无</td>
</tr>
</tbody>
</table>
<h4 id="menu-item"><a class="header-anchor" href="#menu-item" aria-hidden="true">¶</a> menu-item</h4>
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
<td>icon</td>
<td>图标</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>to</td>
<td>path of vue-router，same as the <code>to</code> parameter of vue-router</td>
<td>String</td>
<td>-</td>
</tr>
<tr>
<td>click</td>
<td>点击事件，设置此项 <code>to</code> 将失效</td>
<td>Function</td>
<td>无</td>
</tr>
<tr>
<td>is-active</td>
<td>菜单是否激活</td>
<td>Boolean</td>
<td>false</td>
</tr>
</tbody>
</table>
</section></template>

