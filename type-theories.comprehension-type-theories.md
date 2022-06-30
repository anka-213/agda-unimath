---
title: Comprehension of fibered type theories
---

<pre class="Agda"><a id="64" class="Symbol">{-#</a> <a id="68" class="Keyword">OPTIONS</a> <a id="76" class="Pragma">--without-K</a> <a id="88" class="Pragma">--exact-split</a> <a id="102" class="Pragma">--allow-unsolved-metas</a> <a id="125" class="Pragma">--guardedness</a> <a id="139" class="Symbol">#-}</a>

<a id="144" class="Keyword">module</a> <a id="151" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a> <a id="193" class="Keyword">where</a>

<a id="200" class="Keyword">open</a> <a id="205" class="Keyword">import</a> <a id="212" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="240" class="Keyword">open</a> <a id="245" class="Keyword">import</a> <a id="252" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="290" class="Keyword">open</a> <a id="295" class="Keyword">import</a> <a id="302" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>

<a id="349" class="Keyword">open</a> <a id="354" href="type-theories.dependent-type-theories.html#722" class="Module">dependent</a>
</pre>
## Idea

Given a fibered type theory `S` over `T`, we can form the comprehension type theory `∫ST` analogous to the Grothendieck construction

## Definition

<pre class="Agda"><a id="535" class="Keyword">record</a> <a id="comprehension"></a><a id="542" href="type-theories.comprehension-type-theories.html#542" class="UnsolvedConstraint Record">comprehension</a>
  <a id="558" class="Symbol">{</a><a id="559" href="type-theories.comprehension-type-theories.html#559" class="Bound">l1</a> <a id="562" href="type-theories.comprehension-type-theories.html#562" class="Bound">l2</a> <a id="565" href="type-theories.comprehension-type-theories.html#565" class="Bound">l3</a> <a id="568" href="type-theories.comprehension-type-theories.html#568" class="Bound">l4</a> <a id="571" class="Symbol">:</a> <a id="573" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="578" class="Symbol">}</a> <a id="580" class="Symbol">{</a><a id="581" href="type-theories.comprehension-type-theories.html#581" class="Bound">A</a> <a id="583" class="Symbol">:</a> <a id="585" href="type-theories.dependent-type-theories.html#28238" class="Record">type-theory</a> <a id="597" href="type-theories.comprehension-type-theories.html#559" class="Bound">l1</a> <a id="600" href="type-theories.comprehension-type-theories.html#562" class="Bound">l2</a><a id="602" class="Symbol">}</a>
  <a id="606" class="Symbol">{</a><a id="607" href="type-theories.comprehension-type-theories.html#607" class="Bound">B</a> <a id="609" class="Symbol">:</a> <a id="611" href="type-theories.fibered-dependent-type-theories.html#27254" class="Record">fibered.fibered-type-theory</a> <a id="639" href="type-theories.comprehension-type-theories.html#565" class="Bound">l3</a> <a id="642" href="type-theories.comprehension-type-theories.html#568" class="Bound">l4</a> <a id="645" href="type-theories.comprehension-type-theories.html#581" class="Bound">A</a><a id="646" class="Symbol">}</a> <a id="648" class="Symbol">:</a> <a id="650" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="653" class="Symbol">(</a><a id="654" href="type-theories.comprehension-type-theories.html#559" class="Bound">l1</a> <a id="657" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="659" href="type-theories.comprehension-type-theories.html#562" class="Bound">l2</a> <a id="662" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="664" href="type-theories.comprehension-type-theories.html#565" class="Bound">l3</a> <a id="667" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="669" href="type-theories.comprehension-type-theories.html#568" class="Bound">l4</a><a id="671" class="Symbol">)</a>
  <a id="675" class="Keyword">where</a>
  <a id="683" class="Keyword">coinductive</a>
  <a id="697" class="Keyword">field</a>
    <a id="comprehension.type"></a><a id="707" href="type-theories.comprehension-type-theories.html#707" class="Field">type</a> <a id="712" class="Symbol">:</a> <a id="714" class="UnsolvedMeta Hole">{!!}</a>
    <a id="comprehension.element"></a><a id="723" href="type-theories.comprehension-type-theories.html#723" class="Field">element</a> <a id="731" class="Symbol">:</a> <a id="733" class="UnsolvedMeta Hole">{!!}</a>
    <a id="comprehension.slice"></a><a id="742" href="type-theories.comprehension-type-theories.html#742" class="Field">slice</a> <a id="748" class="Symbol">:</a> <a id="750" class="UnsolvedMeta Hole">{!!}</a>
</pre>