---
title: Discrete fields
---

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a> <a id="127" class="Keyword">where</a>

<a id="134" class="Keyword">open</a> <a id="139" class="Keyword">import</a> <a id="146" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a> <a id="184" class="Keyword">using</a>
  <a id="192" class="Symbol">(</a> <a id="194" href="commutative-algebra.commutative-rings.html#1043" class="Function">Commutative-Ring</a><a id="210" class="Symbol">;</a> <a id="212" href="commutative-algebra.commutative-rings.html#1205" class="Function">ring-Commutative-Ring</a><a id="233" class="Symbol">)</a>

<a id="236" class="Keyword">open</a> <a id="241" class="Keyword">import</a> <a id="248" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="275" class="Keyword">using</a> <a id="281" class="Symbol">(</a><a id="282" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="287" class="Symbol">;</a> <a id="289" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="291" class="Symbol">)</a>

<a id="294" class="Keyword">open</a> <a id="299" class="Keyword">import</a> <a id="306" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a> <a id="333" class="Keyword">using</a> <a id="339" class="Symbol">(</a><a id="340" href="ring-theory.division-rings.html#673" class="Function">is-division-Ring</a><a id="356" class="Symbol">)</a>
</pre>
## Idea

A discrete field is a commutative division ring. They are called discrete, because only nonzero elements are assumed to be invertible.

## Definition

<pre class="Agda"><a id="is-discrete-field-Commutative-Ring"></a><a id="531" href="commutative-algebra.discrete-fields.html#531" class="Function">is-discrete-field-Commutative-Ring</a> <a id="566" class="Symbol">:</a>
  <a id="570" class="Symbol">{</a> <a id="572" href="commutative-algebra.discrete-fields.html#572" class="Bound">l</a> <a id="574" class="Symbol">:</a> <a id="576" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="581" class="Symbol">}</a> <a id="583" class="Symbol">→</a> <a id="585" href="commutative-algebra.commutative-rings.html#1043" class="Function">Commutative-Ring</a> <a id="602" href="commutative-algebra.discrete-fields.html#572" class="Bound">l</a> <a id="604" class="Symbol">→</a> <a id="606" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="609" href="commutative-algebra.discrete-fields.html#572" class="Bound">l</a>
<a id="611" href="commutative-algebra.discrete-fields.html#531" class="Function">is-discrete-field-Commutative-Ring</a> <a id="646" href="commutative-algebra.discrete-fields.html#646" class="Bound">R</a> <a id="648" class="Symbol">=</a>
  <a id="652" href="ring-theory.division-rings.html#673" class="Function">is-division-Ring</a> <a id="669" class="Symbol">(</a><a id="670" href="commutative-algebra.commutative-rings.html#1205" class="Function">ring-Commutative-Ring</a> <a id="692" href="commutative-algebra.discrete-fields.html#646" class="Bound">R</a><a id="693" class="Symbol">)</a>
</pre>