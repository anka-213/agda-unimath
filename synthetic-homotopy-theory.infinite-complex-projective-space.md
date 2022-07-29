---
title: The infinite complex projective space
---

<pre class="Agda"><a id="63" class="Symbol">{-#</a> <a id="67" class="Keyword">OPTIONS</a> <a id="75" class="Pragma">--without-K</a> <a id="87" class="Pragma">--exact-split</a> <a id="101" class="Symbol">#-}</a>

<a id="106" class="Keyword">module</a> <a id="113" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a> <a id="173" class="Keyword">where</a>

<a id="180" class="Keyword">open</a> <a id="185" class="Keyword">import</a> <a id="192" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="224" class="Keyword">open</a> <a id="229" class="Keyword">import</a> <a id="236" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="260" class="Keyword">open</a> <a id="265" class="Keyword">import</a> <a id="272" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="299" class="Keyword">open</a> <a id="304" class="Keyword">import</a> <a id="311" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="339" class="Keyword">open</a> <a id="344" class="Keyword">import</a> <a id="351" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
</pre>
## Definitions

### ℂP∞ as the 1-connected component of the universe at the circle

<pre class="Agda"><a id="ℂP∞"></a><a id="481" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#481" class="Function">ℂP∞</a> <a id="485" class="Symbol">:</a> <a id="487" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="490" class="Symbol">(</a><a id="491" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="496" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="501" class="Symbol">)</a>
<a id="503" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#481" class="Function">ℂP∞</a> <a id="507" class="Symbol">=</a> <a id="509" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="511" class="Symbol">(</a><a id="512" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="515" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="520" class="Symbol">)</a> <a id="522" class="Symbol">(λ</a> <a id="525" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#525" class="Bound">X</a> <a id="527" class="Symbol">→</a> <a id="529" href="foundation.set-truncations.html#4010" class="Function">type-trunc-Set</a> <a id="544" class="Symbol">(</a><a id="545" href="synthetic-homotopy-theory.circle.html#1237" class="Postulate">𝕊¹</a> <a id="548" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="550" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#525" class="Bound">X</a><a id="551" class="Symbol">))</a>

<a id="pt-ℂP∞"></a><a id="555" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#555" class="Function">pt-ℂP∞</a> <a id="562" class="Symbol">:</a> <a id="564" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#481" class="Function">ℂP∞</a>
<a id="568" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="572" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#555" class="Function">pt-ℂP∞</a> <a id="579" class="Symbol">=</a> <a id="581" href="synthetic-homotopy-theory.circle.html#1237" class="Postulate">𝕊¹</a>
<a id="584" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="588" href="synthetic-homotopy-theory.infinite-complex-projective-space.html#555" class="Function">pt-ℂP∞</a> <a id="595" class="Symbol">=</a> <a id="597" href="foundation.set-truncations.html#4277" class="Function">unit-trunc-Set</a> <a id="612" href="foundation-core.equivalences.html#2494" class="Function">id-equiv</a>
</pre>
### ℂP∞ as the 2-truncation of the 2-sphere
