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
<a id="1964" class="Keyword">open</a> <a id="1969" class="Keyword">import</a> <a id="1976" href="elementary-number-theory.classical-finite-types.html" class="Module">elementary-number-theory.classical-finite-types</a>
<a id="2024" class="Keyword">open</a> <a id="2029" class="Keyword">import</a> <a id="2036" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="2079" class="Keyword">open</a> <a id="2084" class="Keyword">import</a> <a id="2091" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="2135" class="Keyword">open</a> <a id="2140" class="Keyword">import</a> <a id="2147" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="2192" class="Keyword">open</a> <a id="2197" class="Keyword">import</a> <a id="2204" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="2256" class="Keyword">open</a> <a id="2261" class="Keyword">import</a> <a id="2268" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="2328" class="Keyword">open</a> <a id="2333" class="Keyword">import</a> <a id="2340" href="elementary-number-theory.decidable-dependent-pair-types.html" class="Module">elementary-number-theory.decidable-dependent-pair-types</a>
<a id="2396" class="Keyword">open</a> <a id="2401" class="Keyword">import</a> <a id="2408" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="2453" class="Keyword">open</a> <a id="2458" class="Keyword">import</a> <a id="2465" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="2508" class="Keyword">open</a> <a id="2513" class="Keyword">import</a> <a id="2520" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="2570" class="Keyword">open</a> <a id="2575" class="Keyword">import</a> <a id="2582" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="2629" class="Keyword">open</a> <a id="2634" class="Keyword">import</a> <a id="2641" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="2695" class="Keyword">open</a> <a id="2700" class="Keyword">import</a> <a id="2707" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="2767" class="Keyword">open</a> <a id="2772" class="Keyword">import</a> <a id="2779" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="2822" class="Keyword">open</a> <a id="2827" class="Keyword">import</a> <a id="2834" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="2884" class="Keyword">open</a> <a id="2889" class="Keyword">import</a> <a id="2896" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="2956" class="Keyword">open</a> <a id="2961" class="Keyword">import</a> <a id="2968" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="3017" class="Keyword">open</a> <a id="3022" class="Keyword">import</a> <a id="3029" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="3085" class="Keyword">open</a> <a id="3090" class="Keyword">import</a> <a id="3097" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="3133" class="Keyword">open</a> <a id="3138" class="Keyword">import</a> <a id="3145" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="3189" class="Keyword">open</a> <a id="3194" class="Keyword">import</a> <a id="3201" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="3245" class="Keyword">open</a> <a id="3250" class="Keyword">import</a> <a id="3257" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="3307" class="Keyword">open</a> <a id="3312" class="Keyword">import</a> <a id="3319" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="3365" class="Keyword">open</a> <a id="3370" class="Keyword">import</a> <a id="3377" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="3412" class="Keyword">open</a> <a id="3417" class="Keyword">import</a> <a id="3424" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="3469" class="Keyword">open</a> <a id="3474" class="Keyword">import</a> <a id="3481" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="3539" class="Keyword">open</a> <a id="3544" class="Keyword">import</a> <a id="3551" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="3616" class="Keyword">open</a> <a id="3621" class="Keyword">import</a> <a id="3628" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="3673" class="Keyword">open</a> <a id="3678" class="Keyword">import</a> <a id="3685" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="3737" class="Keyword">open</a> <a id="3742" class="Keyword">import</a> <a id="3749" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="3807" class="Keyword">open</a> <a id="3812" class="Keyword">import</a> <a id="3819" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="3865" class="Keyword">open</a> <a id="3870" class="Keyword">import</a> <a id="3877" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="3911" class="Keyword">open</a> <a id="3916" class="Keyword">import</a> <a id="3923" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="3968" class="Keyword">open</a> <a id="3973" class="Keyword">import</a> <a id="3980" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="4034" class="Keyword">open</a> <a id="4039" class="Keyword">import</a> <a id="4046" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="4112" class="Keyword">open</a> <a id="4117" class="Keyword">import</a> <a id="4124" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="4168" class="Keyword">open</a> <a id="4173" class="Keyword">import</a> <a id="4180" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="4229" class="Keyword">open</a> <a id="4234" class="Keyword">import</a> <a id="4241" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="4297" class="Keyword">open</a> <a id="4302" class="Keyword">import</a> <a id="4309" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="4350" class="Keyword">open</a> <a id="4355" class="Keyword">import</a> <a id="4362" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="4421" class="Keyword">open</a> <a id="4426" class="Keyword">import</a> <a id="4433" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="4472" class="Keyword">open</a> <a id="4477" class="Keyword">import</a> <a id="4484" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="4537" class="Keyword">open</a> <a id="4542" class="Keyword">import</a> <a id="4549" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="4606" class="Keyword">open</a> <a id="4611" class="Keyword">import</a> <a id="4618" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="4660" class="Keyword">open</a> <a id="4665" class="Keyword">import</a> <a id="4672" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="4723" class="Keyword">open</a> <a id="4728" class="Keyword">import</a> <a id="4735" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="4793" class="Keyword">open</a> <a id="4798" class="Keyword">import</a> <a id="4805" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="4869" class="Keyword">open</a> <a id="4874" class="Keyword">import</a> <a id="4881" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="4934" class="Keyword">open</a> <a id="4939" class="Keyword">import</a> <a id="4946" href="elementary-number-theory.retracts-of-standard-finite-types.html" class="Module">elementary-number-theory.retracts-of-standard-finite-types</a>
<a id="5005" class="Keyword">open</a> <a id="5010" class="Keyword">import</a> <a id="5017" href="elementary-number-theory.skipping-element-standard-finite-type.html" class="Module">elementary-number-theory.skipping-element-standard-finite-type</a>
<a id="5080" class="Keyword">open</a> <a id="5085" class="Keyword">import</a> <a id="5092" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="5153" class="Keyword">open</a> <a id="5158" class="Keyword">import</a> <a id="5165" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="5223" class="Keyword">open</a> <a id="5228" class="Keyword">import</a> <a id="5235" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="5284" class="Keyword">open</a> <a id="5289" class="Keyword">import</a> <a id="5296" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="5340" class="Keyword">open</a> <a id="5345" class="Keyword">import</a> <a id="5352" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="5399" class="Keyword">open</a> <a id="5404" class="Keyword">import</a> <a id="5411" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="5471" class="Keyword">open</a> <a id="5476" class="Keyword">import</a> <a id="5483" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="5537" class="Keyword">open</a> <a id="5542" class="Keyword">import</a> <a id="5549" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="5614" class="Keyword">open</a> <a id="5619" class="Keyword">import</a> <a id="5626" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="5734" class="Keyword">open</a> <a id="5739" class="Keyword">import</a> <a id="5746" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="5792" class="Keyword">open</a> <a id="5797" class="Keyword">import</a> <a id="5804" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="5850" class="Keyword">open</a> <a id="5855" class="Keyword">import</a> <a id="5862" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="5896" class="Keyword">open</a> <a id="5901" class="Keyword">import</a> <a id="5908" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="5948" class="Keyword">open</a> <a id="5953" class="Keyword">import</a> <a id="5960" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="6023" class="Keyword">open</a> <a id="6028" class="Keyword">import</a> <a id="6035" href="foundation.html" class="Module">foundation</a>
<a id="6046" class="Keyword">open</a> <a id="6051" class="Keyword">import</a> <a id="6058" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="6076" class="Keyword">open</a> <a id="6081" class="Keyword">import</a> <a id="6088" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="6107" class="Keyword">open</a> <a id="6112" class="Keyword">import</a> <a id="6119" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="6138" class="Keyword">open</a> <a id="6143" class="Keyword">import</a> <a id="6150" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="6194" class="Keyword">open</a> <a id="6199" class="Keyword">import</a> <a id="6206" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="6231" class="Keyword">open</a> <a id="6236" class="Keyword">import</a> <a id="6243" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="6270" class="Keyword">open</a> <a id="6275" class="Keyword">import</a> <a id="6282" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="6311" class="Keyword">open</a> <a id="6316" class="Keyword">import</a> <a id="6323" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="6354" class="Keyword">open</a> <a id="6359" class="Keyword">import</a> <a id="6366" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="6394" class="Keyword">open</a> <a id="6399" class="Keyword">import</a> <a id="6406" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="6436" class="Keyword">open</a> <a id="6441" class="Keyword">import</a> <a id="6448" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="6468" class="Keyword">open</a> <a id="6473" class="Keyword">import</a> <a id="6480" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="6517" class="Keyword">open</a> <a id="6522" class="Keyword">import</a> <a id="6529" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="6564" class="Keyword">open</a> <a id="6569" class="Keyword">import</a> <a id="6576" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="6634" class="Keyword">open</a> <a id="6639" class="Keyword">import</a> <a id="6646" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="6684" class="Keyword">open</a> <a id="6689" class="Keyword">import</a> <a id="6696" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="6725" class="Keyword">open</a> <a id="6730" class="Keyword">import</a> <a id="6737" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="6760" class="Keyword">open</a> <a id="6765" class="Keyword">import</a> <a id="6772" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="6795" class="Keyword">open</a> <a id="6800" class="Keyword">import</a> <a id="6807" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="6849" class="Keyword">open</a> <a id="6854" class="Keyword">import</a> <a id="6861" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="6893" class="Keyword">open</a> <a id="6898" class="Keyword">import</a> <a id="6905" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="6932" class="Keyword">open</a> <a id="6937" class="Keyword">import</a> <a id="6944" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="6969" class="Keyword">open</a> <a id="6974" class="Keyword">import</a> <a id="6981" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="7010" class="Keyword">open</a> <a id="7015" class="Keyword">import</a> <a id="7022" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="7052" class="Keyword">open</a> <a id="7057" class="Keyword">import</a> <a id="7064" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="7091" class="Keyword">open</a> <a id="7096" class="Keyword">import</a> <a id="7103" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="7122" class="Keyword">open</a> <a id="7127" class="Keyword">import</a> <a id="7134" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="7180" class="Keyword">open</a> <a id="7185" class="Keyword">import</a> <a id="7192" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="7234" class="Keyword">open</a> <a id="7239" class="Keyword">import</a> <a id="7246" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="7278" class="Keyword">open</a> <a id="7283" class="Keyword">import</a> <a id="7290" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="7320" class="Keyword">open</a> <a id="7325" class="Keyword">import</a> <a id="7332" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="7358" class="Keyword">open</a> <a id="7363" class="Keyword">import</a> <a id="7370" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="7404" class="Keyword">open</a> <a id="7409" class="Keyword">import</a> <a id="7416" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="7446" class="Keyword">open</a> <a id="7451" class="Keyword">import</a> <a id="7458" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="7485" class="Keyword">open</a> <a id="7490" class="Keyword">import</a> <a id="7497" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="7529" class="Keyword">open</a> <a id="7534" class="Keyword">import</a> <a id="7541" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="7575" class="Keyword">open</a> <a id="7580" class="Keyword">import</a> <a id="7587" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="7610" class="Keyword">open</a> <a id="7615" class="Keyword">import</a> <a id="7622" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="7692" class="Keyword">open</a> <a id="7697" class="Keyword">import</a> <a id="7704" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="7774" class="Keyword">open</a> <a id="7779" class="Keyword">import</a> <a id="7786" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="7813" class="Keyword">open</a> <a id="7818" class="Keyword">import</a> <a id="7825" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="7873" class="Keyword">open</a> <a id="7878" class="Keyword">import</a> <a id="7885" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="7925" class="Keyword">open</a> <a id="7930" class="Keyword">import</a> <a id="7937" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="7959" class="Keyword">open</a> <a id="7964" class="Keyword">import</a> <a id="7971" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="7994" class="Keyword">open</a> <a id="7999" class="Keyword">import</a> <a id="8006" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="8051" class="Keyword">open</a> <a id="8056" class="Keyword">import</a> <a id="8063" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="8107" class="Keyword">open</a> <a id="8112" class="Keyword">import</a> <a id="8119" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="8155" class="Keyword">open</a> <a id="8160" class="Keyword">import</a> <a id="8167" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="8212" class="Keyword">open</a> <a id="8217" class="Keyword">import</a> <a id="8224" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="8265" class="Keyword">open</a> <a id="8270" class="Keyword">import</a> <a id="8277" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="8312" class="Keyword">open</a> <a id="8317" class="Keyword">import</a> <a id="8324" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="8355" class="Keyword">open</a> <a id="8360" class="Keyword">import</a> <a id="8367" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="8400" class="Keyword">open</a> <a id="8405" class="Keyword">import</a> <a id="8412" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="8445" class="Keyword">open</a> <a id="8450" class="Keyword">import</a> <a id="8457" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="8487" class="Keyword">open</a> <a id="8492" class="Keyword">import</a> <a id="8499" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="8523" class="Keyword">open</a> <a id="8528" class="Keyword">import</a> <a id="8535" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="8573" class="Keyword">open</a> <a id="8578" class="Keyword">import</a> <a id="8585" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="8616" class="Keyword">open</a> <a id="8621" class="Keyword">import</a> <a id="8628" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="8653" class="Keyword">open</a> <a id="8658" class="Keyword">import</a> <a id="8665" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="8693" class="Keyword">open</a> <a id="8698" class="Keyword">import</a> <a id="8705" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="8729" class="Keyword">open</a> <a id="8734" class="Keyword">import</a> <a id="8741" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="8767" class="Keyword">open</a> <a id="8772" class="Keyword">import</a> <a id="8779" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="8814" class="Keyword">open</a> <a id="8819" class="Keyword">import</a> <a id="8826" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="8847" class="Keyword">open</a> <a id="8852" class="Keyword">import</a> <a id="8859" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="8908" class="Keyword">open</a> <a id="8913" class="Keyword">import</a> <a id="8920" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="8961" class="Keyword">open</a> <a id="8966" class="Keyword">import</a> <a id="8973" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="9023" class="Keyword">open</a> <a id="9028" class="Keyword">import</a> <a id="9035" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="9081" class="Keyword">open</a> <a id="9086" class="Keyword">import</a> <a id="9093" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="9133" class="Keyword">open</a> <a id="9138" class="Keyword">import</a> <a id="9145" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="9195" class="Keyword">open</a> <a id="9200" class="Keyword">import</a> <a id="9207" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="9246" class="Keyword">open</a> <a id="9251" class="Keyword">import</a> <a id="9258" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="9298" class="Keyword">open</a> <a id="9303" class="Keyword">import</a> <a id="9310" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="9343" class="Keyword">open</a> <a id="9348" class="Keyword">import</a> <a id="9355" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="9404" class="Keyword">open</a> <a id="9409" class="Keyword">import</a> <a id="9416" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="9441" class="Keyword">open</a> <a id="9446" class="Keyword">import</a> <a id="9453" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="9475" class="Keyword">open</a> <a id="9480" class="Keyword">import</a> <a id="9487" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="9515" class="Keyword">open</a> <a id="9520" class="Keyword">import</a> <a id="9527" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="9553" class="Keyword">open</a> <a id="9558" class="Keyword">import</a> <a id="9565" href="foundation.images.html" class="Module">foundation.images</a>
<a id="9583" class="Keyword">open</a> <a id="9588" class="Keyword">import</a> <a id="9595" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="9630" class="Keyword">open</a> <a id="9635" class="Keyword">import</a> <a id="9642" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="9669" class="Keyword">open</a> <a id="9674" class="Keyword">import</a> <a id="9681" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="9737" class="Keyword">open</a> <a id="9742" class="Keyword">import</a> <a id="9749" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="9778" class="Keyword">open</a> <a id="9783" class="Keyword">import</a> <a id="9790" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="9820" class="Keyword">open</a> <a id="9825" class="Keyword">import</a> <a id="9832" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="9858" class="Keyword">open</a> <a id="9863" class="Keyword">import</a> <a id="9870" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="9897" class="Keyword">open</a> <a id="9902" class="Keyword">import</a> <a id="9909" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="9932" class="Keyword">open</a> <a id="9937" class="Keyword">import</a> <a id="9944" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="9971" class="Keyword">open</a> <a id="9976" class="Keyword">import</a> <a id="9983" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="10015" class="Keyword">open</a> <a id="10020" class="Keyword">import</a> <a id="10027" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="10061" class="Keyword">open</a> <a id="10066" class="Keyword">import</a> <a id="10073" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="10113" class="Keyword">open</a> <a id="10118" class="Keyword">import</a> <a id="10125" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="10156" class="Keyword">open</a> <a id="10161" class="Keyword">import</a> <a id="10168" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="10200" class="Keyword">open</a> <a id="10205" class="Keyword">import</a> <a id="10212" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="10229" class="Keyword">open</a> <a id="10234" class="Keyword">import</a> <a id="10241" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="10266" class="Keyword">open</a> <a id="10271" class="Keyword">import</a> <a id="10278" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="10307" class="Keyword">open</a> <a id="10312" class="Keyword">import</a> <a id="10319" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="10344" class="Keyword">open</a> <a id="10349" class="Keyword">import</a> <a id="10356" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="10377" class="Keyword">open</a> <a id="10382" class="Keyword">import</a> <a id="10389" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="10409" class="Keyword">open</a> <a id="10414" class="Keyword">import</a> <a id="10421" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="10455" class="Keyword">open</a> <a id="10460" class="Keyword">import</a> <a id="10467" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="10491" class="Keyword">open</a> <a id="10496" class="Keyword">import</a> <a id="10503" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="10530" class="Keyword">open</a> <a id="10535" class="Keyword">import</a> <a id="10542" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="10577" class="Keyword">open</a> <a id="10582" class="Keyword">import</a> <a id="10589" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="10629" class="Keyword">open</a> <a id="10634" class="Keyword">import</a> <a id="10641" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="10671" class="Keyword">open</a> <a id="10676" class="Keyword">import</a> <a id="10683" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="10720" class="Keyword">open</a> <a id="10725" class="Keyword">import</a> <a id="10732" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="10756" class="Keyword">open</a> <a id="10761" class="Keyword">import</a> <a id="10768" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="10789" class="Keyword">open</a> <a id="10794" class="Keyword">import</a> <a id="10801" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="10836" class="Keyword">open</a> <a id="10841" class="Keyword">import</a> <a id="10848" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="10885" class="Keyword">open</a> <a id="10890" class="Keyword">import</a> <a id="10897" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="10946" class="Keyword">open</a> <a id="10951" class="Keyword">import</a> <a id="10958" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="10981" class="Keyword">open</a> <a id="10986" class="Keyword">import</a> <a id="10993" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="11016" class="Keyword">open</a> <a id="11021" class="Keyword">import</a> <a id="11028" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="11056" class="Keyword">open</a> <a id="11061" class="Keyword">import</a> <a id="11068" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="11088" class="Keyword">open</a> <a id="11093" class="Keyword">import</a> <a id="11100" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="11131" class="Keyword">open</a> <a id="11136" class="Keyword">import</a> <a id="11143" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="11170" class="Keyword">open</a> <a id="11175" class="Keyword">import</a> <a id="11182" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="11198" class="Keyword">open</a> <a id="11203" class="Keyword">import</a> <a id="11210" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="11241" class="Keyword">open</a> <a id="11246" class="Keyword">import</a> <a id="11253" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="11270" class="Keyword">open</a> <a id="11275" class="Keyword">import</a> <a id="11282" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="11304" class="Keyword">open</a> <a id="11309" class="Keyword">import</a> <a id="11316" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="11343" class="Keyword">open</a> <a id="11348" class="Keyword">import</a> <a id="11355" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="11378" class="Keyword">open</a> <a id="11383" class="Keyword">import</a> <a id="11390" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="11417" class="Keyword">open</a> <a id="11422" class="Keyword">import</a> <a id="11429" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="11462" class="Keyword">open</a> <a id="11467" class="Keyword">import</a> <a id="11474" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="11514" class="Keyword">open</a> <a id="11519" class="Keyword">import</a> <a id="11526" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="11547" class="Keyword">open</a> <a id="11552" class="Keyword">import</a> <a id="11559" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="11588" class="Keyword">open</a> <a id="11593" class="Keyword">import</a> <a id="11600" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="11638" class="Keyword">open</a> <a id="11643" class="Keyword">import</a> <a id="11650" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="11670" class="Keyword">open</a> <a id="11675" class="Keyword">import</a> <a id="11682" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="11706" class="Keyword">open</a> <a id="11711" class="Keyword">import</a> <a id="11718" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="11745" class="Keyword">open</a> <a id="11750" class="Keyword">import</a> <a id="11757" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="11783" class="Keyword">open</a> <a id="11788" class="Keyword">import</a> <a id="11795" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="11822" class="Keyword">open</a> <a id="11827" class="Keyword">import</a> <a id="11834" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="11863" class="Keyword">open</a> <a id="11868" class="Keyword">import</a> <a id="11875" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="11898" class="Keyword">open</a> <a id="11903" class="Keyword">import</a> <a id="11910" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="11961" class="Keyword">open</a> <a id="11966" class="Keyword">import</a> <a id="11973" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="12016" class="Keyword">open</a> <a id="12021" class="Keyword">import</a> <a id="12028" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="12076" class="Keyword">open</a> <a id="12081" class="Keyword">import</a> <a id="12088" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="12126" class="Keyword">open</a> <a id="12131" class="Keyword">import</a> <a id="12138" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="12175" class="Keyword">open</a> <a id="12180" class="Keyword">import</a> <a id="12187" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="12215" class="Keyword">open</a> <a id="12220" class="Keyword">import</a> <a id="12227" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="12263" class="Keyword">open</a> <a id="12268" class="Keyword">import</a> <a id="12275" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="12313" class="Keyword">open</a> <a id="12318" class="Keyword">import</a> <a id="12325" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="12358" class="Keyword">open</a> <a id="12363" class="Keyword">import</a> <a id="12370" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="12391" class="Keyword">open</a> <a id="12396" class="Keyword">import</a> <a id="12403" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="12457" class="Keyword">open</a> <a id="12462" class="Keyword">import</a> <a id="12469" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="12491" class="Keyword">open</a> <a id="12496" class="Keyword">import</a> <a id="12503" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="12538" class="Keyword">open</a> <a id="12543" class="Keyword">import</a> <a id="12550" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="12580" class="Keyword">open</a> <a id="12585" class="Keyword">import</a> <a id="12592" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="12631" class="Keyword">open</a> <a id="12636" class="Keyword">import</a> <a id="12643" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="12697" class="Keyword">open</a> <a id="12702" class="Keyword">import</a> <a id="12709" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="12755" class="Keyword">open</a> <a id="12760" class="Keyword">import</a> <a id="12767" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="12818" class="Keyword">open</a> <a id="12823" class="Keyword">import</a> <a id="12830" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="12871" class="Keyword">open</a> <a id="12876" class="Keyword">import</a> <a id="12883" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="12928" class="Keyword">open</a> <a id="12933" class="Keyword">import</a> <a id="12940" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="12985" class="Keyword">open</a> <a id="12990" class="Keyword">import</a> <a id="12997" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="13033" class="Keyword">open</a> <a id="13038" class="Keyword">import</a> <a id="13045" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="13081" class="Keyword">open</a> <a id="13086" class="Keyword">import</a> <a id="13093" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="13158" class="Keyword">open</a> <a id="13163" class="Keyword">import</a> <a id="13170" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="13225" class="Keyword">open</a> <a id="13230" class="Keyword">import</a> <a id="13237" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="13277" class="Keyword">open</a> <a id="13282" class="Keyword">import</a> <a id="13289" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="13333" class="Keyword">open</a> <a id="13338" class="Keyword">import</a> <a id="13345" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="13390" class="Keyword">open</a> <a id="13395" class="Keyword">import</a> <a id="13402" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="13443" class="Keyword">open</a> <a id="13448" class="Keyword">import</a> <a id="13455" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="13495" class="Keyword">open</a> <a id="13500" class="Keyword">import</a> <a id="13507" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="13534" class="Keyword">open</a> <a id="13539" class="Keyword">import</a> <a id="13546" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="13573" class="Keyword">open</a> <a id="13578" class="Keyword">import</a> <a id="13585" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="13604" class="Keyword">open</a> <a id="13609" class="Keyword">import</a> <a id="13616" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="13656" class="Keyword">open</a> <a id="13661" class="Keyword">import</a> <a id="13668" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="13733" class="Keyword">open</a> <a id="13738" class="Keyword">import</a> <a id="13745" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="13768" class="Keyword">open</a> <a id="13773" class="Keyword">import</a> <a id="13780" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="13804" class="Keyword">open</a> <a id="13809" class="Keyword">import</a> <a id="13816" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="13856" class="Keyword">open</a> <a id="13861" class="Keyword">import</a> <a id="13868" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="13911" class="Keyword">open</a> <a id="13916" class="Keyword">import</a> <a id="13923" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="13957" class="Keyword">open</a> <a id="13962" class="Keyword">import</a> <a id="13969" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="13999" class="Keyword">open</a> <a id="14004" class="Keyword">import</a> <a id="14011" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="14045" class="Keyword">open</a> <a id="14050" class="Keyword">import</a> <a id="14057" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="14092" class="Keyword">open</a> <a id="14097" class="Keyword">import</a> <a id="14104" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="14141" class="Keyword">open</a> <a id="14146" class="Keyword">import</a> <a id="14153" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="14180" class="Keyword">open</a> <a id="14185" class="Keyword">import</a> <a id="14192" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="14220" class="Keyword">open</a> <a id="14225" class="Keyword">import</a> <a id="14232" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="14281" class="Keyword">open</a> <a id="14286" class="Keyword">import</a> <a id="14293" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="14339" class="Keyword">open</a> <a id="14344" class="Keyword">import</a> <a id="14351" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="14391" class="Keyword">open</a> <a id="14396" class="Keyword">import</a> <a id="14403" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="14441" class="Keyword">open</a> <a id="14446" class="Keyword">import</a> <a id="14453" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="14482" class="Keyword">open</a> <a id="14487" class="Keyword">import</a> <a id="14494" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="14524" class="Keyword">open</a> <a id="14529" class="Keyword">import</a> <a id="14536" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="14567" class="Keyword">open</a> <a id="14572" class="Keyword">import</a> <a id="14579" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="14605" class="Keyword">open</a> <a id="14610" class="Keyword">import</a> <a id="14617" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="14668" class="Keyword">open</a> <a id="14673" class="Keyword">import</a> <a id="14680" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="14734" class="Keyword">open</a> <a id="14739" class="Keyword">import</a> <a id="14746" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="14773" class="Keyword">open</a> <a id="14778" class="Keyword">import</a> <a id="14785" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="14818" class="Keyword">open</a> <a id="14823" class="Keyword">import</a> <a id="14830" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="14861" class="Keyword">open</a> <a id="14866" class="Keyword">import</a> <a id="14873" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="14910" class="Keyword">open</a> <a id="14915" class="Keyword">import</a> <a id="14922" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="14947" class="Keyword">open</a> <a id="14952" class="Keyword">import</a> <a id="14959" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="14991" class="Keyword">open</a> <a id="14996" class="Keyword">import</a> <a id="15003" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="15038" class="Keyword">open</a> <a id="15043" class="Keyword">import</a> <a id="15050" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="15079" class="Keyword">open</a> <a id="15084" class="Keyword">import</a> <a id="15091" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="15119" class="Keyword">open</a> <a id="15124" class="Keyword">import</a> <a id="15131" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="15156" class="Keyword">open</a> <a id="15161" class="Keyword">import</a> <a id="15168" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="15189" class="Keyword">open</a> <a id="15194" class="Keyword">import</a> <a id="15201" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="15237" class="Keyword">open</a> <a id="15242" class="Keyword">import</a> <a id="15249" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="15292" class="Keyword">open</a> <a id="15297" class="Keyword">import</a> <a id="15304" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="15329" class="Keyword">open</a> <a id="15334" class="Keyword">import</a> <a id="15341" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="15372" class="Keyword">open</a> <a id="15377" class="Keyword">import</a> <a id="15384" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="15416" class="Keyword">open</a> <a id="15421" class="Keyword">import</a> <a id="15428" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="15462" class="Keyword">open</a> <a id="15467" class="Keyword">import</a> <a id="15474" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="15530" class="Keyword">open</a> <a id="15535" class="Keyword">import</a> <a id="15542" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="15595" class="Keyword">open</a> <a id="15600" class="Keyword">import</a> <a id="15607" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="15634" class="Keyword">open</a> <a id="15639" class="Keyword">import</a> <a id="15646" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="15708" class="Keyword">open</a> <a id="15713" class="Keyword">import</a> <a id="15720" href="graph-theory.html" class="Module">graph-theory</a>
<a id="15733" class="Keyword">open</a> <a id="15738" class="Keyword">import</a> <a id="15745" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="15774" class="Keyword">open</a> <a id="15779" class="Keyword">import</a> <a id="15786" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="15813" class="Keyword">open</a> <a id="15818" class="Keyword">import</a> <a id="15825" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="15847" class="Keyword">open</a> <a id="15852" class="Keyword">import</a> <a id="15859" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="15889" class="Keyword">open</a> <a id="15894" class="Keyword">import</a> <a id="15901" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="15962" class="Keyword">open</a> <a id="15967" class="Keyword">import</a> <a id="15974" href="group-theory.html" class="Module">group-theory</a>
<a id="15987" class="Keyword">open</a> <a id="15992" class="Keyword">import</a> <a id="15999" href="group-theory.abstract-abelian-groups.html" class="Module">group-theory.abstract-abelian-groups</a>
<a id="16036" class="Keyword">open</a> <a id="16041" class="Keyword">import</a> <a id="16048" href="group-theory.abstract-abelian-subgroups.html" class="Module">group-theory.abstract-abelian-subgroups</a>
<a id="16088" class="Keyword">open</a> <a id="16093" class="Keyword">import</a> <a id="16100" href="group-theory.abstract-group-actions.html" class="Module">group-theory.abstract-group-actions</a>
<a id="16136" class="Keyword">open</a> <a id="16141" class="Keyword">import</a> <a id="16148" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="16184" class="Keyword">open</a> <a id="16189" class="Keyword">import</a> <a id="16196" href="group-theory.abstract-groups.html" class="Module">group-theory.abstract-groups</a>
<a id="16225" class="Keyword">open</a> <a id="16230" class="Keyword">import</a> <a id="16237" href="group-theory.abstract-subgroups.html" class="Module">group-theory.abstract-subgroups</a>
<a id="16269" class="Keyword">open</a> <a id="16274" class="Keyword">import</a> <a id="16281" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="16317" class="Keyword">open</a> <a id="16322" class="Keyword">import</a> <a id="16329" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="16358" class="Keyword">open</a> <a id="16363" class="Keyword">import</a> <a id="16370" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="16402" class="Keyword">open</a> <a id="16407" class="Keyword">import</a> <a id="16414" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="16450" class="Keyword">open</a> <a id="16455" class="Keyword">import</a> <a id="16462" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="16494" class="Keyword">open</a> <a id="16499" class="Keyword">import</a> <a id="16506" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="16533" class="Keyword">open</a> <a id="16538" class="Keyword">import</a> <a id="16545" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="16602" class="Keyword">open</a> <a id="16607" class="Keyword">import</a> <a id="16614" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="16629" class="Keyword">open</a> <a id="16634" class="Keyword">import</a> <a id="16641" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="16665" class="Keyword">open</a> <a id="16670" class="Keyword">import</a> <a id="16677" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="16730" class="Keyword">open</a> <a id="16735" class="Keyword">import</a> <a id="16742" href="order-theory.html" class="Module">order-theory</a>
<a id="16755" class="Keyword">open</a> <a id="16760" class="Keyword">import</a> <a id="16767" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="16794" class="Keyword">open</a> <a id="16799" class="Keyword">import</a> <a id="16806" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="16836" class="Keyword">open</a> <a id="16841" class="Keyword">import</a> <a id="16848" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="16884" class="Keyword">open</a> <a id="16889" class="Keyword">import</a> <a id="16896" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="16929" class="Keyword">open</a> <a id="16934" class="Keyword">import</a> <a id="16941" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="16961" class="Keyword">open</a> <a id="16966" class="Keyword">import</a> <a id="16973" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="17023" class="Keyword">open</a> <a id="17028" class="Keyword">import</a> <a id="17035" href="polytopes.html" class="Module">polytopes</a>
<a id="17045" class="Keyword">open</a> <a id="17050" class="Keyword">import</a> <a id="17057" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="17115" class="Keyword">open</a> <a id="17120" class="Keyword">import</a> <a id="17127" href="ring-theory.html" class="Module">ring-theory</a>
<a id="17139" class="Keyword">open</a> <a id="17144" class="Keyword">import</a> <a id="17151" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="17183" class="Keyword">open</a> <a id="17188" class="Keyword">import</a> <a id="17195" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="17225" class="Keyword">open</a> <a id="17230" class="Keyword">import</a> <a id="17237" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a>
<a id="17256" class="Keyword">open</a> <a id="17261" class="Keyword">import</a> <a id="17268" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="17300" class="Keyword">open</a> <a id="17305" class="Keyword">import</a> <a id="17312" href="ring-theory.rings-with-properties.html" class="Module">ring-theory.rings-with-properties</a>
<a id="17346" class="Keyword">open</a> <a id="17351" class="Keyword">import</a> <a id="17358" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="17419" class="Keyword">open</a> <a id="17424" class="Keyword">import</a> <a id="17431" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="17457" class="Keyword">open</a> <a id="17462" class="Keyword">import</a> <a id="17469" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="17508" class="Keyword">open</a> <a id="17513" class="Keyword">import</a> <a id="17520" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="17558" class="Keyword">open</a> <a id="17563" class="Keyword">import</a> <a id="17570" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="17616" class="Keyword">open</a> <a id="17621" class="Keyword">import</a> <a id="17628" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="17665" class="Keyword">open</a> <a id="17670" class="Keyword">import</a> <a id="17677" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="17717" class="Keyword">open</a> <a id="17722" class="Keyword">import</a> <a id="17729" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="17768" class="Keyword">open</a> <a id="17773" class="Keyword">import</a> <a id="17780" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="17813" class="Keyword">open</a> <a id="17818" class="Keyword">import</a> <a id="17825" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="17864" class="Keyword">open</a> <a id="17869" class="Keyword">import</a> <a id="17876" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="17921" class="Keyword">open</a> <a id="17926" class="Keyword">import</a> <a id="17933" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="17985" class="Keyword">open</a> <a id="17990" class="Keyword">import</a> <a id="17997" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="18045" class="Keyword">open</a> <a id="18050" class="Keyword">import</a> <a id="18057" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="18097" class="Keyword">open</a> <a id="18102" class="Keyword">import</a> <a id="18109" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="18156" class="Keyword">open</a> <a id="18161" class="Keyword">import</a> <a id="18168" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="18206" class="Keyword">open</a> <a id="18211" class="Keyword">import</a> <a id="18218" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="18272" class="Keyword">open</a> <a id="18277" class="Keyword">import</a> <a id="18284" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="18331" class="Keyword">open</a> <a id="18336" class="Keyword">import</a> <a id="18343" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="18395" class="Keyword">open</a> <a id="18400" class="Keyword">import</a> <a id="18407" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="18452" class="Keyword">open</a> <a id="18457" class="Keyword">import</a> <a id="18464" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="18503" class="Keyword">open</a> <a id="18508" class="Keyword">import</a> <a id="18515" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="18555" class="Keyword">open</a> <a id="18560" class="Keyword">import</a> <a id="18567" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="18600" class="Keyword">open</a> <a id="18605" class="Keyword">import</a> <a id="18612" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="18657" class="Keyword">open</a> <a id="18662" class="Keyword">import</a> <a id="18669" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="18745" class="Keyword">open</a> <a id="18750" class="Keyword">import</a> <a id="18757" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="18819" class="Keyword">open</a> <a id="18824" class="Keyword">import</a> <a id="18831" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="18855" class="Keyword">open</a> <a id="18860" class="Keyword">import</a> <a id="18867" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="18907" class="Keyword">open</a> <a id="18912" class="Keyword">import</a> <a id="18919" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="18958" class="Keyword">open</a> <a id="18963" class="Keyword">import</a> <a id="18970" href="univalent-combinatorics.cartesian-product-finite-types.html" class="Module">univalent-combinatorics.cartesian-product-finite-types</a>
<a id="19025" class="Keyword">open</a> <a id="19030" class="Keyword">import</a> <a id="19037" href="univalent-combinatorics.coproduct-finite-types.html" class="Module">univalent-combinatorics.coproduct-finite-types</a>
<a id="19084" class="Keyword">open</a> <a id="19089" class="Keyword">import</a> <a id="19096" href="univalent-combinatorics.counting-cartesian-product-types.html" class="Module">univalent-combinatorics.counting-cartesian-product-types</a>
<a id="19153" class="Keyword">open</a> <a id="19158" class="Keyword">import</a> <a id="19165" href="univalent-combinatorics.counting-coproduct-types.html" class="Module">univalent-combinatorics.counting-coproduct-types</a>
<a id="19214" class="Keyword">open</a> <a id="19219" class="Keyword">import</a> <a id="19226" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="19278" class="Keyword">open</a> <a id="19283" class="Keyword">import</a> <a id="19290" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="19348" class="Keyword">open</a> <a id="19353" class="Keyword">import</a> <a id="19360" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="19414" class="Keyword">open</a> <a id="19419" class="Keyword">import</a> <a id="19426" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="19474" class="Keyword">open</a> <a id="19479" class="Keyword">import</a> <a id="19486" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="19534" class="Keyword">open</a> <a id="19539" class="Keyword">import</a> <a id="19546" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="19585" class="Keyword">open</a> <a id="19590" class="Keyword">import</a> <a id="19597" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="19630" class="Keyword">open</a> <a id="19635" class="Keyword">import</a> <a id="19642" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="19701" class="Keyword">open</a> <a id="19706" class="Keyword">import</a> <a id="19713" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="19768" class="Keyword">open</a> <a id="19773" class="Keyword">import</a> <a id="19780" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="19823" class="Keyword">open</a> <a id="19828" class="Keyword">import</a> <a id="19835" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="19890" class="Keyword">open</a> <a id="19895" class="Keyword">import</a> <a id="19902" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="19953" class="Keyword">open</a> <a id="19958" class="Keyword">import</a> <a id="19965" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="20043" class="Keyword">open</a> <a id="20048" class="Keyword">import</a> <a id="20055" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="20095" class="Keyword">open</a> <a id="20100" class="Keyword">import</a> <a id="20107" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="20164" class="Keyword">open</a> <a id="20169" class="Keyword">import</a> <a id="20176" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="20211" class="Keyword">open</a> <a id="20216" class="Keyword">import</a> <a id="20223" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="20269" class="Keyword">open</a> <a id="20274" class="Keyword">import</a> <a id="20281" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="20336" class="Keyword">open</a> <a id="20341" class="Keyword">import</a> <a id="20348" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="20407" class="Keyword">open</a> <a id="20412" class="Keyword">import</a> <a id="20419" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="20456" class="Keyword">open</a> <a id="20461" class="Keyword">import</a> <a id="20468" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="20528" class="Keyword">open</a> <a id="20533" class="Keyword">import</a> <a id="20540" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="20578" class="Keyword">open</a> <a id="20583" class="Keyword">import</a> <a id="20590" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="20642" class="Keyword">open</a> <a id="20647" class="Keyword">import</a> <a id="20654" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="20700" class="Keyword">open</a> <a id="20705" class="Keyword">import</a> <a id="20712" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="20757" class="Keyword">open</a> <a id="20762" class="Keyword">import</a> <a id="20769" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="20806" class="Keyword">open</a> <a id="20811" class="Keyword">import</a> <a id="20818" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="20867" class="Keyword">open</a> <a id="20872" class="Keyword">import</a> <a id="20879" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="20917" class="Keyword">open</a> <a id="20922" class="Keyword">import</a> <a id="20929" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="20984" class="Keyword">open</a> <a id="20989" class="Keyword">import</a> <a id="20996" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="21035" class="Keyword">open</a> <a id="21040" class="Keyword">import</a> <a id="21047" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="21077" class="Keyword">open</a> <a id="21082" class="Keyword">import</a> <a id="21089" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="21119" class="Keyword">open</a> <a id="21124" class="Keyword">import</a> <a id="21131" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="21171" class="Keyword">open</a> <a id="21176" class="Keyword">import</a> <a id="21183" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="21228" class="Keyword">open</a> <a id="21233" class="Keyword">import</a> <a id="21240" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="21290" class="Keyword">open</a> <a id="21295" class="Keyword">import</a> <a id="21302" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="21340" class="Keyword">open</a> <a id="21345" class="Keyword">import</a> <a id="21352" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="21401" class="Keyword">open</a> <a id="21406" class="Keyword">import</a> <a id="21413" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="21466" class="Keyword">open</a> <a id="21471" class="Keyword">import</a> <a id="21478" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="21524" class="Keyword">open</a> <a id="21529" class="Keyword">import</a> <a id="21536" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="21582" class="Keyword">open</a> <a id="21587" class="Keyword">import</a> <a id="21594" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="21642" class="Keyword">open</a> <a id="21647" class="Keyword">import</a> <a id="21654" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="21732" class="Keyword">open</a> <a id="21737" class="Keyword">import</a> <a id="21744" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="21812" class="Keyword">open</a> <a id="21817" class="Keyword">import</a> <a id="21824" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="21837" class="Keyword">open</a> <a id="21842" class="Keyword">import</a> <a id="21849" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="21869" class="Keyword">open</a> <a id="21874" class="Keyword">import</a> <a id="21881" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="21932" class="Keyword">open</a> <a id="21937" class="Keyword">import</a> <a id="21944" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="21969" class="Keyword">open</a> <a id="21974" class="Keyword">import</a> <a id="21981" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="22007" class="Keyword">open</a> <a id="22012" class="Keyword">import</a> <a id="22019" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

