---
title: Discrete fields
---

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a> <a id="127" class="Keyword">where</a>

<a id="134" class="Keyword">open</a> <a id="139" class="Keyword">import</a> <a id="146" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a> <a id="184" class="Keyword">using</a>
  <a id="192" class="Symbol">(</a> <a id="194" href="commutative-algebra.commutative-rings.html#1043" class="Function">Comm-Ring</a><a id="203" class="Symbol">;</a> <a id="205" href="commutative-algebra.commutative-rings.html#1184" class="Function">ring-Comm-Ring</a><a id="219" class="Symbol">)</a>

<a id="222" class="Keyword">open</a> <a id="227" class="Keyword">import</a> <a id="234" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="261" class="Keyword">using</a> <a id="267" class="Symbol">(</a><a id="268" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="273" class="Symbol">;</a> <a id="275" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="277" class="Symbol">)</a>

<a id="280" class="Keyword">open</a> <a id="285" class="Keyword">import</a> <a id="292" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a> <a id="319" class="Keyword">using</a> <a id="325" class="Symbol">(</a><a id="326" href="ring-theory.division-rings.html#662" class="Function">is-division-Ring</a><a id="342" class="Symbol">)</a>
</pre>
## Idea

A discrete field is a commutative division ring. They are called discrete, because only nonzero elements are assumed to be invertible.

## Definition

<pre class="Agda"><a id="is-discrete-field-Comm-Ring"></a><a id="517" href="commutative-algebra.discrete-fields.html#517" class="Function">is-discrete-field-Comm-Ring</a> <a id="545" class="Symbol">:</a>
  <a id="549" class="Symbol">{</a> <a id="551" href="commutative-algebra.discrete-fields.html#551" class="Bound">l</a> <a id="553" class="Symbol">:</a> <a id="555" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="560" class="Symbol">}</a> <a id="562" class="Symbol">→</a> <a id="564" href="commutative-algebra.commutative-rings.html#1043" class="Function">Comm-Ring</a> <a id="574" href="commutative-algebra.discrete-fields.html#551" class="Bound">l</a> <a id="576" class="Symbol">→</a> <a id="578" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="581" href="commutative-algebra.discrete-fields.html#551" class="Bound">l</a>
<a id="583" href="commutative-algebra.discrete-fields.html#517" class="Function">is-discrete-field-Comm-Ring</a> <a id="611" href="commutative-algebra.discrete-fields.html#611" class="Bound">R</a> <a id="613" class="Symbol">=</a> <a id="615" href="ring-theory.division-rings.html#662" class="Function">is-division-Ring</a> <a id="632" class="Symbol">(</a><a id="633" href="commutative-algebra.commutative-rings.html#1184" class="Function">ring-Comm-Ring</a> <a id="648" href="commutative-algebra.discrete-fields.html#611" class="Bound">R</a><a id="649" class="Symbol">)</a>
</pre>