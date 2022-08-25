---
title: Composition of species
---

<pre class="Agda"><a id="48" class="Keyword">module</a> <a id="55" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a> <a id="99" class="Keyword">where</a>

<a id="106" class="Keyword">open</a> <a id="111" class="Keyword">import</a> <a id="118" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="153" class="Keyword">open</a> <a id="158" class="Keyword">import</a> <a id="165" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="195" class="Keyword">open</a> <a id="200" class="Keyword">import</a> <a id="207" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="239" class="Keyword">open</a> <a id="244" class="Keyword">import</a> <a id="251" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="275" class="Keyword">open</a> <a id="280" class="Keyword">import</a> <a id="287" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="313" class="Keyword">open</a> <a id="318" class="Keyword">import</a> <a id="325" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="362" class="Keyword">open</a> <a id="367" class="Keyword">import</a> <a id="374" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="402" class="Keyword">open</a> <a id="407" class="Keyword">import</a> <a id="414" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="465" class="Keyword">open</a> <a id="470" class="Keyword">import</a> <a id="477" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="522" class="Keyword">open</a> <a id="527" class="Keyword">import</a> <a id="534" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="571" class="Keyword">open</a> <a id="576" class="Keyword">import</a> <a id="583" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="618" class="Keyword">open</a> <a id="623" class="Keyword">import</a> <a id="630" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
</pre>
## Idea

A species `S : 𝔽 → UU l` can be thought of as the analytic endofunctor

```md
  X ↦ Σ (A : 𝔽) (S A) × (A → X)
```

Using the formula for composition of analytic endofunctors, we obtain a way to compose species.

## Definition

### Analytic composition of species

<pre class="Agda"><a id="analytic-comp-species"></a><a id="948" href="univalent-combinatorics.composition-species.html#948" class="Function">analytic-comp-species</a> <a id="970" class="Symbol">:</a>
  <a id="974" class="Symbol">{</a><a id="975" href="univalent-combinatorics.composition-species.html#975" class="Bound">l1</a> <a id="978" href="univalent-combinatorics.composition-species.html#978" class="Bound">l2</a> <a id="981" href="univalent-combinatorics.composition-species.html#981" class="Bound">l3</a> <a id="984" class="Symbol">:</a> <a id="986" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="991" class="Symbol">}</a> <a id="993" class="Symbol">→</a> <a id="995" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1003" href="univalent-combinatorics.composition-species.html#975" class="Bound">l1</a> <a id="1006" href="univalent-combinatorics.composition-species.html#978" class="Bound">l2</a> <a id="1009" class="Symbol">→</a> <a id="1011" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1019" href="univalent-combinatorics.composition-species.html#975" class="Bound">l1</a> <a id="1022" href="univalent-combinatorics.composition-species.html#981" class="Bound">l3</a> <a id="1025" class="Symbol">→</a>
  <a id="1029" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1037" href="univalent-combinatorics.composition-species.html#975" class="Bound">l1</a> <a id="1040" class="Symbol">(</a><a id="1041" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1046" href="univalent-combinatorics.composition-species.html#975" class="Bound">l1</a> <a id="1049" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1051" href="univalent-combinatorics.composition-species.html#978" class="Bound">l2</a> <a id="1054" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1056" href="univalent-combinatorics.composition-species.html#981" class="Bound">l3</a><a id="1058" class="Symbol">)</a>
