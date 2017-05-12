<template><section><h2 id="modal-mo-tai-kuang"><a class="header-anchor" href="#modal-mo-tai-kuang" aria-hidden="true">¶</a> Modal 模态框</h2>
<p>模态对话框</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;modal title=\&quot;Modal!\&quot; :width=\&quot;520\&quot; :is-show=\&quot;isShow\&quot; transition=\&quot;fadeDown\&quot; @close=\&quot;isShow=false\&quot;&gt;\n  &lt;h4&gt;Text in a modal&lt;/h4&gt;\n  &lt;p&gt;\n    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,\n    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.\n  &lt;/p&gt;\n&lt;/modal&gt;\n&lt;button @click=\&quot;toggle\&quot; class=\&quot;button is-primary\&quot;&gt;基本模态框&lt;/button&gt;\n\n&lt;modal title=\&quot;自定义按钮文字\&quot; :is-show=\&quot;isShow2\&quot; :show-footer=\&quot;false\&quot; :show-header=\&quot;true\&quot; @close=\&quot;isShow2=false\&quot; ok-text=\&quot;确定\&quot; cancel-text=\&quot;取消\&quot;&gt;\n  &lt;h4&gt;Text in a modal&lt;/h4&gt;\n  &lt;p&gt;\n    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,\n    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.\n  &lt;/p&gt;\n&lt;/modal&gt;\n&lt;button @click=\&quot;toggle2\&quot; class=\&quot;button is-primary\&quot;&gt;自定义按钮文字&lt;/button&gt;\n\n&lt;modal title=\&quot;禁用backdrop背景\&quot; :backdrop=\&quot;false\&quot; :is-show=\&quot;isShow3\&quot; @close=\&quot;isShow3=false\&quot;&gt;\n  &lt;h4&gt;Text in a modal&lt;/h4&gt;\n  &lt;p&gt;\n    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,\n    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.\n  &lt;/p&gt;\n&lt;/modal&gt;\n&lt;button @click=\&quot;toggle3\&quot; class=\&quot;button is-primary\&quot;&gt;禁用backdrop遮罩层&lt;/button&gt;\n\n&lt;modal title=\&quot;禁用遮罩层关闭\&quot; :backdrop-closable=\&quot;false\&quot; :is-show=\&quot;isShow4\&quot; @close=\&quot;isShow4=false\&quot;&gt;\n  &lt;h4&gt;Text in a modal&lt;/h4&gt;\n  &lt;p&gt;\n    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,\n    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.\n  &lt;/p&gt;\n&lt;/modal&gt;\n&lt;button @click=\&quot;toggle4\&quot; class=\&quot;button is-primary\&quot;&gt;禁用backdrop遮罩层关闭&lt;/button&gt;\n\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><modal title="Modal!" :width="520" :is-show="isShow" transition="fadeDown" @close="isShow=false">
  <h4>Text in a modal</h4>
  <p>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  </p>
</modal>
<button @click="toggle" class="button is-primary">基本模态框</button>

<modal title="自定义按钮文字" :is-show="isShow2" :show-footer="false" :show-header="true" @close="isShow2=false" ok-text="确定" cancel-text="取消">
  <h4>Text in a modal</h4>
  <p>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  </p>
</modal>
<button @click="toggle2" class="button is-primary">自定义按钮文字</button>

<modal title="禁用backdrop背景" :backdrop="false" :is-show="isShow3" @close="isShow3=false">
  <h4>Text in a modal</h4>
  <p>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  </p>
</modal>
<button @click="toggle3" class="button is-primary">禁用backdrop遮罩层</button>

<modal title="禁用遮罩层关闭" :backdrop-closable="false" :is-show="isShow4" @close="isShow4=false">
  <h4>Text in a modal</h4>
  <p>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  </p>
</modal>
<button @click="toggle4" class="button is-primary">禁用backdrop遮罩层关闭</button>


