---
title: Discrete fields
---

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="ring-theory.discrete-fields.html" class="Module">ring-theory.discrete-fields</a> <a id="119" class="Keyword">where</a>

<a id="126" class="Keyword">open</a> <a id="131" class="Keyword">import</a> <a id="138" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="165" class="Keyword">using</a> <a id="171" class="Symbol">(</a><a id="172" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="177" class="Symbol">;</a> <a id="179" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="181" class="Symbol">)</a>

<a id="184" class="Keyword">open</a> <a id="189" class="Keyword">import</a> <a id="196" href="ring-theory.commutative-rings.html" class="Module">ring-theory.commutative-rings</a> <a id="226" class="Keyword">using</a> <a id="232" class="Symbol">(</a><a id="233" href="ring-theory.commutative-rings.html#1035" class="Function">Comm-Ring</a><a id="242" class="Symbol">;</a> <a id="244" href="ring-theory.commutative-rings.html#1176" class="Function">ring-Comm-Ring</a><a id="258" class="Symbol">)</a>
<a id="260" class="Keyword">open</a> <a id="265" class="Keyword">import</a> <a id="272" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a> <a id="299" class="Keyword">using</a> <a id="305" class="Symbol">(</a><a id="306" href="ring-theory.division-rings.html#662" class="Function">is-division-Ring</a><a id="322" class="Symbol">)</a>
</pre>
## Idea

A discrete field is a commutative division ring. They are called discrete, because only nonzero elements are assumed to be invertible.

## Definition

<pre class="Agda"><a id="is-discrete-field-Comm-Ring"></a><a id="497" href="ring-theory.discrete-fields.html#497" class="Function">is-discrete-field-Comm-Ring</a> <a id="525" class="Symbol">:</a>
  <a id="529" class="Symbol">{</a> <a id="531" href="ring-theory.discrete-fields.html#531" class="Bound">l</a> <a id="533" class="Symbol">:</a> <a id="535" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="540" class="Symbol">}</a> <a id="542" class="Symbol">→</a> <a id="544" href="ring-theory.commutative-rings.html#1035" class="Function">Comm-Ring</a> <a id="554" href="ring-theory.discrete-fields.html#531" class="Bound">l</a> <a id="556" class="Symbol">→</a> <a id="558" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="561" href="ring-theory.discrete-fields.html#531" class="Bound">l</a>
<a id="563" href="ring-theory.discrete-fields.html#497" class="Function">is-discrete-field-Comm-Ring</a> <a id="591" href="ring-theory.discrete-fields.html#591" class="Bound">R</a> <a id="593" class="Symbol">=</a> <a id="595" href="ring-theory.division-rings.html#662" class="Function">is-division-Ring</a> <a id="612" class="Symbol">(</a><a id="613" href="ring-theory.commutative-rings.html#1176" class="Function">ring-Comm-Ring</a> <a id="628" href="ring-theory.discrete-fields.html#591" class="Bound">R</a><a id="629" class="Symbol">)</a>
</pre>