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
<a id="1746" class="Keyword">open</a> <a id="1751" class="Keyword">import</a> <a id="1758" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="1847" class="Keyword">open</a> <a id="1852" class="Keyword">import</a> <a id="1859" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="1884" class="Keyword">open</a> <a id="1889" class="Keyword">import</a> <a id="1896" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="1945" class="Keyword">open</a> <a id="1950" class="Keyword">import</a> <a id="1957" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="2000" class="Keyword">open</a> <a id="2005" class="Keyword">import</a> <a id="2012" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="2062" class="Keyword">open</a> <a id="2067" class="Keyword">import</a> <a id="2074" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="2121" class="Keyword">open</a> <a id="2126" class="Keyword">import</a> <a id="2133" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="2174" class="Keyword">open</a> <a id="2179" class="Keyword">import</a> <a id="2186" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="2229" class="Keyword">open</a> <a id="2234" class="Keyword">import</a> <a id="2241" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="2285" class="Keyword">open</a> <a id="2290" class="Keyword">import</a> <a id="2297" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="2342" class="Keyword">open</a> <a id="2347" class="Keyword">import</a> <a id="2354" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="2406" class="Keyword">open</a> <a id="2411" class="Keyword">import</a> <a id="2418" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="2459" class="Keyword">open</a> <a id="2464" class="Keyword">import</a> <a id="2471" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="2516" class="Keyword">open</a> <a id="2521" class="Keyword">import</a> <a id="2528" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="2571" class="Keyword">open</a> <a id="2576" class="Keyword">import</a> <a id="2583" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="2633" class="Keyword">open</a> <a id="2638" class="Keyword">import</a> <a id="2645" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="2692" class="Keyword">open</a> <a id="2697" class="Keyword">import</a> <a id="2704" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="2761" class="Keyword">open</a> <a id="2766" class="Keyword">import</a> <a id="2773" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="2827" class="Keyword">open</a> <a id="2832" class="Keyword">import</a> <a id="2839" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="2899" class="Keyword">open</a> <a id="2904" class="Keyword">import</a> <a id="2911" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="2954" class="Keyword">open</a> <a id="2959" class="Keyword">import</a> <a id="2966" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="3016" class="Keyword">open</a> <a id="3021" class="Keyword">import</a> <a id="3028" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="3088" class="Keyword">open</a> <a id="3093" class="Keyword">import</a> <a id="3100" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="3149" class="Keyword">open</a> <a id="3154" class="Keyword">import</a> <a id="3161" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="3217" class="Keyword">open</a> <a id="3222" class="Keyword">import</a> <a id="3229" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="3265" class="Keyword">open</a> <a id="3270" class="Keyword">import</a> <a id="3277" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="3321" class="Keyword">open</a> <a id="3326" class="Keyword">import</a> <a id="3333" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="3377" class="Keyword">open</a> <a id="3382" class="Keyword">import</a> <a id="3389" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="3439" class="Keyword">open</a> <a id="3444" class="Keyword">import</a> <a id="3451" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="3497" class="Keyword">open</a> <a id="3502" class="Keyword">import</a> <a id="3509" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="3544" class="Keyword">open</a> <a id="3549" class="Keyword">import</a> <a id="3556" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="3601" class="Keyword">open</a> <a id="3606" class="Keyword">import</a> <a id="3613" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="3671" class="Keyword">open</a> <a id="3676" class="Keyword">import</a> <a id="3683" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="3748" class="Keyword">open</a> <a id="3753" class="Keyword">import</a> <a id="3760" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="3805" class="Keyword">open</a> <a id="3810" class="Keyword">import</a> <a id="3817" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="3869" class="Keyword">open</a> <a id="3874" class="Keyword">import</a> <a id="3881" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="3939" class="Keyword">open</a> <a id="3944" class="Keyword">import</a> <a id="3951" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="3997" class="Keyword">open</a> <a id="4002" class="Keyword">import</a> <a id="4009" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="4043" class="Keyword">open</a> <a id="4048" class="Keyword">import</a> <a id="4055" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="4100" class="Keyword">open</a> <a id="4105" class="Keyword">import</a> <a id="4112" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="4166" class="Keyword">open</a> <a id="4171" class="Keyword">import</a> <a id="4178" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="4219" class="Keyword">open</a> <a id="4224" class="Keyword">import</a> <a id="4231" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="4297" class="Keyword">open</a> <a id="4302" class="Keyword">import</a> <a id="4309" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="4353" class="Keyword">open</a> <a id="4358" class="Keyword">import</a> <a id="4365" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="4414" class="Keyword">open</a> <a id="4419" class="Keyword">import</a> <a id="4426" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="4482" class="Keyword">open</a> <a id="4487" class="Keyword">import</a> <a id="4494" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="4535" class="Keyword">open</a> <a id="4540" class="Keyword">import</a> <a id="4547" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="4606" class="Keyword">open</a> <a id="4611" class="Keyword">import</a> <a id="4618" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="4657" class="Keyword">open</a> <a id="4662" class="Keyword">import</a> <a id="4669" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="4722" class="Keyword">open</a> <a id="4727" class="Keyword">import</a> <a id="4734" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="4791" class="Keyword">open</a> <a id="4796" class="Keyword">import</a> <a id="4803" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="4845" class="Keyword">open</a> <a id="4850" class="Keyword">import</a> <a id="4857" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="4908" class="Keyword">open</a> <a id="4913" class="Keyword">import</a> <a id="4920" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="4978" class="Keyword">open</a> <a id="4983" class="Keyword">import</a> <a id="4990" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="5054" class="Keyword">open</a> <a id="5059" class="Keyword">import</a> <a id="5066" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="5119" class="Keyword">open</a> <a id="5124" class="Keyword">import</a> <a id="5131" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="5184" class="Keyword">open</a> <a id="5189" class="Keyword">import</a> <a id="5196" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="5257" class="Keyword">open</a> <a id="5262" class="Keyword">import</a> <a id="5269" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="5327" class="Keyword">open</a> <a id="5332" class="Keyword">import</a> <a id="5339" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="5388" class="Keyword">open</a> <a id="5393" class="Keyword">import</a> <a id="5400" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="5444" class="Keyword">open</a> <a id="5449" class="Keyword">import</a> <a id="5456" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="5503" class="Keyword">open</a> <a id="5508" class="Keyword">import</a> <a id="5515" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="5575" class="Keyword">open</a> <a id="5580" class="Keyword">import</a> <a id="5587" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="5641" class="Keyword">open</a> <a id="5646" class="Keyword">import</a> <a id="5653" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="5714" class="Keyword">open</a> <a id="5719" class="Keyword">import</a> <a id="5726" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="5789" class="Keyword">open</a> <a id="5794" class="Keyword">import</a> <a id="5801" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="5866" class="Keyword">open</a> <a id="5871" class="Keyword">import</a> <a id="5878" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="5986" class="Keyword">open</a> <a id="5991" class="Keyword">import</a> <a id="5998" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="6018" class="Keyword">open</a> <a id="6023" class="Keyword">import</a> <a id="6030" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="6076" class="Keyword">open</a> <a id="6081" class="Keyword">import</a> <a id="6088" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="6134" class="Keyword">open</a> <a id="6139" class="Keyword">import</a> <a id="6146" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="6180" class="Keyword">open</a> <a id="6185" class="Keyword">import</a> <a id="6192" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="6232" class="Keyword">open</a> <a id="6237" class="Keyword">import</a> <a id="6244" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="6307" class="Keyword">open</a> <a id="6312" class="Keyword">import</a> <a id="6319" href="foundation.html" class="Module">foundation</a>
<a id="6330" class="Keyword">open</a> <a id="6335" class="Keyword">import</a> <a id="6342" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="6360" class="Keyword">open</a> <a id="6365" class="Keyword">import</a> <a id="6372" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="6391" class="Keyword">open</a> <a id="6396" class="Keyword">import</a> <a id="6403" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="6422" class="Keyword">open</a> <a id="6427" class="Keyword">import</a> <a id="6434" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="6478" class="Keyword">open</a> <a id="6483" class="Keyword">import</a> <a id="6490" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="6515" class="Keyword">open</a> <a id="6520" class="Keyword">import</a> <a id="6527" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="6554" class="Keyword">open</a> <a id="6559" class="Keyword">import</a> <a id="6566" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="6595" class="Keyword">open</a> <a id="6600" class="Keyword">import</a> <a id="6607" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="6638" class="Keyword">open</a> <a id="6643" class="Keyword">import</a> <a id="6650" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="6678" class="Keyword">open</a> <a id="6683" class="Keyword">import</a> <a id="6690" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="6720" class="Keyword">open</a> <a id="6725" class="Keyword">import</a> <a id="6732" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="6752" class="Keyword">open</a> <a id="6757" class="Keyword">import</a> <a id="6764" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="6801" class="Keyword">open</a> <a id="6806" class="Keyword">import</a> <a id="6813" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="6848" class="Keyword">open</a> <a id="6853" class="Keyword">import</a> <a id="6860" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="6918" class="Keyword">open</a> <a id="6923" class="Keyword">import</a> <a id="6930" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="6968" class="Keyword">open</a> <a id="6973" class="Keyword">import</a> <a id="6980" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="7009" class="Keyword">open</a> <a id="7014" class="Keyword">import</a> <a id="7021" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="7044" class="Keyword">open</a> <a id="7049" class="Keyword">import</a> <a id="7056" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="7079" class="Keyword">open</a> <a id="7084" class="Keyword">import</a> <a id="7091" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="7133" class="Keyword">open</a> <a id="7138" class="Keyword">import</a> <a id="7145" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="7177" class="Keyword">open</a> <a id="7182" class="Keyword">import</a> <a id="7189" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="7216" class="Keyword">open</a> <a id="7221" class="Keyword">import</a> <a id="7228" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="7253" class="Keyword">open</a> <a id="7258" class="Keyword">import</a> <a id="7265" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="7294" class="Keyword">open</a> <a id="7299" class="Keyword">import</a> <a id="7306" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="7336" class="Keyword">open</a> <a id="7341" class="Keyword">import</a> <a id="7348" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="7375" class="Keyword">open</a> <a id="7380" class="Keyword">import</a> <a id="7387" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="7406" class="Keyword">open</a> <a id="7411" class="Keyword">import</a> <a id="7418" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="7464" class="Keyword">open</a> <a id="7469" class="Keyword">import</a> <a id="7476" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="7518" class="Keyword">open</a> <a id="7523" class="Keyword">import</a> <a id="7530" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="7562" class="Keyword">open</a> <a id="7567" class="Keyword">import</a> <a id="7574" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="7604" class="Keyword">open</a> <a id="7609" class="Keyword">import</a> <a id="7616" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="7642" class="Keyword">open</a> <a id="7647" class="Keyword">import</a> <a id="7654" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="7688" class="Keyword">open</a> <a id="7693" class="Keyword">import</a> <a id="7700" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="7730" class="Keyword">open</a> <a id="7735" class="Keyword">import</a> <a id="7742" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="7769" class="Keyword">open</a> <a id="7774" class="Keyword">import</a> <a id="7781" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="7813" class="Keyword">open</a> <a id="7818" class="Keyword">import</a> <a id="7825" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="7859" class="Keyword">open</a> <a id="7864" class="Keyword">import</a> <a id="7871" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="7894" class="Keyword">open</a> <a id="7899" class="Keyword">import</a> <a id="7906" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="7976" class="Keyword">open</a> <a id="7981" class="Keyword">import</a> <a id="7988" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="8058" class="Keyword">open</a> <a id="8063" class="Keyword">import</a> <a id="8070" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="8097" class="Keyword">open</a> <a id="8102" class="Keyword">import</a> <a id="8109" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="8157" class="Keyword">open</a> <a id="8162" class="Keyword">import</a> <a id="8169" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="8209" class="Keyword">open</a> <a id="8214" class="Keyword">import</a> <a id="8221" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="8243" class="Keyword">open</a> <a id="8248" class="Keyword">import</a> <a id="8255" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="8278" class="Keyword">open</a> <a id="8283" class="Keyword">import</a> <a id="8290" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="8335" class="Keyword">open</a> <a id="8340" class="Keyword">import</a> <a id="8347" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="8391" class="Keyword">open</a> <a id="8396" class="Keyword">import</a> <a id="8403" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="8439" class="Keyword">open</a> <a id="8444" class="Keyword">import</a> <a id="8451" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="8496" class="Keyword">open</a> <a id="8501" class="Keyword">import</a> <a id="8508" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="8549" class="Keyword">open</a> <a id="8554" class="Keyword">import</a> <a id="8561" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="8596" class="Keyword">open</a> <a id="8601" class="Keyword">import</a> <a id="8608" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="8639" class="Keyword">open</a> <a id="8644" class="Keyword">import</a> <a id="8651" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="8684" class="Keyword">open</a> <a id="8689" class="Keyword">import</a> <a id="8696" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="8729" class="Keyword">open</a> <a id="8734" class="Keyword">import</a> <a id="8741" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="8771" class="Keyword">open</a> <a id="8776" class="Keyword">import</a> <a id="8783" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="8807" class="Keyword">open</a> <a id="8812" class="Keyword">import</a> <a id="8819" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="8857" class="Keyword">open</a> <a id="8862" class="Keyword">import</a> <a id="8869" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="8900" class="Keyword">open</a> <a id="8905" class="Keyword">import</a> <a id="8912" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="8937" class="Keyword">open</a> <a id="8942" class="Keyword">import</a> <a id="8949" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="8977" class="Keyword">open</a> <a id="8982" class="Keyword">import</a> <a id="8989" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="9013" class="Keyword">open</a> <a id="9018" class="Keyword">import</a> <a id="9025" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="9051" class="Keyword">open</a> <a id="9056" class="Keyword">import</a> <a id="9063" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="9098" class="Keyword">open</a> <a id="9103" class="Keyword">import</a> <a id="9110" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="9131" class="Keyword">open</a> <a id="9136" class="Keyword">import</a> <a id="9143" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="9192" class="Keyword">open</a> <a id="9197" class="Keyword">import</a> <a id="9204" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="9245" class="Keyword">open</a> <a id="9250" class="Keyword">import</a> <a id="9257" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="9307" class="Keyword">open</a> <a id="9312" class="Keyword">import</a> <a id="9319" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="9365" class="Keyword">open</a> <a id="9370" class="Keyword">import</a> <a id="9377" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="9417" class="Keyword">open</a> <a id="9422" class="Keyword">import</a> <a id="9429" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="9479" class="Keyword">open</a> <a id="9484" class="Keyword">import</a> <a id="9491" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="9530" class="Keyword">open</a> <a id="9535" class="Keyword">import</a> <a id="9542" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="9582" class="Keyword">open</a> <a id="9587" class="Keyword">import</a> <a id="9594" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="9627" class="Keyword">open</a> <a id="9632" class="Keyword">import</a> <a id="9639" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="9688" class="Keyword">open</a> <a id="9693" class="Keyword">import</a> <a id="9700" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="9725" class="Keyword">open</a> <a id="9730" class="Keyword">import</a> <a id="9737" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="9759" class="Keyword">open</a> <a id="9764" class="Keyword">import</a> <a id="9771" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="9799" class="Keyword">open</a> <a id="9804" class="Keyword">import</a> <a id="9811" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="9837" class="Keyword">open</a> <a id="9842" class="Keyword">import</a> <a id="9849" href="foundation.images.html" class="Module">foundation.images</a>
<a id="9867" class="Keyword">open</a> <a id="9872" class="Keyword">import</a> <a id="9879" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="9914" class="Keyword">open</a> <a id="9919" class="Keyword">import</a> <a id="9926" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="9953" class="Keyword">open</a> <a id="9958" class="Keyword">import</a> <a id="9965" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="10021" class="Keyword">open</a> <a id="10026" class="Keyword">import</a> <a id="10033" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="10062" class="Keyword">open</a> <a id="10067" class="Keyword">import</a> <a id="10074" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="10104" class="Keyword">open</a> <a id="10109" class="Keyword">import</a> <a id="10116" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="10142" class="Keyword">open</a> <a id="10147" class="Keyword">import</a> <a id="10154" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="10181" class="Keyword">open</a> <a id="10186" class="Keyword">import</a> <a id="10193" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="10216" class="Keyword">open</a> <a id="10221" class="Keyword">import</a> <a id="10228" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="10255" class="Keyword">open</a> <a id="10260" class="Keyword">import</a> <a id="10267" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="10299" class="Keyword">open</a> <a id="10304" class="Keyword">import</a> <a id="10311" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="10345" class="Keyword">open</a> <a id="10350" class="Keyword">import</a> <a id="10357" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="10397" class="Keyword">open</a> <a id="10402" class="Keyword">import</a> <a id="10409" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="10440" class="Keyword">open</a> <a id="10445" class="Keyword">import</a> <a id="10452" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="10484" class="Keyword">open</a> <a id="10489" class="Keyword">import</a> <a id="10496" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="10527" class="Keyword">open</a> <a id="10532" class="Keyword">import</a> <a id="10539" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="10556" class="Keyword">open</a> <a id="10561" class="Keyword">import</a> <a id="10568" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="10593" class="Keyword">open</a> <a id="10598" class="Keyword">import</a> <a id="10605" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="10634" class="Keyword">open</a> <a id="10639" class="Keyword">import</a> <a id="10646" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="10671" class="Keyword">open</a> <a id="10676" class="Keyword">import</a> <a id="10683" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="10704" class="Keyword">open</a> <a id="10709" class="Keyword">import</a> <a id="10716" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="10736" class="Keyword">open</a> <a id="10741" class="Keyword">import</a> <a id="10748" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="10782" class="Keyword">open</a> <a id="10787" class="Keyword">import</a> <a id="10794" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="10818" class="Keyword">open</a> <a id="10823" class="Keyword">import</a> <a id="10830" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="10857" class="Keyword">open</a> <a id="10862" class="Keyword">import</a> <a id="10869" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="10904" class="Keyword">open</a> <a id="10909" class="Keyword">import</a> <a id="10916" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="10956" class="Keyword">open</a> <a id="10961" class="Keyword">import</a> <a id="10968" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="10998" class="Keyword">open</a> <a id="11003" class="Keyword">import</a> <a id="11010" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="11047" class="Keyword">open</a> <a id="11052" class="Keyword">import</a> <a id="11059" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="11083" class="Keyword">open</a> <a id="11088" class="Keyword">import</a> <a id="11095" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="11116" class="Keyword">open</a> <a id="11121" class="Keyword">import</a> <a id="11128" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="11163" class="Keyword">open</a> <a id="11168" class="Keyword">import</a> <a id="11175" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="11212" class="Keyword">open</a> <a id="11217" class="Keyword">import</a> <a id="11224" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="11273" class="Keyword">open</a> <a id="11278" class="Keyword">import</a> <a id="11285" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="11308" class="Keyword">open</a> <a id="11313" class="Keyword">import</a> <a id="11320" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="11343" class="Keyword">open</a> <a id="11348" class="Keyword">import</a> <a id="11355" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="11383" class="Keyword">open</a> <a id="11388" class="Keyword">import</a> <a id="11395" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="11415" class="Keyword">open</a> <a id="11420" class="Keyword">import</a> <a id="11427" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="11458" class="Keyword">open</a> <a id="11463" class="Keyword">import</a> <a id="11470" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="11497" class="Keyword">open</a> <a id="11502" class="Keyword">import</a> <a id="11509" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="11525" class="Keyword">open</a> <a id="11530" class="Keyword">import</a> <a id="11537" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="11568" class="Keyword">open</a> <a id="11573" class="Keyword">import</a> <a id="11580" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="11597" class="Keyword">open</a> <a id="11602" class="Keyword">import</a> <a id="11609" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="11631" class="Keyword">open</a> <a id="11636" class="Keyword">import</a> <a id="11643" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="11670" class="Keyword">open</a> <a id="11675" class="Keyword">import</a> <a id="11682" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="11705" class="Keyword">open</a> <a id="11710" class="Keyword">import</a> <a id="11717" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="11744" class="Keyword">open</a> <a id="11749" class="Keyword">import</a> <a id="11756" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="11789" class="Keyword">open</a> <a id="11794" class="Keyword">import</a> <a id="11801" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="11841" class="Keyword">open</a> <a id="11846" class="Keyword">import</a> <a id="11853" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="11874" class="Keyword">open</a> <a id="11879" class="Keyword">import</a> <a id="11886" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="11915" class="Keyword">open</a> <a id="11920" class="Keyword">import</a> <a id="11927" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="11965" class="Keyword">open</a> <a id="11970" class="Keyword">import</a> <a id="11977" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="11997" class="Keyword">open</a> <a id="12002" class="Keyword">import</a> <a id="12009" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="12033" class="Keyword">open</a> <a id="12038" class="Keyword">import</a> <a id="12045" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="12072" class="Keyword">open</a> <a id="12077" class="Keyword">import</a> <a id="12084" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="12114" class="Keyword">open</a> <a id="12119" class="Keyword">import</a> <a id="12126" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="12152" class="Keyword">open</a> <a id="12157" class="Keyword">import</a> <a id="12164" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="12191" class="Keyword">open</a> <a id="12196" class="Keyword">import</a> <a id="12203" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="12232" class="Keyword">open</a> <a id="12237" class="Keyword">import</a> <a id="12244" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="12267" class="Keyword">open</a> <a id="12272" class="Keyword">import</a> <a id="12279" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="12330" class="Keyword">open</a> <a id="12335" class="Keyword">import</a> <a id="12342" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="12385" class="Keyword">open</a> <a id="12390" class="Keyword">import</a> <a id="12397" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="12445" class="Keyword">open</a> <a id="12450" class="Keyword">import</a> <a id="12457" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="12495" class="Keyword">open</a> <a id="12500" class="Keyword">import</a> <a id="12507" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="12544" class="Keyword">open</a> <a id="12549" class="Keyword">import</a> <a id="12556" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="12584" class="Keyword">open</a> <a id="12589" class="Keyword">import</a> <a id="12596" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="12632" class="Keyword">open</a> <a id="12637" class="Keyword">import</a> <a id="12644" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="12682" class="Keyword">open</a> <a id="12687" class="Keyword">import</a> <a id="12694" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="12727" class="Keyword">open</a> <a id="12732" class="Keyword">import</a> <a id="12739" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="12760" class="Keyword">open</a> <a id="12765" class="Keyword">import</a> <a id="12772" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="12826" class="Keyword">open</a> <a id="12831" class="Keyword">import</a> <a id="12838" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="12860" class="Keyword">open</a> <a id="12865" class="Keyword">import</a> <a id="12872" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="12907" class="Keyword">open</a> <a id="12912" class="Keyword">import</a> <a id="12919" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="12949" class="Keyword">open</a> <a id="12954" class="Keyword">import</a> <a id="12961" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="13000" class="Keyword">open</a> <a id="13005" class="Keyword">import</a> <a id="13012" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="13066" class="Keyword">open</a> <a id="13071" class="Keyword">import</a> <a id="13078" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="13124" class="Keyword">open</a> <a id="13129" class="Keyword">import</a> <a id="13136" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="13187" class="Keyword">open</a> <a id="13192" class="Keyword">import</a> <a id="13199" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="13240" class="Keyword">open</a> <a id="13245" class="Keyword">import</a> <a id="13252" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="13297" class="Keyword">open</a> <a id="13302" class="Keyword">import</a> <a id="13309" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="13354" class="Keyword">open</a> <a id="13359" class="Keyword">import</a> <a id="13366" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="13402" class="Keyword">open</a> <a id="13407" class="Keyword">import</a> <a id="13414" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="13450" class="Keyword">open</a> <a id="13455" class="Keyword">import</a> <a id="13462" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="13527" class="Keyword">open</a> <a id="13532" class="Keyword">import</a> <a id="13539" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="13594" class="Keyword">open</a> <a id="13599" class="Keyword">import</a> <a id="13606" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="13646" class="Keyword">open</a> <a id="13651" class="Keyword">import</a> <a id="13658" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="13702" class="Keyword">open</a> <a id="13707" class="Keyword">import</a> <a id="13714" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="13759" class="Keyword">open</a> <a id="13764" class="Keyword">import</a> <a id="13771" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="13812" class="Keyword">open</a> <a id="13817" class="Keyword">import</a> <a id="13824" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="13864" class="Keyword">open</a> <a id="13869" class="Keyword">import</a> <a id="13876" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="13903" class="Keyword">open</a> <a id="13908" class="Keyword">import</a> <a id="13915" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="13942" class="Keyword">open</a> <a id="13947" class="Keyword">import</a> <a id="13954" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="13973" class="Keyword">open</a> <a id="13978" class="Keyword">import</a> <a id="13985" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="14025" class="Keyword">open</a> <a id="14030" class="Keyword">import</a> <a id="14037" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="14102" class="Keyword">open</a> <a id="14107" class="Keyword">import</a> <a id="14114" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="14137" class="Keyword">open</a> <a id="14142" class="Keyword">import</a> <a id="14149" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="14173" class="Keyword">open</a> <a id="14178" class="Keyword">import</a> <a id="14185" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="14225" class="Keyword">open</a> <a id="14230" class="Keyword">import</a> <a id="14237" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="14280" class="Keyword">open</a> <a id="14285" class="Keyword">import</a> <a id="14292" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="14326" class="Keyword">open</a> <a id="14331" class="Keyword">import</a> <a id="14338" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="14368" class="Keyword">open</a> <a id="14373" class="Keyword">import</a> <a id="14380" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="14414" class="Keyword">open</a> <a id="14419" class="Keyword">import</a> <a id="14426" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="14461" class="Keyword">open</a> <a id="14466" class="Keyword">import</a> <a id="14473" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="14510" class="Keyword">open</a> <a id="14515" class="Keyword">import</a> <a id="14522" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="14549" class="Keyword">open</a> <a id="14554" class="Keyword">import</a> <a id="14561" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="14589" class="Keyword">open</a> <a id="14594" class="Keyword">import</a> <a id="14601" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="14650" class="Keyword">open</a> <a id="14655" class="Keyword">import</a> <a id="14662" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="14708" class="Keyword">open</a> <a id="14713" class="Keyword">import</a> <a id="14720" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="14760" class="Keyword">open</a> <a id="14765" class="Keyword">import</a> <a id="14772" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="14810" class="Keyword">open</a> <a id="14815" class="Keyword">import</a> <a id="14822" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="14851" class="Keyword">open</a> <a id="14856" class="Keyword">import</a> <a id="14863" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="14893" class="Keyword">open</a> <a id="14898" class="Keyword">import</a> <a id="14905" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="14936" class="Keyword">open</a> <a id="14941" class="Keyword">import</a> <a id="14948" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="14974" class="Keyword">open</a> <a id="14979" class="Keyword">import</a> <a id="14986" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="15037" class="Keyword">open</a> <a id="15042" class="Keyword">import</a> <a id="15049" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="15103" class="Keyword">open</a> <a id="15108" class="Keyword">import</a> <a id="15115" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="15142" class="Keyword">open</a> <a id="15147" class="Keyword">import</a> <a id="15154" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="15187" class="Keyword">open</a> <a id="15192" class="Keyword">import</a> <a id="15199" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="15230" class="Keyword">open</a> <a id="15235" class="Keyword">import</a> <a id="15242" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="15279" class="Keyword">open</a> <a id="15284" class="Keyword">import</a> <a id="15291" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="15316" class="Keyword">open</a> <a id="15321" class="Keyword">import</a> <a id="15328" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="15360" class="Keyword">open</a> <a id="15365" class="Keyword">import</a> <a id="15372" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="15407" class="Keyword">open</a> <a id="15412" class="Keyword">import</a> <a id="15419" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="15448" class="Keyword">open</a> <a id="15453" class="Keyword">import</a> <a id="15460" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="15488" class="Keyword">open</a> <a id="15493" class="Keyword">import</a> <a id="15500" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="15525" class="Keyword">open</a> <a id="15530" class="Keyword">import</a> <a id="15537" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="15558" class="Keyword">open</a> <a id="15563" class="Keyword">import</a> <a id="15570" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="15606" class="Keyword">open</a> <a id="15611" class="Keyword">import</a> <a id="15618" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="15661" class="Keyword">open</a> <a id="15666" class="Keyword">import</a> <a id="15673" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="15698" class="Keyword">open</a> <a id="15703" class="Keyword">import</a> <a id="15710" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="15741" class="Keyword">open</a> <a id="15746" class="Keyword">import</a> <a id="15753" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="15785" class="Keyword">open</a> <a id="15790" class="Keyword">import</a> <a id="15797" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="15831" class="Keyword">open</a> <a id="15836" class="Keyword">import</a> <a id="15843" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="15899" class="Keyword">open</a> <a id="15904" class="Keyword">import</a> <a id="15911" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="15964" class="Keyword">open</a> <a id="15969" class="Keyword">import</a> <a id="15976" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="16003" class="Keyword">open</a> <a id="16008" class="Keyword">import</a> <a id="16015" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="16077" class="Keyword">open</a> <a id="16082" class="Keyword">import</a> <a id="16089" href="graph-theory.html" class="Module">graph-theory</a>
<a id="16102" class="Keyword">open</a> <a id="16107" class="Keyword">import</a> <a id="16114" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="16155" class="Keyword">open</a> <a id="16160" class="Keyword">import</a> <a id="16167" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="16196" class="Keyword">open</a> <a id="16201" class="Keyword">import</a> <a id="16208" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="16253" class="Keyword">open</a> <a id="16258" class="Keyword">import</a> <a id="16265" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="16309" class="Keyword">open</a> <a id="16314" class="Keyword">import</a> <a id="16321" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="16348" class="Keyword">open</a> <a id="16353" class="Keyword">import</a> <a id="16360" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="16401" class="Keyword">open</a> <a id="16406" class="Keyword">import</a> <a id="16413" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="16462" class="Keyword">open</a> <a id="16467" class="Keyword">import</a> <a id="16474" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="16515" class="Keyword">open</a> <a id="16520" class="Keyword">import</a> <a id="16527" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="16571" class="Keyword">open</a> <a id="16576" class="Keyword">import</a> <a id="16583" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="16620" class="Keyword">open</a> <a id="16625" class="Keyword">import</a> <a id="16632" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="16654" class="Keyword">open</a> <a id="16659" class="Keyword">import</a> <a id="16666" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="16696" class="Keyword">open</a> <a id="16701" class="Keyword">import</a> <a id="16708" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="16746" class="Keyword">open</a> <a id="16751" class="Keyword">import</a> <a id="16758" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="16819" class="Keyword">open</a> <a id="16824" class="Keyword">import</a> <a id="16831" href="group-theory.html" class="Module">group-theory</a>
<a id="16844" class="Keyword">open</a> <a id="16849" class="Keyword">import</a> <a id="16856" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="16884" class="Keyword">open</a> <a id="16889" class="Keyword">import</a> <a id="16896" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="16927" class="Keyword">open</a> <a id="16932" class="Keyword">import</a> <a id="16939" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="16975" class="Keyword">open</a> <a id="16980" class="Keyword">import</a> <a id="16987" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="17019" class="Keyword">open</a> <a id="17024" class="Keyword">import</a> <a id="17031" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="17067" class="Keyword">open</a> <a id="17072" class="Keyword">import</a> <a id="17079" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="17108" class="Keyword">open</a> <a id="17113" class="Keyword">import</a> <a id="17120" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="17156" class="Keyword">open</a> <a id="17161" class="Keyword">import</a> <a id="17168" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="17197" class="Keyword">open</a> <a id="17202" class="Keyword">import</a> <a id="17209" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="17241" class="Keyword">open</a> <a id="17246" class="Keyword">import</a> <a id="17253" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="17278" class="Keyword">open</a> <a id="17283" class="Keyword">import</a> <a id="17290" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="17321" class="Keyword">open</a> <a id="17326" class="Keyword">import</a> <a id="17333" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="17373" class="Keyword">open</a> <a id="17378" class="Keyword">import</a> <a id="17385" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="17422" class="Keyword">open</a> <a id="17427" class="Keyword">import</a> <a id="17434" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="17470" class="Keyword">open</a> <a id="17475" class="Keyword">import</a> <a id="17482" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="17514" class="Keyword">open</a> <a id="17519" class="Keyword">import</a> <a id="17526" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="17553" class="Keyword">open</a> <a id="17558" class="Keyword">import</a> <a id="17565" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="17585" class="Keyword">open</a> <a id="17590" class="Keyword">import</a> <a id="17597" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="17624" class="Keyword">open</a> <a id="17629" class="Keyword">import</a> <a id="17636" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="17678" class="Keyword">open</a> <a id="17683" class="Keyword">import</a> <a id="17690" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="17731" class="Keyword">open</a> <a id="17736" class="Keyword">import</a> <a id="17743" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="17777" class="Keyword">open</a> <a id="17782" class="Keyword">import</a> <a id="17789" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="17824" class="Keyword">open</a> <a id="17829" class="Keyword">import</a> <a id="17836" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="17874" class="Keyword">open</a> <a id="17879" class="Keyword">import</a> <a id="17886" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="17927" class="Keyword">open</a> <a id="17932" class="Keyword">import</a> <a id="17939" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="17980" class="Keyword">open</a> <a id="17985" class="Keyword">import</a> <a id="17992" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="18032" class="Keyword">open</a> <a id="18037" class="Keyword">import</a> <a id="18044" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="18077" class="Keyword">open</a> <a id="18082" class="Keyword">import</a> <a id="18089" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="18126" class="Keyword">open</a> <a id="18131" class="Keyword">import</a> <a id="18138" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="18183" class="Keyword">open</a> <a id="18188" class="Keyword">import</a> <a id="18195" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="18216" class="Keyword">open</a> <a id="18221" class="Keyword">import</a> <a id="18228" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="18262" class="Keyword">open</a> <a id="18267" class="Keyword">import</a> <a id="18274" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="18316" class="Keyword">open</a> <a id="18321" class="Keyword">import</a> <a id="18328" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="18363" class="Keyword">open</a> <a id="18368" class="Keyword">import</a> <a id="18375" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="18414" class="Keyword">open</a> <a id="18419" class="Keyword">import</a> <a id="18426" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="18463" class="Keyword">open</a> <a id="18468" class="Keyword">import</a> <a id="18475" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="18499" class="Keyword">open</a> <a id="18504" class="Keyword">import</a> <a id="18511" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="18536" class="Keyword">open</a> <a id="18541" class="Keyword">import</a> <a id="18548" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="18579" class="Keyword">open</a> <a id="18584" class="Keyword">import</a> <a id="18591" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="18614" class="Keyword">open</a> <a id="18619" class="Keyword">import</a> <a id="18626" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="18674" class="Keyword">open</a> <a id="18679" class="Keyword">import</a> <a id="18686" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="18716" class="Keyword">open</a> <a id="18721" class="Keyword">import</a> <a id="18728" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="18798" class="Keyword">open</a> <a id="18803" class="Keyword">import</a> <a id="18810" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="18825" class="Keyword">open</a> <a id="18830" class="Keyword">import</a> <a id="18837" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="18870" class="Keyword">open</a> <a id="18875" class="Keyword">import</a> <a id="18882" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="18914" class="Keyword">open</a> <a id="18919" class="Keyword">import</a> <a id="18926" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="18964" class="Keyword">open</a> <a id="18969" class="Keyword">import</a> <a id="18976" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="19013" class="Keyword">open</a> <a id="19018" class="Keyword">import</a> <a id="19025" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="19058" class="Keyword">open</a> <a id="19063" class="Keyword">import</a> <a id="19070" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="19094" class="Keyword">open</a> <a id="19099" class="Keyword">import</a> <a id="19106" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="19145" class="Keyword">open</a> <a id="19150" class="Keyword">import</a> <a id="19157" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="19203" class="Keyword">open</a> <a id="19208" class="Keyword">import</a> <a id="19215" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="19260" class="Keyword">open</a> <a id="19265" class="Keyword">import</a> <a id="19272" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="19310" class="Keyword">open</a> <a id="19315" class="Keyword">import</a> <a id="19322" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="19354" class="Keyword">open</a> <a id="19359" class="Keyword">import</a> <a id="19366" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="19419" class="Keyword">open</a> <a id="19424" class="Keyword">import</a> <a id="19431" href="order-theory.html" class="Module">order-theory</a>
<a id="19444" class="Keyword">open</a> <a id="19449" class="Keyword">import</a> <a id="19456" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="19483" class="Keyword">open</a> <a id="19488" class="Keyword">import</a> <a id="19495" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="19525" class="Keyword">open</a> <a id="19530" class="Keyword">import</a> <a id="19537" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="19570" class="Keyword">open</a> <a id="19575" class="Keyword">import</a> <a id="19582" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="19618" class="Keyword">open</a> <a id="19623" class="Keyword">import</a> <a id="19630" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="19657" class="Keyword">open</a> <a id="19662" class="Keyword">import</a> <a id="19669" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="19699" class="Keyword">open</a> <a id="19704" class="Keyword">import</a> <a id="19711" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="19747" class="Keyword">open</a> <a id="19752" class="Keyword">import</a> <a id="19759" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="19791" class="Keyword">open</a> <a id="19796" class="Keyword">import</a> <a id="19803" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="19840" class="Keyword">open</a> <a id="19845" class="Keyword">import</a> <a id="19852" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="19892" class="Keyword">open</a> <a id="19897" class="Keyword">import</a> <a id="19904" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="19939" class="Keyword">open</a> <a id="19944" class="Keyword">import</a> <a id="19951" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="19989" class="Keyword">open</a> <a id="19994" class="Keyword">import</a> <a id="20001" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="20036" class="Keyword">open</a> <a id="20041" class="Keyword">import</a> <a id="20048" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="20083" class="Keyword">open</a> <a id="20088" class="Keyword">import</a> <a id="20095" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="20133" class="Keyword">open</a> <a id="20138" class="Keyword">import</a> <a id="20145" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="20178" class="Keyword">open</a> <a id="20183" class="Keyword">import</a> <a id="20190" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="20210" class="Keyword">open</a> <a id="20215" class="Keyword">import</a> <a id="20222" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="20245" class="Keyword">open</a> <a id="20250" class="Keyword">import</a> <a id="20257" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="20280" class="Keyword">open</a> <a id="20285" class="Keyword">import</a> <a id="20292" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="20318" class="Keyword">open</a> <a id="20323" class="Keyword">import</a> <a id="20330" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="20356" class="Keyword">open</a> <a id="20361" class="Keyword">import</a> <a id="20368" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="20424" class="Keyword">open</a> <a id="20429" class="Keyword">import</a> <a id="20436" href="polytopes.html" class="Module">polytopes</a>
<a id="20446" class="Keyword">open</a> <a id="20451" class="Keyword">import</a> <a id="20458" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="20516" class="Keyword">open</a> <a id="20521" class="Keyword">import</a> <a id="20528" href="ring-theory.html" class="Module">ring-theory</a>
<a id="20540" class="Keyword">open</a> <a id="20545" class="Keyword">import</a> <a id="20552" href="ring-theory.commutative-rings.html" class="Module">ring-theory.commutative-rings</a>
<a id="20582" class="Keyword">open</a> <a id="20587" class="Keyword">import</a> <a id="20594" href="ring-theory.discrete-fields.html" class="Module">ring-theory.discrete-fields</a>
<a id="20622" class="Keyword">open</a> <a id="20627" class="Keyword">import</a> <a id="20634" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="20661" class="Keyword">open</a> <a id="20666" class="Keyword">import</a> <a id="20673" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="20705" class="Keyword">open</a> <a id="20710" class="Keyword">import</a> <a id="20717" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="20747" class="Keyword">open</a> <a id="20752" class="Keyword">import</a> <a id="20759" href="ring-theory.homomorphisms-commutative-rings.html" class="Module">ring-theory.homomorphisms-commutative-rings</a>
<a id="20803" class="Keyword">open</a> <a id="20808" class="Keyword">import</a> <a id="20815" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="20847" class="Keyword">open</a> <a id="20852" class="Keyword">import</a> <a id="20859" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a>
<a id="20878" class="Keyword">open</a> <a id="20883" class="Keyword">import</a> <a id="20890" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="20928" class="Keyword">open</a> <a id="20933" class="Keyword">import</a> <a id="20940" href="ring-theory.isomorphisms-commutative-rings.html" class="Module">ring-theory.isomorphisms-commutative-rings</a>
<a id="20983" class="Keyword">open</a> <a id="20988" class="Keyword">import</a> <a id="20995" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="21026" class="Keyword">open</a> <a id="21031" class="Keyword">import</a> <a id="21038" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="21070" class="Keyword">open</a> <a id="21075" class="Keyword">import</a> <a id="21082" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="21111" class="Keyword">open</a> <a id="21116" class="Keyword">import</a> <a id="21123" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="21184" class="Keyword">open</a> <a id="21189" class="Keyword">import</a> <a id="21196" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="21222" class="Keyword">open</a> <a id="21227" class="Keyword">import</a> <a id="21234" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="21273" class="Keyword">open</a> <a id="21278" class="Keyword">import</a> <a id="21285" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="21323" class="Keyword">open</a> <a id="21328" class="Keyword">import</a> <a id="21335" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="21381" class="Keyword">open</a> <a id="21386" class="Keyword">import</a> <a id="21393" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="21430" class="Keyword">open</a> <a id="21435" class="Keyword">import</a> <a id="21442" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="21482" class="Keyword">open</a> <a id="21487" class="Keyword">import</a> <a id="21494" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="21533" class="Keyword">open</a> <a id="21538" class="Keyword">import</a> <a id="21545" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="21578" class="Keyword">open</a> <a id="21583" class="Keyword">import</a> <a id="21590" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="21629" class="Keyword">open</a> <a id="21634" class="Keyword">import</a> <a id="21641" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="21686" class="Keyword">open</a> <a id="21691" class="Keyword">import</a> <a id="21698" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="21750" class="Keyword">open</a> <a id="21755" class="Keyword">import</a> <a id="21762" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="21810" class="Keyword">open</a> <a id="21815" class="Keyword">import</a> <a id="21822" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="21862" class="Keyword">open</a> <a id="21867" class="Keyword">import</a> <a id="21874" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="21921" class="Keyword">open</a> <a id="21926" class="Keyword">import</a> <a id="21933" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="21971" class="Keyword">open</a> <a id="21976" class="Keyword">import</a> <a id="21983" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="22037" class="Keyword">open</a> <a id="22042" class="Keyword">import</a> <a id="22049" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="22096" class="Keyword">open</a> <a id="22101" class="Keyword">import</a> <a id="22108" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="22160" class="Keyword">open</a> <a id="22165" class="Keyword">import</a> <a id="22172" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="22217" class="Keyword">open</a> <a id="22222" class="Keyword">import</a> <a id="22229" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="22268" class="Keyword">open</a> <a id="22273" class="Keyword">import</a> <a id="22280" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="22320" class="Keyword">open</a> <a id="22325" class="Keyword">import</a> <a id="22332" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="22365" class="Keyword">open</a> <a id="22370" class="Keyword">import</a> <a id="22377" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="22422" class="Keyword">open</a> <a id="22427" class="Keyword">import</a> <a id="22434" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="22510" class="Keyword">open</a> <a id="22515" class="Keyword">import</a> <a id="22522" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="22584" class="Keyword">open</a> <a id="22589" class="Keyword">import</a> <a id="22596" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="22620" class="Keyword">open</a> <a id="22625" class="Keyword">import</a> <a id="22632" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="22672" class="Keyword">open</a> <a id="22677" class="Keyword">import</a> <a id="22684" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="22723" class="Keyword">open</a> <a id="22728" class="Keyword">import</a> <a id="22735" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="22783" class="Keyword">open</a> <a id="22788" class="Keyword">import</a> <a id="22795" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="22842" class="Keyword">open</a> <a id="22847" class="Keyword">import</a> <a id="22854" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="22894" class="Keyword">open</a> <a id="22899" class="Keyword">import</a> <a id="22906" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="22958" class="Keyword">open</a> <a id="22963" class="Keyword">import</a> <a id="22970" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="23028" class="Keyword">open</a> <a id="23033" class="Keyword">import</a> <a id="23040" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="23094" class="Keyword">open</a> <a id="23099" class="Keyword">import</a> <a id="23106" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="23154" class="Keyword">open</a> <a id="23159" class="Keyword">import</a> <a id="23166" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="23214" class="Keyword">open</a> <a id="23219" class="Keyword">import</a> <a id="23226" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="23265" class="Keyword">open</a> <a id="23270" class="Keyword">import</a> <a id="23277" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="23310" class="Keyword">open</a> <a id="23315" class="Keyword">import</a> <a id="23322" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="23352" class="Keyword">open</a> <a id="23357" class="Keyword">import</a> <a id="23364" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="23423" class="Keyword">open</a> <a id="23428" class="Keyword">import</a> <a id="23435" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="23490" class="Keyword">open</a> <a id="23495" class="Keyword">import</a> <a id="23502" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="23545" class="Keyword">open</a> <a id="23550" class="Keyword">import</a> <a id="23557" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="23612" class="Keyword">open</a> <a id="23617" class="Keyword">import</a> <a id="23624" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="23675" class="Keyword">open</a> <a id="23680" class="Keyword">import</a> <a id="23687" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="23765" class="Keyword">open</a> <a id="23770" class="Keyword">import</a> <a id="23777" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="23817" class="Keyword">open</a> <a id="23822" class="Keyword">import</a> <a id="23829" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="23886" class="Keyword">open</a> <a id="23891" class="Keyword">import</a> <a id="23898" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="23933" class="Keyword">open</a> <a id="23938" class="Keyword">import</a> <a id="23945" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="23991" class="Keyword">open</a> <a id="23996" class="Keyword">import</a> <a id="24003" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="24058" class="Keyword">open</a> <a id="24063" class="Keyword">import</a> <a id="24070" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="24113" class="Keyword">open</a> <a id="24118" class="Keyword">import</a> <a id="24125" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="24184" class="Keyword">open</a> <a id="24189" class="Keyword">import</a> <a id="24196" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="24233" class="Keyword">open</a> <a id="24238" class="Keyword">import</a> <a id="24245" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="24305" class="Keyword">open</a> <a id="24310" class="Keyword">import</a> <a id="24317" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="24355" class="Keyword">open</a> <a id="24360" class="Keyword">import</a> <a id="24367" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="24419" class="Keyword">open</a> <a id="24424" class="Keyword">import</a> <a id="24431" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="24477" class="Keyword">open</a> <a id="24482" class="Keyword">import</a> <a id="24489" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="24534" class="Keyword">open</a> <a id="24539" class="Keyword">import</a> <a id="24546" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="24583" class="Keyword">open</a> <a id="24588" class="Keyword">import</a> <a id="24595" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="24644" class="Keyword">open</a> <a id="24649" class="Keyword">import</a> <a id="24656" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="24694" class="Keyword">open</a> <a id="24699" class="Keyword">import</a> <a id="24706" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="24761" class="Keyword">open</a> <a id="24766" class="Keyword">import</a> <a id="24773" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="24812" class="Keyword">open</a> <a id="24817" class="Keyword">import</a> <a id="24824" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="24854" class="Keyword">open</a> <a id="24859" class="Keyword">import</a> <a id="24866" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="24896" class="Keyword">open</a> <a id="24901" class="Keyword">import</a> <a id="24908" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="24951" class="Keyword">open</a> <a id="24956" class="Keyword">import</a> <a id="24963" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="25003" class="Keyword">open</a> <a id="25008" class="Keyword">import</a> <a id="25015" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="25060" class="Keyword">open</a> <a id="25065" class="Keyword">import</a> <a id="25072" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="25122" class="Keyword">open</a> <a id="25127" class="Keyword">import</a> <a id="25134" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="25172" class="Keyword">open</a> <a id="25177" class="Keyword">import</a> <a id="25184" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="25233" class="Keyword">open</a> <a id="25238" class="Keyword">import</a> <a id="25245" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="25308" class="Keyword">open</a> <a id="25313" class="Keyword">import</a> <a id="25320" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="25373" class="Keyword">open</a> <a id="25378" class="Keyword">import</a> <a id="25385" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="25431" class="Keyword">open</a> <a id="25436" class="Keyword">import</a> <a id="25443" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="25489" class="Keyword">open</a> <a id="25494" class="Keyword">import</a> <a id="25501" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="25549" class="Keyword">open</a> <a id="25554" class="Keyword">import</a> <a id="25561" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="25631" class="Keyword">open</a> <a id="25636" class="Keyword">import</a> <a id="25643" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="25656" class="Keyword">open</a> <a id="25661" class="Keyword">import</a> <a id="25668" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="25688" class="Keyword">open</a> <a id="25693" class="Keyword">import</a> <a id="25700" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="25751" class="Keyword">open</a> <a id="25756" class="Keyword">import</a> <a id="25763" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="25788" class="Keyword">open</a> <a id="25793" class="Keyword">import</a> <a id="25800" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="25826" class="Keyword">open</a> <a id="25831" class="Keyword">import</a> <a id="25838" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

