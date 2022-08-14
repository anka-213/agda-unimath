---
title: Integer partitions
---

<pre class="Agda"><a id="44" class="Symbol">{-#</a> <a id="48" class="Keyword">OPTIONS</a> <a id="56" class="Pragma">--without-K</a> <a id="68" class="Pragma">--exact-split</a> <a id="82" class="Symbol">#-}</a>

<a id="87" class="Keyword">module</a> <a id="94" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a> <a id="138" class="Keyword">where</a>

<a id="145" class="Keyword">open</a> <a id="150" class="Keyword">import</a> <a id="157" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="207" class="Keyword">open</a> <a id="212" class="Keyword">import</a> <a id="219" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="260" class="Keyword">open</a> <a id="265" class="Keyword">import</a> <a id="272" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>

<a id="322" class="Keyword">open</a> <a id="327" class="Keyword">import</a> <a id="334" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="366" class="Keyword">open</a> <a id="371" class="Keyword">import</a> <a id="378" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="404" class="Keyword">open</a> <a id="409" class="Keyword">import</a> <a id="416" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="442" class="Keyword">open</a> <a id="447" class="Keyword">import</a> <a id="454" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="482" class="Keyword">open</a> <a id="487" class="Keyword">import</a> <a id="494" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="531" class="Keyword">open</a> <a id="536" class="Keyword">import</a> <a id="543" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
</pre>
## Idea

An integer partition of a natural number n is a list of nonzero natural numbers that sum up to n, up to reordering. We define the number `p n` of integer partitions of `n` as the number of connected components in the type of finite Ferrer diagrams of `Fin n`.