</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>通过设置<code>cancel-text</code>和<code>ok-text</code>自定义按钮文字</li>
<li>设置<code>backdrop</code>为false可禁用遮罩层</li>
<li>设置<code>backdrop-closable</code>为false可禁用遮罩层关闭</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Modal!"</span> <span class="hljs-attr">:width</span>=<span class="hljs-string">"520"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow"</span> <span class="hljs-attr">transition</span>=<span class="hljs-string">"fadeDown"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>基本模态框<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"自定义按钮文字"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow2"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:show-header</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow2=false"</span> <span class="hljs-attr">ok-text</span>=<span class="hljs-string">"确定"</span> <span class="hljs-attr">cancel-text</span>=<span class="hljs-string">"取消"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle2"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>自定义按钮文字<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"禁用backdrop背景"</span> <span class="hljs-attr">:backdrop</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow3"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow3=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle3"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>禁用backdrop遮罩层<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"禁用遮罩层关闭"</span> <span class="hljs-attr">:backdrop-closable</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow4"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow4=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle4"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>禁用backdrop遮罩层关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>


</code></pre>
</div>
                  <summary>
  #### 基本
  * 通过设置`cancel-text`和`ok-text`自定义按钮文字
  * 设置`backdrop`为false可禁用遮罩层
  * 设置`backdrop-closable`为false可禁用遮罩层关闭
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Modal!"</span> <span class="hljs-attr">:width</span>=<span class="hljs-string">"520"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow"</span> <span class="hljs-attr">transition</span>=<span class="hljs-string">"fadeDown"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>基本模态框<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"自定义按钮文字"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow2"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:show-header</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow2=false"</span> <span class="hljs-attr">ok-text</span>=<span class="hljs-string">"确定"</span> <span class="hljs-attr">cancel-text</span>=<span class="hljs-string">"取消"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle2"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>自定义按钮文字<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"禁用backdrop背景"</span> <span class="hljs-attr">:backdrop</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow3"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow3=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle3"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>禁用backdrop遮罩层<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"禁用遮罩层关闭"</span> <span class="hljs-attr">:backdrop-closable</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow4"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow4=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle4"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>禁用backdrop遮罩层关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>


</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;modal title=\&quot;回调处理\&quot; :on-ok=\&quot;okCb\&quot; :on-cancel=\&quot;cancelCb\&quot; :is-show=\&quot;isShowA\&quot; @close=\&quot;isShowA=false\&quot;&gt;\n  &lt;h4&gt;Text in a modal&lt;/h4&gt;\n  &lt;p&gt;\n    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,\n    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.\n  &lt;/p&gt;\n&lt;/modal&gt;\n&lt;button @click=\&quot;toggleA\&quot; class=\&quot;button is-primary\&quot;&gt;回调函数&lt;/button&gt;\n\n&lt;modal title=\&quot;异步关闭\&quot; :on-ok=\&quot;okCloseCb\&quot; ok-text=\&quot;确定\&quot; :ok-loading=\&quot;true\&quot; :is-show=\&quot;isShowC\&quot; @close=\&quot;isShowC=false\&quot;&gt;\n  &lt;h4&gt;Text in a modal&lt;/h4&gt;\n  &lt;p&gt;\n    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,\n    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.\n  &lt;/p&gt;\n&lt;/modal&gt;\n&lt;button @click=\&quot;toggleC\&quot; class=\&quot;button is-primary\&quot;&gt;异步关闭&lt;/button&gt;\n\n\n\n&quot;,&quot;script&quot;:&quot;\nexport default {\n  data() {\n    return {\n      isShow: false,\n    };\n  },\n  methods: {\n    toggle() {\n      this.isShow = !this.isShow;\n    },\n    okCb() {\n      this.$notify.open({\n        type: 'success',\n        title: `ok回调`,\n      });\n    },\n    cancelCb() {\n      this.$notify.open({\n        type: 'success',\n        title: `cancel回调`,\n      });\n    },\n    okCloseCb() {\n      setTimeout(() =&gt; {\n        this.toggle();\n      }, 2000);\n    },\n  },\n};\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><modal title="回调处理" :on-ok="okCb" :on-cancel="cancelCb" :is-show="isShowA" @close="isShowA=false">
  <h4>Text in a modal</h4>
  <p>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  </p>
