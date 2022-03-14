# Univalent mathematics in Agda

Welcome to the website of the `agda-unimath` formalization project.

[![build](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml)

<pre class="Agda"><a id="281" class="Symbol">{-#</a> <a id="285" class="Keyword">OPTIONS</a> <a id="293" class="Pragma">--without-K</a> <a id="305" class="Pragma">--exact-split</a> <a id="319" class="Symbol">#-}</a>
</pre>
## Category theory

<pre class="Agda"><a id="356" class="Keyword">open</a> <a id="361" class="Keyword">import</a> <a id="368" href="category-theory.html" class="Module">category-theory</a>
<a id="384" class="Keyword">open</a> <a id="389" class="Keyword">import</a> <a id="396" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="444" class="Keyword">open</a> <a id="449" class="Keyword">import</a> <a id="456" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="483" class="Keyword">open</a> <a id="488" class="Keyword">import</a> <a id="495" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="535" class="Keyword">open</a> <a id="540" class="Keyword">import</a> <a id="547" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="596" class="Keyword">open</a> <a id="601" class="Keyword">import</a> <a id="608" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="651" class="Keyword">open</a> <a id="656" class="Keyword">import</a> <a id="663" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="699" class="Keyword">open</a> <a id="704" class="Keyword">import</a> <a id="711" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="756" class="Keyword">open</a> <a id="761" class="Keyword">import</a> <a id="768" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="807" class="Keyword">open</a> <a id="812" class="Keyword">import</a> <a id="819" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="890" class="Keyword">open</a> <a id="895" class="Keyword">import</a> <a id="902" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="942" class="Keyword">open</a> <a id="947" class="Keyword">import</a> <a id="954" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="1003" class="Keyword">open</a> <a id="1008" class="Keyword">import</a> <a id="1015" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="1058" class="Keyword">open</a> <a id="1063" class="Keyword">import</a> <a id="1070" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="1103" class="Keyword">open</a> <a id="1108" class="Keyword">import</a> <a id="1115" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="1151" class="Keyword">open</a> <a id="1156" class="Keyword">import</a> <a id="1163" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="1213" class="Keyword">open</a> <a id="1218" class="Keyword">import</a> <a id="1225" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="1273" class="Keyword">open</a> <a id="1278" class="Keyword">import</a> <a id="1285" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="1342" class="Keyword">open</a> <a id="1347" class="Keyword">import</a> <a id="1354" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="1405" class="Keyword">open</a> <a id="1410" class="Keyword">import</a> <a id="1417" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="1468" class="Keyword">open</a> <a id="1473" class="Keyword">import</a> <a id="1480" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="1540" class="Keyword">open</a> <a id="1545" class="Keyword">import</a> <a id="1552" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="1606" class="Keyword">open</a> <a id="1611" class="Keyword">import</a> <a id="1618" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="1690" class="Keyword">open</a> <a id="1695" class="Keyword">import</a> <a id="1702" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="1727" class="Keyword">open</a> <a id="1732" class="Keyword">import</a> <a id="1739" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="1788" class="Keyword">open</a> <a id="1793" class="Keyword">import</a> <a id="1800" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="1843" class="Keyword">open</a> <a id="1848" class="Keyword">import</a> <a id="1855" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="1905" class="Keyword">open</a> <a id="1910" class="Keyword">import</a> <a id="1917" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="1964" class="Keyword">open</a> <a id="1969" class="Keyword">import</a> <a id="1976" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="2019" class="Keyword">open</a> <a id="2024" class="Keyword">import</a> <a id="2031" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="2075" class="Keyword">open</a> <a id="2080" class="Keyword">import</a> <a id="2087" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="2132" class="Keyword">open</a> <a id="2137" class="Keyword">import</a> <a id="2144" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="2196" class="Keyword">open</a> <a id="2201" class="Keyword">import</a> <a id="2208" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="2249" class="Keyword">open</a> <a id="2254" class="Keyword">import</a> <a id="2261" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="2306" class="Keyword">open</a> <a id="2311" class="Keyword">import</a> <a id="2318" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="2361" class="Keyword">open</a> <a id="2366" class="Keyword">import</a> <a id="2373" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="2423" class="Keyword">open</a> <a id="2428" class="Keyword">import</a> <a id="2435" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="2482" class="Keyword">open</a> <a id="2487" class="Keyword">import</a> <a id="2494" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="2551" class="Keyword">open</a> <a id="2556" class="Keyword">import</a> <a id="2563" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="2617" class="Keyword">open</a> <a id="2622" class="Keyword">import</a> <a id="2629" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="2689" class="Keyword">open</a> <a id="2694" class="Keyword">import</a> <a id="2701" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="2744" class="Keyword">open</a> <a id="2749" class="Keyword">import</a> <a id="2756" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="2806" class="Keyword">open</a> <a id="2811" class="Keyword">import</a> <a id="2818" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="2878" class="Keyword">open</a> <a id="2883" class="Keyword">import</a> <a id="2890" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="2939" class="Keyword">open</a> <a id="2944" class="Keyword">import</a> <a id="2951" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="3007" class="Keyword">open</a> <a id="3012" class="Keyword">import</a> <a id="3019" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="3055" class="Keyword">open</a> <a id="3060" class="Keyword">import</a> <a id="3067" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="3111" class="Keyword">open</a> <a id="3116" class="Keyword">import</a> <a id="3123" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="3167" class="Keyword">open</a> <a id="3172" class="Keyword">import</a> <a id="3179" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="3229" class="Keyword">open</a> <a id="3234" class="Keyword">import</a> <a id="3241" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="3287" class="Keyword">open</a> <a id="3292" class="Keyword">import</a> <a id="3299" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="3334" class="Keyword">open</a> <a id="3339" class="Keyword">import</a> <a id="3346" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="3391" class="Keyword">open</a> <a id="3396" class="Keyword">import</a> <a id="3403" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="3461" class="Keyword">open</a> <a id="3466" class="Keyword">import</a> <a id="3473" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="3538" class="Keyword">open</a> <a id="3543" class="Keyword">import</a> <a id="3550" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="3595" class="Keyword">open</a> <a id="3600" class="Keyword">import</a> <a id="3607" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="3659" class="Keyword">open</a> <a id="3664" class="Keyword">import</a> <a id="3671" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="3729" class="Keyword">open</a> <a id="3734" class="Keyword">import</a> <a id="3741" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="3787" class="Keyword">open</a> <a id="3792" class="Keyword">import</a> <a id="3799" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="3833" class="Keyword">open</a> <a id="3838" class="Keyword">import</a> <a id="3845" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="3890" class="Keyword">open</a> <a id="3895" class="Keyword">import</a> <a id="3902" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="3956" class="Keyword">open</a> <a id="3961" class="Keyword">import</a> <a id="3968" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="4034" class="Keyword">open</a> <a id="4039" class="Keyword">import</a> <a id="4046" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="4090" class="Keyword">open</a> <a id="4095" class="Keyword">import</a> <a id="4102" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="4151" class="Keyword">open</a> <a id="4156" class="Keyword">import</a> <a id="4163" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="4219" class="Keyword">open</a> <a id="4224" class="Keyword">import</a> <a id="4231" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="4272" class="Keyword">open</a> <a id="4277" class="Keyword">import</a> <a id="4284" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="4343" class="Keyword">open</a> <a id="4348" class="Keyword">import</a> <a id="4355" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="4394" class="Keyword">open</a> <a id="4399" class="Keyword">import</a> <a id="4406" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="4459" class="Keyword">open</a> <a id="4464" class="Keyword">import</a> <a id="4471" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="4528" class="Keyword">open</a> <a id="4533" class="Keyword">import</a> <a id="4540" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="4582" class="Keyword">open</a> <a id="4587" class="Keyword">import</a> <a id="4594" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="4645" class="Keyword">open</a> <a id="4650" class="Keyword">import</a> <a id="4657" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="4715" class="Keyword">open</a> <a id="4720" class="Keyword">import</a> <a id="4727" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="4791" class="Keyword">open</a> <a id="4796" class="Keyword">import</a> <a id="4803" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="4856" class="Keyword">open</a> <a id="4861" class="Keyword">import</a> <a id="4868" href="elementary-number-theory.skipping-element-standard-finite-type.html" class="Module">elementary-number-theory.skipping-element-standard-finite-type</a>
<a id="4931" class="Keyword">open</a> <a id="4936" class="Keyword">import</a> <a id="4943" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="5004" class="Keyword">open</a> <a id="5009" class="Keyword">import</a> <a id="5016" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="5074" class="Keyword">open</a> <a id="5079" class="Keyword">import</a> <a id="5086" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="5135" class="Keyword">open</a> <a id="5140" class="Keyword">import</a> <a id="5147" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="5191" class="Keyword">open</a> <a id="5196" class="Keyword">import</a> <a id="5203" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="5250" class="Keyword">open</a> <a id="5255" class="Keyword">import</a> <a id="5262" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="5322" class="Keyword">open</a> <a id="5327" class="Keyword">import</a> <a id="5334" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="5388" class="Keyword">open</a> <a id="5393" class="Keyword">import</a> <a id="5400" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="5461" class="Keyword">open</a> <a id="5466" class="Keyword">import</a> <a id="5473" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="5536" class="Keyword">open</a> <a id="5541" class="Keyword">import</a> <a id="5548" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="5613" class="Keyword">open</a> <a id="5618" class="Keyword">import</a> <a id="5625" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="5733" class="Keyword">open</a> <a id="5738" class="Keyword">import</a> <a id="5745" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="5765" class="Keyword">open</a> <a id="5770" class="Keyword">import</a> <a id="5777" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="5823" class="Keyword">open</a> <a id="5828" class="Keyword">import</a> <a id="5835" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="5881" class="Keyword">open</a> <a id="5886" class="Keyword">import</a> <a id="5893" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="5927" class="Keyword">open</a> <a id="5932" class="Keyword">import</a> <a id="5939" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="5979" class="Keyword">open</a> <a id="5984" class="Keyword">import</a> <a id="5991" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="6054" class="Keyword">open</a> <a id="6059" class="Keyword">import</a> <a id="6066" href="foundation.html" class="Module">foundation</a>
<a id="6077" class="Keyword">open</a> <a id="6082" class="Keyword">import</a> <a id="6089" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="6107" class="Keyword">open</a> <a id="6112" class="Keyword">import</a> <a id="6119" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="6138" class="Keyword">open</a> <a id="6143" class="Keyword">import</a> <a id="6150" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="6169" class="Keyword">open</a> <a id="6174" class="Keyword">import</a> <a id="6181" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="6225" class="Keyword">open</a> <a id="6230" class="Keyword">import</a> <a id="6237" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="6262" class="Keyword">open</a> <a id="6267" class="Keyword">import</a> <a id="6274" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="6301" class="Keyword">open</a> <a id="6306" class="Keyword">import</a> <a id="6313" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="6342" class="Keyword">open</a> <a id="6347" class="Keyword">import</a> <a id="6354" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="6385" class="Keyword">open</a> <a id="6390" class="Keyword">import</a> <a id="6397" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="6425" class="Keyword">open</a> <a id="6430" class="Keyword">import</a> <a id="6437" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="6467" class="Keyword">open</a> <a id="6472" class="Keyword">import</a> <a id="6479" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="6499" class="Keyword">open</a> <a id="6504" class="Keyword">import</a> <a id="6511" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="6548" class="Keyword">open</a> <a id="6553" class="Keyword">import</a> <a id="6560" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="6595" class="Keyword">open</a> <a id="6600" class="Keyword">import</a> <a id="6607" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="6665" class="Keyword">open</a> <a id="6670" class="Keyword">import</a> <a id="6677" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="6715" class="Keyword">open</a> <a id="6720" class="Keyword">import</a> <a id="6727" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="6756" class="Keyword">open</a> <a id="6761" class="Keyword">import</a> <a id="6768" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="6791" class="Keyword">open</a> <a id="6796" class="Keyword">import</a> <a id="6803" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="6826" class="Keyword">open</a> <a id="6831" class="Keyword">import</a> <a id="6838" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="6880" class="Keyword">open</a> <a id="6885" class="Keyword">import</a> <a id="6892" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="6924" class="Keyword">open</a> <a id="6929" class="Keyword">import</a> <a id="6936" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="6963" class="Keyword">open</a> <a id="6968" class="Keyword">import</a> <a id="6975" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="7000" class="Keyword">open</a> <a id="7005" class="Keyword">import</a> <a id="7012" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="7041" class="Keyword">open</a> <a id="7046" class="Keyword">import</a> <a id="7053" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="7083" class="Keyword">open</a> <a id="7088" class="Keyword">import</a> <a id="7095" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="7122" class="Keyword">open</a> <a id="7127" class="Keyword">import</a> <a id="7134" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="7153" class="Keyword">open</a> <a id="7158" class="Keyword">import</a> <a id="7165" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="7211" class="Keyword">open</a> <a id="7216" class="Keyword">import</a> <a id="7223" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="7265" class="Keyword">open</a> <a id="7270" class="Keyword">import</a> <a id="7277" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="7309" class="Keyword">open</a> <a id="7314" class="Keyword">import</a> <a id="7321" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="7351" class="Keyword">open</a> <a id="7356" class="Keyword">import</a> <a id="7363" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="7389" class="Keyword">open</a> <a id="7394" class="Keyword">import</a> <a id="7401" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="7435" class="Keyword">open</a> <a id="7440" class="Keyword">import</a> <a id="7447" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="7477" class="Keyword">open</a> <a id="7482" class="Keyword">import</a> <a id="7489" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="7516" class="Keyword">open</a> <a id="7521" class="Keyword">import</a> <a id="7528" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="7560" class="Keyword">open</a> <a id="7565" class="Keyword">import</a> <a id="7572" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="7606" class="Keyword">open</a> <a id="7611" class="Keyword">import</a> <a id="7618" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="7641" class="Keyword">open</a> <a id="7646" class="Keyword">import</a> <a id="7653" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="7723" class="Keyword">open</a> <a id="7728" class="Keyword">import</a> <a id="7735" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="7805" class="Keyword">open</a> <a id="7810" class="Keyword">import</a> <a id="7817" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="7844" class="Keyword">open</a> <a id="7849" class="Keyword">import</a> <a id="7856" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="7904" class="Keyword">open</a> <a id="7909" class="Keyword">import</a> <a id="7916" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="7956" class="Keyword">open</a> <a id="7961" class="Keyword">import</a> <a id="7968" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="7990" class="Keyword">open</a> <a id="7995" class="Keyword">import</a> <a id="8002" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="8025" class="Keyword">open</a> <a id="8030" class="Keyword">import</a> <a id="8037" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="8082" class="Keyword">open</a> <a id="8087" class="Keyword">import</a> <a id="8094" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="8138" class="Keyword">open</a> <a id="8143" class="Keyword">import</a> <a id="8150" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="8186" class="Keyword">open</a> <a id="8191" class="Keyword">import</a> <a id="8198" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="8243" class="Keyword">open</a> <a id="8248" class="Keyword">import</a> <a id="8255" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="8296" class="Keyword">open</a> <a id="8301" class="Keyword">import</a> <a id="8308" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="8343" class="Keyword">open</a> <a id="8348" class="Keyword">import</a> <a id="8355" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="8386" class="Keyword">open</a> <a id="8391" class="Keyword">import</a> <a id="8398" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="8431" class="Keyword">open</a> <a id="8436" class="Keyword">import</a> <a id="8443" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="8476" class="Keyword">open</a> <a id="8481" class="Keyword">import</a> <a id="8488" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="8518" class="Keyword">open</a> <a id="8523" class="Keyword">import</a> <a id="8530" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="8554" class="Keyword">open</a> <a id="8559" class="Keyword">import</a> <a id="8566" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="8604" class="Keyword">open</a> <a id="8609" class="Keyword">import</a> <a id="8616" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="8647" class="Keyword">open</a> <a id="8652" class="Keyword">import</a> <a id="8659" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="8684" class="Keyword">open</a> <a id="8689" class="Keyword">import</a> <a id="8696" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="8724" class="Keyword">open</a> <a id="8729" class="Keyword">import</a> <a id="8736" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="8760" class="Keyword">open</a> <a id="8765" class="Keyword">import</a> <a id="8772" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="8798" class="Keyword">open</a> <a id="8803" class="Keyword">import</a> <a id="8810" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="8845" class="Keyword">open</a> <a id="8850" class="Keyword">import</a> <a id="8857" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="8878" class="Keyword">open</a> <a id="8883" class="Keyword">import</a> <a id="8890" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="8939" class="Keyword">open</a> <a id="8944" class="Keyword">import</a> <a id="8951" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="8992" class="Keyword">open</a> <a id="8997" class="Keyword">import</a> <a id="9004" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="9054" class="Keyword">open</a> <a id="9059" class="Keyword">import</a> <a id="9066" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="9112" class="Keyword">open</a> <a id="9117" class="Keyword">import</a> <a id="9124" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="9164" class="Keyword">open</a> <a id="9169" class="Keyword">import</a> <a id="9176" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="9226" class="Keyword">open</a> <a id="9231" class="Keyword">import</a> <a id="9238" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="9277" class="Keyword">open</a> <a id="9282" class="Keyword">import</a> <a id="9289" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="9329" class="Keyword">open</a> <a id="9334" class="Keyword">import</a> <a id="9341" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="9374" class="Keyword">open</a> <a id="9379" class="Keyword">import</a> <a id="9386" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="9435" class="Keyword">open</a> <a id="9440" class="Keyword">import</a> <a id="9447" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="9472" class="Keyword">open</a> <a id="9477" class="Keyword">import</a> <a id="9484" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="9506" class="Keyword">open</a> <a id="9511" class="Keyword">import</a> <a id="9518" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="9546" class="Keyword">open</a> <a id="9551" class="Keyword">import</a> <a id="9558" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="9584" class="Keyword">open</a> <a id="9589" class="Keyword">import</a> <a id="9596" href="foundation.images.html" class="Module">foundation.images</a>
<a id="9614" class="Keyword">open</a> <a id="9619" class="Keyword">import</a> <a id="9626" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="9661" class="Keyword">open</a> <a id="9666" class="Keyword">import</a> <a id="9673" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="9700" class="Keyword">open</a> <a id="9705" class="Keyword">import</a> <a id="9712" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="9768" class="Keyword">open</a> <a id="9773" class="Keyword">import</a> <a id="9780" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="9809" class="Keyword">open</a> <a id="9814" class="Keyword">import</a> <a id="9821" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="9851" class="Keyword">open</a> <a id="9856" class="Keyword">import</a> <a id="9863" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="9889" class="Keyword">open</a> <a id="9894" class="Keyword">import</a> <a id="9901" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="9928" class="Keyword">open</a> <a id="9933" class="Keyword">import</a> <a id="9940" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="9963" class="Keyword">open</a> <a id="9968" class="Keyword">import</a> <a id="9975" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="10002" class="Keyword">open</a> <a id="10007" class="Keyword">import</a> <a id="10014" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="10046" class="Keyword">open</a> <a id="10051" class="Keyword">import</a> <a id="10058" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="10092" class="Keyword">open</a> <a id="10097" class="Keyword">import</a> <a id="10104" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="10144" class="Keyword">open</a> <a id="10149" class="Keyword">import</a> <a id="10156" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="10187" class="Keyword">open</a> <a id="10192" class="Keyword">import</a> <a id="10199" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="10231" class="Keyword">open</a> <a id="10236" class="Keyword">import</a> <a id="10243" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="10260" class="Keyword">open</a> <a id="10265" class="Keyword">import</a> <a id="10272" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="10297" class="Keyword">open</a> <a id="10302" class="Keyword">import</a> <a id="10309" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="10338" class="Keyword">open</a> <a id="10343" class="Keyword">import</a> <a id="10350" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="10375" class="Keyword">open</a> <a id="10380" class="Keyword">import</a> <a id="10387" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="10408" class="Keyword">open</a> <a id="10413" class="Keyword">import</a> <a id="10420" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="10440" class="Keyword">open</a> <a id="10445" class="Keyword">import</a> <a id="10452" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="10486" class="Keyword">open</a> <a id="10491" class="Keyword">import</a> <a id="10498" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="10522" class="Keyword">open</a> <a id="10527" class="Keyword">import</a> <a id="10534" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="10561" class="Keyword">open</a> <a id="10566" class="Keyword">import</a> <a id="10573" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="10608" class="Keyword">open</a> <a id="10613" class="Keyword">import</a> <a id="10620" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="10660" class="Keyword">open</a> <a id="10665" class="Keyword">import</a> <a id="10672" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="10702" class="Keyword">open</a> <a id="10707" class="Keyword">import</a> <a id="10714" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="10751" class="Keyword">open</a> <a id="10756" class="Keyword">import</a> <a id="10763" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="10787" class="Keyword">open</a> <a id="10792" class="Keyword">import</a> <a id="10799" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="10820" class="Keyword">open</a> <a id="10825" class="Keyword">import</a> <a id="10832" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="10867" class="Keyword">open</a> <a id="10872" class="Keyword">import</a> <a id="10879" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="10916" class="Keyword">open</a> <a id="10921" class="Keyword">import</a> <a id="10928" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="10977" class="Keyword">open</a> <a id="10982" class="Keyword">import</a> <a id="10989" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="11012" class="Keyword">open</a> <a id="11017" class="Keyword">import</a> <a id="11024" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="11047" class="Keyword">open</a> <a id="11052" class="Keyword">import</a> <a id="11059" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="11087" class="Keyword">open</a> <a id="11092" class="Keyword">import</a> <a id="11099" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="11119" class="Keyword">open</a> <a id="11124" class="Keyword">import</a> <a id="11131" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="11162" class="Keyword">open</a> <a id="11167" class="Keyword">import</a> <a id="11174" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="11201" class="Keyword">open</a> <a id="11206" class="Keyword">import</a> <a id="11213" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="11229" class="Keyword">open</a> <a id="11234" class="Keyword">import</a> <a id="11241" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="11272" class="Keyword">open</a> <a id="11277" class="Keyword">import</a> <a id="11284" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="11301" class="Keyword">open</a> <a id="11306" class="Keyword">import</a> <a id="11313" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="11335" class="Keyword">open</a> <a id="11340" class="Keyword">import</a> <a id="11347" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="11374" class="Keyword">open</a> <a id="11379" class="Keyword">import</a> <a id="11386" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="11409" class="Keyword">open</a> <a id="11414" class="Keyword">import</a> <a id="11421" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="11448" class="Keyword">open</a> <a id="11453" class="Keyword">import</a> <a id="11460" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="11493" class="Keyword">open</a> <a id="11498" class="Keyword">import</a> <a id="11505" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="11545" class="Keyword">open</a> <a id="11550" class="Keyword">import</a> <a id="11557" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="11578" class="Keyword">open</a> <a id="11583" class="Keyword">import</a> <a id="11590" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="11619" class="Keyword">open</a> <a id="11624" class="Keyword">import</a> <a id="11631" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="11669" class="Keyword">open</a> <a id="11674" class="Keyword">import</a> <a id="11681" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="11701" class="Keyword">open</a> <a id="11706" class="Keyword">import</a> <a id="11713" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="11737" class="Keyword">open</a> <a id="11742" class="Keyword">import</a> <a id="11749" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="11776" class="Keyword">open</a> <a id="11781" class="Keyword">import</a> <a id="11788" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="11818" class="Keyword">open</a> <a id="11823" class="Keyword">import</a> <a id="11830" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="11856" class="Keyword">open</a> <a id="11861" class="Keyword">import</a> <a id="11868" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="11895" class="Keyword">open</a> <a id="11900" class="Keyword">import</a> <a id="11907" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="11936" class="Keyword">open</a> <a id="11941" class="Keyword">import</a> <a id="11948" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="11971" class="Keyword">open</a> <a id="11976" class="Keyword">import</a> <a id="11983" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="12034" class="Keyword">open</a> <a id="12039" class="Keyword">import</a> <a id="12046" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="12089" class="Keyword">open</a> <a id="12094" class="Keyword">import</a> <a id="12101" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="12149" class="Keyword">open</a> <a id="12154" class="Keyword">import</a> <a id="12161" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="12199" class="Keyword">open</a> <a id="12204" class="Keyword">import</a> <a id="12211" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="12248" class="Keyword">open</a> <a id="12253" class="Keyword">import</a> <a id="12260" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="12288" class="Keyword">open</a> <a id="12293" class="Keyword">import</a> <a id="12300" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="12336" class="Keyword">open</a> <a id="12341" class="Keyword">import</a> <a id="12348" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="12386" class="Keyword">open</a> <a id="12391" class="Keyword">import</a> <a id="12398" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="12431" class="Keyword">open</a> <a id="12436" class="Keyword">import</a> <a id="12443" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="12464" class="Keyword">open</a> <a id="12469" class="Keyword">import</a> <a id="12476" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="12530" class="Keyword">open</a> <a id="12535" class="Keyword">import</a> <a id="12542" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="12564" class="Keyword">open</a> <a id="12569" class="Keyword">import</a> <a id="12576" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="12611" class="Keyword">open</a> <a id="12616" class="Keyword">import</a> <a id="12623" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="12653" class="Keyword">open</a> <a id="12658" class="Keyword">import</a> <a id="12665" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="12704" class="Keyword">open</a> <a id="12709" class="Keyword">import</a> <a id="12716" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="12770" class="Keyword">open</a> <a id="12775" class="Keyword">import</a> <a id="12782" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="12828" class="Keyword">open</a> <a id="12833" class="Keyword">import</a> <a id="12840" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="12891" class="Keyword">open</a> <a id="12896" class="Keyword">import</a> <a id="12903" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="12944" class="Keyword">open</a> <a id="12949" class="Keyword">import</a> <a id="12956" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="13001" class="Keyword">open</a> <a id="13006" class="Keyword">import</a> <a id="13013" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="13058" class="Keyword">open</a> <a id="13063" class="Keyword">import</a> <a id="13070" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="13106" class="Keyword">open</a> <a id="13111" class="Keyword">import</a> <a id="13118" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="13154" class="Keyword">open</a> <a id="13159" class="Keyword">import</a> <a id="13166" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="13231" class="Keyword">open</a> <a id="13236" class="Keyword">import</a> <a id="13243" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="13298" class="Keyword">open</a> <a id="13303" class="Keyword">import</a> <a id="13310" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="13350" class="Keyword">open</a> <a id="13355" class="Keyword">import</a> <a id="13362" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="13406" class="Keyword">open</a> <a id="13411" class="Keyword">import</a> <a id="13418" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="13463" class="Keyword">open</a> <a id="13468" class="Keyword">import</a> <a id="13475" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="13516" class="Keyword">open</a> <a id="13521" class="Keyword">import</a> <a id="13528" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="13568" class="Keyword">open</a> <a id="13573" class="Keyword">import</a> <a id="13580" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="13607" class="Keyword">open</a> <a id="13612" class="Keyword">import</a> <a id="13619" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="13646" class="Keyword">open</a> <a id="13651" class="Keyword">import</a> <a id="13658" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="13677" class="Keyword">open</a> <a id="13682" class="Keyword">import</a> <a id="13689" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="13729" class="Keyword">open</a> <a id="13734" class="Keyword">import</a> <a id="13741" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="13806" class="Keyword">open</a> <a id="13811" class="Keyword">import</a> <a id="13818" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="13841" class="Keyword">open</a> <a id="13846" class="Keyword">import</a> <a id="13853" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="13877" class="Keyword">open</a> <a id="13882" class="Keyword">import</a> <a id="13889" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="13929" class="Keyword">open</a> <a id="13934" class="Keyword">import</a> <a id="13941" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="13984" class="Keyword">open</a> <a id="13989" class="Keyword">import</a> <a id="13996" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="14030" class="Keyword">open</a> <a id="14035" class="Keyword">import</a> <a id="14042" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="14072" class="Keyword">open</a> <a id="14077" class="Keyword">import</a> <a id="14084" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="14118" class="Keyword">open</a> <a id="14123" class="Keyword">import</a> <a id="14130" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="14165" class="Keyword">open</a> <a id="14170" class="Keyword">import</a> <a id="14177" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="14214" class="Keyword">open</a> <a id="14219" class="Keyword">import</a> <a id="14226" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="14253" class="Keyword">open</a> <a id="14258" class="Keyword">import</a> <a id="14265" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="14293" class="Keyword">open</a> <a id="14298" class="Keyword">import</a> <a id="14305" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="14354" class="Keyword">open</a> <a id="14359" class="Keyword">import</a> <a id="14366" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="14412" class="Keyword">open</a> <a id="14417" class="Keyword">import</a> <a id="14424" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="14464" class="Keyword">open</a> <a id="14469" class="Keyword">import</a> <a id="14476" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="14514" class="Keyword">open</a> <a id="14519" class="Keyword">import</a> <a id="14526" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="14555" class="Keyword">open</a> <a id="14560" class="Keyword">import</a> <a id="14567" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="14597" class="Keyword">open</a> <a id="14602" class="Keyword">import</a> <a id="14609" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="14640" class="Keyword">open</a> <a id="14645" class="Keyword">import</a> <a id="14652" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="14678" class="Keyword">open</a> <a id="14683" class="Keyword">import</a> <a id="14690" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="14741" class="Keyword">open</a> <a id="14746" class="Keyword">import</a> <a id="14753" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="14807" class="Keyword">open</a> <a id="14812" class="Keyword">import</a> <a id="14819" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="14846" class="Keyword">open</a> <a id="14851" class="Keyword">import</a> <a id="14858" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="14891" class="Keyword">open</a> <a id="14896" class="Keyword">import</a> <a id="14903" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="14934" class="Keyword">open</a> <a id="14939" class="Keyword">import</a> <a id="14946" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="14983" class="Keyword">open</a> <a id="14988" class="Keyword">import</a> <a id="14995" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="15020" class="Keyword">open</a> <a id="15025" class="Keyword">import</a> <a id="15032" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="15064" class="Keyword">open</a> <a id="15069" class="Keyword">import</a> <a id="15076" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="15111" class="Keyword">open</a> <a id="15116" class="Keyword">import</a> <a id="15123" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="15152" class="Keyword">open</a> <a id="15157" class="Keyword">import</a> <a id="15164" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="15192" class="Keyword">open</a> <a id="15197" class="Keyword">import</a> <a id="15204" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="15229" class="Keyword">open</a> <a id="15234" class="Keyword">import</a> <a id="15241" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="15262" class="Keyword">open</a> <a id="15267" class="Keyword">import</a> <a id="15274" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="15310" class="Keyword">open</a> <a id="15315" class="Keyword">import</a> <a id="15322" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="15365" class="Keyword">open</a> <a id="15370" class="Keyword">import</a> <a id="15377" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="15402" class="Keyword">open</a> <a id="15407" class="Keyword">import</a> <a id="15414" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="15445" class="Keyword">open</a> <a id="15450" class="Keyword">import</a> <a id="15457" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="15489" class="Keyword">open</a> <a id="15494" class="Keyword">import</a> <a id="15501" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="15535" class="Keyword">open</a> <a id="15540" class="Keyword">import</a> <a id="15547" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="15603" class="Keyword">open</a> <a id="15608" class="Keyword">import</a> <a id="15615" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="15668" class="Keyword">open</a> <a id="15673" class="Keyword">import</a> <a id="15680" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="15707" class="Keyword">open</a> <a id="15712" class="Keyword">import</a> <a id="15719" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="15781" class="Keyword">open</a> <a id="15786" class="Keyword">import</a> <a id="15793" href="graph-theory.html" class="Module">graph-theory</a>
<a id="15806" class="Keyword">open</a> <a id="15811" class="Keyword">import</a> <a id="15818" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="15847" class="Keyword">open</a> <a id="15852" class="Keyword">import</a> <a id="15859" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="15886" class="Keyword">open</a> <a id="15891" class="Keyword">import</a> <a id="15898" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="15920" class="Keyword">open</a> <a id="15925" class="Keyword">import</a> <a id="15932" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="15962" class="Keyword">open</a> <a id="15967" class="Keyword">import</a> <a id="15974" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="16035" class="Keyword">open</a> <a id="16040" class="Keyword">import</a> <a id="16047" href="group-theory.html" class="Module">group-theory</a>
<a id="16060" class="Keyword">open</a> <a id="16065" class="Keyword">import</a> <a id="16072" href="group-theory.abstract-abelian-groups.html" class="Module">group-theory.abstract-abelian-groups</a>
<a id="16109" class="Keyword">open</a> <a id="16114" class="Keyword">import</a> <a id="16121" href="group-theory.abstract-abelian-subgroups.html" class="Module">group-theory.abstract-abelian-subgroups</a>
<a id="16161" class="Keyword">open</a> <a id="16166" class="Keyword">import</a> <a id="16173" href="group-theory.abstract-group-actions.html" class="Module">group-theory.abstract-group-actions</a>
<a id="16209" class="Keyword">open</a> <a id="16214" class="Keyword">import</a> <a id="16221" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="16257" class="Keyword">open</a> <a id="16262" class="Keyword">import</a> <a id="16269" href="group-theory.abstract-groups.html" class="Module">group-theory.abstract-groups</a>
<a id="16298" class="Keyword">open</a> <a id="16303" class="Keyword">import</a> <a id="16310" href="group-theory.abstract-subgroups.html" class="Module">group-theory.abstract-subgroups</a>
<a id="16342" class="Keyword">open</a> <a id="16347" class="Keyword">import</a> <a id="16354" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="16390" class="Keyword">open</a> <a id="16395" class="Keyword">import</a> <a id="16402" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="16431" class="Keyword">open</a> <a id="16436" class="Keyword">import</a> <a id="16443" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="16475" class="Keyword">open</a> <a id="16480" class="Keyword">import</a> <a id="16487" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="16523" class="Keyword">open</a> <a id="16528" class="Keyword">import</a> <a id="16535" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="16567" class="Keyword">open</a> <a id="16572" class="Keyword">import</a> <a id="16579" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="16606" class="Keyword">open</a> <a id="16611" class="Keyword">import</a> <a id="16618" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="16675" class="Keyword">open</a> <a id="16680" class="Keyword">import</a> <a id="16687" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="16702" class="Keyword">open</a> <a id="16707" class="Keyword">import</a> <a id="16714" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="16738" class="Keyword">open</a> <a id="16743" class="Keyword">import</a> <a id="16750" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="16803" class="Keyword">open</a> <a id="16808" class="Keyword">import</a> <a id="16815" href="order-theory.html" class="Module">order-theory</a>
<a id="16828" class="Keyword">open</a> <a id="16833" class="Keyword">import</a> <a id="16840" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="16867" class="Keyword">open</a> <a id="16872" class="Keyword">import</a> <a id="16879" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="16909" class="Keyword">open</a> <a id="16914" class="Keyword">import</a> <a id="16921" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="16957" class="Keyword">open</a> <a id="16962" class="Keyword">import</a> <a id="16969" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="17002" class="Keyword">open</a> <a id="17007" class="Keyword">import</a> <a id="17014" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="17034" class="Keyword">open</a> <a id="17039" class="Keyword">import</a> <a id="17046" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="17096" class="Keyword">open</a> <a id="17101" class="Keyword">import</a> <a id="17108" href="polytopes.html" class="Module">polytopes</a>
<a id="17118" class="Keyword">open</a> <a id="17123" class="Keyword">import</a> <a id="17130" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="17188" class="Keyword">open</a> <a id="17193" class="Keyword">import</a> <a id="17200" href="ring-theory.html" class="Module">ring-theory</a>
<a id="17212" class="Keyword">open</a> <a id="17217" class="Keyword">import</a> <a id="17224" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="17256" class="Keyword">open</a> <a id="17261" class="Keyword">import</a> <a id="17268" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="17298" class="Keyword">open</a> <a id="17303" class="Keyword">import</a> <a id="17310" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a>
<a id="17329" class="Keyword">open</a> <a id="17334" class="Keyword">import</a> <a id="17341" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="17373" class="Keyword">open</a> <a id="17378" class="Keyword">import</a> <a id="17385" href="ring-theory.rings-with-properties.html" class="Module">ring-theory.rings-with-properties</a>
<a id="17419" class="Keyword">open</a> <a id="17424" class="Keyword">import</a> <a id="17431" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="17492" class="Keyword">open</a> <a id="17497" class="Keyword">import</a> <a id="17504" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="17530" class="Keyword">open</a> <a id="17535" class="Keyword">import</a> <a id="17542" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="17581" class="Keyword">open</a> <a id="17586" class="Keyword">import</a> <a id="17593" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="17631" class="Keyword">open</a> <a id="17636" class="Keyword">import</a> <a id="17643" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="17689" class="Keyword">open</a> <a id="17694" class="Keyword">import</a> <a id="17701" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="17738" class="Keyword">open</a> <a id="17743" class="Keyword">import</a> <a id="17750" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="17790" class="Keyword">open</a> <a id="17795" class="Keyword">import</a> <a id="17802" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="17841" class="Keyword">open</a> <a id="17846" class="Keyword">import</a> <a id="17853" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="17886" class="Keyword">open</a> <a id="17891" class="Keyword">import</a> <a id="17898" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="17937" class="Keyword">open</a> <a id="17942" class="Keyword">import</a> <a id="17949" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="17994" class="Keyword">open</a> <a id="17999" class="Keyword">import</a> <a id="18006" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="18058" class="Keyword">open</a> <a id="18063" class="Keyword">import</a> <a id="18070" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="18118" class="Keyword">open</a> <a id="18123" class="Keyword">import</a> <a id="18130" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="18170" class="Keyword">open</a> <a id="18175" class="Keyword">import</a> <a id="18182" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="18229" class="Keyword">open</a> <a id="18234" class="Keyword">import</a> <a id="18241" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="18279" class="Keyword">open</a> <a id="18284" class="Keyword">import</a> <a id="18291" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="18345" class="Keyword">open</a> <a id="18350" class="Keyword">import</a> <a id="18357" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="18404" class="Keyword">open</a> <a id="18409" class="Keyword">import</a> <a id="18416" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="18468" class="Keyword">open</a> <a id="18473" class="Keyword">import</a> <a id="18480" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="18525" class="Keyword">open</a> <a id="18530" class="Keyword">import</a> <a id="18537" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="18576" class="Keyword">open</a> <a id="18581" class="Keyword">import</a> <a id="18588" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="18628" class="Keyword">open</a> <a id="18633" class="Keyword">import</a> <a id="18640" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="18673" class="Keyword">open</a> <a id="18678" class="Keyword">import</a> <a id="18685" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="18730" class="Keyword">open</a> <a id="18735" class="Keyword">import</a> <a id="18742" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="18818" class="Keyword">open</a> <a id="18823" class="Keyword">import</a> <a id="18830" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="18892" class="Keyword">open</a> <a id="18897" class="Keyword">import</a> <a id="18904" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="18928" class="Keyword">open</a> <a id="18933" class="Keyword">import</a> <a id="18940" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="18980" class="Keyword">open</a> <a id="18985" class="Keyword">import</a> <a id="18992" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="19031" class="Keyword">open</a> <a id="19036" class="Keyword">import</a> <a id="19043" href="univalent-combinatorics.cartesian-product-finite-types.html" class="Module">univalent-combinatorics.cartesian-product-finite-types</a>
<a id="19098" class="Keyword">open</a> <a id="19103" class="Keyword">import</a> <a id="19110" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="19157" class="Keyword">open</a> <a id="19162" class="Keyword">import</a> <a id="19169" href="univalent-combinatorics.coproduct-finite-types.html" class="Module">univalent-combinatorics.coproduct-finite-types</a>
<a id="19216" class="Keyword">open</a> <a id="19221" class="Keyword">import</a> <a id="19228" href="univalent-combinatorics.counting-cartesian-product-types.html" class="Module">univalent-combinatorics.counting-cartesian-product-types</a>
<a id="19285" class="Keyword">open</a> <a id="19290" class="Keyword">import</a> <a id="19297" href="univalent-combinatorics.counting-coproduct-types.html" class="Module">univalent-combinatorics.counting-coproduct-types</a>
<a id="19346" class="Keyword">open</a> <a id="19351" class="Keyword">import</a> <a id="19358" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="19410" class="Keyword">open</a> <a id="19415" class="Keyword">import</a> <a id="19422" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="19480" class="Keyword">open</a> <a id="19485" class="Keyword">import</a> <a id="19492" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="19546" class="Keyword">open</a> <a id="19551" class="Keyword">import</a> <a id="19558" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="19606" class="Keyword">open</a> <a id="19611" class="Keyword">import</a> <a id="19618" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="19666" class="Keyword">open</a> <a id="19671" class="Keyword">import</a> <a id="19678" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="19717" class="Keyword">open</a> <a id="19722" class="Keyword">import</a> <a id="19729" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="19762" class="Keyword">open</a> <a id="19767" class="Keyword">import</a> <a id="19774" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="19833" class="Keyword">open</a> <a id="19838" class="Keyword">import</a> <a id="19845" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="19900" class="Keyword">open</a> <a id="19905" class="Keyword">import</a> <a id="19912" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="19955" class="Keyword">open</a> <a id="19960" class="Keyword">import</a> <a id="19967" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="20022" class="Keyword">open</a> <a id="20027" class="Keyword">import</a> <a id="20034" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="20085" class="Keyword">open</a> <a id="20090" class="Keyword">import</a> <a id="20097" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="20175" class="Keyword">open</a> <a id="20180" class="Keyword">import</a> <a id="20187" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="20227" class="Keyword">open</a> <a id="20232" class="Keyword">import</a> <a id="20239" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="20296" class="Keyword">open</a> <a id="20301" class="Keyword">import</a> <a id="20308" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="20343" class="Keyword">open</a> <a id="20348" class="Keyword">import</a> <a id="20355" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="20401" class="Keyword">open</a> <a id="20406" class="Keyword">import</a> <a id="20413" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="20468" class="Keyword">open</a> <a id="20473" class="Keyword">import</a> <a id="20480" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="20539" class="Keyword">open</a> <a id="20544" class="Keyword">import</a> <a id="20551" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="20588" class="Keyword">open</a> <a id="20593" class="Keyword">import</a> <a id="20600" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="20660" class="Keyword">open</a> <a id="20665" class="Keyword">import</a> <a id="20672" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="20710" class="Keyword">open</a> <a id="20715" class="Keyword">import</a> <a id="20722" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="20774" class="Keyword">open</a> <a id="20779" class="Keyword">import</a> <a id="20786" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="20832" class="Keyword">open</a> <a id="20837" class="Keyword">import</a> <a id="20844" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="20889" class="Keyword">open</a> <a id="20894" class="Keyword">import</a> <a id="20901" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="20938" class="Keyword">open</a> <a id="20943" class="Keyword">import</a> <a id="20950" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="20999" class="Keyword">open</a> <a id="21004" class="Keyword">import</a> <a id="21011" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="21049" class="Keyword">open</a> <a id="21054" class="Keyword">import</a> <a id="21061" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="21116" class="Keyword">open</a> <a id="21121" class="Keyword">import</a> <a id="21128" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="21167" class="Keyword">open</a> <a id="21172" class="Keyword">import</a> <a id="21179" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="21209" class="Keyword">open</a> <a id="21214" class="Keyword">import</a> <a id="21221" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="21251" class="Keyword">open</a> <a id="21256" class="Keyword">import</a> <a id="21263" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="21303" class="Keyword">open</a> <a id="21308" class="Keyword">import</a> <a id="21315" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="21360" class="Keyword">open</a> <a id="21365" class="Keyword">import</a> <a id="21372" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="21422" class="Keyword">open</a> <a id="21427" class="Keyword">import</a> <a id="21434" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="21472" class="Keyword">open</a> <a id="21477" class="Keyword">import</a> <a id="21484" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="21533" class="Keyword">open</a> <a id="21538" class="Keyword">import</a> <a id="21545" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="21598" class="Keyword">open</a> <a id="21603" class="Keyword">import</a> <a id="21610" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="21656" class="Keyword">open</a> <a id="21661" class="Keyword">import</a> <a id="21668" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="21714" class="Keyword">open</a> <a id="21719" class="Keyword">import</a> <a id="21726" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="21774" class="Keyword">open</a> <a id="21779" class="Keyword">import</a> <a id="21786" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="21864" class="Keyword">open</a> <a id="21869" class="Keyword">import</a> <a id="21876" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="21944" class="Keyword">open</a> <a id="21949" class="Keyword">import</a> <a id="21956" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="21969" class="Keyword">open</a> <a id="21974" class="Keyword">import</a> <a id="21981" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="22001" class="Keyword">open</a> <a id="22006" class="Keyword">import</a> <a id="22013" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="22064" class="Keyword">open</a> <a id="22069" class="Keyword">import</a> <a id="22076" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="22101" class="Keyword">open</a> <a id="22106" class="Keyword">import</a> <a id="22113" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="22139" class="Keyword">open</a> <a id="22144" class="Keyword">import</a> <a id="22151" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

