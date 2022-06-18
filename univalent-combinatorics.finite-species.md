---
title: Finite species
---

<pre class="Agda"><a id="40" class="Symbol">{-#</a> <a id="44" class="Keyword">OPTIONS</a> <a id="52" class="Pragma">--without-K</a> <a id="64" class="Pragma">--exact-split</a> <a id="78" class="Symbol">#-}</a>

<a id="83" class="Keyword">module</a> <a id="90" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a> <a id="129" class="Keyword">where</a>

<a id="136" class="Keyword">open</a> <a id="141" class="Keyword">import</a> <a id="148" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="176" class="Keyword">open</a> <a id="181" class="Keyword">import</a> <a id="188" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="225" class="Keyword">open</a> <a id="230" class="Keyword">import</a> <a id="237" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
</pre>
### Idea

In this file, we define the type of finite species. A finite
species is just a map from 𝔽 to 𝔽.

## Definition

<pre class="Agda"><a id="finite-species"></a><a id="404" href="univalent-combinatorics.finite-species.html#404" class="Function">finite-species</a> <a id="419" class="Symbol">:</a> <a id="421" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="424" class="Symbol">(</a><a id="425" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="430" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="435" class="Symbol">)</a>
<a id="437" href="univalent-combinatorics.finite-species.html#404" class="Function">finite-species</a> <a id="452" class="Symbol">=</a> <a id="454" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a> <a id="456" class="Symbol">→</a> <a id="458" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a>

<a id="species-finite-species"></a><a id="461" href="univalent-combinatorics.finite-species.html#461" class="Function">species-finite-species</a> <a id="484" class="Symbol">:</a> <a id="486" href="univalent-combinatorics.finite-species.html#404" class="Function">finite-species</a> <a id="501" class="Symbol">→</a> <a id="503" href="univalent-combinatorics.species.html#375" class="Function">species</a> <a id="511" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="517" href="univalent-combinatorics.finite-species.html#461" class="Function">species-finite-species</a> <a id="540" href="univalent-combinatorics.finite-species.html#540" class="Bound">F</a> <a id="542" href="univalent-combinatorics.finite-species.html#542" class="Bound">X</a> <a id="544" class="Symbol">=</a> <a id="546" href="univalent-combinatorics.finite-types.html#4503" class="Function">type-𝔽</a> <a id="553" href="univalent-combinatorics.finite-species.html#542" class="Bound">X</a>
</pre>