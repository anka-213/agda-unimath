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

<pre class="Agda"><a id="4474" class="Keyword">open</a> <a id="4479" class="Keyword">import</a> <a id="4486" href="finite-groups.abstract-quaternion-group.html" class="Module">finite-groups.abstract-quaternion-group</a>
<a id="4526" class="Keyword">open</a> <a id="4531" class="Keyword">import</a> <a id="4538" href="finite-groups.finite-groups.html" class="Module">finite-groups.finite-groups</a>
<a id="4566" class="Keyword">open</a> <a id="4571" class="Keyword">import</a> <a id="4578" href="finite-groups.concrete-quaternion-group.html" class="Module">finite-groups.concrete-quaternion-group</a>
<a id="4618" class="Keyword">open</a> <a id="4623" class="Keyword">import</a> <a id="4630" href="finite-groups.transpositions.html" class="Module">finite-groups.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="4687" class="Keyword">open</a> <a id="4692" class="Keyword">import</a> <a id="4699" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="4717" class="Keyword">open</a> <a id="4722" class="Keyword">import</a> <a id="4729" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="4748" class="Keyword">open</a> <a id="4753" class="Keyword">import</a> <a id="4760" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="4779" class="Keyword">open</a> <a id="4784" class="Keyword">import</a> <a id="4791" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="4835" class="Keyword">open</a> <a id="4840" class="Keyword">import</a> <a id="4847" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="4872" class="Keyword">open</a> <a id="4877" class="Keyword">import</a> <a id="4884" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="4911" class="Keyword">open</a> <a id="4916" class="Keyword">import</a> <a id="4923" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="4951" class="Keyword">open</a> <a id="4956" class="Keyword">import</a> <a id="4963" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="4993" class="Keyword">open</a> <a id="4998" class="Keyword">import</a> <a id="5005" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="5025" class="Keyword">open</a> <a id="5030" class="Keyword">import</a> <a id="5037" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="5074" class="Keyword">open</a> <a id="5079" class="Keyword">import</a> <a id="5086" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="5121" class="Keyword">open</a> <a id="5126" class="Keyword">import</a> <a id="5133" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="5191" class="Keyword">open</a> <a id="5196" class="Keyword">import</a> <a id="5203" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="5241" class="Keyword">open</a> <a id="5246" class="Keyword">import</a> <a id="5253" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="5282" class="Keyword">open</a> <a id="5287" class="Keyword">import</a> <a id="5294" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="5317" class="Keyword">open</a> <a id="5322" class="Keyword">import</a> <a id="5329" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="5352" class="Keyword">open</a> <a id="5357" class="Keyword">import</a> <a id="5364" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="5406" class="Keyword">open</a> <a id="5411" class="Keyword">import</a> <a id="5418" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="5450" class="Keyword">open</a> <a id="5455" class="Keyword">import</a> <a id="5462" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="5489" class="Keyword">open</a> <a id="5494" class="Keyword">import</a> <a id="5501" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="5526" class="Keyword">open</a> <a id="5531" class="Keyword">import</a> <a id="5538" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="5567" class="Keyword">open</a> <a id="5572" class="Keyword">import</a> <a id="5579" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="5609" class="Keyword">open</a> <a id="5614" class="Keyword">import</a> <a id="5621" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="5648" class="Keyword">open</a> <a id="5653" class="Keyword">import</a> <a id="5660" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="5679" class="Keyword">open</a> <a id="5684" class="Keyword">import</a> <a id="5691" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="5737" class="Keyword">open</a> <a id="5742" class="Keyword">import</a> <a id="5749" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="5791" class="Keyword">open</a> <a id="5796" class="Keyword">import</a> <a id="5803" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="5835" class="Keyword">open</a> <a id="5840" class="Keyword">import</a> <a id="5847" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="5877" class="Keyword">open</a> <a id="5882" class="Keyword">import</a> <a id="5889" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="5915" class="Keyword">open</a> <a id="5920" class="Keyword">import</a> <a id="5927" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="5961" class="Keyword">open</a> <a id="5966" class="Keyword">import</a> <a id="5973" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="6003" class="Keyword">open</a> <a id="6008" class="Keyword">import</a> <a id="6015" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="6042" class="Keyword">open</a> <a id="6047" class="Keyword">import</a> <a id="6054" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="6086" class="Keyword">open</a> <a id="6091" class="Keyword">import</a> <a id="6098" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="6132" class="Keyword">open</a> <a id="6137" class="Keyword">import</a> <a id="6144" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="6167" class="Keyword">open</a> <a id="6172" class="Keyword">import</a> <a id="6179" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="6249" class="Keyword">open</a> <a id="6254" class="Keyword">import</a> <a id="6261" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="6331" class="Keyword">open</a> <a id="6336" class="Keyword">import</a> <a id="6343" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="6370" class="Keyword">open</a> <a id="6375" class="Keyword">import</a> <a id="6382" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="6430" class="Keyword">open</a> <a id="6435" class="Keyword">import</a> <a id="6442" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="6482" class="Keyword">open</a> <a id="6487" class="Keyword">import</a> <a id="6494" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="6516" class="Keyword">open</a> <a id="6521" class="Keyword">import</a> <a id="6528" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="6551" class="Keyword">open</a> <a id="6556" class="Keyword">import</a> <a id="6563" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="6608" class="Keyword">open</a> <a id="6613" class="Keyword">import</a> <a id="6620" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="6664" class="Keyword">open</a> <a id="6669" class="Keyword">import</a> <a id="6676" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="6712" class="Keyword">open</a> <a id="6717" class="Keyword">import</a> <a id="6724" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="6769" class="Keyword">open</a> <a id="6774" class="Keyword">import</a> <a id="6781" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="6822" class="Keyword">open</a> <a id="6827" class="Keyword">import</a> <a id="6834" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="6869" class="Keyword">open</a> <a id="6874" class="Keyword">import</a> <a id="6881" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="6912" class="Keyword">open</a> <a id="6917" class="Keyword">import</a> <a id="6924" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="6957" class="Keyword">open</a> <a id="6962" class="Keyword">import</a> <a id="6969" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="7002" class="Keyword">open</a> <a id="7007" class="Keyword">import</a> <a id="7014" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="7044" class="Keyword">open</a> <a id="7049" class="Keyword">import</a> <a id="7056" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="7080" class="Keyword">open</a> <a id="7085" class="Keyword">import</a> <a id="7092" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="7130" class="Keyword">open</a> <a id="7135" class="Keyword">import</a> <a id="7142" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="7173" class="Keyword">open</a> <a id="7178" class="Keyword">import</a> <a id="7185" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="7210" class="Keyword">open</a> <a id="7215" class="Keyword">import</a> <a id="7222" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="7250" class="Keyword">open</a> <a id="7255" class="Keyword">import</a> <a id="7262" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="7286" class="Keyword">open</a> <a id="7291" class="Keyword">import</a> <a id="7298" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="7324" class="Keyword">open</a> <a id="7329" class="Keyword">import</a> <a id="7336" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="7371" class="Keyword">open</a> <a id="7376" class="Keyword">import</a> <a id="7383" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="7404" class="Keyword">open</a> <a id="7409" class="Keyword">import</a> <a id="7416" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="7465" class="Keyword">open</a> <a id="7470" class="Keyword">import</a> <a id="7477" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="7518" class="Keyword">open</a> <a id="7523" class="Keyword">import</a> <a id="7530" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="7580" class="Keyword">open</a> <a id="7585" class="Keyword">import</a> <a id="7592" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="7638" class="Keyword">open</a> <a id="7643" class="Keyword">import</a> <a id="7650" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="7690" class="Keyword">open</a> <a id="7695" class="Keyword">import</a> <a id="7702" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="7752" class="Keyword">open</a> <a id="7757" class="Keyword">import</a> <a id="7764" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="7803" class="Keyword">open</a> <a id="7808" class="Keyword">import</a> <a id="7815" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="7855" class="Keyword">open</a> <a id="7860" class="Keyword">import</a> <a id="7867" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="7916" class="Keyword">open</a> <a id="7921" class="Keyword">import</a> <a id="7928" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="7953" class="Keyword">open</a> <a id="7958" class="Keyword">import</a> <a id="7965" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="7987" class="Keyword">open</a> <a id="7992" class="Keyword">import</a> <a id="7999" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="8027" class="Keyword">open</a> <a id="8032" class="Keyword">import</a> <a id="8039" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="8065" class="Keyword">open</a> <a id="8070" class="Keyword">import</a> <a id="8077" href="foundation.images.html" class="Module">foundation.images</a>
<a id="8095" class="Keyword">open</a> <a id="8100" class="Keyword">import</a> <a id="8107" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="8142" class="Keyword">open</a> <a id="8147" class="Keyword">import</a> <a id="8154" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="8181" class="Keyword">open</a> <a id="8186" class="Keyword">import</a> <a id="8193" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="8249" class="Keyword">open</a> <a id="8254" class="Keyword">import</a> <a id="8261" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="8290" class="Keyword">open</a> <a id="8295" class="Keyword">import</a> <a id="8302" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="8332" class="Keyword">open</a> <a id="8337" class="Keyword">import</a> <a id="8344" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="8370" class="Keyword">open</a> <a id="8375" class="Keyword">import</a> <a id="8382" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="8409" class="Keyword">open</a> <a id="8414" class="Keyword">import</a> <a id="8421" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="8444" class="Keyword">open</a> <a id="8449" class="Keyword">import</a> <a id="8456" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="8483" class="Keyword">open</a> <a id="8488" class="Keyword">import</a> <a id="8495" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="8527" class="Keyword">open</a> <a id="8532" class="Keyword">import</a> <a id="8539" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="8573" class="Keyword">open</a> <a id="8578" class="Keyword">import</a> <a id="8585" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="8625" class="Keyword">open</a> <a id="8630" class="Keyword">import</a> <a id="8637" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="8668" class="Keyword">open</a> <a id="8673" class="Keyword">import</a> <a id="8680" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="8712" class="Keyword">open</a> <a id="8717" class="Keyword">import</a> <a id="8724" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="8741" class="Keyword">open</a> <a id="8746" class="Keyword">import</a> <a id="8753" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="8778" class="Keyword">open</a> <a id="8783" class="Keyword">import</a> <a id="8790" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="8819" class="Keyword">open</a> <a id="8824" class="Keyword">import</a> <a id="8831" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="8856" class="Keyword">open</a> <a id="8861" class="Keyword">import</a> <a id="8868" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="8889" class="Keyword">open</a> <a id="8894" class="Keyword">import</a> <a id="8901" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="8921" class="Keyword">open</a> <a id="8926" class="Keyword">import</a> <a id="8933" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="8967" class="Keyword">open</a> <a id="8972" class="Keyword">import</a> <a id="8979" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="9006" class="Keyword">open</a> <a id="9011" class="Keyword">import</a> <a id="9018" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="9053" class="Keyword">open</a> <a id="9058" class="Keyword">import</a> <a id="9065" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="9105" class="Keyword">open</a> <a id="9110" class="Keyword">import</a> <a id="9117" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="9147" class="Keyword">open</a> <a id="9152" class="Keyword">import</a> <a id="9159" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="9196" class="Keyword">open</a> <a id="9201" class="Keyword">import</a> <a id="9208" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="9232" class="Keyword">open</a> <a id="9237" class="Keyword">import</a> <a id="9244" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="9265" class="Keyword">open</a> <a id="9270" class="Keyword">import</a> <a id="9277" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="9312" class="Keyword">open</a> <a id="9317" class="Keyword">import</a> <a id="9324" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="9373" class="Keyword">open</a> <a id="9378" class="Keyword">import</a> <a id="9385" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="9408" class="Keyword">open</a> <a id="9413" class="Keyword">import</a> <a id="9420" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="9443" class="Keyword">open</a> <a id="9448" class="Keyword">import</a> <a id="9455" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="9483" class="Keyword">open</a> <a id="9488" class="Keyword">import</a> <a id="9495" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="9515" class="Keyword">open</a> <a id="9520" class="Keyword">import</a> <a id="9527" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="9558" class="Keyword">open</a> <a id="9563" class="Keyword">import</a> <a id="9570" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="9597" class="Keyword">open</a> <a id="9602" class="Keyword">import</a> <a id="9609" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="9625" class="Keyword">open</a> <a id="9630" class="Keyword">import</a> <a id="9637" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="9668" class="Keyword">open</a> <a id="9673" class="Keyword">import</a> <a id="9680" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="9697" class="Keyword">open</a> <a id="9702" class="Keyword">import</a> <a id="9709" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="9731" class="Keyword">open</a> <a id="9736" class="Keyword">import</a> <a id="9743" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="9770" class="Keyword">open</a> <a id="9775" class="Keyword">import</a> <a id="9782" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="9805" class="Keyword">open</a> <a id="9810" class="Keyword">import</a> <a id="9817" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="9844" class="Keyword">open</a> <a id="9849" class="Keyword">import</a> <a id="9856" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="9889" class="Keyword">open</a> <a id="9894" class="Keyword">import</a> <a id="9901" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="9941" class="Keyword">open</a> <a id="9946" class="Keyword">import</a> <a id="9953" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="9974" class="Keyword">open</a> <a id="9979" class="Keyword">import</a> <a id="9986" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="10015" class="Keyword">open</a> <a id="10020" class="Keyword">import</a> <a id="10027" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="10065" class="Keyword">open</a> <a id="10070" class="Keyword">import</a> <a id="10077" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="10097" class="Keyword">open</a> <a id="10102" class="Keyword">import</a> <a id="10109" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="10133" class="Keyword">open</a> <a id="10138" class="Keyword">import</a> <a id="10145" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="10172" class="Keyword">open</a> <a id="10177" class="Keyword">import</a> <a id="10184" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="10210" class="Keyword">open</a> <a id="10215" class="Keyword">import</a> <a id="10222" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="10249" class="Keyword">open</a> <a id="10254" class="Keyword">import</a> <a id="10261" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="10290" class="Keyword">open</a> <a id="10295" class="Keyword">import</a> <a id="10302" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="10353" class="Keyword">open</a> <a id="10358" class="Keyword">import</a> <a id="10365" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="10408" class="Keyword">open</a> <a id="10413" class="Keyword">import</a> <a id="10420" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="10468" class="Keyword">open</a> <a id="10473" class="Keyword">import</a> <a id="10480" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="10518" class="Keyword">open</a> <a id="10523" class="Keyword">import</a> <a id="10530" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="10567" class="Keyword">open</a> <a id="10572" class="Keyword">import</a> <a id="10579" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="10607" class="Keyword">open</a> <a id="10612" class="Keyword">import</a> <a id="10619" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="10655" class="Keyword">open</a> <a id="10660" class="Keyword">import</a> <a id="10667" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="10705" class="Keyword">open</a> <a id="10710" class="Keyword">import</a> <a id="10717" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="10750" class="Keyword">open</a> <a id="10755" class="Keyword">import</a> <a id="10762" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="10783" class="Keyword">open</a> <a id="10788" class="Keyword">import</a> <a id="10795" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="10849" class="Keyword">open</a> <a id="10854" class="Keyword">import</a> <a id="10861" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="10883" class="Keyword">open</a> <a id="10888" class="Keyword">import</a> <a id="10895" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="10930" class="Keyword">open</a> <a id="10935" class="Keyword">import</a> <a id="10942" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="10981" class="Keyword">open</a> <a id="10986" class="Keyword">import</a> <a id="10993" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="11047" class="Keyword">open</a> <a id="11052" class="Keyword">import</a> <a id="11059" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="11105" class="Keyword">open</a> <a id="11110" class="Keyword">import</a> <a id="11117" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="11168" class="Keyword">open</a> <a id="11173" class="Keyword">import</a> <a id="11180" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="11221" class="Keyword">open</a> <a id="11226" class="Keyword">import</a> <a id="11233" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="11278" class="Keyword">open</a> <a id="11283" class="Keyword">import</a> <a id="11290" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="11335" class="Keyword">open</a> <a id="11340" class="Keyword">import</a> <a id="11347" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="11383" class="Keyword">open</a> <a id="11388" class="Keyword">import</a> <a id="11395" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="11431" class="Keyword">open</a> <a id="11436" class="Keyword">import</a> <a id="11443" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="11508" class="Keyword">open</a> <a id="11513" class="Keyword">import</a> <a id="11520" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="11575" class="Keyword">open</a> <a id="11580" class="Keyword">import</a> <a id="11587" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="11627" class="Keyword">open</a> <a id="11632" class="Keyword">import</a> <a id="11639" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="11683" class="Keyword">open</a> <a id="11688" class="Keyword">import</a> <a id="11695" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="11740" class="Keyword">open</a> <a id="11745" class="Keyword">import</a> <a id="11752" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="11793" class="Keyword">open</a> <a id="11798" class="Keyword">import</a> <a id="11805" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="11845" class="Keyword">open</a> <a id="11850" class="Keyword">import</a> <a id="11857" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="11884" class="Keyword">open</a> <a id="11889" class="Keyword">import</a> <a id="11896" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="11923" class="Keyword">open</a> <a id="11928" class="Keyword">import</a> <a id="11935" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="11954" class="Keyword">open</a> <a id="11959" class="Keyword">import</a> <a id="11966" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="12006" class="Keyword">open</a> <a id="12011" class="Keyword">import</a> <a id="12018" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="12083" class="Keyword">open</a> <a id="12088" class="Keyword">import</a> <a id="12095" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="12118" class="Keyword">open</a> <a id="12123" class="Keyword">import</a> <a id="12130" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="12154" class="Keyword">open</a> <a id="12159" class="Keyword">import</a> <a id="12166" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="12206" class="Keyword">open</a> <a id="12211" class="Keyword">import</a> <a id="12218" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="12261" class="Keyword">open</a> <a id="12266" class="Keyword">import</a> <a id="12273" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="12307" class="Keyword">open</a> <a id="12312" class="Keyword">import</a> <a id="12319" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="12349" class="Keyword">open</a> <a id="12354" class="Keyword">import</a> <a id="12361" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="12395" class="Keyword">open</a> <a id="12400" class="Keyword">import</a> <a id="12407" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="12442" class="Keyword">open</a> <a id="12447" class="Keyword">import</a> <a id="12454" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="12491" class="Keyword">open</a> <a id="12496" class="Keyword">import</a> <a id="12503" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="12530" class="Keyword">open</a> <a id="12535" class="Keyword">import</a> <a id="12542" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="12591" class="Keyword">open</a> <a id="12596" class="Keyword">import</a> <a id="12603" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="12649" class="Keyword">open</a> <a id="12654" class="Keyword">import</a> <a id="12661" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="12701" class="Keyword">open</a> <a id="12706" class="Keyword">import</a> <a id="12713" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="12751" class="Keyword">open</a> <a id="12756" class="Keyword">import</a> <a id="12763" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="12792" class="Keyword">open</a> <a id="12797" class="Keyword">import</a> <a id="12804" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="12834" class="Keyword">open</a> <a id="12839" class="Keyword">import</a> <a id="12846" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="12877" class="Keyword">open</a> <a id="12882" class="Keyword">import</a> <a id="12889" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="12915" class="Keyword">open</a> <a id="12920" class="Keyword">import</a> <a id="12927" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="12978" class="Keyword">open</a> <a id="12983" class="Keyword">import</a> <a id="12990" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="13044" class="Keyword">open</a> <a id="13049" class="Keyword">import</a> <a id="13056" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="13083" class="Keyword">open</a> <a id="13088" class="Keyword">import</a> <a id="13095" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="13128" class="Keyword">open</a> <a id="13133" class="Keyword">import</a> <a id="13140" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="13171" class="Keyword">open</a> <a id="13176" class="Keyword">import</a> <a id="13183" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="13220" class="Keyword">open</a> <a id="13225" class="Keyword">import</a> <a id="13232" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="13264" class="Keyword">open</a> <a id="13269" class="Keyword">import</a> <a id="13276" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="13311" class="Keyword">open</a> <a id="13316" class="Keyword">import</a> <a id="13323" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="13352" class="Keyword">open</a> <a id="13357" class="Keyword">import</a> <a id="13364" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="13392" class="Keyword">open</a> <a id="13397" class="Keyword">import</a> <a id="13404" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="13429" class="Keyword">open</a> <a id="13434" class="Keyword">import</a> <a id="13441" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="13462" class="Keyword">open</a> <a id="13467" class="Keyword">import</a> <a id="13474" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="13510" class="Keyword">open</a> <a id="13515" class="Keyword">import</a> <a id="13522" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="13565" class="Keyword">open</a> <a id="13570" class="Keyword">import</a> <a id="13577" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="13602" class="Keyword">open</a> <a id="13607" class="Keyword">import</a> <a id="13614" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="13645" class="Keyword">open</a> <a id="13650" class="Keyword">import</a> <a id="13657" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="13689" class="Keyword">open</a> <a id="13694" class="Keyword">import</a> <a id="13701" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="13735" class="Keyword">open</a> <a id="13740" class="Keyword">import</a> <a id="13747" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="13803" class="Keyword">open</a> <a id="13808" class="Keyword">import</a> <a id="13815" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="13868" class="Keyword">open</a> <a id="13873" class="Keyword">import</a> <a id="13880" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="13907" class="Keyword">open</a> <a id="13912" class="Keyword">import</a> <a id="13919" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="13981" class="Keyword">open</a> <a id="13986" class="Keyword">import</a> <a id="13993" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="14022" class="Keyword">open</a> <a id="14027" class="Keyword">import</a> <a id="14034" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="14061" class="Keyword">open</a> <a id="14066" class="Keyword">import</a> <a id="14073" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="14095" class="Keyword">open</a> <a id="14100" class="Keyword">import</a> <a id="14107" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="14137" class="Keyword">open</a> <a id="14142" class="Keyword">import</a> <a id="14149" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Groups 

