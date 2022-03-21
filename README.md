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
<a id="2004" class="Keyword">open</a> <a id="2009" class="Keyword">import</a> <a id="2016" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="2057" class="Keyword">open</a> <a id="2062" class="Keyword">import</a> <a id="2069" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="2112" class="Keyword">open</a> <a id="2117" class="Keyword">import</a> <a id="2124" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="2168" class="Keyword">open</a> <a id="2173" class="Keyword">import</a> <a id="2180" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="2225" class="Keyword">open</a> <a id="2230" class="Keyword">import</a> <a id="2237" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="2289" class="Keyword">open</a> <a id="2294" class="Keyword">import</a> <a id="2301" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="2342" class="Keyword">open</a> <a id="2347" class="Keyword">import</a> <a id="2354" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="2399" class="Keyword">open</a> <a id="2404" class="Keyword">import</a> <a id="2411" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="2454" class="Keyword">open</a> <a id="2459" class="Keyword">import</a> <a id="2466" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="2516" class="Keyword">open</a> <a id="2521" class="Keyword">import</a> <a id="2528" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="2575" class="Keyword">open</a> <a id="2580" class="Keyword">import</a> <a id="2587" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="2644" class="Keyword">open</a> <a id="2649" class="Keyword">import</a> <a id="2656" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="2710" class="Keyword">open</a> <a id="2715" class="Keyword">import</a> <a id="2722" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="2782" class="Keyword">open</a> <a id="2787" class="Keyword">import</a> <a id="2794" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="2837" class="Keyword">open</a> <a id="2842" class="Keyword">import</a> <a id="2849" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="2899" class="Keyword">open</a> <a id="2904" class="Keyword">import</a> <a id="2911" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="2971" class="Keyword">open</a> <a id="2976" class="Keyword">import</a> <a id="2983" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="3032" class="Keyword">open</a> <a id="3037" class="Keyword">import</a> <a id="3044" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="3100" class="Keyword">open</a> <a id="3105" class="Keyword">import</a> <a id="3112" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="3148" class="Keyword">open</a> <a id="3153" class="Keyword">import</a> <a id="3160" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="3204" class="Keyword">open</a> <a id="3209" class="Keyword">import</a> <a id="3216" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="3260" class="Keyword">open</a> <a id="3265" class="Keyword">import</a> <a id="3272" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="3322" class="Keyword">open</a> <a id="3327" class="Keyword">import</a> <a id="3334" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="3380" class="Keyword">open</a> <a id="3385" class="Keyword">import</a> <a id="3392" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="3427" class="Keyword">open</a> <a id="3432" class="Keyword">import</a> <a id="3439" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="3484" class="Keyword">open</a> <a id="3489" class="Keyword">import</a> <a id="3496" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="3554" class="Keyword">open</a> <a id="3559" class="Keyword">import</a> <a id="3566" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="3631" class="Keyword">open</a> <a id="3636" class="Keyword">import</a> <a id="3643" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="3688" class="Keyword">open</a> <a id="3693" class="Keyword">import</a> <a id="3700" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="3752" class="Keyword">open</a> <a id="3757" class="Keyword">import</a> <a id="3764" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="3822" class="Keyword">open</a> <a id="3827" class="Keyword">import</a> <a id="3834" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="3880" class="Keyword">open</a> <a id="3885" class="Keyword">import</a> <a id="3892" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="3926" class="Keyword">open</a> <a id="3931" class="Keyword">import</a> <a id="3938" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="3983" class="Keyword">open</a> <a id="3988" class="Keyword">import</a> <a id="3995" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="4049" class="Keyword">open</a> <a id="4054" class="Keyword">import</a> <a id="4061" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="4102" class="Keyword">open</a> <a id="4107" class="Keyword">import</a> <a id="4114" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="4180" class="Keyword">open</a> <a id="4185" class="Keyword">import</a> <a id="4192" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="4236" class="Keyword">open</a> <a id="4241" class="Keyword">import</a> <a id="4248" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="4297" class="Keyword">open</a> <a id="4302" class="Keyword">import</a> <a id="4309" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="4365" class="Keyword">open</a> <a id="4370" class="Keyword">import</a> <a id="4377" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="4418" class="Keyword">open</a> <a id="4423" class="Keyword">import</a> <a id="4430" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="4489" class="Keyword">open</a> <a id="4494" class="Keyword">import</a> <a id="4501" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="4540" class="Keyword">open</a> <a id="4545" class="Keyword">import</a> <a id="4552" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="4605" class="Keyword">open</a> <a id="4610" class="Keyword">import</a> <a id="4617" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="4674" class="Keyword">open</a> <a id="4679" class="Keyword">import</a> <a id="4686" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="4728" class="Keyword">open</a> <a id="4733" class="Keyword">import</a> <a id="4740" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="4791" class="Keyword">open</a> <a id="4796" class="Keyword">import</a> <a id="4803" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="4861" class="Keyword">open</a> <a id="4866" class="Keyword">import</a> <a id="4873" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="4937" class="Keyword">open</a> <a id="4942" class="Keyword">import</a> <a id="4949" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="5002" class="Keyword">open</a> <a id="5007" class="Keyword">import</a> <a id="5014" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="5067" class="Keyword">open</a> <a id="5072" class="Keyword">import</a> <a id="5079" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="5140" class="Keyword">open</a> <a id="5145" class="Keyword">import</a> <a id="5152" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="5210" class="Keyword">open</a> <a id="5215" class="Keyword">import</a> <a id="5222" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="5271" class="Keyword">open</a> <a id="5276" class="Keyword">import</a> <a id="5283" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="5327" class="Keyword">open</a> <a id="5332" class="Keyword">import</a> <a id="5339" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="5386" class="Keyword">open</a> <a id="5391" class="Keyword">import</a> <a id="5398" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="5458" class="Keyword">open</a> <a id="5463" class="Keyword">import</a> <a id="5470" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="5524" class="Keyword">open</a> <a id="5529" class="Keyword">import</a> <a id="5536" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="5597" class="Keyword">open</a> <a id="5602" class="Keyword">import</a> <a id="5609" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="5672" class="Keyword">open</a> <a id="5677" class="Keyword">import</a> <a id="5684" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="5749" class="Keyword">open</a> <a id="5754" class="Keyword">import</a> <a id="5761" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="5869" class="Keyword">open</a> <a id="5874" class="Keyword">import</a> <a id="5881" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="5901" class="Keyword">open</a> <a id="5906" class="Keyword">import</a> <a id="5913" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="5959" class="Keyword">open</a> <a id="5964" class="Keyword">import</a> <a id="5971" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="6017" class="Keyword">open</a> <a id="6022" class="Keyword">import</a> <a id="6029" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="6063" class="Keyword">open</a> <a id="6068" class="Keyword">import</a> <a id="6075" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="6115" class="Keyword">open</a> <a id="6120" class="Keyword">import</a> <a id="6127" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="6190" class="Keyword">open</a> <a id="6195" class="Keyword">import</a> <a id="6202" href="foundation.html" class="Module">foundation</a>
<a id="6213" class="Keyword">open</a> <a id="6218" class="Keyword">import</a> <a id="6225" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="6243" class="Keyword">open</a> <a id="6248" class="Keyword">import</a> <a id="6255" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="6274" class="Keyword">open</a> <a id="6279" class="Keyword">import</a> <a id="6286" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="6305" class="Keyword">open</a> <a id="6310" class="Keyword">import</a> <a id="6317" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="6361" class="Keyword">open</a> <a id="6366" class="Keyword">import</a> <a id="6373" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="6398" class="Keyword">open</a> <a id="6403" class="Keyword">import</a> <a id="6410" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="6437" class="Keyword">open</a> <a id="6442" class="Keyword">import</a> <a id="6449" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="6478" class="Keyword">open</a> <a id="6483" class="Keyword">import</a> <a id="6490" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="6521" class="Keyword">open</a> <a id="6526" class="Keyword">import</a> <a id="6533" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="6561" class="Keyword">open</a> <a id="6566" class="Keyword">import</a> <a id="6573" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="6603" class="Keyword">open</a> <a id="6608" class="Keyword">import</a> <a id="6615" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="6635" class="Keyword">open</a> <a id="6640" class="Keyword">import</a> <a id="6647" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="6684" class="Keyword">open</a> <a id="6689" class="Keyword">import</a> <a id="6696" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="6731" class="Keyword">open</a> <a id="6736" class="Keyword">import</a> <a id="6743" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="6801" class="Keyword">open</a> <a id="6806" class="Keyword">import</a> <a id="6813" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="6851" class="Keyword">open</a> <a id="6856" class="Keyword">import</a> <a id="6863" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="6892" class="Keyword">open</a> <a id="6897" class="Keyword">import</a> <a id="6904" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="6927" class="Keyword">open</a> <a id="6932" class="Keyword">import</a> <a id="6939" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="6962" class="Keyword">open</a> <a id="6967" class="Keyword">import</a> <a id="6974" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="7016" class="Keyword">open</a> <a id="7021" class="Keyword">import</a> <a id="7028" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="7060" class="Keyword">open</a> <a id="7065" class="Keyword">import</a> <a id="7072" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="7099" class="Keyword">open</a> <a id="7104" class="Keyword">import</a> <a id="7111" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="7136" class="Keyword">open</a> <a id="7141" class="Keyword">import</a> <a id="7148" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="7177" class="Keyword">open</a> <a id="7182" class="Keyword">import</a> <a id="7189" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="7219" class="Keyword">open</a> <a id="7224" class="Keyword">import</a> <a id="7231" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="7258" class="Keyword">open</a> <a id="7263" class="Keyword">import</a> <a id="7270" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="7289" class="Keyword">open</a> <a id="7294" class="Keyword">import</a> <a id="7301" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="7347" class="Keyword">open</a> <a id="7352" class="Keyword">import</a> <a id="7359" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="7401" class="Keyword">open</a> <a id="7406" class="Keyword">import</a> <a id="7413" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="7445" class="Keyword">open</a> <a id="7450" class="Keyword">import</a> <a id="7457" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="7487" class="Keyword">open</a> <a id="7492" class="Keyword">import</a> <a id="7499" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="7525" class="Keyword">open</a> <a id="7530" class="Keyword">import</a> <a id="7537" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="7571" class="Keyword">open</a> <a id="7576" class="Keyword">import</a> <a id="7583" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="7613" class="Keyword">open</a> <a id="7618" class="Keyword">import</a> <a id="7625" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="7652" class="Keyword">open</a> <a id="7657" class="Keyword">import</a> <a id="7664" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="7696" class="Keyword">open</a> <a id="7701" class="Keyword">import</a> <a id="7708" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="7742" class="Keyword">open</a> <a id="7747" class="Keyword">import</a> <a id="7754" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="7777" class="Keyword">open</a> <a id="7782" class="Keyword">import</a> <a id="7789" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="7859" class="Keyword">open</a> <a id="7864" class="Keyword">import</a> <a id="7871" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="7941" class="Keyword">open</a> <a id="7946" class="Keyword">import</a> <a id="7953" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="7980" class="Keyword">open</a> <a id="7985" class="Keyword">import</a> <a id="7992" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="8040" class="Keyword">open</a> <a id="8045" class="Keyword">import</a> <a id="8052" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="8092" class="Keyword">open</a> <a id="8097" class="Keyword">import</a> <a id="8104" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="8126" class="Keyword">open</a> <a id="8131" class="Keyword">import</a> <a id="8138" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="8161" class="Keyword">open</a> <a id="8166" class="Keyword">import</a> <a id="8173" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="8218" class="Keyword">open</a> <a id="8223" class="Keyword">import</a> <a id="8230" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="8274" class="Keyword">open</a> <a id="8279" class="Keyword">import</a> <a id="8286" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="8322" class="Keyword">open</a> <a id="8327" class="Keyword">import</a> <a id="8334" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="8379" class="Keyword">open</a> <a id="8384" class="Keyword">import</a> <a id="8391" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="8432" class="Keyword">open</a> <a id="8437" class="Keyword">import</a> <a id="8444" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="8479" class="Keyword">open</a> <a id="8484" class="Keyword">import</a> <a id="8491" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="8522" class="Keyword">open</a> <a id="8527" class="Keyword">import</a> <a id="8534" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="8567" class="Keyword">open</a> <a id="8572" class="Keyword">import</a> <a id="8579" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="8612" class="Keyword">open</a> <a id="8617" class="Keyword">import</a> <a id="8624" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="8654" class="Keyword">open</a> <a id="8659" class="Keyword">import</a> <a id="8666" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="8690" class="Keyword">open</a> <a id="8695" class="Keyword">import</a> <a id="8702" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="8740" class="Keyword">open</a> <a id="8745" class="Keyword">import</a> <a id="8752" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="8783" class="Keyword">open</a> <a id="8788" class="Keyword">import</a> <a id="8795" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="8820" class="Keyword">open</a> <a id="8825" class="Keyword">import</a> <a id="8832" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="8860" class="Keyword">open</a> <a id="8865" class="Keyword">import</a> <a id="8872" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="8896" class="Keyword">open</a> <a id="8901" class="Keyword">import</a> <a id="8908" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="8934" class="Keyword">open</a> <a id="8939" class="Keyword">import</a> <a id="8946" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="8981" class="Keyword">open</a> <a id="8986" class="Keyword">import</a> <a id="8993" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="9014" class="Keyword">open</a> <a id="9019" class="Keyword">import</a> <a id="9026" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="9075" class="Keyword">open</a> <a id="9080" class="Keyword">import</a> <a id="9087" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="9128" class="Keyword">open</a> <a id="9133" class="Keyword">import</a> <a id="9140" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="9190" class="Keyword">open</a> <a id="9195" class="Keyword">import</a> <a id="9202" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="9248" class="Keyword">open</a> <a id="9253" class="Keyword">import</a> <a id="9260" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="9300" class="Keyword">open</a> <a id="9305" class="Keyword">import</a> <a id="9312" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="9362" class="Keyword">open</a> <a id="9367" class="Keyword">import</a> <a id="9374" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="9413" class="Keyword">open</a> <a id="9418" class="Keyword">import</a> <a id="9425" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="9465" class="Keyword">open</a> <a id="9470" class="Keyword">import</a> <a id="9477" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="9510" class="Keyword">open</a> <a id="9515" class="Keyword">import</a> <a id="9522" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="9571" class="Keyword">open</a> <a id="9576" class="Keyword">import</a> <a id="9583" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="9608" class="Keyword">open</a> <a id="9613" class="Keyword">import</a> <a id="9620" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="9642" class="Keyword">open</a> <a id="9647" class="Keyword">import</a> <a id="9654" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="9682" class="Keyword">open</a> <a id="9687" class="Keyword">import</a> <a id="9694" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="9720" class="Keyword">open</a> <a id="9725" class="Keyword">import</a> <a id="9732" href="foundation.images.html" class="Module">foundation.images</a>
<a id="9750" class="Keyword">open</a> <a id="9755" class="Keyword">import</a> <a id="9762" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="9797" class="Keyword">open</a> <a id="9802" class="Keyword">import</a> <a id="9809" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="9836" class="Keyword">open</a> <a id="9841" class="Keyword">import</a> <a id="9848" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="9904" class="Keyword">open</a> <a id="9909" class="Keyword">import</a> <a id="9916" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="9945" class="Keyword">open</a> <a id="9950" class="Keyword">import</a> <a id="9957" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="9987" class="Keyword">open</a> <a id="9992" class="Keyword">import</a> <a id="9999" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="10025" class="Keyword">open</a> <a id="10030" class="Keyword">import</a> <a id="10037" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="10064" class="Keyword">open</a> <a id="10069" class="Keyword">import</a> <a id="10076" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="10099" class="Keyword">open</a> <a id="10104" class="Keyword">import</a> <a id="10111" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="10138" class="Keyword">open</a> <a id="10143" class="Keyword">import</a> <a id="10150" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="10182" class="Keyword">open</a> <a id="10187" class="Keyword">import</a> <a id="10194" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="10228" class="Keyword">open</a> <a id="10233" class="Keyword">import</a> <a id="10240" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="10280" class="Keyword">open</a> <a id="10285" class="Keyword">import</a> <a id="10292" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="10323" class="Keyword">open</a> <a id="10328" class="Keyword">import</a> <a id="10335" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="10367" class="Keyword">open</a> <a id="10372" class="Keyword">import</a> <a id="10379" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="10396" class="Keyword">open</a> <a id="10401" class="Keyword">import</a> <a id="10408" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="10433" class="Keyword">open</a> <a id="10438" class="Keyword">import</a> <a id="10445" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="10474" class="Keyword">open</a> <a id="10479" class="Keyword">import</a> <a id="10486" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="10511" class="Keyword">open</a> <a id="10516" class="Keyword">import</a> <a id="10523" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="10544" class="Keyword">open</a> <a id="10549" class="Keyword">import</a> <a id="10556" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="10576" class="Keyword">open</a> <a id="10581" class="Keyword">import</a> <a id="10588" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="10622" class="Keyword">open</a> <a id="10627" class="Keyword">import</a> <a id="10634" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="10658" class="Keyword">open</a> <a id="10663" class="Keyword">import</a> <a id="10670" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="10697" class="Keyword">open</a> <a id="10702" class="Keyword">import</a> <a id="10709" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="10744" class="Keyword">open</a> <a id="10749" class="Keyword">import</a> <a id="10756" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="10796" class="Keyword">open</a> <a id="10801" class="Keyword">import</a> <a id="10808" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="10838" class="Keyword">open</a> <a id="10843" class="Keyword">import</a> <a id="10850" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="10887" class="Keyword">open</a> <a id="10892" class="Keyword">import</a> <a id="10899" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="10923" class="Keyword">open</a> <a id="10928" class="Keyword">import</a> <a id="10935" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="10956" class="Keyword">open</a> <a id="10961" class="Keyword">import</a> <a id="10968" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="11003" class="Keyword">open</a> <a id="11008" class="Keyword">import</a> <a id="11015" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="11052" class="Keyword">open</a> <a id="11057" class="Keyword">import</a> <a id="11064" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="11113" class="Keyword">open</a> <a id="11118" class="Keyword">import</a> <a id="11125" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="11148" class="Keyword">open</a> <a id="11153" class="Keyword">import</a> <a id="11160" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="11183" class="Keyword">open</a> <a id="11188" class="Keyword">import</a> <a id="11195" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="11223" class="Keyword">open</a> <a id="11228" class="Keyword">import</a> <a id="11235" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="11255" class="Keyword">open</a> <a id="11260" class="Keyword">import</a> <a id="11267" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="11298" class="Keyword">open</a> <a id="11303" class="Keyword">import</a> <a id="11310" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="11337" class="Keyword">open</a> <a id="11342" class="Keyword">import</a> <a id="11349" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="11365" class="Keyword">open</a> <a id="11370" class="Keyword">import</a> <a id="11377" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="11408" class="Keyword">open</a> <a id="11413" class="Keyword">import</a> <a id="11420" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="11437" class="Keyword">open</a> <a id="11442" class="Keyword">import</a> <a id="11449" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="11471" class="Keyword">open</a> <a id="11476" class="Keyword">import</a> <a id="11483" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="11510" class="Keyword">open</a> <a id="11515" class="Keyword">import</a> <a id="11522" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="11545" class="Keyword">open</a> <a id="11550" class="Keyword">import</a> <a id="11557" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="11584" class="Keyword">open</a> <a id="11589" class="Keyword">import</a> <a id="11596" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="11629" class="Keyword">open</a> <a id="11634" class="Keyword">import</a> <a id="11641" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="11681" class="Keyword">open</a> <a id="11686" class="Keyword">import</a> <a id="11693" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="11714" class="Keyword">open</a> <a id="11719" class="Keyword">import</a> <a id="11726" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="11755" class="Keyword">open</a> <a id="11760" class="Keyword">import</a> <a id="11767" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="11805" class="Keyword">open</a> <a id="11810" class="Keyword">import</a> <a id="11817" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="11837" class="Keyword">open</a> <a id="11842" class="Keyword">import</a> <a id="11849" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="11873" class="Keyword">open</a> <a id="11878" class="Keyword">import</a> <a id="11885" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="11912" class="Keyword">open</a> <a id="11917" class="Keyword">import</a> <a id="11924" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="11954" class="Keyword">open</a> <a id="11959" class="Keyword">import</a> <a id="11966" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="11992" class="Keyword">open</a> <a id="11997" class="Keyword">import</a> <a id="12004" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="12031" class="Keyword">open</a> <a id="12036" class="Keyword">import</a> <a id="12043" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="12072" class="Keyword">open</a> <a id="12077" class="Keyword">import</a> <a id="12084" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="12107" class="Keyword">open</a> <a id="12112" class="Keyword">import</a> <a id="12119" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="12170" class="Keyword">open</a> <a id="12175" class="Keyword">import</a> <a id="12182" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="12225" class="Keyword">open</a> <a id="12230" class="Keyword">import</a> <a id="12237" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="12285" class="Keyword">open</a> <a id="12290" class="Keyword">import</a> <a id="12297" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="12335" class="Keyword">open</a> <a id="12340" class="Keyword">import</a> <a id="12347" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="12384" class="Keyword">open</a> <a id="12389" class="Keyword">import</a> <a id="12396" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="12424" class="Keyword">open</a> <a id="12429" class="Keyword">import</a> <a id="12436" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="12472" class="Keyword">open</a> <a id="12477" class="Keyword">import</a> <a id="12484" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="12522" class="Keyword">open</a> <a id="12527" class="Keyword">import</a> <a id="12534" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="12567" class="Keyword">open</a> <a id="12572" class="Keyword">import</a> <a id="12579" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="12600" class="Keyword">open</a> <a id="12605" class="Keyword">import</a> <a id="12612" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="12666" class="Keyword">open</a> <a id="12671" class="Keyword">import</a> <a id="12678" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="12700" class="Keyword">open</a> <a id="12705" class="Keyword">import</a> <a id="12712" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="12747" class="Keyword">open</a> <a id="12752" class="Keyword">import</a> <a id="12759" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="12789" class="Keyword">open</a> <a id="12794" class="Keyword">import</a> <a id="12801" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="12840" class="Keyword">open</a> <a id="12845" class="Keyword">import</a> <a id="12852" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="12906" class="Keyword">open</a> <a id="12911" class="Keyword">import</a> <a id="12918" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="12964" class="Keyword">open</a> <a id="12969" class="Keyword">import</a> <a id="12976" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="13027" class="Keyword">open</a> <a id="13032" class="Keyword">import</a> <a id="13039" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="13080" class="Keyword">open</a> <a id="13085" class="Keyword">import</a> <a id="13092" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="13137" class="Keyword">open</a> <a id="13142" class="Keyword">import</a> <a id="13149" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="13194" class="Keyword">open</a> <a id="13199" class="Keyword">import</a> <a id="13206" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="13242" class="Keyword">open</a> <a id="13247" class="Keyword">import</a> <a id="13254" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="13290" class="Keyword">open</a> <a id="13295" class="Keyword">import</a> <a id="13302" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="13367" class="Keyword">open</a> <a id="13372" class="Keyword">import</a> <a id="13379" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="13434" class="Keyword">open</a> <a id="13439" class="Keyword">import</a> <a id="13446" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="13486" class="Keyword">open</a> <a id="13491" class="Keyword">import</a> <a id="13498" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="13542" class="Keyword">open</a> <a id="13547" class="Keyword">import</a> <a id="13554" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="13599" class="Keyword">open</a> <a id="13604" class="Keyword">import</a> <a id="13611" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="13652" class="Keyword">open</a> <a id="13657" class="Keyword">import</a> <a id="13664" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="13704" class="Keyword">open</a> <a id="13709" class="Keyword">import</a> <a id="13716" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="13743" class="Keyword">open</a> <a id="13748" class="Keyword">import</a> <a id="13755" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="13782" class="Keyword">open</a> <a id="13787" class="Keyword">import</a> <a id="13794" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="13813" class="Keyword">open</a> <a id="13818" class="Keyword">import</a> <a id="13825" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="13865" class="Keyword">open</a> <a id="13870" class="Keyword">import</a> <a id="13877" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="13942" class="Keyword">open</a> <a id="13947" class="Keyword">import</a> <a id="13954" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="13977" class="Keyword">open</a> <a id="13982" class="Keyword">import</a> <a id="13989" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="14013" class="Keyword">open</a> <a id="14018" class="Keyword">import</a> <a id="14025" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="14065" class="Keyword">open</a> <a id="14070" class="Keyword">import</a> <a id="14077" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="14120" class="Keyword">open</a> <a id="14125" class="Keyword">import</a> <a id="14132" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="14166" class="Keyword">open</a> <a id="14171" class="Keyword">import</a> <a id="14178" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="14208" class="Keyword">open</a> <a id="14213" class="Keyword">import</a> <a id="14220" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="14254" class="Keyword">open</a> <a id="14259" class="Keyword">import</a> <a id="14266" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="14301" class="Keyword">open</a> <a id="14306" class="Keyword">import</a> <a id="14313" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="14350" class="Keyword">open</a> <a id="14355" class="Keyword">import</a> <a id="14362" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="14389" class="Keyword">open</a> <a id="14394" class="Keyword">import</a> <a id="14401" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="14429" class="Keyword">open</a> <a id="14434" class="Keyword">import</a> <a id="14441" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="14490" class="Keyword">open</a> <a id="14495" class="Keyword">import</a> <a id="14502" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="14548" class="Keyword">open</a> <a id="14553" class="Keyword">import</a> <a id="14560" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="14600" class="Keyword">open</a> <a id="14605" class="Keyword">import</a> <a id="14612" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="14650" class="Keyword">open</a> <a id="14655" class="Keyword">import</a> <a id="14662" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="14691" class="Keyword">open</a> <a id="14696" class="Keyword">import</a> <a id="14703" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="14733" class="Keyword">open</a> <a id="14738" class="Keyword">import</a> <a id="14745" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="14776" class="Keyword">open</a> <a id="14781" class="Keyword">import</a> <a id="14788" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="14814" class="Keyword">open</a> <a id="14819" class="Keyword">import</a> <a id="14826" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="14877" class="Keyword">open</a> <a id="14882" class="Keyword">import</a> <a id="14889" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="14943" class="Keyword">open</a> <a id="14948" class="Keyword">import</a> <a id="14955" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="14982" class="Keyword">open</a> <a id="14987" class="Keyword">import</a> <a id="14994" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="15027" class="Keyword">open</a> <a id="15032" class="Keyword">import</a> <a id="15039" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="15070" class="Keyword">open</a> <a id="15075" class="Keyword">import</a> <a id="15082" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="15119" class="Keyword">open</a> <a id="15124" class="Keyword">import</a> <a id="15131" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="15156" class="Keyword">open</a> <a id="15161" class="Keyword">import</a> <a id="15168" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="15200" class="Keyword">open</a> <a id="15205" class="Keyword">import</a> <a id="15212" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="15247" class="Keyword">open</a> <a id="15252" class="Keyword">import</a> <a id="15259" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="15288" class="Keyword">open</a> <a id="15293" class="Keyword">import</a> <a id="15300" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="15328" class="Keyword">open</a> <a id="15333" class="Keyword">import</a> <a id="15340" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="15365" class="Keyword">open</a> <a id="15370" class="Keyword">import</a> <a id="15377" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="15398" class="Keyword">open</a> <a id="15403" class="Keyword">import</a> <a id="15410" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="15446" class="Keyword">open</a> <a id="15451" class="Keyword">import</a> <a id="15458" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="15501" class="Keyword">open</a> <a id="15506" class="Keyword">import</a> <a id="15513" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="15538" class="Keyword">open</a> <a id="15543" class="Keyword">import</a> <a id="15550" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="15581" class="Keyword">open</a> <a id="15586" class="Keyword">import</a> <a id="15593" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="15625" class="Keyword">open</a> <a id="15630" class="Keyword">import</a> <a id="15637" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="15671" class="Keyword">open</a> <a id="15676" class="Keyword">import</a> <a id="15683" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="15739" class="Keyword">open</a> <a id="15744" class="Keyword">import</a> <a id="15751" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="15804" class="Keyword">open</a> <a id="15809" class="Keyword">import</a> <a id="15816" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="15843" class="Keyword">open</a> <a id="15848" class="Keyword">import</a> <a id="15855" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="15917" class="Keyword">open</a> <a id="15922" class="Keyword">import</a> <a id="15929" href="graph-theory.html" class="Module">graph-theory</a>
<a id="15942" class="Keyword">open</a> <a id="15947" class="Keyword">import</a> <a id="15954" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="15995" class="Keyword">open</a> <a id="16000" class="Keyword">import</a> <a id="16007" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="16036" class="Keyword">open</a> <a id="16041" class="Keyword">import</a> <a id="16048" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="16093" class="Keyword">open</a> <a id="16098" class="Keyword">import</a> <a id="16105" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="16149" class="Keyword">open</a> <a id="16154" class="Keyword">import</a> <a id="16161" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="16188" class="Keyword">open</a> <a id="16193" class="Keyword">import</a> <a id="16200" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="16241" class="Keyword">open</a> <a id="16246" class="Keyword">import</a> <a id="16253" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="16302" class="Keyword">open</a> <a id="16307" class="Keyword">import</a> <a id="16314" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="16355" class="Keyword">open</a> <a id="16360" class="Keyword">import</a> <a id="16367" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="16411" class="Keyword">open</a> <a id="16416" class="Keyword">import</a> <a id="16423" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="16460" class="Keyword">open</a> <a id="16465" class="Keyword">import</a> <a id="16472" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="16494" class="Keyword">open</a> <a id="16499" class="Keyword">import</a> <a id="16506" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="16536" class="Keyword">open</a> <a id="16541" class="Keyword">import</a> <a id="16548" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="16586" class="Keyword">open</a> <a id="16591" class="Keyword">import</a> <a id="16598" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="16659" class="Keyword">open</a> <a id="16664" class="Keyword">import</a> <a id="16671" href="group-theory.html" class="Module">group-theory</a>
<a id="16684" class="Keyword">open</a> <a id="16689" class="Keyword">import</a> <a id="16696" href="group-theory.abstract-abelian-groups.html" class="Module">group-theory.abstract-abelian-groups</a>
<a id="16733" class="Keyword">open</a> <a id="16738" class="Keyword">import</a> <a id="16745" href="group-theory.abstract-abelian-subgroups.html" class="Module">group-theory.abstract-abelian-subgroups</a>
<a id="16785" class="Keyword">open</a> <a id="16790" class="Keyword">import</a> <a id="16797" href="group-theory.abstract-group-actions.html" class="Module">group-theory.abstract-group-actions</a>
<a id="16833" class="Keyword">open</a> <a id="16838" class="Keyword">import</a> <a id="16845" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="16881" class="Keyword">open</a> <a id="16886" class="Keyword">import</a> <a id="16893" href="group-theory.abstract-groups.html" class="Module">group-theory.abstract-groups</a>
<a id="16922" class="Keyword">open</a> <a id="16927" class="Keyword">import</a> <a id="16934" href="group-theory.abstract-subgroups.html" class="Module">group-theory.abstract-subgroups</a>
<a id="16966" class="Keyword">open</a> <a id="16971" class="Keyword">import</a> <a id="16978" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="17014" class="Keyword">open</a> <a id="17019" class="Keyword">import</a> <a id="17026" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="17055" class="Keyword">open</a> <a id="17060" class="Keyword">import</a> <a id="17067" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="17099" class="Keyword">open</a> <a id="17104" class="Keyword">import</a> <a id="17111" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="17147" class="Keyword">open</a> <a id="17152" class="Keyword">import</a> <a id="17159" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="17191" class="Keyword">open</a> <a id="17196" class="Keyword">import</a> <a id="17203" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="17230" class="Keyword">open</a> <a id="17235" class="Keyword">import</a> <a id="17242" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="17299" class="Keyword">open</a> <a id="17304" class="Keyword">import</a> <a id="17311" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="17326" class="Keyword">open</a> <a id="17331" class="Keyword">import</a> <a id="17338" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="17362" class="Keyword">open</a> <a id="17367" class="Keyword">import</a> <a id="17374" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="17427" class="Keyword">open</a> <a id="17432" class="Keyword">import</a> <a id="17439" href="order-theory.html" class="Module">order-theory</a>
<a id="17452" class="Keyword">open</a> <a id="17457" class="Keyword">import</a> <a id="17464" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="17491" class="Keyword">open</a> <a id="17496" class="Keyword">import</a> <a id="17503" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="17533" class="Keyword">open</a> <a id="17538" class="Keyword">import</a> <a id="17545" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="17578" class="Keyword">open</a> <a id="17583" class="Keyword">import</a> <a id="17590" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="17626" class="Keyword">open</a> <a id="17631" class="Keyword">import</a> <a id="17638" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="17665" class="Keyword">open</a> <a id="17670" class="Keyword">import</a> <a id="17677" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="17707" class="Keyword">open</a> <a id="17712" class="Keyword">import</a> <a id="17719" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="17755" class="Keyword">open</a> <a id="17760" class="Keyword">import</a> <a id="17767" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="17799" class="Keyword">open</a> <a id="17804" class="Keyword">import</a> <a id="17811" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="17848" class="Keyword">open</a> <a id="17853" class="Keyword">import</a> <a id="17860" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="17900" class="Keyword">open</a> <a id="17905" class="Keyword">import</a> <a id="17912" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="17947" class="Keyword">open</a> <a id="17952" class="Keyword">import</a> <a id="17959" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="17997" class="Keyword">open</a> <a id="18002" class="Keyword">import</a> <a id="18009" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="18044" class="Keyword">open</a> <a id="18049" class="Keyword">import</a> <a id="18056" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="18091" class="Keyword">open</a> <a id="18096" class="Keyword">import</a> <a id="18103" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="18141" class="Keyword">open</a> <a id="18146" class="Keyword">import</a> <a id="18153" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="18186" class="Keyword">open</a> <a id="18191" class="Keyword">import</a> <a id="18198" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="18218" class="Keyword">open</a> <a id="18223" class="Keyword">import</a> <a id="18230" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="18253" class="Keyword">open</a> <a id="18258" class="Keyword">import</a> <a id="18265" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="18288" class="Keyword">open</a> <a id="18293" class="Keyword">import</a> <a id="18300" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="18326" class="Keyword">open</a> <a id="18331" class="Keyword">import</a> <a id="18338" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="18364" class="Keyword">open</a> <a id="18369" class="Keyword">import</a> <a id="18376" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="18432" class="Keyword">open</a> <a id="18437" class="Keyword">import</a> <a id="18444" href="polytopes.html" class="Module">polytopes</a>
<a id="18454" class="Keyword">open</a> <a id="18459" class="Keyword">import</a> <a id="18466" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="18524" class="Keyword">open</a> <a id="18529" class="Keyword">import</a> <a id="18536" href="ring-theory.html" class="Module">ring-theory</a>
<a id="18548" class="Keyword">open</a> <a id="18553" class="Keyword">import</a> <a id="18560" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="18592" class="Keyword">open</a> <a id="18597" class="Keyword">import</a> <a id="18604" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="18634" class="Keyword">open</a> <a id="18639" class="Keyword">import</a> <a id="18646" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a>
<a id="18665" class="Keyword">open</a> <a id="18670" class="Keyword">import</a> <a id="18677" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="18709" class="Keyword">open</a> <a id="18714" class="Keyword">import</a> <a id="18721" href="ring-theory.rings-with-properties.html" class="Module">ring-theory.rings-with-properties</a>
<a id="18755" class="Keyword">open</a> <a id="18760" class="Keyword">import</a> <a id="18767" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="18828" class="Keyword">open</a> <a id="18833" class="Keyword">import</a> <a id="18840" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="18866" class="Keyword">open</a> <a id="18871" class="Keyword">import</a> <a id="18878" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="18917" class="Keyword">open</a> <a id="18922" class="Keyword">import</a> <a id="18929" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="18967" class="Keyword">open</a> <a id="18972" class="Keyword">import</a> <a id="18979" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="19025" class="Keyword">open</a> <a id="19030" class="Keyword">import</a> <a id="19037" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="19074" class="Keyword">open</a> <a id="19079" class="Keyword">import</a> <a id="19086" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="19126" class="Keyword">open</a> <a id="19131" class="Keyword">import</a> <a id="19138" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="19177" class="Keyword">open</a> <a id="19182" class="Keyword">import</a> <a id="19189" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="19222" class="Keyword">open</a> <a id="19227" class="Keyword">import</a> <a id="19234" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="19273" class="Keyword">open</a> <a id="19278" class="Keyword">import</a> <a id="19285" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="19330" class="Keyword">open</a> <a id="19335" class="Keyword">import</a> <a id="19342" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="19394" class="Keyword">open</a> <a id="19399" class="Keyword">import</a> <a id="19406" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="19454" class="Keyword">open</a> <a id="19459" class="Keyword">import</a> <a id="19466" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="19506" class="Keyword">open</a> <a id="19511" class="Keyword">import</a> <a id="19518" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="19565" class="Keyword">open</a> <a id="19570" class="Keyword">import</a> <a id="19577" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="19615" class="Keyword">open</a> <a id="19620" class="Keyword">import</a> <a id="19627" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="19681" class="Keyword">open</a> <a id="19686" class="Keyword">import</a> <a id="19693" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="19740" class="Keyword">open</a> <a id="19745" class="Keyword">import</a> <a id="19752" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="19804" class="Keyword">open</a> <a id="19809" class="Keyword">import</a> <a id="19816" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="19861" class="Keyword">open</a> <a id="19866" class="Keyword">import</a> <a id="19873" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="19912" class="Keyword">open</a> <a id="19917" class="Keyword">import</a> <a id="19924" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="19964" class="Keyword">open</a> <a id="19969" class="Keyword">import</a> <a id="19976" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="20009" class="Keyword">open</a> <a id="20014" class="Keyword">import</a> <a id="20021" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="20066" class="Keyword">open</a> <a id="20071" class="Keyword">import</a> <a id="20078" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="20154" class="Keyword">open</a> <a id="20159" class="Keyword">import</a> <a id="20166" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="20228" class="Keyword">open</a> <a id="20233" class="Keyword">import</a> <a id="20240" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="20264" class="Keyword">open</a> <a id="20269" class="Keyword">import</a> <a id="20276" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="20316" class="Keyword">open</a> <a id="20321" class="Keyword">import</a> <a id="20328" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="20367" class="Keyword">open</a> <a id="20372" class="Keyword">import</a> <a id="20379" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="20427" class="Keyword">open</a> <a id="20432" class="Keyword">import</a> <a id="20439" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="20486" class="Keyword">open</a> <a id="20491" class="Keyword">import</a> <a id="20498" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="20538" class="Keyword">open</a> <a id="20543" class="Keyword">import</a> <a id="20550" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="20602" class="Keyword">open</a> <a id="20607" class="Keyword">import</a> <a id="20614" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="20672" class="Keyword">open</a> <a id="20677" class="Keyword">import</a> <a id="20684" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="20738" class="Keyword">open</a> <a id="20743" class="Keyword">import</a> <a id="20750" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="20798" class="Keyword">open</a> <a id="20803" class="Keyword">import</a> <a id="20810" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="20858" class="Keyword">open</a> <a id="20863" class="Keyword">import</a> <a id="20870" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="20909" class="Keyword">open</a> <a id="20914" class="Keyword">import</a> <a id="20921" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="20954" class="Keyword">open</a> <a id="20959" class="Keyword">import</a> <a id="20966" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="21025" class="Keyword">open</a> <a id="21030" class="Keyword">import</a> <a id="21037" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="21092" class="Keyword">open</a> <a id="21097" class="Keyword">import</a> <a id="21104" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="21147" class="Keyword">open</a> <a id="21152" class="Keyword">import</a> <a id="21159" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="21214" class="Keyword">open</a> <a id="21219" class="Keyword">import</a> <a id="21226" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="21277" class="Keyword">open</a> <a id="21282" class="Keyword">import</a> <a id="21289" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="21367" class="Keyword">open</a> <a id="21372" class="Keyword">import</a> <a id="21379" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="21419" class="Keyword">open</a> <a id="21424" class="Keyword">import</a> <a id="21431" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="21488" class="Keyword">open</a> <a id="21493" class="Keyword">import</a> <a id="21500" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="21535" class="Keyword">open</a> <a id="21540" class="Keyword">import</a> <a id="21547" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="21593" class="Keyword">open</a> <a id="21598" class="Keyword">import</a> <a id="21605" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="21660" class="Keyword">open</a> <a id="21665" class="Keyword">import</a> <a id="21672" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="21731" class="Keyword">open</a> <a id="21736" class="Keyword">import</a> <a id="21743" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="21780" class="Keyword">open</a> <a id="21785" class="Keyword">import</a> <a id="21792" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="21852" class="Keyword">open</a> <a id="21857" class="Keyword">import</a> <a id="21864" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="21902" class="Keyword">open</a> <a id="21907" class="Keyword">import</a> <a id="21914" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="21966" class="Keyword">open</a> <a id="21971" class="Keyword">import</a> <a id="21978" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="22024" class="Keyword">open</a> <a id="22029" class="Keyword">import</a> <a id="22036" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="22081" class="Keyword">open</a> <a id="22086" class="Keyword">import</a> <a id="22093" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="22130" class="Keyword">open</a> <a id="22135" class="Keyword">import</a> <a id="22142" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="22191" class="Keyword">open</a> <a id="22196" class="Keyword">import</a> <a id="22203" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="22241" class="Keyword">open</a> <a id="22246" class="Keyword">import</a> <a id="22253" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="22308" class="Keyword">open</a> <a id="22313" class="Keyword">import</a> <a id="22320" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="22359" class="Keyword">open</a> <a id="22364" class="Keyword">import</a> <a id="22371" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="22401" class="Keyword">open</a> <a id="22406" class="Keyword">import</a> <a id="22413" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="22443" class="Keyword">open</a> <a id="22448" class="Keyword">import</a> <a id="22455" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="22495" class="Keyword">open</a> <a id="22500" class="Keyword">import</a> <a id="22507" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="22552" class="Keyword">open</a> <a id="22557" class="Keyword">import</a> <a id="22564" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="22614" class="Keyword">open</a> <a id="22619" class="Keyword">import</a> <a id="22626" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="22664" class="Keyword">open</a> <a id="22669" class="Keyword">import</a> <a id="22676" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="22725" class="Keyword">open</a> <a id="22730" class="Keyword">import</a> <a id="22737" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="22800" class="Keyword">open</a> <a id="22805" class="Keyword">import</a> <a id="22812" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="22865" class="Keyword">open</a> <a id="22870" class="Keyword">import</a> <a id="22877" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="22923" class="Keyword">open</a> <a id="22928" class="Keyword">import</a> <a id="22935" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="22981" class="Keyword">open</a> <a id="22986" class="Keyword">import</a> <a id="22993" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="23041" class="Keyword">open</a> <a id="23046" class="Keyword">import</a> <a id="23053" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="23131" class="Keyword">open</a> <a id="23136" class="Keyword">import</a> <a id="23143" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="23211" class="Keyword">open</a> <a id="23216" class="Keyword">import</a> <a id="23223" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="23236" class="Keyword">open</a> <a id="23241" class="Keyword">import</a> <a id="23248" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="23268" class="Keyword">open</a> <a id="23273" class="Keyword">import</a> <a id="23280" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="23331" class="Keyword">open</a> <a id="23336" class="Keyword">import</a> <a id="23343" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="23368" class="Keyword">open</a> <a id="23373" class="Keyword">import</a> <a id="23380" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="23406" class="Keyword">open</a> <a id="23411" class="Keyword">import</a> <a id="23418" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