</modal>
<button @click="toggleA" class="button is-primary">回调函数</button>

<modal title="异步关闭" :on-ok="okCloseCb" ok-text="确定" :ok-loading="true" :is-show="isShowC" @close="isShowC=false">
  <h4>Text in a modal</h4>
  <p>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  </p>
</modal>
<button @click="toggleC" class="button is-primary">异步关闭</button>



</div>
                    <div slot="description"><h4 id="hui-diao-he-yi-bu-guan-bi"><a class="header-anchor" href="#hui-diao-he-yi-bu-guan-bi" aria-hidden="true">¶</a> 回调和异步关闭</h4>
<ul>
<li>设置<code>on-ok</code>或<code>on-cancel</code>，为modal添加回调</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"回调处理"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"okCb"</span> <span class="hljs-attr">:on-cancel</span>=<span class="hljs-string">"cancelCb"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowA"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowA=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleA"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>回调函数<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"异步关闭"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"okCloseCb"</span> <span class="hljs-attr">ok-text</span>=<span class="hljs-string">"确定"</span> <span class="hljs-attr">:ok-loading</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowC"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowC=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleC"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>异步关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>


<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  data() {
    <span class="hljs-keyword">return</span> {
      <span class="hljs-attr">isShow</span>: <span class="hljs-literal">false</span>,
    };
  },
  <span class="hljs-attr">methods</span>: {
    toggle() {
      <span class="hljs-keyword">this</span>.isShow = !<span class="hljs-keyword">this</span>.isShow;
    },
    okCb() {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">title</span>: <span class="hljs-string">`ok回调`</span>,
      });
    },
    cancelCb() {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">title</span>: <span class="hljs-string">`cancel回调`</span>,
      });
    },
    okCloseCb() {
      setTimeout(<span class="hljs-function"><span class="hljs-params">()</span> =&gt;</span> {
        <span class="hljs-keyword">this</span>.toggle();
      }, <span class="hljs-number">2000</span>);
    },
  },
};
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 回调和异步关闭
  * 设置`on-ok`或`on-cancel`，为modal添加回调
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"回调处理"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"okCb"</span> <span class="hljs-attr">:on-cancel</span>=<span class="hljs-string">"cancelCb"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowA"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowA=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleA"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>回调函数<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"异步关闭"</span> <span class="hljs-attr">:on-ok</span>=<span class="hljs-string">"okCloseCb"</span> <span class="hljs-attr">ok-text</span>=<span class="hljs-string">"确定"</span> <span class="hljs-attr">:ok-loading</span>=<span class="hljs-string">"true"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowC"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowC=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleC"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>异步关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>


