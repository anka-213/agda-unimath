---
title: Directed graph structures on standard finite sets
---

<pre class="Agda"><a id="75" class="Symbol">{-#</a> <a id="79" class="Keyword">OPTIONS</a> <a id="87" class="Pragma">--without-K</a> <a id="99" class="Pragma">--exact-split</a> <a id="113" class="Symbol">#-}</a>

<a id="118" class="Keyword">module</a> <a id="125" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a> <a id="188" class="Keyword">where</a>

<a id="195" class="Keyword">open</a> <a id="200" class="Keyword">import</a> <a id="207" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="249" class="Keyword">open</a> <a id="254" class="Keyword">import</a> <a id="261" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="293" class="Keyword">open</a> <a id="298" class="Keyword">import</a> <a id="305" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="333" class="Keyword">open</a> <a id="338" class="Keyword">import</a> <a id="345" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Definition

<pre class="Agda"><a id="Directed-Graph-Fin"></a><a id="419" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html#419" class="Function">Directed-Graph-Fin</a> <a id="438" class="Symbol">:</a> <a id="440" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="443" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="449" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html#419" class="Function">Directed-Graph-Fin</a> <a id="468" class="Symbol">=</a> <a id="470" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="472" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="474" class="Symbol">(λ</a> <a id="477" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html#477" class="Bound">V</a> <a id="479" class="Symbol">→</a> <a id="481" href="univalent-combinatorics.standard-finite-types.html#2392" class="Function">Fin</a> <a id="485" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html#477" class="Bound">V</a> <a id="487" class="Symbol">→</a> <a id="489" href="univalent-combinatorics.standard-finite-types.html#2392" class="Function">Fin</a> <a id="493" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html#477" class="Bound">V</a> <a id="495" class="Symbol">→</a> <a id="497" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="498" class="Symbol">)</a>
</pre>