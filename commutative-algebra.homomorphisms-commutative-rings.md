---
title: Homomorphisms of commutative rings
---

<pre class="Agda"><a id="60" class="Symbol">{-#</a> <a id="64" class="Keyword">OPTIONS</a> <a id="72" class="Pragma">--without-K</a> <a id="84" class="Pragma">--exact-split</a> <a id="98" class="Symbol">#-}</a>

<a id="103" class="Keyword">module</a> <a id="110" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a> <a id="162" class="Keyword">where</a>

<a id="169" class="Keyword">open</a> <a id="174" class="Keyword">import</a> <a id="181" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a> <a id="219" class="Keyword">using</a>
  <a id="227" class="Symbol">(</a> <a id="229" href="commutative-algebra.commutative-rings.html#1043" class="Function">Commutative-Ring</a><a id="245" class="Symbol">;</a> <a id="247" href="commutative-algebra.commutative-rings.html#1205" class="Function">ring-Commutative-Ring</a><a id="268" class="Symbol">)</a>

<a id="271" class="Keyword">open</a> <a id="276" class="Keyword">import</a> <a id="283" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="310" class="Keyword">using</a> <a id="316" class="Symbol">(</a><a id="317" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="322" class="Symbol">;</a> <a id="324" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="326" class="Symbol">;</a> <a id="328" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="331" class="Symbol">)</a>

<a id="334" class="Keyword">open</a> <a id="339" class="Keyword">import</a> <a id="346" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a> <a id="378" class="Keyword">using</a> <a id="384" class="Symbol">(</a><a id="385" href="ring-theory.homomorphisms-rings.html#3835" class="Function">type-hom-Ring</a><a id="398" class="Symbol">)</a>
</pre>
## Idea

A morphism of commutative rings is just a morphism between their underlying rings.

## Definition

<pre class="Agda"><a id="type-hom-Commutative-Ring"></a><a id="521" href="commutative-algebra.homomorphisms-commutative-rings.html#521" class="Function">type-hom-Commutative-Ring</a> <a id="547" class="Symbol">:</a>
  <a id="551" class="Symbol">{</a> <a id="553" href="commutative-algebra.homomorphisms-commutative-rings.html#553" class="Bound">l1</a> <a id="556" href="commutative-algebra.homomorphisms-commutative-rings.html#556" class="Bound">l2</a> <a id="559" class="Symbol">:</a> <a id="561" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="566" class="Symbol">}</a> <a id="568" class="Symbol">→</a> <a id="570" href="commutative-algebra.commutative-rings.html#1043" class="Function">Commutative-Ring</a> <a id="587" href="commutative-algebra.homomorphisms-commutative-rings.html#553" class="Bound">l1</a> <a id="590" class="Symbol">→</a> <a id="592" href="commutative-algebra.commutative-rings.html#1043" class="Function">Commutative-Ring</a> <a id="609" href="commutative-algebra.homomorphisms-commutative-rings.html#556" class="Bound">l2</a> <a id="612" class="Symbol">→</a> <a id="614" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="617" class="Symbol">(</a><a id="618" href="commutative-algebra.homomorphisms-commutative-rings.html#553" class="Bound">l1</a> <a id="621" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="623" href="commutative-algebra.homomorphisms-commutative-rings.html#556" class="Bound">l2</a><a id="625" class="Symbol">)</a>
<a id="627" href="commutative-algebra.homomorphisms-commutative-rings.html#521" class="Function">type-hom-Commutative-Ring</a> <a id="653" href="commutative-algebra.homomorphisms-commutative-rings.html#653" class="Bound">R1</a> <a id="656" href="commutative-algebra.homomorphisms-commutative-rings.html#656" class="Bound">R2</a> <a id="659" class="Symbol">=</a>
  <a id="663" href="ring-theory.homomorphisms-rings.html#3835" class="Function">type-hom-Ring</a> <a id="677" class="Symbol">(</a><a id="678" href="commutative-algebra.commutative-rings.html#1205" class="Function">ring-Commutative-Ring</a> <a id="700" href="commutative-algebra.homomorphisms-commutative-rings.html#653" class="Bound">R1</a><a id="702" class="Symbol">)</a> <a id="704" class="Symbol">(</a><a id="705" href="commutative-algebra.commutative-rings.html#1205" class="Function">ring-Commutative-Ring</a> <a id="727" href="commutative-algebra.homomorphisms-commutative-rings.html#656" class="Bound">R2</a><a id="729" class="Symbol">)</a>
</pre>