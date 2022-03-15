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
<a id="4896" class="Keyword">open</a> <a id="4901" class="Keyword">import</a> <a id="4908" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="4961" class="Keyword">open</a> <a id="4966" class="Keyword">import</a> <a id="4973" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="5034" class="Keyword">open</a> <a id="5039" class="Keyword">import</a> <a id="5046" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="5104" class="Keyword">open</a> <a id="5109" class="Keyword">import</a> <a id="5116" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="5165" class="Keyword">open</a> <a id="5170" class="Keyword">import</a> <a id="5177" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="5221" class="Keyword">open</a> <a id="5226" class="Keyword">import</a> <a id="5233" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="5280" class="Keyword">open</a> <a id="5285" class="Keyword">import</a> <a id="5292" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="5352" class="Keyword">open</a> <a id="5357" class="Keyword">import</a> <a id="5364" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="5418" class="Keyword">open</a> <a id="5423" class="Keyword">import</a> <a id="5430" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="5491" class="Keyword">open</a> <a id="5496" class="Keyword">import</a> <a id="5503" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="5566" class="Keyword">open</a> <a id="5571" class="Keyword">import</a> <a id="5578" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="5643" class="Keyword">open</a> <a id="5648" class="Keyword">import</a> <a id="5655" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="5763" class="Keyword">open</a> <a id="5768" class="Keyword">import</a> <a id="5775" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="5795" class="Keyword">open</a> <a id="5800" class="Keyword">import</a> <a id="5807" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="5853" class="Keyword">open</a> <a id="5858" class="Keyword">import</a> <a id="5865" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="5911" class="Keyword">open</a> <a id="5916" class="Keyword">import</a> <a id="5923" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="5957" class="Keyword">open</a> <a id="5962" class="Keyword">import</a> <a id="5969" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="6009" class="Keyword">open</a> <a id="6014" class="Keyword">import</a> <a id="6021" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="6084" class="Keyword">open</a> <a id="6089" class="Keyword">import</a> <a id="6096" href="foundation.html" class="Module">foundation</a>
<a id="6107" class="Keyword">open</a> <a id="6112" class="Keyword">import</a> <a id="6119" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="6137" class="Keyword">open</a> <a id="6142" class="Keyword">import</a> <a id="6149" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="6168" class="Keyword">open</a> <a id="6173" class="Keyword">import</a> <a id="6180" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="6199" class="Keyword">open</a> <a id="6204" class="Keyword">import</a> <a id="6211" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="6255" class="Keyword">open</a> <a id="6260" class="Keyword">import</a> <a id="6267" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="6292" class="Keyword">open</a> <a id="6297" class="Keyword">import</a> <a id="6304" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="6331" class="Keyword">open</a> <a id="6336" class="Keyword">import</a> <a id="6343" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="6372" class="Keyword">open</a> <a id="6377" class="Keyword">import</a> <a id="6384" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="6415" class="Keyword">open</a> <a id="6420" class="Keyword">import</a> <a id="6427" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="6455" class="Keyword">open</a> <a id="6460" class="Keyword">import</a> <a id="6467" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="6497" class="Keyword">open</a> <a id="6502" class="Keyword">import</a> <a id="6509" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="6529" class="Keyword">open</a> <a id="6534" class="Keyword">import</a> <a id="6541" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="6578" class="Keyword">open</a> <a id="6583" class="Keyword">import</a> <a id="6590" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="6625" class="Keyword">open</a> <a id="6630" class="Keyword">import</a> <a id="6637" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="6695" class="Keyword">open</a> <a id="6700" class="Keyword">import</a> <a id="6707" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="6745" class="Keyword">open</a> <a id="6750" class="Keyword">import</a> <a id="6757" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="6786" class="Keyword">open</a> <a id="6791" class="Keyword">import</a> <a id="6798" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="6821" class="Keyword">open</a> <a id="6826" class="Keyword">import</a> <a id="6833" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="6856" class="Keyword">open</a> <a id="6861" class="Keyword">import</a> <a id="6868" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="6910" class="Keyword">open</a> <a id="6915" class="Keyword">import</a> <a id="6922" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="6954" class="Keyword">open</a> <a id="6959" class="Keyword">import</a> <a id="6966" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="6993" class="Keyword">open</a> <a id="6998" class="Keyword">import</a> <a id="7005" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="7030" class="Keyword">open</a> <a id="7035" class="Keyword">import</a> <a id="7042" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="7071" class="Keyword">open</a> <a id="7076" class="Keyword">import</a> <a id="7083" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="7113" class="Keyword">open</a> <a id="7118" class="Keyword">import</a> <a id="7125" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="7152" class="Keyword">open</a> <a id="7157" class="Keyword">import</a> <a id="7164" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="7183" class="Keyword">open</a> <a id="7188" class="Keyword">import</a> <a id="7195" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="7241" class="Keyword">open</a> <a id="7246" class="Keyword">import</a> <a id="7253" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="7295" class="Keyword">open</a> <a id="7300" class="Keyword">import</a> <a id="7307" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="7339" class="Keyword">open</a> <a id="7344" class="Keyword">import</a> <a id="7351" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="7381" class="Keyword">open</a> <a id="7386" class="Keyword">import</a> <a id="7393" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="7419" class="Keyword">open</a> <a id="7424" class="Keyword">import</a> <a id="7431" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="7465" class="Keyword">open</a> <a id="7470" class="Keyword">import</a> <a id="7477" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="7507" class="Keyword">open</a> <a id="7512" class="Keyword">import</a> <a id="7519" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="7546" class="Keyword">open</a> <a id="7551" class="Keyword">import</a> <a id="7558" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="7590" class="Keyword">open</a> <a id="7595" class="Keyword">import</a> <a id="7602" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="7636" class="Keyword">open</a> <a id="7641" class="Keyword">import</a> <a id="7648" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="7671" class="Keyword">open</a> <a id="7676" class="Keyword">import</a> <a id="7683" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="7753" class="Keyword">open</a> <a id="7758" class="Keyword">import</a> <a id="7765" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="7835" class="Keyword">open</a> <a id="7840" class="Keyword">import</a> <a id="7847" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="7874" class="Keyword">open</a> <a id="7879" class="Keyword">import</a> <a id="7886" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="7934" class="Keyword">open</a> <a id="7939" class="Keyword">import</a> <a id="7946" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="7986" class="Keyword">open</a> <a id="7991" class="Keyword">import</a> <a id="7998" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="8020" class="Keyword">open</a> <a id="8025" class="Keyword">import</a> <a id="8032" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="8055" class="Keyword">open</a> <a id="8060" class="Keyword">import</a> <a id="8067" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="8112" class="Keyword">open</a> <a id="8117" class="Keyword">import</a> <a id="8124" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="8168" class="Keyword">open</a> <a id="8173" class="Keyword">import</a> <a id="8180" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="8216" class="Keyword">open</a> <a id="8221" class="Keyword">import</a> <a id="8228" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="8273" class="Keyword">open</a> <a id="8278" class="Keyword">import</a> <a id="8285" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="8326" class="Keyword">open</a> <a id="8331" class="Keyword">import</a> <a id="8338" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="8373" class="Keyword">open</a> <a id="8378" class="Keyword">import</a> <a id="8385" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="8416" class="Keyword">open</a> <a id="8421" class="Keyword">import</a> <a id="8428" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="8461" class="Keyword">open</a> <a id="8466" class="Keyword">import</a> <a id="8473" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="8506" class="Keyword">open</a> <a id="8511" class="Keyword">import</a> <a id="8518" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="8548" class="Keyword">open</a> <a id="8553" class="Keyword">import</a> <a id="8560" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="8584" class="Keyword">open</a> <a id="8589" class="Keyword">import</a> <a id="8596" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="8634" class="Keyword">open</a> <a id="8639" class="Keyword">import</a> <a id="8646" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="8677" class="Keyword">open</a> <a id="8682" class="Keyword">import</a> <a id="8689" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="8714" class="Keyword">open</a> <a id="8719" class="Keyword">import</a> <a id="8726" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="8754" class="Keyword">open</a> <a id="8759" class="Keyword">import</a> <a id="8766" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="8790" class="Keyword">open</a> <a id="8795" class="Keyword">import</a> <a id="8802" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="8828" class="Keyword">open</a> <a id="8833" class="Keyword">import</a> <a id="8840" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="8875" class="Keyword">open</a> <a id="8880" class="Keyword">import</a> <a id="8887" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="8908" class="Keyword">open</a> <a id="8913" class="Keyword">import</a> <a id="8920" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="8969" class="Keyword">open</a> <a id="8974" class="Keyword">import</a> <a id="8981" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="9022" class="Keyword">open</a> <a id="9027" class="Keyword">import</a> <a id="9034" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="9084" class="Keyword">open</a> <a id="9089" class="Keyword">import</a> <a id="9096" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="9142" class="Keyword">open</a> <a id="9147" class="Keyword">import</a> <a id="9154" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="9194" class="Keyword">open</a> <a id="9199" class="Keyword">import</a> <a id="9206" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="9256" class="Keyword">open</a> <a id="9261" class="Keyword">import</a> <a id="9268" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="9307" class="Keyword">open</a> <a id="9312" class="Keyword">import</a> <a id="9319" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="9359" class="Keyword">open</a> <a id="9364" class="Keyword">import</a> <a id="9371" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="9404" class="Keyword">open</a> <a id="9409" class="Keyword">import</a> <a id="9416" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="9465" class="Keyword">open</a> <a id="9470" class="Keyword">import</a> <a id="9477" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="9502" class="Keyword">open</a> <a id="9507" class="Keyword">import</a> <a id="9514" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="9536" class="Keyword">open</a> <a id="9541" class="Keyword">import</a> <a id="9548" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="9576" class="Keyword">open</a> <a id="9581" class="Keyword">import</a> <a id="9588" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="9614" class="Keyword">open</a> <a id="9619" class="Keyword">import</a> <a id="9626" href="foundation.images.html" class="Module">foundation.images</a>
<a id="9644" class="Keyword">open</a> <a id="9649" class="Keyword">import</a> <a id="9656" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="9691" class="Keyword">open</a> <a id="9696" class="Keyword">import</a> <a id="9703" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="9730" class="Keyword">open</a> <a id="9735" class="Keyword">import</a> <a id="9742" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="9798" class="Keyword">open</a> <a id="9803" class="Keyword">import</a> <a id="9810" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="9839" class="Keyword">open</a> <a id="9844" class="Keyword">import</a> <a id="9851" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="9881" class="Keyword">open</a> <a id="9886" class="Keyword">import</a> <a id="9893" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="9919" class="Keyword">open</a> <a id="9924" class="Keyword">import</a> <a id="9931" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="9958" class="Keyword">open</a> <a id="9963" class="Keyword">import</a> <a id="9970" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="9993" class="Keyword">open</a> <a id="9998" class="Keyword">import</a> <a id="10005" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="10032" class="Keyword">open</a> <a id="10037" class="Keyword">import</a> <a id="10044" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="10076" class="Keyword">open</a> <a id="10081" class="Keyword">import</a> <a id="10088" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="10122" class="Keyword">open</a> <a id="10127" class="Keyword">import</a> <a id="10134" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="10174" class="Keyword">open</a> <a id="10179" class="Keyword">import</a> <a id="10186" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="10217" class="Keyword">open</a> <a id="10222" class="Keyword">import</a> <a id="10229" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="10261" class="Keyword">open</a> <a id="10266" class="Keyword">import</a> <a id="10273" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="10290" class="Keyword">open</a> <a id="10295" class="Keyword">import</a> <a id="10302" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="10327" class="Keyword">open</a> <a id="10332" class="Keyword">import</a> <a id="10339" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="10368" class="Keyword">open</a> <a id="10373" class="Keyword">import</a> <a id="10380" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="10405" class="Keyword">open</a> <a id="10410" class="Keyword">import</a> <a id="10417" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="10438" class="Keyword">open</a> <a id="10443" class="Keyword">import</a> <a id="10450" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="10470" class="Keyword">open</a> <a id="10475" class="Keyword">import</a> <a id="10482" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="10516" class="Keyword">open</a> <a id="10521" class="Keyword">import</a> <a id="10528" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="10552" class="Keyword">open</a> <a id="10557" class="Keyword">import</a> <a id="10564" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="10591" class="Keyword">open</a> <a id="10596" class="Keyword">import</a> <a id="10603" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="10638" class="Keyword">open</a> <a id="10643" class="Keyword">import</a> <a id="10650" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="10690" class="Keyword">open</a> <a id="10695" class="Keyword">import</a> <a id="10702" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="10732" class="Keyword">open</a> <a id="10737" class="Keyword">import</a> <a id="10744" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="10781" class="Keyword">open</a> <a id="10786" class="Keyword">import</a> <a id="10793" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="10817" class="Keyword">open</a> <a id="10822" class="Keyword">import</a> <a id="10829" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="10850" class="Keyword">open</a> <a id="10855" class="Keyword">import</a> <a id="10862" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="10897" class="Keyword">open</a> <a id="10902" class="Keyword">import</a> <a id="10909" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="10946" class="Keyword">open</a> <a id="10951" class="Keyword">import</a> <a id="10958" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="11007" class="Keyword">open</a> <a id="11012" class="Keyword">import</a> <a id="11019" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="11042" class="Keyword">open</a> <a id="11047" class="Keyword">import</a> <a id="11054" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="11077" class="Keyword">open</a> <a id="11082" class="Keyword">import</a> <a id="11089" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="11117" class="Keyword">open</a> <a id="11122" class="Keyword">import</a> <a id="11129" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="11149" class="Keyword">open</a> <a id="11154" class="Keyword">import</a> <a id="11161" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="11192" class="Keyword">open</a> <a id="11197" class="Keyword">import</a> <a id="11204" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="11231" class="Keyword">open</a> <a id="11236" class="Keyword">import</a> <a id="11243" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="11259" class="Keyword">open</a> <a id="11264" class="Keyword">import</a> <a id="11271" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="11302" class="Keyword">open</a> <a id="11307" class="Keyword">import</a> <a id="11314" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="11331" class="Keyword">open</a> <a id="11336" class="Keyword">import</a> <a id="11343" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="11365" class="Keyword">open</a> <a id="11370" class="Keyword">import</a> <a id="11377" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="11404" class="Keyword">open</a> <a id="11409" class="Keyword">import</a> <a id="11416" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="11439" class="Keyword">open</a> <a id="11444" class="Keyword">import</a> <a id="11451" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="11478" class="Keyword">open</a> <a id="11483" class="Keyword">import</a> <a id="11490" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="11523" class="Keyword">open</a> <a id="11528" class="Keyword">import</a> <a id="11535" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="11575" class="Keyword">open</a> <a id="11580" class="Keyword">import</a> <a id="11587" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="11608" class="Keyword">open</a> <a id="11613" class="Keyword">import</a> <a id="11620" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="11649" class="Keyword">open</a> <a id="11654" class="Keyword">import</a> <a id="11661" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="11699" class="Keyword">open</a> <a id="11704" class="Keyword">import</a> <a id="11711" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="11731" class="Keyword">open</a> <a id="11736" class="Keyword">import</a> <a id="11743" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="11767" class="Keyword">open</a> <a id="11772" class="Keyword">import</a> <a id="11779" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="11806" class="Keyword">open</a> <a id="11811" class="Keyword">import</a> <a id="11818" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="11848" class="Keyword">open</a> <a id="11853" class="Keyword">import</a> <a id="11860" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="11886" class="Keyword">open</a> <a id="11891" class="Keyword">import</a> <a id="11898" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="11925" class="Keyword">open</a> <a id="11930" class="Keyword">import</a> <a id="11937" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="11966" class="Keyword">open</a> <a id="11971" class="Keyword">import</a> <a id="11978" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="12001" class="Keyword">open</a> <a id="12006" class="Keyword">import</a> <a id="12013" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="12064" class="Keyword">open</a> <a id="12069" class="Keyword">import</a> <a id="12076" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="12119" class="Keyword">open</a> <a id="12124" class="Keyword">import</a> <a id="12131" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="12179" class="Keyword">open</a> <a id="12184" class="Keyword">import</a> <a id="12191" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="12229" class="Keyword">open</a> <a id="12234" class="Keyword">import</a> <a id="12241" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="12278" class="Keyword">open</a> <a id="12283" class="Keyword">import</a> <a id="12290" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="12318" class="Keyword">open</a> <a id="12323" class="Keyword">import</a> <a id="12330" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="12366" class="Keyword">open</a> <a id="12371" class="Keyword">import</a> <a id="12378" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="12416" class="Keyword">open</a> <a id="12421" class="Keyword">import</a> <a id="12428" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="12461" class="Keyword">open</a> <a id="12466" class="Keyword">import</a> <a id="12473" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="12494" class="Keyword">open</a> <a id="12499" class="Keyword">import</a> <a id="12506" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="12560" class="Keyword">open</a> <a id="12565" class="Keyword">import</a> <a id="12572" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="12594" class="Keyword">open</a> <a id="12599" class="Keyword">import</a> <a id="12606" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="12641" class="Keyword">open</a> <a id="12646" class="Keyword">import</a> <a id="12653" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="12683" class="Keyword">open</a> <a id="12688" class="Keyword">import</a> <a id="12695" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="12734" class="Keyword">open</a> <a id="12739" class="Keyword">import</a> <a id="12746" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="12800" class="Keyword">open</a> <a id="12805" class="Keyword">import</a> <a id="12812" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="12858" class="Keyword">open</a> <a id="12863" class="Keyword">import</a> <a id="12870" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="12921" class="Keyword">open</a> <a id="12926" class="Keyword">import</a> <a id="12933" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="12974" class="Keyword">open</a> <a id="12979" class="Keyword">import</a> <a id="12986" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="13031" class="Keyword">open</a> <a id="13036" class="Keyword">import</a> <a id="13043" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="13088" class="Keyword">open</a> <a id="13093" class="Keyword">import</a> <a id="13100" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="13136" class="Keyword">open</a> <a id="13141" class="Keyword">import</a> <a id="13148" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="13184" class="Keyword">open</a> <a id="13189" class="Keyword">import</a> <a id="13196" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="13261" class="Keyword">open</a> <a id="13266" class="Keyword">import</a> <a id="13273" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="13328" class="Keyword">open</a> <a id="13333" class="Keyword">import</a> <a id="13340" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="13380" class="Keyword">open</a> <a id="13385" class="Keyword">import</a> <a id="13392" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="13436" class="Keyword">open</a> <a id="13441" class="Keyword">import</a> <a id="13448" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="13493" class="Keyword">open</a> <a id="13498" class="Keyword">import</a> <a id="13505" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="13546" class="Keyword">open</a> <a id="13551" class="Keyword">import</a> <a id="13558" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="13598" class="Keyword">open</a> <a id="13603" class="Keyword">import</a> <a id="13610" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="13637" class="Keyword">open</a> <a id="13642" class="Keyword">import</a> <a id="13649" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="13676" class="Keyword">open</a> <a id="13681" class="Keyword">import</a> <a id="13688" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="13707" class="Keyword">open</a> <a id="13712" class="Keyword">import</a> <a id="13719" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="13759" class="Keyword">open</a> <a id="13764" class="Keyword">import</a> <a id="13771" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="13836" class="Keyword">open</a> <a id="13841" class="Keyword">import</a> <a id="13848" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="13871" class="Keyword">open</a> <a id="13876" class="Keyword">import</a> <a id="13883" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="13907" class="Keyword">open</a> <a id="13912" class="Keyword">import</a> <a id="13919" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="13959" class="Keyword">open</a> <a id="13964" class="Keyword">import</a> <a id="13971" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="14014" class="Keyword">open</a> <a id="14019" class="Keyword">import</a> <a id="14026" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="14060" class="Keyword">open</a> <a id="14065" class="Keyword">import</a> <a id="14072" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="14102" class="Keyword">open</a> <a id="14107" class="Keyword">import</a> <a id="14114" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="14148" class="Keyword">open</a> <a id="14153" class="Keyword">import</a> <a id="14160" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="14195" class="Keyword">open</a> <a id="14200" class="Keyword">import</a> <a id="14207" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="14244" class="Keyword">open</a> <a id="14249" class="Keyword">import</a> <a id="14256" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="14283" class="Keyword">open</a> <a id="14288" class="Keyword">import</a> <a id="14295" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="14323" class="Keyword">open</a> <a id="14328" class="Keyword">import</a> <a id="14335" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="14384" class="Keyword">open</a> <a id="14389" class="Keyword">import</a> <a id="14396" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="14442" class="Keyword">open</a> <a id="14447" class="Keyword">import</a> <a id="14454" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="14494" class="Keyword">open</a> <a id="14499" class="Keyword">import</a> <a id="14506" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="14544" class="Keyword">open</a> <a id="14549" class="Keyword">import</a> <a id="14556" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="14585" class="Keyword">open</a> <a id="14590" class="Keyword">import</a> <a id="14597" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="14627" class="Keyword">open</a> <a id="14632" class="Keyword">import</a> <a id="14639" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="14670" class="Keyword">open</a> <a id="14675" class="Keyword">import</a> <a id="14682" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="14708" class="Keyword">open</a> <a id="14713" class="Keyword">import</a> <a id="14720" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="14771" class="Keyword">open</a> <a id="14776" class="Keyword">import</a> <a id="14783" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="14837" class="Keyword">open</a> <a id="14842" class="Keyword">import</a> <a id="14849" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="14876" class="Keyword">open</a> <a id="14881" class="Keyword">import</a> <a id="14888" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="14921" class="Keyword">open</a> <a id="14926" class="Keyword">import</a> <a id="14933" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="14964" class="Keyword">open</a> <a id="14969" class="Keyword">import</a> <a id="14976" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="15013" class="Keyword">open</a> <a id="15018" class="Keyword">import</a> <a id="15025" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="15050" class="Keyword">open</a> <a id="15055" class="Keyword">import</a> <a id="15062" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="15094" class="Keyword">open</a> <a id="15099" class="Keyword">import</a> <a id="15106" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="15141" class="Keyword">open</a> <a id="15146" class="Keyword">import</a> <a id="15153" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="15182" class="Keyword">open</a> <a id="15187" class="Keyword">import</a> <a id="15194" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="15222" class="Keyword">open</a> <a id="15227" class="Keyword">import</a> <a id="15234" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="15259" class="Keyword">open</a> <a id="15264" class="Keyword">import</a> <a id="15271" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="15292" class="Keyword">open</a> <a id="15297" class="Keyword">import</a> <a id="15304" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="15340" class="Keyword">open</a> <a id="15345" class="Keyword">import</a> <a id="15352" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="15395" class="Keyword">open</a> <a id="15400" class="Keyword">import</a> <a id="15407" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="15432" class="Keyword">open</a> <a id="15437" class="Keyword">import</a> <a id="15444" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="15475" class="Keyword">open</a> <a id="15480" class="Keyword">import</a> <a id="15487" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="15519" class="Keyword">open</a> <a id="15524" class="Keyword">import</a> <a id="15531" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="15565" class="Keyword">open</a> <a id="15570" class="Keyword">import</a> <a id="15577" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="15633" class="Keyword">open</a> <a id="15638" class="Keyword">import</a> <a id="15645" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="15698" class="Keyword">open</a> <a id="15703" class="Keyword">import</a> <a id="15710" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="15737" class="Keyword">open</a> <a id="15742" class="Keyword">import</a> <a id="15749" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="15811" class="Keyword">open</a> <a id="15816" class="Keyword">import</a> <a id="15823" href="graph-theory.html" class="Module">graph-theory</a>
<a id="15836" class="Keyword">open</a> <a id="15841" class="Keyword">import</a> <a id="15848" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="15877" class="Keyword">open</a> <a id="15882" class="Keyword">import</a> <a id="15889" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="15916" class="Keyword">open</a> <a id="15921" class="Keyword">import</a> <a id="15928" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="15950" class="Keyword">open</a> <a id="15955" class="Keyword">import</a> <a id="15962" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="15992" class="Keyword">open</a> <a id="15997" class="Keyword">import</a> <a id="16004" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="16065" class="Keyword">open</a> <a id="16070" class="Keyword">import</a> <a id="16077" href="group-theory.html" class="Module">group-theory</a>
<a id="16090" class="Keyword">open</a> <a id="16095" class="Keyword">import</a> <a id="16102" href="group-theory.abstract-abelian-groups.html" class="Module">group-theory.abstract-abelian-groups</a>
<a id="16139" class="Keyword">open</a> <a id="16144" class="Keyword">import</a> <a id="16151" href="group-theory.abstract-abelian-subgroups.html" class="Module">group-theory.abstract-abelian-subgroups</a>
<a id="16191" class="Keyword">open</a> <a id="16196" class="Keyword">import</a> <a id="16203" href="group-theory.abstract-group-actions.html" class="Module">group-theory.abstract-group-actions</a>
<a id="16239" class="Keyword">open</a> <a id="16244" class="Keyword">import</a> <a id="16251" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="16287" class="Keyword">open</a> <a id="16292" class="Keyword">import</a> <a id="16299" href="group-theory.abstract-groups.html" class="Module">group-theory.abstract-groups</a>
<a id="16328" class="Keyword">open</a> <a id="16333" class="Keyword">import</a> <a id="16340" href="group-theory.abstract-subgroups.html" class="Module">group-theory.abstract-subgroups</a>
<a id="16372" class="Keyword">open</a> <a id="16377" class="Keyword">import</a> <a id="16384" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="16420" class="Keyword">open</a> <a id="16425" class="Keyword">import</a> <a id="16432" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="16461" class="Keyword">open</a> <a id="16466" class="Keyword">import</a> <a id="16473" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="16505" class="Keyword">open</a> <a id="16510" class="Keyword">import</a> <a id="16517" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="16553" class="Keyword">open</a> <a id="16558" class="Keyword">import</a> <a id="16565" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="16597" class="Keyword">open</a> <a id="16602" class="Keyword">import</a> <a id="16609" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="16636" class="Keyword">open</a> <a id="16641" class="Keyword">import</a> <a id="16648" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="16705" class="Keyword">open</a> <a id="16710" class="Keyword">import</a> <a id="16717" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="16732" class="Keyword">open</a> <a id="16737" class="Keyword">import</a> <a id="16744" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="16768" class="Keyword">open</a> <a id="16773" class="Keyword">import</a> <a id="16780" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="16833" class="Keyword">open</a> <a id="16838" class="Keyword">import</a> <a id="16845" href="order-theory.html" class="Module">order-theory</a>
<a id="16858" class="Keyword">open</a> <a id="16863" class="Keyword">import</a> <a id="16870" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="16897" class="Keyword">open</a> <a id="16902" class="Keyword">import</a> <a id="16909" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="16939" class="Keyword">open</a> <a id="16944" class="Keyword">import</a> <a id="16951" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="16987" class="Keyword">open</a> <a id="16992" class="Keyword">import</a> <a id="16999" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="17032" class="Keyword">open</a> <a id="17037" class="Keyword">import</a> <a id="17044" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="17064" class="Keyword">open</a> <a id="17069" class="Keyword">import</a> <a id="17076" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="17126" class="Keyword">open</a> <a id="17131" class="Keyword">import</a> <a id="17138" href="polytopes.html" class="Module">polytopes</a>
<a id="17148" class="Keyword">open</a> <a id="17153" class="Keyword">import</a> <a id="17160" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="17218" class="Keyword">open</a> <a id="17223" class="Keyword">import</a> <a id="17230" href="ring-theory.html" class="Module">ring-theory</a>
<a id="17242" class="Keyword">open</a> <a id="17247" class="Keyword">import</a> <a id="17254" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="17286" class="Keyword">open</a> <a id="17291" class="Keyword">import</a> <a id="17298" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="17328" class="Keyword">open</a> <a id="17333" class="Keyword">import</a> <a id="17340" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a>
<a id="17359" class="Keyword">open</a> <a id="17364" class="Keyword">import</a> <a id="17371" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="17403" class="Keyword">open</a> <a id="17408" class="Keyword">import</a> <a id="17415" href="ring-theory.rings-with-properties.html" class="Module">ring-theory.rings-with-properties</a>
<a id="17449" class="Keyword">open</a> <a id="17454" class="Keyword">import</a> <a id="17461" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="17522" class="Keyword">open</a> <a id="17527" class="Keyword">import</a> <a id="17534" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="17560" class="Keyword">open</a> <a id="17565" class="Keyword">import</a> <a id="17572" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="17611" class="Keyword">open</a> <a id="17616" class="Keyword">import</a> <a id="17623" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="17661" class="Keyword">open</a> <a id="17666" class="Keyword">import</a> <a id="17673" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="17719" class="Keyword">open</a> <a id="17724" class="Keyword">import</a> <a id="17731" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="17768" class="Keyword">open</a> <a id="17773" class="Keyword">import</a> <a id="17780" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="17820" class="Keyword">open</a> <a id="17825" class="Keyword">import</a> <a id="17832" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="17871" class="Keyword">open</a> <a id="17876" class="Keyword">import</a> <a id="17883" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="17916" class="Keyword">open</a> <a id="17921" class="Keyword">import</a> <a id="17928" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="17967" class="Keyword">open</a> <a id="17972" class="Keyword">import</a> <a id="17979" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="18024" class="Keyword">open</a> <a id="18029" class="Keyword">import</a> <a id="18036" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="18088" class="Keyword">open</a> <a id="18093" class="Keyword">import</a> <a id="18100" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="18148" class="Keyword">open</a> <a id="18153" class="Keyword">import</a> <a id="18160" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="18200" class="Keyword">open</a> <a id="18205" class="Keyword">import</a> <a id="18212" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="18259" class="Keyword">open</a> <a id="18264" class="Keyword">import</a> <a id="18271" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="18309" class="Keyword">open</a> <a id="18314" class="Keyword">import</a> <a id="18321" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="18375" class="Keyword">open</a> <a id="18380" class="Keyword">import</a> <a id="18387" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="18434" class="Keyword">open</a> <a id="18439" class="Keyword">import</a> <a id="18446" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="18498" class="Keyword">open</a> <a id="18503" class="Keyword">import</a> <a id="18510" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="18555" class="Keyword">open</a> <a id="18560" class="Keyword">import</a> <a id="18567" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="18606" class="Keyword">open</a> <a id="18611" class="Keyword">import</a> <a id="18618" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="18658" class="Keyword">open</a> <a id="18663" class="Keyword">import</a> <a id="18670" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="18703" class="Keyword">open</a> <a id="18708" class="Keyword">import</a> <a id="18715" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="18760" class="Keyword">open</a> <a id="18765" class="Keyword">import</a> <a id="18772" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="18848" class="Keyword">open</a> <a id="18853" class="Keyword">import</a> <a id="18860" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="18922" class="Keyword">open</a> <a id="18927" class="Keyword">import</a> <a id="18934" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="18958" class="Keyword">open</a> <a id="18963" class="Keyword">import</a> <a id="18970" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="19010" class="Keyword">open</a> <a id="19015" class="Keyword">import</a> <a id="19022" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="19061" class="Keyword">open</a> <a id="19066" class="Keyword">import</a> <a id="19073" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="19121" class="Keyword">open</a> <a id="19126" class="Keyword">import</a> <a id="19133" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="19180" class="Keyword">open</a> <a id="19185" class="Keyword">import</a> <a id="19192" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="19232" class="Keyword">open</a> <a id="19237" class="Keyword">import</a> <a id="19244" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="19296" class="Keyword">open</a> <a id="19301" class="Keyword">import</a> <a id="19308" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="19366" class="Keyword">open</a> <a id="19371" class="Keyword">import</a> <a id="19378" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="19432" class="Keyword">open</a> <a id="19437" class="Keyword">import</a> <a id="19444" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="19492" class="Keyword">open</a> <a id="19497" class="Keyword">import</a> <a id="19504" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="19552" class="Keyword">open</a> <a id="19557" class="Keyword">import</a> <a id="19564" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="19603" class="Keyword">open</a> <a id="19608" class="Keyword">import</a> <a id="19615" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="19648" class="Keyword">open</a> <a id="19653" class="Keyword">import</a> <a id="19660" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="19719" class="Keyword">open</a> <a id="19724" class="Keyword">import</a> <a id="19731" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="19786" class="Keyword">open</a> <a id="19791" class="Keyword">import</a> <a id="19798" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="19841" class="Keyword">open</a> <a id="19846" class="Keyword">import</a> <a id="19853" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="19908" class="Keyword">open</a> <a id="19913" class="Keyword">import</a> <a id="19920" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="19971" class="Keyword">open</a> <a id="19976" class="Keyword">import</a> <a id="19983" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="20061" class="Keyword">open</a> <a id="20066" class="Keyword">import</a> <a id="20073" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="20113" class="Keyword">open</a> <a id="20118" class="Keyword">import</a> <a id="20125" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="20182" class="Keyword">open</a> <a id="20187" class="Keyword">import</a> <a id="20194" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="20229" class="Keyword">open</a> <a id="20234" class="Keyword">import</a> <a id="20241" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="20287" class="Keyword">open</a> <a id="20292" class="Keyword">import</a> <a id="20299" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="20354" class="Keyword">open</a> <a id="20359" class="Keyword">import</a> <a id="20366" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="20425" class="Keyword">open</a> <a id="20430" class="Keyword">import</a> <a id="20437" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="20474" class="Keyword">open</a> <a id="20479" class="Keyword">import</a> <a id="20486" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="20546" class="Keyword">open</a> <a id="20551" class="Keyword">import</a> <a id="20558" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="20596" class="Keyword">open</a> <a id="20601" class="Keyword">import</a> <a id="20608" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="20660" class="Keyword">open</a> <a id="20665" class="Keyword">import</a> <a id="20672" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="20718" class="Keyword">open</a> <a id="20723" class="Keyword">import</a> <a id="20730" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="20775" class="Keyword">open</a> <a id="20780" class="Keyword">import</a> <a id="20787" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="20824" class="Keyword">open</a> <a id="20829" class="Keyword">import</a> <a id="20836" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="20885" class="Keyword">open</a> <a id="20890" class="Keyword">import</a> <a id="20897" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="20935" class="Keyword">open</a> <a id="20940" class="Keyword">import</a> <a id="20947" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="21002" class="Keyword">open</a> <a id="21007" class="Keyword">import</a> <a id="21014" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="21053" class="Keyword">open</a> <a id="21058" class="Keyword">import</a> <a id="21065" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="21095" class="Keyword">open</a> <a id="21100" class="Keyword">import</a> <a id="21107" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="21137" class="Keyword">open</a> <a id="21142" class="Keyword">import</a> <a id="21149" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="21189" class="Keyword">open</a> <a id="21194" class="Keyword">import</a> <a id="21201" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="21246" class="Keyword">open</a> <a id="21251" class="Keyword">import</a> <a id="21258" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="21308" class="Keyword">open</a> <a id="21313" class="Keyword">import</a> <a id="21320" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="21358" class="Keyword">open</a> <a id="21363" class="Keyword">import</a> <a id="21370" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="21419" class="Keyword">open</a> <a id="21424" class="Keyword">import</a> <a id="21431" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="21494" class="Keyword">open</a> <a id="21499" class="Keyword">import</a> <a id="21506" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="21559" class="Keyword">open</a> <a id="21564" class="Keyword">import</a> <a id="21571" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="21617" class="Keyword">open</a> <a id="21622" class="Keyword">import</a> <a id="21629" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="21675" class="Keyword">open</a> <a id="21680" class="Keyword">import</a> <a id="21687" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="21735" class="Keyword">open</a> <a id="21740" class="Keyword">import</a> <a id="21747" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="21825" class="Keyword">open</a> <a id="21830" class="Keyword">import</a> <a id="21837" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="21905" class="Keyword">open</a> <a id="21910" class="Keyword">import</a> <a id="21917" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="21930" class="Keyword">open</a> <a id="21935" class="Keyword">import</a> <a id="21942" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="21962" class="Keyword">open</a> <a id="21967" class="Keyword">import</a> <a id="21974" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="22025" class="Keyword">open</a> <a id="22030" class="Keyword">import</a> <a id="22037" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="22062" class="Keyword">open</a> <a id="22067" class="Keyword">import</a> <a id="22074" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="22100" class="Keyword">open</a> <a id="22105" class="Keyword">import</a> <a id="22112" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