<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  data() {
    <span class="hljs-keyword">return</span> {
      <span class="hljs-attr">isShow</span>: <span class="hljs-literal">false</span>,
    };
  },
  <span class="hljs-attr">methods</span>: {
    toggle() {
      <span class="hljs-keyword">this</span>.isShow = !<span class="hljs-keyword">this</span>.isShow;
    },
    okCb() {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">title</span>: <span class="hljs-string">`ok回调`</span>,
      });
    },
    cancelCb() {
      <span class="hljs-keyword">this</span>.$notify.open({
        <span class="hljs-attr">type</span>: <span class="hljs-string">'success'</span>,
        <span class="hljs-attr">title</span>: <span class="hljs-string">`cancel回调`</span>,
      });
    },
    okCloseCb() {
      setTimeout(<span class="hljs-function"><span class="hljs-params">()</span> =&gt;</span> {
        <span class="hljs-keyword">this</span>.toggle();
      }, <span class="hljs-number">2000</span>);
    },
  },
};
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</demo-box>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;modal title=\&quot;回调处理\&quot; :is-show=\&quot;isShowE\&quot; @close=\&quot;isShowE=false\&quot;&gt;\n  &lt;div slot=\&quot;header\&quot; class=\&quot;columns\&quot; style=\&quot;width: 100%\&quot;&gt;\n    &lt;div class=\&quot;tabs is-pulled-left\&quot;&gt;\n      &lt;ul&gt;\n        &lt;li class=\&quot;is-active\&quot;&gt;&lt;a&gt;Pictures&lt;/a&gt;&lt;/li&gt;\n        &lt;li&gt;&lt;a&gt;Music&lt;/a&gt;&lt;/li&gt;\n        &lt;li&gt;&lt;a&gt;Videos&lt;/a&gt;&lt;/li&gt;\n        &lt;li&gt;&lt;a&gt;Documents&lt;/a&gt;&lt;/li&gt;\n      &lt;/ul&gt;\n    &lt;/div&gt;\n    &lt;button class=\&quot;button is-primary is-pulled-right\&quot; @click=\&quot;toggleE\&quot;&gt;Close&lt;/button&gt;\n  &lt;/div&gt;\n  &lt;h4&gt;Text in a modal&lt;/h4&gt;\n  &lt;p&gt;\n    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,\n    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.\n  &lt;/p&gt;\n  &lt;p&gt;&lt;button class=\&quot;button is-primary\&quot; @click=\&quot;toggleE\&quot;&gt;Close&lt;/button&gt;&lt;/p&gt;\n  &lt;p&gt;Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor&lt;/p&gt;\n  &lt;div slot=\&quot;footer\&quot;&gt;我来组成尾部&lt;/div&gt;\n&lt;/modal&gt;\n&lt;button @click=\&quot;toggleE\&quot; class=\&quot;button\&quot;&gt;自定义头部尾部&lt;/button&gt;\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><modal title="回调处理" :is-show="isShowE" @close="isShowE=false">
  <div slot="header" class="columns" style="width: 100%">
    <div class="tabs is-pulled-left">
      <ul>
        <li class="is-active"><a>Pictures</a></li>
        <li><a>Music</a></li>
        <li><a>Videos</a></li>
        <li><a>Documents</a></li>
      </ul>
    </div>
    <button class="button is-primary is-pulled-right" @click="toggleE">Close</button>
  </div>
  <h4>Text in a modal</h4>
  <p>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  </p>
  <p><button class="button is-primary" @click="toggleE">Close</button></p>
  <p>Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor</p>
  <div slot="footer">我来组成尾部</div>
</modal>
<button @click="toggleE" class="button">自定义头部尾部</button>
</div>
                    <div slot="description"><h4 id="zi-ding-yi-tou-wei"><a class="header-anchor" href="#zi-ding-yi-tou-wei" aria-hidden="true">¶</a> 自定义头尾</h4>
<ul>
<li>通过Vue的Slot功能可灵活定义Modal的头部和尾部</li>
<li><code>slot=&quot;header&quot;</code>定义头部，<code>slot=&quot;footer&quot;</code>定义尾部</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"回调处理"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowE"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowE=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"header"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 100%"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"tabs is-pulled-left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">ul</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"is-active"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Pictures<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Music<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Videos<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Documents<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">ul</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-pulled-right"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleE"</span>&gt;</span>Close<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleE"</span>&gt;</span>Close<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"footer"</span>&gt;</span>我来组成尾部<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleE"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>自定义头部尾部<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### 自定义头尾
  * 通过Vue的Slot功能可灵活定义Modal的头部和尾部
  * `slot="header"`定义头部，`slot="footer"`定义尾部
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">modal</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"回调处理"</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowE"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowE=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"header"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"columns"</span> <span class="hljs-attr">style</span>=<span class="hljs-string">"width: 100%"</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"tabs is-pulled-left"</span>&gt;</span>
      <span class="hljs-tag">&lt;<span class="hljs-name">ul</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"is-active"</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Pictures<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Music<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Videos<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
        <span class="hljs-tag">&lt;<span class="hljs-name">li</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">a</span>&gt;</span>Documents<span class="hljs-tag">&lt;/<span class="hljs-name">a</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">li</span>&gt;</span>
      <span class="hljs-tag">&lt;/<span class="hljs-name">ul</span>&gt;</span>
    <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
    <span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary is-pulled-right"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleE"</span>&gt;</span>Close<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
  <span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h4</span>&gt;</span>Text in a modal<span class="hljs-tag">&lt;/<span class="hljs-name">h4</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>
    Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem. Praesent commodo cursus magna,
    vel scelerisque nisl consectetur et. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleE"</span>&gt;</span>Close<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor<span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">div</span> <span class="hljs-attr">slot</span>=<span class="hljs-string">"footer"</span>&gt;</span>我来组成尾部<span class="hljs-tag">&lt;/<span class="hljs-name">div</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">modal</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleE"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>自定义头部尾部<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
