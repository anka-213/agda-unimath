---
title: Retracts of the type of natural numbers
---

<pre class="Agda"><a id="65" class="Symbol">{-#</a> <a id="69" class="Keyword">OPTIONS</a> <a id="77" class="Pragma">--without-K</a> <a id="89" class="Pragma">--exact-split</a> <a id="103" class="Symbol">#-}</a>

<a id="108" class="Keyword">module</a> <a id="115" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a> <a id="168" class="Keyword">where</a>

<a id="175" class="Keyword">open</a> <a id="180" class="Keyword">import</a> <a id="187" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a> <a id="237" class="Keyword">using</a>
  <a id="245" class="Symbol">(</a> <a id="247" href="elementary-number-theory.equality-natural-numbers.html#2644" class="Function">has-decidable-equality-ℕ</a><a id="271" class="Symbol">)</a>
<a id="273" class="Keyword">open</a> <a id="278" class="Keyword">import</a> <a id="285" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="326" class="Keyword">using</a> <a id="332" class="Symbol">(</a><a id="333" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="334" class="Symbol">)</a>

<a id="337" class="Keyword">open</a> <a id="342" class="Keyword">import</a> <a id="349" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a> <a id="375" class="Keyword">using</a>
  <a id="383" class="Symbol">(</a> <a id="385" href="foundation.decidable-maps.html#758" class="Function">is-decidable-map</a><a id="401" class="Symbol">;</a> <a id="403" href="foundation.decidable-maps.html#869" class="Function">is-decidable-map-retr</a><a id="424" class="Symbol">)</a>
<a id="426" class="Keyword">open</a> <a id="431" class="Keyword">import</a> <a id="438" href="foundation.retractions.html" class="Module">foundation.retractions</a> <a id="461" class="Keyword">using</a> <a id="467" class="Symbol">(</a><a id="468" href="foundation-core.retractions.html#607" class="Function">retr</a><a id="472" class="Symbol">)</a>
<a id="474" class="Keyword">open</a> <a id="479" class="Keyword">import</a> <a id="486" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="513" class="Keyword">using</a> <a id="519" class="Symbol">(</a><a id="520" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="525" class="Symbol">;</a> <a id="527" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="529" class="Symbol">)</a>
</pre>
## Idea

If `i : A → ℕ` has a retraction, then `i` is a decidable map.

<pre class="Agda"><a id="is-decidable-map-retr-ℕ"></a><a id="616" href="elementary-number-theory.retracts-of-natural-numbers.html#616" class="Function">is-decidable-map-retr-ℕ</a> <a id="640" class="Symbol">:</a>
  <a id="644" class="Symbol">{</a><a id="645" href="elementary-number-theory.retracts-of-natural-numbers.html#645" class="Bound">l1</a> <a id="648" class="Symbol">:</a> <a id="650" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="655" class="Symbol">}</a> <a id="657" class="Symbol">{</a><a id="658" href="elementary-number-theory.retracts-of-natural-numbers.html#658" class="Bound">A</a> <a id="660" class="Symbol">:</a> <a id="662" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="665" href="elementary-number-theory.retracts-of-natural-numbers.html#645" class="Bound">l1</a><a id="667" class="Symbol">}</a> <a id="669" class="Symbol">(</a><a id="670" href="elementary-number-theory.retracts-of-natural-numbers.html#670" class="Bound">i</a> <a id="672" class="Symbol">:</a> <a id="674" href="elementary-number-theory.retracts-of-natural-numbers.html#658" class="Bound">A</a> <a id="676" class="Symbol">→</a> <a id="678" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="679" class="Symbol">)</a> <a id="681" class="Symbol">→</a> <a id="683" href="foundation-core.retractions.html#607" class="Function">retr</a> <a id="688" href="elementary-number-theory.retracts-of-natural-numbers.html#670" class="Bound">i</a> <a id="690" class="Symbol">→</a> <a id="692" href="foundation.decidable-maps.html#758" class="Function">is-decidable-map</a> <a id="709" href="elementary-number-theory.retracts-of-natural-numbers.html#670" class="Bound">i</a>
<a id="711" href="elementary-number-theory.retracts-of-natural-numbers.html#616" class="Function">is-decidable-map-retr-ℕ</a> <a id="735" class="Symbol">=</a>
  <a id="739" href="foundation.decidable-maps.html#869" class="Function">is-decidable-map-retr</a> <a id="761" href="elementary-number-theory.equality-natural-numbers.html#2644" class="Function">has-decidable-equality-ℕ</a>
</pre>