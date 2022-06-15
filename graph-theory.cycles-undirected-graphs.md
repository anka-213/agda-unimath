---
title: Cycles in undirected graphs
---

<pre class="Agda"><a id="53" class="Symbol">{-#</a> <a id="57" class="Keyword">OPTIONS</a> <a id="65" class="Pragma">--without-K</a> <a id="77" class="Pragma">--exact-split</a> <a id="91" class="Symbol">#-}</a>

<a id="96" class="Keyword">module</a> <a id="103" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a> <a id="141" class="Keyword">where</a>

<a id="148" class="Keyword">open</a> <a id="153" class="Keyword">import</a> <a id="160" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="202" class="Keyword">open</a> <a id="207" class="Keyword">import</a> <a id="214" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="246" class="Keyword">open</a> <a id="251" class="Keyword">import</a> <a id="258" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="286" class="Keyword">open</a> <a id="291" class="Keyword">import</a> <a id="298" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="340" class="Keyword">open</a> <a id="345" class="Keyword">import</a> <a id="352" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="374" class="Keyword">open</a> <a id="379" class="Keyword">import</a> <a id="386" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Idea

A cycle in an undirected graph `G` consists of a `k`-gon `H` equipped with an embedding of graphs from `H` into `G`.

## Definition

<pre class="Agda"><a id="572" class="Keyword">module</a> <a id="579" href="graph-theory.cycles-undirected-graphs.html#579" class="Module">_</a>
  <a id="583" class="Symbol">{</a><a id="584" href="graph-theory.cycles-undirected-graphs.html#584" class="Bound">l1</a> <a id="587" href="graph-theory.cycles-undirected-graphs.html#587" class="Bound">l2</a> <a id="590" class="Symbol">:</a> <a id="592" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="597" class="Symbol">}</a> <a id="599" class="Symbol">(</a><a id="600" href="graph-theory.cycles-undirected-graphs.html#600" class="Bound">k</a> <a id="602" class="Symbol">:</a> <a id="604" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="605" class="Symbol">)</a> <a id="607" class="Symbol">(</a><a id="608" href="graph-theory.cycles-undirected-graphs.html#608" class="Bound">G</a> <a id="610" class="Symbol">:</a> <a id="612" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="629" href="graph-theory.cycles-undirected-graphs.html#584" class="Bound">l1</a> <a id="632" href="graph-theory.cycles-undirected-graphs.html#587" class="Bound">l2</a><a id="634" class="Symbol">)</a>
  <a id="638" class="Keyword">where</a>

  <a id="647" href="graph-theory.cycles-undirected-graphs.html#647" class="Function">cycle-Undirected-Graph</a> <a id="670" class="Symbol">:</a> <a id="672" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="675" class="Symbol">(</a><a id="676" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="681" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="687" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="689" href="graph-theory.cycles-undirected-graphs.html#584" class="Bound">l1</a> <a id="692" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="694" href="graph-theory.cycles-undirected-graphs.html#587" class="Bound">l2</a><a id="696" class="Symbol">)</a>
  <a id="700" href="graph-theory.cycles-undirected-graphs.html#647" class="Function">cycle-Undirected-Graph</a> <a id="723" class="Symbol">=</a>
    <a id="729" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="731" class="Symbol">(</a><a id="732" href="graph-theory.polygons.html#2934" class="Function">Polygon</a> <a id="740" href="graph-theory.cycles-undirected-graphs.html#600" class="Bound">k</a><a id="741" class="Symbol">)</a> <a id="743" class="Symbol">(λ</a> <a id="746" href="graph-theory.cycles-undirected-graphs.html#746" class="Bound">H</a> <a id="748" class="Symbol">→</a> <a id="750" href="graph-theory.embeddings-undirected-graphs.html#1742" class="Function">emb-Undirected-Graph</a> <a id="771" class="Symbol">(</a><a id="772" href="graph-theory.polygons.html#3134" class="Function">undirected-graph-Polygon</a> <a id="797" href="graph-theory.cycles-undirected-graphs.html#600" class="Bound">k</a> <a id="799" href="graph-theory.cycles-undirected-graphs.html#746" class="Bound">H</a><a id="800" class="Symbol">)</a> <a id="802" href="graph-theory.cycles-undirected-graphs.html#608" class="Bound">G</a><a id="803" class="Symbol">)</a>
</pre>