<a id="1060" href="univalent-combinatorics.composition-species.html#948" class="Function">analytic-comp-species</a> <a id="1082" class="Symbol">{</a><a id="1083" href="univalent-combinatorics.composition-species.html#1083" class="Bound">l1</a><a id="1085" class="Symbol">}</a> <a id="1087" class="Symbol">{</a><a id="1088" href="univalent-combinatorics.composition-species.html#1088" class="Bound">l2</a><a id="1090" class="Symbol">}</a> <a id="1092" class="Symbol">{</a><a id="1093" href="univalent-combinatorics.composition-species.html#1093" class="Bound">l3</a><a id="1095" class="Symbol">}</a> <a id="1097" href="univalent-combinatorics.composition-species.html#1097" class="Bound">S</a> <a id="1099" href="univalent-combinatorics.composition-species.html#1099" class="Bound">T</a> <a id="1101" href="univalent-combinatorics.composition-species.html#1101" class="Bound">X</a> <a id="1103" class="Symbol">=</a>
  <a id="1107" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1109" class="Symbol">(</a> <a id="1111" href="univalent-combinatorics.partitions.html#1956" class="Function">partition-𝔽</a> <a id="1123" href="univalent-combinatorics.composition-species.html#1083" class="Bound">l1</a> <a id="1126" href="univalent-combinatorics.composition-species.html#1083" class="Bound">l1</a> <a id="1129" href="univalent-combinatorics.composition-species.html#1101" class="Bound">X</a><a id="1130" class="Symbol">)</a>
    <a id="1136" class="Symbol">(</a> <a id="1138" class="Symbol">λ</a> <a id="1140" href="univalent-combinatorics.composition-species.html#1140" class="Bound">P</a> <a id="1142" class="Symbol">→</a>
      <a id="1150" class="Symbol">(</a> <a id="1152" href="univalent-combinatorics.composition-species.html#1099" class="Bound">T</a> <a id="1154" class="Symbol">(</a><a id="1155" href="univalent-combinatorics.partitions.html#2302" class="Function">finite-indexing-type-partition-𝔽</a> <a id="1188" href="univalent-combinatorics.composition-species.html#1101" class="Bound">X</a> <a id="1190" href="univalent-combinatorics.composition-species.html#1140" class="Bound">P</a><a id="1191" class="Symbol">))</a> <a id="1194" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a>
      <a id="1202" class="Symbol">(</a> <a id="1204" class="Symbol">(</a><a id="1205" href="univalent-combinatorics.composition-species.html#1205" class="Bound">y</a> <a id="1207" class="Symbol">:</a> <a id="1209" href="univalent-combinatorics.partitions.html#2388" class="Function">indexing-type-partition-𝔽</a> <a id="1235" href="univalent-combinatorics.composition-species.html#1101" class="Bound">X</a> <a id="1237" href="univalent-combinatorics.composition-species.html#1140" class="Bound">P</a><a id="1238" class="Symbol">)</a> <a id="1240" class="Symbol">→</a>
        <a id="1250" href="univalent-combinatorics.composition-species.html#1097" class="Bound">S</a> <a id="1252" class="Symbol">(</a><a id="1253" href="univalent-combinatorics.partitions.html#2836" class="Function">finite-block-partition-𝔽</a> <a id="1278" href="univalent-combinatorics.composition-species.html#1101" class="Bound">X</a> <a id="1280" href="univalent-combinatorics.composition-species.html#1140" class="Bound">P</a> <a id="1282" href="univalent-combinatorics.composition-species.html#1205" class="Bound">y</a><a id="1283" class="Symbol">)))</a>
</pre>
### The analytic unit for composition of species

<pre class="Agda"><a id="analytic-unit-species"></a><a id="1350" href="univalent-combinatorics.composition-species.html#1350" class="Function">analytic-unit-species</a> <a id="1372" class="Symbol">:</a> <a id="1374" class="Symbol">{</a><a id="1375" href="univalent-combinatorics.composition-species.html#1375" class="Bound">l1</a> <a id="1378" class="Symbol">:</a> <a id="1380" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1385" class="Symbol">}</a> <a id="1387" class="Symbol">→</a> <a id="1389" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1397" href="univalent-combinatorics.composition-species.html#1375" class="Bound">l1</a> <a id="1400" href="univalent-combinatorics.composition-species.html#1375" class="Bound">l1</a>
<a id="1403" href="univalent-combinatorics.composition-species.html#1350" class="Function">analytic-unit-species</a> <a id="1425" href="univalent-combinatorics.composition-species.html#1425" class="Bound">X</a> <a id="1427" class="Symbol">=</a> <a id="1429" href="foundation-core.contractible-types.html#1006" class="Function">is-contr</a> <a id="1438" class="Symbol">(</a><a id="1439" href="univalent-combinatorics.finite-types.html#4606" class="Function">type-𝔽</a> <a id="1446" href="univalent-combinatorics.composition-species.html#1425" class="Bound">X</a><a id="1447" class="Symbol">)</a>
</pre>
## Properties

### Unit laws for analytic composition of species

<pre class="Agda"><a id="1528" class="Comment">{-
left-unit-law-comp-species :
  {l1 l2 : Level} (F : species l1 l2) →
  equiv-species (analytic-comp-species analytic-unit-species F) F
left-unit-law-comp-species F X =
  {!!}
-}</a>
</pre>