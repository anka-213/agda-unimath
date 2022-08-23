---
title: Undirected graph structures on standard finite sets
---

<pre class="Agda"><a id="77" class="Symbol">{-#</a> <a id="81" class="Keyword">OPTIONS</a> <a id="89" class="Pragma">--without-K</a> <a id="101" class="Pragma">--exact-split</a> <a id="115" class="Symbol">#-}</a>

<a id="120" class="Keyword">module</a> <a id="127" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a> <a id="192" class="Keyword">where</a>

<a id="199" class="Keyword">open</a> <a id="204" class="Keyword">import</a> <a id="211" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="253" class="Keyword">open</a> <a id="258" class="Keyword">import</a> <a id="265" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="297" class="Keyword">open</a> <a id="302" class="Keyword">import</a> <a id="309" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="336" class="Keyword">open</a> <a id="341" class="Keyword">import</a> <a id="348" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>

<a id="376" class="Keyword">open</a> <a id="381" class="Keyword">import</a> <a id="388" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Definition

<pre class="Agda"><a id="Undirected-Graph-Fin"></a><a id="462" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html#462" class="Function">Undirected-Graph-Fin</a> <a id="483" class="Symbol">:</a> <a id="485" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="488" class="Symbol">(</a><a id="489" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="494" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="499" class="Symbol">)</a>
<a id="501" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html#462" class="Function">Undirected-Graph-Fin</a> <a id="522" class="Symbol">=</a> <a id="524" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="526" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="528" class="Symbol">(λ</a> <a id="531" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html#531" class="Bound">V</a> <a id="533" class="Symbol">→</a> <a id="535" href="foundation.unordered-pairs.html#2489" class="Function">unordered-pair</a> <a id="550" class="Symbol">(</a><a id="551" href="univalent-combinatorics.standard-finite-types.html#2392" class="Function">Fin</a> <a id="555" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html#531" class="Bound">V</a><a id="556" class="Symbol">)</a> <a id="558" class="Symbol">→</a> <a id="560" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="561" class="Symbol">)</a>
</pre>
