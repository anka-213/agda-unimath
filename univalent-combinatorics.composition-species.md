---
title: Composition of species
---

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a> <a id="142" class="Keyword">where</a>

<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="196" class="Keyword">open</a> <a id="201" class="Keyword">import</a> <a id="208" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="238" class="Keyword">open</a> <a id="243" class="Keyword">import</a> <a id="250" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="282" class="Keyword">open</a> <a id="287" class="Keyword">import</a> <a id="294" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="318" class="Keyword">open</a> <a id="323" class="Keyword">import</a> <a id="330" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="358" class="Keyword">open</a> <a id="363" class="Keyword">import</a> <a id="370" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="421" class="Keyword">open</a> <a id="426" class="Keyword">import</a> <a id="433" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="470" class="Keyword">open</a> <a id="475" class="Keyword">import</a> <a id="482" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
</pre>
## Idea

A species `S : 𝔽 → UU l` can be thought of as the analytic endofunctor

```md
  X ↦ Σ (A : 𝔽) (S A) × (A → X)
```

Using the formula for composition of analytic endofunctors, we obtain a way to compose species.

## Definition

### Analytic composition of species

<pre class="Agda"><a id="analytic-comp-species"></a><a id="800" href="univalent-combinatorics.composition-species.html#800" class="Function">analytic-comp-species</a> <a id="822" class="Symbol">:</a>
  <a id="826" class="Symbol">{</a><a id="827" href="univalent-combinatorics.composition-species.html#827" class="Bound">l1</a> <a id="830" href="univalent-combinatorics.composition-species.html#830" class="Bound">l2</a> <a id="833" class="Symbol">:</a> <a id="835" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="840" class="Symbol">}</a> <a id="842" class="Symbol">→</a> <a id="844" href="univalent-combinatorics.species.html#273" class="Function">species</a> <a id="852" href="univalent-combinatorics.composition-species.html#827" class="Bound">l1</a> <a id="855" class="Symbol">→</a> <a id="857" href="univalent-combinatorics.species.html#273" class="Function">species</a> <a id="865" href="univalent-combinatorics.composition-species.html#830" class="Bound">l2</a> <a id="868" class="Symbol">→</a> <a id="870" href="univalent-combinatorics.species.html#273" class="Function">species</a> <a id="878" class="Symbol">(</a><a id="879" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="884" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="890" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="892" href="univalent-combinatorics.composition-species.html#827" class="Bound">l1</a> <a id="895" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="897" href="univalent-combinatorics.composition-species.html#830" class="Bound">l2</a><a id="899" class="Symbol">)</a>
<a id="901" href="univalent-combinatorics.composition-species.html#800" class="Function">analytic-comp-species</a> <a id="923" href="univalent-combinatorics.composition-species.html#923" class="Bound">S</a> <a id="925" href="univalent-combinatorics.composition-species.html#925" class="Bound">T</a> <a id="927" href="univalent-combinatorics.composition-species.html#927" class="Bound">X</a> <a id="929" class="Symbol">=</a>
  <a id="933" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="935" class="Symbol">(</a> <a id="937" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a><a id="938" class="Symbol">)</a>
    <a id="944" class="Symbol">(</a> <a id="946" class="Symbol">λ</a> <a id="948" href="univalent-combinatorics.composition-species.html#948" class="Bound">Y</a> <a id="950" class="Symbol">→</a>
      <a id="958" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="960" class="Symbol">(</a> <a id="962" href="univalent-combinatorics.finite-types.html#4503" class="Function">type-𝔽</a> <a id="969" href="univalent-combinatorics.composition-species.html#948" class="Bound">Y</a> <a id="971" class="Symbol">→</a> <a id="973" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a><a id="974" class="Symbol">)</a>
        <a id="984" class="Symbol">(</a> <a id="986" class="Symbol">λ</a> <a id="988" href="univalent-combinatorics.composition-species.html#988" class="Bound">Z</a> <a id="990" class="Symbol">→</a>
          <a id="1002" class="Symbol">(</a> <a id="1004" class="Symbol">(</a><a id="1005" href="univalent-combinatorics.finite-types.html#4503" class="Function">type-𝔽</a> <a id="1012" class="Symbol">(</a><a id="1013" href="univalent-combinatorics.dependent-sum-finite-types.html#2962" class="Function">Σ-𝔽</a> <a id="1017" href="univalent-combinatorics.composition-species.html#948" class="Bound">Y</a> <a id="1019" href="univalent-combinatorics.composition-species.html#988" class="Bound">Z</a><a id="1020" class="Symbol">)</a> <a id="1022" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="1024" href="univalent-combinatorics.finite-types.html#4503" class="Function">type-𝔽</a> <a id="1031" href="univalent-combinatorics.composition-species.html#927" class="Bound">X</a><a id="1032" class="Symbol">))</a> <a id="1035" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a>
          <a id="1047" class="Symbol">(</a> <a id="1049" href="univalent-combinatorics.composition-species.html#925" class="Bound">T</a> <a id="1051" href="univalent-combinatorics.composition-species.html#948" class="Bound">Y</a> <a id="1053" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1055" class="Symbol">((</a><a id="1057" href="univalent-combinatorics.composition-species.html#1057" class="Bound">y</a> <a id="1059" class="Symbol">:</a> <a id="1061" href="univalent-combinatorics.finite-types.html#4503" class="Function">type-𝔽</a> <a id="1068" href="univalent-combinatorics.composition-species.html#948" class="Bound">Y</a><a id="1069" class="Symbol">)</a> <a id="1071" class="Symbol">→</a> <a id="1073" href="univalent-combinatorics.composition-species.html#923" class="Bound">S</a> <a id="1075" class="Symbol">(</a><a id="1076" href="univalent-combinatorics.composition-species.html#988" class="Bound">Z</a> <a id="1078" href="univalent-combinatorics.composition-species.html#1057" class="Bound">y</a><a id="1079" class="Symbol">)))))</a>
</pre>
### The analytic unit for composition of species

<pre class="Agda"><a id="analytic-unit-species"></a><a id="1148" href="univalent-combinatorics.composition-species.html#1148" class="Function">analytic-unit-species</a> <a id="1170" class="Symbol">:</a> <a id="1172" class="Symbol">(</a><a id="1173" href="univalent-combinatorics.composition-species.html#1173" class="Bound">l</a> <a id="1175" class="Symbol">:</a> <a id="1177" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1182" class="Symbol">)</a> <a id="1184" class="Symbol">→</a> <a id="1186" href="univalent-combinatorics.species.html#273" class="Function">species</a> <a id="1194" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="1200" href="univalent-combinatorics.composition-species.html#1148" class="Function">analytic-unit-species</a> <a id="1222" href="univalent-combinatorics.composition-species.html#1222" class="Bound">l</a> <a id="1224" href="univalent-combinatorics.composition-species.html#1224" class="Bound">X</a> <a id="1226" class="Symbol">=</a> <a id="1228" href="foundation-core.contractible-types.html#992" class="Function">is-contr</a> <a id="1237" class="Symbol">(</a><a id="1238" href="univalent-combinatorics.finite-types.html#4503" class="Function">type-𝔽</a> <a id="1245" href="univalent-combinatorics.composition-species.html#1224" class="Bound">X</a><a id="1246" class="Symbol">)</a>
</pre>