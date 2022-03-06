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
<a id="6430" class="Keyword">open</a> <a id="6435" class="Keyword">import</a> <a id="6442" href="foundation.elementhood-relation-W-types.html" class="Module">foundation.elementhood-relation-W-types</a>
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
<a id="7130" class="Keyword">open</a> <a id="7135" class="Keyword">import</a> <a id="7142" href="foundation.extensional-W-types.html" class="Module">foundation.extensional-W-types</a>
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
<a id="8142" class="Keyword">open</a> <a id="8147" class="Keyword">import</a> <a id="8154" href="foundation.indexed-W-types.html" class="Module">foundation.indexed-W-types</a>
<a id="8181" class="Keyword">open</a> <a id="8186" class="Keyword">import</a> <a id="8193" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="8249" class="Keyword">open</a> <a id="8254" class="Keyword">import</a> <a id="8261" href="foundation.induction-W-types.html" class="Module">foundation.induction-W-types</a>
<a id="8290" class="Keyword">open</a> <a id="8295" class="Keyword">import</a> <a id="8302" href="foundation.inequality-W-types.html" class="Module">foundation.inequality-W-types</a>
<a id="8332" class="Keyword">open</a> <a id="8337" class="Keyword">import</a> <a id="8344" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="8370" class="Keyword">open</a> <a id="8375" class="Keyword">import</a> <a id="8382" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="8409" class="Keyword">open</a> <a id="8414" class="Keyword">import</a> <a id="8421" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="8444" class="Keyword">open</a> <a id="8449" class="Keyword">import</a> <a id="8456" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="8483" class="Keyword">open</a> <a id="8488" class="Keyword">import</a> <a id="8495" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="8527" class="Keyword">open</a> <a id="8532" class="Keyword">import</a> <a id="8539" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="8573" class="Keyword">open</a> <a id="8578" class="Keyword">import</a> <a id="8585" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="8625" class="Keyword">open</a> <a id="8630" class="Keyword">import</a> <a id="8637" href="foundation.lists.html" class="Module">foundation.lists</a>
<a id="8654" class="Keyword">open</a> <a id="8659" class="Keyword">import</a> <a id="8666" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="8697" class="Keyword">open</a> <a id="8702" class="Keyword">import</a> <a id="8709" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="8741" class="Keyword">open</a> <a id="8746" class="Keyword">import</a> <a id="8753" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="8770" class="Keyword">open</a> <a id="8775" class="Keyword">import</a> <a id="8782" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="8807" class="Keyword">open</a> <a id="8812" class="Keyword">import</a> <a id="8819" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="8848" class="Keyword">open</a> <a id="8853" class="Keyword">import</a> <a id="8860" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="8885" class="Keyword">open</a> <a id="8890" class="Keyword">import</a> <a id="8897" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="8918" class="Keyword">open</a> <a id="8923" class="Keyword">import</a> <a id="8930" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="8950" class="Keyword">open</a> <a id="8955" class="Keyword">import</a> <a id="8962" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="8996" class="Keyword">open</a> <a id="9001" class="Keyword">import</a> <a id="9008" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="9035" class="Keyword">open</a> <a id="9040" class="Keyword">import</a> <a id="9047" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="9082" class="Keyword">open</a> <a id="9087" class="Keyword">import</a> <a id="9094" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="9134" class="Keyword">open</a> <a id="9139" class="Keyword">import</a> <a id="9146" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="9176" class="Keyword">open</a> <a id="9181" class="Keyword">import</a> <a id="9188" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="9225" class="Keyword">open</a> <a id="9230" class="Keyword">import</a> <a id="9237" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="9261" class="Keyword">open</a> <a id="9266" class="Keyword">import</a> <a id="9273" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="9294" class="Keyword">open</a> <a id="9299" class="Keyword">import</a> <a id="9306" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="9341" class="Keyword">open</a> <a id="9346" class="Keyword">import</a> <a id="9353" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="9402" class="Keyword">open</a> <a id="9407" class="Keyword">import</a> <a id="9414" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="9437" class="Keyword">open</a> <a id="9442" class="Keyword">import</a> <a id="9449" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="9472" class="Keyword">open</a> <a id="9477" class="Keyword">import</a> <a id="9484" href="foundation.Russells-paradox.html" class="Module">foundation.Russells-paradox</a>
<a id="9512" class="Keyword">open</a> <a id="9517" class="Keyword">import</a> <a id="9524" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="9544" class="Keyword">open</a> <a id="9549" class="Keyword">import</a> <a id="9556" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="9587" class="Keyword">open</a> <a id="9592" class="Keyword">import</a> <a id="9599" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="9626" class="Keyword">open</a> <a id="9631" class="Keyword">import</a> <a id="9638" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="9654" class="Keyword">open</a> <a id="9659" class="Keyword">import</a> <a id="9666" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="9697" class="Keyword">open</a> <a id="9702" class="Keyword">import</a> <a id="9709" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="9726" class="Keyword">open</a> <a id="9731" class="Keyword">import</a> <a id="9738" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="9760" class="Keyword">open</a> <a id="9765" class="Keyword">import</a> <a id="9772" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="9799" class="Keyword">open</a> <a id="9804" class="Keyword">import</a> <a id="9811" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="9834" class="Keyword">open</a> <a id="9839" class="Keyword">import</a> <a id="9846" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="9873" class="Keyword">open</a> <a id="9878" class="Keyword">import</a> <a id="9885" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="9918" class="Keyword">open</a> <a id="9923" class="Keyword">import</a> <a id="9930" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="9970" class="Keyword">open</a> <a id="9975" class="Keyword">import</a> <a id="9982" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="10003" class="Keyword">open</a> <a id="10008" class="Keyword">import</a> <a id="10015" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="10044" class="Keyword">open</a> <a id="10049" class="Keyword">import</a> <a id="10056" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="10094" class="Keyword">open</a> <a id="10099" class="Keyword">import</a> <a id="10106" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="10126" class="Keyword">open</a> <a id="10131" class="Keyword">import</a> <a id="10138" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="10162" class="Keyword">open</a> <a id="10167" class="Keyword">import</a> <a id="10174" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="10201" class="Keyword">open</a> <a id="10206" class="Keyword">import</a> <a id="10213" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="10239" class="Keyword">open</a> <a id="10244" class="Keyword">import</a> <a id="10251" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="10278" class="Keyword">open</a> <a id="10283" class="Keyword">import</a> <a id="10290" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="10319" class="Keyword">open</a> <a id="10324" class="Keyword">import</a> <a id="10331" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="10382" class="Keyword">open</a> <a id="10387" class="Keyword">import</a> <a id="10394" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="10437" class="Keyword">open</a> <a id="10442" class="Keyword">import</a> <a id="10449" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="10497" class="Keyword">open</a> <a id="10502" class="Keyword">import</a> <a id="10509" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="10547" class="Keyword">open</a> <a id="10552" class="Keyword">import</a> <a id="10559" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="10596" class="Keyword">open</a> <a id="10601" class="Keyword">import</a> <a id="10608" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="10636" class="Keyword">open</a> <a id="10641" class="Keyword">import</a> <a id="10648" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="10684" class="Keyword">open</a> <a id="10689" class="Keyword">import</a> <a id="10696" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="10734" class="Keyword">open</a> <a id="10739" class="Keyword">import</a> <a id="10746" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="10767" class="Keyword">open</a> <a id="10772" class="Keyword">import</a> <a id="10779" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="10833" class="Keyword">open</a> <a id="10838" class="Keyword">import</a> <a id="10845" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="10867" class="Keyword">open</a> <a id="10872" class="Keyword">import</a> <a id="10879" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="10914" class="Keyword">open</a> <a id="10919" class="Keyword">import</a> <a id="10926" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="10965" class="Keyword">open</a> <a id="10970" class="Keyword">import</a> <a id="10977" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="11031" class="Keyword">open</a> <a id="11036" class="Keyword">import</a> <a id="11043" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="11089" class="Keyword">open</a> <a id="11094" class="Keyword">import</a> <a id="11101" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="11152" class="Keyword">open</a> <a id="11157" class="Keyword">import</a> <a id="11164" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="11205" class="Keyword">open</a> <a id="11210" class="Keyword">import</a> <a id="11217" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="11262" class="Keyword">open</a> <a id="11267" class="Keyword">import</a> <a id="11274" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="11319" class="Keyword">open</a> <a id="11324" class="Keyword">import</a> <a id="11331" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="11367" class="Keyword">open</a> <a id="11372" class="Keyword">import</a> <a id="11379" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="11415" class="Keyword">open</a> <a id="11420" class="Keyword">import</a> <a id="11427" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="11492" class="Keyword">open</a> <a id="11497" class="Keyword">import</a> <a id="11504" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="11559" class="Keyword">open</a> <a id="11564" class="Keyword">import</a> <a id="11571" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="11611" class="Keyword">open</a> <a id="11616" class="Keyword">import</a> <a id="11623" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="11667" class="Keyword">open</a> <a id="11672" class="Keyword">import</a> <a id="11679" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="11724" class="Keyword">open</a> <a id="11729" class="Keyword">import</a> <a id="11736" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="11776" class="Keyword">open</a> <a id="11781" class="Keyword">import</a> <a id="11788" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="11815" class="Keyword">open</a> <a id="11820" class="Keyword">import</a> <a id="11827" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="11854" class="Keyword">open</a> <a id="11859" class="Keyword">import</a> <a id="11866" href="foundation.W-types.html" class="Module">foundation.W-types</a>
<a id="11885" class="Keyword">open</a> <a id="11890" class="Keyword">import</a> <a id="11897" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="11937" class="Keyword">open</a> <a id="11942" class="Keyword">import</a> <a id="11949" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="12014" class="Keyword">open</a> <a id="12019" class="Keyword">import</a> <a id="12026" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="12049" class="Keyword">open</a> <a id="12054" class="Keyword">import</a> <a id="12061" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="12085" class="Keyword">open</a> <a id="12090" class="Keyword">import</a> <a id="12097" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="12137" class="Keyword">open</a> <a id="12142" class="Keyword">import</a> <a id="12149" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="12192" class="Keyword">open</a> <a id="12197" class="Keyword">import</a> <a id="12204" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="12238" class="Keyword">open</a> <a id="12243" class="Keyword">import</a> <a id="12250" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="12280" class="Keyword">open</a> <a id="12285" class="Keyword">import</a> <a id="12292" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="12326" class="Keyword">open</a> <a id="12331" class="Keyword">import</a> <a id="12338" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="12373" class="Keyword">open</a> <a id="12378" class="Keyword">import</a> <a id="12385" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="12422" class="Keyword">open</a> <a id="12427" class="Keyword">import</a> <a id="12434" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="12461" class="Keyword">open</a> <a id="12466" class="Keyword">import</a> <a id="12473" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="12522" class="Keyword">open</a> <a id="12527" class="Keyword">import</a> <a id="12534" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="12580" class="Keyword">open</a> <a id="12585" class="Keyword">import</a> <a id="12592" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="12632" class="Keyword">open</a> <a id="12637" class="Keyword">import</a> <a id="12644" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="12682" class="Keyword">open</a> <a id="12687" class="Keyword">import</a> <a id="12694" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="12723" class="Keyword">open</a> <a id="12728" class="Keyword">import</a> <a id="12735" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="12765" class="Keyword">open</a> <a id="12770" class="Keyword">import</a> <a id="12777" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="12808" class="Keyword">open</a> <a id="12813" class="Keyword">import</a> <a id="12820" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="12846" class="Keyword">open</a> <a id="12851" class="Keyword">import</a> <a id="12858" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="12909" class="Keyword">open</a> <a id="12914" class="Keyword">import</a> <a id="12921" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="12975" class="Keyword">open</a> <a id="12980" class="Keyword">import</a> <a id="12987" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="13014" class="Keyword">open</a> <a id="13019" class="Keyword">import</a> <a id="13026" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="13059" class="Keyword">open</a> <a id="13064" class="Keyword">import</a> <a id="13071" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="13102" class="Keyword">open</a> <a id="13107" class="Keyword">import</a> <a id="13114" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="13151" class="Keyword">open</a> <a id="13156" class="Keyword">import</a> <a id="13163" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="13195" class="Keyword">open</a> <a id="13200" class="Keyword">import</a> <a id="13207" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="13242" class="Keyword">open</a> <a id="13247" class="Keyword">import</a> <a id="13254" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="13283" class="Keyword">open</a> <a id="13288" class="Keyword">import</a> <a id="13295" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="13323" class="Keyword">open</a> <a id="13328" class="Keyword">import</a> <a id="13335" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="13360" class="Keyword">open</a> <a id="13365" class="Keyword">import</a> <a id="13372" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="13393" class="Keyword">open</a> <a id="13398" class="Keyword">import</a> <a id="13405" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="13441" class="Keyword">open</a> <a id="13446" class="Keyword">import</a> <a id="13453" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="13496" class="Keyword">open</a> <a id="13501" class="Keyword">import</a> <a id="13508" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="13533" class="Keyword">open</a> <a id="13538" class="Keyword">import</a> <a id="13545" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="13576" class="Keyword">open</a> <a id="13581" class="Keyword">import</a> <a id="13588" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="13620" class="Keyword">open</a> <a id="13625" class="Keyword">import</a> <a id="13632" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="13666" class="Keyword">open</a> <a id="13671" class="Keyword">import</a> <a id="13678" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="13734" class="Keyword">open</a> <a id="13739" class="Keyword">import</a> <a id="13746" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="13799" class="Keyword">open</a> <a id="13804" class="Keyword">import</a> <a id="13811" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="13838" class="Keyword">open</a> <a id="13843" class="Keyword">import</a> <a id="13850" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="13912" class="Keyword">open</a> <a id="13917" class="Keyword">import</a> <a id="13924" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="13953" class="Keyword">open</a> <a id="13958" class="Keyword">import</a> <a id="13965" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="13992" class="Keyword">open</a> <a id="13997" class="Keyword">import</a> <a id="14004" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="14026" class="Keyword">open</a> <a id="14031" class="Keyword">import</a> <a id="14038" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="14068" class="Keyword">open</a> <a id="14073" class="Keyword">import</a> <a id="14080" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Groups 

