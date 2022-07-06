---
title: Quotients of finite types
---

<pre class="Agda"><a id="51" class="Symbol">{-#</a> <a id="55" class="Keyword">OPTIONS</a> <a id="63" class="Pragma">--without-K</a> <a id="75" class="Pragma">--exact-split</a> <a id="89" class="Pragma">--allow-unsolved-metas</a> <a id="112" class="Symbol">#-}</a>

<a id="117" class="Keyword">module</a> <a id="124" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a> <a id="171" class="Keyword">where</a>

<a id="178" class="Keyword">open</a> <a id="183" class="Keyword">import</a> <a id="190" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="221" class="Keyword">open</a> <a id="226" class="Keyword">import</a> <a id="233" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="261" class="Keyword">open</a> <a id="266" class="Keyword">import</a> <a id="273" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="329" class="Keyword">open</a> <a id="334" class="Keyword">import</a> <a id="341" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="379" class="Keyword">open</a> <a id="384" class="Keyword">import</a> <a id="391" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Idea

The quotient of a finite type by a decidable equivalence relation is again a finite type. In this file we set up some infrastructure for such quotients.

## Definition

<pre class="Agda"><a id="619" class="Keyword">module</a> <a id="626" href="univalent-combinatorics.quotients-finite-types.html#626" class="Module">_</a>
  <a id="630" class="Symbol">(</a><a id="631" href="univalent-combinatorics.quotients-finite-types.html#631" class="Bound">X</a> <a id="633" class="Symbol">:</a> <a id="635" href="univalent-combinatorics.finite-types.html#4635" class="Function">𝔽</a><a id="636" class="Symbol">)</a> <a id="638" class="Symbol">(</a><a id="639" href="univalent-combinatorics.quotients-finite-types.html#639" class="Bound">R</a> <a id="641" class="Symbol">:</a> <a id="643" href="univalent-combinatorics.decidable-equivalence-relations.html#663" class="Function">Decidable-Equivalence-Relation-𝔽</a> <a id="676" href="univalent-combinatorics.quotients-finite-types.html#631" class="Bound">X</a><a id="677" class="Symbol">)</a>
  <a id="681" class="Keyword">where</a>

  <a id="690" href="univalent-combinatorics.quotients-finite-types.html#690" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a> <a id="741" class="Symbol">:</a> <a id="743" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="746" class="Symbol">(</a><a id="747" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="752" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="757" class="Symbol">)</a>
  <a id="761" href="univalent-combinatorics.quotients-finite-types.html#690" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a> <a id="812" class="Symbol">=</a>
    <a id="818" href="foundation.equivalence-classes.html#2706" class="Function">equivalence-class</a>
      <a id="842" class="Symbol">(</a> <a id="844" href="univalent-combinatorics.decidable-equivalence-relations.html#2144" class="Function">equivalence-relation-Decidable-Equivalence-Relation-𝔽</a> <a id="898" href="univalent-combinatorics.quotients-finite-types.html#631" class="Bound">X</a> <a id="900" href="univalent-combinatorics.quotients-finite-types.html#639" class="Bound">R</a><a id="901" class="Symbol">)</a>

  <a id="906" href="univalent-combinatorics.quotients-finite-types.html#906" class="Function">is-finite-equivalence-class-Decidable-Equivalence-Relation-𝔽&#39;</a> <a id="968" class="Symbol">:</a>
    <a id="974" href="univalent-combinatorics.finite-types.html#4244" class="Function">is-finite</a> <a id="984" href="univalent-combinatorics.quotients-finite-types.html#690" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a>
  <a id="1037" href="univalent-combinatorics.quotients-finite-types.html#906" class="Function">is-finite-equivalence-class-Decidable-Equivalence-Relation-𝔽&#39;</a> <a id="1099" class="Symbol">=</a>
    <a id="1105" href="univalent-combinatorics.image-of-maps.html#1501" class="Function">is-finite-im</a>
      <a id="1124" class="Symbol">(</a> <a id="1126" href="univalent-combinatorics.finite-types.html#4734" class="Function">is-finite-type-𝔽</a> <a id="1143" href="univalent-combinatorics.quotients-finite-types.html#631" class="Bound">X</a><a id="1144" class="Symbol">)</a>
      <a id="1152" class="Hole">{!!}</a>

  <a id="1160" href="univalent-combinatorics.quotients-finite-types.html#1160" class="Function">quotient-𝔽</a> <a id="1171" class="Symbol">:</a> <a id="1173" href="univalent-combinatorics.finite-types.html#4635" class="Function">𝔽</a>
  <a id="1177" href="univalent-combinatorics.quotients-finite-types.html#1160" class="Function">quotient-𝔽</a> <a id="1188" class="Symbol">=</a> <a id="1190" class="Hole">{!!}</a>
</pre>