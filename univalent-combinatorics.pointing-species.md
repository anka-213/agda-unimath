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

<pre class="Agda"><a id="pointing-species"></a><a id="499" href="univalent-combinatorics.pointing-species.html#499" class="Function">pointing-species</a> <a id="516" class="Symbol">:</a> <a id="518" class="Symbol">{</a><a id="519" href="univalent-combinatorics.pointing-species.html#519" class="Bound">l1</a> <a id="522" href="univalent-combinatorics.pointing-species.html#522" class="Bound">l2</a> <a id="525" class="Symbol">:</a> <a id="527" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="532" class="Symbol">}</a> <a id="534" class="Symbol">→</a> <a id="536" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="544" href="univalent-combinatorics.pointing-species.html#519" class="Bound">l1</a> <a id="547" href="univalent-combinatorics.pointing-species.html#522" class="Bound">l2</a> <a id="550" class="Symbol">→</a> <a id="552" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="560" href="univalent-combinatorics.pointing-species.html#519" class="Bound">l1</a> <a id="563" class="Symbol">(</a><a id="564" href="univalent-combinatorics.pointing-species.html#519" class="Bound">l1</a> <a id="567" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="569" href="univalent-combinatorics.pointing-species.html#522" class="Bound">l2</a><a id="571" class="Symbol">)</a>
<a id="573" href="univalent-combinatorics.pointing-species.html#499" class="Function">pointing-species</a> <a id="590" href="univalent-combinatorics.pointing-species.html#590" class="Bound">F</a> <a id="592" href="univalent-combinatorics.pointing-species.html#592" class="Bound">X</a> <a id="594" class="Symbol">=</a> <a id="596" href="univalent-combinatorics.finite-types.html#4606" class="Function">type-𝔽</a> <a id="603" href="univalent-combinatorics.pointing-species.html#592" class="Bound">X</a> <a id="605" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a> <a id="607" href="univalent-combinatorics.pointing-species.html#590" class="Bound">F</a> <a id="609" href="univalent-combinatorics.pointing-species.html#592" class="Bound">X</a>
</pre>