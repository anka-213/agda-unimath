# Graph theory

<pre class="Agda"><a id="25" class="Symbol">{-#</a> <a id="29" class="Keyword">OPTIONS</a> <a id="37" class="Pragma">--without-K</a> <a id="49" class="Pragma">--exact-split</a> <a id="63" class="Symbol">#-}</a>

<a id="68" class="Keyword">module</a> <a id="75" href="graph-theory.html" class="Module">graph-theory</a> <a id="88" class="Keyword">where</a>
</pre>
<pre class="Agda"><a id="107" class="Keyword">open</a> <a id="112" class="Keyword">import</a> <a id="119" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a> <a id="160" class="Keyword">public</a>
<a id="167" class="Keyword">open</a> <a id="172" class="Keyword">import</a> <a id="179" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a> <a id="208" class="Keyword">public</a>
<a id="215" class="Keyword">open</a> <a id="220" class="Keyword">import</a> <a id="227" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a> <a id="272" class="Keyword">public</a>
<a id="279" class="Keyword">open</a> <a id="284" class="Keyword">import</a> <a id="291" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a> <a id="333" class="Keyword">public</a>
<a id="340" class="Keyword">open</a> <a id="345" class="Keyword">import</a> <a id="352" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a> <a id="396" class="Keyword">public</a>
<a id="403" class="Keyword">open</a> <a id="408" class="Keyword">import</a> <a id="415" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a> <a id="465" class="Keyword">public</a>
<a id="472" class="Keyword">open</a> <a id="477" class="Keyword">import</a> <a id="484" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a> <a id="511" class="Keyword">public</a>
<a id="518" class="Keyword">open</a> <a id="523" class="Keyword">import</a> <a id="530" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a> <a id="571" class="Keyword">public</a>
<a id="578" class="Keyword">open</a> <a id="583" class="Keyword">import</a> <a id="590" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a> <a id="613" class="Keyword">public</a>
<a id="620" class="Keyword">open</a> <a id="625" class="Keyword">import</a> <a id="632" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a> <a id="681" class="Keyword">public</a>
<a id="688" class="Keyword">open</a> <a id="693" class="Keyword">import</a> <a id="700" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a> <a id="739" class="Keyword">public</a>
<a id="746" class="Keyword">open</a> <a id="751" class="Keyword">import</a> <a id="758" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a> <a id="799" class="Keyword">public</a>
<a id="806" class="Keyword">open</a> <a id="811" class="Keyword">import</a> <a id="818" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a> <a id="862" class="Keyword">public</a>
<a id="869" class="Keyword">open</a> <a id="874" class="Keyword">import</a> <a id="881" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a> <a id="918" class="Keyword">public</a>
<a id="925" class="Keyword">open</a> <a id="930" class="Keyword">import</a> <a id="937" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a> <a id="959" class="Keyword">public</a>
<a id="966" class="Keyword">open</a> <a id="971" class="Keyword">import</a> <a id="978" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a> <a id="1008" class="Keyword">public</a>
<a id="1015" class="Keyword">open</a> <a id="1020" class="Keyword">import</a> <a id="1027" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a> <a id="1066" class="Keyword">public</a>
<a id="1073" class="Keyword">open</a> <a id="1078" class="Keyword">import</a> <a id="1085" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a> <a id="1123" class="Keyword">public</a>
<a id="1130" class="Keyword">open</a> <a id="1135" class="Keyword">import</a> <a id="1142" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a> <a id="1200" class="Keyword">public</a>
<a id="1207" class="Keyword">open</a> <a id="1212" class="Keyword">import</a> <a id="1219" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a> <a id="1250" class="Keyword">public</a>
<a id="1257" class="Keyword">open</a> <a id="1262" class="Keyword">import</a> <a id="1269" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a> <a id="1297" class="Keyword">public</a>
</pre>