<pre class="Agda"><a id="14136" class="Keyword">open</a> <a id="14141" class="Keyword">import</a> <a id="14148" href="groups.abstract-abelian-groups.html" class="Module">groups.abstract-abelian-groups</a>
<a id="14179" class="Keyword">open</a> <a id="14184" class="Keyword">import</a> <a id="14191" href="groups.abstract-abelian-subgroups.html" class="Module">groups.abstract-abelian-subgroups</a>
<a id="14225" class="Keyword">open</a> <a id="14230" class="Keyword">import</a> <a id="14237" href="groups.abstract-group-actions.html" class="Module">groups.abstract-group-actions</a>
<a id="14267" class="Keyword">open</a> <a id="14272" class="Keyword">import</a> <a id="14279" href="groups.abstract-group-torsors.html" class="Module">groups.abstract-group-torsors</a>
<a id="14309" class="Keyword">open</a> <a id="14314" class="Keyword">import</a> <a id="14321" href="groups.abstract-groups.html" class="Module">groups.abstract-groups</a>
<a id="14344" class="Keyword">open</a> <a id="14349" class="Keyword">import</a> <a id="14356" href="groups.abstract-subgroups.html" class="Module">groups.abstract-subgroups</a>
<a id="14382" class="Keyword">open</a> <a id="14387" class="Keyword">import</a> <a id="14394" href="groups.concrete-group-actions.html" class="Module">groups.concrete-group-actions</a>
<a id="14424" class="Keyword">open</a> <a id="14429" class="Keyword">import</a> <a id="14436" href="groups.concrete-groups.html" class="Module">groups.concrete-groups</a>
<a id="14459" class="Keyword">open</a> <a id="14464" class="Keyword">import</a> <a id="14471" href="groups.concrete-subgroups.html" class="Module">groups.concrete-subgroups</a>
<a id="14497" class="Keyword">open</a> <a id="14502" class="Keyword">import</a> <a id="14509" href="groups.examples-higher-groups.html" class="Module">groups.examples-higher-groups</a>
<a id="14539" class="Keyword">open</a> <a id="14544" class="Keyword">import</a> <a id="14551" href="groups.furstenberg-groups.html" class="Module">groups.furstenberg-groups</a>
<a id="14577" class="Keyword">open</a> <a id="14582" class="Keyword">import</a> <a id="14589" href="groups.higher-groups.html" class="Module">groups.higher-groups</a>
<a id="14610" class="Keyword">open</a> <a id="14615" class="Keyword">import</a> <a id="14622" href="groups.sheargroups.html" class="Module">groups.sheargroups</a>
</pre>
## Order theory

