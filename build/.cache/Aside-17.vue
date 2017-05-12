<template><section><h2 id="aside-ce-bian-mo-tai-kuang"><a class="header-anchor" href="#aside-ce-bian-mo-tai-kuang" aria-hidden="true">¶</a> Aside 侧边模态框</h2>
<p>从侧边滑出的模态框</p>
<h3 id="dai-ma-yan-shi"><a class="header-anchor" href="#dai-ma-yan-shi" aria-hidden="true">¶</a> 代码演示</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;b-aside :is-show=\&quot;isShow\&quot; title=\&quot;Left Aside!\&quot; @close=\&quot;isShow=false\&quot;&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n&lt;/b-aside&gt;\n&lt;button @click=\&quot;toggle\&quot; class=\&quot;button is-primary\&quot;&gt;左侧模态框&lt;/button&gt;\n\n&lt;b-aside :is-show=\&quot;isShowRight\&quot; title=\&quot;Right Aside!\&quot; :show-footer=\&quot;false\&quot; placement=\&quot;right\&quot; :backdrop=\&quot;false\&quot; @close=\&quot;isShowRight=false\&quot;&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n  &lt;p&gt;&lt;code&gt;右侧Aside并且不显示footer&lt;/code&gt;&lt;/p&gt;\n&lt;/b-aside&gt;\n&lt;button @click=\&quot;toggleRight\&quot; class=\&quot;button is-primary\&quot;&gt;右侧模态框&lt;/button&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
                    <div class="box-demo-show" slot="component"><b-aside :is-show="isShow" title="Left Aside!" @close="isShow=false">
  <h3>Dolor sit amet</h3>
  <p>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  </p>
  <h3>Dolor sit amet</h3>
  <p>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  </p>
</b-aside>
<button @click="toggle" class="button is-primary">左侧模态框</button>

<b-aside :is-show="isShowRight" title="Right Aside!" :show-footer="false" placement="right" :backdrop="false" @close="isShowRight=false">
  <h3>Dolor sit amet</h3>
  <p>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  </p>
  <h3>Dolor sit amet</h3>
  <p>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  </p>
  <p><code>右侧Aside并且不显示footer</code></p>
</b-aside>
<button @click="toggleRight" class="button is-primary">右侧模态框</button>

</div>
                    <div slot="description"><h4 id="ji-ben"><a class="header-anchor" href="#ji-ben" aria-hidden="true">¶</a> 基本</h4>
<ul>
<li>aside基本拥有modal所有的特性</li>
<li>通过<code>placement</code>设置侧边模态框的位置，目前支持 left 和 right</li>
</ul>
</div>
                    <div class="highlight" slot="code"><pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">b-aside</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow"</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Left Aside!"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">b-aside</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>左侧模态框<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">b-aside</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowRight"</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Right Aside!"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span> <span class="hljs-attr">:backdrop</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowRight=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">code</span>&gt;</span>右侧Aside并且不显示footer<span class="hljs-tag">&lt;/<span class="hljs-name">code</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">b-aside</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleRight"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>右侧模态框<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### 基本
  * aside基本拥有modal所有的特性
  * 通过`placement`设置侧边模态框的位置，目前支持 left 和 right
</summary>
<pre><code class="language-html"><span class="hljs-tag">&lt;<span class="hljs-name">b-aside</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShow"</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Left Aside!"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShow=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">b-aside</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>左侧模态框<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">b-aside</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowRight"</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Right Aside!"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span> <span class="hljs-attr">:backdrop</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowRight=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">code</span>&gt;</span>右侧Aside并且不显示footer<span class="hljs-tag">&lt;/<span class="hljs-name">code</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">b-aside</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleRight"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>右侧模态框<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<p>Aside是基于modal的组件，所以它拥有modal所有的特性，具体的参数可参考modal的文档，唯一不同的是Aside通过<code>placement</code>设置位置</p>
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
<td>placement</td>
<td>位置</td>
<td>String</td>
<td>left</td>
</tr>
<tr>
<td>width</td>
<td>宽度</td>
<td>Number</td>
<td>400</td>
</tr>
</tbody>
</table>

</section></template>

<script>
export default {
  data() {
    return {
      isShow: false,
      isShowRight: false,
    };
  },
  methods: {
    toggle() {
      this.isShow = !this.isShow;
    },
    toggleRight() {
      this.isShowRight = !this.isShowRight;
    },
  },
};
</script>