</code></pre>
</demo-box>
<h3 id="quan-ju-fang-fa-modal"><a class="header-anchor" href="#quan-ju-fang-fa-modal" aria-hidden="true">¶</a> 全局方法($modal)</h3>
<p>为了方便使用提示信息类的modal，Vue-Blu为Vue.prototype注册了$modal对象，可使用<code>this.$modal.open(config)</code>来快捷调用modal</p>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;\n&lt;button @click=\&quot;openModal\&quot; class=\&quot;button\&quot;&gt;$modal.open&lt;/button&gt;\n&lt;button @click=\&quot;openConfirm\&quot; class=\&quot;button is-primary\&quot;&gt;$modal.confirm&lt;/button&gt;\n&lt;button @click=\&quot;openAlert\&quot; class=\&quot;button is-danger\&quot;&gt;$modal.alert&lt;/button&gt;\n&lt;button @click=\&quot;manualClose\&quot; class=\&quot;button is-primary\&quot;&gt;手动关闭&lt;/button&gt;\n&lt;button @click=\&quot;disableHeader\&quot; class=\&quot;button is-primary\&quot;&gt;不显示Header&lt;/button&gt;\n\n&quot;,&quot;script&quot;:&quot;\nexport default {\n  methods: {\n    openModal() {\n      this.$modal.open({\n        autoClose: 3,\n        content: '将在3秒后自动关闭...'\n      });\n    },\n    openConfirm() {\n      this.$modal.confirm({\n        content: '确定删除这条信息?',\n        onOk: this.okCb,\n      });\n    },\n    openAlert() {\n      this.$modal.alert({\n        content: '操作失败！请联系管理员',\n      });\n    },\n    manualClose() {\n      const m = this.$modal.open({\n        content: '将在3秒后调用close()关闭...'\n      });\n      setTimeout(() =&gt; {\n        m.close();\n      },3000);\n    },\n    disableHeader() {\n      this.$modal.open({\n        content: '不显示header',\n        showHeader: false,\n      });\n    },\n  },\n};\n&quot;,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component">
<button @click="openModal" class="button">$modal.open</button>
<button @click="openConfirm" class="button is-primary">$modal.confirm</button>
<button @click="openAlert" class="button is-danger">$modal.alert</button>
<button @click="manualClose" class="button is-primary">手动关闭</button>
<button @click="disableHeader" class="button is-primary">不显示Header</button>

</div>
                    <div slot="description"><h4 id="modal"><a class="header-anchor" href="#modal" aria-hidden="true">¶</a> $modal</h4>
