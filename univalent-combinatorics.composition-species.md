---
title: Composition of species
---

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Pragma">--allow-unsolved-metas</a> <a id="109" class="Symbol">#-}</a>

<a id="114" class="Keyword">module</a> <a id="121" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a> <a id="165" class="Keyword">where</a>

<a id="172" class="Keyword">open</a> <a id="177" class="Keyword">import</a> <a id="184" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="219" class="Keyword">open</a> <a id="224" class="Keyword">import</a> <a id="231" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="261" class="Keyword">open</a> <a id="266" class="Keyword">import</a> <a id="273" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="305" class="Keyword">open</a> <a id="310" class="Keyword">import</a> <a id="317" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="341" class="Keyword">open</a> <a id="346" class="Keyword">import</a> <a id="353" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="379" class="Keyword">open</a> <a id="384" class="Keyword">import</a> <a id="391" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="428" class="Keyword">open</a> <a id="433" class="Keyword">import</a> <a id="440" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="468" class="Keyword">open</a> <a id="473" class="Keyword">import</a> <a id="480" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="531" class="Keyword">open</a> <a id="536" class="Keyword">import</a> <a id="543" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="588" class="Keyword">open</a> <a id="593" class="Keyword">import</a> <a id="600" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="637" class="Keyword">open</a> <a id="642" class="Keyword">import</a> <a id="649" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="684" class="Keyword">open</a> <a id="689" class="Keyword">import</a> <a id="696" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
</pre>
## Idea

A species `S : 𝔽 → UU l` can be thought of as the analytic endofunctor

```md
  X ↦ Σ (A : 𝔽) (S A) × (A → X)
```

Using the formula for composition of analytic endofunctors, we obtain a way to compose species.

## Definition

### Analytic composition of species

