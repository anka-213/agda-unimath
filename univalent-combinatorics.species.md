---
title: Species
---

<pre class="Agda"><a id="33" class="Symbol">{-#</a> <a id="37" class="Keyword">OPTIONS</a> <a id="45" class="Pragma">--without-K</a> <a id="57" class="Pragma">--exact-split</a> <a id="71" class="Symbol">#-}</a>

<a id="76" class="Keyword">module</a> <a id="83" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a> <a id="115" class="Keyword">where</a>

<a id="122" class="Keyword">open</a> <a id="127" class="Keyword">import</a> <a id="134" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="161" class="Keyword">using</a> <a id="167" class="Symbol">(</a><a id="168" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="173" class="Symbol">;</a> <a id="175" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="177" class="Symbol">;</a> <a id="179" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="183" class="Symbol">)</a>

<a id="186" class="Keyword">open</a> <a id="191" class="Keyword">import</a> <a id="198" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="235" class="Keyword">using</a> <a id="241" class="Symbol">(</a><a id="242" href="univalent-combinatorics.finite-types.html#4106" class="Function">𝔽</a><a id="243" class="Symbol">)</a>
</pre>
## Definition

<pre class="Agda"><a id="species"></a><a id="273" href="univalent-combinatorics.species.html#273" class="Function">species</a> <a id="281" class="Symbol">:</a> <a id="283" class="Symbol">(</a><a id="284" href="univalent-combinatorics.species.html#284" class="Bound">l</a> <a id="286" class="Symbol">:</a> <a id="288" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="293" class="Symbol">)</a> <a id="295" class="Symbol">→</a> <a id="297" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="300" class="Symbol">(</a><a id="301" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="306" href="univalent-combinatorics.species.html#284" class="Bound">l</a><a id="307" class="Symbol">)</a>
<a id="309" href="univalent-combinatorics.species.html#273" class="Function">species</a> <a id="317" href="univalent-combinatorics.species.html#317" class="Bound">l</a> <a id="319" class="Symbol">=</a> <a id="321" href="univalent-combinatorics.finite-types.html#4106" class="Function">𝔽</a> <a id="323" class="Symbol">→</a> <a id="325" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="328" href="univalent-combinatorics.species.html#317" class="Bound">l</a>
</pre>