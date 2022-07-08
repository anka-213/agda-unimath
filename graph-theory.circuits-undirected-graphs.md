---
title: Circuits in undirected graphs
---

<pre class="Agda"><a id="55" class="Symbol">{-#</a> <a id="59" class="Keyword">OPTIONS</a> <a id="67" class="Pragma">--without-K</a> <a id="79" class="Pragma">--exact-split</a> <a id="93" class="Symbol">#-}</a>

<a id="98" class="Keyword">module</a> <a id="105" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a> <a id="145" class="Keyword">where</a>

<a id="152" class="Keyword">open</a> <a id="157" class="Keyword">import</a> <a id="164" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="206" class="Keyword">open</a> <a id="211" class="Keyword">import</a> <a id="218" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="250" class="Keyword">open</a> <a id="255" class="Keyword">import</a> <a id="262" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="290" class="Keyword">open</a> <a id="295" class="Keyword">import</a> <a id="302" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="324" class="Keyword">open</a> <a id="329" class="Keyword">import</a> <a id="336" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="394" class="Keyword">open</a> <a id="399" class="Keyword">import</a> <a id="406" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Idea

A circuit in an undirected graph `G` consists of a `k`-gon `H` equipped with a totally faithful morphism of graphs from `H` to `G`. In other words, a circuit is a closed walk with no repeated edges.

## Definition

<pre class="Agda"><a id="674" class="Keyword">module</a> <a id="681" href="graph-theory.circuits-undirected-graphs.html#681" class="Module">_</a>
  <a id="685" class="Symbol">{</a><a id="686" href="graph-theory.circuits-undirected-graphs.html#686" class="Bound">l1</a> <a id="689" href="graph-theory.circuits-undirected-graphs.html#689" class="Bound">l2</a> <a id="692" class="Symbol">:</a> <a id="694" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="699" class="Symbol">}</a> <a id="701" class="Symbol">(</a><a id="702" href="graph-theory.circuits-undirected-graphs.html#702" class="Bound">k</a> <a id="704" class="Symbol">:</a> <a id="706" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a><a id="707" class="Symbol">)</a> <a id="709" class="Symbol">(</a><a id="710" href="graph-theory.circuits-undirected-graphs.html#710" class="Bound">G</a> <a id="712" class="Symbol">:</a> <a id="714" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="731" href="graph-theory.circuits-undirected-graphs.html#686" class="Bound">l1</a> <a id="734" href="graph-theory.circuits-undirected-graphs.html#689" class="Bound">l2</a><a id="736" class="Symbol">)</a>
  <a id="740" class="Keyword">where</a>

  <a id="749" href="graph-theory.circuits-undirected-graphs.html#749" class="Function">circuit-Undirected-Graph</a> <a id="774" class="Symbol">:</a> <a id="776" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="779" class="Symbol">(</a><a id="780" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="785" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="791" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="793" href="graph-theory.circuits-undirected-graphs.html#686" class="Bound">l1</a> <a id="796" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="798" href="graph-theory.circuits-undirected-graphs.html#689" class="Bound">l2</a><a id="800" class="Symbol">)</a>
  <a id="804" href="graph-theory.circuits-undirected-graphs.html#749" class="Function">circuit-Undirected-Graph</a> <a id="829" class="Symbol">=</a>
    <a id="835" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="837" class="Symbol">(</a> <a id="839" href="graph-theory.polygons.html#2934" class="Function">Polygon</a> <a id="847" href="graph-theory.circuits-undirected-graphs.html#702" class="Bound">k</a><a id="848" class="Symbol">)</a>
      <a id="856" class="Symbol">(</a> <a id="858" class="Symbol">λ</a> <a id="860" href="graph-theory.circuits-undirected-graphs.html#860" class="Bound">H</a> <a id="862" class="Symbol">→</a>
        <a id="872" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#991" class="Function">totally-faithful-hom-Undirected-Graph</a> <a id="910" class="Symbol">(</a><a id="911" href="graph-theory.polygons.html#3134" class="Function">undirected-graph-Polygon</a> <a id="936" href="graph-theory.circuits-undirected-graphs.html#702" class="Bound">k</a> <a id="938" href="graph-theory.circuits-undirected-graphs.html#860" class="Bound">H</a><a id="939" class="Symbol">)</a> <a id="941" href="graph-theory.circuits-undirected-graphs.html#710" class="Bound">G</a><a id="942" class="Symbol">)</a>
</pre>