<pre class="Agda"><a id="analytic-comp-species"></a><a id="1014" href="univalent-combinatorics.composition-species.html#1014" class="Function">analytic-comp-species</a> <a id="1036" class="Symbol">:</a>
  <a id="1040" class="Symbol">{</a><a id="1041" href="univalent-combinatorics.composition-species.html#1041" class="Bound">l1</a> <a id="1044" href="univalent-combinatorics.composition-species.html#1044" class="Bound">l2</a> <a id="1047" class="Symbol">:</a> <a id="1049" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1054" class="Symbol">}</a> <a id="1056" class="Symbol">→</a> <a id="1058" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1066" href="univalent-combinatorics.composition-species.html#1041" class="Bound">l1</a> <a id="1069" class="Symbol">→</a> <a id="1071" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1079" href="univalent-combinatorics.composition-species.html#1044" class="Bound">l2</a> <a id="1082" class="Symbol">→</a> <a id="1084" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1092" class="Symbol">(</a><a id="1093" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1098" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="1104" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1106" href="univalent-combinatorics.composition-species.html#1041" class="Bound">l1</a> <a id="1109" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1111" href="univalent-combinatorics.composition-species.html#1044" class="Bound">l2</a><a id="1113" class="Symbol">)</a>
<a id="1115" href="univalent-combinatorics.composition-species.html#1014" class="Function">analytic-comp-species</a> <a id="1137" href="univalent-combinatorics.composition-species.html#1137" class="Bound">S</a> <a id="1139" href="univalent-combinatorics.composition-species.html#1139" class="Bound">T</a> <a id="1141" href="univalent-combinatorics.composition-species.html#1141" class="Bound">X</a> <a id="1143" class="Symbol">=</a>
  <a id="1147" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1149" class="Symbol">(</a> <a id="1151" href="univalent-combinatorics.partitions.html#1956" class="Function">partition-𝔽</a> <a id="1163" href="univalent-combinatorics.composition-species.html#1141" class="Bound">X</a><a id="1164" class="Symbol">)</a>
    <a id="1170" class="Symbol">(</a> <a id="1172" class="Symbol">λ</a> <a id="1174" href="univalent-combinatorics.composition-species.html#1174" class="Bound">P</a> <a id="1176" class="Symbol">→</a>
      <a id="1184" class="Symbol">(</a> <a id="1186" href="univalent-combinatorics.composition-species.html#1139" class="Bound">T</a> <a id="1188" class="Symbol">(</a><a id="1189" href="univalent-combinatorics.partitions.html#2216" class="Function">finite-indexing-type-partition-𝔽</a> <a id="1222" href="univalent-combinatorics.composition-species.html#1141" class="Bound">X</a> <a id="1224" href="univalent-combinatorics.composition-species.html#1174" class="Bound">P</a><a id="1225" class="Symbol">))</a> <a id="1228" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a>
      <a id="1236" class="Symbol">(</a> <a id="1238" class="Symbol">(</a><a id="1239" href="univalent-combinatorics.composition-species.html#1239" class="Bound">y</a> <a id="1241" class="Symbol">:</a> <a id="1243" href="univalent-combinatorics.partitions.html#2299" class="Function">indexing-type-partition-𝔽</a> <a id="1269" href="univalent-combinatorics.composition-species.html#1141" class="Bound">X</a> <a id="1271" href="univalent-combinatorics.composition-species.html#1174" class="Bound">P</a><a id="1272" class="Symbol">)</a> <a id="1274" class="Symbol">→</a>
        <a id="1284" href="univalent-combinatorics.composition-species.html#1137" class="Bound">S</a> <a id="1286" class="Symbol">(</a><a id="1287" href="univalent-combinatorics.partitions.html#2750" class="Function">finite-block-partition-𝔽</a> <a id="1312" href="univalent-combinatorics.composition-species.html#1141" class="Bound">X</a> <a id="1314" href="univalent-combinatorics.composition-species.html#1174" class="Bound">P</a> <a id="1316" href="univalent-combinatorics.composition-species.html#1239" class="Bound">y</a><a id="1317" class="Symbol">)))</a>
</pre>
### The analytic unit for composition of species

<pre class="Agda"><a id="analytic-unit-species"></a><a id="1384" href="univalent-combinatorics.composition-species.html#1384" class="Function">analytic-unit-species</a> <a id="1406" class="Symbol">:</a> <a id="1408" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1416" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="1422" href="univalent-combinatorics.composition-species.html#1384" class="Function">analytic-unit-species</a> <a id="1444" href="univalent-combinatorics.composition-species.html#1444" class="Bound">X</a> <a id="1446" class="Symbol">=</a> <a id="1448" href="foundation-core.contractible-types.html#1006" class="Function">is-contr</a> <a id="1457" class="Symbol">(</a><a id="1458" href="univalent-combinatorics.finite-types.html#4912" class="Function">type-𝔽</a> <a id="1465" href="univalent-combinatorics.composition-species.html#1444" class="Bound">X</a><a id="1466" class="Symbol">)</a>
</pre>
## Properties

### Unit laws for analytic composition of species

<pre class="Agda"><a id="left-unit-law-comp-species"></a><a id="1547" href="univalent-combinatorics.composition-species.html#1547" class="Function">left-unit-law-comp-species</a> <a id="1574" class="Symbol">:</a>
  <a id="1578" class="Symbol">{</a><a id="1579" href="univalent-combinatorics.composition-species.html#1579" class="Bound">l</a> <a id="1581" class="Symbol">:</a> <a id="1583" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1588" class="Symbol">}</a> <a id="1590" class="Symbol">(</a><a id="1591" href="univalent-combinatorics.composition-species.html#1591" class="Bound">F</a> <a id="1593" class="Symbol">:</a> <a id="1595" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="1603" href="univalent-combinatorics.composition-species.html#1579" class="Bound">l</a><a id="1604" class="Symbol">)</a> <a id="1606" class="Symbol">→</a>
  <a id="1610" href="univalent-combinatorics.equivalences-species.html#677" class="Function">equiv-species</a> <a id="1624" class="Symbol">(</a><a id="1625" href="univalent-combinatorics.composition-species.html#1014" class="Function">analytic-comp-species</a> <a id="1647" href="univalent-combinatorics.composition-species.html#1384" class="Function">analytic-unit-species</a> <a id="1669" href="univalent-combinatorics.composition-species.html#1591" class="Bound">F</a><a id="1670" class="Symbol">)</a> <a id="1672" href="univalent-combinatorics.composition-species.html#1591" class="Bound">F</a>
<a id="1674" href="univalent-combinatorics.composition-species.html#1547" class="Function">left-unit-law-comp-species</a> <a id="1701" href="univalent-combinatorics.composition-species.html#1701" class="Bound">F</a> <a id="1703" href="univalent-combinatorics.composition-species.html#1703" class="Bound">X</a> <a id="1705" class="Symbol">=</a>
  <a id="1709" class="Hole">{!!}</a>
</pre>