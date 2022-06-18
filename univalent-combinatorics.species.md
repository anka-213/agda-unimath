---
title: Species
---

<pre class="Agda"><a id="33" class="Symbol">{-#</a> <a id="37" class="Keyword">OPTIONS</a> <a id="45" class="Pragma">--without-K</a> <a id="57" class="Pragma">--exact-split</a> <a id="71" class="Symbol">#-}</a>

<a id="76" class="Keyword">module</a> <a id="83" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a> <a id="115" class="Keyword">where</a>

<a id="122" class="Keyword">open</a> <a id="127" class="Keyword">import</a> <a id="134" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="161" class="Keyword">using</a> <a id="167" class="Symbol">(</a><a id="168" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="173" class="Symbol">;</a> <a id="175" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="177" class="Symbol">;</a> <a id="179" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="183" class="Symbol">)</a>

<a id="186" class="Keyword">open</a> <a id="191" class="Keyword">import</a> <a id="198" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="235" class="Keyword">using</a> <a id="241" class="Symbol">(</a><a id="242" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a><a id="243" class="Symbol">)</a>
</pre>
### Idea

In this file, we define the type of species. A species is just a
map from 𝔽 to a universe.

## Definition

<pre class="Agda"><a id="species"></a><a id="375" href="univalent-combinatorics.species.html#375" class="Function">species</a> <a id="383" class="Symbol">:</a> <a id="385" class="Symbol">(</a><a id="386" href="univalent-combinatorics.species.html#386" class="Bound">l</a> <a id="388" class="Symbol">:</a> <a id="390" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="395" class="Symbol">)</a> <a id="397" class="Symbol">→</a> <a id="399" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="402" class="Symbol">(</a><a id="403" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="408" href="univalent-combinatorics.species.html#386" class="Bound">l</a><a id="409" class="Symbol">)</a>
<a id="411" href="univalent-combinatorics.species.html#375" class="Function">species</a> <a id="419" href="univalent-combinatorics.species.html#419" class="Bound">l</a> <a id="421" class="Symbol">=</a> <a id="423" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a> <a id="425" class="Symbol">→</a> <a id="427" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="430" href="univalent-combinatorics.species.html#419" class="Bound">l</a>
</pre>