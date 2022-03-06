# Univalent mathematics in Agda

Welcome to the website of the `agda-unimath` formalization project.

[![build](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml)

<pre class="Agda"><a id="281" class="Symbol">{-#</a> <a id="285" class="Keyword">OPTIONS</a> <a id="293" class="Pragma">--without-K</a> <a id="305" class="Pragma">--exact-split</a> <a id="319" class="Symbol">#-}</a>
</pre>
## Categories

<pre class="Agda"><a id="351" class="Keyword">open</a> <a id="356" class="Keyword">import</a> <a id="363" href="categories.html" class="Module">categories</a>
<a id="374" class="Keyword">open</a> <a id="379" class="Keyword">import</a> <a id="386" href="categories.adjunctions.html" class="Module">categories.adjunctions</a>
<a id="409" class="Keyword">open</a> <a id="414" class="Keyword">import</a> <a id="421" href="categories.categories.html" class="Module">categories.categories</a>
<a id="443" class="Keyword">open</a> <a id="448" class="Keyword">import</a> <a id="455" href="categories.functors.html" class="Module">categories.functors</a>
<a id="475" class="Keyword">open</a> <a id="480" class="Keyword">import</a> <a id="487" href="categories.large-categories.html" class="Module">categories.large-categories</a>
<a id="515" class="Keyword">open</a> <a id="520" class="Keyword">import</a> <a id="527" href="categories.natural-transformations.html" class="Module">categories.natural-transformations</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="604" class="Keyword">open</a> <a id="609" class="Keyword">import</a> <a id="616" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="665" class="Keyword">open</a> <a id="670" class="Keyword">import</a> <a id="677" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="720" class="Keyword">open</a> <a id="725" class="Keyword">import</a> <a id="732" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="782" class="Keyword">open</a> <a id="787" class="Keyword">import</a> <a id="794" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="841" class="Keyword">open</a> <a id="846" class="Keyword">import</a> <a id="853" href="elementary-number-theory.classical-finite-types.html" class="Module">elementary-number-theory.classical-finite-types</a>
<a id="901" class="Keyword">open</a> <a id="906" class="Keyword">import</a> <a id="913" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="956" class="Keyword">open</a> <a id="961" class="Keyword">import</a> <a id="968" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="1012" class="Keyword">open</a> <a id="1017" class="Keyword">import</a> <a id="1024" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="1069" class="Keyword">open</a> <a id="1074" class="Keyword">import</a> <a id="1081" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="1133" class="Keyword">open</a> <a id="1138" class="Keyword">import</a> <a id="1145" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="1205" class="Keyword">open</a> <a id="1210" class="Keyword">import</a> <a id="1217" href="elementary-number-theory.decidable-dependent-pair-types.html" class="Module">elementary-number-theory.decidable-dependent-pair-types</a>
<a id="1273" class="Keyword">open</a> <a id="1278" class="Keyword">import</a> <a id="1285" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="1330" class="Keyword">open</a> <a id="1335" class="Keyword">import</a> <a id="1342" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="1385" class="Keyword">open</a> <a id="1390" class="Keyword">import</a> <a id="1397" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="1447" class="Keyword">open</a> <a id="1452" class="Keyword">import</a> <a id="1459" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="1506" class="Keyword">open</a> <a id="1511" class="Keyword">import</a> <a id="1518" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="1572" class="Keyword">open</a> <a id="1577" class="Keyword">import</a> <a id="1584" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="1644" class="Keyword">open</a> <a id="1649" class="Keyword">import</a> <a id="1656" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="1699" class="Keyword">open</a> <a id="1704" class="Keyword">import</a> <a id="1711" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="1761" class="Keyword">open</a> <a id="1766" class="Keyword">import</a> <a id="1773" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="1833" class="Keyword">open</a> <a id="1838" class="Keyword">import</a> <a id="1845" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="1901" class="Keyword">open</a> <a id="1906" class="Keyword">import</a> <a id="1913" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="1949" class="Keyword">open</a> <a id="1954" class="Keyword">import</a> <a id="1961" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="2005" class="Keyword">open</a> <a id="2010" class="Keyword">import</a> <a id="2017" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="2061" class="Keyword">open</a> <a id="2066" class="Keyword">import</a> <a id="2073" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="2123" class="Keyword">open</a> <a id="2128" class="Keyword">import</a> <a id="2135" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="2181" class="Keyword">open</a> <a id="2186" class="Keyword">import</a> <a id="2193" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="2228" class="Keyword">open</a> <a id="2233" class="Keyword">import</a> <a id="2240" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="2285" class="Keyword">open</a> <a id="2290" class="Keyword">import</a> <a id="2297" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="2355" class="Keyword">open</a> <a id="2360" class="Keyword">import</a> <a id="2367" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="2432" class="Keyword">open</a> <a id="2437" class="Keyword">import</a> <a id="2444" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="2489" class="Keyword">open</a> <a id="2494" class="Keyword">import</a> <a id="2501" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="2553" class="Keyword">open</a> <a id="2558" class="Keyword">import</a> <a id="2565" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="2623" class="Keyword">open</a> <a id="2628" class="Keyword">import</a> <a id="2635" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="2681" class="Keyword">open</a> <a id="2686" class="Keyword">import</a> <a id="2693" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="2727" class="Keyword">open</a> <a id="2732" class="Keyword">import</a> <a id="2739" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="2784" class="Keyword">open</a> <a id="2789" class="Keyword">import</a> <a id="2796" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="2850" class="Keyword">open</a> <a id="2855" class="Keyword">import</a> <a id="2862" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="2928" class="Keyword">open</a> <a id="2933" class="Keyword">import</a> <a id="2940" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="2984" class="Keyword">open</a> <a id="2989" class="Keyword">import</a> <a id="2996" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="3045" class="Keyword">open</a> <a id="3050" class="Keyword">import</a> <a id="3057" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="3113" class="Keyword">open</a> <a id="3118" class="Keyword">import</a> <a id="3125" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="3166" class="Keyword">open</a> <a id="3171" class="Keyword">import</a> <a id="3178" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="3237" class="Keyword">open</a> <a id="3242" class="Keyword">import</a> <a id="3249" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="3288" class="Keyword">open</a> <a id="3293" class="Keyword">import</a> <a id="3300" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="3353" class="Keyword">open</a> <a id="3358" class="Keyword">import</a> <a id="3365" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="3422" class="Keyword">open</a> <a id="3427" class="Keyword">import</a> <a id="3434" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="3476" class="Keyword">open</a> <a id="3481" class="Keyword">import</a> <a id="3488" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="3539" class="Keyword">open</a> <a id="3544" class="Keyword">import</a> <a id="3551" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="3615" class="Keyword">open</a> <a id="3620" class="Keyword">import</a> <a id="3627" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="3680" class="Keyword">open</a> <a id="3685" class="Keyword">import</a> <a id="3692" href="elementary-number-theory.retracts-of-standard-finite-types.html" class="Module">elementary-number-theory.retracts-of-standard-finite-types</a>
<a id="3751" class="Keyword">open</a> <a id="3756" class="Keyword">import</a> <a id="3763" href="elementary-number-theory.skipping-element-standard-finite-type.html" class="Module">elementary-number-theory.skipping-element-standard-finite-type</a>
<a id="3826" class="Keyword">open</a> <a id="3831" class="Keyword">import</a> <a id="3838" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="3899" class="Keyword">open</a> <a id="3904" class="Keyword">import</a> <a id="3911" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="3969" class="Keyword">open</a> <a id="3974" class="Keyword">import</a> <a id="3981" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="4030" class="Keyword">open</a> <a id="4035" class="Keyword">import</a> <a id="4042" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="4086" class="Keyword">open</a> <a id="4091" class="Keyword">import</a> <a id="4098" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="4145" class="Keyword">open</a> <a id="4150" class="Keyword">import</a> <a id="4157" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="4217" class="Keyword">open</a> <a id="4222" class="Keyword">import</a> <a id="4229" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="4283" class="Keyword">open</a> <a id="4288" class="Keyword">import</a> <a id="4295" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="4360" class="Keyword">open</a> <a id="4365" class="Keyword">import</a> <a id="4372" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite groups

<pre class="Agda"><a id="4474" class="Keyword">open</a> <a id="4479" class="Keyword">import</a> <a id="4486" href="finite-groups.finite-groups.html" class="Module">finite-groups.finite-groups</a>
<a id="4514" class="Keyword">open</a> <a id="4519" class="Keyword">import</a> <a id="4526" href="finite-groups.quaternion-group.html" class="Module">finite-groups.quaternion-group</a>
<a id="4557" class="Keyword">open</a> <a id="4562" class="Keyword">import</a> <a id="4569" href="finite-groups.transpositions.html" class="Module">finite-groups.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="4626" class="Keyword">open</a> <a id="4631" class="Keyword">import</a> <a id="4638" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="4656" class="Keyword">open</a> <a id="4661" class="Keyword">import</a> <a id="4668" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="4687" class="Keyword">open</a> <a id="4692" class="Keyword">import</a> <a id="4699" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="4718" class="Keyword">open</a> <a id="4723" class="Keyword">import</a> <a id="4730" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="4774" class="Keyword">open</a> <a id="4779" class="Keyword">import</a> <a id="4786" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="4811" class="Keyword">open</a> <a id="4816" class="Keyword">import</a> <a id="4823" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="4850" class="Keyword">open</a> <a id="4855" class="Keyword">import</a> <a id="4862" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="4890" class="Keyword">open</a> <a id="4895" class="Keyword">import</a> <a id="4902" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="4932" class="Keyword">open</a> <a id="4937" class="Keyword">import</a> <a id="4944" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="4964" class="Keyword">open</a> <a id="4969" class="Keyword">import</a> <a id="4976" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="5013" class="Keyword">open</a> <a id="5018" class="Keyword">import</a> <a id="5025" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="5060" class="Keyword">open</a> <a id="5065" class="Keyword">import</a> <a id="5072" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="5130" class="Keyword">open</a> <a id="5135" class="Keyword">import</a> <a id="5142" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="5180" class="Keyword">open</a> <a id="5185" class="Keyword">import</a> <a id="5192" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="5221" class="Keyword">open</a> <a id="5226" class="Keyword">import</a> <a id="5233" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="5256" class="Keyword">open</a> <a id="5261" class="Keyword">import</a> <a id="5268" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="5291" class="Keyword">open</a> <a id="5296" class="Keyword">import</a> <a id="5303" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="5345" class="Keyword">open</a> <a id="5350" class="Keyword">import</a> <a id="5357" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="5389" class="Keyword">open</a> <a id="5394" class="Keyword">import</a> <a id="5401" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="5428" class="Keyword">open</a> <a id="5433" class="Keyword">import</a> <a id="5440" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="5465" class="Keyword">open</a> <a id="5470" class="Keyword">import</a> <a id="5477" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="5506" class="Keyword">open</a> <a id="5511" class="Keyword">import</a> <a id="5518" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="5548" class="Keyword">open</a> <a id="5553" class="Keyword">import</a> <a id="5560" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="5587" class="Keyword">open</a> <a id="5592" class="Keyword">import</a> <a id="5599" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="5618" class="Keyword">open</a> <a id="5623" class="Keyword">import</a> <a id="5630" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="5676" class="Keyword">open</a> <a id="5681" class="Keyword">import</a> <a id="5688" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="5730" class="Keyword">open</a> <a id="5735" class="Keyword">import</a> <a id="5742" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="5774" class="Keyword">open</a> <a id="5779" class="Keyword">import</a> <a id="5786" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="5816" class="Keyword">open</a> <a id="5821" class="Keyword">import</a> <a id="5828" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="5854" class="Keyword">open</a> <a id="5859" class="Keyword">import</a> <a id="5866" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="5900" class="Keyword">open</a> <a id="5905" class="Keyword">import</a> <a id="5912" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="5942" class="Keyword">open</a> <a id="5947" class="Keyword">import</a> <a id="5954" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="5981" class="Keyword">open</a> <a id="5986" class="Keyword">import</a> <a id="5993" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="6025" class="Keyword">open</a> <a id="6030" class="Keyword">import</a> <a id="6037" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="6071" class="Keyword">open</a> <a id="6076" class="Keyword">import</a> <a id="6083" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="6106" class="Keyword">open</a> <a id="6111" class="Keyword">import</a> <a id="6118" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="6188" class="Keyword">open</a> <a id="6193" class="Keyword">import</a> <a id="6200" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="6270" class="Keyword">open</a> <a id="6275" class="Keyword">import</a> <a id="6282" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="6309" class="Keyword">open</a> <a id="6314" class="Keyword">import</a> <a id="6321" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="6369" class="Keyword">open</a> <a id="6374" class="Keyword">import</a> <a id="6381" href="foundation.elementhood-relation-W-types.html" class="Module">foundation.elementhood-relation-W-types</a>
<a id="6421" class="Keyword">open</a> <a id="6426" class="Keyword">import</a> <a id="6433" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="6455" class="Keyword">open</a> <a id="6460" class="Keyword">import</a> <a id="6467" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="6490" class="Keyword">open</a> <a id="6495" class="Keyword">import</a> <a id="6502" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="6547" class="Keyword">open</a> <a id="6552" class="Keyword">import</a> <a id="6559" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="6603" class="Keyword">open</a> <a id="6608" class="Keyword">import</a> <a id="6615" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="6651" class="Keyword">open</a> <a id="6656" class="Keyword">import</a> <a id="6663" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="6708" class="Keyword">open</a> <a id="6713" class="Keyword">import</a> <a id="6720" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="6761" class="Keyword">open</a> <a id="6766" class="Keyword">import</a> <a id="6773" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="6808" class="Keyword">open</a> <a id="6813" class="Keyword">import</a> <a id="6820" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="6851" class="Keyword">open</a> <a id="6856" class="Keyword">import</a> <a id="6863" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="6896" class="Keyword">open</a> <a id="6901" class="Keyword">import</a> <a id="6908" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="6941" class="Keyword">open</a> <a id="6946" class="Keyword">import</a> <a id="6953" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="6983" class="Keyword">open</a> <a id="6988" class="Keyword">import</a> <a id="6995" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="7019" class="Keyword">open</a> <a id="7024" class="Keyword">import</a> <a id="7031" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="7069" class="Keyword">open</a> <a id="7074" class="Keyword">import</a> <a id="7081" href="foundation.extensional-W-types.html" class="Module">foundation.extensional-W-types</a>
<a id="7112" class="Keyword">open</a> <a id="7117" class="Keyword">import</a> <a id="7124" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="7149" class="Keyword">open</a> <a id="7154" class="Keyword">import</a> <a id="7161" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="7189" class="Keyword">open</a> <a id="7194" class="Keyword">import</a> <a id="7201" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="7225" class="Keyword">open</a> <a id="7230" class="Keyword">import</a> <a id="7237" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="7263" class="Keyword">open</a> <a id="7268" class="Keyword">import</a> <a id="7275" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="7310" class="Keyword">open</a> <a id="7315" class="Keyword">import</a> <a id="7322" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="7343" class="Keyword">open</a> <a id="7348" class="Keyword">import</a> <a id="7355" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="7404" class="Keyword">open</a> <a id="7409" class="Keyword">import</a> <a id="7416" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="7457" class="Keyword">open</a> <a id="7462" class="Keyword">import</a> <a id="7469" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="7519" class="Keyword">open</a> <a id="7524" class="Keyword">import</a> <a id="7531" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="7577" class="Keyword">open</a> <a id="7582" class="Keyword">import</a> <a id="7589" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="7629" class="Keyword">open</a> <a id="7634" class="Keyword">import</a> <a id="7641" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="7691" class="Keyword">open</a> <a id="7696" class="Keyword">import</a> <a id="7703" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="7742" class="Keyword">open</a> <a id="7747" class="Keyword">import</a> <a id="7754" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="7794" class="Keyword">open</a> <a id="7799" class="Keyword">import</a> <a id="7806" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="7855" class="Keyword">open</a> <a id="7860" class="Keyword">import</a> <a id="7867" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="7892" class="Keyword">open</a> <a id="7897" class="Keyword">import</a> <a id="7904" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="7926" class="Keyword">open</a> <a id="7931" class="Keyword">import</a> <a id="7938" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="7966" class="Keyword">open</a> <a id="7971" class="Keyword">import</a> <a id="7978" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="8004" class="Keyword">open</a> <a id="8009" class="Keyword">import</a> <a id="8016" href="foundation.images.html" class="Module">foundation.images</a>
<a id="8034" class="Keyword">open</a> <a id="8039" class="Keyword">import</a> <a id="8046" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="8081" class="Keyword">open</a> <a id="8086" class="Keyword">import</a> <a id="8093" href="foundation.indexed-W-types.html" class="Module">foundation.indexed-W-types</a>
<a id="8120" class="Keyword">open</a> <a id="8125" class="Keyword">import</a> <a id="8132" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="8188" class="Keyword">open</a> <a id="8193" class="Keyword">import</a> <a id="8200" href="foundation.induction-W-types.html" class="Module">foundation.induction-W-types</a>
<a id="8229" class="Keyword">open</a> <a id="8234" class="Keyword">import</a> <a id="8241" href="foundation.inequality-W-types.html" class="Module">foundation.inequality-W-types</a>
<a id="8271" class="Keyword">open</a> <a id="8276" class="Keyword">import</a> <a id="8283" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="8309" class="Keyword">open</a> <a id="8314" class="Keyword">import</a> <a id="8321" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="8348" class="Keyword">open</a> <a id="8353" class="Keyword">import</a> <a id="8360" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="8387" class="Keyword">open</a> <a id="8392" class="Keyword">import</a> <a id="8399" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="8431" class="Keyword">open</a> <a id="8436" class="Keyword">import</a> <a id="8443" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="8477" class="Keyword">open</a> <a id="8482" class="Keyword">import</a> <a id="8489" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="8529" class="Keyword">open</a> <a id="8534" class="Keyword">import</a> <a id="8541" href="foundation.lists.html" class="Module">foundation.lists</a>
<a id="8558" class="Keyword">open</a> <a id="8563" class="Keyword">import</a> <a id="8570" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="8601" class="Keyword">open</a> <a id="8606" class="Keyword">import</a> <a id="8613" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="8645" class="Keyword">open</a> <a id="8650" class="Keyword">import</a> <a id="8657" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="8674" class="Keyword">open</a> <a id="8679" class="Keyword">import</a> <a id="8686" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="8711" class="Keyword">open</a> <a id="8716" class="Keyword">import</a> <a id="8723" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="8752" class="Keyword">open</a> <a id="8757" class="Keyword">import</a> <a id="8764" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="8789" class="Keyword">open</a> <a id="8794" class="Keyword">import</a> <a id="8801" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="8822" class="Keyword">open</a> <a id="8827" class="Keyword">import</a> <a id="8834" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="8854" class="Keyword">open</a> <a id="8859" class="Keyword">import</a> <a id="8866" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="8900" class="Keyword">open</a> <a id="8905" class="Keyword">import</a> <a id="8912" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="8939" class="Keyword">open</a> <a id="8944" class="Keyword">import</a> <a id="8951" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="8986" class="Keyword">open</a> <a id="8991" class="Keyword">import</a> <a id="8998" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="9038" class="Keyword">open</a> <a id="9043" class="Keyword">import</a> <a id="9050" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="9080" class="Keyword">open</a> <a id="9085" class="Keyword">import</a> <a id="9092" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="9129" class="Keyword">open</a> <a id="9134" class="Keyword">import</a> <a id="9141" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="9165" class="Keyword">open</a> <a id="9170" class="Keyword">import</a> <a id="9177" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="9198" class="Keyword">open</a> <a id="9203" class="Keyword">import</a> <a id="9210" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="9245" class="Keyword">open</a> <a id="9250" class="Keyword">import</a> <a id="9257" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="9306" class="Keyword">open</a> <a id="9311" class="Keyword">import</a> <a id="9318" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="9341" class="Keyword">open</a> <a id="9346" class="Keyword">import</a> <a id="9353" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="9376" class="Keyword">open</a> <a id="9381" class="Keyword">import</a> <a id="9388" href="foundation.Russells-paradox.html" class="Module">foundation.Russells-paradox</a>
<a id="9416" class="Keyword">open</a> <a id="9421" class="Keyword">import</a> <a id="9428" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="9448" class="Keyword">open</a> <a id="9453" class="Keyword">import</a> <a id="9460" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="9491" class="Keyword">open</a> <a id="9496" class="Keyword">import</a> <a id="9503" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="9530" class="Keyword">open</a> <a id="9535" class="Keyword">import</a> <a id="9542" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="9558" class="Keyword">open</a> <a id="9563" class="Keyword">import</a> <a id="9570" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="9601" class="Keyword">open</a> <a id="9606" class="Keyword">import</a> <a id="9613" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="9630" class="Keyword">open</a> <a id="9635" class="Keyword">import</a> <a id="9642" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="9664" class="Keyword">open</a> <a id="9669" class="Keyword">import</a> <a id="9676" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="9703" class="Keyword">open</a> <a id="9708" class="Keyword">import</a> <a id="9715" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="9738" class="Keyword">open</a> <a id="9743" class="Keyword">import</a> <a id="9750" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="9777" class="Keyword">open</a> <a id="9782" class="Keyword">import</a> <a id="9789" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="9822" class="Keyword">open</a> <a id="9827" class="Keyword">import</a> <a id="9834" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="9874" class="Keyword">open</a> <a id="9879" class="Keyword">import</a> <a id="9886" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="9907" class="Keyword">open</a> <a id="9912" class="Keyword">import</a> <a id="9919" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="9948" class="Keyword">open</a> <a id="9953" class="Keyword">import</a> <a id="9960" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="9998" class="Keyword">open</a> <a id="10003" class="Keyword">import</a> <a id="10010" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="10030" class="Keyword">open</a> <a id="10035" class="Keyword">import</a> <a id="10042" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="10066" class="Keyword">open</a> <a id="10071" class="Keyword">import</a> <a id="10078" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="10105" class="Keyword">open</a> <a id="10110" class="Keyword">import</a> <a id="10117" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="10143" class="Keyword">open</a> <a id="10148" class="Keyword">import</a> <a id="10155" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="10182" class="Keyword">open</a> <a id="10187" class="Keyword">import</a> <a id="10194" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="10223" class="Keyword">open</a> <a id="10228" class="Keyword">import</a> <a id="10235" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="10286" class="Keyword">open</a> <a id="10291" class="Keyword">import</a> <a id="10298" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="10341" class="Keyword">open</a> <a id="10346" class="Keyword">import</a> <a id="10353" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="10401" class="Keyword">open</a> <a id="10406" class="Keyword">import</a> <a id="10413" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="10451" class="Keyword">open</a> <a id="10456" class="Keyword">import</a> <a id="10463" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="10500" class="Keyword">open</a> <a id="10505" class="Keyword">import</a> <a id="10512" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="10540" class="Keyword">open</a> <a id="10545" class="Keyword">import</a> <a id="10552" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="10588" class="Keyword">open</a> <a id="10593" class="Keyword">import</a> <a id="10600" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="10638" class="Keyword">open</a> <a id="10643" class="Keyword">import</a> <a id="10650" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="10671" class="Keyword">open</a> <a id="10676" class="Keyword">import</a> <a id="10683" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="10737" class="Keyword">open</a> <a id="10742" class="Keyword">import</a> <a id="10749" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="10771" class="Keyword">open</a> <a id="10776" class="Keyword">import</a> <a id="10783" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="10818" class="Keyword">open</a> <a id="10823" class="Keyword">import</a> <a id="10830" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="10869" class="Keyword">open</a> <a id="10874" class="Keyword">import</a> <a id="10881" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="10935" class="Keyword">open</a> <a id="10940" class="Keyword">import</a> <a id="10947" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="10993" class="Keyword">open</a> <a id="10998" class="Keyword">import</a> <a id="11005" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="11056" class="Keyword">open</a> <a id="11061" class="Keyword">import</a> <a id="11068" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="11109" class="Keyword">open</a> <a id="11114" class="Keyword">import</a> <a id="11121" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="11166" class="Keyword">open</a> <a id="11171" class="Keyword">import</a> <a id="11178" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="11223" class="Keyword">open</a> <a id="11228" class="Keyword">import</a> <a id="11235" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="11271" class="Keyword">open</a> <a id="11276" class="Keyword">import</a> <a id="11283" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="11319" class="Keyword">open</a> <a id="11324" class="Keyword">import</a> <a id="11331" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="11396" class="Keyword">open</a> <a id="11401" class="Keyword">import</a> <a id="11408" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="11463" class="Keyword">open</a> <a id="11468" class="Keyword">import</a> <a id="11475" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="11515" class="Keyword">open</a> <a id="11520" class="Keyword">import</a> <a id="11527" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="11571" class="Keyword">open</a> <a id="11576" class="Keyword">import</a> <a id="11583" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="11628" class="Keyword">open</a> <a id="11633" class="Keyword">import</a> <a id="11640" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="11680" class="Keyword">open</a> <a id="11685" class="Keyword">import</a> <a id="11692" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="11719" class="Keyword">open</a> <a id="11724" class="Keyword">import</a> <a id="11731" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="11758" class="Keyword">open</a> <a id="11763" class="Keyword">import</a> <a id="11770" href="foundation.W-types.html" class="Module">foundation.W-types</a>
<a id="11789" class="Keyword">open</a> <a id="11794" class="Keyword">import</a> <a id="11801" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="11841" class="Keyword">open</a> <a id="11846" class="Keyword">import</a> <a id="11853" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="11918" class="Keyword">open</a> <a id="11923" class="Keyword">import</a> <a id="11930" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="11953" class="Keyword">open</a> <a id="11958" class="Keyword">import</a> <a id="11965" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="11989" class="Keyword">open</a> <a id="11994" class="Keyword">import</a> <a id="12001" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="12041" class="Keyword">open</a> <a id="12046" class="Keyword">import</a> <a id="12053" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="12096" class="Keyword">open</a> <a id="12101" class="Keyword">import</a> <a id="12108" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="12142" class="Keyword">open</a> <a id="12147" class="Keyword">import</a> <a id="12154" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="12184" class="Keyword">open</a> <a id="12189" class="Keyword">import</a> <a id="12196" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="12230" class="Keyword">open</a> <a id="12235" class="Keyword">import</a> <a id="12242" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="12277" class="Keyword">open</a> <a id="12282" class="Keyword">import</a> <a id="12289" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="12326" class="Keyword">open</a> <a id="12331" class="Keyword">import</a> <a id="12338" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="12365" class="Keyword">open</a> <a id="12370" class="Keyword">import</a> <a id="12377" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="12426" class="Keyword">open</a> <a id="12431" class="Keyword">import</a> <a id="12438" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="12484" class="Keyword">open</a> <a id="12489" class="Keyword">import</a> <a id="12496" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="12536" class="Keyword">open</a> <a id="12541" class="Keyword">import</a> <a id="12548" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="12586" class="Keyword">open</a> <a id="12591" class="Keyword">import</a> <a id="12598" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="12627" class="Keyword">open</a> <a id="12632" class="Keyword">import</a> <a id="12639" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="12669" class="Keyword">open</a> <a id="12674" class="Keyword">import</a> <a id="12681" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="12712" class="Keyword">open</a> <a id="12717" class="Keyword">import</a> <a id="12724" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="12750" class="Keyword">open</a> <a id="12755" class="Keyword">import</a> <a id="12762" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="12813" class="Keyword">open</a> <a id="12818" class="Keyword">import</a> <a id="12825" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="12879" class="Keyword">open</a> <a id="12884" class="Keyword">import</a> <a id="12891" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="12918" class="Keyword">open</a> <a id="12923" class="Keyword">import</a> <a id="12930" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="12963" class="Keyword">open</a> <a id="12968" class="Keyword">import</a> <a id="12975" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="13006" class="Keyword">open</a> <a id="13011" class="Keyword">import</a> <a id="13018" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="13055" class="Keyword">open</a> <a id="13060" class="Keyword">import</a> <a id="13067" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="13099" class="Keyword">open</a> <a id="13104" class="Keyword">import</a> <a id="13111" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="13146" class="Keyword">open</a> <a id="13151" class="Keyword">import</a> <a id="13158" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="13187" class="Keyword">open</a> <a id="13192" class="Keyword">import</a> <a id="13199" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="13227" class="Keyword">open</a> <a id="13232" class="Keyword">import</a> <a id="13239" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="13264" class="Keyword">open</a> <a id="13269" class="Keyword">import</a> <a id="13276" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="13297" class="Keyword">open</a> <a id="13302" class="Keyword">import</a> <a id="13309" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="13345" class="Keyword">open</a> <a id="13350" class="Keyword">import</a> <a id="13357" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="13400" class="Keyword">open</a> <a id="13405" class="Keyword">import</a> <a id="13412" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="13437" class="Keyword">open</a> <a id="13442" class="Keyword">import</a> <a id="13449" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="13480" class="Keyword">open</a> <a id="13485" class="Keyword">import</a> <a id="13492" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="13524" class="Keyword">open</a> <a id="13529" class="Keyword">import</a> <a id="13536" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="13570" class="Keyword">open</a> <a id="13575" class="Keyword">import</a> <a id="13582" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="13638" class="Keyword">open</a> <a id="13643" class="Keyword">import</a> <a id="13650" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="13703" class="Keyword">open</a> <a id="13708" class="Keyword">import</a> <a id="13715" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="13742" class="Keyword">open</a> <a id="13747" class="Keyword">import</a> <a id="13754" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="13816" class="Keyword">open</a> <a id="13821" class="Keyword">import</a> <a id="13828" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="13857" class="Keyword">open</a> <a id="13862" class="Keyword">import</a> <a id="13869" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="13896" class="Keyword">open</a> <a id="13901" class="Keyword">import</a> <a id="13908" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="13930" class="Keyword">open</a> <a id="13935" class="Keyword">import</a> <a id="13942" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="13972" class="Keyword">open</a> <a id="13977" class="Keyword">import</a> <a id="13984" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Groups 

<pre class="Agda"><a id="14040" class="Keyword">open</a> <a id="14045" class="Keyword">import</a> <a id="14052" href="groups.abstract-abelian-groups.html" class="Module">groups.abstract-abelian-groups</a>
<a id="14083" class="Keyword">open</a> <a id="14088" class="Keyword">import</a> <a id="14095" href="groups.abstract-abelian-subgroups.html" class="Module">groups.abstract-abelian-subgroups</a>
<a id="14129" class="Keyword">open</a> <a id="14134" class="Keyword">import</a> <a id="14141" href="groups.abstract-group-actions.html" class="Module">groups.abstract-group-actions</a>
<a id="14171" class="Keyword">open</a> <a id="14176" class="Keyword">import</a> <a id="14183" href="groups.abstract-group-torsors.html" class="Module">groups.abstract-group-torsors</a>
<a id="14213" class="Keyword">open</a> <a id="14218" class="Keyword">import</a> <a id="14225" href="groups.abstract-groups.html" class="Module">groups.abstract-groups</a>
<a id="14248" class="Keyword">open</a> <a id="14253" class="Keyword">import</a> <a id="14260" href="groups.abstract-subgroups.html" class="Module">groups.abstract-subgroups</a>
<a id="14286" class="Keyword">open</a> <a id="14291" class="Keyword">import</a> <a id="14298" href="groups.concrete-group-actions.html" class="Module">groups.concrete-group-actions</a>
<a id="14328" class="Keyword">open</a> <a id="14333" class="Keyword">import</a> <a id="14340" href="groups.concrete-groups.html" class="Module">groups.concrete-groups</a>
<a id="14363" class="Keyword">open</a> <a id="14368" class="Keyword">import</a> <a id="14375" href="groups.concrete-subgroups.html" class="Module">groups.concrete-subgroups</a>
<a id="14401" class="Keyword">open</a> <a id="14406" class="Keyword">import</a> <a id="14413" href="groups.examples-higher-groups.html" class="Module">groups.examples-higher-groups</a>
<a id="14443" class="Keyword">open</a> <a id="14448" class="Keyword">import</a> <a id="14455" href="groups.furstenberg-groups.html" class="Module">groups.furstenberg-groups</a>
<a id="14481" class="Keyword">open</a> <a id="14486" class="Keyword">import</a> <a id="14493" href="groups.higher-groups.html" class="Module">groups.higher-groups</a>
<a id="14514" class="Keyword">open</a> <a id="14519" class="Keyword">import</a> <a id="14526" href="groups.sheargroups.html" class="Module">groups.sheargroups</a>
</pre>
## Order theory

<pre class="Agda"><a id="14575" class="Keyword">open</a> <a id="14580" class="Keyword">import</a> <a id="14587" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="14614" class="Keyword">open</a> <a id="14619" class="Keyword">import</a> <a id="14626" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="14656" class="Keyword">open</a> <a id="14661" class="Keyword">import</a> <a id="14668" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="14704" class="Keyword">open</a> <a id="14709" class="Keyword">import</a> <a id="14716" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="14749" class="Keyword">open</a> <a id="14754" class="Keyword">import</a> <a id="14761" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="14781" class="Keyword">open</a> <a id="14786" class="Keyword">import</a> <a id="14793" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="14843" class="Keyword">open</a> <a id="14848" class="Keyword">import</a> <a id="14855" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Rings

<pre class="Agda"><a id="14907" class="Keyword">open</a> <a id="14912" class="Keyword">import</a> <a id="14919" href="rings.eisenstein-integers.html" class="Module">rings.eisenstein-integers</a>
<a id="14945" class="Keyword">open</a> <a id="14950" class="Keyword">import</a> <a id="14957" href="rings.gaussian-integers.html" class="Module">rings.gaussian-integers</a>
<a id="14981" class="Keyword">open</a> <a id="14986" class="Keyword">import</a> <a id="14993" href="rings.ideals.html" class="Module">rings.ideals</a>
<a id="15006" class="Keyword">open</a> <a id="15011" class="Keyword">import</a> <a id="15018" href="rings.localizations-rings.html" class="Module">rings.localizations-rings</a>
<a id="15044" class="Keyword">open</a> <a id="15049" class="Keyword">import</a> <a id="15056" href="rings.rings-with-properties.html" class="Module">rings.rings-with-properties</a>
<a id="15084" class="Keyword">open</a> <a id="15089" class="Keyword">import</a> <a id="15096" href="rings.rings.html" class="Module">rings.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="15151" class="Keyword">open</a> <a id="15156" class="Keyword">import</a> <a id="15163" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="15202" class="Keyword">open</a> <a id="15207" class="Keyword">import</a> <a id="15214" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="15252" class="Keyword">open</a> <a id="15257" class="Keyword">import</a> <a id="15264" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="15310" class="Keyword">open</a> <a id="15315" class="Keyword">import</a> <a id="15322" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="15359" class="Keyword">open</a> <a id="15364" class="Keyword">import</a> <a id="15371" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="15411" class="Keyword">open</a> <a id="15416" class="Keyword">import</a> <a id="15423" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="15462" class="Keyword">open</a> <a id="15467" class="Keyword">import</a> <a id="15474" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="15507" class="Keyword">open</a> <a id="15512" class="Keyword">import</a> <a id="15519" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="15558" class="Keyword">open</a> <a id="15563" class="Keyword">import</a> <a id="15570" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="15618" class="Keyword">open</a> <a id="15623" class="Keyword">import</a> <a id="15630" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="15670" class="Keyword">open</a> <a id="15675" class="Keyword">import</a> <a id="15682" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="15715" class="Keyword">open</a> <a id="15720" class="Keyword">import</a> <a id="15727" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="15817" class="Keyword">open</a> <a id="15822" class="Keyword">import</a> <a id="15829" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="15869" class="Keyword">open</a> <a id="15874" class="Keyword">import</a> <a id="15881" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="15920" class="Keyword">open</a> <a id="15925" class="Keyword">import</a> <a id="15932" href="univalent-combinatorics.cartesian-product-finite-types.html" class="Module">univalent-combinatorics.cartesian-product-finite-types</a>
<a id="15987" class="Keyword">open</a> <a id="15992" class="Keyword">import</a> <a id="15999" href="univalent-combinatorics.coproduct-finite-types.html" class="Module">univalent-combinatorics.coproduct-finite-types</a>
<a id="16046" class="Keyword">open</a> <a id="16051" class="Keyword">import</a> <a id="16058" href="univalent-combinatorics.counting-cartesian-product-types.html" class="Module">univalent-combinatorics.counting-cartesian-product-types</a>
<a id="16115" class="Keyword">open</a> <a id="16120" class="Keyword">import</a> <a id="16127" href="univalent-combinatorics.counting-coproduct-types.html" class="Module">univalent-combinatorics.counting-coproduct-types</a>
<a id="16176" class="Keyword">open</a> <a id="16181" class="Keyword">import</a> <a id="16188" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="16240" class="Keyword">open</a> <a id="16245" class="Keyword">import</a> <a id="16252" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="16310" class="Keyword">open</a> <a id="16315" class="Keyword">import</a> <a id="16322" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="16376" class="Keyword">open</a> <a id="16381" class="Keyword">import</a> <a id="16388" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="16436" class="Keyword">open</a> <a id="16441" class="Keyword">import</a> <a id="16448" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="16496" class="Keyword">open</a> <a id="16501" class="Keyword">import</a> <a id="16508" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="16547" class="Keyword">open</a> <a id="16552" class="Keyword">import</a> <a id="16559" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="16592" class="Keyword">open</a> <a id="16597" class="Keyword">import</a> <a id="16604" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="16663" class="Keyword">open</a> <a id="16668" class="Keyword">import</a> <a id="16675" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="16730" class="Keyword">open</a> <a id="16735" class="Keyword">import</a> <a id="16742" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="16785" class="Keyword">open</a> <a id="16790" class="Keyword">import</a> <a id="16797" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="16852" class="Keyword">open</a> <a id="16857" class="Keyword">import</a> <a id="16864" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="16915" class="Keyword">open</a> <a id="16920" class="Keyword">import</a> <a id="16927" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="17005" class="Keyword">open</a> <a id="17010" class="Keyword">import</a> <a id="17017" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="17057" class="Keyword">open</a> <a id="17062" class="Keyword">import</a> <a id="17069" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="17104" class="Keyword">open</a> <a id="17109" class="Keyword">import</a> <a id="17116" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="17173" class="Keyword">open</a> <a id="17178" class="Keyword">import</a> <a id="17185" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="17231" class="Keyword">open</a> <a id="17236" class="Keyword">import</a> <a id="17243" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="17298" class="Keyword">open</a> <a id="17303" class="Keyword">import</a> <a id="17310" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="17347" class="Keyword">open</a> <a id="17352" class="Keyword">import</a> <a id="17359" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="17418" class="Keyword">open</a> <a id="17423" class="Keyword">import</a> <a id="17430" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="17490" class="Keyword">open</a> <a id="17495" class="Keyword">import</a> <a id="17502" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="17540" class="Keyword">open</a> <a id="17545" class="Keyword">import</a> <a id="17552" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="17604" class="Keyword">open</a> <a id="17609" class="Keyword">import</a> <a id="17616" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="17662" class="Keyword">open</a> <a id="17667" class="Keyword">import</a> <a id="17674" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="17719" class="Keyword">open</a> <a id="17724" class="Keyword">import</a> <a id="17731" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="17768" class="Keyword">open</a> <a id="17773" class="Keyword">import</a> <a id="17780" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="17829" class="Keyword">open</a> <a id="17834" class="Keyword">import</a> <a id="17841" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="17879" class="Keyword">open</a> <a id="17884" class="Keyword">import</a> <a id="17891" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="17946" class="Keyword">open</a> <a id="17951" class="Keyword">import</a> <a id="17958" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="17997" class="Keyword">open</a> <a id="18002" class="Keyword">import</a> <a id="18009" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="18039" class="Keyword">open</a> <a id="18044" class="Keyword">import</a> <a id="18051" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="18091" class="Keyword">open</a> <a id="18096" class="Keyword">import</a> <a id="18103" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="18148" class="Keyword">open</a> <a id="18153" class="Keyword">import</a> <a id="18160" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="18198" class="Keyword">open</a> <a id="18203" class="Keyword">import</a> <a id="18210" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="18259" class="Keyword">open</a> <a id="18264" class="Keyword">import</a> <a id="18271" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="18317" class="Keyword">open</a> <a id="18322" class="Keyword">import</a> <a id="18329" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="18377" class="Keyword">open</a> <a id="18382" class="Keyword">import</a> <a id="18389" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="18467" class="Keyword">open</a> <a id="18472" class="Keyword">import</a> <a id="18479" href="univalent-foundations.functoriality-loop-spaces.html" class="Module">univalent-foundations.functoriality-loop-spaces</a>
<a id="18527" class="Keyword">open</a> <a id="18532" class="Keyword">import</a> <a id="18539" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
<a id="18577" class="Keyword">open</a> <a id="18582" class="Keyword">import</a> <a id="18589" href="univalent-foundations.iterated-loop-spaces.html" class="Module">univalent-foundations.iterated-loop-spaces</a>
<a id="18632" class="Keyword">open</a> <a id="18637" class="Keyword">import</a> <a id="18644" href="univalent-foundations.loop-spaces.html" class="Module">univalent-foundations.loop-spaces</a>
<a id="18678" class="Keyword">open</a> <a id="18683" class="Keyword">import</a> <a id="18690" href="univalent-foundations.pointed-dependent-functions.html" class="Module">univalent-foundations.pointed-dependent-functions</a>
<a id="18740" class="Keyword">open</a> <a id="18745" class="Keyword">import</a> <a id="18752" href="univalent-foundations.pointed-equivalences.html" class="Module">univalent-foundations.pointed-equivalences</a>
<a id="18795" class="Keyword">open</a> <a id="18800" class="Keyword">import</a> <a id="18807" href="univalent-foundations.pointed-families-of-types.html" class="Module">univalent-foundations.pointed-families-of-types</a>
<a id="18855" class="Keyword">open</a> <a id="18860" class="Keyword">import</a> <a id="18867" href="univalent-foundations.pointed-homotopies.html" class="Module">univalent-foundations.pointed-homotopies</a>
<a id="18908" class="Keyword">open</a> <a id="18913" class="Keyword">import</a> <a id="18920" href="univalent-foundations.pointed-maps.html" class="Module">univalent-foundations.pointed-maps</a>
<a id="18955" class="Keyword">open</a> <a id="18960" class="Keyword">import</a> <a id="18967" href="univalent-foundations.pointed-types.html" class="Module">univalent-foundations.pointed-types</a>
<a id="19003" class="Keyword">open</a> <a id="19008" class="Keyword">import</a> <a id="19015" href="univalent-foundations.truncations.html" class="Module">univalent-foundations.truncations</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

