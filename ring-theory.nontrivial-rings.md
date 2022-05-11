---
title: Nontrivial rings
---

<pre class="Agda"><a id="42" class="Symbol">{-#</a> <a id="46" class="Keyword">OPTIONS</a> <a id="54" class="Pragma">--without-K</a> <a id="66" class="Pragma">--exact-split</a> <a id="80" class="Symbol">#-}</a>

<a id="85" class="Keyword">module</a> <a id="92" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a> <a id="121" class="Keyword">where</a>

<a id="128" class="Keyword">open</a> <a id="133" class="Keyword">import</a> <a id="140" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="166" class="Keyword">using</a> <a id="172" class="Symbol">(</a><a id="173" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="175" class="Symbol">)</a>
<a id="177" class="Keyword">open</a> <a id="182" class="Keyword">import</a> <a id="189" href="foundation.negation.html" class="Module">foundation.negation</a> <a id="209" class="Keyword">using</a> <a id="215" class="Symbol">(</a><a id="216" href="foundation-core.negation.html#452" class="Function">¬</a><a id="217" class="Symbol">)</a>
<a id="219" class="Keyword">open</a> <a id="224" class="Keyword">import</a> <a id="231" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="258" class="Keyword">using</a> <a id="264" class="Symbol">(</a><a id="265" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="270" class="Symbol">;</a> <a id="272" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="274" class="Symbol">)</a>

<a id="277" class="Keyword">open</a> <a id="282" class="Keyword">import</a> <a id="289" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="307" class="Keyword">using</a> <a id="313" class="Symbol">(</a><a id="314" href="ring-theory.rings.html#2466" class="Function">Ring</a><a id="318" class="Symbol">;</a> <a id="320" href="ring-theory.rings.html#5102" class="Function">zero-Ring</a><a id="329" class="Symbol">;</a> <a id="331" href="ring-theory.rings.html#7892" class="Function">one-Ring</a><a id="339" class="Symbol">)</a>
</pre>
## Idea

Nontrivial rings are rings in which `0 ≠ 1`.

## Definition

<pre class="Agda"><a id="is-nontrivial-Ring"></a><a id="424" href="ring-theory.nontrivial-rings.html#424" class="Function">is-nontrivial-Ring</a> <a id="443" class="Symbol">:</a>
  <a id="447" class="Symbol">{</a> <a id="449" href="ring-theory.nontrivial-rings.html#449" class="Bound">l</a> <a id="451" class="Symbol">:</a> <a id="453" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="458" class="Symbol">}</a> <a id="460" class="Symbol">→</a> <a id="462" href="ring-theory.rings.html#2466" class="Function">Ring</a> <a id="467" href="ring-theory.nontrivial-rings.html#449" class="Bound">l</a> <a id="469" class="Symbol">→</a> <a id="471" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="474" href="ring-theory.nontrivial-rings.html#449" class="Bound">l</a>
<a id="476" href="ring-theory.nontrivial-rings.html#424" class="Function">is-nontrivial-Ring</a> <a id="495" href="ring-theory.nontrivial-rings.html#495" class="Bound">R</a> <a id="497" class="Symbol">=</a> <a id="499" href="foundation-core.negation.html#452" class="Function">¬</a> <a id="501" class="Symbol">(</a><a id="502" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="505" class="Symbol">(</a><a id="506" href="ring-theory.rings.html#5102" class="Function">zero-Ring</a> <a id="516" href="ring-theory.nontrivial-rings.html#495" class="Bound">R</a><a id="517" class="Symbol">)</a> <a id="519" class="Symbol">(</a><a id="520" href="ring-theory.rings.html#7892" class="Function">one-Ring</a> <a id="529" href="ring-theory.nontrivial-rings.html#495" class="Bound">R</a><a id="530" class="Symbol">))</a>
</pre>