<pre class="Agda"><a id="14205" class="Keyword">open</a> <a id="14210" class="Keyword">import</a> <a id="14217" href="groups.abstract-abelian-groups.html" class="Module">groups.abstract-abelian-groups</a>
<a id="14248" class="Keyword">open</a> <a id="14253" class="Keyword">import</a> <a id="14260" href="groups.abstract-abelian-subgroups.html" class="Module">groups.abstract-abelian-subgroups</a>
<a id="14294" class="Keyword">open</a> <a id="14299" class="Keyword">import</a> <a id="14306" href="groups.abstract-group-actions.html" class="Module">groups.abstract-group-actions</a>
<a id="14336" class="Keyword">open</a> <a id="14341" class="Keyword">import</a> <a id="14348" href="groups.abstract-group-torsors.html" class="Module">groups.abstract-group-torsors</a>
<a id="14378" class="Keyword">open</a> <a id="14383" class="Keyword">import</a> <a id="14390" href="groups.abstract-groups.html" class="Module">groups.abstract-groups</a>
<a id="14413" class="Keyword">open</a> <a id="14418" class="Keyword">import</a> <a id="14425" href="groups.abstract-subgroups.html" class="Module">groups.abstract-subgroups</a>
<a id="14451" class="Keyword">open</a> <a id="14456" class="Keyword">import</a> <a id="14463" href="groups.concrete-group-actions.html" class="Module">groups.concrete-group-actions</a>
<a id="14493" class="Keyword">open</a> <a id="14498" class="Keyword">import</a> <a id="14505" href="groups.concrete-groups.html" class="Module">groups.concrete-groups</a>
<a id="14528" class="Keyword">open</a> <a id="14533" class="Keyword">import</a> <a id="14540" href="groups.concrete-subgroups.html" class="Module">groups.concrete-subgroups</a>
<a id="14566" class="Keyword">open</a> <a id="14571" class="Keyword">import</a> <a id="14578" href="groups.examples-higher-groups.html" class="Module">groups.examples-higher-groups</a>
<a id="14608" class="Keyword">open</a> <a id="14613" class="Keyword">import</a> <a id="14620" href="groups.furstenberg-groups.html" class="Module">groups.furstenberg-groups</a>
<a id="14646" class="Keyword">open</a> <a id="14651" class="Keyword">import</a> <a id="14658" href="groups.higher-groups.html" class="Module">groups.higher-groups</a>
<a id="14679" class="Keyword">open</a> <a id="14684" class="Keyword">import</a> <a id="14691" href="groups.sheargroups.html" class="Module">groups.sheargroups</a>
</pre>
## Order theory

