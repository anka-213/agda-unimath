---
title: The invariant basis property of rings
---

<pre class="Agda"><a id="63" class="Symbol">{-#</a> <a id="67" class="Keyword">OPTIONS</a> <a id="75" class="Pragma">--without-K</a> <a id="87" class="Pragma">--exact-split</a> <a id="101" class="Symbol">#-}</a>

<a id="106" class="Keyword">module</a> <a id="113" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a> <a id="156" class="Keyword">where</a>

<a id="163" class="Keyword">open</a> <a id="168" class="Keyword">import</a> <a id="175" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="217" class="Keyword">open</a> <a id="222" class="Keyword">import</a> <a id="229" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="255" class="Keyword">open</a> <a id="260" class="Keyword">import</a> <a id="267" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="295" class="Keyword">open</a> <a id="300" class="Keyword">import</a> <a id="307" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="344" class="Keyword">open</a> <a id="349" class="Keyword">import</a> <a id="356" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="387" class="Keyword">open</a> <a id="392" class="Keyword">import</a> <a id="399" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>

<a id="418" class="Keyword">open</a> <a id="423" class="Keyword">import</a> <a id="430" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Idea

A ring R is said to satisfy the invariant basis property if `R^m ≅ R^n` implies `m = n` for any two natural numbers `m` and `n`.

## Definition

<pre class="Agda"><a id="invariant-basis-property-Ring"></a><a id="643" href="ring-theory.invariant-basis-property-rings.html#643" class="Function">invariant-basis-property-Ring</a> <a id="673" class="Symbol">:</a>
  <a id="677" class="Symbol">{</a><a id="678" href="ring-theory.invariant-basis-property-rings.html#678" class="Bound">l1</a> <a id="681" class="Symbol">:</a> <a id="683" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="688" class="Symbol">}</a> <a id="690" class="Symbol">→</a> <a id="692" href="ring-theory.rings.html#2466" class="Function">Ring</a> <a id="697" href="ring-theory.invariant-basis-property-rings.html#678" class="Bound">l1</a> <a id="700" class="Symbol">→</a> <a id="702" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="705" href="ring-theory.invariant-basis-property-rings.html#678" class="Bound">l1</a>
<a id="708" href="ring-theory.invariant-basis-property-rings.html#643" class="Function">invariant-basis-property-Ring</a> <a id="738" href="ring-theory.invariant-basis-property-rings.html#738" class="Bound">R</a> <a id="740" class="Symbol">=</a>
  <a id="744" class="Symbol">(</a><a id="745" href="ring-theory.invariant-basis-property-rings.html#745" class="Bound">m</a> <a id="747" href="ring-theory.invariant-basis-property-rings.html#747" class="Bound">n</a> <a id="749" class="Symbol">:</a> <a id="751" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="752" class="Symbol">)</a> <a id="754" class="Symbol">→</a>
  <a id="758" href="ring-theory.isomorphisms-rings.html#5885" class="Function">iso-Ring</a> <a id="767" class="Symbol">(</a><a id="768" href="ring-theory.dependent-products-rings.html#4328" class="Function">Π-Ring</a> <a id="775" class="Symbol">{</a><a id="776" class="Argument">I</a> <a id="778" class="Symbol">=</a> <a id="780" href="univalent-combinatorics.standard-finite-types.html#2149" class="Function">Fin</a> <a id="784" href="ring-theory.invariant-basis-property-rings.html#745" class="Bound">m</a><a id="785" class="Symbol">}</a> <a id="787" class="Symbol">(λ</a> <a id="790" href="ring-theory.invariant-basis-property-rings.html#790" class="Bound">i</a> <a id="792" class="Symbol">→</a> <a id="794" href="ring-theory.invariant-basis-property-rings.html#738" class="Bound">R</a><a id="795" class="Symbol">))</a> <a id="798" class="Symbol">(</a><a id="799" href="ring-theory.dependent-products-rings.html#4328" class="Function">Π-Ring</a> <a id="806" class="Symbol">{</a><a id="807" class="Argument">I</a> <a id="809" class="Symbol">=</a> <a id="811" href="univalent-combinatorics.standard-finite-types.html#2149" class="Function">Fin</a> <a id="815" href="ring-theory.invariant-basis-property-rings.html#747" class="Bound">n</a><a id="816" class="Symbol">}</a> <a id="818" class="Symbol">(λ</a> <a id="821" href="ring-theory.invariant-basis-property-rings.html#821" class="Bound">i</a> <a id="823" class="Symbol">→</a> <a id="825" href="ring-theory.invariant-basis-property-rings.html#738" class="Bound">R</a><a id="826" class="Symbol">))</a> <a id="829" class="Symbol">→</a>
  <a id="833" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="836" href="ring-theory.invariant-basis-property-rings.html#745" class="Bound">m</a> <a id="838" href="ring-theory.invariant-basis-property-rings.html#747" class="Bound">n</a>
</pre>