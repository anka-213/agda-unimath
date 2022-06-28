---
title: Sequences
---

<pre class="Agda"><a id="35" class="Symbol">{-#</a> <a id="39" class="Keyword">OPTIONS</a> <a id="47" class="Pragma">--without-K</a> <a id="59" class="Pragma">--exact-split</a> <a id="73" class="Symbol">#-}</a>

<a id="78" class="Keyword">module</a> <a id="85" href="foundation.sequences.html" class="Module">foundation.sequences</a> <a id="106" class="Keyword">where</a>

<a id="113" class="Keyword">open</a> <a id="118" class="Keyword">import</a> <a id="125" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="167" class="Keyword">open</a> <a id="172" class="Keyword">import</a> <a id="179" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="200" class="Keyword">open</a> <a id="205" class="Keyword">import</a> <a id="212" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

A sequence of elements in a type `A` is a map `ℕ → A`.

## Definition

### Sequences of elements of a type

<pre class="Agda"><a id="sequence"></a><a id="369" href="foundation.sequences.html#369" class="Function">sequence</a> <a id="378" class="Symbol">:</a> <a id="380" class="Symbol">{</a><a id="381" href="foundation.sequences.html#381" class="Bound">l</a> <a id="383" class="Symbol">:</a> <a id="385" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="390" class="Symbol">}</a> <a id="392" class="Symbol">→</a> <a id="394" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="397" href="foundation.sequences.html#381" class="Bound">l</a> <a id="399" class="Symbol">→</a> <a id="401" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="404" href="foundation.sequences.html#381" class="Bound">l</a>
<a id="406" href="foundation.sequences.html#369" class="Function">sequence</a> <a id="415" href="foundation.sequences.html#415" class="Bound">A</a> <a id="417" class="Symbol">=</a> <a id="419" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a> <a id="421" class="Symbol">→</a> <a id="423" href="foundation.sequences.html#415" class="Bound">A</a>
</pre>
### Functoriality of sequences

<pre class="Agda"><a id="map-sequence"></a><a id="470" href="foundation.sequences.html#470" class="Function">map-sequence</a> <a id="483" class="Symbol">:</a>
  <a id="487" class="Symbol">{</a><a id="488" href="foundation.sequences.html#488" class="Bound">l1</a> <a id="491" href="foundation.sequences.html#491" class="Bound">l2</a> <a id="494" class="Symbol">:</a> <a id="496" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="501" class="Symbol">}</a> <a id="503" class="Symbol">{</a><a id="504" href="foundation.sequences.html#504" class="Bound">A</a> <a id="506" class="Symbol">:</a> <a id="508" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="511" href="foundation.sequences.html#488" class="Bound">l1</a><a id="513" class="Symbol">}</a> <a id="515" class="Symbol">{</a><a id="516" href="foundation.sequences.html#516" class="Bound">B</a> <a id="518" class="Symbol">:</a> <a id="520" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="523" href="foundation.sequences.html#491" class="Bound">l2</a><a id="525" class="Symbol">}</a> <a id="527" class="Symbol">→</a> <a id="529" class="Symbol">(</a><a id="530" href="foundation.sequences.html#504" class="Bound">A</a> <a id="532" class="Symbol">→</a> <a id="534" href="foundation.sequences.html#516" class="Bound">B</a><a id="535" class="Symbol">)</a> <a id="537" class="Symbol">→</a> <a id="539" href="foundation.sequences.html#369" class="Function">sequence</a> <a id="548" href="foundation.sequences.html#504" class="Bound">A</a> <a id="550" class="Symbol">→</a> <a id="552" href="foundation.sequences.html#369" class="Function">sequence</a> <a id="561" href="foundation.sequences.html#516" class="Bound">B</a>
<a id="563" href="foundation.sequences.html#470" class="Function">map-sequence</a> <a id="576" href="foundation.sequences.html#576" class="Bound">f</a> <a id="578" href="foundation.sequences.html#578" class="Bound">a</a> <a id="580" class="Symbol">=</a> <a id="582" href="foundation.sequences.html#576" class="Bound">f</a> <a id="584" href="foundation-core.functions.html#420" class="Function Operator">∘</a> <a id="586" href="foundation.sequences.html#578" class="Bound">a</a>
</pre>