---
title: Univalent mathematics in Agda
---

Welcome to the website of the `agda-unimath` formalization project.

[![CI](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml/badge.svg)](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml) [![pages-build-deployment](https://github.com/UniMath/agda-unimath/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/UniMath/agda-unimath/actions/workflows/pages/pages-build-deployment)

The `agda-unimath` library is a new formalisation project for univalent mathematics in Agda. Our goal is to formalize an extensive curriculum of mathematics from the univalent point of view. Furthermore, we think libraries of formalized mathematics have the potential to be useful, and informative resources for mathematicians. Our library is designed to work towards this goal, and we welcome contributions to the library about any topic in mathematics.

The library is built in Agda 2.6.2. It can be compiled by running `make check` from the main folder of the repository.

## Joining the project

Great, you want to contribute something! The best way to start is to find us in our chat channels on the [agda-unimath discord](https://discord.gg/Zp2e8hYsuX). We have a vibing community there, and you're more than welcome to join us just to hang out.

Once you've decided what you want to contribute, the best way to proceed is to make your own fork of the library. Within your fork, make a separate branch in which you will be making your contributions. Now you're ready to start your project! When you've completed your formalization you can proceed by making a pull request. Then we will review your contributions, and merge it when it is ready for the `agda-unimath` library.

## Statement of inclusion

There are many reasons to contribute something to a library of formalized mathematics. Some do it just for fun, some do it for their research, some do it to learn something. Whatever your reason is, we welcome your contributions! To keep the experience of contributing something to our library enjoyable for everyone, we strive for an inclusive community of contributors. You can expect from us that we are kind and respectful in discussions, that we will be mindful of your pronouns and use [inclusive language](https://www.apa.org/about/apa/equity-diversity-inclusion/language-guidelines), and that we value your input regardless of your level of experience or status in the community. We're commited to providing a safe and welcoming environment to people of any gender identity, sexual orientation, race, colour, age, ability, ethnicity, background, or fluency in English -- here on github, in online communication channels, and in person. Homotopy type theory is difficult enough without all the barriers that many of us have to face, so we hope to bring some of those down a bit.

:rainbow: Happy contributing!

Elisabeth Bonnevier  
Jonathan Prieto-Cubides  
Egbert Rijke

<pre class="Agda"><a id="2980" class="Symbol">{-#</a> <a id="2984" class="Keyword">OPTIONS</a> <a id="2992" class="Pragma">--without-K</a> <a id="3004" class="Pragma">--exact-split</a> <a id="3018" class="Pragma">--guardedness</a> <a id="3032" class="Symbol">#-}</a>
</pre>
See the list of all Agda modules [here](everything.html).

## Category theory

<pre class="Agda"><a id="3128" class="Keyword">open</a> <a id="3133" class="Keyword">import</a> <a id="3140" href="category-theory.html" class="Module">category-theory</a>
<a id="3156" class="Keyword">open</a> <a id="3161" class="Keyword">import</a> <a id="3168" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="3216" class="Keyword">open</a> <a id="3221" class="Keyword">import</a> <a id="3228" href="category-theory.anafunctors.html" class="Module">category-theory.anafunctors</a>
<a id="3256" class="Keyword">open</a> <a id="3261" class="Keyword">import</a> <a id="3268" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="3295" class="Keyword">open</a> <a id="3300" class="Keyword">import</a> <a id="3307" href="category-theory.epimorphisms-large-precategories.html" class="Module">category-theory.epimorphisms-large-precategories</a>
<a id="3356" class="Keyword">open</a> <a id="3361" class="Keyword">import</a> <a id="3368" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="3408" class="Keyword">open</a> <a id="3413" class="Keyword">import</a> <a id="3420" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="3469" class="Keyword">open</a> <a id="3474" class="Keyword">import</a> <a id="3481" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="3524" class="Keyword">open</a> <a id="3529" class="Keyword">import</a> <a id="3536" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="3572" class="Keyword">open</a> <a id="3577" class="Keyword">import</a> <a id="3584" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="3629" class="Keyword">open</a> <a id="3634" class="Keyword">import</a> <a id="3641" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="3680" class="Keyword">open</a> <a id="3685" class="Keyword">import</a> <a id="3692" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="3763" class="Keyword">open</a> <a id="3768" class="Keyword">import</a> <a id="3775" href="category-theory.initial-objects-precategories.html" class="Module">category-theory.initial-objects-precategories</a>
<a id="3821" class="Keyword">open</a> <a id="3826" class="Keyword">import</a> <a id="3833" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="3873" class="Keyword">open</a> <a id="3878" class="Keyword">import</a> <a id="3885" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="3934" class="Keyword">open</a> <a id="3939" class="Keyword">import</a> <a id="3946" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="3989" class="Keyword">open</a> <a id="3994" class="Keyword">import</a> <a id="4001" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="4034" class="Keyword">open</a> <a id="4039" class="Keyword">import</a> <a id="4046" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="4082" class="Keyword">open</a> <a id="4087" class="Keyword">import</a> <a id="4094" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="4144" class="Keyword">open</a> <a id="4149" class="Keyword">import</a> <a id="4156" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="4204" class="Keyword">open</a> <a id="4209" class="Keyword">import</a> <a id="4216" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="4273" class="Keyword">open</a> <a id="4278" class="Keyword">import</a> <a id="4285" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="4336" class="Keyword">open</a> <a id="4341" class="Keyword">import</a> <a id="4348" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="4399" class="Keyword">open</a> <a id="4404" class="Keyword">import</a> <a id="4411" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="4471" class="Keyword">open</a> <a id="4476" class="Keyword">import</a> <a id="4483" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="4537" class="Keyword">open</a> <a id="4542" class="Keyword">import</a> <a id="4549" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
<a id="4579" class="Keyword">open</a> <a id="4584" class="Keyword">import</a> <a id="4591" href="category-theory.slice-precategories.html" class="Module">category-theory.slice-precategories</a>
<a id="4627" class="Keyword">open</a> <a id="4632" class="Keyword">import</a> <a id="4639" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Commutative algebra

<pre class="Agda"><a id="4723" class="Keyword">open</a> <a id="4728" class="Keyword">import</a> <a id="4735" href="commutative-algebra.html" class="Module">commutative-algebra</a>
<a id="4755" class="Keyword">open</a> <a id="4760" class="Keyword">import</a> <a id="4767" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>
<a id="4805" class="Keyword">open</a> <a id="4810" class="Keyword">import</a> <a id="4817" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a>
<a id="4853" class="Keyword">open</a> <a id="4858" class="Keyword">import</a> <a id="4865" href="commutative-algebra.eisenstein-integers.html" class="Module">commutative-algebra.eisenstein-integers</a>
<a id="4905" class="Keyword">open</a> <a id="4910" class="Keyword">import</a> <a id="4917" href="commutative-algebra.gaussian-integers.html" class="Module">commutative-algebra.gaussian-integers</a>
<a id="4955" class="Keyword">open</a> <a id="4960" class="Keyword">import</a> <a id="4967" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a>
<a id="5019" class="Keyword">open</a> <a id="5024" class="Keyword">import</a> <a id="5031" href="commutative-algebra.ideals-commutative-rings.html" class="Module">commutative-algebra.ideals-commutative-rings</a>
<a id="5076" class="Keyword">open</a> <a id="5081" class="Keyword">import</a> <a id="5088" href="commutative-algebra.isomorphisms-commutative-rings.html" class="Module">commutative-algebra.isomorphisms-commutative-rings</a>
<a id="5139" class="Keyword">open</a> <a id="5144" class="Keyword">import</a> <a id="5151" href="commutative-algebra.prime-ideals-commutative-rings.html" class="Module">commutative-algebra.prime-ideals-commutative-rings</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="5244" class="Keyword">open</a> <a id="5249" class="Keyword">import</a> <a id="5256" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5281" class="Keyword">open</a> <a id="5286" class="Keyword">import</a> <a id="5293" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5342" class="Keyword">open</a> <a id="5347" class="Keyword">import</a> <a id="5354" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5397" class="Keyword">open</a> <a id="5402" class="Keyword">import</a> <a id="5409" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5459" class="Keyword">open</a> <a id="5464" class="Keyword">import</a> <a id="5471" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5517" class="Keyword">open</a> <a id="5522" class="Keyword">import</a> <a id="5529" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5576" class="Keyword">open</a> <a id="5581" class="Keyword">import</a> <a id="5588" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5647" class="Keyword">open</a> <a id="5652" class="Keyword">import</a> <a id="5659" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="5700" class="Keyword">open</a> <a id="5705" class="Keyword">import</a> <a id="5712" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="5755" class="Keyword">open</a> <a id="5760" class="Keyword">import</a> <a id="5767" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="5811" class="Keyword">open</a> <a id="5816" class="Keyword">import</a> <a id="5823" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="5868" class="Keyword">open</a> <a id="5873" class="Keyword">import</a> <a id="5880" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="5932" class="Keyword">open</a> <a id="5937" class="Keyword">import</a> <a id="5944" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="6004" class="Keyword">open</a> <a id="6009" class="Keyword">import</a> <a id="6016" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="6057" class="Keyword">open</a> <a id="6062" class="Keyword">import</a> <a id="6069" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6114" class="Keyword">open</a> <a id="6119" class="Keyword">import</a> <a id="6126" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6173" class="Keyword">open</a> <a id="6178" class="Keyword">import</a> <a id="6185" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6228" class="Keyword">open</a> <a id="6233" class="Keyword">import</a> <a id="6240" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6290" class="Keyword">open</a> <a id="6295" class="Keyword">import</a> <a id="6302" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6349" class="Keyword">open</a> <a id="6354" class="Keyword">import</a> <a id="6361" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6418" class="Keyword">open</a> <a id="6423" class="Keyword">import</a> <a id="6430" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6484" class="Keyword">open</a> <a id="6489" class="Keyword">import</a> <a id="6496" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6556" class="Keyword">open</a> <a id="6561" class="Keyword">import</a> <a id="6568" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6611" class="Keyword">open</a> <a id="6616" class="Keyword">import</a> <a id="6623" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="6673" class="Keyword">open</a> <a id="6678" class="Keyword">import</a> <a id="6685" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="6745" class="Keyword">open</a> <a id="6750" class="Keyword">import</a> <a id="6757" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="6806" class="Keyword">open</a> <a id="6811" class="Keyword">import</a> <a id="6818" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="6874" class="Keyword">open</a> <a id="6879" class="Keyword">import</a> <a id="6886" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="6922" class="Keyword">open</a> <a id="6927" class="Keyword">import</a> <a id="6934" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="6978" class="Keyword">open</a> <a id="6983" class="Keyword">import</a> <a id="6990" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="7034" class="Keyword">open</a> <a id="7039" class="Keyword">import</a> <a id="7046" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7096" class="Keyword">open</a> <a id="7101" class="Keyword">import</a> <a id="7108" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7154" class="Keyword">open</a> <a id="7159" class="Keyword">import</a> <a id="7166" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7201" class="Keyword">open</a> <a id="7206" class="Keyword">import</a> <a id="7213" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7258" class="Keyword">open</a> <a id="7263" class="Keyword">import</a> <a id="7270" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7328" class="Keyword">open</a> <a id="7333" class="Keyword">import</a> <a id="7340" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7405" class="Keyword">open</a> <a id="7410" class="Keyword">import</a> <a id="7417" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7460" class="Keyword">open</a> <a id="7465" class="Keyword">import</a> <a id="7472" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7526" class="Keyword">open</a> <a id="7531" class="Keyword">import</a> <a id="7538" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7583" class="Keyword">open</a> <a id="7588" class="Keyword">import</a> <a id="7595" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7647" class="Keyword">open</a> <a id="7652" class="Keyword">import</a> <a id="7659" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7717" class="Keyword">open</a> <a id="7722" class="Keyword">import</a> <a id="7729" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="7775" class="Keyword">open</a> <a id="7780" class="Keyword">import</a> <a id="7787" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="7831" class="Keyword">open</a> <a id="7836" class="Keyword">import</a> <a id="7843" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="7877" class="Keyword">open</a> <a id="7882" class="Keyword">import</a> <a id="7889" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="7943" class="Keyword">open</a> <a id="7948" class="Keyword">import</a> <a id="7955" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="8004" class="Keyword">open</a> <a id="8009" class="Keyword">import</a> <a id="8016" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="8057" class="Keyword">open</a> <a id="8062" class="Keyword">import</a> <a id="8069" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8118" class="Keyword">open</a> <a id="8123" class="Keyword">import</a> <a id="8130" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8196" class="Keyword">open</a> <a id="8201" class="Keyword">import</a> <a id="8208" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8252" class="Keyword">open</a> <a id="8257" class="Keyword">import</a> <a id="8264" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8313" class="Keyword">open</a> <a id="8318" class="Keyword">import</a> <a id="8325" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8381" class="Keyword">open</a> <a id="8386" class="Keyword">import</a> <a id="8393" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8434" class="Keyword">open</a> <a id="8439" class="Keyword">import</a> <a id="8446" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8495" class="Keyword">open</a> <a id="8500" class="Keyword">import</a> <a id="8507" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8566" class="Keyword">open</a> <a id="8571" class="Keyword">import</a> <a id="8578" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8617" class="Keyword">open</a> <a id="8622" class="Keyword">import</a> <a id="8629" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8682" class="Keyword">open</a> <a id="8687" class="Keyword">import</a> <a id="8694" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="8751" class="Keyword">open</a> <a id="8756" class="Keyword">import</a> <a id="8763" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="8805" class="Keyword">open</a> <a id="8810" class="Keyword">import</a> <a id="8817" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="8868" class="Keyword">open</a> <a id="8873" class="Keyword">import</a> <a id="8880" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="8938" class="Keyword">open</a> <a id="8943" class="Keyword">import</a> <a id="8950" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9014" class="Keyword">open</a> <a id="9019" class="Keyword">import</a> <a id="9026" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9079" class="Keyword">open</a> <a id="9084" class="Keyword">import</a> <a id="9091" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9144" class="Keyword">open</a> <a id="9149" class="Keyword">import</a> <a id="9156" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9217" class="Keyword">open</a> <a id="9222" class="Keyword">import</a> <a id="9229" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9287" class="Keyword">open</a> <a id="9292" class="Keyword">import</a> <a id="9299" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9348" class="Keyword">open</a> <a id="9353" class="Keyword">import</a> <a id="9360" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9403" class="Keyword">open</a> <a id="9408" class="Keyword">import</a> <a id="9415" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9459" class="Keyword">open</a> <a id="9464" class="Keyword">import</a> <a id="9471" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9518" class="Keyword">open</a> <a id="9523" class="Keyword">import</a> <a id="9530" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9591" class="Keyword">open</a> <a id="9596" class="Keyword">import</a> <a id="9603" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9666" class="Keyword">open</a> <a id="9671" class="Keyword">import</a> <a id="9678" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="9738" class="Keyword">open</a> <a id="9743" class="Keyword">import</a> <a id="9750" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="9804" class="Keyword">open</a> <a id="9809" class="Keyword">import</a> <a id="9816" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="9881" class="Keyword">open</a> <a id="9886" class="Keyword">import</a> <a id="9893" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10001" class="Keyword">open</a> <a id="10006" class="Keyword">import</a> <a id="10013" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10033" class="Keyword">open</a> <a id="10038" class="Keyword">import</a> <a id="10045" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10091" class="Keyword">open</a> <a id="10096" class="Keyword">import</a> <a id="10103" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10149" class="Keyword">open</a> <a id="10154" class="Keyword">import</a> <a id="10161" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10195" class="Keyword">open</a> <a id="10200" class="Keyword">import</a> <a id="10207" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10242" class="Keyword">open</a> <a id="10247" class="Keyword">import</a> <a id="10254" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10292" class="Keyword">open</a> <a id="10297" class="Keyword">import</a> <a id="10304" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10342" class="Keyword">open</a> <a id="10347" class="Keyword">import</a> <a id="10354" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10394" class="Keyword">open</a> <a id="10399" class="Keyword">import</a> <a id="10406" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10439" class="Keyword">open</a> <a id="10444" class="Keyword">import</a> <a id="10451" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10489" class="Keyword">open</a> <a id="10494" class="Keyword">import</a> <a id="10501" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10564" class="Keyword">open</a> <a id="10569" class="Keyword">import</a> <a id="10576" href="foundation.html" class="Module">foundation</a>
<a id="10587" class="Keyword">open</a> <a id="10592" class="Keyword">import</a> <a id="10599" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10617" class="Keyword">open</a> <a id="10622" class="Keyword">import</a> <a id="10629" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10648" class="Keyword">open</a> <a id="10653" class="Keyword">import</a> <a id="10660" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10679" class="Keyword">open</a> <a id="10684" class="Keyword">import</a> <a id="10691" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="10735" class="Keyword">open</a> <a id="10740" class="Keyword">import</a> <a id="10747" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="10772" class="Keyword">open</a> <a id="10777" class="Keyword">import</a> <a id="10784" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="10811" class="Keyword">open</a> <a id="10816" class="Keyword">import</a> <a id="10823" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="10840" class="Keyword">open</a> <a id="10845" class="Keyword">import</a> <a id="10852" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="10881" class="Keyword">open</a> <a id="10886" class="Keyword">import</a> <a id="10893" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="10949" class="Keyword">open</a> <a id="10954" class="Keyword">import</a> <a id="10961" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="10992" class="Keyword">open</a> <a id="10997" class="Keyword">import</a> <a id="11004" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11058" class="Keyword">open</a> <a id="11063" class="Keyword">import</a> <a id="11070" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11098" class="Keyword">open</a> <a id="11103" class="Keyword">import</a> <a id="11110" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11140" class="Keyword">open</a> <a id="11145" class="Keyword">import</a> <a id="11152" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11172" class="Keyword">open</a> <a id="11177" class="Keyword">import</a> <a id="11184" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11229" class="Keyword">open</a> <a id="11234" class="Keyword">import</a> <a id="11241" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11278" class="Keyword">open</a> <a id="11283" class="Keyword">import</a> <a id="11290" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11325" class="Keyword">open</a> <a id="11330" class="Keyword">import</a> <a id="11337" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11395" class="Keyword">open</a> <a id="11400" class="Keyword">import</a> <a id="11407" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11445" class="Keyword">open</a> <a id="11450" class="Keyword">import</a> <a id="11457" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11491" class="Keyword">open</a> <a id="11496" class="Keyword">import</a> <a id="11503" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11532" class="Keyword">open</a> <a id="11537" class="Keyword">import</a> <a id="11544" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11567" class="Keyword">open</a> <a id="11572" class="Keyword">import</a> <a id="11579" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="11606" class="Keyword">open</a> <a id="11611" class="Keyword">import</a> <a id="11618" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11641" class="Keyword">open</a> <a id="11646" class="Keyword">import</a> <a id="11653" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="11695" class="Keyword">open</a> <a id="11700" class="Keyword">import</a> <a id="11707" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="11739" class="Keyword">open</a> <a id="11744" class="Keyword">import</a> <a id="11751" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="11778" class="Keyword">open</a> <a id="11783" class="Keyword">import</a> <a id="11790" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="11815" class="Keyword">open</a> <a id="11820" class="Keyword">import</a> <a id="11827" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="11856" class="Keyword">open</a> <a id="11861" class="Keyword">import</a> <a id="11868" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="11898" class="Keyword">open</a> <a id="11903" class="Keyword">import</a> <a id="11910" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="11937" class="Keyword">open</a> <a id="11942" class="Keyword">import</a> <a id="11949" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="11968" class="Keyword">open</a> <a id="11973" class="Keyword">import</a> <a id="11980" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12026" class="Keyword">open</a> <a id="12031" class="Keyword">import</a> <a id="12038" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12080" class="Keyword">open</a> <a id="12085" class="Keyword">import</a> <a id="12092" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12124" class="Keyword">open</a> <a id="12129" class="Keyword">import</a> <a id="12136" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12166" class="Keyword">open</a> <a id="12171" class="Keyword">import</a> <a id="12178" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12204" class="Keyword">open</a> <a id="12209" class="Keyword">import</a> <a id="12216" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12250" class="Keyword">open</a> <a id="12255" class="Keyword">import</a> <a id="12262" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12292" class="Keyword">open</a> <a id="12297" class="Keyword">import</a> <a id="12304" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12331" class="Keyword">open</a> <a id="12336" class="Keyword">import</a> <a id="12343" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12375" class="Keyword">open</a> <a id="12380" class="Keyword">import</a> <a id="12387" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12421" class="Keyword">open</a> <a id="12426" class="Keyword">import</a> <a id="12433" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12456" class="Keyword">open</a> <a id="12461" class="Keyword">import</a> <a id="12468" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="12538" class="Keyword">open</a> <a id="12543" class="Keyword">import</a> <a id="12550" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="12620" class="Keyword">open</a> <a id="12625" class="Keyword">import</a> <a id="12632" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12659" class="Keyword">open</a> <a id="12664" class="Keyword">import</a> <a id="12671" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12699" class="Keyword">open</a> <a id="12704" class="Keyword">import</a> <a id="12711" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12748" class="Keyword">open</a> <a id="12753" class="Keyword">import</a> <a id="12760" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12808" class="Keyword">open</a> <a id="12813" class="Keyword">import</a> <a id="12820" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="12860" class="Keyword">open</a> <a id="12865" class="Keyword">import</a> <a id="12872" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="12894" class="Keyword">open</a> <a id="12899" class="Keyword">import</a> <a id="12906" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="12929" class="Keyword">open</a> <a id="12934" class="Keyword">import</a> <a id="12941" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="12966" class="Keyword">open</a> <a id="12971" class="Keyword">import</a> <a id="12978" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13023" class="Keyword">open</a> <a id="13028" class="Keyword">import</a> <a id="13035" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13079" class="Keyword">open</a> <a id="13084" class="Keyword">import</a> <a id="13091" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13127" class="Keyword">open</a> <a id="13132" class="Keyword">import</a> <a id="13139" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13184" class="Keyword">open</a> <a id="13189" class="Keyword">import</a> <a id="13196" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13237" class="Keyword">open</a> <a id="13242" class="Keyword">import</a> <a id="13249" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13284" class="Keyword">open</a> <a id="13289" class="Keyword">import</a> <a id="13296" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13327" class="Keyword">open</a> <a id="13332" class="Keyword">import</a> <a id="13339" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13372" class="Keyword">open</a> <a id="13377" class="Keyword">import</a> <a id="13384" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13417" class="Keyword">open</a> <a id="13422" class="Keyword">import</a> <a id="13429" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13459" class="Keyword">open</a> <a id="13464" class="Keyword">import</a> <a id="13471" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13495" class="Keyword">open</a> <a id="13500" class="Keyword">import</a> <a id="13507" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13545" class="Keyword">open</a> <a id="13550" class="Keyword">import</a> <a id="13557" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13588" class="Keyword">open</a> <a id="13593" class="Keyword">import</a> <a id="13600" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13625" class="Keyword">open</a> <a id="13630" class="Keyword">import</a> <a id="13637" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13665" class="Keyword">open</a> <a id="13670" class="Keyword">import</a> <a id="13677" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13701" class="Keyword">open</a> <a id="13706" class="Keyword">import</a> <a id="13713" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13739" class="Keyword">open</a> <a id="13744" class="Keyword">import</a> <a id="13751" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="13786" class="Keyword">open</a> <a id="13791" class="Keyword">import</a> <a id="13798" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="13819" class="Keyword">open</a> <a id="13824" class="Keyword">import</a> <a id="13831" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="13880" class="Keyword">open</a> <a id="13885" class="Keyword">import</a> <a id="13892" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="13933" class="Keyword">open</a> <a id="13938" class="Keyword">import</a> <a id="13945" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="13995" class="Keyword">open</a> <a id="14000" class="Keyword">import</a> <a id="14007" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14053" class="Keyword">open</a> <a id="14058" class="Keyword">import</a> <a id="14065" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14105" class="Keyword">open</a> <a id="14110" class="Keyword">import</a> <a id="14117" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14167" class="Keyword">open</a> <a id="14172" class="Keyword">import</a> <a id="14179" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14218" class="Keyword">open</a> <a id="14223" class="Keyword">import</a> <a id="14230" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14270" class="Keyword">open</a> <a id="14275" class="Keyword">import</a> <a id="14282" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14315" class="Keyword">open</a> <a id="14320" class="Keyword">import</a> <a id="14327" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14376" class="Keyword">open</a> <a id="14381" class="Keyword">import</a> <a id="14388" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14413" class="Keyword">open</a> <a id="14418" class="Keyword">import</a> <a id="14425" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14463" class="Keyword">open</a> <a id="14468" class="Keyword">import</a> <a id="14475" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14497" class="Keyword">open</a> <a id="14502" class="Keyword">import</a> <a id="14509" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14537" class="Keyword">open</a> <a id="14542" class="Keyword">import</a> <a id="14549" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14575" class="Keyword">open</a> <a id="14580" class="Keyword">import</a> <a id="14587" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14605" class="Keyword">open</a> <a id="14610" class="Keyword">import</a> <a id="14617" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14652" class="Keyword">open</a> <a id="14657" class="Keyword">import</a> <a id="14664" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="14691" class="Keyword">open</a> <a id="14696" class="Keyword">import</a> <a id="14703" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="14759" class="Keyword">open</a> <a id="14764" class="Keyword">import</a> <a id="14771" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="14800" class="Keyword">open</a> <a id="14805" class="Keyword">import</a> <a id="14812" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="14842" class="Keyword">open</a> <a id="14847" class="Keyword">import</a> <a id="14854" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="14881" class="Keyword">open</a> <a id="14886" class="Keyword">import</a> <a id="14893" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="14919" class="Keyword">open</a> <a id="14924" class="Keyword">import</a> <a id="14931" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="14958" class="Keyword">open</a> <a id="14963" class="Keyword">import</a> <a id="14970" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="14994" class="Keyword">open</a> <a id="14999" class="Keyword">import</a> <a id="15006" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15029" class="Keyword">open</a> <a id="15034" class="Keyword">import</a> <a id="15041" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15068" class="Keyword">open</a> <a id="15073" class="Keyword">import</a> <a id="15080" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15112" class="Keyword">open</a> <a id="15117" class="Keyword">import</a> <a id="15124" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15159" class="Keyword">open</a> <a id="15164" class="Keyword">import</a> <a id="15171" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15202" class="Keyword">open</a> <a id="15207" class="Keyword">import</a> <a id="15214" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15247" class="Keyword">open</a> <a id="15252" class="Keyword">import</a> <a id="15259" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15293" class="Keyword">open</a> <a id="15298" class="Keyword">import</a> <a id="15305" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15345" class="Keyword">open</a> <a id="15350" class="Keyword">import</a> <a id="15357" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15388" class="Keyword">open</a> <a id="15393" class="Keyword">import</a> <a id="15400" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15432" class="Keyword">open</a> <a id="15437" class="Keyword">import</a> <a id="15444" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15475" class="Keyword">open</a> <a id="15480" class="Keyword">import</a> <a id="15487" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15504" class="Keyword">open</a> <a id="15509" class="Keyword">import</a> <a id="15516" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15541" class="Keyword">open</a> <a id="15546" class="Keyword">import</a> <a id="15553" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15582" class="Keyword">open</a> <a id="15587" class="Keyword">import</a> <a id="15594" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15619" class="Keyword">open</a> <a id="15624" class="Keyword">import</a> <a id="15631" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15652" class="Keyword">open</a> <a id="15657" class="Keyword">import</a> <a id="15664" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="15688" class="Keyword">open</a> <a id="15693" class="Keyword">import</a> <a id="15700" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="15720" class="Keyword">open</a> <a id="15725" class="Keyword">import</a> <a id="15732" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="15766" class="Keyword">open</a> <a id="15771" class="Keyword">import</a> <a id="15778" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="15816" class="Keyword">open</a> <a id="15821" class="Keyword">import</a> <a id="15828" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="15852" class="Keyword">open</a> <a id="15857" class="Keyword">import</a> <a id="15864" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="15891" class="Keyword">open</a> <a id="15896" class="Keyword">import</a> <a id="15903" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="15938" class="Keyword">open</a> <a id="15943" class="Keyword">import</a> <a id="15950" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="15971" class="Keyword">open</a> <a id="15976" class="Keyword">import</a> <a id="15983" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16019" class="Keyword">open</a> <a id="16024" class="Keyword">import</a> <a id="16031" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16076" class="Keyword">open</a> <a id="16081" class="Keyword">import</a> <a id="16088" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16134" class="Keyword">open</a> <a id="16139" class="Keyword">import</a> <a id="16146" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16186" class="Keyword">open</a> <a id="16191" class="Keyword">import</a> <a id="16198" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16228" class="Keyword">open</a> <a id="16233" class="Keyword">import</a> <a id="16240" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16277" class="Keyword">open</a> <a id="16282" class="Keyword">import</a> <a id="16289" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16313" class="Keyword">open</a> <a id="16318" class="Keyword">import</a> <a id="16325" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16346" class="Keyword">open</a> <a id="16351" class="Keyword">import</a> <a id="16358" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16393" class="Keyword">open</a> <a id="16398" class="Keyword">import</a> <a id="16405" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16442" class="Keyword">open</a> <a id="16447" class="Keyword">import</a> <a id="16454" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16503" class="Keyword">open</a> <a id="16508" class="Keyword">import</a> <a id="16515" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16548" class="Keyword">open</a> <a id="16553" class="Keyword">import</a> <a id="16560" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16583" class="Keyword">open</a> <a id="16588" class="Keyword">import</a> <a id="16595" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="16618" class="Keyword">open</a> <a id="16623" class="Keyword">import</a> <a id="16630" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="16653" class="Keyword">open</a> <a id="16658" class="Keyword">import</a> <a id="16665" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="16693" class="Keyword">open</a> <a id="16698" class="Keyword">import</a> <a id="16705" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="16725" class="Keyword">open</a> <a id="16730" class="Keyword">import</a> <a id="16737" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="16758" class="Keyword">open</a> <a id="16763" class="Keyword">import</a> <a id="16770" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="16801" class="Keyword">open</a> <a id="16806" class="Keyword">import</a> <a id="16813" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="16840" class="Keyword">open</a> <a id="16845" class="Keyword">import</a> <a id="16852" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="16868" class="Keyword">open</a> <a id="16873" class="Keyword">import</a> <a id="16880" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="16911" class="Keyword">open</a> <a id="16916" class="Keyword">import</a> <a id="16923" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="16940" class="Keyword">open</a> <a id="16945" class="Keyword">import</a> <a id="16952" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="16974" class="Keyword">open</a> <a id="16979" class="Keyword">import</a> <a id="16986" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17013" class="Keyword">open</a> <a id="17018" class="Keyword">import</a> <a id="17025" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17048" class="Keyword">open</a> <a id="17053" class="Keyword">import</a> <a id="17060" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17087" class="Keyword">open</a> <a id="17092" class="Keyword">import</a> <a id="17099" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17132" class="Keyword">open</a> <a id="17137" class="Keyword">import</a> <a id="17144" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17184" class="Keyword">open</a> <a id="17189" class="Keyword">import</a> <a id="17196" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17217" class="Keyword">open</a> <a id="17222" class="Keyword">import</a> <a id="17229" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17258" class="Keyword">open</a> <a id="17263" class="Keyword">import</a> <a id="17270" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17308" class="Keyword">open</a> <a id="17313" class="Keyword">import</a> <a id="17320" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17340" class="Keyword">open</a> <a id="17345" class="Keyword">import</a> <a id="17352" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17376" class="Keyword">open</a> <a id="17381" class="Keyword">import</a> <a id="17388" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17415" class="Keyword">open</a> <a id="17420" class="Keyword">import</a> <a id="17427" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17459" class="Keyword">open</a> <a id="17464" class="Keyword">import</a> <a id="17471" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17501" class="Keyword">open</a> <a id="17506" class="Keyword">import</a> <a id="17513" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17539" class="Keyword">open</a> <a id="17544" class="Keyword">import</a> <a id="17551" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17578" class="Keyword">open</a> <a id="17583" class="Keyword">import</a> <a id="17590" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="17619" class="Keyword">open</a> <a id="17624" class="Keyword">import</a> <a id="17631" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="17654" class="Keyword">open</a> <a id="17659" class="Keyword">import</a> <a id="17666" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="17717" class="Keyword">open</a> <a id="17722" class="Keyword">import</a> <a id="17729" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="17772" class="Keyword">open</a> <a id="17777" class="Keyword">import</a> <a id="17784" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="17832" class="Keyword">open</a> <a id="17837" class="Keyword">import</a> <a id="17844" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="17882" class="Keyword">open</a> <a id="17887" class="Keyword">import</a> <a id="17894" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="17931" class="Keyword">open</a> <a id="17936" class="Keyword">import</a> <a id="17943" href="foundation.union.html" class="Module">foundation.union</a>
<a id="17960" class="Keyword">open</a> <a id="17965" class="Keyword">import</a> <a id="17972" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18000" class="Keyword">open</a> <a id="18005" class="Keyword">import</a> <a id="18012" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18048" class="Keyword">open</a> <a id="18053" class="Keyword">import</a> <a id="18060" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18098" class="Keyword">open</a> <a id="18103" class="Keyword">import</a> <a id="18110" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18143" class="Keyword">open</a> <a id="18148" class="Keyword">import</a> <a id="18155" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18176" class="Keyword">open</a> <a id="18181" class="Keyword">import</a> <a id="18188" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18242" class="Keyword">open</a> <a id="18247" class="Keyword">import</a> <a id="18254" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18276" class="Keyword">open</a> <a id="18281" class="Keyword">import</a> <a id="18288" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18323" class="Keyword">open</a> <a id="18328" class="Keyword">import</a> <a id="18335" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18365" class="Keyword">open</a> <a id="18370" class="Keyword">import</a> <a id="18377" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18416" class="Keyword">open</a> <a id="18421" class="Keyword">import</a> <a id="18428" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18482" class="Keyword">open</a> <a id="18487" class="Keyword">import</a> <a id="18494" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18540" class="Keyword">open</a> <a id="18545" class="Keyword">import</a> <a id="18552" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18603" class="Keyword">open</a> <a id="18608" class="Keyword">import</a> <a id="18615" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="18656" class="Keyword">open</a> <a id="18661" class="Keyword">import</a> <a id="18668" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="18713" class="Keyword">open</a> <a id="18718" class="Keyword">import</a> <a id="18725" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="18770" class="Keyword">open</a> <a id="18775" class="Keyword">import</a> <a id="18782" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="18818" class="Keyword">open</a> <a id="18823" class="Keyword">import</a> <a id="18830" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="18866" class="Keyword">open</a> <a id="18871" class="Keyword">import</a> <a id="18878" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="18943" class="Keyword">open</a> <a id="18948" class="Keyword">import</a> <a id="18955" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19010" class="Keyword">open</a> <a id="19015" class="Keyword">import</a> <a id="19022" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19062" class="Keyword">open</a> <a id="19067" class="Keyword">import</a> <a id="19074" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19118" class="Keyword">open</a> <a id="19123" class="Keyword">import</a> <a id="19130" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19175" class="Keyword">open</a> <a id="19180" class="Keyword">import</a> <a id="19187" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19228" class="Keyword">open</a> <a id="19233" class="Keyword">import</a> <a id="19240" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19280" class="Keyword">open</a> <a id="19285" class="Keyword">import</a> <a id="19292" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19319" class="Keyword">open</a> <a id="19324" class="Keyword">import</a> <a id="19331" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19367" class="Keyword">open</a> <a id="19372" class="Keyword">import</a> <a id="19379" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19406" class="Keyword">open</a> <a id="19411" class="Keyword">import</a> <a id="19418" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19455" class="Keyword">open</a> <a id="19460" class="Keyword">import</a> <a id="19467" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19495" class="Keyword">open</a> <a id="19500" class="Keyword">import</a> <a id="19507" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19526" class="Keyword">open</a> <a id="19531" class="Keyword">import</a> <a id="19538" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19578" class="Keyword">open</a> <a id="19583" class="Keyword">import</a> <a id="19590" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19622" class="Keyword">open</a> <a id="19627" class="Keyword">import</a> <a id="19634" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="19682" class="Keyword">open</a> <a id="19687" class="Keyword">import</a> <a id="19694" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="19717" class="Keyword">open</a> <a id="19722" class="Keyword">import</a> <a id="19729" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="19753" class="Keyword">open</a> <a id="19758" class="Keyword">import</a> <a id="19765" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="19805" class="Keyword">open</a> <a id="19810" class="Keyword">import</a> <a id="19817" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="19860" class="Keyword">open</a> <a id="19865" class="Keyword">import</a> <a id="19872" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="19906" class="Keyword">open</a> <a id="19911" class="Keyword">import</a> <a id="19918" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="19950" class="Keyword">open</a> <a id="19955" class="Keyword">import</a> <a id="19962" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="19992" class="Keyword">open</a> <a id="19997" class="Keyword">import</a> <a id="20004" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20038" class="Keyword">open</a> <a id="20043" class="Keyword">import</a> <a id="20050" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20085" class="Keyword">open</a> <a id="20090" class="Keyword">import</a> <a id="20097" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20134" class="Keyword">open</a> <a id="20139" class="Keyword">import</a> <a id="20146" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20173" class="Keyword">open</a> <a id="20178" class="Keyword">import</a> <a id="20185" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20213" class="Keyword">open</a> <a id="20218" class="Keyword">import</a> <a id="20225" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20274" class="Keyword">open</a> <a id="20279" class="Keyword">import</a> <a id="20286" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20332" class="Keyword">open</a> <a id="20337" class="Keyword">import</a> <a id="20344" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20384" class="Keyword">open</a> <a id="20389" class="Keyword">import</a> <a id="20396" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20434" class="Keyword">open</a> <a id="20439" class="Keyword">import</a> <a id="20446" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20475" class="Keyword">open</a> <a id="20480" class="Keyword">import</a> <a id="20487" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20517" class="Keyword">open</a> <a id="20522" class="Keyword">import</a> <a id="20529" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20560" class="Keyword">open</a> <a id="20565" class="Keyword">import</a> <a id="20572" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="20612" class="Keyword">open</a> <a id="20617" class="Keyword">import</a> <a id="20624" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="20650" class="Keyword">open</a> <a id="20655" class="Keyword">import</a> <a id="20662" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="20717" class="Keyword">open</a> <a id="20722" class="Keyword">import</a> <a id="20729" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="20780" class="Keyword">open</a> <a id="20785" class="Keyword">import</a> <a id="20792" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="20837" class="Keyword">open</a> <a id="20842" class="Keyword">import</a> <a id="20849" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="20903" class="Keyword">open</a> <a id="20908" class="Keyword">import</a> <a id="20915" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="20942" class="Keyword">open</a> <a id="20947" class="Keyword">import</a> <a id="20954" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="20987" class="Keyword">open</a> <a id="20992" class="Keyword">import</a> <a id="20999" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21030" class="Keyword">open</a> <a id="21035" class="Keyword">import</a> <a id="21042" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21079" class="Keyword">open</a> <a id="21084" class="Keyword">import</a> <a id="21091" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21116" class="Keyword">open</a> <a id="21121" class="Keyword">import</a> <a id="21128" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21160" class="Keyword">open</a> <a id="21165" class="Keyword">import</a> <a id="21172" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21207" class="Keyword">open</a> <a id="21212" class="Keyword">import</a> <a id="21219" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21248" class="Keyword">open</a> <a id="21253" class="Keyword">import</a> <a id="21260" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21286" class="Keyword">open</a> <a id="21291" class="Keyword">import</a> <a id="21298" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21326" class="Keyword">open</a> <a id="21331" class="Keyword">import</a> <a id="21338" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21363" class="Keyword">open</a> <a id="21368" class="Keyword">import</a> <a id="21375" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21396" class="Keyword">open</a> <a id="21401" class="Keyword">import</a> <a id="21408" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21444" class="Keyword">open</a> <a id="21449" class="Keyword">import</a> <a id="21456" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21499" class="Keyword">open</a> <a id="21504" class="Keyword">import</a> <a id="21511" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21536" class="Keyword">open</a> <a id="21541" class="Keyword">import</a> <a id="21548" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21579" class="Keyword">open</a> <a id="21584" class="Keyword">import</a> <a id="21591" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21623" class="Keyword">open</a> <a id="21628" class="Keyword">import</a> <a id="21635" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="21669" class="Keyword">open</a> <a id="21674" class="Keyword">import</a> <a id="21681" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="21737" class="Keyword">open</a> <a id="21742" class="Keyword">import</a> <a id="21749" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="21802" class="Keyword">open</a> <a id="21807" class="Keyword">import</a> <a id="21814" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="21841" class="Keyword">open</a> <a id="21846" class="Keyword">import</a> <a id="21853" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="21898" class="Keyword">open</a> <a id="21903" class="Keyword">import</a> <a id="21910" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="21972" class="Keyword">open</a> <a id="21977" class="Keyword">import</a> <a id="21984" href="graph-theory.html" class="Module">graph-theory</a>
<a id="21997" class="Keyword">open</a> <a id="22002" class="Keyword">import</a> <a id="22009" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22050" class="Keyword">open</a> <a id="22055" class="Keyword">import</a> <a id="22062" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22091" class="Keyword">open</a> <a id="22096" class="Keyword">import</a> <a id="22103" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22148" class="Keyword">open</a> <a id="22153" class="Keyword">import</a> <a id="22160" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22204" class="Keyword">open</a> <a id="22209" class="Keyword">import</a> <a id="22216" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="22243" class="Keyword">open</a> <a id="22248" class="Keyword">import</a> <a id="22255" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="22296" class="Keyword">open</a> <a id="22301" class="Keyword">import</a> <a id="22308" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="22331" class="Keyword">open</a> <a id="22336" class="Keyword">import</a> <a id="22343" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="22392" class="Keyword">open</a> <a id="22397" class="Keyword">import</a> <a id="22404" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="22443" class="Keyword">open</a> <a id="22448" class="Keyword">import</a> <a id="22455" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="22496" class="Keyword">open</a> <a id="22501" class="Keyword">import</a> <a id="22508" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22552" class="Keyword">open</a> <a id="22557" class="Keyword">import</a> <a id="22564" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22601" class="Keyword">open</a> <a id="22606" class="Keyword">import</a> <a id="22613" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="22635" class="Keyword">open</a> <a id="22640" class="Keyword">import</a> <a id="22647" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="22677" class="Keyword">open</a> <a id="22682" class="Keyword">import</a> <a id="22689" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="22728" class="Keyword">open</a> <a id="22733" class="Keyword">import</a> <a id="22740" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="22778" class="Keyword">open</a> <a id="22783" class="Keyword">import</a> <a id="22790" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="22821" class="Keyword">open</a> <a id="22826" class="Keyword">import</a> <a id="22833" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="22860" class="Keyword">open</a> <a id="22865" class="Keyword">import</a> <a id="22872" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="22930" class="Keyword">open</a> <a id="22935" class="Keyword">import</a> <a id="22942" href="group-theory.html" class="Module">group-theory</a>
<a id="22955" class="Keyword">open</a> <a id="22960" class="Keyword">import</a> <a id="22967" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="22995" class="Keyword">open</a> <a id="23000" class="Keyword">import</a> <a id="23007" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="23038" class="Keyword">open</a> <a id="23043" class="Keyword">import</a> <a id="23050" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="23086" class="Keyword">open</a> <a id="23091" class="Keyword">import</a> <a id="23098" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="23149" class="Keyword">open</a> <a id="23154" class="Keyword">import</a> <a id="23161" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="23194" class="Keyword">open</a> <a id="23199" class="Keyword">import</a> <a id="23206" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="23253" class="Keyword">open</a> <a id="23258" class="Keyword">import</a> <a id="23265" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="23304" class="Keyword">open</a> <a id="23309" class="Keyword">import</a> <a id="23316" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="23356" class="Keyword">open</a> <a id="23361" class="Keyword">import</a> <a id="23368" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="23411" class="Keyword">open</a> <a id="23416" class="Keyword">import</a> <a id="23423" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="23455" class="Keyword">open</a> <a id="23460" class="Keyword">import</a> <a id="23467" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="23503" class="Keyword">open</a> <a id="23508" class="Keyword">import</a> <a id="23515" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="23544" class="Keyword">open</a> <a id="23549" class="Keyword">import</a> <a id="23556" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="23589" class="Keyword">open</a> <a id="23594" class="Keyword">import</a> <a id="23601" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="23637" class="Keyword">open</a> <a id="23642" class="Keyword">import</a> <a id="23649" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="23678" class="Keyword">open</a> <a id="23683" class="Keyword">import</a> <a id="23690" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="23722" class="Keyword">open</a> <a id="23727" class="Keyword">import</a> <a id="23734" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="23759" class="Keyword">open</a> <a id="23764" class="Keyword">import</a> <a id="23771" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="23802" class="Keyword">open</a> <a id="23807" class="Keyword">import</a> <a id="23814" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="23861" class="Keyword">open</a> <a id="23866" class="Keyword">import</a> <a id="23873" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="23906" class="Keyword">open</a> <a id="23911" class="Keyword">import</a> <a id="23918" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="23958" class="Keyword">open</a> <a id="23963" class="Keyword">import</a> <a id="23970" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="24007" class="Keyword">open</a> <a id="24012" class="Keyword">import</a> <a id="24019" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="24055" class="Keyword">open</a> <a id="24060" class="Keyword">import</a> <a id="24067" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="24099" class="Keyword">open</a> <a id="24104" class="Keyword">import</a> <a id="24111" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="24138" class="Keyword">open</a> <a id="24143" class="Keyword">import</a> <a id="24150" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="24170" class="Keyword">open</a> <a id="24175" class="Keyword">import</a> <a id="24182" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="24209" class="Keyword">open</a> <a id="24214" class="Keyword">import</a> <a id="24221" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="24263" class="Keyword">open</a> <a id="24268" class="Keyword">import</a> <a id="24275" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="24322" class="Keyword">open</a> <a id="24327" class="Keyword">import</a> <a id="24334" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="24375" class="Keyword">open</a> <a id="24380" class="Keyword">import</a> <a id="24387" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="24421" class="Keyword">open</a> <a id="24426" class="Keyword">import</a> <a id="24433" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="24468" class="Keyword">open</a> <a id="24473" class="Keyword">import</a> <a id="24480" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="24518" class="Keyword">open</a> <a id="24523" class="Keyword">import</a> <a id="24530" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="24562" class="Keyword">open</a> <a id="24567" class="Keyword">import</a> <a id="24574" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="24615" class="Keyword">open</a> <a id="24620" class="Keyword">import</a> <a id="24627" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="24668" class="Keyword">open</a> <a id="24673" class="Keyword">import</a> <a id="24680" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="24720" class="Keyword">open</a> <a id="24725" class="Keyword">import</a> <a id="24732" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="24765" class="Keyword">open</a> <a id="24770" class="Keyword">import</a> <a id="24777" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="24814" class="Keyword">open</a> <a id="24819" class="Keyword">import</a> <a id="24826" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="24871" class="Keyword">open</a> <a id="24876" class="Keyword">import</a> <a id="24883" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="24911" class="Keyword">open</a> <a id="24916" class="Keyword">import</a> <a id="24923" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="24944" class="Keyword">open</a> <a id="24949" class="Keyword">import</a> <a id="24956" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="24990" class="Keyword">open</a> <a id="24995" class="Keyword">import</a> <a id="25002" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="25036" class="Keyword">open</a> <a id="25041" class="Keyword">import</a> <a id="25048" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="25083" class="Keyword">open</a> <a id="25088" class="Keyword">import</a> <a id="25095" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="25137" class="Keyword">open</a> <a id="25142" class="Keyword">import</a> <a id="25149" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="25184" class="Keyword">open</a> <a id="25189" class="Keyword">import</a> <a id="25196" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="25235" class="Keyword">open</a> <a id="25240" class="Keyword">import</a> <a id="25247" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="25284" class="Keyword">open</a> <a id="25289" class="Keyword">import</a> <a id="25296" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="25320" class="Keyword">open</a> <a id="25325" class="Keyword">import</a> <a id="25332" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="25357" class="Keyword">open</a> <a id="25362" class="Keyword">import</a> <a id="25369" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="25400" class="Keyword">open</a> <a id="25405" class="Keyword">import</a> <a id="25412" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="25463" class="Keyword">open</a> <a id="25468" class="Keyword">import</a> <a id="25475" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="25498" class="Keyword">open</a> <a id="25503" class="Keyword">import</a> <a id="25510" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="25558" class="Keyword">open</a> <a id="25563" class="Keyword">import</a> <a id="25570" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="25600" class="Keyword">open</a> <a id="25605" class="Keyword">import</a> <a id="25612" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="25682" class="Keyword">open</a> <a id="25687" class="Keyword">import</a> <a id="25694" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="25709" class="Keyword">open</a> <a id="25714" class="Keyword">import</a> <a id="25721" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="25754" class="Keyword">open</a> <a id="25759" class="Keyword">import</a> <a id="25766" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="25798" class="Keyword">open</a> <a id="25803" class="Keyword">import</a> <a id="25810" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="25852" class="Keyword">open</a> <a id="25857" class="Keyword">import</a> <a id="25864" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="25902" class="Keyword">open</a> <a id="25907" class="Keyword">import</a> <a id="25914" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="25951" class="Keyword">open</a> <a id="25956" class="Keyword">import</a> <a id="25963" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="25996" class="Keyword">open</a> <a id="26001" class="Keyword">import</a> <a id="26008" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="26032" class="Keyword">open</a> <a id="26037" class="Keyword">import</a> <a id="26044" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="26083" class="Keyword">open</a> <a id="26088" class="Keyword">import</a> <a id="26095" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="26141" class="Keyword">open</a> <a id="26146" class="Keyword">import</a> <a id="26153" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="26198" class="Keyword">open</a> <a id="26203" class="Keyword">import</a> <a id="26210" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="26248" class="Keyword">open</a> <a id="26253" class="Keyword">import</a> <a id="26260" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="26292" class="Keyword">open</a> <a id="26297" class="Keyword">import</a> <a id="26304" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="26357" class="Keyword">open</a> <a id="26362" class="Keyword">import</a> <a id="26369" href="order-theory.html" class="Module">order-theory</a>
<a id="26382" class="Keyword">open</a> <a id="26387" class="Keyword">import</a> <a id="26394" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="26421" class="Keyword">open</a> <a id="26426" class="Keyword">import</a> <a id="26433" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="26463" class="Keyword">open</a> <a id="26468" class="Keyword">import</a> <a id="26475" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="26508" class="Keyword">open</a> <a id="26513" class="Keyword">import</a> <a id="26520" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="26556" class="Keyword">open</a> <a id="26561" class="Keyword">import</a> <a id="26568" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="26595" class="Keyword">open</a> <a id="26600" class="Keyword">import</a> <a id="26607" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="26637" class="Keyword">open</a> <a id="26642" class="Keyword">import</a> <a id="26649" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="26685" class="Keyword">open</a> <a id="26690" class="Keyword">import</a> <a id="26697" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="26739" class="Keyword">open</a> <a id="26744" class="Keyword">import</a> <a id="26751" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="26783" class="Keyword">open</a> <a id="26788" class="Keyword">import</a> <a id="26795" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="26826" class="Keyword">open</a> <a id="26831" class="Keyword">import</a> <a id="26838" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="26864" class="Keyword">open</a> <a id="26869" class="Keyword">import</a> <a id="26876" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="26905" class="Keyword">open</a> <a id="26910" class="Keyword">import</a> <a id="26917" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="26954" class="Keyword">open</a> <a id="26959" class="Keyword">import</a> <a id="26966" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="27006" class="Keyword">open</a> <a id="27011" class="Keyword">import</a> <a id="27018" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="27040" class="Keyword">open</a> <a id="27045" class="Keyword">import</a> <a id="27052" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="27087" class="Keyword">open</a> <a id="27092" class="Keyword">import</a> <a id="27099" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="27137" class="Keyword">open</a> <a id="27142" class="Keyword">import</a> <a id="27149" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="27188" class="Keyword">open</a> <a id="27193" class="Keyword">import</a> <a id="27200" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="27235" class="Keyword">open</a> <a id="27240" class="Keyword">import</a> <a id="27247" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="27282" class="Keyword">open</a> <a id="27287" class="Keyword">import</a> <a id="27294" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="27332" class="Keyword">open</a> <a id="27337" class="Keyword">import</a> <a id="27344" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="27375" class="Keyword">open</a> <a id="27380" class="Keyword">import</a> <a id="27387" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="27429" class="Keyword">open</a> <a id="27434" class="Keyword">import</a> <a id="27441" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="27486" class="Keyword">open</a> <a id="27491" class="Keyword">import</a> <a id="27498" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="27531" class="Keyword">open</a> <a id="27536" class="Keyword">import</a> <a id="27543" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="27563" class="Keyword">open</a> <a id="27568" class="Keyword">import</a> <a id="27575" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="27598" class="Keyword">open</a> <a id="27603" class="Keyword">import</a> <a id="27610" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="27633" class="Keyword">open</a> <a id="27638" class="Keyword">import</a> <a id="27645" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="27671" class="Keyword">open</a> <a id="27676" class="Keyword">import</a> <a id="27683" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="27709" class="Keyword">open</a> <a id="27714" class="Keyword">import</a> <a id="27721" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="27777" class="Keyword">open</a> <a id="27782" class="Keyword">import</a> <a id="27789" href="polytopes.html" class="Module">polytopes</a>
<a id="27799" class="Keyword">open</a> <a id="27804" class="Keyword">import</a> <a id="27811" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="27869" class="Keyword">open</a> <a id="27874" class="Keyword">import</a> <a id="27881" href="ring-theory.html" class="Module">ring-theory</a>
<a id="27893" class="Keyword">open</a> <a id="27898" class="Keyword">import</a> <a id="27905" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="27942" class="Keyword">open</a> <a id="27947" class="Keyword">import</a> <a id="27954" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="27981" class="Keyword">open</a> <a id="27986" class="Keyword">import</a> <a id="27993" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="28025" class="Keyword">open</a> <a id="28030" class="Keyword">import</a> <a id="28037" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="28083" class="Keyword">open</a> <a id="28088" class="Keyword">import</a> <a id="28095" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="28120" class="Keyword">open</a> <a id="28125" class="Keyword">import</a> <a id="28132" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="28175" class="Keyword">open</a> <a id="28180" class="Keyword">import</a> <a id="28187" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="28225" class="Keyword">open</a> <a id="28230" class="Keyword">import</a> <a id="28237" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="28268" class="Keyword">open</a> <a id="28273" class="Keyword">import</a> <a id="28280" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="28312" class="Keyword">open</a> <a id="28317" class="Keyword">import</a> <a id="28324" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="28350" class="Keyword">open</a> <a id="28355" class="Keyword">import</a> <a id="28362" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="28391" class="Keyword">open</a> <a id="28396" class="Keyword">import</a> <a id="28403" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="28440" class="Keyword">open</a> <a id="28445" class="Keyword">import</a> <a id="28452" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="28481" class="Keyword">open</a> <a id="28486" class="Keyword">import</a> <a id="28493" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="28520" class="Keyword">open</a> <a id="28525" class="Keyword">import</a> <a id="28532" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="28569" class="Keyword">open</a> <a id="28574" class="Keyword">import</a> <a id="28581" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="28608" class="Keyword">open</a> <a id="28613" class="Keyword">import</a> <a id="28620" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="28653" class="Keyword">open</a> <a id="28658" class="Keyword">import</a> <a id="28665" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="28683" class="Keyword">open</a> <a id="28688" class="Keyword">import</a> <a id="28695" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="28749" class="Keyword">open</a> <a id="28754" class="Keyword">import</a> <a id="28761" href="set-theory.html" class="Module">set-theory</a>
<a id="28772" class="Keyword">open</a> <a id="28777" class="Keyword">import</a> <a id="28784" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="28810" class="Keyword">open</a> <a id="28815" class="Keyword">import</a> <a id="28822" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="28884" class="Keyword">open</a> <a id="28889" class="Keyword">import</a> <a id="28896" href="structured-types.html" class="Module">structured-types</a>
<a id="28913" class="Keyword">open</a> <a id="28918" class="Keyword">import</a> <a id="28925" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="28969" class="Keyword">open</a> <a id="28974" class="Keyword">import</a> <a id="28981" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="29045" class="Keyword">open</a> <a id="29050" class="Keyword">import</a> <a id="29057" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="29103" class="Keyword">open</a> <a id="29108" class="Keyword">import</a> <a id="29115" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="29139" class="Keyword">open</a> <a id="29144" class="Keyword">import</a> <a id="29151" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="29220" class="Keyword">open</a> <a id="29225" class="Keyword">import</a> <a id="29232" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="29266" class="Keyword">open</a> <a id="29271" class="Keyword">import</a> <a id="29278" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="29339" class="Keyword">open</a> <a id="29344" class="Keyword">import</a> <a id="29351" href="structured-types.morphisms-wild-unital-magmas.html" class="Module">structured-types.morphisms-wild-unital-magmas</a>
<a id="29397" class="Keyword">open</a> <a id="29402" class="Keyword">import</a> <a id="29409" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="29454" class="Keyword">open</a> <a id="29459" class="Keyword">import</a> <a id="29466" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="29504" class="Keyword">open</a> <a id="29509" class="Keyword">import</a> <a id="29516" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="29559" class="Keyword">open</a> <a id="29564" class="Keyword">import</a> <a id="29571" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="29607" class="Keyword">open</a> <a id="29612" class="Keyword">import</a> <a id="29619" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="29649" class="Keyword">open</a> <a id="29654" class="Keyword">import</a> <a id="29661" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="29692" class="Keyword">open</a> <a id="29697" class="Keyword">import</a> <a id="29704" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="29755" class="Keyword">open</a> <a id="29760" class="Keyword">import</a> <a id="29767" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="29822" class="Keyword">open</a> <a id="29827" class="Keyword">import</a> <a id="29834" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="29863" class="Keyword">open</a> <a id="29868" class="Keyword">import</a> <a id="29875" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="29903" class="Keyword">open</a> <a id="29908" class="Keyword">import</a> <a id="29915" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="29945" class="Keyword">open</a> <a id="29950" class="Keyword">import</a> <a id="29957" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="29991" class="Keyword">open</a> <a id="29996" class="Keyword">import</a> <a id="30003" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
<a id="30036" class="Keyword">open</a> <a id="30041" class="Keyword">import</a> <a id="30048" href="structured-types.wild-unital-magmas.html" class="Module">structured-types.wild-unital-magmas</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="30127" class="Keyword">open</a> <a id="30132" class="Keyword">import</a> <a id="30139" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="30165" class="Keyword">open</a> <a id="30170" class="Keyword">import</a> <a id="30177" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="30216" class="Keyword">open</a> <a id="30221" class="Keyword">import</a> <a id="30228" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="30266" class="Keyword">open</a> <a id="30271" class="Keyword">import</a> <a id="30278" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="30324" class="Keyword">open</a> <a id="30329" class="Keyword">import</a> <a id="30336" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="30373" class="Keyword">open</a> <a id="30378" class="Keyword">import</a> <a id="30385" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="30425" class="Keyword">open</a> <a id="30430" class="Keyword">import</a> <a id="30437" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="30476" class="Keyword">open</a> <a id="30481" class="Keyword">import</a> <a id="30488" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="30521" class="Keyword">open</a> <a id="30526" class="Keyword">import</a> <a id="30533" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="30568" class="Keyword">open</a> <a id="30573" class="Keyword">import</a> <a id="30580" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="30619" class="Keyword">open</a> <a id="30624" class="Keyword">import</a> <a id="30631" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="30676" class="Keyword">open</a> <a id="30681" class="Keyword">import</a> <a id="30688" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="30740" class="Keyword">open</a> <a id="30745" class="Keyword">import</a> <a id="30752" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="30805" class="Keyword">open</a> <a id="30810" class="Keyword">import</a> <a id="30817" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="30865" class="Keyword">open</a> <a id="30870" class="Keyword">import</a> <a id="30877" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="30917" class="Keyword">open</a> <a id="30922" class="Keyword">import</a> <a id="30929" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="30976" class="Keyword">open</a> <a id="30981" class="Keyword">import</a> <a id="30988" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="31029" class="Keyword">open</a> <a id="31034" class="Keyword">import</a> <a id="31041" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="31079" class="Keyword">open</a> <a id="31084" class="Keyword">import</a> <a id="31091" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="31136" class="Keyword">open</a> <a id="31141" class="Keyword">import</a> <a id="31148" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="31197" class="Keyword">open</a> <a id="31202" class="Keyword">import</a> <a id="31209" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="31286" class="Keyword">open</a> <a id="31291" class="Keyword">import</a> <a id="31298" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="31350" class="Keyword">open</a> <a id="31355" class="Keyword">import</a> <a id="31362" href="type-theories.html" class="Module">type-theories</a>
<a id="31376" class="Keyword">open</a> <a id="31381" class="Keyword">import</a> <a id="31388" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="31430" class="Keyword">open</a> <a id="31435" class="Keyword">import</a> <a id="31442" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="31480" class="Keyword">open</a> <a id="31485" class="Keyword">import</a> <a id="31492" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="31538" class="Keyword">open</a> <a id="31543" class="Keyword">import</a> <a id="31550" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="31597" class="Keyword">open</a> <a id="31602" class="Keyword">import</a> <a id="31609" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="31644" class="Keyword">open</a> <a id="31649" class="Keyword">import</a> <a id="31656" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="31734" class="Keyword">open</a> <a id="31739" class="Keyword">import</a> <a id="31746" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="31770" class="Keyword">open</a> <a id="31775" class="Keyword">import</a> <a id="31782" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="31835" class="Keyword">open</a> <a id="31840" class="Keyword">import</a> <a id="31847" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="31890" class="Keyword">open</a> <a id="31895" class="Keyword">import</a> <a id="31902" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="31942" class="Keyword">open</a> <a id="31947" class="Keyword">import</a> <a id="31954" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="31993" class="Keyword">open</a> <a id="31998" class="Keyword">import</a> <a id="32005" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="32053" class="Keyword">open</a> <a id="32058" class="Keyword">import</a> <a id="32065" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="32112" class="Keyword">open</a> <a id="32117" class="Keyword">import</a> <a id="32124" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="32176" class="Keyword">open</a> <a id="32181" class="Keyword">import</a> <a id="32188" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="32232" class="Keyword">open</a> <a id="32237" class="Keyword">import</a> <a id="32244" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="32284" class="Keyword">open</a> <a id="32289" class="Keyword">import</a> <a id="32296" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="32348" class="Keyword">open</a> <a id="32353" class="Keyword">import</a> <a id="32360" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="32414" class="Keyword">open</a> <a id="32419" class="Keyword">import</a> <a id="32426" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="32474" class="Keyword">open</a> <a id="32479" class="Keyword">import</a> <a id="32486" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="32525" class="Keyword">open</a> <a id="32530" class="Keyword">import</a> <a id="32537" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="32570" class="Keyword">open</a> <a id="32575" class="Keyword">import</a> <a id="32582" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="32612" class="Keyword">open</a> <a id="32617" class="Keyword">import</a> <a id="32624" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="32683" class="Keyword">open</a> <a id="32688" class="Keyword">import</a> <a id="32695" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="32750" class="Keyword">open</a> <a id="32755" class="Keyword">import</a> <a id="32762" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="32809" class="Keyword">open</a> <a id="32814" class="Keyword">import</a> <a id="32821" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="32864" class="Keyword">open</a> <a id="32869" class="Keyword">import</a> <a id="32876" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="32921" class="Keyword">open</a> <a id="32926" class="Keyword">import</a> <a id="32933" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="32982" class="Keyword">open</a> <a id="32987" class="Keyword">import</a> <a id="32994" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="33045" class="Keyword">open</a> <a id="33050" class="Keyword">import</a> <a id="33057" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="33135" class="Keyword">open</a> <a id="33140" class="Keyword">import</a> <a id="33147" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="33187" class="Keyword">open</a> <a id="33192" class="Keyword">import</a> <a id="33199" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="33256" class="Keyword">open</a> <a id="33261" class="Keyword">import</a> <a id="33268" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="33303" class="Keyword">open</a> <a id="33308" class="Keyword">import</a> <a id="33315" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="33361" class="Keyword">open</a> <a id="33366" class="Keyword">import</a> <a id="33373" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="33428" class="Keyword">open</a> <a id="33433" class="Keyword">import</a> <a id="33440" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="33483" class="Keyword">open</a> <a id="33488" class="Keyword">import</a> <a id="33495" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="33554" class="Keyword">open</a> <a id="33559" class="Keyword">import</a> <a id="33566" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="33603" class="Keyword">open</a> <a id="33608" class="Keyword">import</a> <a id="33615" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="33656" class="Keyword">open</a> <a id="33661" class="Keyword">import</a> <a id="33668" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="33707" class="Keyword">open</a> <a id="33712" class="Keyword">import</a> <a id="33719" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="33757" class="Keyword">open</a> <a id="33762" class="Keyword">import</a> <a id="33769" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="33821" class="Keyword">open</a> <a id="33826" class="Keyword">import</a> <a id="33833" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="33878" class="Keyword">open</a> <a id="33883" class="Keyword">import</a> <a id="33890" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="33927" class="Keyword">open</a> <a id="33932" class="Keyword">import</a> <a id="33939" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="33988" class="Keyword">open</a> <a id="33993" class="Keyword">import</a> <a id="34000" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="34039" class="Keyword">open</a> <a id="34044" class="Keyword">import</a> <a id="34051" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="34089" class="Keyword">open</a> <a id="34094" class="Keyword">import</a> <a id="34101" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="34156" class="Keyword">open</a> <a id="34161" class="Keyword">import</a> <a id="34168" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="34207" class="Keyword">open</a> <a id="34212" class="Keyword">import</a> <a id="34219" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="34267" class="Keyword">open</a> <a id="34272" class="Keyword">import</a> <a id="34279" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="34326" class="Keyword">open</a> <a id="34331" class="Keyword">import</a> <a id="34338" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="34376" class="Keyword">open</a> <a id="34381" class="Keyword">import</a> <a id="34388" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="34418" class="Keyword">open</a> <a id="34423" class="Keyword">import</a> <a id="34430" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="34487" class="Keyword">open</a> <a id="34492" class="Keyword">import</a> <a id="34499" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="34553" class="Keyword">open</a> <a id="34558" class="Keyword">import</a> <a id="34565" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="34595" class="Keyword">open</a> <a id="34600" class="Keyword">import</a> <a id="34607" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="34670" class="Keyword">open</a> <a id="34675" class="Keyword">import</a> <a id="34682" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="34725" class="Keyword">open</a> <a id="34730" class="Keyword">import</a> <a id="34737" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="34772" class="Keyword">open</a> <a id="34777" class="Keyword">import</a> <a id="34784" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="34824" class="Keyword">open</a> <a id="34829" class="Keyword">import</a> <a id="34836" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="34881" class="Keyword">open</a> <a id="34886" class="Keyword">import</a> <a id="34893" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="34943" class="Keyword">open</a> <a id="34948" class="Keyword">import</a> <a id="34955" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="34993" class="Keyword">open</a> <a id="34998" class="Keyword">import</a> <a id="35005" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="35054" class="Keyword">open</a> <a id="35059" class="Keyword">import</a> <a id="35066" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="35113" class="Keyword">open</a> <a id="35118" class="Keyword">import</a> <a id="35125" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="35188" class="Keyword">open</a> <a id="35193" class="Keyword">import</a> <a id="35200" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="35232" class="Keyword">open</a> <a id="35237" class="Keyword">import</a> <a id="35244" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="35297" class="Keyword">open</a> <a id="35302" class="Keyword">import</a> <a id="35309" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="35355" class="Keyword">open</a> <a id="35360" class="Keyword">import</a> <a id="35367" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="35413" class="Keyword">open</a> <a id="35418" class="Keyword">import</a> <a id="35425" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="35473" class="Keyword">open</a> <a id="35478" class="Keyword">import</a> <a id="35485" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="35525" class="Keyword">open</a> <a id="35530" class="Keyword">import</a> <a id="35537" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="35582" class="Keyword">open</a> <a id="35587" class="Keyword">import</a> <a id="35594" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>