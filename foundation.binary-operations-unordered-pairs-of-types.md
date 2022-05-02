---
title: Binary operations on unordered pairs of types
---

<pre class="Agda"><a id="71" class="Symbol">{-#</a> <a id="75" class="Keyword">OPTIONS</a> <a id="83" class="Pragma">--without-K</a> <a id="95" class="Pragma">--exact-split</a> <a id="109" class="Symbol">#-}</a>

<a id="114" class="Keyword">module</a> <a id="121" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a> <a id="175" class="Keyword">where</a>

<a id="182" class="Keyword">open</a> <a id="187" class="Keyword">import</a> <a id="194" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="239" class="Keyword">open</a> <a id="244" class="Keyword">import</a> <a id="251" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="278" class="Keyword">open</a> <a id="283" class="Keyword">import</a> <a id="290" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
</pre>
## Idea

A binary operation on an unordered pair of types A indexed by a 2-element type I is a map `((i : I) → A i) →  B`.

## Definition

<pre class="Agda"><a id="binary-operation-unordered-pair-types"></a><a id="469" href="foundation.binary-operations-unordered-pairs-of-types.html#469" class="Function">binary-operation-unordered-pair-types</a> <a id="507" class="Symbol">:</a>
  <a id="511" class="Symbol">{</a><a id="512" href="foundation.binary-operations-unordered-pairs-of-types.html#512" class="Bound">l1</a> <a id="515" href="foundation.binary-operations-unordered-pairs-of-types.html#515" class="Bound">l2</a> <a id="518" class="Symbol">:</a> <a id="520" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="525" class="Symbol">}</a> <a id="527" class="Symbol">(</a><a id="528" href="foundation.binary-operations-unordered-pairs-of-types.html#528" class="Bound">A</a> <a id="530" class="Symbol">:</a> <a id="532" href="foundation.unordered-pairs.html#2381" class="Function">unordered-pair</a> <a id="547" class="Symbol">(</a><a id="548" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="551" href="foundation.binary-operations-unordered-pairs-of-types.html#512" class="Bound">l1</a><a id="553" class="Symbol">))</a> <a id="556" class="Symbol">(</a><a id="557" href="foundation.binary-operations-unordered-pairs-of-types.html#557" class="Bound">B</a> <a id="559" class="Symbol">:</a> <a id="561" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="564" href="foundation.binary-operations-unordered-pairs-of-types.html#515" class="Bound">l2</a><a id="566" class="Symbol">)</a> <a id="568" class="Symbol">→</a> <a id="570" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="573" class="Symbol">(</a><a id="574" href="foundation.binary-operations-unordered-pairs-of-types.html#512" class="Bound">l1</a> <a id="577" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="579" href="foundation.binary-operations-unordered-pairs-of-types.html#515" class="Bound">l2</a><a id="581" class="Symbol">)</a>
<a id="583" href="foundation.binary-operations-unordered-pairs-of-types.html#469" class="Function">binary-operation-unordered-pair-types</a> <a id="621" href="foundation.binary-operations-unordered-pairs-of-types.html#621" class="Bound">A</a> <a id="623" href="foundation.binary-operations-unordered-pairs-of-types.html#623" class="Bound">B</a> <a id="625" class="Symbol">=</a> <a id="627" href="foundation.products-unordered-pairs-of-types.html#1091" class="Function">product-unordered-pair-types</a> <a id="656" href="foundation.binary-operations-unordered-pairs-of-types.html#621" class="Bound">A</a> <a id="658" class="Symbol">→</a> <a id="660" href="foundation.binary-operations-unordered-pairs-of-types.html#623" class="Bound">B</a>
</pre>