<pre class="Agda"><a id="14740" class="Keyword">open</a> <a id="14745" class="Keyword">import</a> <a id="14752" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="14779" class="Keyword">open</a> <a id="14784" class="Keyword">import</a> <a id="14791" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="14821" class="Keyword">open</a> <a id="14826" class="Keyword">import</a> <a id="14833" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="14869" class="Keyword">open</a> <a id="14874" class="Keyword">import</a> <a id="14881" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="14914" class="Keyword">open</a> <a id="14919" class="Keyword">import</a> <a id="14926" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="14946" class="Keyword">open</a> <a id="14951" class="Keyword">import</a> <a id="14958" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="15008" class="Keyword">open</a> <a id="15013" class="Keyword">import</a> <a id="15020" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Rings

<pre class="Agda"><a id="15072" class="Keyword">open</a> <a id="15077" class="Keyword">import</a> <a id="15084" href="rings.eisenstein-integers.html" class="Module">rings.eisenstein-integers</a>
<a id="15110" class="Keyword">open</a> <a id="15115" class="Keyword">import</a> <a id="15122" href="rings.gaussian-integers.html" class="Module">rings.gaussian-integers</a>
<a id="15146" class="Keyword">open</a> <a id="15151" class="Keyword">import</a> <a id="15158" href="rings.ideals.html" class="Module">rings.ideals</a>
<a id="15171" class="Keyword">open</a> <a id="15176" class="Keyword">import</a> <a id="15183" href="rings.localizations-rings.html" class="Module">rings.localizations-rings</a>
<a id="15209" class="Keyword">open</a> <a id="15214" class="Keyword">import</a> <a id="15221" href="rings.rings-with-properties.html" class="Module">rings.rings-with-properties</a>
<a id="15249" class="Keyword">open</a> <a id="15254" class="Keyword">import</a> <a id="15261" href="rings.rings.html" class="Module">rings.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="15316" class="Keyword">open</a> <a id="15321" class="Keyword">import</a> <a id="15328" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="15367" class="Keyword">open</a> <a id="15372" class="Keyword">import</a> <a id="15379" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="15417" class="Keyword">open</a> <a id="15422" class="Keyword">import</a> <a id="15429" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="15475" class="Keyword">open</a> <a id="15480" class="Keyword">import</a> <a id="15487" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="15524" class="Keyword">open</a> <a id="15529" class="Keyword">import</a> <a id="15536" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="15576" class="Keyword">open</a> <a id="15581" class="Keyword">import</a> <a id="15588" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="15627" class="Keyword">open</a> <a id="15632" class="Keyword">import</a> <a id="15639" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="15672" class="Keyword">open</a> <a id="15677" class="Keyword">import</a> <a id="15684" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="15723" class="Keyword">open</a> <a id="15728" class="Keyword">import</a> <a id="15735" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="15783" class="Keyword">open</a> <a id="15788" class="Keyword">import</a> <a id="15795" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="15835" class="Keyword">open</a> <a id="15840" class="Keyword">import</a> <a id="15847" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="15901" class="Keyword">open</a> <a id="15906" class="Keyword">import</a> <a id="15913" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="15960" class="Keyword">open</a> <a id="15965" class="Keyword">import</a> <a id="15972" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="16024" class="Keyword">open</a> <a id="16029" class="Keyword">import</a> <a id="16036" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="16081" class="Keyword">open</a> <a id="16086" class="Keyword">import</a> <a id="16093" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="16132" class="Keyword">open</a> <a id="16137" class="Keyword">import</a> <a id="16144" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="16184" class="Keyword">open</a> <a id="16189" class="Keyword">import</a> <a id="16196" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="16229" class="Keyword">open</a> <a id="16234" class="Keyword">import</a> <a id="16241" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="16331" class="Keyword">open</a> <a id="16336" class="Keyword">import</a> <a id="16343" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="16383" class="Keyword">open</a> <a id="16388" class="Keyword">import</a> <a id="16395" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="16434" class="Keyword">open</a> <a id="16439" class="Keyword">import</a> <a id="16446" href="univalent-combinatorics.cartesian-product-finite-types.html" class="Module">univalent-combinatorics.cartesian-product-finite-types</a>
<a id="16501" class="Keyword">open</a> <a id="16506" class="Keyword">import</a> <a id="16513" href="univalent-combinatorics.coproduct-finite-types.html" class="Module">univalent-combinatorics.coproduct-finite-types</a>
<a id="16560" class="Keyword">open</a> <a id="16565" class="Keyword">import</a> <a id="16572" href="univalent-combinatorics.counting-cartesian-product-types.html" class="Module">univalent-combinatorics.counting-cartesian-product-types</a>
<a id="16629" class="Keyword">open</a> <a id="16634" class="Keyword">import</a> <a id="16641" href="univalent-combinatorics.counting-coproduct-types.html" class="Module">univalent-combinatorics.counting-coproduct-types</a>
<a id="16690" class="Keyword">open</a> <a id="16695" class="Keyword">import</a> <a id="16702" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="16754" class="Keyword">open</a> <a id="16759" class="Keyword">import</a> <a id="16766" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="16824" class="Keyword">open</a> <a id="16829" class="Keyword">import</a> <a id="16836" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="16890" class="Keyword">open</a> <a id="16895" class="Keyword">import</a> <a id="16902" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="16950" class="Keyword">open</a> <a id="16955" class="Keyword">import</a> <a id="16962" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="17010" class="Keyword">open</a> <a id="17015" class="Keyword">import</a> <a id="17022" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="17061" class="Keyword">open</a> <a id="17066" class="Keyword">import</a> <a id="17073" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="17106" class="Keyword">open</a> <a id="17111" class="Keyword">import</a> <a id="17118" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="17177" class="Keyword">open</a> <a id="17182" class="Keyword">import</a> <a id="17189" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="17244" class="Keyword">open</a> <a id="17249" class="Keyword">import</a> <a id="17256" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="17299" class="Keyword">open</a> <a id="17304" class="Keyword">import</a> <a id="17311" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="17366" class="Keyword">open</a> <a id="17371" class="Keyword">import</a> <a id="17378" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="17429" class="Keyword">open</a> <a id="17434" class="Keyword">import</a> <a id="17441" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="17519" class="Keyword">open</a> <a id="17524" class="Keyword">import</a> <a id="17531" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="17571" class="Keyword">open</a> <a id="17576" class="Keyword">import</a> <a id="17583" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="17618" class="Keyword">open</a> <a id="17623" class="Keyword">import</a> <a id="17630" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="17687" class="Keyword">open</a> <a id="17692" class="Keyword">import</a> <a id="17699" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="17745" class="Keyword">open</a> <a id="17750" class="Keyword">import</a> <a id="17757" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="17812" class="Keyword">open</a> <a id="17817" class="Keyword">import</a> <a id="17824" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="17861" class="Keyword">open</a> <a id="17866" class="Keyword">import</a> <a id="17873" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="17932" class="Keyword">open</a> <a id="17937" class="Keyword">import</a> <a id="17944" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="18004" class="Keyword">open</a> <a id="18009" class="Keyword">import</a> <a id="18016" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="18054" class="Keyword">open</a> <a id="18059" class="Keyword">import</a> <a id="18066" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="18118" class="Keyword">open</a> <a id="18123" class="Keyword">import</a> <a id="18130" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="18176" class="Keyword">open</a> <a id="18181" class="Keyword">import</a> <a id="18188" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="18233" class="Keyword">open</a> <a id="18238" class="Keyword">import</a> <a id="18245" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="18282" class="Keyword">open</a> <a id="18287" class="Keyword">import</a> <a id="18294" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="18343" class="Keyword">open</a> <a id="18348" class="Keyword">import</a> <a id="18355" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="18393" class="Keyword">open</a> <a id="18398" class="Keyword">import</a> <a id="18405" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="18460" class="Keyword">open</a> <a id="18465" class="Keyword">import</a> <a id="18472" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="18511" class="Keyword">open</a> <a id="18516" class="Keyword">import</a> <a id="18523" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="18553" class="Keyword">open</a> <a id="18558" class="Keyword">import</a> <a id="18565" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="18595" class="Keyword">open</a> <a id="18600" class="Keyword">import</a> <a id="18607" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="18647" class="Keyword">open</a> <a id="18652" class="Keyword">import</a> <a id="18659" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="18704" class="Keyword">open</a> <a id="18709" class="Keyword">import</a> <a id="18716" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="18754" class="Keyword">open</a> <a id="18759" class="Keyword">import</a> <a id="18766" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="18815" class="Keyword">open</a> <a id="18820" class="Keyword">import</a> <a id="18827" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="18873" class="Keyword">open</a> <a id="18878" class="Keyword">import</a> <a id="18885" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="18933" class="Keyword">open</a> <a id="18938" class="Keyword">import</a> <a id="18945" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="19023" class="Keyword">open</a> <a id="19028" class="Keyword">import</a> <a id="19035" href="univalent-foundations.functoriality-loop-spaces.html" class="Module">univalent-foundations.functoriality-loop-spaces</a>
<a id="19083" class="Keyword">open</a> <a id="19088" class="Keyword">import</a> <a id="19095" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
<a id="19133" class="Keyword">open</a> <a id="19138" class="Keyword">import</a> <a id="19145" href="univalent-foundations.iterated-loop-spaces.html" class="Module">univalent-foundations.iterated-loop-spaces</a>
<a id="19188" class="Keyword">open</a> <a id="19193" class="Keyword">import</a> <a id="19200" href="univalent-foundations.loop-spaces.html" class="Module">univalent-foundations.loop-spaces</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

