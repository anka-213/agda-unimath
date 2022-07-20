---
title: Cartesian products of species
---

<pre class="Agda"><a id="55" class="Symbol">{-#</a> <a id="59" class="Keyword">OPTIONS</a> <a id="67" class="Pragma">--without-K</a> <a id="79" class="Pragma">--exact-split</a> <a id="93" class="Symbol">#-}</a>

<a id="98" class="Keyword">module</a> <a id="105" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a> <a id="156" class="Keyword">where</a>

<a id="163" class="Keyword">open</a> <a id="168" class="Keyword">import</a> <a id="175" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="210" class="Keyword">open</a> <a id="215" class="Keyword">import</a> <a id="222" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="246" class="Keyword">open</a> <a id="251" class="Keyword">import</a> <a id="258" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="308" class="Keyword">open</a> <a id="313" class="Keyword">import</a> <a id="320" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="371" class="Keyword">open</a> <a id="376" class="Keyword">import</a> <a id="383" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="411" class="Keyword">open</a> <a id="416" class="Keyword">import</a> <a id="423" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="455" class="Keyword">open</a> <a id="460" class="Keyword">import</a> <a id="467" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="504" class="Keyword">open</a> <a id="509" class="Keyword">import</a> <a id="516" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="558" class="Keyword">open</a> <a id="563" class="Keyword">import</a> <a id="570" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="615" class="Keyword">open</a> <a id="620" class="Keyword">import</a> <a id="627" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
</pre>
## Idea

The cartesian product of two species `F` and `G` is their pointwise cartesian product.

## Definition

<pre class="Agda"><a id="prod-species"></a><a id="794" href="univalent-combinatorics.cartesian-products-species.html#794" class="Function">prod-species</a> <a id="807" class="Symbol">:</a>
  <a id="811" class="Symbol">{</a><a id="812" href="univalent-combinatorics.cartesian-products-species.html#812" class="Bound">l1</a> <a id="815" href="univalent-combinatorics.cartesian-products-species.html#815" class="Bound">l2</a> <a id="818" class="Symbol">:</a> <a id="820" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="825" class="Symbol">}</a> <a id="827" class="Symbol">(</a><a id="828" href="univalent-combinatorics.cartesian-products-species.html#828" class="Bound">F</a> <a id="830" class="Symbol">:</a> <a id="832" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="840" href="univalent-combinatorics.cartesian-products-species.html#812" class="Bound">l1</a><a id="842" class="Symbol">)</a> <a id="844" class="Symbol">(</a><a id="845" href="univalent-combinatorics.cartesian-products-species.html#845" class="Bound">G</a> <a id="847" class="Symbol">:</a> <a id="849" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="857" href="univalent-combinatorics.cartesian-products-species.html#815" class="Bound">l2</a><a id="859" class="Symbol">)</a> <a id="861" class="Symbol">(</a><a id="862" href="univalent-combinatorics.cartesian-products-species.html#862" class="Bound">X</a> <a id="864" class="Symbol">:</a> <a id="866" href="univalent-combinatorics.finite-types.html#4873" class="Function">𝔽</a><a id="867" class="Symbol">)</a> <a id="869" class="Symbol">→</a> <a id="871" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="874" class="Symbol">(</a><a id="875" href="univalent-combinatorics.cartesian-products-species.html#812" class="Bound">l1</a> <a id="878" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="880" href="univalent-combinatorics.cartesian-products-species.html#815" class="Bound">l2</a><a id="882" class="Symbol">)</a>
<a id="884" href="univalent-combinatorics.cartesian-products-species.html#794" class="Function">prod-species</a> <a id="897" href="univalent-combinatorics.cartesian-products-species.html#897" class="Bound">F</a> <a id="899" href="univalent-combinatorics.cartesian-products-species.html#899" class="Bound">G</a> <a id="901" href="univalent-combinatorics.cartesian-products-species.html#901" class="Bound">X</a> <a id="903" class="Symbol">=</a> <a id="905" class="Symbol">(</a><a id="906" href="univalent-combinatorics.cartesian-products-species.html#897" class="Bound">F</a> <a id="908" href="univalent-combinatorics.cartesian-products-species.html#901" class="Bound">X</a><a id="909" class="Symbol">)</a> <a id="911" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a> <a id="913" class="Symbol">(</a><a id="914" href="univalent-combinatorics.cartesian-products-species.html#899" class="Bound">G</a> <a id="916" href="univalent-combinatorics.cartesian-products-species.html#901" class="Bound">X</a><a id="917" class="Symbol">)</a>
</pre>
## Properties

### The adjunction between cartesian products and exponents of species

<pre class="Agda"><a id="equiv-universal-property-exponents-species"></a><a id="1020" href="univalent-combinatorics.cartesian-products-species.html#1020" class="Function">equiv-universal-property-exponents-species</a> <a id="1063" class="Symbol">:</a>
  <a id="1067" class="Symbol">{</a><a id="1068" href="univalent-combinatorics.cartesian-products-species.html#1068" class="Bound">l1</a> <a id="1071" href="univalent-combinatorics.cartesian-products-species.html#1071" class="Bound">l2</a> <a id="1074" href="univalent-combinatorics.cartesian-products-species.html#1074" class="Bound">l3</a> <a id="1077" class="Symbol">:</a> <a id="1079" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1084" class="Symbol">}</a> <a id="1086" class="Symbol">(</a><a id="1087" href="univalent-combinatorics.cartesian-products-species.html#1087" class="Bound">F</a> <a id="1089" class="Symbol">:</a> <a id="1091" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1099" href="univalent-combinatorics.cartesian-products-species.html#1068" class="Bound">l1</a><a id="1101" class="Symbol">)</a> <a id="1103" class="Symbol">(</a><a id="1104" href="univalent-combinatorics.cartesian-products-species.html#1104" class="Bound">G</a> <a id="1106" class="Symbol">:</a> <a id="1108" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1116" href="univalent-combinatorics.cartesian-products-species.html#1071" class="Bound">l2</a><a id="1118" class="Symbol">)</a> <a id="1120" class="Symbol">(</a><a id="1121" href="univalent-combinatorics.cartesian-products-species.html#1121" class="Bound">H</a> <a id="1123" class="Symbol">:</a> <a id="1125" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1133" href="univalent-combinatorics.cartesian-products-species.html#1074" class="Bound">l3</a><a id="1135" class="Symbol">)</a> <a id="1137" class="Symbol">→</a>
  <a id="1141" href="univalent-combinatorics.morphisms-species.html#833" class="Function">hom-species</a> <a id="1153" class="Symbol">(</a><a id="1154" href="univalent-combinatorics.cartesian-products-species.html#794" class="Function">prod-species</a> <a id="1167" href="univalent-combinatorics.cartesian-products-species.html#1087" class="Bound">F</a> <a id="1169" href="univalent-combinatorics.cartesian-products-species.html#1104" class="Bound">G</a><a id="1170" class="Symbol">)</a> <a id="1172" href="univalent-combinatorics.cartesian-products-species.html#1121" class="Bound">H</a> <a id="1174" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="1176" href="univalent-combinatorics.morphisms-species.html#833" class="Function">hom-species</a> <a id="1188" href="univalent-combinatorics.cartesian-products-species.html#1087" class="Bound">F</a> <a id="1190" class="Symbol">(</a><a id="1191" href="univalent-combinatorics.exponents-species.html#682" class="Function">function-species</a> <a id="1208" href="univalent-combinatorics.cartesian-products-species.html#1104" class="Bound">G</a> <a id="1210" href="univalent-combinatorics.cartesian-products-species.html#1121" class="Bound">H</a><a id="1211" class="Symbol">)</a>
<a id="1213" href="univalent-combinatorics.cartesian-products-species.html#1020" class="Function">equiv-universal-property-exponents-species</a> <a id="1256" href="univalent-combinatorics.cartesian-products-species.html#1256" class="Bound">F</a> <a id="1258" href="univalent-combinatorics.cartesian-products-species.html#1258" class="Bound">G</a> <a id="1260" href="univalent-combinatorics.cartesian-products-species.html#1260" class="Bound">H</a> <a id="1262" class="Symbol">=</a>
  <a id="1266" href="foundation-core.functoriality-dependent-function-types.html#2227" class="Function">equiv-map-Π</a> <a id="1278" class="Symbol">(λ</a> <a id="1281" href="univalent-combinatorics.cartesian-products-species.html#1281" class="Bound">X</a> <a id="1283" class="Symbol">→</a> <a id="1285" href="foundation.universal-property-dependent-pair-types.html#1013" class="Function">equiv-ev-pair</a><a id="1298" class="Symbol">)</a>
</pre>