<ul>
<li><code>this.$modal</code>包含<code>open</code> <code>confirm</code> <code>alert</code> 三个方法</li>
<li><code>this.$modal.open(config)</code>快捷打开modal</li>
<li>通过<code>icon</code>自定义图标</li>
<li>通过设置<code>autoClose</code>倒计时自动关闭modal</li>
<li>$modal实例化后，可通过调用它的<code>close</code>方法手动关闭modal</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"openModal"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>$modal.open<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"openConfirm"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>$modal.confirm<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"openAlert"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span>&gt;</span>$modal.alert<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"manualClose"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>手动关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"disableHeader"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>不显示Header<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  <span class="hljs-attr">methods</span>: {
    openModal() {
      <span class="hljs-keyword">this</span>.$modal.open({
        <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
        <span class="hljs-attr">content</span>: <span class="hljs-string">'将在3秒后自动关闭...'</span>
      });
    },
    openConfirm() {
      <span class="hljs-keyword">this</span>.$modal.confirm({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'确定删除这条信息?'</span>,
        <span class="hljs-attr">onOk</span>: <span class="hljs-keyword">this</span>.okCb,
      });
    },
    openAlert() {
      <span class="hljs-keyword">this</span>.$modal.alert({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'操作失败！请联系管理员'</span>,
      });
    },
    manualClose() {
      <span class="hljs-keyword">const</span> m = <span class="hljs-keyword">this</span>.$modal.open({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'将在3秒后调用close()关闭...'</span>
      });
      setTimeout(<span class="hljs-function"><span class="hljs-params">()</span> =&gt;</span> {
        m.close();
      },<span class="hljs-number">3000</span>);
    },
    disableHeader() {
      <span class="hljs-keyword">this</span>.$modal.open({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'不显示header'</span>,
        <span class="hljs-attr">showHeader</span>: <span class="hljs-literal">false</span>,
      });
    },
  },
};
</span><span class="hljs-tag">&lt;/<span class="hljs-name">script</span>&gt;</span>
</code></pre>
</div>
                  <summary>
  #### $modal
  * `this.$modal`包含`open` `confirm` `alert` 三个方法
  * `this.$modal.open(config)`快捷打开modal
  * 通过`icon`自定义图标
  * 通过设置`autoClose`倒计时自动关闭modal
  * $modal实例化后，可通过调用它的`close`方法手动关闭modal
