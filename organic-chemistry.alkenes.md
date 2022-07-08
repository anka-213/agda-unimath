---
title: Alkynes
---

<pre class="Agda"><a id="33" class="Symbol">{-#</a> <a id="37" class="Keyword">OPTIONS</a> <a id="45" class="Pragma">--without-K</a> <a id="57" class="Pragma">--exact-split</a> <a id="71" class="Symbol">#-}</a>

<a id="76" class="Keyword">module</a> <a id="83" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a> <a id="109" class="Keyword">where</a>

<a id="116" class="Keyword">open</a> <a id="121" class="Keyword">import</a> <a id="128" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="170" class="Keyword">open</a> <a id="175" class="Keyword">import</a> <a id="182" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="214" class="Keyword">open</a> <a id="219" class="Keyword">import</a> <a id="226" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="253" class="Keyword">open</a> <a id="258" class="Keyword">import</a> <a id="265" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>

<a id="288" class="Keyword">open</a> <a id="293" class="Keyword">import</a> <a id="300" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>

<a id="338" class="Keyword">open</a> <a id="343" class="Keyword">import</a> <a id="350" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
<a id="386" class="Keyword">open</a> <a id="391" class="Keyword">import</a> <a id="398" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
</pre>
## Idea

An **n-alkene** is a hydrocarbon equipped with a choice of $n$ carbons, each of which has a double bond. For an n-alkene, the embedding from the given type (the first component of the n-alkene structure) specifies which carbons have double bonds. For example, 1-butene and but-2-ene have the same geometry, and the embedding is what differentiates them (while the third tautometer, isobutylene, is branched, thus has a different geometry).

## Definition

<pre class="Agda"><a id="n-alkene"></a><a id="907" href="organic-chemistry.alkenes.html#907" class="Function">n-alkene</a> <a id="916" class="Symbol">:</a> <a id="918" href="organic-chemistry.hydrocarbons.html#1564" class="Function">hydrocarbon</a> <a id="930" class="Symbol">→</a> <a id="932" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="934" class="Symbol">→</a> <a id="936" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="939" class="Symbol">(</a><a id="940" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="945" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="950" class="Symbol">)</a>
<a id="952" href="organic-chemistry.alkenes.html#907" class="Function">n-alkene</a> <a id="961" href="organic-chemistry.alkenes.html#961" class="Bound">H</a> <a id="963" href="organic-chemistry.alkenes.html#963" class="Bound">n</a> <a id="965" class="Symbol">=</a>
  <a id="969" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="971" class="Symbol">(</a><a id="972" href="univalent-combinatorics.finite-types.html#5722" class="Function">UU-Fin</a> <a id="979" href="organic-chemistry.alkenes.html#963" class="Bound">n</a><a id="980" class="Symbol">)</a> <a id="982" class="Symbol">λ</a> <a id="984" href="organic-chemistry.alkenes.html#984" class="Bound">carbons</a> <a id="992" class="Symbol">→</a>
    <a id="998" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1000" class="Symbol">(</a> <a id="1002" href="univalent-combinatorics.finite-types.html#5784" class="Function">type-UU-Fin</a> <a id="1014" href="organic-chemistry.alkenes.html#963" class="Bound">n</a> <a id="1016" href="organic-chemistry.alkenes.html#984" class="Bound">carbons</a> <a id="1024" href="foundation-core.embeddings.html#1074" class="Function Operator">↪</a> <a id="1026" href="organic-chemistry.hydrocarbons.html#2659" class="Function">vertex-hydrocarbon</a> <a id="1045" href="organic-chemistry.alkenes.html#961" class="Bound">H</a><a id="1046" class="Symbol">)</a>
      <a id="1054" class="Symbol">(</a> <a id="1056" class="Symbol">λ</a> <a id="1058" href="organic-chemistry.alkenes.html#1058" class="Bound">embed-carbons</a> <a id="1072" class="Symbol">→</a>
        <a id="1082" class="Symbol">(</a> <a id="1084" href="organic-chemistry.alkenes.html#1084" class="Bound">c</a> <a id="1086" class="Symbol">:</a> <a id="1088" href="univalent-combinatorics.finite-types.html#5784" class="Function">type-UU-Fin</a> <a id="1100" href="organic-chemistry.alkenes.html#963" class="Bound">n</a> <a id="1102" href="organic-chemistry.alkenes.html#984" class="Bound">carbons</a><a id="1109" class="Symbol">)</a> <a id="1111" class="Symbol">→</a>
        <a id="1121" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1125" class="Symbol">(</a><a id="1126" href="organic-chemistry.saturated-carbons.html#1682" class="Function">has-double-bond-hydrocarbon</a> <a id="1154" href="organic-chemistry.alkenes.html#961" class="Bound">H</a> <a id="1156" class="Symbol">(</a><a id="1157" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1161" href="organic-chemistry.alkenes.html#1058" class="Bound">embed-carbons</a> <a id="1175" href="organic-chemistry.alkenes.html#1084" class="Bound">c</a><a id="1176" class="Symbol">)))</a>
</pre>