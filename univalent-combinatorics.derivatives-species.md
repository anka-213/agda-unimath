---
title: Derivatives of species
---

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a> <a id="142" class="Keyword">where</a>

<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="189" class="Keyword">open</a> <a id="194" class="Keyword">import</a> <a id="201" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="290" class="Keyword">open</a> <a id="295" class="Keyword">import</a> <a id="302" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
</pre>
## Idea

When we think of a species as the coefficients of a formal power series, the derivative of a species is the species representing the derivative of that formal power series.

## Definition

<pre class="Agda"><a id="derivative-species"></a><a id="545" href="univalent-combinatorics.derivatives-species.html#545" class="Function">derivative-species</a> <a id="564" class="Symbol">:</a>
  <a id="568" class="Symbol">{</a><a id="569" href="univalent-combinatorics.derivatives-species.html#569" class="Bound">l</a> <a id="571" class="Symbol">:</a> <a id="573" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="578" class="Symbol">}</a> <a id="580" class="Symbol">→</a> <a id="582" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="590" href="univalent-combinatorics.derivatives-species.html#569" class="Bound">l</a> <a id="592" class="Symbol">→</a> <a id="594" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="602" href="univalent-combinatorics.derivatives-species.html#569" class="Bound">l</a>
<a id="604" href="univalent-combinatorics.derivatives-species.html#545" class="Function">derivative-species</a> <a id="623" href="univalent-combinatorics.derivatives-species.html#623" class="Bound">F</a> <a id="625" href="univalent-combinatorics.derivatives-species.html#625" class="Bound">X</a> <a id="627" class="Symbol">=</a> <a id="629" href="univalent-combinatorics.derivatives-species.html#623" class="Bound">F</a> <a id="631" class="Symbol">(</a><a id="632" href="univalent-combinatorics.coproduct-types.html#5414" class="Function">coprod-𝔽</a> <a id="641" href="univalent-combinatorics.derivatives-species.html#625" class="Bound">X</a> <a id="643" href="univalent-combinatorics.finite-types.html#8917" class="Function">unit-𝔽</a><a id="649" class="Symbol">)</a>
</pre>