---
title: Quotients of finite types
---

<pre class="Agda"><a id="51" class="Symbol">{-#</a> <a id="55" class="Keyword">OPTIONS</a> <a id="63" class="Pragma">--without-K</a> <a id="75" class="Pragma">--exact-split</a> <a id="89" class="Pragma">--allow-unsolved-metas</a> <a id="112" class="Symbol">#-}</a>

<a id="117" class="Keyword">module</a> <a id="124" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a> <a id="171" class="Keyword">where</a>

<a id="178" class="Keyword">open</a> <a id="183" class="Keyword">import</a> <a id="190" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="224" class="Keyword">open</a> <a id="229" class="Keyword">import</a> <a id="236" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="267" class="Keyword">open</a> <a id="272" class="Keyword">import</a> <a id="279" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="307" class="Keyword">open</a> <a id="312" class="Keyword">import</a> <a id="319" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="375" class="Keyword">open</a> <a id="380" class="Keyword">import</a> <a id="387" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="426" class="Keyword">open</a> <a id="431" class="Keyword">import</a> <a id="438" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="484" class="Keyword">open</a> <a id="489" class="Keyword">import</a> <a id="496" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="534" class="Keyword">open</a> <a id="539" class="Keyword">import</a> <a id="546" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Idea

The quotient of a finite type by a decidable equivalence relation is again a finite type. In this file we set up some infrastructure for such quotients.

## Definition

<pre class="Agda"><a id="774" class="Keyword">module</a> <a id="781" href="univalent-combinatorics.quotients-finite-types.html#781" class="Module">_</a>
  <a id="785" class="Symbol">(</a><a id="786" href="univalent-combinatorics.quotients-finite-types.html#786" class="Bound">X</a> <a id="788" class="Symbol">:</a> <a id="790" href="univalent-combinatorics.finite-types.html#4877" class="Function">𝔽</a><a id="791" class="Symbol">)</a> <a id="793" class="Symbol">(</a><a id="794" href="univalent-combinatorics.quotients-finite-types.html#794" class="Bound">R</a> <a id="796" class="Symbol">:</a> <a id="798" href="univalent-combinatorics.decidable-equivalence-relations.html#663" class="Function">Decidable-Equivalence-Relation-𝔽</a> <a id="831" href="univalent-combinatorics.quotients-finite-types.html#786" class="Bound">X</a><a id="832" class="Symbol">)</a>
  <a id="836" class="Keyword">where</a>

  <a id="845" href="univalent-combinatorics.quotients-finite-types.html#845" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a> <a id="896" class="Symbol">:</a> <a id="898" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="901" class="Symbol">(</a><a id="902" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="907" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="912" class="Symbol">)</a>
  <a id="916" href="univalent-combinatorics.quotients-finite-types.html#845" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a> <a id="967" class="Symbol">=</a>
    <a id="973" href="foundation.equivalence-classes.html#2698" class="Function">equivalence-class</a>
      <a id="997" class="Symbol">(</a> <a id="999" href="univalent-combinatorics.decidable-equivalence-relations.html#2144" class="Function">equivalence-relation-Decidable-Equivalence-Relation-𝔽</a> <a id="1053" href="univalent-combinatorics.quotients-finite-types.html#786" class="Bound">X</a> <a id="1055" href="univalent-combinatorics.quotients-finite-types.html#794" class="Bound">R</a><a id="1056" class="Symbol">)</a>

  <a id="1061" href="univalent-combinatorics.quotients-finite-types.html#1061" class="Function">is-finite-equivalence-class-Decidable-Equivalence-Relation-𝔽&#39;</a> <a id="1123" class="Symbol">:</a>
    <a id="1129" href="univalent-combinatorics.finite-types.html#4138" class="Function">is-finite</a> <a id="1139" href="univalent-combinatorics.quotients-finite-types.html#845" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a>
  <a id="1192" href="univalent-combinatorics.quotients-finite-types.html#1061" class="Function">is-finite-equivalence-class-Decidable-Equivalence-Relation-𝔽&#39;</a> <a id="1254" class="Symbol">=</a>
    <a id="1260" href="univalent-combinatorics.image-of-maps.html#1501" class="Function">is-finite-im</a>
      <a id="1279" class="Symbol">(</a> <a id="1281" href="univalent-combinatorics.finite-types.html#4961" class="Function">is-finite-type-𝔽</a> <a id="1298" href="univalent-combinatorics.quotients-finite-types.html#786" class="Bound">X</a><a id="1299" class="Symbol">)</a>
      <a id="1307" class="Symbol">(</a> <a id="1309" href="univalent-combinatorics.equality-finite-types.html#1723" class="Function">has-decidable-equality-is-finite</a>
        <a id="1350" class="Symbol">(</a> <a id="1352" class="Hole">{!is-finite-decidable-subtype!}</a><a id="1383" class="Symbol">))</a>

  <a id="1389" href="univalent-combinatorics.quotients-finite-types.html#1389" class="Function">quotient-𝔽</a> <a id="1400" class="Symbol">:</a> <a id="1402" href="univalent-combinatorics.finite-types.html#4877" class="Function">𝔽</a>
  <a id="1406" href="univalent-combinatorics.quotients-finite-types.html#1389" class="Function">quotient-𝔽</a> <a id="1417" class="Symbol">=</a> <a id="1419" class="Hole">{!!}</a>
</pre>