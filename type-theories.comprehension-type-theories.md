---
title: Comprehension of fibered type theories
---

<pre class="Agda"><a id="64" class="Symbol">{-#</a> <a id="68" class="Keyword">OPTIONS</a> <a id="76" class="Pragma">--guardedness</a> <a id="90" class="Symbol">#-}</a>

<a id="95" class="Keyword">module</a> <a id="102" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a> <a id="144" class="Keyword">where</a>

<a id="151" class="Keyword">open</a> <a id="156" class="Keyword">import</a> <a id="163" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="191" class="Keyword">open</a> <a id="196" class="Keyword">import</a> <a id="203" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>

<a id="300" class="Keyword">open</a> <a id="305" href="type-theories.dependent-type-theories.html#673" class="Module">dependent</a>
</pre>
## Idea

Given a fibered type theory `S` over `T`, we can form the comprehension type theory `∫ST` analogous to the Grothendieck construction

## Definition

<pre class="Agda"><a id="486" class="Comment">{-
record comprehension
  {l1 l2 l3 l4 : Level} {A : type-theory l1 l2}
  {B : fibered.fibered-type-theory l3 l4 A} : UU (l1 ⊔ l2 ⊔ l3 ⊔ l4)
  where
  coinductive
  field
    type : {!!}
    element : {!!}
    slice : {!!}
-}</a>
</pre>