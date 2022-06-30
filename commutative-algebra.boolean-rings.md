---
title: Boolean rings
---

<pre class="Agda"><a id="39" class="Symbol">{-#</a> <a id="43" class="Keyword">OPTIONS</a> <a id="51" class="Pragma">--without-K</a> <a id="63" class="Pragma">--exact-split</a> <a id="77" class="Symbol">#-}</a>

<a id="82" class="Keyword">module</a> <a id="89" href="commutative-algebra.boolean-rings.html" class="Module">commutative-algebra.boolean-rings</a> <a id="123" class="Keyword">where</a>

<a id="130" class="Keyword">open</a> <a id="135" class="Keyword">import</a> <a id="142" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>

<a id="181" class="Keyword">open</a> <a id="186" class="Keyword">import</a> <a id="193" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="225" class="Keyword">open</a> <a id="230" class="Keyword">import</a> <a id="237" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="265" class="Keyword">open</a> <a id="270" class="Keyword">import</a> <a id="277" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
</pre>
## Idea

A boolean ring is a commutative ring in wich every element is idempotent.

## Definition

<pre class="Agda"><a id="is-boolean-Commutative-Ring"></a><a id="427" href="commutative-algebra.boolean-rings.html#427" class="Function">is-boolean-Commutative-Ring</a> <a id="455" class="Symbol">:</a>
  <a id="459" class="Symbol">{</a><a id="460" href="commutative-algebra.boolean-rings.html#460" class="Bound">l</a> <a id="462" class="Symbol">:</a> <a id="464" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="469" class="Symbol">}</a> <a id="471" class="Symbol">(</a><a id="472" href="commutative-algebra.boolean-rings.html#472" class="Bound">R</a> <a id="474" class="Symbol">:</a> <a id="476" href="commutative-algebra.commutative-rings.html#1514" class="Function">Commutative-Ring</a> <a id="493" href="commutative-algebra.boolean-rings.html#460" class="Bound">l</a><a id="494" class="Symbol">)</a> <a id="496" class="Symbol">→</a> <a id="498" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="501" href="commutative-algebra.boolean-rings.html#460" class="Bound">l</a>
<a id="503" href="commutative-algebra.boolean-rings.html#427" class="Function">is-boolean-Commutative-Ring</a> <a id="531" href="commutative-algebra.boolean-rings.html#531" class="Bound">R</a> <a id="533" class="Symbol">=</a>
  <a id="537" class="Symbol">(</a><a id="538" href="commutative-algebra.boolean-rings.html#538" class="Bound">x</a> <a id="540" class="Symbol">:</a> <a id="542" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="564" href="commutative-algebra.boolean-rings.html#531" class="Bound">R</a><a id="565" class="Symbol">)</a> <a id="567" class="Symbol">→</a>
  <a id="571" href="ring-theory.idempotent-elements-rings.html#613" class="Function">is-idempotent-element-Ring</a> <a id="598" class="Symbol">(</a><a id="599" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="621" href="commutative-algebra.boolean-rings.html#531" class="Bound">R</a><a id="622" class="Symbol">)</a> <a id="624" href="commutative-algebra.boolean-rings.html#538" class="Bound">x</a>

<a id="Boolean-Ring"></a><a id="627" href="commutative-algebra.boolean-rings.html#627" class="Function">Boolean-Ring</a> <a id="640" class="Symbol">:</a> <a id="642" class="Symbol">(</a><a id="643" href="commutative-algebra.boolean-rings.html#643" class="Bound">l</a> <a id="645" class="Symbol">:</a> <a id="647" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="652" class="Symbol">)</a> <a id="654" class="Symbol">→</a> <a id="656" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="659" class="Symbol">(</a><a id="660" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="665" href="commutative-algebra.boolean-rings.html#643" class="Bound">l</a><a id="666" class="Symbol">)</a>
<a id="668" href="commutative-algebra.boolean-rings.html#627" class="Function">Boolean-Ring</a> <a id="681" href="commutative-algebra.boolean-rings.html#681" class="Bound">l</a> <a id="683" class="Symbol">=</a> <a id="685" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="687" class="Symbol">(</a><a id="688" href="commutative-algebra.commutative-rings.html#1514" class="Function">Commutative-Ring</a> <a id="705" href="commutative-algebra.boolean-rings.html#681" class="Bound">l</a><a id="706" class="Symbol">)</a> <a id="708" href="commutative-algebra.boolean-rings.html#427" class="Function">is-boolean-Commutative-Ring</a>

<a id="737" class="Keyword">module</a> <a id="744" href="commutative-algebra.boolean-rings.html#744" class="Module">_</a>
  <a id="748" class="Symbol">{</a><a id="749" href="commutative-algebra.boolean-rings.html#749" class="Bound">l</a> <a id="751" class="Symbol">:</a> <a id="753" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="758" class="Symbol">}</a> <a id="760" class="Symbol">(</a><a id="761" href="commutative-algebra.boolean-rings.html#761" class="Bound">R</a> <a id="763" class="Symbol">:</a> <a id="765" href="commutative-algebra.boolean-rings.html#627" class="Function">Boolean-Ring</a> <a id="778" href="commutative-algebra.boolean-rings.html#749" class="Bound">l</a><a id="779" class="Symbol">)</a>
  <a id="783" class="Keyword">where</a>

  <a id="792" href="commutative-algebra.boolean-rings.html#792" class="Function">commutative-ring-Boolean-Ring</a> <a id="822" class="Symbol">:</a> <a id="824" href="commutative-algebra.commutative-rings.html#1514" class="Function">Commutative-Ring</a> <a id="841" href="commutative-algebra.boolean-rings.html#749" class="Bound">l</a>
  <a id="845" href="commutative-algebra.boolean-rings.html#792" class="Function">commutative-ring-Boolean-Ring</a> <a id="875" class="Symbol">=</a> <a id="877" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="881" href="commutative-algebra.boolean-rings.html#761" class="Bound">R</a>
</pre>