<pre class="Agda"><a id="14671" class="Keyword">open</a> <a id="14676" class="Keyword">import</a> <a id="14683" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="14710" class="Keyword">open</a> <a id="14715" class="Keyword">import</a> <a id="14722" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="14752" class="Keyword">open</a> <a id="14757" class="Keyword">import</a> <a id="14764" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="14800" class="Keyword">open</a> <a id="14805" class="Keyword">import</a> <a id="14812" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="14845" class="Keyword">open</a> <a id="14850" class="Keyword">import</a> <a id="14857" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="14877" class="Keyword">open</a> <a id="14882" class="Keyword">import</a> <a id="14889" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="14939" class="Keyword">open</a> <a id="14944" class="Keyword">import</a> <a id="14951" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Rings

<pre class="Agda"><a id="15003" class="Keyword">open</a> <a id="15008" class="Keyword">import</a> <a id="15015" href="rings.eisenstein-integers.html" class="Module">rings.eisenstein-integers</a>
<a id="15041" class="Keyword">open</a> <a id="15046" class="Keyword">import</a> <a id="15053" href="rings.gaussian-integers.html" class="Module">rings.gaussian-integers</a>
<a id="15077" class="Keyword">open</a> <a id="15082" class="Keyword">import</a> <a id="15089" href="rings.ideals.html" class="Module">rings.ideals</a>
<a id="15102" class="Keyword">open</a> <a id="15107" class="Keyword">import</a> <a id="15114" href="rings.localizations-rings.html" class="Module">rings.localizations-rings</a>
<a id="15140" class="Keyword">open</a> <a id="15145" class="Keyword">import</a> <a id="15152" href="rings.rings-with-properties.html" class="Module">rings.rings-with-properties</a>
<a id="15180" class="Keyword">open</a> <a id="15185" class="Keyword">import</a> <a id="15192" href="rings.rings.html" class="Module">rings.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="15247" class="Keyword">open</a> <a id="15252" class="Keyword">import</a> <a id="15259" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="15298" class="Keyword">open</a> <a id="15303" class="Keyword">import</a> <a id="15310" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="15348" class="Keyword">open</a> <a id="15353" class="Keyword">import</a> <a id="15360" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="15406" class="Keyword">open</a> <a id="15411" class="Keyword">import</a> <a id="15418" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="15455" class="Keyword">open</a> <a id="15460" class="Keyword">import</a> <a id="15467" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="15507" class="Keyword">open</a> <a id="15512" class="Keyword">import</a> <a id="15519" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="15558" class="Keyword">open</a> <a id="15563" class="Keyword">import</a> <a id="15570" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="15603" class="Keyword">open</a> <a id="15608" class="Keyword">import</a> <a id="15615" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="15654" class="Keyword">open</a> <a id="15659" class="Keyword">import</a> <a id="15666" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="15714" class="Keyword">open</a> <a id="15719" class="Keyword">import</a> <a id="15726" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="15766" class="Keyword">open</a> <a id="15771" class="Keyword">import</a> <a id="15778" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="15811" class="Keyword">open</a> <a id="15816" class="Keyword">import</a> <a id="15823" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="15913" class="Keyword">open</a> <a id="15918" class="Keyword">import</a> <a id="15925" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="15965" class="Keyword">open</a> <a id="15970" class="Keyword">import</a> <a id="15977" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="16016" class="Keyword">open</a> <a id="16021" class="Keyword">import</a> <a id="16028" href="univalent-combinatorics.cartesian-product-finite-types.html" class="Module">univalent-combinatorics.cartesian-product-finite-types</a>
<a id="16083" class="Keyword">open</a> <a id="16088" class="Keyword">import</a> <a id="16095" href="univalent-combinatorics.coproduct-finite-types.html" class="Module">univalent-combinatorics.coproduct-finite-types</a>
<a id="16142" class="Keyword">open</a> <a id="16147" class="Keyword">import</a> <a id="16154" href="univalent-combinatorics.counting-cartesian-product-types.html" class="Module">univalent-combinatorics.counting-cartesian-product-types</a>
<a id="16211" class="Keyword">open</a> <a id="16216" class="Keyword">import</a> <a id="16223" href="univalent-combinatorics.counting-coproduct-types.html" class="Module">univalent-combinatorics.counting-coproduct-types</a>
<a id="16272" class="Keyword">open</a> <a id="16277" class="Keyword">import</a> <a id="16284" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="16336" class="Keyword">open</a> <a id="16341" class="Keyword">import</a> <a id="16348" href="univalent-combinatorics.counting-dependent-function-types.html" class="Module">univalent-combinatorics.counting-dependent-function-types</a>
<a id="16406" class="Keyword">open</a> <a id="16411" class="Keyword">import</a> <a id="16418" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="16472" class="Keyword">open</a> <a id="16477" class="Keyword">import</a> <a id="16484" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="16532" class="Keyword">open</a> <a id="16537" class="Keyword">import</a> <a id="16544" href="univalent-combinatorics.counting-function-types.html" class="Module">univalent-combinatorics.counting-function-types</a>
<a id="16592" class="Keyword">open</a> <a id="16597" class="Keyword">import</a> <a id="16604" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="16643" class="Keyword">open</a> <a id="16648" class="Keyword">import</a> <a id="16655" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="16688" class="Keyword">open</a> <a id="16693" class="Keyword">import</a> <a id="16700" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="16759" class="Keyword">open</a> <a id="16764" class="Keyword">import</a> <a id="16771" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="16826" class="Keyword">open</a> <a id="16831" class="Keyword">import</a> <a id="16838" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="16881" class="Keyword">open</a> <a id="16886" class="Keyword">import</a> <a id="16893" href="univalent-combinatorics.dependent-product-finite-types.html" class="Module">univalent-combinatorics.dependent-product-finite-types</a>
<a id="16948" class="Keyword">open</a> <a id="16953" class="Keyword">import</a> <a id="16960" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="17011" class="Keyword">open</a> <a id="17016" class="Keyword">import</a> <a id="17023" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="17101" class="Keyword">open</a> <a id="17106" class="Keyword">import</a> <a id="17113" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="17153" class="Keyword">open</a> <a id="17158" class="Keyword">import</a> <a id="17165" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="17200" class="Keyword">open</a> <a id="17205" class="Keyword">import</a> <a id="17212" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="17269" class="Keyword">open</a> <a id="17274" class="Keyword">import</a> <a id="17281" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="17327" class="Keyword">open</a> <a id="17332" class="Keyword">import</a> <a id="17339" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="17394" class="Keyword">open</a> <a id="17399" class="Keyword">import</a> <a id="17406" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="17443" class="Keyword">open</a> <a id="17448" class="Keyword">import</a> <a id="17455" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="17514" class="Keyword">open</a> <a id="17519" class="Keyword">import</a> <a id="17526" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a>
<a id="17586" class="Keyword">open</a> <a id="17591" class="Keyword">import</a> <a id="17598" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="17636" class="Keyword">open</a> <a id="17641" class="Keyword">import</a> <a id="17648" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="17700" class="Keyword">open</a> <a id="17705" class="Keyword">import</a> <a id="17712" href="univalent-combinatorics.finite-function-types.html" class="Module">univalent-combinatorics.finite-function-types</a>
<a id="17758" class="Keyword">open</a> <a id="17763" class="Keyword">import</a> <a id="17770" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="17815" class="Keyword">open</a> <a id="17820" class="Keyword">import</a> <a id="17827" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="17864" class="Keyword">open</a> <a id="17869" class="Keyword">import</a> <a id="17876" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="17925" class="Keyword">open</a> <a id="17930" class="Keyword">import</a> <a id="17937" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="17975" class="Keyword">open</a> <a id="17980" class="Keyword">import</a> <a id="17987" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="18042" class="Keyword">open</a> <a id="18047" class="Keyword">import</a> <a id="18054" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="18093" class="Keyword">open</a> <a id="18098" class="Keyword">import</a> <a id="18105" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="18135" class="Keyword">open</a> <a id="18140" class="Keyword">import</a> <a id="18147" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="18187" class="Keyword">open</a> <a id="18192" class="Keyword">import</a> <a id="18199" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="18244" class="Keyword">open</a> <a id="18249" class="Keyword">import</a> <a id="18256" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="18294" class="Keyword">open</a> <a id="18299" class="Keyword">import</a> <a id="18306" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="18355" class="Keyword">open</a> <a id="18360" class="Keyword">import</a> <a id="18367" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="18413" class="Keyword">open</a> <a id="18418" class="Keyword">import</a> <a id="18425" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="18473" class="Keyword">open</a> <a id="18478" class="Keyword">import</a> <a id="18485" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Univalent foundation