</summary>
<pre><code class="language-html">
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"openModal"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button"</span>&gt;</span>$modal.open<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"openConfirm"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>$modal.confirm<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"openAlert"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-danger"</span>&gt;</span>$modal.alert<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"manualClose"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>手动关闭<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"disableHeader"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>不显示Header<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">script</span>&gt;</span><span class="javascript">
<span class="hljs-keyword">export</span> <span class="hljs-keyword">default</span> {
  <span class="hljs-attr">methods</span>: {
    openModal() {
      <span class="hljs-keyword">this</span>.$modal.open({
        <span class="hljs-attr">autoClose</span>: <span class="hljs-number">3</span>,
        <span class="hljs-attr">content</span>: <span class="hljs-string">'将在3秒后自动关闭...'</span>
      });
    },
    openConfirm() {
      <span class="hljs-keyword">this</span>.$modal.confirm({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'确定删除这条信息?'</span>,
        <span class="hljs-attr">onOk</span>: <span class="hljs-keyword">this</span>.okCb,
      });
    },
    openAlert() {
      <span class="hljs-keyword">this</span>.$modal.alert({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'操作失败！请联系管理员'</span>,
      });
    },
    manualClose() {
      <span class="hljs-keyword">const</span> m = <span class="hljs-keyword">this</span>.$modal.open({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'将在3秒后调用close()关闭...'</span>
      });
      setTimeout(<span class="hljs-function"><span class="hljs-params">()</span> =&gt;</span> {
        m.close();
      },<span class="hljs-number">3000</span>);
    },
    disableHeader() {
      <span class="hljs-keyword">this</span>.$modal.open({
        <span class="hljs-attr">content</span>: <span class="hljs-string">'不显示header'</span>,
        <span class="hljs-attr">showHeader</span>: <span class="hljs-literal">false</span>,
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
<td>is-show</td>
<td>modal是否显示</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>title</td>
<td>标题</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>ok-text</td>
<td>确定按钮的文字</td>
<td>String</td>
<td>OK</td>
</tr>
<tr>
<td>cancel-text</td>
<td>取消按钮的文字</td>
<td>String</td>
<td>Cancel</td>
</tr>
<tr>
<td>on-ok</td>
<td>点击ok后的回调</td>
<td>Function</td>
<td>无</td>
</tr>
<tr>
<td>on-cancel</td>
<td>点击cancel后的回调</td>
<td>Function</td>
<td>无</td>
</tr>
<tr>
<td>backdrop</td>
<td>是否显示遮罩层</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>backdrop-closable</td>
<td>遮罩层是否可关闭modal</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>okLoading</td>
<td>确定按钮loading（开启后点击ok将不会自动关闭modal）</td>
<td>Boolean</td>
<td>false</td>
</tr>
<tr>
<td>width</td>
<td>modal的宽度</td>
<td>Number</td>
<td>640</td>
</tr>
<tr>
<td>transition</td>
<td>过渡效果,可选值见 #link</td>
<td>String</td>
<td>fade</td>
</tr>
<tr>
<td>show-header</td>
<td>是否显示头部</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>show-footer</td>
<td>是否显示尾部</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>show-ok</td>
<td>是否显示ok按钮</td>
<td>Boolean</td>
<td>true</td>
</tr>
<tr>
<td>show-cancel</td>
<td>是否显示cancel按钮</td>
<td>Boolean</td>
<td>true</td>
</tr>
</tbody>
</table>
<h4 id="modal-quan-ju-dui-xiang"><a class="header-anchor" href="#modal-quan-ju-dui-xiang" aria-hidden="true">¶</a> $modal全局对象</h4>
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
<td>width</td>
<td>modal的宽度</td>
<td>Number</td>
<td>400</td>
</tr>
<tr>
<td>icon</td>
<td>图标</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>title</td>
<td>标题</td>
<td>String</td>
<td></td>
</tr>
<tr>
<td>content</td>
<td>内容</td>
<td>String</td>
<td>无</td>
</tr>
<tr>
<td>autoClose</td>
<td>自动关闭的倒计时秒数</td>
<td>Number</td>
<td>0(表示禁用自动关闭)</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  data() {
    return {
      isShow: false,
      isShow2: false,
      isShow3: false,
      isShow4: false,
      isShowA: false,
      isShowB: false,
      isShowC: false,
      isShowE: false,
    };
  },

  methods: {
    toggle() {
      this.isShow = !this.isShow;
    },
    toggle2() {
      this.isShow2 = !this.isShow2;
    },
    toggle3() {
      this.isShow3 = !this.isShow3;
    },
    toggle4() {
      this.isShow4 = !this.isShow4;
    },
    toggleA() {
      this.isShowA = !this.isShowA;
    },
    toggleB() {
      this.isShowB = !this.isShowB;
    },
    toggleC() {
      this.isShowC = !this.isShowC;
    },
    toggleE() {
      this.isShowE = !this.isShowE;
    },
    okCb() {
      this.$notify.open({
        type: 'success',
        title: `ok回调`,
      });
    },
    cancelCb() {
      this.$notify.open({
        type: 'success',
        title: `cancel回调`,
      });
    },
    okCloseCb() {
      setTimeout(() => {
        this.toggleC();
      }, 2000);
    },
    openModal() {
      this.$modal.open({
        autoClose: 3,
        content: '将在3秒后自动关闭...'
      });
    },

    openConfirm() {
      this.$modal.confirm({
        content: '确定删除这条信息?',
        onOk: this.okCb,
      });
    },
    openAlert() {
      this.$modal.alert({
        content: '操作失败！请联系管理员',
      });
    },
    manualClose() {
      const m = this.$modal.open({
        content: '将在3秒后调用close()关闭...'
      });
      setTimeout(() => {
        m.close();
      },3000);
    },
    disableHeader() {
      this.$modal.open({
        content: '不显示header',
        showHeader: false,
      });
    },
  }
};
</script>