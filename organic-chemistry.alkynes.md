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

<pre class="Agda"><a id="n-alkyne"></a><a id="572" href="organic-chemistry.alkynes.html#572" class="Function">n-alkyne</a> <a id="581" class="Symbol">:</a> <a id="583" class="Symbol">{</a><a id="584" href="organic-chemistry.alkynes.html#584" class="Bound">l1</a> <a id="587" href="organic-chemistry.alkynes.html#587" class="Bound">l2</a> <a id="590" class="Symbol">:</a> <a id="592" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="597" class="Symbol">}</a> <a id="599" class="Symbol">→</a> <a id="601" href="organic-chemistry.hydrocarbons.html#1564" class="Function">hydrocarbon</a> <a id="613" href="organic-chemistry.alkynes.html#584" class="Bound">l1</a> <a id="616" href="organic-chemistry.alkynes.html#587" class="Bound">l2</a> <a id="619" class="Symbol">→</a> <a id="621" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="623" class="Symbol">→</a> <a id="625" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="628" class="Symbol">(</a><a id="629" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="634" href="organic-chemistry.alkynes.html#584" class="Bound">l1</a> <a id="637" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="639" href="organic-chemistry.alkynes.html#587" class="Bound">l2</a><a id="641" class="Symbol">)</a>
<a id="643" href="organic-chemistry.alkynes.html#572" class="Function">n-alkyne</a> <a id="652" class="Symbol">{</a><a id="653" href="organic-chemistry.alkynes.html#653" class="Bound">l1</a><a id="655" class="Symbol">}</a> <a id="657" class="Symbol">{</a><a id="658" href="organic-chemistry.alkynes.html#658" class="Bound">l2</a><a id="660" class="Symbol">}</a> <a id="662" href="organic-chemistry.alkynes.html#662" class="Bound">H</a> <a id="664" href="organic-chemistry.alkynes.html#664" class="Bound">n</a> <a id="666" class="Symbol">=</a>
  <a id="670" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="672" class="Symbol">(</a> <a id="674" href="univalent-combinatorics.finite-types.html#5087" class="Function">UU-Fin</a> <a id="681" href="organic-chemistry.alkynes.html#653" class="Bound">l1</a> <a id="684" href="organic-chemistry.alkynes.html#664" class="Bound">n</a><a id="685" class="Symbol">)</a>
    <a id="691" class="Symbol">(</a> <a id="693" class="Symbol">λ</a> <a id="695" href="organic-chemistry.alkynes.html#695" class="Bound">carbons</a> <a id="703" class="Symbol">→</a>
      <a id="711" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="713" class="Symbol">(</a> <a id="715" href="univalent-combinatorics.finite-types.html#5170" class="Function">type-UU-Fin</a> <a id="727" href="organic-chemistry.alkynes.html#664" class="Bound">n</a> <a id="729" href="organic-chemistry.alkynes.html#695" class="Bound">carbons</a> <a id="737" href="foundation-core.embeddings.html#1074" class="Function Operator">↪</a> <a id="739" href="organic-chemistry.hydrocarbons.html#2727" class="Function">vertex-hydrocarbon</a> <a id="758" href="organic-chemistry.alkynes.html#662" class="Bound">H</a><a id="759" class="Symbol">)</a>
        <a id="769" class="Symbol">(</a> <a id="771" class="Symbol">λ</a> <a id="773" href="organic-chemistry.alkynes.html#773" class="Bound">embed-carbons</a> <a id="787" class="Symbol">→</a>
          <a id="799" class="Symbol">(</a><a id="800" href="organic-chemistry.alkynes.html#800" class="Bound">c</a> <a id="802" class="Symbol">:</a> <a id="804" href="univalent-combinatorics.finite-types.html#5170" class="Function">type-UU-Fin</a> <a id="816" href="organic-chemistry.alkynes.html#664" class="Bound">n</a> <a id="818" href="organic-chemistry.alkynes.html#695" class="Bound">carbons</a><a id="825" class="Symbol">)</a> <a id="827" class="Symbol">→</a>
          <a id="839" href="organic-chemistry.saturated-carbons.html#1876" class="Function">has-triple-bond-hydrocarbon</a> <a id="867" href="organic-chemistry.alkynes.html#662" class="Bound">H</a> <a id="869" class="Symbol">(</a><a id="870" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="874" href="organic-chemistry.alkynes.html#773" class="Bound">embed-carbons</a> <a id="888" href="organic-chemistry.alkynes.html#800" class="Bound">c</a><a id="889" class="Symbol">)))</a>
</pre>