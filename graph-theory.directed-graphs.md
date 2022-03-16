# Directed graphs

<pre class="Agda"><a id="28" class="Symbol">{-#</a> <a id="32" class="Keyword">OPTIONS</a> <a id="40" class="Pragma">--without-K</a> <a id="52" class="Pragma">--exact-split</a> <a id="66" class="Symbol">#-}</a>

<a id="71" class="Keyword">module</a> <a id="78" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a> <a id="107" class="Keyword">where</a>

<a id="114" class="Keyword">open</a> <a id="119" class="Keyword">import</a> <a id="126" href="univalent-foundations.html" class="Module">univalent-foundations</a> <a id="148" class="Keyword">public</a>
</pre>
## Idea

A graph consists of a type of vertices equipped with a binary, type valued relation of edges.

## Definition

<pre class="Agda"><a id="Graph"></a><a id="287" href="graph-theory.directed-graphs.html#287" class="Function">Graph</a> <a id="293" class="Symbol">:</a> <a id="295" class="Symbol">(</a><a id="296" href="graph-theory.directed-graphs.html#296" class="Bound">l1</a> <a id="299" href="graph-theory.directed-graphs.html#299" class="Bound">l2</a> <a id="302" class="Symbol">:</a> <a id="304" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="309" class="Symbol">)</a> <a id="311" class="Symbol">→</a> <a id="313" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="316" class="Symbol">(</a><a id="317" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="322" href="graph-theory.directed-graphs.html#296" class="Bound">l1</a> <a id="325" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="327" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="332" href="graph-theory.directed-graphs.html#299" class="Bound">l2</a><a id="334" class="Symbol">)</a>
<a id="336" href="graph-theory.directed-graphs.html#287" class="Function">Graph</a> <a id="342" href="graph-theory.directed-graphs.html#342" class="Bound">l1</a> <a id="345" href="graph-theory.directed-graphs.html#345" class="Bound">l2</a> <a id="348" class="Symbol">=</a> <a id="350" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="352" class="Symbol">(</a><a id="353" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="356" href="graph-theory.directed-graphs.html#342" class="Bound">l1</a><a id="358" class="Symbol">)</a> <a id="360" class="Symbol">(λ</a> <a id="363" href="graph-theory.directed-graphs.html#363" class="Bound">V</a> <a id="365" class="Symbol">→</a> <a id="367" href="graph-theory.directed-graphs.html#363" class="Bound">V</a> <a id="369" class="Symbol">→</a> <a id="371" href="graph-theory.directed-graphs.html#363" class="Bound">V</a> <a id="373" class="Symbol">→</a> <a id="375" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="378" href="graph-theory.directed-graphs.html#345" class="Bound">l2</a><a id="380" class="Symbol">)</a>

<a id="383" class="Keyword">module</a> <a id="390" href="graph-theory.directed-graphs.html#390" class="Module">_</a>
  <a id="394" class="Symbol">{</a><a id="395" href="graph-theory.directed-graphs.html#395" class="Bound">l1</a> <a id="398" href="graph-theory.directed-graphs.html#398" class="Bound">l2</a> <a id="401" class="Symbol">:</a> <a id="403" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="408" class="Symbol">}</a> <a id="410" class="Symbol">(</a><a id="411" href="graph-theory.directed-graphs.html#411" class="Bound">G</a> <a id="413" class="Symbol">:</a> <a id="415" href="graph-theory.directed-graphs.html#287" class="Function">Graph</a> <a id="421" href="graph-theory.directed-graphs.html#395" class="Bound">l1</a> <a id="424" href="graph-theory.directed-graphs.html#398" class="Bound">l2</a><a id="426" class="Symbol">)</a>
  <a id="430" class="Keyword">where</a>

  <a id="439" href="graph-theory.directed-graphs.html#439" class="Function">vertex-Graph</a> <a id="452" class="Symbol">:</a> <a id="454" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="457" href="graph-theory.directed-graphs.html#395" class="Bound">l1</a>
  <a id="462" href="graph-theory.directed-graphs.html#439" class="Function">vertex-Graph</a> <a id="475" class="Symbol">=</a> <a id="477" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="481" href="graph-theory.directed-graphs.html#411" class="Bound">G</a>

  <a id="486" href="graph-theory.directed-graphs.html#486" class="Function">edge-Graph</a> <a id="497" class="Symbol">:</a> <a id="499" href="graph-theory.directed-graphs.html#439" class="Function">vertex-Graph</a> <a id="512" class="Symbol">→</a> <a id="514" href="graph-theory.directed-graphs.html#439" class="Function">vertex-Graph</a> <a id="527" class="Symbol">→</a> <a id="529" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="532" href="graph-theory.directed-graphs.html#398" class="Bound">l2</a>
  <a id="537" href="graph-theory.directed-graphs.html#486" class="Function">edge-Graph</a> <a id="548" class="Symbol">=</a> <a id="550" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="554" href="graph-theory.directed-graphs.html#411" class="Bound">G</a>
</pre>