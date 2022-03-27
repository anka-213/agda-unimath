# Univalent mathematics in Agda

Welcome to the website of the `agda-unimath` formalization project.

[![build](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml)

<pre class="Agda"><a id="281" class="Symbol">{-#</a> <a id="285" class="Keyword">OPTIONS</a> <a id="293" class="Pragma">--without-K</a> <a id="305" class="Pragma">--exact-split</a> <a id="319" class="Symbol">#-}</a>
</pre>
## Category theory

<pre class="Agda"><a id="356" class="Keyword">open</a> <a id="361" class="Keyword">import</a> <a id="368" href="category-theory.html" class="Module">category-theory</a>
<a id="384" class="Keyword">open</a> <a id="389" class="Keyword">import</a> <a id="396" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="444" class="Keyword">open</a> <a id="449" class="Keyword">import</a> <a id="456" href="category-theory.anafunctors.html" class="Module">category-theory.anafunctors</a>
<a id="484" class="Keyword">open</a> <a id="489" class="Keyword">import</a> <a id="496" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="523" class="Keyword">open</a> <a id="528" class="Keyword">import</a> <a id="535" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="575" class="Keyword">open</a> <a id="580" class="Keyword">import</a> <a id="587" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="636" class="Keyword">open</a> <a id="641" class="Keyword">import</a> <a id="648" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="691" class="Keyword">open</a> <a id="696" class="Keyword">import</a> <a id="703" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="739" class="Keyword">open</a> <a id="744" class="Keyword">import</a> <a id="751" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="796" class="Keyword">open</a> <a id="801" class="Keyword">import</a> <a id="808" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="847" class="Keyword">open</a> <a id="852" class="Keyword">import</a> <a id="859" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="930" class="Keyword">open</a> <a id="935" class="Keyword">import</a> <a id="942" href="category-theory.initial-objects-precategories.html" class="Module">category-theory.initial-objects-precategories</a>
<a id="988" class="Keyword">open</a> <a id="993" class="Keyword">import</a> <a id="1000" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="1040" class="Keyword">open</a> <a id="1045" class="Keyword">import</a> <a id="1052" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="1101" class="Keyword">open</a> <a id="1106" class="Keyword">import</a> <a id="1113" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="1156" class="Keyword">open</a> <a id="1161" class="Keyword">import</a> <a id="1168" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="1201" class="Keyword">open</a> <a id="1206" class="Keyword">import</a> <a id="1213" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="1249" class="Keyword">open</a> <a id="1254" class="Keyword">import</a> <a id="1261" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="1311" class="Keyword">open</a> <a id="1316" class="Keyword">import</a> <a id="1323" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="1371" class="Keyword">open</a> <a id="1376" class="Keyword">import</a> <a id="1383" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="1440" class="Keyword">open</a> <a id="1445" class="Keyword">import</a> <a id="1452" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="1503" class="Keyword">open</a> <a id="1508" class="Keyword">import</a> <a id="1515" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="1566" class="Keyword">open</a> <a id="1571" class="Keyword">import</a> <a id="1578" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="1638" class="Keyword">open</a> <a id="1643" class="Keyword">import</a> <a id="1650" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="1704" class="Keyword">open</a> <a id="1709" class="Keyword">import</a> <a id="1716" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
<a id="1746" class="Keyword">open</a> <a id="1751" class="Keyword">import</a> <a id="1758" href="category-theory.slice-precategories.html" class="Module">category-theory.slice-precategories</a>
<a id="1794" class="Keyword">open</a> <a id="1799" class="Keyword">import</a> <a id="1806" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="1895" class="Keyword">open</a> <a id="1900" class="Keyword">import</a> <a id="1907" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="1932" class="Keyword">open</a> <a id="1937" class="Keyword">import</a> <a id="1944" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="1993" class="Keyword">open</a> <a id="1998" class="Keyword">import</a> <a id="2005" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="2048" class="Keyword">open</a> <a id="2053" class="Keyword">import</a> <a id="2060" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="2110" class="Keyword">open</a> <a id="2115" class="Keyword">import</a> <a id="2122" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="2168" class="Keyword">open</a> <a id="2173" class="Keyword">import</a> <a id="2180" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="2227" class="Keyword">open</a> <a id="2232" class="Keyword">import</a> <a id="2239" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="2298" class="Keyword">open</a> <a id="2303" class="Keyword">import</a> <a id="2310" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="2351" class="Keyword">open</a> <a id="2356" class="Keyword">import</a> <a id="2363" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="2406" class="Keyword">open</a> <a id="2411" class="Keyword">import</a> <a id="2418" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="2462" class="Keyword">open</a> <a id="2467" class="Keyword">import</a> <a id="2474" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="2519" class="Keyword">open</a> <a id="2524" class="Keyword">import</a> <a id="2531" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="2583" class="Keyword">open</a> <a id="2588" class="Keyword">import</a> <a id="2595" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="2655" class="Keyword">open</a> <a id="2660" class="Keyword">import</a> <a id="2667" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="2708" class="Keyword">open</a> <a id="2713" class="Keyword">import</a> <a id="2720" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="2765" class="Keyword">open</a> <a id="2770" class="Keyword">import</a> <a id="2777" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="2824" class="Keyword">open</a> <a id="2829" class="Keyword">import</a> <a id="2836" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="2879" class="Keyword">open</a> <a id="2884" class="Keyword">import</a> <a id="2891" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="2941" class="Keyword">open</a> <a id="2946" class="Keyword">import</a> <a id="2953" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="3000" class="Keyword">open</a> <a id="3005" class="Keyword">import</a> <a id="3012" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="3069" class="Keyword">open</a> <a id="3074" class="Keyword">import</a> <a id="3081" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="3135" class="Keyword">open</a> <a id="3140" class="Keyword">import</a> <a id="3147" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="3207" class="Keyword">open</a> <a id="3212" class="Keyword">import</a> <a id="3219" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="3262" class="Keyword">open</a> <a id="3267" class="Keyword">import</a> <a id="3274" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="3324" class="Keyword">open</a> <a id="3329" class="Keyword">import</a> <a id="3336" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="3396" class="Keyword">open</a> <a id="3401" class="Keyword">import</a> <a id="3408" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="3457" class="Keyword">open</a> <a id="3462" class="Keyword">import</a> <a id="3469" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="3525" class="Keyword">open</a> <a id="3530" class="Keyword">import</a> <a id="3537" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="3573" class="Keyword">open</a> <a id="3578" class="Keyword">import</a> <a id="3585" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="3629" class="Keyword">open</a> <a id="3634" class="Keyword">import</a> <a id="3641" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="3685" class="Keyword">open</a> <a id="3690" class="Keyword">import</a> <a id="3697" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="3747" class="Keyword">open</a> <a id="3752" class="Keyword">import</a> <a id="3759" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="3805" class="Keyword">open</a> <a id="3810" class="Keyword">import</a> <a id="3817" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="3852" class="Keyword">open</a> <a id="3857" class="Keyword">import</a> <a id="3864" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="3909" class="Keyword">open</a> <a id="3914" class="Keyword">import</a> <a id="3921" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="3979" class="Keyword">open</a> <a id="3984" class="Keyword">import</a> <a id="3991" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="4056" class="Keyword">open</a> <a id="4061" class="Keyword">import</a> <a id="4068" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="4111" class="Keyword">open</a> <a id="4116" class="Keyword">import</a> <a id="4123" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="4177" class="Keyword">open</a> <a id="4182" class="Keyword">import</a> <a id="4189" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="4234" class="Keyword">open</a> <a id="4239" class="Keyword">import</a> <a id="4246" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="4298" class="Keyword">open</a> <a id="4303" class="Keyword">import</a> <a id="4310" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="4368" class="Keyword">open</a> <a id="4373" class="Keyword">import</a> <a id="4380" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="4426" class="Keyword">open</a> <a id="4431" class="Keyword">import</a> <a id="4438" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="4472" class="Keyword">open</a> <a id="4477" class="Keyword">import</a> <a id="4484" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="4529" class="Keyword">open</a> <a id="4534" class="Keyword">import</a> <a id="4541" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="4595" class="Keyword">open</a> <a id="4600" class="Keyword">import</a> <a id="4607" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="4656" class="Keyword">open</a> <a id="4661" class="Keyword">import</a> <a id="4668" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="4709" class="Keyword">open</a> <a id="4714" class="Keyword">import</a> <a id="4721" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="4770" class="Keyword">open</a> <a id="4775" class="Keyword">import</a> <a id="4782" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="4848" class="Keyword">open</a> <a id="4853" class="Keyword">import</a> <a id="4860" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="4904" class="Keyword">open</a> <a id="4909" class="Keyword">import</a> <a id="4916" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="4965" class="Keyword">open</a> <a id="4970" class="Keyword">import</a> <a id="4977" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="5033" class="Keyword">open</a> <a id="5038" class="Keyword">import</a> <a id="5045" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="5086" class="Keyword">open</a> <a id="5091" class="Keyword">import</a> <a id="5098" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="5147" class="Keyword">open</a> <a id="5152" class="Keyword">import</a> <a id="5159" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="5218" class="Keyword">open</a> <a id="5223" class="Keyword">import</a> <a id="5230" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="5269" class="Keyword">open</a> <a id="5274" class="Keyword">import</a> <a id="5281" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="5334" class="Keyword">open</a> <a id="5339" class="Keyword">import</a> <a id="5346" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="5403" class="Keyword">open</a> <a id="5408" class="Keyword">import</a> <a id="5415" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="5457" class="Keyword">open</a> <a id="5462" class="Keyword">import</a> <a id="5469" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="5520" class="Keyword">open</a> <a id="5525" class="Keyword">import</a> <a id="5532" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="5590" class="Keyword">open</a> <a id="5595" class="Keyword">import</a> <a id="5602" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="5666" class="Keyword">open</a> <a id="5671" class="Keyword">import</a> <a id="5678" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="5731" class="Keyword">open</a> <a id="5736" class="Keyword">import</a> <a id="5743" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="5796" class="Keyword">open</a> <a id="5801" class="Keyword">import</a> <a id="5808" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="5869" class="Keyword">open</a> <a id="5874" class="Keyword">import</a> <a id="5881" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="5939" class="Keyword">open</a> <a id="5944" class="Keyword">import</a> <a id="5951" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="6000" class="Keyword">open</a> <a id="6005" class="Keyword">import</a> <a id="6012" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="6056" class="Keyword">open</a> <a id="6061" class="Keyword">import</a> <a id="6068" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="6111" class="Keyword">open</a> <a id="6116" class="Keyword">import</a> <a id="6123" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="6170" class="Keyword">open</a> <a id="6175" class="Keyword">import</a> <a id="6182" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="6243" class="Keyword">open</a> <a id="6248" class="Keyword">import</a> <a id="6255" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="6318" class="Keyword">open</a> <a id="6323" class="Keyword">import</a> <a id="6330" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="6390" class="Keyword">open</a> <a id="6395" class="Keyword">import</a> <a id="6402" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="6456" class="Keyword">open</a> <a id="6461" class="Keyword">import</a> <a id="6468" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="6533" class="Keyword">open</a> <a id="6538" class="Keyword">import</a> <a id="6545" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="6653" class="Keyword">open</a> <a id="6658" class="Keyword">import</a> <a id="6665" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="6685" class="Keyword">open</a> <a id="6690" class="Keyword">import</a> <a id="6697" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="6743" class="Keyword">open</a> <a id="6748" class="Keyword">import</a> <a id="6755" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="6801" class="Keyword">open</a> <a id="6806" class="Keyword">import</a> <a id="6813" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="6847" class="Keyword">open</a> <a id="6852" class="Keyword">import</a> <a id="6859" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="6894" class="Keyword">open</a> <a id="6899" class="Keyword">import</a> <a id="6906" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="6944" class="Keyword">open</a> <a id="6949" class="Keyword">import</a> <a id="6956" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="6994" class="Keyword">open</a> <a id="6999" class="Keyword">import</a> <a id="7006" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="7046" class="Keyword">open</a> <a id="7051" class="Keyword">import</a> <a id="7058" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="7091" class="Keyword">open</a> <a id="7096" class="Keyword">import</a> <a id="7103" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="7141" class="Keyword">open</a> <a id="7146" class="Keyword">import</a> <a id="7153" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="7216" class="Keyword">open</a> <a id="7221" class="Keyword">import</a> <a id="7228" href="foundation.html" class="Module">foundation</a>
<a id="7239" class="Keyword">open</a> <a id="7244" class="Keyword">import</a> <a id="7251" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="7269" class="Keyword">open</a> <a id="7274" class="Keyword">import</a> <a id="7281" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="7300" class="Keyword">open</a> <a id="7305" class="Keyword">import</a> <a id="7312" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="7331" class="Keyword">open</a> <a id="7336" class="Keyword">import</a> <a id="7343" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="7387" class="Keyword">open</a> <a id="7392" class="Keyword">import</a> <a id="7399" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="7424" class="Keyword">open</a> <a id="7429" class="Keyword">import</a> <a id="7436" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="7463" class="Keyword">open</a> <a id="7468" class="Keyword">import</a> <a id="7475" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="7504" class="Keyword">open</a> <a id="7509" class="Keyword">import</a> <a id="7516" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="7547" class="Keyword">open</a> <a id="7552" class="Keyword">import</a> <a id="7559" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="7587" class="Keyword">open</a> <a id="7592" class="Keyword">import</a> <a id="7599" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="7629" class="Keyword">open</a> <a id="7634" class="Keyword">import</a> <a id="7641" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="7661" class="Keyword">open</a> <a id="7666" class="Keyword">import</a> <a id="7673" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="7710" class="Keyword">open</a> <a id="7715" class="Keyword">import</a> <a id="7722" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="7757" class="Keyword">open</a> <a id="7762" class="Keyword">import</a> <a id="7769" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="7827" class="Keyword">open</a> <a id="7832" class="Keyword">import</a> <a id="7839" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="7877" class="Keyword">open</a> <a id="7882" class="Keyword">import</a> <a id="7889" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="7918" class="Keyword">open</a> <a id="7923" class="Keyword">import</a> <a id="7930" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="7953" class="Keyword">open</a> <a id="7958" class="Keyword">import</a> <a id="7965" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="7988" class="Keyword">open</a> <a id="7993" class="Keyword">import</a> <a id="8000" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="8042" class="Keyword">open</a> <a id="8047" class="Keyword">import</a> <a id="8054" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="8086" class="Keyword">open</a> <a id="8091" class="Keyword">import</a> <a id="8098" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="8125" class="Keyword">open</a> <a id="8130" class="Keyword">import</a> <a id="8137" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="8162" class="Keyword">open</a> <a id="8167" class="Keyword">import</a> <a id="8174" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="8203" class="Keyword">open</a> <a id="8208" class="Keyword">import</a> <a id="8215" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="8245" class="Keyword">open</a> <a id="8250" class="Keyword">import</a> <a id="8257" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="8284" class="Keyword">open</a> <a id="8289" class="Keyword">import</a> <a id="8296" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="8315" class="Keyword">open</a> <a id="8320" class="Keyword">import</a> <a id="8327" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="8373" class="Keyword">open</a> <a id="8378" class="Keyword">import</a> <a id="8385" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="8427" class="Keyword">open</a> <a id="8432" class="Keyword">import</a> <a id="8439" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="8471" class="Keyword">open</a> <a id="8476" class="Keyword">import</a> <a id="8483" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="8513" class="Keyword">open</a> <a id="8518" class="Keyword">import</a> <a id="8525" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="8551" class="Keyword">open</a> <a id="8556" class="Keyword">import</a> <a id="8563" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="8597" class="Keyword">open</a> <a id="8602" class="Keyword">import</a> <a id="8609" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="8639" class="Keyword">open</a> <a id="8644" class="Keyword">import</a> <a id="8651" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="8678" class="Keyword">open</a> <a id="8683" class="Keyword">import</a> <a id="8690" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="8722" class="Keyword">open</a> <a id="8727" class="Keyword">import</a> <a id="8734" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="8768" class="Keyword">open</a> <a id="8773" class="Keyword">import</a> <a id="8780" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="8803" class="Keyword">open</a> <a id="8808" class="Keyword">import</a> <a id="8815" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="8885" class="Keyword">open</a> <a id="8890" class="Keyword">import</a> <a id="8897" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="8967" class="Keyword">open</a> <a id="8972" class="Keyword">import</a> <a id="8979" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="9006" class="Keyword">open</a> <a id="9011" class="Keyword">import</a> <a id="9018" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="9066" class="Keyword">open</a> <a id="9071" class="Keyword">import</a> <a id="9078" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="9118" class="Keyword">open</a> <a id="9123" class="Keyword">import</a> <a id="9130" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="9152" class="Keyword">open</a> <a id="9157" class="Keyword">import</a> <a id="9164" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="9187" class="Keyword">open</a> <a id="9192" class="Keyword">import</a> <a id="9199" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="9244" class="Keyword">open</a> <a id="9249" class="Keyword">import</a> <a id="9256" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="9300" class="Keyword">open</a> <a id="9305" class="Keyword">import</a> <a id="9312" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="9348" class="Keyword">open</a> <a id="9353" class="Keyword">import</a> <a id="9360" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="9405" class="Keyword">open</a> <a id="9410" class="Keyword">import</a> <a id="9417" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="9458" class="Keyword">open</a> <a id="9463" class="Keyword">import</a> <a id="9470" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="9505" class="Keyword">open</a> <a id="9510" class="Keyword">import</a> <a id="9517" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="9548" class="Keyword">open</a> <a id="9553" class="Keyword">import</a> <a id="9560" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="9593" class="Keyword">open</a> <a id="9598" class="Keyword">import</a> <a id="9605" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="9638" class="Keyword">open</a> <a id="9643" class="Keyword">import</a> <a id="9650" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="9680" class="Keyword">open</a> <a id="9685" class="Keyword">import</a> <a id="9692" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="9716" class="Keyword">open</a> <a id="9721" class="Keyword">import</a> <a id="9728" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="9766" class="Keyword">open</a> <a id="9771" class="Keyword">import</a> <a id="9778" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="9809" class="Keyword">open</a> <a id="9814" class="Keyword">import</a> <a id="9821" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="9846" class="Keyword">open</a> <a id="9851" class="Keyword">import</a> <a id="9858" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="9886" class="Keyword">open</a> <a id="9891" class="Keyword">import</a> <a id="9898" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="9922" class="Keyword">open</a> <a id="9927" class="Keyword">import</a> <a id="9934" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="9960" class="Keyword">open</a> <a id="9965" class="Keyword">import</a> <a id="9972" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="10007" class="Keyword">open</a> <a id="10012" class="Keyword">import</a> <a id="10019" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="10040" class="Keyword">open</a> <a id="10045" class="Keyword">import</a> <a id="10052" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="10101" class="Keyword">open</a> <a id="10106" class="Keyword">import</a> <a id="10113" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="10154" class="Keyword">open</a> <a id="10159" class="Keyword">import</a> <a id="10166" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="10216" class="Keyword">open</a> <a id="10221" class="Keyword">import</a> <a id="10228" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="10274" class="Keyword">open</a> <a id="10279" class="Keyword">import</a> <a id="10286" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="10326" class="Keyword">open</a> <a id="10331" class="Keyword">import</a> <a id="10338" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="10388" class="Keyword">open</a> <a id="10393" class="Keyword">import</a> <a id="10400" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="10439" class="Keyword">open</a> <a id="10444" class="Keyword">import</a> <a id="10451" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="10491" class="Keyword">open</a> <a id="10496" class="Keyword">import</a> <a id="10503" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="10536" class="Keyword">open</a> <a id="10541" class="Keyword">import</a> <a id="10548" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="10597" class="Keyword">open</a> <a id="10602" class="Keyword">import</a> <a id="10609" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="10634" class="Keyword">open</a> <a id="10639" class="Keyword">import</a> <a id="10646" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="10668" class="Keyword">open</a> <a id="10673" class="Keyword">import</a> <a id="10680" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="10708" class="Keyword">open</a> <a id="10713" class="Keyword">import</a> <a id="10720" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="10746" class="Keyword">open</a> <a id="10751" class="Keyword">import</a> <a id="10758" href="foundation.images.html" class="Module">foundation.images</a>
<a id="10776" class="Keyword">open</a> <a id="10781" class="Keyword">import</a> <a id="10788" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="10823" class="Keyword">open</a> <a id="10828" class="Keyword">import</a> <a id="10835" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="10862" class="Keyword">open</a> <a id="10867" class="Keyword">import</a> <a id="10874" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="10930" class="Keyword">open</a> <a id="10935" class="Keyword">import</a> <a id="10942" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="10971" class="Keyword">open</a> <a id="10976" class="Keyword">import</a> <a id="10983" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="11013" class="Keyword">open</a> <a id="11018" class="Keyword">import</a> <a id="11025" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="11051" class="Keyword">open</a> <a id="11056" class="Keyword">import</a> <a id="11063" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="11090" class="Keyword">open</a> <a id="11095" class="Keyword">import</a> <a id="11102" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="11125" class="Keyword">open</a> <a id="11130" class="Keyword">import</a> <a id="11137" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="11164" class="Keyword">open</a> <a id="11169" class="Keyword">import</a> <a id="11176" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="11208" class="Keyword">open</a> <a id="11213" class="Keyword">import</a> <a id="11220" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="11254" class="Keyword">open</a> <a id="11259" class="Keyword">import</a> <a id="11266" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="11306" class="Keyword">open</a> <a id="11311" class="Keyword">import</a> <a id="11318" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="11349" class="Keyword">open</a> <a id="11354" class="Keyword">import</a> <a id="11361" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="11393" class="Keyword">open</a> <a id="11398" class="Keyword">import</a> <a id="11405" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="11436" class="Keyword">open</a> <a id="11441" class="Keyword">import</a> <a id="11448" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="11465" class="Keyword">open</a> <a id="11470" class="Keyword">import</a> <a id="11477" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="11502" class="Keyword">open</a> <a id="11507" class="Keyword">import</a> <a id="11514" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="11543" class="Keyword">open</a> <a id="11548" class="Keyword">import</a> <a id="11555" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="11580" class="Keyword">open</a> <a id="11585" class="Keyword">import</a> <a id="11592" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="11613" class="Keyword">open</a> <a id="11618" class="Keyword">import</a> <a id="11625" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="11645" class="Keyword">open</a> <a id="11650" class="Keyword">import</a> <a id="11657" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="11691" class="Keyword">open</a> <a id="11696" class="Keyword">import</a> <a id="11703" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="11727" class="Keyword">open</a> <a id="11732" class="Keyword">import</a> <a id="11739" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="11766" class="Keyword">open</a> <a id="11771" class="Keyword">import</a> <a id="11778" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="11813" class="Keyword">open</a> <a id="11818" class="Keyword">import</a> <a id="11825" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="11865" class="Keyword">open</a> <a id="11870" class="Keyword">import</a> <a id="11877" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="11907" class="Keyword">open</a> <a id="11912" class="Keyword">import</a> <a id="11919" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="11956" class="Keyword">open</a> <a id="11961" class="Keyword">import</a> <a id="11968" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="11992" class="Keyword">open</a> <a id="11997" class="Keyword">import</a> <a id="12004" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="12025" class="Keyword">open</a> <a id="12030" class="Keyword">import</a> <a id="12037" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="12072" class="Keyword">open</a> <a id="12077" class="Keyword">import</a> <a id="12084" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="12121" class="Keyword">open</a> <a id="12126" class="Keyword">import</a> <a id="12133" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="12182" class="Keyword">open</a> <a id="12187" class="Keyword">import</a> <a id="12194" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="12217" class="Keyword">open</a> <a id="12222" class="Keyword">import</a> <a id="12229" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="12252" class="Keyword">open</a> <a id="12257" class="Keyword">import</a> <a id="12264" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="12292" class="Keyword">open</a> <a id="12297" class="Keyword">import</a> <a id="12304" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="12324" class="Keyword">open</a> <a id="12329" class="Keyword">import</a> <a id="12336" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="12367" class="Keyword">open</a> <a id="12372" class="Keyword">import</a> <a id="12379" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="12406" class="Keyword">open</a> <a id="12411" class="Keyword">import</a> <a id="12418" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="12434" class="Keyword">open</a> <a id="12439" class="Keyword">import</a> <a id="12446" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="12477" class="Keyword">open</a> <a id="12482" class="Keyword">import</a> <a id="12489" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="12506" class="Keyword">open</a> <a id="12511" class="Keyword">import</a> <a id="12518" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="12540" class="Keyword">open</a> <a id="12545" class="Keyword">import</a> <a id="12552" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="12579" class="Keyword">open</a> <a id="12584" class="Keyword">import</a> <a id="12591" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="12614" class="Keyword">open</a> <a id="12619" class="Keyword">import</a> <a id="12626" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="12653" class="Keyword">open</a> <a id="12658" class="Keyword">import</a> <a id="12665" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="12698" class="Keyword">open</a> <a id="12703" class="Keyword">import</a> <a id="12710" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="12750" class="Keyword">open</a> <a id="12755" class="Keyword">import</a> <a id="12762" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="12783" class="Keyword">open</a> <a id="12788" class="Keyword">import</a> <a id="12795" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="12824" class="Keyword">open</a> <a id="12829" class="Keyword">import</a> <a id="12836" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="12874" class="Keyword">open</a> <a id="12879" class="Keyword">import</a> <a id="12886" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="12906" class="Keyword">open</a> <a id="12911" class="Keyword">import</a> <a id="12918" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="12942" class="Keyword">open</a> <a id="12947" class="Keyword">import</a> <a id="12954" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="12981" class="Keyword">open</a> <a id="12986" class="Keyword">import</a> <a id="12993" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="13023" class="Keyword">open</a> <a id="13028" class="Keyword">import</a> <a id="13035" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="13061" class="Keyword">open</a> <a id="13066" class="Keyword">import</a> <a id="13073" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="13100" class="Keyword">open</a> <a id="13105" class="Keyword">import</a> <a id="13112" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="13141" class="Keyword">open</a> <a id="13146" class="Keyword">import</a> <a id="13153" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="13176" class="Keyword">open</a> <a id="13181" class="Keyword">import</a> <a id="13188" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="13239" class="Keyword">open</a> <a id="13244" class="Keyword">import</a> <a id="13251" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="13294" class="Keyword">open</a> <a id="13299" class="Keyword">import</a> <a id="13306" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="13354" class="Keyword">open</a> <a id="13359" class="Keyword">import</a> <a id="13366" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="13404" class="Keyword">open</a> <a id="13409" class="Keyword">import</a> <a id="13416" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="13453" class="Keyword">open</a> <a id="13458" class="Keyword">import</a> <a id="13465" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="13493" class="Keyword">open</a> <a id="13498" class="Keyword">import</a> <a id="13505" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="13541" class="Keyword">open</a> <a id="13546" class="Keyword">import</a> <a id="13553" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="13591" class="Keyword">open</a> <a id="13596" class="Keyword">import</a> <a id="13603" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="13636" class="Keyword">open</a> <a id="13641" class="Keyword">import</a> <a id="13648" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="13669" class="Keyword">open</a> <a id="13674" class="Keyword">import</a> <a id="13681" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="13735" class="Keyword">open</a> <a id="13740" class="Keyword">import</a> <a id="13747" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="13769" class="Keyword">open</a> <a id="13774" class="Keyword">import</a> <a id="13781" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="13816" class="Keyword">open</a> <a id="13821" class="Keyword">import</a> <a id="13828" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="13858" class="Keyword">open</a> <a id="13863" class="Keyword">import</a> <a id="13870" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="13909" class="Keyword">open</a> <a id="13914" class="Keyword">import</a> <a id="13921" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="13975" class="Keyword">open</a> <a id="13980" class="Keyword">import</a> <a id="13987" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="14033" class="Keyword">open</a> <a id="14038" class="Keyword">import</a> <a id="14045" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="14096" class="Keyword">open</a> <a id="14101" class="Keyword">import</a> <a id="14108" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="14149" class="Keyword">open</a> <a id="14154" class="Keyword">import</a> <a id="14161" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="14206" class="Keyword">open</a> <a id="14211" class="Keyword">import</a> <a id="14218" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="14263" class="Keyword">open</a> <a id="14268" class="Keyword">import</a> <a id="14275" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="14311" class="Keyword">open</a> <a id="14316" class="Keyword">import</a> <a id="14323" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="14359" class="Keyword">open</a> <a id="14364" class="Keyword">import</a> <a id="14371" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="14436" class="Keyword">open</a> <a id="14441" class="Keyword">import</a> <a id="14448" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="14503" class="Keyword">open</a> <a id="14508" class="Keyword">import</a> <a id="14515" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="14555" class="Keyword">open</a> <a id="14560" class="Keyword">import</a> <a id="14567" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="14611" class="Keyword">open</a> <a id="14616" class="Keyword">import</a> <a id="14623" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="14668" class="Keyword">open</a> <a id="14673" class="Keyword">import</a> <a id="14680" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="14721" class="Keyword">open</a> <a id="14726" class="Keyword">import</a> <a id="14733" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="14773" class="Keyword">open</a> <a id="14778" class="Keyword">import</a> <a id="14785" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="14812" class="Keyword">open</a> <a id="14817" class="Keyword">import</a> <a id="14824" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="14851" class="Keyword">open</a> <a id="14856" class="Keyword">import</a> <a id="14863" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="14882" class="Keyword">open</a> <a id="14887" class="Keyword">import</a> <a id="14894" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="14934" class="Keyword">open</a> <a id="14939" class="Keyword">import</a> <a id="14946" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="15011" class="Keyword">open</a> <a id="15016" class="Keyword">import</a> <a id="15023" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="15046" class="Keyword">open</a> <a id="15051" class="Keyword">import</a> <a id="15058" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="15082" class="Keyword">open</a> <a id="15087" class="Keyword">import</a> <a id="15094" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="15134" class="Keyword">open</a> <a id="15139" class="Keyword">import</a> <a id="15146" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="15189" class="Keyword">open</a> <a id="15194" class="Keyword">import</a> <a id="15201" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="15235" class="Keyword">open</a> <a id="15240" class="Keyword">import</a> <a id="15247" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="15277" class="Keyword">open</a> <a id="15282" class="Keyword">import</a> <a id="15289" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="15323" class="Keyword">open</a> <a id="15328" class="Keyword">import</a> <a id="15335" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="15370" class="Keyword">open</a> <a id="15375" class="Keyword">import</a> <a id="15382" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="15419" class="Keyword">open</a> <a id="15424" class="Keyword">import</a> <a id="15431" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="15458" class="Keyword">open</a> <a id="15463" class="Keyword">import</a> <a id="15470" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="15498" class="Keyword">open</a> <a id="15503" class="Keyword">import</a> <a id="15510" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="15559" class="Keyword">open</a> <a id="15564" class="Keyword">import</a> <a id="15571" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="15617" class="Keyword">open</a> <a id="15622" class="Keyword">import</a> <a id="15629" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="15669" class="Keyword">open</a> <a id="15674" class="Keyword">import</a> <a id="15681" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="15719" class="Keyword">open</a> <a id="15724" class="Keyword">import</a> <a id="15731" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="15760" class="Keyword">open</a> <a id="15765" class="Keyword">import</a> <a id="15772" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="15802" class="Keyword">open</a> <a id="15807" class="Keyword">import</a> <a id="15814" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="15845" class="Keyword">open</a> <a id="15850" class="Keyword">import</a> <a id="15857" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="15883" class="Keyword">open</a> <a id="15888" class="Keyword">import</a> <a id="15895" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="15946" class="Keyword">open</a> <a id="15951" class="Keyword">import</a> <a id="15958" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="16012" class="Keyword">open</a> <a id="16017" class="Keyword">import</a> <a id="16024" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="16051" class="Keyword">open</a> <a id="16056" class="Keyword">import</a> <a id="16063" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="16096" class="Keyword">open</a> <a id="16101" class="Keyword">import</a> <a id="16108" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="16139" class="Keyword">open</a> <a id="16144" class="Keyword">import</a> <a id="16151" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="16188" class="Keyword">open</a> <a id="16193" class="Keyword">import</a> <a id="16200" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="16225" class="Keyword">open</a> <a id="16230" class="Keyword">import</a> <a id="16237" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="16269" class="Keyword">open</a> <a id="16274" class="Keyword">import</a> <a id="16281" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="16316" class="Keyword">open</a> <a id="16321" class="Keyword">import</a> <a id="16328" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="16357" class="Keyword">open</a> <a id="16362" class="Keyword">import</a> <a id="16369" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="16397" class="Keyword">open</a> <a id="16402" class="Keyword">import</a> <a id="16409" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="16434" class="Keyword">open</a> <a id="16439" class="Keyword">import</a> <a id="16446" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="16467" class="Keyword">open</a> <a id="16472" class="Keyword">import</a> <a id="16479" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="16515" class="Keyword">open</a> <a id="16520" class="Keyword">import</a> <a id="16527" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="16570" class="Keyword">open</a> <a id="16575" class="Keyword">import</a> <a id="16582" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="16607" class="Keyword">open</a> <a id="16612" class="Keyword">import</a> <a id="16619" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="16650" class="Keyword">open</a> <a id="16655" class="Keyword">import</a> <a id="16662" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="16694" class="Keyword">open</a> <a id="16699" class="Keyword">import</a> <a id="16706" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="16740" class="Keyword">open</a> <a id="16745" class="Keyword">import</a> <a id="16752" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="16808" class="Keyword">open</a> <a id="16813" class="Keyword">import</a> <a id="16820" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="16873" class="Keyword">open</a> <a id="16878" class="Keyword">import</a> <a id="16885" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="16912" class="Keyword">open</a> <a id="16917" class="Keyword">import</a> <a id="16924" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="16986" class="Keyword">open</a> <a id="16991" class="Keyword">import</a> <a id="16998" href="graph-theory.html" class="Module">graph-theory</a>
<a id="17011" class="Keyword">open</a> <a id="17016" class="Keyword">import</a> <a id="17023" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="17064" class="Keyword">open</a> <a id="17069" class="Keyword">import</a> <a id="17076" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="17105" class="Keyword">open</a> <a id="17110" class="Keyword">import</a> <a id="17117" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="17162" class="Keyword">open</a> <a id="17167" class="Keyword">import</a> <a id="17174" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="17218" class="Keyword">open</a> <a id="17223" class="Keyword">import</a> <a id="17230" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="17257" class="Keyword">open</a> <a id="17262" class="Keyword">import</a> <a id="17269" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="17310" class="Keyword">open</a> <a id="17315" class="Keyword">import</a> <a id="17322" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="17371" class="Keyword">open</a> <a id="17376" class="Keyword">import</a> <a id="17383" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="17422" class="Keyword">open</a> <a id="17427" class="Keyword">import</a> <a id="17434" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="17475" class="Keyword">open</a> <a id="17480" class="Keyword">import</a> <a id="17487" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="17531" class="Keyword">open</a> <a id="17536" class="Keyword">import</a> <a id="17543" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="17580" class="Keyword">open</a> <a id="17585" class="Keyword">import</a> <a id="17592" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="17614" class="Keyword">open</a> <a id="17619" class="Keyword">import</a> <a id="17626" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="17656" class="Keyword">open</a> <a id="17661" class="Keyword">import</a> <a id="17668" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="17707" class="Keyword">open</a> <a id="17712" class="Keyword">import</a> <a id="17719" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="17757" class="Keyword">open</a> <a id="17762" class="Keyword">import</a> <a id="17769" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="17830" class="Keyword">open</a> <a id="17835" class="Keyword">import</a> <a id="17842" href="group-theory.html" class="Module">group-theory</a>
<a id="17855" class="Keyword">open</a> <a id="17860" class="Keyword">import</a> <a id="17867" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="17895" class="Keyword">open</a> <a id="17900" class="Keyword">import</a> <a id="17907" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="17938" class="Keyword">open</a> <a id="17943" class="Keyword">import</a> <a id="17950" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="17986" class="Keyword">open</a> <a id="17991" class="Keyword">import</a> <a id="17998" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="18049" class="Keyword">open</a> <a id="18054" class="Keyword">import</a> <a id="18061" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="18093" class="Keyword">open</a> <a id="18098" class="Keyword">import</a> <a id="18105" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="18141" class="Keyword">open</a> <a id="18146" class="Keyword">import</a> <a id="18153" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="18182" class="Keyword">open</a> <a id="18187" class="Keyword">import</a> <a id="18194" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="18230" class="Keyword">open</a> <a id="18235" class="Keyword">import</a> <a id="18242" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="18271" class="Keyword">open</a> <a id="18276" class="Keyword">import</a> <a id="18283" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="18315" class="Keyword">open</a> <a id="18320" class="Keyword">import</a> <a id="18327" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="18352" class="Keyword">open</a> <a id="18357" class="Keyword">import</a> <a id="18364" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="18395" class="Keyword">open</a> <a id="18400" class="Keyword">import</a> <a id="18407" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="18454" class="Keyword">open</a> <a id="18459" class="Keyword">import</a> <a id="18466" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="18506" class="Keyword">open</a> <a id="18511" class="Keyword">import</a> <a id="18518" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="18555" class="Keyword">open</a> <a id="18560" class="Keyword">import</a> <a id="18567" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="18603" class="Keyword">open</a> <a id="18608" class="Keyword">import</a> <a id="18615" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="18647" class="Keyword">open</a> <a id="18652" class="Keyword">import</a> <a id="18659" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="18686" class="Keyword">open</a> <a id="18691" class="Keyword">import</a> <a id="18698" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="18718" class="Keyword">open</a> <a id="18723" class="Keyword">import</a> <a id="18730" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="18757" class="Keyword">open</a> <a id="18762" class="Keyword">import</a> <a id="18769" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="18811" class="Keyword">open</a> <a id="18816" class="Keyword">import</a> <a id="18823" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="18864" class="Keyword">open</a> <a id="18869" class="Keyword">import</a> <a id="18876" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="18910" class="Keyword">open</a> <a id="18915" class="Keyword">import</a> <a id="18922" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="18957" class="Keyword">open</a> <a id="18962" class="Keyword">import</a> <a id="18969" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="19007" class="Keyword">open</a> <a id="19012" class="Keyword">import</a> <a id="19019" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="19060" class="Keyword">open</a> <a id="19065" class="Keyword">import</a> <a id="19072" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="19113" class="Keyword">open</a> <a id="19118" class="Keyword">import</a> <a id="19125" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="19165" class="Keyword">open</a> <a id="19170" class="Keyword">import</a> <a id="19177" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="19210" class="Keyword">open</a> <a id="19215" class="Keyword">import</a> <a id="19222" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="19259" class="Keyword">open</a> <a id="19264" class="Keyword">import</a> <a id="19271" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="19316" class="Keyword">open</a> <a id="19321" class="Keyword">import</a> <a id="19328" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="19349" class="Keyword">open</a> <a id="19354" class="Keyword">import</a> <a id="19361" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="19395" class="Keyword">open</a> <a id="19400" class="Keyword">import</a> <a id="19407" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="19449" class="Keyword">open</a> <a id="19454" class="Keyword">import</a> <a id="19461" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="19496" class="Keyword">open</a> <a id="19501" class="Keyword">import</a> <a id="19508" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="19547" class="Keyword">open</a> <a id="19552" class="Keyword">import</a> <a id="19559" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="19596" class="Keyword">open</a> <a id="19601" class="Keyword">import</a> <a id="19608" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="19632" class="Keyword">open</a> <a id="19637" class="Keyword">import</a> <a id="19644" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="19669" class="Keyword">open</a> <a id="19674" class="Keyword">import</a> <a id="19681" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="19712" class="Keyword">open</a> <a id="19717" class="Keyword">import</a> <a id="19724" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="19747" class="Keyword">open</a> <a id="19752" class="Keyword">import</a> <a id="19759" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="19807" class="Keyword">open</a> <a id="19812" class="Keyword">import</a> <a id="19819" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="19849" class="Keyword">open</a> <a id="19854" class="Keyword">import</a> <a id="19861" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="19931" class="Keyword">open</a> <a id="19936" class="Keyword">import</a> <a id="19943" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="19958" class="Keyword">open</a> <a id="19963" class="Keyword">import</a> <a id="19970" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="20003" class="Keyword">open</a> <a id="20008" class="Keyword">import</a> <a id="20015" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="20047" class="Keyword">open</a> <a id="20052" class="Keyword">import</a> <a id="20059" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="20101" class="Keyword">open</a> <a id="20106" class="Keyword">import</a> <a id="20113" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="20151" class="Keyword">open</a> <a id="20156" class="Keyword">import</a> <a id="20163" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="20200" class="Keyword">open</a> <a id="20205" class="Keyword">import</a> <a id="20212" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="20245" class="Keyword">open</a> <a id="20250" class="Keyword">import</a> <a id="20257" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="20281" class="Keyword">open</a> <a id="20286" class="Keyword">import</a> <a id="20293" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="20332" class="Keyword">open</a> <a id="20337" class="Keyword">import</a> <a id="20344" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="20390" class="Keyword">open</a> <a id="20395" class="Keyword">import</a> <a id="20402" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="20447" class="Keyword">open</a> <a id="20452" class="Keyword">import</a> <a id="20459" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="20497" class="Keyword">open</a> <a id="20502" class="Keyword">import</a> <a id="20509" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="20541" class="Keyword">open</a> <a id="20546" class="Keyword">import</a> <a id="20553" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="20606" class="Keyword">open</a> <a id="20611" class="Keyword">import</a> <a id="20618" href="order-theory.html" class="Module">order-theory</a>
<a id="20631" class="Keyword">open</a> <a id="20636" class="Keyword">import</a> <a id="20643" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="20670" class="Keyword">open</a> <a id="20675" class="Keyword">import</a> <a id="20682" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="20712" class="Keyword">open</a> <a id="20717" class="Keyword">import</a> <a id="20724" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="20757" class="Keyword">open</a> <a id="20762" class="Keyword">import</a> <a id="20769" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="20805" class="Keyword">open</a> <a id="20810" class="Keyword">import</a> <a id="20817" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="20844" class="Keyword">open</a> <a id="20849" class="Keyword">import</a> <a id="20856" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="20886" class="Keyword">open</a> <a id="20891" class="Keyword">import</a> <a id="20898" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="20934" class="Keyword">open</a> <a id="20939" class="Keyword">import</a> <a id="20946" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="20988" class="Keyword">open</a> <a id="20993" class="Keyword">import</a> <a id="21000" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="21032" class="Keyword">open</a> <a id="21037" class="Keyword">import</a> <a id="21044" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="21081" class="Keyword">open</a> <a id="21086" class="Keyword">import</a> <a id="21093" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="21133" class="Keyword">open</a> <a id="21138" class="Keyword">import</a> <a id="21145" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="21180" class="Keyword">open</a> <a id="21185" class="Keyword">import</a> <a id="21192" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="21230" class="Keyword">open</a> <a id="21235" class="Keyword">import</a> <a id="21242" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="21277" class="Keyword">open</a> <a id="21282" class="Keyword">import</a> <a id="21289" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="21324" class="Keyword">open</a> <a id="21329" class="Keyword">import</a> <a id="21336" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="21374" class="Keyword">open</a> <a id="21379" class="Keyword">import</a> <a id="21386" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="21417" class="Keyword">open</a> <a id="21422" class="Keyword">import</a> <a id="21429" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="21462" class="Keyword">open</a> <a id="21467" class="Keyword">import</a> <a id="21474" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="21494" class="Keyword">open</a> <a id="21499" class="Keyword">import</a> <a id="21506" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="21529" class="Keyword">open</a> <a id="21534" class="Keyword">import</a> <a id="21541" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="21564" class="Keyword">open</a> <a id="21569" class="Keyword">import</a> <a id="21576" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="21602" class="Keyword">open</a> <a id="21607" class="Keyword">import</a> <a id="21614" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="21640" class="Keyword">open</a> <a id="21645" class="Keyword">import</a> <a id="21652" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="21708" class="Keyword">open</a> <a id="21713" class="Keyword">import</a> <a id="21720" href="polytopes.html" class="Module">polytopes</a>
<a id="21730" class="Keyword">open</a> <a id="21735" class="Keyword">import</a> <a id="21742" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="21800" class="Keyword">open</a> <a id="21805" class="Keyword">import</a> <a id="21812" href="ring-theory.html" class="Module">ring-theory</a>
<a id="21824" class="Keyword">open</a> <a id="21829" class="Keyword">import</a> <a id="21836" href="ring-theory.commutative-rings.html" class="Module">ring-theory.commutative-rings</a>
<a id="21866" class="Keyword">open</a> <a id="21871" class="Keyword">import</a> <a id="21878" href="ring-theory.discrete-fields.html" class="Module">ring-theory.discrete-fields</a>
<a id="21906" class="Keyword">open</a> <a id="21911" class="Keyword">import</a> <a id="21918" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="21945" class="Keyword">open</a> <a id="21950" class="Keyword">import</a> <a id="21957" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="21989" class="Keyword">open</a> <a id="21994" class="Keyword">import</a> <a id="22001" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="22031" class="Keyword">open</a> <a id="22036" class="Keyword">import</a> <a id="22043" href="ring-theory.homomorphisms-commutative-rings.html" class="Module">ring-theory.homomorphisms-commutative-rings</a>
<a id="22087" class="Keyword">open</a> <a id="22092" class="Keyword">import</a> <a id="22099" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="22131" class="Keyword">open</a> <a id="22136" class="Keyword">import</a> <a id="22143" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a>
<a id="22162" class="Keyword">open</a> <a id="22167" class="Keyword">import</a> <a id="22174" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="22212" class="Keyword">open</a> <a id="22217" class="Keyword">import</a> <a id="22224" href="ring-theory.isomorphisms-commutative-rings.html" class="Module">ring-theory.isomorphisms-commutative-rings</a>
<a id="22267" class="Keyword">open</a> <a id="22272" class="Keyword">import</a> <a id="22279" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="22310" class="Keyword">open</a> <a id="22315" class="Keyword">import</a> <a id="22322" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="22354" class="Keyword">open</a> <a id="22359" class="Keyword">import</a> <a id="22366" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="22395" class="Keyword">open</a> <a id="22400" class="Keyword">import</a> <a id="22407" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="22468" class="Keyword">open</a> <a id="22473" class="Keyword">import</a> <a id="22480" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="22506" class="Keyword">open</a> <a id="22511" class="Keyword">import</a> <a id="22518" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="22557" class="Keyword">open</a> <a id="22562" class="Keyword">import</a> <a id="22569" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="22607" class="Keyword">open</a> <a id="22612" class="Keyword">import</a> <a id="22619" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="22665" class="Keyword">open</a> <a id="22670" class="Keyword">import</a> <a id="22677" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="22714" class="Keyword">open</a> <a id="22719" class="Keyword">import</a> <a id="22726" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="22766" class="Keyword">open</a> <a id="22771" class="Keyword">import</a> <a id="22778" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="22817" class="Keyword">open</a> <a id="22822" class="Keyword">import</a> <a id="22829" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="22862" class="Keyword">open</a> <a id="22867" class="Keyword">import</a> <a id="22874" href="synthetic-homotopy-theory.commutative-operations.html" class="Module">synthetic-homotopy-theory.commutative-operations</a>
<a id="22923" class="Keyword">open</a> <a id="22928" class="Keyword">import</a> <a id="22935" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="22974" class="Keyword">open</a> <a id="22979" class="Keyword">import</a> <a id="22986" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="23031" class="Keyword">open</a> <a id="23036" class="Keyword">import</a> <a id="23043" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="23095" class="Keyword">open</a> <a id="23100" class="Keyword">import</a> <a id="23107" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="23160" class="Keyword">open</a> <a id="23165" class="Keyword">import</a> <a id="23172" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="23220" class="Keyword">open</a> <a id="23225" class="Keyword">import</a> <a id="23232" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="23272" class="Keyword">open</a> <a id="23277" class="Keyword">import</a> <a id="23284" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="23331" class="Keyword">open</a> <a id="23336" class="Keyword">import</a> <a id="23343" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="23381" class="Keyword">open</a> <a id="23386" class="Keyword">import</a> <a id="23393" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="23447" class="Keyword">open</a> <a id="23452" class="Keyword">import</a> <a id="23459" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="23506" class="Keyword">open</a> <a id="23511" class="Keyword">import</a> <a id="23518" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="23570" class="Keyword">open</a> <a id="23575" class="Keyword">import</a> <a id="23582" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="23627" class="Keyword">open</a> <a id="23632" class="Keyword">import</a> <a id="23639" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="23678" class="Keyword">open</a> <a id="23683" class="Keyword">import</a> <a id="23690" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="23730" class="Keyword">open</a> <a id="23735" class="Keyword">import</a> <a id="23742" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="23775" class="Keyword">open</a> <a id="23780" class="Keyword">import</a> <a id="23787" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="23832" class="Keyword">open</a> <a id="23837" class="Keyword">import</a> <a id="23844" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="23920" class="Keyword">open</a> <a id="23925" class="Keyword">import</a> <a id="23932" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="23994" class="Keyword">open</a> <a id="23999" class="Keyword">import</a> <a id="24006" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="24030" class="Keyword">open</a> <a id="24035" class="Keyword">import</a> <a id="24042" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="24085" class="Keyword">open</a> <a id="24090" class="Keyword">import</a> <a id="24097" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="24137" class="Keyword">open</a> <a id="24142" class="Keyword">import</a> <a id="24149" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="24188" class="Keyword">open</a> <a id="24193" class="Keyword">import</a> <a id="24200" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="24248" class="Keyword">open</a> <a id="24253" class="Keyword">import</a> <a id="24260" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="24307" class="Keyword">open</a> <a id="24312" class="Keyword">import</a> <a id="24319" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="24371" class="Keyword">open</a> <a id="24376" class="Keyword">import</a> <a id="24383" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="24423" class="Keyword">open</a> <a id="24428" class="Keyword">import</a> <a id="24435" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="24487" class="Keyword">open</a> <a id="24492" class="Keyword">import</a> <a id="24499" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="24557" class="Keyword">open</a> <a id="24562" class="Keyword">import</a> <a id="24569" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="24623" class="Keyword">open</a> <a id="24628" class="Keyword">import</a> <a id="24635" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="24683" class="Keyword">open</a> <a id="24688" class="Keyword">import</a> <a id="24695" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="24743" class="Keyword">open</a> <a id="24748" class="Keyword">import</a> <a id="24755" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="24794" class="Keyword">open</a> <a id="24799" class="Keyword">import</a> <a id="24806" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="24839" class="Keyword">open</a> <a id="24844" class="Keyword">import</a> <a id="24851" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="24881" class="Keyword">open</a> <a id="24886" class="Keyword">import</a> <a id="24893" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="24952" class="Keyword">open</a> <a id="24957" class="Keyword">import</a> <a id="24964" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="25019" class="Keyword">open</a> <a id="25024" class="Keyword">import</a> <a id="25031" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="25074" class="Keyword">open</a> <a id="25079" class="Keyword">import</a> <a id="25086" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="25141" class="Keyword">open</a> <a id="25146" class="Keyword">import</a> <a id="25153" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="25204" class="Keyword">open</a> <a id="25209" class="Keyword">import</a> <a id="25216" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="25294" class="Keyword">open</a> <a id="25299" class="Keyword">import</a> <a id="25306" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="25346" class="Keyword">open</a> <a id="25351" class="Keyword">import</a> <a id="25358" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="25415" class="Keyword">open</a> <a id="25420" class="Keyword">import</a> <a id="25427" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="25462" class="Keyword">open</a> <a id="25467" class="Keyword">import</a> <a id="25474" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="25520" class="Keyword">open</a> <a id="25525" class="Keyword">import</a> <a id="25532" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="25587" class="Keyword">open</a> <a id="25592" class="Keyword">import</a> <a id="25599" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="25642" class="Keyword">open</a> <a id="25647" class="Keyword">import</a> <a id="25654" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="25713" class="Keyword">open</a> <a id="25718" class="Keyword">import</a> <a id="25725" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="25762" class="Keyword">open</a> <a id="25767" class="Keyword">import</a> <a id="25774" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="25834" class="Keyword">open</a> <a id="25839" class="Keyword">import</a> <a id="25846" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="25884" class="Keyword">open</a> <a id="25889" class="Keyword">import</a> <a id="25896" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="25948" class="Keyword">open</a> <a id="25953" class="Keyword">import</a> <a id="25960" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="26006" class="Keyword">open</a> <a id="26011" class="Keyword">import</a> <a id="26018" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="26063" class="Keyword">open</a> <a id="26068" class="Keyword">import</a> <a id="26075" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="26112" class="Keyword">open</a> <a id="26117" class="Keyword">import</a> <a id="26124" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="26173" class="Keyword">open</a> <a id="26178" class="Keyword">import</a> <a id="26185" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="26223" class="Keyword">open</a> <a id="26228" class="Keyword">import</a> <a id="26235" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="26290" class="Keyword">open</a> <a id="26295" class="Keyword">import</a> <a id="26302" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="26341" class="Keyword">open</a> <a id="26346" class="Keyword">import</a> <a id="26353" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="26383" class="Keyword">open</a> <a id="26388" class="Keyword">import</a> <a id="26395" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="26425" class="Keyword">open</a> <a id="26430" class="Keyword">import</a> <a id="26437" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="26480" class="Keyword">open</a> <a id="26485" class="Keyword">import</a> <a id="26492" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="26532" class="Keyword">open</a> <a id="26537" class="Keyword">import</a> <a id="26544" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="26589" class="Keyword">open</a> <a id="26594" class="Keyword">import</a> <a id="26601" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="26651" class="Keyword">open</a> <a id="26656" class="Keyword">import</a> <a id="26663" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="26701" class="Keyword">open</a> <a id="26706" class="Keyword">import</a> <a id="26713" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="26762" class="Keyword">open</a> <a id="26767" class="Keyword">import</a> <a id="26774" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="26837" class="Keyword">open</a> <a id="26842" class="Keyword">import</a> <a id="26849" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="26881" class="Keyword">open</a> <a id="26886" class="Keyword">import</a> <a id="26893" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="26946" class="Keyword">open</a> <a id="26951" class="Keyword">import</a> <a id="26958" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="27004" class="Keyword">open</a> <a id="27009" class="Keyword">import</a> <a id="27016" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="27062" class="Keyword">open</a> <a id="27067" class="Keyword">import</a> <a id="27074" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="27122" class="Keyword">open</a> <a id="27127" class="Keyword">import</a> <a id="27134" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="27204" class="Keyword">open</a> <a id="27209" class="Keyword">import</a> <a id="27216" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="27229" class="Keyword">open</a> <a id="27234" class="Keyword">import</a> <a id="27241" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="27261" class="Keyword">open</a> <a id="27266" class="Keyword">import</a> <a id="27273" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="27324" class="Keyword">open</a> <a id="27329" class="Keyword">import</a> <a id="27336" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="27361" class="Keyword">open</a> <a id="27366" class="Keyword">import</a> <a id="27373" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="27399" class="Keyword">open</a> <a id="27404" class="Keyword">import</a> <a id="27411" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

