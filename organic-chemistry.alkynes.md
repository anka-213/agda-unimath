---
title: Alkynes
---

<pre class="Agda"><a id="33" class="Symbol">{-#</a> <a id="37" class="Keyword">OPTIONS</a> <a id="45" class="Pragma">--without-K</a> <a id="57" class="Pragma">--exact-split</a> <a id="71" class="Symbol">#-}</a>

<a id="76" class="Keyword">module</a> <a id="83" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a> <a id="109" class="Keyword">where</a>

<a id="116" class="Keyword">open</a> <a id="121" class="Keyword">import</a> <a id="128" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="170" class="Keyword">open</a> <a id="175" class="Keyword">import</a> <a id="182" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="214" class="Keyword">open</a> <a id="219" class="Keyword">import</a> <a id="226" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="253" class="Keyword">open</a> <a id="258" class="Keyword">import</a> <a id="265" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>

<a id="288" class="Keyword">open</a> <a id="293" class="Keyword">import</a> <a id="300" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>

<a id="338" class="Keyword">open</a> <a id="343" class="Keyword">import</a> <a id="350" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
<a id="386" class="Keyword">open</a> <a id="391" class="Keyword">import</a> <a id="398" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
</pre>
## Idea

An **n-alkyne** is a hydrocarbon equipped with a choice of $n$ carbons, each of which has a triple bond.

## Definition

<pre class="Agda"><a id="n-alkyne"></a><a id="572" href="organic-chemistry.alkynes.html#572" class="Function">n-alkyne</a> <a id="581" class="Symbol">:</a> <a id="583" href="organic-chemistry.hydrocarbons.html#1564" class="Function">hydrocarbon</a> <a id="595" class="Symbol">→</a> <a id="597" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="599" class="Symbol">→</a> <a id="601" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="604" class="Symbol">(</a><a id="605" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="610" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="615" class="Symbol">)</a>
<a id="617" href="organic-chemistry.alkynes.html#572" class="Function">n-alkyne</a> <a id="626" href="organic-chemistry.alkynes.html#626" class="Bound">H</a> <a id="628" href="organic-chemistry.alkynes.html#628" class="Bound">n</a> <a id="630" class="Symbol">=</a>
  <a id="634" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="636" class="Symbol">(</a><a id="637" href="univalent-combinatorics.finite-types.html#5852" class="Function">UU-Fin</a> <a id="644" href="organic-chemistry.alkynes.html#628" class="Bound">n</a><a id="645" class="Symbol">)</a> <a id="647" class="Symbol">λ</a> <a id="649" href="organic-chemistry.alkynes.html#649" class="Bound">carbons</a> <a id="657" class="Symbol">→</a>
    <a id="663" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="665" class="Symbol">(</a><a id="666" href="univalent-combinatorics.finite-types.html#5914" class="Function">type-UU-Fin</a> <a id="678" href="organic-chemistry.alkynes.html#628" class="Bound">n</a> <a id="680" href="organic-chemistry.alkynes.html#649" class="Bound">carbons</a> <a id="688" href="foundation-core.embeddings.html#1074" class="Function Operator">↪</a> <a id="690" href="organic-chemistry.hydrocarbons.html#2659" class="Function">vertex-hydrocarbon</a> <a id="709" href="organic-chemistry.alkynes.html#626" class="Bound">H</a><a id="710" class="Symbol">)</a> <a id="712" class="Symbol">λ</a> <a id="714" href="organic-chemistry.alkynes.html#714" class="Bound">embed-carbons</a> <a id="728" class="Symbol">→</a>
      <a id="736" class="Symbol">(</a><a id="737" href="organic-chemistry.alkynes.html#737" class="Bound">c</a> <a id="739" class="Symbol">:</a> <a id="741" href="univalent-combinatorics.finite-types.html#5914" class="Function">type-UU-Fin</a> <a id="753" href="organic-chemistry.alkynes.html#628" class="Bound">n</a> <a id="755" href="organic-chemistry.alkynes.html#649" class="Bound">carbons</a><a id="762" class="Symbol">)</a> <a id="764" class="Symbol">→</a> <a id="766" href="organic-chemistry.saturated-carbons.html#1828" class="Function">has-triple-bond-hydrocarbon</a> <a id="794" href="organic-chemistry.alkynes.html#626" class="Bound">H</a> <a id="796" class="Symbol">(</a><a id="797" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="801" href="organic-chemistry.alkynes.html#714" class="Bound">embed-carbons</a> <a id="815" href="organic-chemistry.alkynes.html#737" class="Bound">c</a><a id="816" class="Symbol">)</a>
</pre>