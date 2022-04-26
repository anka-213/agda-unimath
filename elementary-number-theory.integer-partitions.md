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

An integer partition of a natural number n is a list of nonzero natural numbers that sum up to n, up to reordering.

## Definition

<pre class="Agda"><a id="list-nonzero-ℕ"></a><a id="727" href="elementary-number-theory.integer-partitions.html#727" class="Function">list-nonzero-ℕ</a> <a id="742" class="Symbol">:</a> <a id="744" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="747" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="753" href="elementary-number-theory.integer-partitions.html#727" class="Function">list-nonzero-ℕ</a> <a id="768" class="Symbol">=</a> <a id="770" href="univalent-combinatorics.lists.html#2152" class="Datatype">list</a> <a id="775" href="elementary-number-theory.nonzero-natural-numbers.html#710" class="Function">nonzero-ℕ</a>

<a id="sum-list-nonzero-ℕ"></a><a id="786" href="elementary-number-theory.integer-partitions.html#786" class="Function">sum-list-nonzero-ℕ</a> <a id="805" class="Symbol">:</a> <a id="807" href="elementary-number-theory.integer-partitions.html#727" class="Function">list-nonzero-ℕ</a> <a id="822" class="Symbol">→</a> <a id="824" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a>
<a id="826" href="elementary-number-theory.integer-partitions.html#786" class="Function">sum-list-nonzero-ℕ</a> <a id="845" href="univalent-combinatorics.lists.html#2195" class="InductiveConstructor">nil</a> <a id="849" class="Symbol">=</a> <a id="851" class="Number">0</a>
<a id="853" href="elementary-number-theory.integer-partitions.html#786" class="Function">sum-list-nonzero-ℕ</a> <a id="872" class="Symbol">(</a><a id="873" href="univalent-combinatorics.lists.html#2210" class="InductiveConstructor">cons</a> <a id="878" href="elementary-number-theory.integer-partitions.html#878" class="Bound">x</a> <a id="880" href="elementary-number-theory.integer-partitions.html#880" class="Bound">l</a><a id="881" class="Symbol">)</a> <a id="883" class="Symbol">=</a> <a id="885" href="elementary-number-theory.addition-natural-numbers.html#988" class="Function">add-ℕ</a> <a id="891" class="Symbol">(</a><a id="892" href="elementary-number-theory.nonzero-natural-numbers.html#761" class="Function">nat-nonzero-ℕ</a> <a id="906" href="elementary-number-theory.integer-partitions.html#878" class="Bound">x</a><a id="907" class="Symbol">)</a> <a id="909" class="Symbol">(</a><a id="910" href="elementary-number-theory.integer-partitions.html#786" class="Function">sum-list-nonzero-ℕ</a> <a id="929" href="elementary-number-theory.integer-partitions.html#880" class="Bound">l</a><a id="930" class="Symbol">)</a>

<a id="integer-partition&#39;"></a><a id="933" href="elementary-number-theory.integer-partitions.html#933" class="Function">integer-partition&#39;</a> <a id="952" class="Symbol">:</a> <a id="954" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a> <a id="956" class="Symbol">→</a> <a id="958" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="961" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="967" href="elementary-number-theory.integer-partitions.html#933" class="Function">integer-partition&#39;</a> <a id="986" class="Symbol">=</a> <a id="988" href="foundation-core.fibers-of-maps.html#928" class="Function">fib</a> <a id="992" href="elementary-number-theory.integer-partitions.html#786" class="Function">sum-list-nonzero-ℕ</a>
</pre>