<pre class="Agda"><a id="18563" class="Keyword">open</a> <a id="18568" class="Keyword">import</a> <a id="18575" href="univalent-foundations.functoriality-loop-spaces.html" class="Module">univalent-foundations.functoriality-loop-spaces</a>
<a id="18623" class="Keyword">open</a> <a id="18628" class="Keyword">import</a> <a id="18635" href="univalent-foundations.isolated-points.html" class="Module">univalent-foundations.isolated-points</a>
<a id="18673" class="Keyword">open</a> <a id="18678" class="Keyword">import</a> <a id="18685" href="univalent-foundations.iterated-loop-spaces.html" class="Module">univalent-foundations.iterated-loop-spaces</a>
<a id="18728" class="Keyword">open</a> <a id="18733" class="Keyword">import</a> <a id="18740" href="univalent-foundations.loop-spaces.html" class="Module">univalent-foundations.loop-spaces</a>
<a id="18774" class="Keyword">open</a> <a id="18779" class="Keyword">import</a> <a id="18786" href="univalent-foundations.pointed-dependent-functions.html" class="Module">univalent-foundations.pointed-dependent-functions</a>
<a id="18836" class="Keyword">open</a> <a id="18841" class="Keyword">import</a> <a id="18848" href="univalent-foundations.pointed-equivalences.html" class="Module">univalent-foundations.pointed-equivalences</a>
<a id="18891" class="Keyword">open</a> <a id="18896" class="Keyword">import</a> <a id="18903" href="univalent-foundations.pointed-families-of-types.html" class="Module">univalent-foundations.pointed-families-of-types</a>
<a id="18951" class="Keyword">open</a> <a id="18956" class="Keyword">import</a> <a id="18963" href="univalent-foundations.pointed-homotopies.html" class="Module">univalent-foundations.pointed-homotopies</a>
<a id="19004" class="Keyword">open</a> <a id="19009" class="Keyword">import</a> <a id="19016" href="univalent-foundations.pointed-maps.html" class="Module">univalent-foundations.pointed-maps</a>
<a id="19051" class="Keyword">open</a> <a id="19056" class="Keyword">import</a> <a id="19063" href="univalent-foundations.pointed-types.html" class="Module">univalent-foundations.pointed-types</a>
<a id="19099" class="Keyword">open</a> <a id="19104" class="Keyword">import</a> <a id="19111" href="univalent-foundations.truncations.html" class="Module">univalent-foundations.truncations</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

