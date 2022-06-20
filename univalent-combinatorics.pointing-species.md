---
title: Pointing of species
---

<pre class="Agda"><a id="45" class="Symbol">{-#</a> <a id="49" class="Keyword">OPTIONS</a> <a id="57" class="Pragma">--without-K</a> <a id="69" class="Pragma">--exact-split</a> <a id="83" class="Symbol">#-}</a>

<a id="88" class="Keyword">module</a> <a id="95" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a> <a id="136" class="Keyword">where</a>

<a id="143" class="Keyword">open</a> <a id="148" class="Keyword">import</a> <a id="155" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="190" class="Keyword">open</a> <a id="195" class="Keyword">import</a> <a id="202" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="230" class="Keyword">open</a> <a id="235" class="Keyword">import</a> <a id="242" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="279" class="Keyword">open</a> <a id="284" class="Keyword">import</a> <a id="291" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
</pre>
## Idea

A pointing of a species `F` is the species `F*` given by `F* X := X × (F X)`. In other words, it is the species of pointed `F`-structures

## Definition

<pre class="Agda"><a id="pointing-species"></a><a id="499" href="univalent-combinatorics.pointing-species.html#499" class="Function">pointing-species</a> <a id="516" class="Symbol">:</a> <a id="518" class="Symbol">{</a><a id="519" href="univalent-combinatorics.pointing-species.html#519" class="Bound">l</a> <a id="521" class="Symbol">:</a> <a id="523" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="528" class="Symbol">}</a> <a id="530" class="Symbol">→</a> <a id="532" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="540" href="univalent-combinatorics.pointing-species.html#519" class="Bound">l</a> <a id="542" class="Symbol">→</a> <a id="544" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="552" href="univalent-combinatorics.pointing-species.html#519" class="Bound">l</a>
<a id="554" href="univalent-combinatorics.pointing-species.html#499" class="Function">pointing-species</a> <a id="571" href="univalent-combinatorics.pointing-species.html#571" class="Bound">F</a> <a id="573" href="univalent-combinatorics.pointing-species.html#573" class="Bound">X</a> <a id="575" class="Symbol">=</a> <a id="577" href="univalent-combinatorics.finite-types.html#4687" class="Function">type-𝔽</a> <a id="584" href="univalent-combinatorics.pointing-species.html#573" class="Bound">X</a> <a id="586" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="588" href="univalent-combinatorics.pointing-species.html#571" class="Bound">F</a> <a id="590" href="univalent-combinatorics.pointing-species.html#573" class="Bound">X</a>
</pre>