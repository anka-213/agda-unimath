---
title: Closed walks in undirected graphs
---

<pre class="Agda"><a id="59" class="Symbol">{-#</a> <a id="63" class="Keyword">OPTIONS</a> <a id="71" class="Pragma">--without-K</a> <a id="83" class="Pragma">--exact-split</a> <a id="97" class="Symbol">#-}</a>

<a id="102" class="Keyword">module</a> <a id="109" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a> <a id="153" class="Keyword">where</a>

<a id="160" class="Keyword">open</a> <a id="165" class="Keyword">import</a> <a id="172" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="214" class="Keyword">open</a> <a id="219" class="Keyword">import</a> <a id="226" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="258" class="Keyword">open</a> <a id="263" class="Keyword">import</a> <a id="270" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="298" class="Keyword">open</a> <a id="303" class="Keyword">import</a> <a id="310" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="351" class="Keyword">open</a> <a id="356" class="Keyword">import</a> <a id="363" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="385" class="Keyword">open</a> <a id="390" class="Keyword">import</a> <a id="397" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Idea

A closed walk of length `k : ℕ` in an undirected graph `G` is a morphism of graphs from a `k`-gon into `G`.

## Definition

<pre class="Agda"><a id="574" class="Keyword">module</a> <a id="581" href="graph-theory.closed-walks-undirected-graphs.html#581" class="Module">_</a>
  <a id="585" class="Symbol">{</a><a id="586" href="graph-theory.closed-walks-undirected-graphs.html#586" class="Bound">l1</a> <a id="589" href="graph-theory.closed-walks-undirected-graphs.html#589" class="Bound">l2</a> <a id="592" class="Symbol">:</a> <a id="594" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="599" class="Symbol">}</a> <a id="601" class="Symbol">(</a><a id="602" href="graph-theory.closed-walks-undirected-graphs.html#602" class="Bound">k</a> <a id="604" class="Symbol">:</a> <a id="606" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="607" class="Symbol">)</a> <a id="609" class="Symbol">(</a><a id="610" href="graph-theory.closed-walks-undirected-graphs.html#610" class="Bound">G</a> <a id="612" class="Symbol">:</a> <a id="614" href="graph-theory.undirected-graphs.html#1059" class="Function">Undirected-Graph</a> <a id="631" href="graph-theory.closed-walks-undirected-graphs.html#586" class="Bound">l1</a> <a id="634" href="graph-theory.closed-walks-undirected-graphs.html#589" class="Bound">l2</a><a id="636" class="Symbol">)</a>
  <a id="640" class="Keyword">where</a>
  
  <a id="651" href="graph-theory.closed-walks-undirected-graphs.html#651" class="Function">closed-walk-Undirected-Graph</a> <a id="680" class="Symbol">:</a> <a id="682" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="685" class="Symbol">(</a><a id="686" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="691" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="697" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="699" href="graph-theory.closed-walks-undirected-graphs.html#586" class="Bound">l1</a> <a id="702" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="704" href="graph-theory.closed-walks-undirected-graphs.html#589" class="Bound">l2</a><a id="706" class="Symbol">)</a>
  <a id="710" href="graph-theory.closed-walks-undirected-graphs.html#651" class="Function">closed-walk-Undirected-Graph</a> <a id="739" class="Symbol">=</a>
    <a id="745" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="747" class="Symbol">(</a><a id="748" href="graph-theory.polygons.html#2934" class="Function">Polygon</a> <a id="756" href="graph-theory.closed-walks-undirected-graphs.html#602" class="Bound">k</a><a id="757" class="Symbol">)</a> <a id="759" class="Symbol">(λ</a> <a id="762" href="graph-theory.closed-walks-undirected-graphs.html#762" class="Bound">H</a> <a id="764" class="Symbol">→</a> <a id="766" href="graph-theory.morphisms-undirected-graphs.html#1538" class="Function">hom-Undirected-Graph</a> <a id="787" class="Symbol">(</a><a id="788" href="graph-theory.polygons.html#3134" class="Function">undirected-graph-Polygon</a> <a id="813" href="graph-theory.closed-walks-undirected-graphs.html#602" class="Bound">k</a> <a id="815" href="graph-theory.closed-walks-undirected-graphs.html#762" class="Bound">H</a><a id="816" class="Symbol">)</a> <a id="818" href="graph-theory.closed-walks-undirected-graphs.html#610" class="Bound">G</a><a id="819" class="Symbol">)</a>
</pre>