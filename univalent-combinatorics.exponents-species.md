---
title: Exponents of species
---

<pre class="Agda"><a id="46" class="Symbol">{-#</a> <a id="50" class="Keyword">OPTIONS</a> <a id="58" class="Pragma">--without-K</a> <a id="70" class="Pragma">--exact-split</a> <a id="84" class="Symbol">#-}</a>

<a id="89" class="Keyword">module</a> <a id="96" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a> <a id="138" class="Keyword">where</a>

<a id="145" class="Keyword">open</a> <a id="150" class="Keyword">import</a> <a id="157" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="192" class="Keyword">open</a> <a id="197" class="Keyword">import</a> <a id="204" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="231" class="Keyword">open</a> <a id="236" class="Keyword">import</a> <a id="243" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="275" class="Keyword">open</a> <a id="280" class="Keyword">import</a> <a id="287" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="311" class="Keyword">open</a> <a id="316" class="Keyword">import</a> <a id="323" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a> 
<a id="365" class="Keyword">open</a> <a id="370" class="Keyword">import</a> <a id="377" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="405" class="Keyword">open</a> <a id="410" class="Keyword">import</a> <a id="417" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="454" class="Keyword">open</a> <a id="459" class="Keyword">import</a> <a id="466" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="508" class="Keyword">open</a> <a id="513" class="Keyword">import</a> <a id="520" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
</pre>
## Idea

The exponent of two species `F` and `G` is the pointwise exponent

## Definition

### Exponents of species

<pre class="Agda"><a id="function-species"></a><a id="682" href="univalent-combinatorics.exponents-species.html#682" class="Function">function-species</a> <a id="699" class="Symbol">:</a> <a id="701" class="Symbol">{</a><a id="702" href="univalent-combinatorics.exponents-species.html#702" class="Bound">l1</a> <a id="705" href="univalent-combinatorics.exponents-species.html#705" class="Bound">l2</a> <a id="708" class="Symbol">:</a> <a id="710" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="715" class="Symbol">}</a> <a id="717" class="Symbol">→</a> <a id="719" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="727" href="univalent-combinatorics.exponents-species.html#702" class="Bound">l1</a> <a id="730" class="Symbol">→</a> <a id="732" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="740" href="univalent-combinatorics.exponents-species.html#705" class="Bound">l2</a> <a id="743" class="Symbol">→</a> <a id="745" href="univalent-combinatorics.finite-types.html#4913" class="Function">𝔽</a> <a id="747" class="Symbol">→</a> <a id="749" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="752" class="Symbol">(</a><a id="753" href="univalent-combinatorics.exponents-species.html#702" class="Bound">l1</a> <a id="756" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="758" href="univalent-combinatorics.exponents-species.html#705" class="Bound">l2</a><a id="760" class="Symbol">)</a>
<a id="762" href="univalent-combinatorics.exponents-species.html#682" class="Function">function-species</a> <a id="779" href="univalent-combinatorics.exponents-species.html#779" class="Bound">F</a> <a id="781" href="univalent-combinatorics.exponents-species.html#781" class="Bound">G</a> <a id="783" href="univalent-combinatorics.exponents-species.html#783" class="Bound">X</a> <a id="785" class="Symbol">=</a> <a id="787" href="univalent-combinatorics.exponents-species.html#779" class="Bound">F</a> <a id="789" href="univalent-combinatorics.exponents-species.html#783" class="Bound">X</a> <a id="791" class="Symbol">→</a> <a id="793" href="univalent-combinatorics.exponents-species.html#781" class="Bound">G</a> <a id="795" href="univalent-combinatorics.exponents-species.html#783" class="Bound">X</a>
</pre>