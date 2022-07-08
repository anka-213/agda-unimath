---
title: Counting the elements of the fiber of a map
---

<pre class="Agda"><a id="69" class="Symbol">{-#</a> <a id="73" class="Keyword">OPTIONS</a> <a id="81" class="Pragma">--without-K</a> <a id="93" class="Pragma">--exact-split</a> <a id="107" class="Symbol">#-}</a>

<a id="112" class="Keyword">module</a> <a id="119" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a> <a id="167" class="Keyword">where</a>

<a id="174" class="Keyword">open</a> <a id="179" class="Keyword">import</a> <a id="186" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a> <a id="235" class="Keyword">using</a>
  <a id="243" class="Symbol">(</a> <a id="245" href="elementary-number-theory.sums-of-natural-numbers.html#1661" class="Function">sum-count-ℕ</a><a id="256" class="Symbol">)</a>

<a id="259" class="Keyword">open</a> <a id="264" class="Keyword">import</a> <a id="271" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a> <a id="297" class="Keyword">using</a> <a id="303" class="Symbol">(</a><a id="304" href="foundation-core.fibers-of-maps.html#942" class="Function">fib</a><a id="307" class="Symbol">;</a> <a id="309" href="foundation-core.fibers-of-maps.html#5254" class="Function">equiv-total-fib</a><a id="324" class="Symbol">)</a>
<a id="326" class="Keyword">open</a> <a id="331" class="Keyword">import</a> <a id="338" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="364" class="Keyword">using</a> <a id="370" class="Symbol">(</a><a id="371" href="foundation-core.identity-types.html#1767" class="Datatype">Id</a><a id="373" class="Symbol">)</a>
<a id="375" class="Keyword">open</a> <a id="380" class="Keyword">import</a> <a id="387" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="414" class="Keyword">using</a> <a id="420" class="Symbol">(</a><a id="421" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="426" class="Symbol">;</a> <a id="428" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="430" class="Symbol">)</a>

<a id="433" class="Keyword">open</a> <a id="438" class="Keyword">import</a> <a id="445" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a> <a id="478" class="Keyword">using</a>
  <a id="486" class="Symbol">(</a> <a id="488" href="univalent-combinatorics.counting.html#1901" class="Function">count</a><a id="493" class="Symbol">;</a> <a id="495" href="univalent-combinatorics.counting.html#3709" class="Function">count-equiv&#39;</a><a id="507" class="Symbol">;</a> <a id="509" href="univalent-combinatorics.counting.html#2029" class="Function">number-of-elements-count</a><a id="533" class="Symbol">)</a>
<a id="535" class="Keyword">open</a> <a id="540" class="Keyword">import</a> <a id="547" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a> <a id="601" class="Keyword">using</a>
  <a id="609" class="Symbol">(</a> <a id="611" href="univalent-combinatorics.counting-dependent-pair-types.html#5328" class="Function">count-fiber-count-Σ</a><a id="630" class="Symbol">;</a> <a id="632" href="univalent-combinatorics.counting-dependent-pair-types.html#9018" class="Function">sum-number-of-elements-count-fiber-count-Σ</a><a id="674" class="Symbol">)</a>
<a id="676" class="Keyword">open</a> <a id="681" class="Keyword">import</a> <a id="688" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a> <a id="728" class="Keyword">using</a> <a id="734" class="Symbol">(</a><a id="735" href="univalent-combinatorics.double-counting.html#1110" class="Function">double-counting</a><a id="750" class="Symbol">)</a>
</pre>