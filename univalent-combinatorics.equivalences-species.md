---
title: Equivalences of species
---

<pre class="Agda"><a id="49" class="Symbol">{-#</a> <a id="53" class="Keyword">OPTIONS</a> <a id="61" class="Pragma">--without-K</a> <a id="73" class="Pragma">--exact-split</a> <a id="87" class="Symbol">#-}</a>

<a id="92" class="Keyword">module</a> <a id="99" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a> <a id="144" class="Keyword">where</a>

<a id="151" class="Keyword">open</a> <a id="156" class="Keyword">import</a> <a id="163" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="193" class="Keyword">open</a> <a id="198" class="Keyword">import</a> <a id="205" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="237" class="Keyword">open</a> <a id="242" class="Keyword">import</a> <a id="249" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="294" class="Keyword">open</a> <a id="299" class="Keyword">import</a> <a id="306" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="327" class="Keyword">open</a> <a id="332" class="Keyword">import</a> <a id="339" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="363" class="Keyword">open</a> <a id="368" class="Keyword">import</a> <a id="375" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="401" class="Keyword">open</a> <a id="406" class="Keyword">import</a> <a id="413" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="435" class="Keyword">open</a> <a id="440" class="Keyword">import</a> <a id="447" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="475" class="Keyword">open</a> <a id="480" class="Keyword">import</a> <a id="487" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="524" class="Keyword">open</a> <a id="529" class="Keyword">import</a> <a id="536" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>

</pre>
## Idea

An equivalence of species from `F` to `G` is a pointwise equivalence.

## Definition

<pre class="Agda"><a id="equiv-species"></a><a id="677" href="univalent-combinatorics.equivalences-species.html#677" class="Function">equiv-species</a> <a id="691" class="Symbol">:</a>
  <a id="695" class="Symbol">{</a><a id="696" href="univalent-combinatorics.equivalences-species.html#696" class="Bound">l1</a> <a id="699" href="univalent-combinatorics.equivalences-species.html#699" class="Bound">l2</a> <a id="702" class="Symbol">:</a> <a id="704" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="709" class="Symbol">}</a> <a id="711" class="Symbol">→</a> <a id="713" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="721" href="univalent-combinatorics.equivalences-species.html#696" class="Bound">l1</a> <a id="724" class="Symbol">→</a> <a id="726" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="734" href="univalent-combinatorics.equivalences-species.html#699" class="Bound">l2</a> <a id="737" class="Symbol">→</a> <a id="739" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="742" class="Symbol">(</a><a id="743" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="748" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="754" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="756" href="univalent-combinatorics.equivalences-species.html#696" class="Bound">l1</a> <a id="759" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="761" href="univalent-combinatorics.equivalences-species.html#699" class="Bound">l2</a><a id="763" class="Symbol">)</a>
<a id="765" href="univalent-combinatorics.equivalences-species.html#677" class="Function">equiv-species</a> <a id="779" href="univalent-combinatorics.equivalences-species.html#779" class="Bound">F</a> <a id="781" href="univalent-combinatorics.equivalences-species.html#781" class="Bound">G</a> <a id="783" class="Symbol">=</a> <a id="785" class="Symbol">(</a><a id="786" href="univalent-combinatorics.equivalences-species.html#786" class="Bound">X</a> <a id="788" class="Symbol">:</a> <a id="790" href="univalent-combinatorics.finite-types.html#4635" class="Function">𝔽</a><a id="791" class="Symbol">)</a> <a id="793" class="Symbol">→</a> <a id="795" href="univalent-combinatorics.equivalences-species.html#779" class="Bound">F</a> <a id="797" href="univalent-combinatorics.equivalences-species.html#786" class="Bound">X</a> <a id="799" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="801" href="univalent-combinatorics.equivalences-species.html#781" class="Bound">G</a> <a id="803" href="univalent-combinatorics.equivalences-species.html#786" class="Bound">X</a>
</pre>
## Properties

### The identity type of two species is equivalent to the type of equivalences between them

<pre class="Agda"><a id="extensionality-species"></a><a id="926" href="univalent-combinatorics.equivalences-species.html#926" class="Function">extensionality-species</a> <a id="949" class="Symbol">:</a>
  <a id="953" class="Symbol">{</a><a id="954" href="univalent-combinatorics.equivalences-species.html#954" class="Bound">l</a> <a id="956" class="Symbol">:</a> <a id="958" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="963" class="Symbol">}</a> <a id="965" class="Symbol">→</a> <a id="967" class="Symbol">(</a><a id="968" href="univalent-combinatorics.equivalences-species.html#968" class="Bound">F</a> <a id="970" href="univalent-combinatorics.equivalences-species.html#970" class="Bound">G</a> <a id="972" class="Symbol">:</a> <a id="974" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="982" href="univalent-combinatorics.equivalences-species.html#954" class="Bound">l</a><a id="983" class="Symbol">)</a> <a id="985" class="Symbol">→</a> <a id="987" class="Symbol">(</a><a id="988" href="foundation-core.identity-types.html#1767" class="Datatype">Id</a> <a id="991" href="univalent-combinatorics.equivalences-species.html#968" class="Bound">F</a> <a id="993" href="univalent-combinatorics.equivalences-species.html#970" class="Bound">G</a><a id="994" class="Symbol">)</a> <a id="996" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="998" class="Symbol">(</a><a id="999" href="univalent-combinatorics.equivalences-species.html#677" class="Function">equiv-species</a> <a id="1013" href="univalent-combinatorics.equivalences-species.html#968" class="Bound">F</a> <a id="1015" href="univalent-combinatorics.equivalences-species.html#970" class="Bound">G</a><a id="1016" class="Symbol">)</a>  
<a id="1020" href="univalent-combinatorics.equivalences-species.html#926" class="Function">extensionality-species</a> <a id="1043" class="Symbol">=</a> <a id="1045" href="foundation.univalence.html#2899" class="Function">extensionality-fam</a>
</pre> 