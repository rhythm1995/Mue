<template><section><h2 id="aside"><a class="header-anchor" href="#aside" aria-hidden="true">¶</a> Aside</h2>
<p>Create a smooth off-canvas sidebar that slides in and out of the page</p>
<h3 id="examples"><a class="header-anchor" href="#examples" aria-hidden="true">¶</a> Examples</h3>
<demo-box :jsfiddle="{&quot;html&quot;:&quot;&lt;b-aside :is-show=\&quot;isShow\&quot; title=\&quot;Left Aside!\&quot; @close=\&quot;isShow=false\&quot;&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n&lt;/b-aside&gt;\n&lt;button @click=\&quot;toggle\&quot; class=\&quot;button is-primary\&quot;&gt;Left Aside&lt;/button&gt;\n\n&lt;b-aside :is-show=\&quot;isShowRight\&quot; title=\&quot;Right Aside!\&quot; :show-footer=\&quot;false\&quot; placement=\&quot;right\&quot; :backdrop=\&quot;false\&quot; @close=\&quot;isShowRight=false\&quot;&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n  &lt;h3&gt;Dolor sit amet&lt;/h3&gt;\n  &lt;p&gt;Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,\n    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.\n  &lt;/p&gt;\n  &lt;p&gt;&lt;code&gt;Right Aside with no footer&lt;/code&gt;&lt;/p&gt;\n&lt;/b-aside&gt;\n&lt;button @click=\&quot;toggleRight\&quot; class=\&quot;button is-primary\&quot;&gt;Right Aside&lt;/button&gt;\n\n&quot;,&quot;script&quot;:null,&quot;style&quot;:null}">
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
<button @click="toggle" class="button is-primary">Left Aside</button>

<b-aside :is-show="isShowRight" title="Right Aside!" :show-footer="false" placement="right" :backdrop="false" @close="isShowRight=false">
  <h3>Dolor sit amet</h3>
  <p>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  </p>
  <h3>Dolor sit amet</h3>
  <p>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  </p>
  <p><code>Right Aside with no footer</code></p>
</b-aside>
<button @click="toggleRight" class="button is-primary">Right Aside</button>

</div>
                    <div slot="description"><h4 id="basic"><a class="header-anchor" href="#basic" aria-hidden="true">¶</a> Basic</h4>
<ul>
<li>aside component is inherited from modal component,so it has all feature of modal</li>
<li>Sets which side that that the component slides from by <code>placement</code>，accept left and right</li>
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
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Left Aside<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">b-aside</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowRight"</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Right Aside!"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span> <span class="hljs-attr">:backdrop</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowRight=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">code</span>&gt;</span>Right Aside with no footer<span class="hljs-tag">&lt;/<span class="hljs-name">code</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">b-aside</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleRight"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Right Aside<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

</code></pre>
</div>
                  <summary>
  #### Basic
  * aside component is inherited from modal component,so it has all feature of modal
  * Sets which side that that the component slides from by `placement`，accept left and right
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
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggle"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Left Aside<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

<span class="hljs-tag">&lt;<span class="hljs-name">b-aside</span> <span class="hljs-attr">:is-show</span>=<span class="hljs-string">"isShowRight"</span> <span class="hljs-attr">title</span>=<span class="hljs-string">"Right Aside!"</span> <span class="hljs-attr">:show-footer</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">placement</span>=<span class="hljs-string">"right"</span> <span class="hljs-attr">:backdrop</span>=<span class="hljs-string">"false"</span> <span class="hljs-attr">@close</span>=<span class="hljs-string">"isShowRight=false"</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">h3</span>&gt;</span>Dolor sit amet<span class="hljs-tag">&lt;/<span class="hljs-name">h3</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span>Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo,
    fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
  <span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
  <span class="hljs-tag">&lt;<span class="hljs-name">p</span>&gt;</span><span class="hljs-tag">&lt;<span class="hljs-name">code</span>&gt;</span>Right Aside with no footer<span class="hljs-tag">&lt;/<span class="hljs-name">code</span>&gt;</span><span class="hljs-tag">&lt;/<span class="hljs-name">p</span>&gt;</span>
<span class="hljs-tag">&lt;/<span class="hljs-name">b-aside</span>&gt;</span>
<span class="hljs-tag">&lt;<span class="hljs-name">button</span> <span class="hljs-attr">@click</span>=<span class="hljs-string">"toggleRight"</span> <span class="hljs-attr">class</span>=<span class="hljs-string">"button is-primary"</span>&gt;</span>Right Aside<span class="hljs-tag">&lt;/<span class="hljs-name">button</span>&gt;</span>

</code></pre>
</demo-box>
<h3 id="api"><a class="header-anchor" href="#api" aria-hidden="true">¶</a> API</h3>
<p>Aside component is inherited from modal component,so it has all feature of modal,Consult
<router-link to="/en/components/modal">Modal's documentation</router-link> to find more APIs.</p>
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
<td>placement</td>
<td>position</td>
<td>String</td>
<td>left</td>
</tr>
<tr>
<td>width</td>
<td>width</td>
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