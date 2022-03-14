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
<a id="930" class="Keyword">open</a> <a id="935" class="Keyword">import</a> <a id="942" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="982" class="Keyword">open</a> <a id="987" class="Keyword">import</a> <a id="994" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="1043" class="Keyword">open</a> <a id="1048" class="Keyword">import</a> <a id="1055" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="1098" class="Keyword">open</a> <a id="1103" class="Keyword">import</a> <a id="1110" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="1143" class="Keyword">open</a> <a id="1148" class="Keyword">import</a> <a id="1155" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="1191" class="Keyword">open</a> <a id="1196" class="Keyword">import</a> <a id="1203" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="1253" class="Keyword">open</a> <a id="1258" class="Keyword">import</a> <a id="1265" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="1313" class="Keyword">open</a> <a id="1318" class="Keyword">import</a> <a id="1325" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="1382" class="Keyword">open</a> <a id="1387" class="Keyword">import</a> <a id="1394" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="1445" class="Keyword">open</a> <a id="1450" class="Keyword">import</a> <a id="1457" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="1508" class="Keyword">open</a> <a id="1513" class="Keyword">import</a> <a id="1520" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="1580" class="Keyword">open</a> <a id="1585" class="Keyword">import</a> <a id="1592" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="1646" class="Keyword">open</a> <a id="1651" class="Keyword">import</a> <a id="1658" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="1730" class="Keyword">open</a> <a id="1735" class="Keyword">import</a> <a id="1742" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="1767" class="Keyword">open</a> <a id="1772" class="Keyword">import</a> <a id="1779" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="1828" class="Keyword">open</a> <a id="1833" class="Keyword">import</a> <a id="1840" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="1883" class="Keyword">open</a> <a id="1888" class="Keyword">import</a> <a id="1895" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="1945" class="Keyword">open</a> <a id="1950" class="Keyword">import</a> <a id="1957" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="2004" class="Keyword">open</a> <a id="2009" class="Keyword">import</a> <a id="2016" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="2059" class="Keyword">open</a> <a id="2064" class="Keyword">import</a> <a id="2071" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="2115" class="Keyword">open</a> <a id="2120" class="Keyword">import</a> <a id="2127" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="2172" class="Keyword">open</a> <a id="2177" class="Keyword">import</a> <a id="2184" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="2236" class="Keyword">open</a> <a id="2241" class="Keyword">import</a> <a id="2248" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="2289" class="Keyword">open</a> <a id="2294" class="Keyword">import</a> <a id="2301" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="2346" class="Keyword">open</a> <a id="2351" class="Keyword">import</a> <a id="2358" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="2401" class="Keyword">open</a> <a id="2406" class="Keyword">import</a> <a id="2413" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="2463" class="Keyword">open</a> <a id="2468" class="Keyword">import</a> <a id="2475" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="2522" class="Keyword">open</a> <a id="2527" class="Keyword">import</a> <a id="2534" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="2591" class="Keyword">open</a> <a id="2596" class="Keyword">import</a> <a id="2603" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="2657" class="Keyword">open</a> <a id="2662" class="Keyword">import</a> <a id="2669" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="2729" class="Keyword">open</a> <a id="2734" class="Keyword">import</a> <a id="2741" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="2784" class="Keyword">open</a> <a id="2789" class="Keyword">import</a> <a id="2796" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="2846" class="Keyword">open</a> <a id="2851" class="Keyword">import</a> <a id="2858" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="2918" class="Keyword">open</a> <a id="2923" class="Keyword">import</a> <a id="2930" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="2979" class="Keyword">open</a> <a id="2984" class="Keyword">import</a> <a id="2991" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="3047" class="Keyword">open</a> <a id="3052" class="Keyword">import</a> <a id="3059" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="3095" class="Keyword">open</a> <a id="3100" class="Keyword">import</a> <a id="3107" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="3151" class="Keyword">open</a> <a id="3156" class="Keyword">import</a> <a id="3163" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="3207" class="Keyword">open</a> <a id="3212" class="Keyword">import</a> <a id="3219" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="3269" class="Keyword">open</a> <a id="3274" class="Keyword">import</a> <a id="3281" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="3327" class="Keyword">open</a> <a id="3332" class="Keyword">import</a> <a id="3339" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="3374" class="Keyword">open</a> <a id="3379" class="Keyword">import</a> <a id="3386" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="3431" class="Keyword">open</a> <a id="3436" class="Keyword">import</a> <a id="3443" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="3501" class="Keyword">open</a> <a id="3506" class="Keyword">import</a> <a id="3513" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="3578" class="Keyword">open</a> <a id="3583" class="Keyword">import</a> <a id="3590" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="3635" class="Keyword">open</a> <a id="3640" class="Keyword">import</a> <a id="3647" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="3699" class="Keyword">open</a> <a id="3704" class="Keyword">import</a> <a id="3711" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="3769" class="Keyword">open</a> <a id="3774" class="Keyword">import</a> <a id="3781" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="3827" class="Keyword">open</a> <a id="3832" class="Keyword">import</a> <a id="3839" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="3873" class="Keyword">open</a> <a id="3878" class="Keyword">import</a> <a id="3885" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="3930" class="Keyword">open</a> <a id="3935" class="Keyword">import</a> <a id="3942" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="3996" class="Keyword">open</a> <a id="4001" class="Keyword">import</a> <a id="4008" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="4074" class="Keyword">open</a> <a id="4079" class="Keyword">import</a> <a id="4086" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="4130" class="Keyword">open</a> <a id="4135" class="Keyword">import</a> <a id="4142" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="4191" class="Keyword">open</a> <a id="4196" class="Keyword">import</a> <a id="4203" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="4259" class="Keyword">open</a> <a id="4264" class="Keyword">import</a> <a id="4271" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="4312" class="Keyword">open</a> <a id="4317" class="Keyword">import</a> <a id="4324" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="4383" class="Keyword">open</a> <a id="4388" class="Keyword">import</a> <a id="4395" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="4434" class="Keyword">open</a> <a id="4439" class="Keyword">import</a> <a id="4446" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="4499" class="Keyword">open</a> <a id="4504" class="Keyword">import</a> <a id="4511" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="4568" class="Keyword">open</a> <a id="4573" class="Keyword">import</a> <a id="4580" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="4622" class="Keyword">open</a> <a id="4627" class="Keyword">import</a> <a id="4634" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="4685" class="Keyword">open</a> <a id="4690" class="Keyword">import</a> <a id="4697" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="4755" class="Keyword">open</a> <a id="4760" class="Keyword">import</a> <a id="4767" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="4831" class="Keyword">open</a> <a id="4836" class="Keyword">import</a> <a id="4843" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="4896" class="Keyword">open</a> <a id="4901" class="Keyword">import</a> <a id="4908" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="4969" class="Keyword">open</a> <a id="4974" class="Keyword">import</a> <a id="4981" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="5039" class="Keyword">open</a> <a id="5044" class="Keyword">import</a> <a id="5051" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="5100" class="Keyword">open</a> <a id="5105" class="Keyword">import</a> <a id="5112" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="5156" class="Keyword">open</a> <a id="5161" class="Keyword">import</a> <a id="5168" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="5215" class="Keyword">open</a> <a id="5220" class="Keyword">import</a> <a id="5227" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="5287" class="Keyword">open</a> <a id="5292" class="Keyword">import</a> <a id="5299" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="5353" class="Keyword">open</a> <a id="5358" class="Keyword">import</a> <a id="5365" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="5426" class="Keyword">open</a> <a id="5431" class="Keyword">import</a> <a id="5438" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="5501" class="Keyword">open</a> <a id="5506" class="Keyword">import</a> <a id="5513" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="5578" class="Keyword">open</a> <a id="5583" class="Keyword">import</a> <a id="5590" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="5698" class="Keyword">open</a> <a id="5703" class="Keyword">import</a> <a id="5710" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="5730" class="Keyword">open</a> <a id="5735" class="Keyword">import</a> <a id="5742" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="5788" class="Keyword">open</a> <a id="5793" class="Keyword">import</a> <a id="5800" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="5846" class="Keyword">open</a> <a id="5851" class="Keyword">import</a> <a id="5858" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="5892" class="Keyword">open</a> <a id="5897" class="Keyword">import</a> <a id="5904" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="5944" class="Keyword">open</a> <a id="5949" class="Keyword">import</a> <a id="5956" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="6019" class="Keyword">open</a> <a id="6024" class="Keyword">import</a> <a id="6031" href="foundation.html" class="Module">foundation</a>
<a id="6042" class="Keyword">open</a> <a id="6047" class="Keyword">import</a> <a id="6054" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="6072" class="Keyword">open</a> <a id="6077" class="Keyword">import</a> <a id="6084" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="6103" class="Keyword">open</a> <a id="6108" class="Keyword">import</a> <a id="6115" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="6134" class="Keyword">open</a> <a id="6139" class="Keyword">import</a> <a id="6146" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="6190" class="Keyword">open</a> <a id="6195" class="Keyword">import</a> <a id="6202" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="6227" class="Keyword">open</a> <a id="6232" class="Keyword">import</a> <a id="6239" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="6266" class="Keyword">open</a> <a id="6271" class="Keyword">import</a> <a id="6278" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="6307" class="Keyword">open</a> <a id="6312" class="Keyword">import</a> <a id="6319" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="6350" class="Keyword">open</a> <a id="6355" class="Keyword">import</a> <a id="6362" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="6390" class="Keyword">open</a> <a id="6395" class="Keyword">import</a> <a id="6402" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="6432" class="Keyword">open</a> <a id="6437" class="Keyword">import</a> <a id="6444" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="6464" class="Keyword">open</a> <a id="6469" class="Keyword">import</a> <a id="6476" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="6513" class="Keyword">open</a> <a id="6518" class="Keyword">import</a> <a id="6525" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="6560" class="Keyword">open</a> <a id="6565" class="Keyword">import</a> <a id="6572" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="6630" class="Keyword">open</a> <a id="6635" class="Keyword">import</a> <a id="6642" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="6680" class="Keyword">open</a> <a id="6685" class="Keyword">import</a> <a id="6692" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="6721" class="Keyword">open</a> <a id="6726" class="Keyword">import</a> <a id="6733" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="6756" class="Keyword">open</a> <a id="6761" class="Keyword">import</a> <a id="6768" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="6791" class="Keyword">open</a> <a id="6796" class="Keyword">import</a> <a id="6803" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="6845" class="Keyword">open</a> <a id="6850" class="Keyword">import</a> <a id="6857" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="6889" class="Keyword">open</a> <a id="6894" class="Keyword">import</a> <a id="6901" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="6928" class="Keyword">open</a> <a id="6933" class="Keyword">import</a> <a id="6940" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="6965" class="Keyword">open</a> <a id="6970" class="Keyword">import</a> <a id="6977" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="7006" class="Keyword">open</a> <a id="7011" class="Keyword">import</a> <a id="7018" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="7048" class="Keyword">open</a> <a id="7053" class="Keyword">import</a> <a id="7060" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="7087" class="Keyword">open</a> <a id="7092" class="Keyword">import</a> <a id="7099" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="7118" class="Keyword">open</a> <a id="7123" class="Keyword">import</a> <a id="7130" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="7176" class="Keyword">open</a> <a id="7181" class="Keyword">import</a> <a id="7188" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="7230" class="Keyword">open</a> <a id="7235" class="Keyword">import</a> <a id="7242" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="7274" class="Keyword">open</a> <a id="7279" class="Keyword">import</a> <a id="7286" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="7316" class="Keyword">open</a> <a id="7321" class="Keyword">import</a> <a id="7328" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="7354" class="Keyword">open</a> <a id="7359" class="Keyword">import</a> <a id="7366" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="7400" class="Keyword">open</a> <a id="7405" class="Keyword">import</a> <a id="7412" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="7442" class="Keyword">open</a> <a id="7447" class="Keyword">import</a> <a id="7454" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="7481" class="Keyword">open</a> <a id="7486" class="Keyword">import</a> <a id="7493" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="7525" class="Keyword">open</a> <a id="7530" class="Keyword">import</a> <a id="7537" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="7571" class="Keyword">open</a> <a id="7576" class="Keyword">import</a> <a id="7583" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="7606" class="Keyword">open</a> <a id="7611" class="Keyword">import</a> <a id="7618" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="7688" class="Keyword">open</a> <a id="7693" class="Keyword">import</a> <a id="7700" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="7770" class="Keyword">open</a> <a id="7775" class="Keyword">import</a> <a id="7782" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="7809" class="Keyword">open</a> <a id="7814" class="Keyword">import</a> <a id="7821" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="7869" class="Keyword">open</a> <a id="7874" class="Keyword">import</a> <a id="7881" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="7921" class="Keyword">open</a> <a id="7926" class="Keyword">import</a> <a id="7933" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="7955" class="Keyword">open</a> <a id="7960" class="Keyword">import</a> <a id="7967" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="7990" class="Keyword">open</a> <a id="7995" class="Keyword">import</a> <a id="8002" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="8047" class="Keyword">open</a> <a id="8052" class="Keyword">import</a> <a id="8059" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="8103" class="Keyword">open</a> <a id="8108" class="Keyword">import</a> <a id="8115" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="8151" class="Keyword">open</a> <a id="8156" class="Keyword">import</a> <a id="8163" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="8208" class="Keyword">open</a> <a id="8213" class="Keyword">import</a> <a id="8220" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="8261" class="Keyword">open</a> <a id="8266" class="Keyword">import</a> <a id="8273" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="8308" class="Keyword">open</a> <a id="8313" class="Keyword">import</a> <a id="8320" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="8351" class="Keyword">open</a> <a id="8356" class="Keyword">import</a> <a id="8363" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="8396" class="Keyword">open</a> <a id="8401" class="Keyword">import</a> <a id="8408" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="8441" class="Keyword">open</a> <a id="8446" class="Keyword">import</a> <a id="8453" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="8483" class="Keyword">open</a> <a id="8488" class="Keyword">import</a> <a id="8495" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="8519" class="Keyword">open</a> <a id="8524" class="Keyword">import</a> <a id="8531" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="8569" class="Keyword">open</a> <a id="8574" class="Keyword">import</a> <a id="8581" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="8612" class="Keyword">open</a> <a id="8617" class="Keyword">import</a> <a id="8624" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="8649" class="Keyword">open</a> <a id="8654" class="Keyword">import</a> <a id="8661" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="8689" class="Keyword">open</a> <a id="8694" class="Keyword">import</a> <a id="8701" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="8725" class="Keyword">open</a> <a id="8730" class="Keyword">import</a> <a id="8737" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="8763" class="Keyword">open</a> <a id="8768" class="Keyword">import</a> <a id="8775" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="8810" class="Keyword">open</a> <a id="8815" class="Keyword">import</a> <a id="8822" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="8843" class="Keyword">open</a> <a id="8848" class="Keyword">import</a> <a id="8855" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="8904" class="Keyword">open</a> <a id="8909" class="Keyword">import</a> <a id="8916" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="8957" class="Keyword">open</a> <a id="8962" class="Keyword">import</a> <a id="8969" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="9019" class="Keyword">open</a> <a id="9024" class="Keyword">import</a> <a id="9031" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="9077" class="Keyword">open</a> <a id="9082" class="Keyword">import</a> <a id="9089" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="9129" class="Keyword">open</a> <a id="9134" class="Keyword">import</a> <a id="9141" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="9191" class="Keyword">open</a> <a id="9196" class="Keyword">import</a> <a id="9203" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="9242" class="Keyword">open</a> <a id="9247" class="Keyword">import</a> <a id="9254" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="9294" class="Keyword">open</a> <a id="9299" class="Keyword">import</a> <a id="9306" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="9339" class="Keyword">open</a> <a id="9344" class="Keyword">import</a> <a id="9351" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="9400" class="Keyword">open</a> <a id="9405" class="Keyword">import</a> <a id="9412" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="9437" class="Keyword">open</a> <a id="9442" class="Keyword">import</a> <a id="9449" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="9471" class="Keyword">open</a> <a id="9476" class="Keyword">import</a> <a id="9483" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="9511" class="Keyword">open</a> <a id="9516" class="Keyword">import</a> <a id="9523" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="9549" class="Keyword">open</a> <a id="9554" class="Keyword">import</a> <a id="9561" href="foundation.images.html" class="Module">foundation.images</a>
<a id="9579" class="Keyword">open</a> <a id="9584" class="Keyword">import</a> <a id="9591" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="9626" class="Keyword">open</a> <a id="9631" class="Keyword">import</a> <a id="9638" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="9665" class="Keyword">open</a> <a id="9670" class="Keyword">import</a> <a id="9677" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="9733" class="Keyword">open</a> <a id="9738" class="Keyword">import</a> <a id="9745" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="9774" class="Keyword">open</a> <a id="9779" class="Keyword">import</a> <a id="9786" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="9816" class="Keyword">open</a> <a id="9821" class="Keyword">import</a> <a id="9828" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="9854" class="Keyword">open</a> <a id="9859" class="Keyword">import</a> <a id="9866" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="9893" class="Keyword">open</a> <a id="9898" class="Keyword">import</a> <a id="9905" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="9928" class="Keyword">open</a> <a id="9933" class="Keyword">import</a> <a id="9940" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="9967" class="Keyword">open</a> <a id="9972" class="Keyword">import</a> <a id="9979" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="10011" class="Keyword">open</a> <a id="10016" class="Keyword">import</a> <a id="10023" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="10057" class="Keyword">open</a> <a id="10062" class="Keyword">import</a> <a id="10069" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="10109" class="Keyword">open</a> <a id="10114" class="Keyword">import</a> <a id="10121" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="10152" class="Keyword">open</a> <a id="10157" class="Keyword">import</a> <a id="10164" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="10196" class="Keyword">open</a> <a id="10201" class="Keyword">import</a> <a id="10208" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="10225" class="Keyword">open</a> <a id="10230" class="Keyword">import</a> <a id="10237" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="10262" class="Keyword">open</a> <a id="10267" class="Keyword">import</a> <a id="10274" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="10303" class="Keyword">open</a> <a id="10308" class="Keyword">import</a> <a id="10315" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="10340" class="Keyword">open</a> <a id="10345" class="Keyword">import</a> <a id="10352" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="10373" class="Keyword">open</a> <a id="10378" class="Keyword">import</a> <a id="10385" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="10405" class="Keyword">open</a> <a id="10410" class="Keyword">import</a> <a id="10417" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="10451" class="Keyword">open</a> <a id="10456" class="Keyword">import</a> <a id="10463" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="10487" class="Keyword">open</a> <a id="10492" class="Keyword">import</a> <a id="10499" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="10526" class="Keyword">open</a> <a id="10531" class="Keyword">import</a> <a id="10538" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="10573" class="Keyword">open</a> <a id="10578" class="Keyword">import</a> <a id="10585" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="10625" class="Keyword">open</a> <a id="10630" class="Keyword">import</a> <a id="10637" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="10667" class="Keyword">open</a> <a id="10672" class="Keyword">import</a> <a id="10679" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="10716" class="Keyword">open</a> <a id="10721" class="Keyword">import</a> <a id="10728" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="10752" class="Keyword">open</a> <a id="10757" class="Keyword">import</a> <a id="10764" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="10785" class="Keyword">open</a> <a id="10790" class="Keyword">import</a> <a id="10797" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="10832" class="Keyword">open</a> <a id="10837" class="Keyword">import</a> <a id="10844" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="10881" class="Keyword">open</a> <a id="10886" class="Keyword">import</a> <a id="10893" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="10942" class="Keyword">open</a> <a id="10947" class="Keyword">import</a> <a id="10954" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="10977" class="Keyword">open</a> <a id="10982" class="Keyword">import</a> <a id="10989" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="11012" class="Keyword">open</a> <a id="11017" class="Keyword">import</a> <a id="11024" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="11052" class="Keyword">open</a> <a id="11057" class="Keyword">import</a> <a id="11064" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="11084" class="Keyword">open</a> <a id="11089" class="Keyword">import</a> <a id="11096" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="11127" class="Keyword">open</a> <a id="11132" class="Keyword">import</a> <a id="11139" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="11166" class="Keyword">open</a> <a id="11171" class="Keyword">import</a> <a id="11178" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="11194" class="Keyword">open</a> <a id="11199" class="Keyword">import</a> <a id="11206" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="11237" class="Keyword">open</a> <a id="11242" class="Keyword">import</a> <a id="11249" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="11266" class="Keyword">open</a> <a id="11271" class="Keyword">import</a> <a id="11278" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="11300" class="Keyword">open</a> <a id="11305" class="Keyword">import</a> <a id="11312" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="11339" class="Keyword">open</a> <a id="11344" class="Keyword">import</a> <a id="11351" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="11374" class="Keyword">open</a> <a id="11379" class="Keyword">import</a> <a id="11386" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="11413" class="Keyword">open</a> <a id="11418" class="Keyword">import</a> <a id="11425" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="11458" class="Keyword">open</a> <a id="11463" class="Keyword">import</a> <a id="11470" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="11510" class="Keyword">open</a> <a id="11515" class="Keyword">import</a> <a id="11522" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="11543" class="Keyword">open</a> <a id="11548" class="Keyword">import</a> <a id="11555" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="11584" class="Keyword">open</a> <a id="11589" class="Keyword">import</a> <a id="11596" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="11634" class="Keyword">open</a> <a id="11639" class="Keyword">import</a> <a id="11646" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="11666" class="Keyword">open</a> <a id="11671" class="Keyword">import</a> <a id="11678" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="11702" class="Keyword">open</a> <a id="11707" class="Keyword">import</a> <a id="11714" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="11741" class="Keyword">open</a> <a id="11746" class="Keyword">import</a> <a id="11753" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="11783" class="Keyword">open</a> <a id="11788" class="Keyword">import</a> <a id="11795" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="11821" class="Keyword">open</a> <a id="11826" class="Keyword">import</a> <a id="11833" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="11860" class="Keyword">open</a> <a id="11865" class="Keyword">import</a> <a id="11872" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="11901" class="Keyword">open</a> <a id="11906" class="Keyword">import</a> <a id="11913" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="11936" class="Keyword">open</a> <a id="11941" class="Keyword">import</a> <a id="11948" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="11999" class="Keyword">open</a> <a id="12004" class="Keyword">import</a> <a id="12011" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="12054" class="Keyword">open</a> <a id="12059" class="Keyword">import</a> <a id="12066" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="12114" class="Keyword">open</a> <a id="12119" class="Keyword">import</a> <a id="12126" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="12164" class="Keyword">open</a> <a id="12169" class="Keyword">import</a> <a id="12176" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="12213" class="Keyword">open</a> <a id="12218" class="Keyword">import</a> <a id="12225" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="12253" class="Keyword">open</a> <a id="12258" class="Keyword">import</a> <a id="12265" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="12301" class="Keyword">open</a> <a id="12306" class="Keyword">import</a> <a id="12313" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="12351" class="Keyword">open</a> <a id="12356" class="Keyword">import</a> <a id="12363" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="12396" class="Keyword">open</a> <a id="12401" class="Keyword">import</a> <a id="12408" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="12429" class="Keyword">open</a> <a id="12434" class="Keyword">import</a> <a id="12441" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="12495" class="Keyword">open</a> <a id="12500" class="Keyword">import</a> <a id="12507" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="12529" class="Keyword">open</a> <a id="12534" class="Keyword">import</a> <a id="12541" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="12576" class="Keyword">open</a> <a id="12581" class="Keyword">import</a> <a id="12588" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="12618" class="Keyword">open</a> <a id="12623" class="Keyword">import</a> <a id="12630" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="12669" class="Keyword">open</a> <a id="12674" class="Keyword">import</a> <a id="12681" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="12735" class="Keyword">open</a> <a id="12740" class="Keyword">import</a> <a id="12747" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="12793" class="Keyword">open</a> <a id="12798" class="Keyword">import</a> <a id="12805" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="12856" class="Keyword">open</a> <a id="12861" class="Keyword">import</a> <a id="12868" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="12909" class="Keyword">open</a> <a id="12914" class="Keyword">import</a> <a id="12921" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="12966" class="Keyword">open</a> <a id="12971" class="Keyword">import</a> <a id="12978" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="13023" class="Keyword">open</a> <a id="13028" class="Keyword">import</a> <a id="13035" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="13071" class="Keyword">open</a> <a id="13076" class="Keyword">import</a> <a id="13083" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="13119" class="Keyword">open</a> <a id="13124" class="Keyword">import</a> <a id="13131" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="13196" class="Keyword">open</a> <a id="13201" class="Keyword">import</a> <a id="13208" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="13263" class="Keyword">open</a> <a id="13268" class="Keyword">import</a> <a id="13275" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="13315" class="Keyword">open</a> <a id="13320" class="Keyword">import</a> <a id="13327" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="13371" class="Keyword">open</a> <a id="13376" class="Keyword">import</a> <a id="13383" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="13428" class="Keyword">open</a> <a id="13433" class="Keyword">import</a> <a id="13440" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="13481" class="Keyword">open</a> <a id="13486" class="Keyword">import</a> <a id="13493" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="13533" class="Keyword">open</a> <a id="13538" class="Keyword">import</a> <a id="13545" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="13572" class="Keyword">open</a> <a id="13577" class="Keyword">import</a> <a id="13584" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="13611" class="Keyword">open</a> <a id="13616" class="Keyword">import</a> <a id="13623" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="13642" class="Keyword">open</a> <a id="13647" class="Keyword">import</a> <a id="13654" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="13694" class="Keyword">open</a> <a id="13699" class="Keyword">import</a> <a id="13706" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="13771" class="Keyword">open</a> <a id="13776" class="Keyword">import</a> <a id="13783" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="13806" class="Keyword">open</a> <a id="13811" class="Keyword">import</a> <a id="13818" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="13842" class="Keyword">open</a> <a id="13847" class="Keyword">import</a> <a id="13854" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="13894" class="Keyword">open</a> <a id="13899" class="Keyword">import</a> <a id="13906" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="13949" class="Keyword">open</a> <a id="13954" class="Keyword">import</a> <a id="13961" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="13995" class="Keyword">open</a> <a id="14000" class="Keyword">import</a> <a id="14007" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="14037" class="Keyword">open</a> <a id="14042" class="Keyword">import</a> <a id="14049" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="14083" class="Keyword">open</a> <a id="14088" class="Keyword">import</a> <a id="14095" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="14130" class="Keyword">open</a> <a id="14135" class="Keyword">import</a> <a id="14142" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="14179" class="Keyword">open</a> <a id="14184" class="Keyword">import</a> <a id="14191" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="14218" class="Keyword">open</a> <a id="14223" class="Keyword">import</a> <a id="14230" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="14258" class="Keyword">open</a> <a id="14263" class="Keyword">import</a> <a id="14270" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="14319" class="Keyword">open</a> <a id="14324" class="Keyword">import</a> <a id="14331" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="14377" class="Keyword">open</a> <a id="14382" class="Keyword">import</a> <a id="14389" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="14429" class="Keyword">open</a> <a id="14434" class="Keyword">import</a> <a id="14441" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="14479" class="Keyword">open</a> <a id="14484" class="Keyword">import</a> <a id="14491" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="14520" class="Keyword">open</a> <a id="14525" class="Keyword">import</a> <a id="14532" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="14562" class="Keyword">open</a> <a id="14567" class="Keyword">import</a> <a id="14574" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="14605" class="Keyword">open</a> <a id="14610" class="Keyword">import</a> <a id="14617" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="14643" class="Keyword">open</a> <a id="14648" class="Keyword">import</a> <a id="14655" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="14706" class="Keyword">open</a> <a id="14711" class="Keyword">import</a> <a id="14718" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="14772" class="Keyword">open</a> <a id="14777" class="Keyword">import</a> <a id="14784" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="14811" class="Keyword">open</a> <a id="14816" class="Keyword">import</a> <a id="14823" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="14856" class="Keyword">open</a> <a id="14861" class="Keyword">import</a> <a id="14868" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="14899" class="Keyword">open</a> <a id="14904" class="Keyword">import</a> <a id="14911" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="14948" class="Keyword">open</a> <a id="14953" class="Keyword">import</a> <a id="14960" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="14985" class="Keyword">open</a> <a id="14990" class="Keyword">import</a> <a id="14997" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="15029" class="Keyword">open</a> <a id="15034" class="Keyword">import</a> <a id="15041" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="15076" class="Keyword">open</a> <a id="15081" class="Keyword">import</a> <a id="15088" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="15117" class="Keyword">open</a> <a id="15122" class="Keyword">import</a> <a id="15129" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="15157" class="Keyword">open</a> <a id="15162" class="Keyword">import</a> <a id="15169" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="15194" class="Keyword">open</a> <a id="15199" class="Keyword">import</a> <a id="15206" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="15227" class="Keyword">open</a> <a id="15232" class="Keyword">import</a> <a id="15239" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="15275" class="Keyword">open</a> <a id="15280" class="Keyword">import</a> <a id="15287" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="15330" class="Keyword">open</a> <a id="15335" class="Keyword">import</a> <a id="15342" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="15367" class="Keyword">open</a> <a id="15372" class="Keyword">import</a> <a id="15379" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="15410" class="Keyword">open</a> <a id="15415" class="Keyword">import</a> <a id="15422" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="15454" class="Keyword">open</a> <a id="15459" class="Keyword">import</a> <a id="15466" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="15500" class="Keyword">open</a> <a id="15505" class="Keyword">import</a> <a id="15512" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="15568" class="Keyword">open</a> <a id="15573" class="Keyword">import</a> <a id="15580" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="15633" class="Keyword">open</a> <a id="15638" class="Keyword">import</a> <a id="15645" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="15672" class="Keyword">open</a> <a id="15677" class="Keyword">import</a> <a id="15684" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="15746" class="Keyword">open</a> <a id="15751" class="Keyword">import</a> <a id="15758" href="graph-theory.html" class="Module">graph-theory</a>
<a id="15771" class="Keyword">open</a> <a id="15776" class="Keyword">import</a> <a id="15783" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="15812" class="Keyword">open</a> <a id="15817" class="Keyword">import</a> <a id="15824" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="15851" class="Keyword">open</a> <a id="15856" class="Keyword">import</a> <a id="15863" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="15885" class="Keyword">open</a> <a id="15890" class="Keyword">import</a> <a id="15897" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="15927" class="Keyword">open</a> <a id="15932" class="Keyword">import</a> <a id="15939" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="16000" class="Keyword">open</a> <a id="16005" class="Keyword">import</a> <a id="16012" href="group-theory.html" class="Module">group-theory</a>
<a id="16025" class="Keyword">open</a> <a id="16030" class="Keyword">import</a> <a id="16037" href="group-theory.abstract-abelian-groups.html" class="Module">group-theory.abstract-abelian-groups</a>
<a id="16074" class="Keyword">open</a> <a id="16079" class="Keyword">import</a> <a id="16086" href="group-theory.abstract-abelian-subgroups.html" class="Module">group-theory.abstract-abelian-subgroups</a>
<a id="16126" class="Keyword">open</a> <a id="16131" class="Keyword">import</a> <a id="16138" href="group-theory.abstract-group-actions.html" class="Module">group-theory.abstract-group-actions</a>
<a id="16174" class="Keyword">open</a> <a id="16179" class="Keyword">import</a> <a id="16186" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="16222" class="Keyword">open</a> <a id="16227" class="Keyword">import</a> <a id="16234" href="group-theory.abstract-groups.html" class="Module">group-theory.abstract-groups</a>
<a id="16263" class="Keyword">open</a> <a id="16268" class="Keyword">import</a> <a id="16275" href="group-theory.abstract-subgroups.html" class="Module">group-theory.abstract-subgroups</a>
<a id="16307" class="Keyword">open</a> <a id="16312" class="Keyword">import</a> <a id="16319" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="16355" class="Keyword">open</a> <a id="16360" class="Keyword">import</a> <a id="16367" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="16396" class="Keyword">open</a> <a id="16401" class="Keyword">import</a> <a id="16408" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="16440" class="Keyword">open</a> <a id="16445" class="Keyword">import</a> <a id="16452" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="16488" class="Keyword">open</a> <a id="16493" class="Keyword">import</a> <a id="16500" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="16532" class="Keyword">open</a> <a id="16537" class="Keyword">import</a> <a id="16544" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="16571" class="Keyword">open</a> <a id="16576" class="Keyword">import</a> <a id="16583" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="16640" class="Keyword">open</a> <a id="16645" class="Keyword">import</a> <a id="16652" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="16667" class="Keyword">open</a> <a id="16672" class="Keyword">import</a> <a id="16679" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="16703" class="Keyword">open</a> <a id="16708" class="Keyword">import</a> <a id="16715" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="16768" class="Keyword">open</a> <a id="16773" class="Keyword">import</a> <a id="16780" href="order-theory.html" class="Module">order-theory</a>
<a id="16793" class="Keyword">open</a> <a id="16798" class="Keyword">import</a> <a id="16805" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="16832" class="Keyword">open</a> <a id="16837" class="Keyword">import</a> <a id="16844" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="16874" class="Keyword">open</a> <a id="16879" class="Keyword">import</a> <a id="16886" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="16922" class="Keyword">open</a> <a id="16927" class="Keyword">import</a> <a id="16934" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="16967" class="Keyword">open</a> <a id="16972" class="Keyword">import</a> <a id="16979" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="16999" class="Keyword">open</a> <a id="17004" class="Keyword">import</a> <a id="17011" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="17061" class="Keyword">open</a> <a id="17066" class="Keyword">import</a> <a id="17073" href="polytopes.html" class="Module">polytopes</a>
<a id="17083" class="Keyword">open</a> <a id="17088" class="Keyword">import</a> <a id="17095" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="17153" class="Keyword">open</a> <a id="17158" class="Keyword">import</a> <a id="17165" href="ring-theory.html" class="Module">ring-theory</a>
<a id="17177" class="Keyword">open</a> <a id="17182" class="Keyword">import</a> <a id="17189" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="17221" class="Keyword">open</a> <a id="17226" class="Keyword">import</a> <a id="17233" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="17263" class="Keyword">open</a> <a id="17268" class="Keyword">import</a> <a id="17275" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a>
<a id="17294" class="Keyword">open</a> <a id="17299" class="Keyword">import</a> <a id="17306" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="17338" class="Keyword">open</a> <a id="17343" class="Keyword">import</a> <a id="17350" href="ring-theory.rings-with-properties.html" class="Module">ring-theory.rings-with-properties</a>
<a id="17384" class="Keyword">open</a> <a id="17389" class="Keyword">import</a> <a id="17396" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="17457" class="Keyword">open</a> <a id="17462" class="Keyword">import</a> <a id="17469" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="17495" class="Keyword">open</a> <a id="17500" class="Keyword">import</a> <a id="17507" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="17546" class="Keyword">open</a> <a id="17551" class="Keyword">import</a> <a id="17558" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="17596" class="Keyword">open</a> <a id="17601" class="Keyword">import</a> <a id="17608" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="17654" class="Keyword">open</a> <a id="17659" class="Keyword">import</a> <a id="17666" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="17703" class="Keyword">open</a> <a id="17708" class="Keyword">import</a> <a id="17715" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="17755" class="Keyword">open</a> <a id="17760" class="Keyword">import</a> <a id="17767" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="17806" class="Keyword">open</a> <a id="17811" class="Keyword">import</a> <a id="17818" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="17851" class="Keyword">open</a> <a id="17856" class="Keyword">import</a> <a id="17863" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="17902" class="Keyword">open</a> <a id="17907" class="Keyword">import</a> <a id="17914" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="17959" class="Keyword">open</a> <a id="17964" class="Keyword">import</a> <a id="17971" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="18023" class="Keyword">open</a> <a id="18028" class="Keyword">import</a> <a id="18035" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="18083" class="Keyword">open</a> <a id="18088" class="Keyword">import</a> <a id="18095" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="18135" class="Keyword">open</a> <a id="18140" class="Keyword">import</a> <a id="18147" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="18194" class="Keyword">open</a> <a id="18199" class="Keyword">import</a> <a id="18206" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="18244" class="Keyword">open</a> <a id="18249" class="Keyword">import</a> <a id="18256" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="18310" class="Keyword">open</a> <a id="18315" class="Keyword">import</a> <a id="18322" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="18369" class="Keyword">open</a> <a id="18374" class="Keyword">import</a> <a id="18381" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="18433" class="Keyword">open</a> <a id="18438" class="Keyword">import</a> <a id="18445" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="18490" class="Keyword">open</a> <a id="18495" class="Keyword">import</a> <a id="18502" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="18541" class="Keyword">open</a> <a id="18546" class="Keyword">import</a> <a id="18553" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="18593" class="Keyword">open</a> <a id="18598" class="Keyword">import</a> <a id="18605" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="18638" class="Keyword">open</a> <a id="18643" class="Keyword">import</a> <a id="18650" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="18695" class="Keyword">open</a> <a id="18700" class="Keyword">import</a> <a id="18707" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="18783" class="Keyword">open</a> <a id="18788" class="Keyword">import</a> <a id="18795" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="18857" class="Keyword">open</a> <a id="18862" class="Keyword">import</a> <a id="18869" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="18893" class="Keyword">open</a> <a id="18898" class="Keyword">import</a> <a id="18905" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="18945" class="Keyword">open</a> <a id="18950" class="Keyword">import</a> <a id="18957" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="18996" class="Keyword">open</a> <a id="19001" class="Keyword">import</a> <a id="19008" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="19056" class="Keyword">open</a> <a id="19061" class="Keyword">import</a> <a id="19068" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="19115" class="Keyword">open</a> <a id="19120" class="Keyword">import</a> <a id="19127" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="19167" class="Keyword">open</a> <a id="19172" class="Keyword">import</a> <a id="19179" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="19231" class="Keyword">open</a> <a id="19236" class="Keyword">import</a> <a id="19243" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="19301" class="Keyword">open</a> <a id="19306" class="Keyword">import</a> <a id="19313" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="19367" class="Keyword">open</a> <a id="19372" class="Keyword">import</a> <a id="19379" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="19427" class="Keyword">open</a> <a id="19432" class="Keyword">import</a> <a id="19439" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="19487" class="Keyword">open</a> <a id="19492" class="Keyword">import</a> <a id="19499" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="19538" class="Keyword">open</a> <a id="19543" class="Keyword">import</a> <a id="19550" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="19583" class="Keyword">open</a> <a id="19588" class="Keyword">import</a> <a id="19595" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="19654" class="Keyword">open</a> <a id="19659" class="Keyword">import</a> <a id="19666" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="19721" class="Keyword">open</a> <a id="19726" class="Keyword">import</a> <a id="19733" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="19776" class="Keyword">open</a> <a id="19781" class="Keyword">import</a> <a id="19788" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="19843" class="Keyword">open</a> <a id="19848" class="Keyword">import</a> <a id="19855" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="19906" class="Keyword">open</a> <a id="19911" class="Keyword">import</a> <a id="19918" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="19996" class="Keyword">open</a> <a id="20001" class="Keyword">import</a> <a id="20008" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="20048" class="Keyword">open</a> <a id="20053" class="Keyword">import</a> <a id="20060" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="20117" class="Keyword">open</a> <a id="20122" class="Keyword">import</a> <a id="20129" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="20164" class="Keyword">open</a> <a id="20169" class="Keyword">import</a> <a id="20176" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="20222" class="Keyword">open</a> <a id="20227" class="Keyword">import</a> <a id="20234" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="20289" class="Keyword">open</a> <a id="20294" class="Keyword">import</a> <a id="20301" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="20360" class="Keyword">open</a> <a id="20365" class="Keyword">import</a> <a id="20372" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="20409" class="Keyword">open</a> <a id="20414" class="Keyword">import</a> <a id="20421" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="20481" class="Keyword">open</a> <a id="20486" class="Keyword">import</a> <a id="20493" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="20531" class="Keyword">open</a> <a id="20536" class="Keyword">import</a> <a id="20543" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="20595" class="Keyword">open</a> <a id="20600" class="Keyword">import</a> <a id="20607" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="20653" class="Keyword">open</a> <a id="20658" class="Keyword">import</a> <a id="20665" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="20710" class="Keyword">open</a> <a id="20715" class="Keyword">import</a> <a id="20722" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="20759" class="Keyword">open</a> <a id="20764" class="Keyword">import</a> <a id="20771" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="20820" class="Keyword">open</a> <a id="20825" class="Keyword">import</a> <a id="20832" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="20870" class="Keyword">open</a> <a id="20875" class="Keyword">import</a> <a id="20882" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="20937" class="Keyword">open</a> <a id="20942" class="Keyword">import</a> <a id="20949" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="20988" class="Keyword">open</a> <a id="20993" class="Keyword">import</a> <a id="21000" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="21030" class="Keyword">open</a> <a id="21035" class="Keyword">import</a> <a id="21042" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="21072" class="Keyword">open</a> <a id="21077" class="Keyword">import</a> <a id="21084" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="21124" class="Keyword">open</a> <a id="21129" class="Keyword">import</a> <a id="21136" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="21181" class="Keyword">open</a> <a id="21186" class="Keyword">import</a> <a id="21193" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="21243" class="Keyword">open</a> <a id="21248" class="Keyword">import</a> <a id="21255" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="21293" class="Keyword">open</a> <a id="21298" class="Keyword">import</a> <a id="21305" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="21354" class="Keyword">open</a> <a id="21359" class="Keyword">import</a> <a id="21366" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="21429" class="Keyword">open</a> <a id="21434" class="Keyword">import</a> <a id="21441" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="21494" class="Keyword">open</a> <a id="21499" class="Keyword">import</a> <a id="21506" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="21552" class="Keyword">open</a> <a id="21557" class="Keyword">import</a> <a id="21564" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="21610" class="Keyword">open</a> <a id="21615" class="Keyword">import</a> <a id="21622" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="21670" class="Keyword">open</a> <a id="21675" class="Keyword">import</a> <a id="21682" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="21760" class="Keyword">open</a> <a id="21765" class="Keyword">import</a> <a id="21772" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="21840" class="Keyword">open</a> <a id="21845" class="Keyword">import</a> <a id="21852" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="21865" class="Keyword">open</a> <a id="21870" class="Keyword">import</a> <a id="21877" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="21897" class="Keyword">open</a> <a id="21902" class="Keyword">import</a> <a id="21909" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="21960" class="Keyword">open</a> <a id="21965" class="Keyword">import</a> <a id="21972" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="21997" class="Keyword">open</a> <a id="22002" class="Keyword">import</a> <a id="22009" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="22035" class="Keyword">open</a> <a id="22040" class="Keyword">import</a> <a id="22047" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

