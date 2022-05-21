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
</pre>
## Elementary number theory

<pre class="Agda"><a id="5181" class="Keyword">open</a> <a id="5186" class="Keyword">import</a> <a id="5193" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5218" class="Keyword">open</a> <a id="5223" class="Keyword">import</a> <a id="5230" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5279" class="Keyword">open</a> <a id="5284" class="Keyword">import</a> <a id="5291" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5334" class="Keyword">open</a> <a id="5339" class="Keyword">import</a> <a id="5346" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5396" class="Keyword">open</a> <a id="5401" class="Keyword">import</a> <a id="5408" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5454" class="Keyword">open</a> <a id="5459" class="Keyword">import</a> <a id="5466" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5513" class="Keyword">open</a> <a id="5518" class="Keyword">import</a> <a id="5525" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5584" class="Keyword">open</a> <a id="5589" class="Keyword">import</a> <a id="5596" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="5637" class="Keyword">open</a> <a id="5642" class="Keyword">import</a> <a id="5649" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="5692" class="Keyword">open</a> <a id="5697" class="Keyword">import</a> <a id="5704" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="5748" class="Keyword">open</a> <a id="5753" class="Keyword">import</a> <a id="5760" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="5805" class="Keyword">open</a> <a id="5810" class="Keyword">import</a> <a id="5817" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="5869" class="Keyword">open</a> <a id="5874" class="Keyword">import</a> <a id="5881" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="5941" class="Keyword">open</a> <a id="5946" class="Keyword">import</a> <a id="5953" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="5994" class="Keyword">open</a> <a id="5999" class="Keyword">import</a> <a id="6006" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6051" class="Keyword">open</a> <a id="6056" class="Keyword">import</a> <a id="6063" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6110" class="Keyword">open</a> <a id="6115" class="Keyword">import</a> <a id="6122" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6165" class="Keyword">open</a> <a id="6170" class="Keyword">import</a> <a id="6177" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6227" class="Keyword">open</a> <a id="6232" class="Keyword">import</a> <a id="6239" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6286" class="Keyword">open</a> <a id="6291" class="Keyword">import</a> <a id="6298" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6355" class="Keyword">open</a> <a id="6360" class="Keyword">import</a> <a id="6367" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6421" class="Keyword">open</a> <a id="6426" class="Keyword">import</a> <a id="6433" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6493" class="Keyword">open</a> <a id="6498" class="Keyword">import</a> <a id="6505" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6548" class="Keyword">open</a> <a id="6553" class="Keyword">import</a> <a id="6560" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="6610" class="Keyword">open</a> <a id="6615" class="Keyword">import</a> <a id="6622" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="6682" class="Keyword">open</a> <a id="6687" class="Keyword">import</a> <a id="6694" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="6743" class="Keyword">open</a> <a id="6748" class="Keyword">import</a> <a id="6755" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="6811" class="Keyword">open</a> <a id="6816" class="Keyword">import</a> <a id="6823" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="6859" class="Keyword">open</a> <a id="6864" class="Keyword">import</a> <a id="6871" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="6915" class="Keyword">open</a> <a id="6920" class="Keyword">import</a> <a id="6927" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="6971" class="Keyword">open</a> <a id="6976" class="Keyword">import</a> <a id="6983" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7033" class="Keyword">open</a> <a id="7038" class="Keyword">import</a> <a id="7045" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7091" class="Keyword">open</a> <a id="7096" class="Keyword">import</a> <a id="7103" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7138" class="Keyword">open</a> <a id="7143" class="Keyword">import</a> <a id="7150" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7195" class="Keyword">open</a> <a id="7200" class="Keyword">import</a> <a id="7207" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7265" class="Keyword">open</a> <a id="7270" class="Keyword">import</a> <a id="7277" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7342" class="Keyword">open</a> <a id="7347" class="Keyword">import</a> <a id="7354" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7397" class="Keyword">open</a> <a id="7402" class="Keyword">import</a> <a id="7409" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7463" class="Keyword">open</a> <a id="7468" class="Keyword">import</a> <a id="7475" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7520" class="Keyword">open</a> <a id="7525" class="Keyword">import</a> <a id="7532" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7584" class="Keyword">open</a> <a id="7589" class="Keyword">import</a> <a id="7596" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7654" class="Keyword">open</a> <a id="7659" class="Keyword">import</a> <a id="7666" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="7712" class="Keyword">open</a> <a id="7717" class="Keyword">import</a> <a id="7724" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="7768" class="Keyword">open</a> <a id="7773" class="Keyword">import</a> <a id="7780" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="7814" class="Keyword">open</a> <a id="7819" class="Keyword">import</a> <a id="7826" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="7880" class="Keyword">open</a> <a id="7885" class="Keyword">import</a> <a id="7892" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="7941" class="Keyword">open</a> <a id="7946" class="Keyword">import</a> <a id="7953" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="7994" class="Keyword">open</a> <a id="7999" class="Keyword">import</a> <a id="8006" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8055" class="Keyword">open</a> <a id="8060" class="Keyword">import</a> <a id="8067" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8133" class="Keyword">open</a> <a id="8138" class="Keyword">import</a> <a id="8145" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8189" class="Keyword">open</a> <a id="8194" class="Keyword">import</a> <a id="8201" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8250" class="Keyword">open</a> <a id="8255" class="Keyword">import</a> <a id="8262" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8318" class="Keyword">open</a> <a id="8323" class="Keyword">import</a> <a id="8330" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8371" class="Keyword">open</a> <a id="8376" class="Keyword">import</a> <a id="8383" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8432" class="Keyword">open</a> <a id="8437" class="Keyword">import</a> <a id="8444" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8503" class="Keyword">open</a> <a id="8508" class="Keyword">import</a> <a id="8515" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8554" class="Keyword">open</a> <a id="8559" class="Keyword">import</a> <a id="8566" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8619" class="Keyword">open</a> <a id="8624" class="Keyword">import</a> <a id="8631" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="8688" class="Keyword">open</a> <a id="8693" class="Keyword">import</a> <a id="8700" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="8742" class="Keyword">open</a> <a id="8747" class="Keyword">import</a> <a id="8754" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="8805" class="Keyword">open</a> <a id="8810" class="Keyword">import</a> <a id="8817" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="8875" class="Keyword">open</a> <a id="8880" class="Keyword">import</a> <a id="8887" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="8951" class="Keyword">open</a> <a id="8956" class="Keyword">import</a> <a id="8963" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9016" class="Keyword">open</a> <a id="9021" class="Keyword">import</a> <a id="9028" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9081" class="Keyword">open</a> <a id="9086" class="Keyword">import</a> <a id="9093" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9154" class="Keyword">open</a> <a id="9159" class="Keyword">import</a> <a id="9166" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9224" class="Keyword">open</a> <a id="9229" class="Keyword">import</a> <a id="9236" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9285" class="Keyword">open</a> <a id="9290" class="Keyword">import</a> <a id="9297" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9340" class="Keyword">open</a> <a id="9345" class="Keyword">import</a> <a id="9352" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9396" class="Keyword">open</a> <a id="9401" class="Keyword">import</a> <a id="9408" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9455" class="Keyword">open</a> <a id="9460" class="Keyword">import</a> <a id="9467" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9528" class="Keyword">open</a> <a id="9533" class="Keyword">import</a> <a id="9540" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9603" class="Keyword">open</a> <a id="9608" class="Keyword">import</a> <a id="9615" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="9675" class="Keyword">open</a> <a id="9680" class="Keyword">import</a> <a id="9687" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="9741" class="Keyword">open</a> <a id="9746" class="Keyword">import</a> <a id="9753" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="9818" class="Keyword">open</a> <a id="9823" class="Keyword">import</a> <a id="9830" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="9938" class="Keyword">open</a> <a id="9943" class="Keyword">import</a> <a id="9950" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="9970" class="Keyword">open</a> <a id="9975" class="Keyword">import</a> <a id="9982" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10028" class="Keyword">open</a> <a id="10033" class="Keyword">import</a> <a id="10040" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10086" class="Keyword">open</a> <a id="10091" class="Keyword">import</a> <a id="10098" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10132" class="Keyword">open</a> <a id="10137" class="Keyword">import</a> <a id="10144" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10179" class="Keyword">open</a> <a id="10184" class="Keyword">import</a> <a id="10191" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10229" class="Keyword">open</a> <a id="10234" class="Keyword">import</a> <a id="10241" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10279" class="Keyword">open</a> <a id="10284" class="Keyword">import</a> <a id="10291" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10331" class="Keyword">open</a> <a id="10336" class="Keyword">import</a> <a id="10343" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10376" class="Keyword">open</a> <a id="10381" class="Keyword">import</a> <a id="10388" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10426" class="Keyword">open</a> <a id="10431" class="Keyword">import</a> <a id="10438" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10501" class="Keyword">open</a> <a id="10506" class="Keyword">import</a> <a id="10513" href="foundation.html" class="Module">foundation</a>
<a id="10524" class="Keyword">open</a> <a id="10529" class="Keyword">import</a> <a id="10536" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10554" class="Keyword">open</a> <a id="10559" class="Keyword">import</a> <a id="10566" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10585" class="Keyword">open</a> <a id="10590" class="Keyword">import</a> <a id="10597" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10616" class="Keyword">open</a> <a id="10621" class="Keyword">import</a> <a id="10628" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="10672" class="Keyword">open</a> <a id="10677" class="Keyword">import</a> <a id="10684" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="10709" class="Keyword">open</a> <a id="10714" class="Keyword">import</a> <a id="10721" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="10748" class="Keyword">open</a> <a id="10753" class="Keyword">import</a> <a id="10760" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="10777" class="Keyword">open</a> <a id="10782" class="Keyword">import</a> <a id="10789" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="10818" class="Keyword">open</a> <a id="10823" class="Keyword">import</a> <a id="10830" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="10886" class="Keyword">open</a> <a id="10891" class="Keyword">import</a> <a id="10898" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="10929" class="Keyword">open</a> <a id="10934" class="Keyword">import</a> <a id="10941" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="10995" class="Keyword">open</a> <a id="11000" class="Keyword">import</a> <a id="11007" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11035" class="Keyword">open</a> <a id="11040" class="Keyword">import</a> <a id="11047" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11077" class="Keyword">open</a> <a id="11082" class="Keyword">import</a> <a id="11089" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11109" class="Keyword">open</a> <a id="11114" class="Keyword">import</a> <a id="11121" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11166" class="Keyword">open</a> <a id="11171" class="Keyword">import</a> <a id="11178" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11215" class="Keyword">open</a> <a id="11220" class="Keyword">import</a> <a id="11227" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11262" class="Keyword">open</a> <a id="11267" class="Keyword">import</a> <a id="11274" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11332" class="Keyword">open</a> <a id="11337" class="Keyword">import</a> <a id="11344" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11382" class="Keyword">open</a> <a id="11387" class="Keyword">import</a> <a id="11394" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11428" class="Keyword">open</a> <a id="11433" class="Keyword">import</a> <a id="11440" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11469" class="Keyword">open</a> <a id="11474" class="Keyword">import</a> <a id="11481" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11504" class="Keyword">open</a> <a id="11509" class="Keyword">import</a> <a id="11516" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="11543" class="Keyword">open</a> <a id="11548" class="Keyword">import</a> <a id="11555" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11578" class="Keyword">open</a> <a id="11583" class="Keyword">import</a> <a id="11590" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="11632" class="Keyword">open</a> <a id="11637" class="Keyword">import</a> <a id="11644" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="11676" class="Keyword">open</a> <a id="11681" class="Keyword">import</a> <a id="11688" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="11715" class="Keyword">open</a> <a id="11720" class="Keyword">import</a> <a id="11727" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="11752" class="Keyword">open</a> <a id="11757" class="Keyword">import</a> <a id="11764" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="11793" class="Keyword">open</a> <a id="11798" class="Keyword">import</a> <a id="11805" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="11835" class="Keyword">open</a> <a id="11840" class="Keyword">import</a> <a id="11847" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="11874" class="Keyword">open</a> <a id="11879" class="Keyword">import</a> <a id="11886" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="11905" class="Keyword">open</a> <a id="11910" class="Keyword">import</a> <a id="11917" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="11963" class="Keyword">open</a> <a id="11968" class="Keyword">import</a> <a id="11975" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12017" class="Keyword">open</a> <a id="12022" class="Keyword">import</a> <a id="12029" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12061" class="Keyword">open</a> <a id="12066" class="Keyword">import</a> <a id="12073" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12103" class="Keyword">open</a> <a id="12108" class="Keyword">import</a> <a id="12115" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12141" class="Keyword">open</a> <a id="12146" class="Keyword">import</a> <a id="12153" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12187" class="Keyword">open</a> <a id="12192" class="Keyword">import</a> <a id="12199" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12229" class="Keyword">open</a> <a id="12234" class="Keyword">import</a> <a id="12241" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12268" class="Keyword">open</a> <a id="12273" class="Keyword">import</a> <a id="12280" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12312" class="Keyword">open</a> <a id="12317" class="Keyword">import</a> <a id="12324" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12358" class="Keyword">open</a> <a id="12363" class="Keyword">import</a> <a id="12370" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12393" class="Keyword">open</a> <a id="12398" class="Keyword">import</a> <a id="12405" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="12475" class="Keyword">open</a> <a id="12480" class="Keyword">import</a> <a id="12487" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="12557" class="Keyword">open</a> <a id="12562" class="Keyword">import</a> <a id="12569" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12596" class="Keyword">open</a> <a id="12601" class="Keyword">import</a> <a id="12608" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12636" class="Keyword">open</a> <a id="12641" class="Keyword">import</a> <a id="12648" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12685" class="Keyword">open</a> <a id="12690" class="Keyword">import</a> <a id="12697" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12745" class="Keyword">open</a> <a id="12750" class="Keyword">import</a> <a id="12757" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="12797" class="Keyword">open</a> <a id="12802" class="Keyword">import</a> <a id="12809" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="12831" class="Keyword">open</a> <a id="12836" class="Keyword">import</a> <a id="12843" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="12866" class="Keyword">open</a> <a id="12871" class="Keyword">import</a> <a id="12878" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="12903" class="Keyword">open</a> <a id="12908" class="Keyword">import</a> <a id="12915" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="12960" class="Keyword">open</a> <a id="12965" class="Keyword">import</a> <a id="12972" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13016" class="Keyword">open</a> <a id="13021" class="Keyword">import</a> <a id="13028" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13064" class="Keyword">open</a> <a id="13069" class="Keyword">import</a> <a id="13076" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13121" class="Keyword">open</a> <a id="13126" class="Keyword">import</a> <a id="13133" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13174" class="Keyword">open</a> <a id="13179" class="Keyword">import</a> <a id="13186" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13221" class="Keyword">open</a> <a id="13226" class="Keyword">import</a> <a id="13233" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13264" class="Keyword">open</a> <a id="13269" class="Keyword">import</a> <a id="13276" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13309" class="Keyword">open</a> <a id="13314" class="Keyword">import</a> <a id="13321" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13354" class="Keyword">open</a> <a id="13359" class="Keyword">import</a> <a id="13366" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13396" class="Keyword">open</a> <a id="13401" class="Keyword">import</a> <a id="13408" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13432" class="Keyword">open</a> <a id="13437" class="Keyword">import</a> <a id="13444" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13482" class="Keyword">open</a> <a id="13487" class="Keyword">import</a> <a id="13494" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13525" class="Keyword">open</a> <a id="13530" class="Keyword">import</a> <a id="13537" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13562" class="Keyword">open</a> <a id="13567" class="Keyword">import</a> <a id="13574" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13602" class="Keyword">open</a> <a id="13607" class="Keyword">import</a> <a id="13614" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13638" class="Keyword">open</a> <a id="13643" class="Keyword">import</a> <a id="13650" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13676" class="Keyword">open</a> <a id="13681" class="Keyword">import</a> <a id="13688" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="13723" class="Keyword">open</a> <a id="13728" class="Keyword">import</a> <a id="13735" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="13756" class="Keyword">open</a> <a id="13761" class="Keyword">import</a> <a id="13768" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="13817" class="Keyword">open</a> <a id="13822" class="Keyword">import</a> <a id="13829" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="13870" class="Keyword">open</a> <a id="13875" class="Keyword">import</a> <a id="13882" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="13932" class="Keyword">open</a> <a id="13937" class="Keyword">import</a> <a id="13944" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="13990" class="Keyword">open</a> <a id="13995" class="Keyword">import</a> <a id="14002" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14042" class="Keyword">open</a> <a id="14047" class="Keyword">import</a> <a id="14054" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14104" class="Keyword">open</a> <a id="14109" class="Keyword">import</a> <a id="14116" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14155" class="Keyword">open</a> <a id="14160" class="Keyword">import</a> <a id="14167" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14207" class="Keyword">open</a> <a id="14212" class="Keyword">import</a> <a id="14219" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14252" class="Keyword">open</a> <a id="14257" class="Keyword">import</a> <a id="14264" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14313" class="Keyword">open</a> <a id="14318" class="Keyword">import</a> <a id="14325" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14350" class="Keyword">open</a> <a id="14355" class="Keyword">import</a> <a id="14362" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14400" class="Keyword">open</a> <a id="14405" class="Keyword">import</a> <a id="14412" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14434" class="Keyword">open</a> <a id="14439" class="Keyword">import</a> <a id="14446" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14474" class="Keyword">open</a> <a id="14479" class="Keyword">import</a> <a id="14486" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14512" class="Keyword">open</a> <a id="14517" class="Keyword">import</a> <a id="14524" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14542" class="Keyword">open</a> <a id="14547" class="Keyword">import</a> <a id="14554" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14589" class="Keyword">open</a> <a id="14594" class="Keyword">import</a> <a id="14601" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="14628" class="Keyword">open</a> <a id="14633" class="Keyword">import</a> <a id="14640" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="14696" class="Keyword">open</a> <a id="14701" class="Keyword">import</a> <a id="14708" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="14737" class="Keyword">open</a> <a id="14742" class="Keyword">import</a> <a id="14749" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="14779" class="Keyword">open</a> <a id="14784" class="Keyword">import</a> <a id="14791" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="14818" class="Keyword">open</a> <a id="14823" class="Keyword">import</a> <a id="14830" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="14856" class="Keyword">open</a> <a id="14861" class="Keyword">import</a> <a id="14868" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="14895" class="Keyword">open</a> <a id="14900" class="Keyword">import</a> <a id="14907" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="14931" class="Keyword">open</a> <a id="14936" class="Keyword">import</a> <a id="14943" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="14966" class="Keyword">open</a> <a id="14971" class="Keyword">import</a> <a id="14978" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15005" class="Keyword">open</a> <a id="15010" class="Keyword">import</a> <a id="15017" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15049" class="Keyword">open</a> <a id="15054" class="Keyword">import</a> <a id="15061" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15096" class="Keyword">open</a> <a id="15101" class="Keyword">import</a> <a id="15108" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15139" class="Keyword">open</a> <a id="15144" class="Keyword">import</a> <a id="15151" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15184" class="Keyword">open</a> <a id="15189" class="Keyword">import</a> <a id="15196" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15230" class="Keyword">open</a> <a id="15235" class="Keyword">import</a> <a id="15242" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15282" class="Keyword">open</a> <a id="15287" class="Keyword">import</a> <a id="15294" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15325" class="Keyword">open</a> <a id="15330" class="Keyword">import</a> <a id="15337" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15369" class="Keyword">open</a> <a id="15374" class="Keyword">import</a> <a id="15381" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15412" class="Keyword">open</a> <a id="15417" class="Keyword">import</a> <a id="15424" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15441" class="Keyword">open</a> <a id="15446" class="Keyword">import</a> <a id="15453" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15478" class="Keyword">open</a> <a id="15483" class="Keyword">import</a> <a id="15490" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15519" class="Keyword">open</a> <a id="15524" class="Keyword">import</a> <a id="15531" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15556" class="Keyword">open</a> <a id="15561" class="Keyword">import</a> <a id="15568" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15589" class="Keyword">open</a> <a id="15594" class="Keyword">import</a> <a id="15601" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="15625" class="Keyword">open</a> <a id="15630" class="Keyword">import</a> <a id="15637" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="15657" class="Keyword">open</a> <a id="15662" class="Keyword">import</a> <a id="15669" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="15703" class="Keyword">open</a> <a id="15708" class="Keyword">import</a> <a id="15715" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="15753" class="Keyword">open</a> <a id="15758" class="Keyword">import</a> <a id="15765" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="15789" class="Keyword">open</a> <a id="15794" class="Keyword">import</a> <a id="15801" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="15828" class="Keyword">open</a> <a id="15833" class="Keyword">import</a> <a id="15840" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="15875" class="Keyword">open</a> <a id="15880" class="Keyword">import</a> <a id="15887" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="15908" class="Keyword">open</a> <a id="15913" class="Keyword">import</a> <a id="15920" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="15956" class="Keyword">open</a> <a id="15961" class="Keyword">import</a> <a id="15968" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16013" class="Keyword">open</a> <a id="16018" class="Keyword">import</a> <a id="16025" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16071" class="Keyword">open</a> <a id="16076" class="Keyword">import</a> <a id="16083" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16123" class="Keyword">open</a> <a id="16128" class="Keyword">import</a> <a id="16135" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16165" class="Keyword">open</a> <a id="16170" class="Keyword">import</a> <a id="16177" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16214" class="Keyword">open</a> <a id="16219" class="Keyword">import</a> <a id="16226" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16250" class="Keyword">open</a> <a id="16255" class="Keyword">import</a> <a id="16262" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16283" class="Keyword">open</a> <a id="16288" class="Keyword">import</a> <a id="16295" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16330" class="Keyword">open</a> <a id="16335" class="Keyword">import</a> <a id="16342" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16379" class="Keyword">open</a> <a id="16384" class="Keyword">import</a> <a id="16391" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16440" class="Keyword">open</a> <a id="16445" class="Keyword">import</a> <a id="16452" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16485" class="Keyword">open</a> <a id="16490" class="Keyword">import</a> <a id="16497" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16520" class="Keyword">open</a> <a id="16525" class="Keyword">import</a> <a id="16532" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="16555" class="Keyword">open</a> <a id="16560" class="Keyword">import</a> <a id="16567" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="16590" class="Keyword">open</a> <a id="16595" class="Keyword">import</a> <a id="16602" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="16630" class="Keyword">open</a> <a id="16635" class="Keyword">import</a> <a id="16642" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="16662" class="Keyword">open</a> <a id="16667" class="Keyword">import</a> <a id="16674" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="16695" class="Keyword">open</a> <a id="16700" class="Keyword">import</a> <a id="16707" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="16738" class="Keyword">open</a> <a id="16743" class="Keyword">import</a> <a id="16750" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="16777" class="Keyword">open</a> <a id="16782" class="Keyword">import</a> <a id="16789" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="16805" class="Keyword">open</a> <a id="16810" class="Keyword">import</a> <a id="16817" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="16848" class="Keyword">open</a> <a id="16853" class="Keyword">import</a> <a id="16860" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="16877" class="Keyword">open</a> <a id="16882" class="Keyword">import</a> <a id="16889" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="16911" class="Keyword">open</a> <a id="16916" class="Keyword">import</a> <a id="16923" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="16950" class="Keyword">open</a> <a id="16955" class="Keyword">import</a> <a id="16962" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="16985" class="Keyword">open</a> <a id="16990" class="Keyword">import</a> <a id="16997" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17024" class="Keyword">open</a> <a id="17029" class="Keyword">import</a> <a id="17036" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17069" class="Keyword">open</a> <a id="17074" class="Keyword">import</a> <a id="17081" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17121" class="Keyword">open</a> <a id="17126" class="Keyword">import</a> <a id="17133" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17154" class="Keyword">open</a> <a id="17159" class="Keyword">import</a> <a id="17166" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17195" class="Keyword">open</a> <a id="17200" class="Keyword">import</a> <a id="17207" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17245" class="Keyword">open</a> <a id="17250" class="Keyword">import</a> <a id="17257" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17277" class="Keyword">open</a> <a id="17282" class="Keyword">import</a> <a id="17289" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17313" class="Keyword">open</a> <a id="17318" class="Keyword">import</a> <a id="17325" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17352" class="Keyword">open</a> <a id="17357" class="Keyword">import</a> <a id="17364" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17396" class="Keyword">open</a> <a id="17401" class="Keyword">import</a> <a id="17408" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17438" class="Keyword">open</a> <a id="17443" class="Keyword">import</a> <a id="17450" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17476" class="Keyword">open</a> <a id="17481" class="Keyword">import</a> <a id="17488" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17515" class="Keyword">open</a> <a id="17520" class="Keyword">import</a> <a id="17527" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="17556" class="Keyword">open</a> <a id="17561" class="Keyword">import</a> <a id="17568" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="17591" class="Keyword">open</a> <a id="17596" class="Keyword">import</a> <a id="17603" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="17654" class="Keyword">open</a> <a id="17659" class="Keyword">import</a> <a id="17666" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="17709" class="Keyword">open</a> <a id="17714" class="Keyword">import</a> <a id="17721" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="17769" class="Keyword">open</a> <a id="17774" class="Keyword">import</a> <a id="17781" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="17819" class="Keyword">open</a> <a id="17824" class="Keyword">import</a> <a id="17831" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="17868" class="Keyword">open</a> <a id="17873" class="Keyword">import</a> <a id="17880" href="foundation.union.html" class="Module">foundation.union</a>
<a id="17897" class="Keyword">open</a> <a id="17902" class="Keyword">import</a> <a id="17909" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="17937" class="Keyword">open</a> <a id="17942" class="Keyword">import</a> <a id="17949" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="17985" class="Keyword">open</a> <a id="17990" class="Keyword">import</a> <a id="17997" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18035" class="Keyword">open</a> <a id="18040" class="Keyword">import</a> <a id="18047" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18080" class="Keyword">open</a> <a id="18085" class="Keyword">import</a> <a id="18092" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18113" class="Keyword">open</a> <a id="18118" class="Keyword">import</a> <a id="18125" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18179" class="Keyword">open</a> <a id="18184" class="Keyword">import</a> <a id="18191" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18213" class="Keyword">open</a> <a id="18218" class="Keyword">import</a> <a id="18225" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18260" class="Keyword">open</a> <a id="18265" class="Keyword">import</a> <a id="18272" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18302" class="Keyword">open</a> <a id="18307" class="Keyword">import</a> <a id="18314" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18353" class="Keyword">open</a> <a id="18358" class="Keyword">import</a> <a id="18365" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18419" class="Keyword">open</a> <a id="18424" class="Keyword">import</a> <a id="18431" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18477" class="Keyword">open</a> <a id="18482" class="Keyword">import</a> <a id="18489" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18540" class="Keyword">open</a> <a id="18545" class="Keyword">import</a> <a id="18552" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="18593" class="Keyword">open</a> <a id="18598" class="Keyword">import</a> <a id="18605" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="18650" class="Keyword">open</a> <a id="18655" class="Keyword">import</a> <a id="18662" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="18707" class="Keyword">open</a> <a id="18712" class="Keyword">import</a> <a id="18719" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="18755" class="Keyword">open</a> <a id="18760" class="Keyword">import</a> <a id="18767" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="18803" class="Keyword">open</a> <a id="18808" class="Keyword">import</a> <a id="18815" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="18880" class="Keyword">open</a> <a id="18885" class="Keyword">import</a> <a id="18892" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="18947" class="Keyword">open</a> <a id="18952" class="Keyword">import</a> <a id="18959" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="18999" class="Keyword">open</a> <a id="19004" class="Keyword">import</a> <a id="19011" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19055" class="Keyword">open</a> <a id="19060" class="Keyword">import</a> <a id="19067" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19112" class="Keyword">open</a> <a id="19117" class="Keyword">import</a> <a id="19124" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19165" class="Keyword">open</a> <a id="19170" class="Keyword">import</a> <a id="19177" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19217" class="Keyword">open</a> <a id="19222" class="Keyword">import</a> <a id="19229" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19256" class="Keyword">open</a> <a id="19261" class="Keyword">import</a> <a id="19268" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19304" class="Keyword">open</a> <a id="19309" class="Keyword">import</a> <a id="19316" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19343" class="Keyword">open</a> <a id="19348" class="Keyword">import</a> <a id="19355" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19392" class="Keyword">open</a> <a id="19397" class="Keyword">import</a> <a id="19404" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19432" class="Keyword">open</a> <a id="19437" class="Keyword">import</a> <a id="19444" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19463" class="Keyword">open</a> <a id="19468" class="Keyword">import</a> <a id="19475" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19515" class="Keyword">open</a> <a id="19520" class="Keyword">import</a> <a id="19527" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19559" class="Keyword">open</a> <a id="19564" class="Keyword">import</a> <a id="19571" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="19619" class="Keyword">open</a> <a id="19624" class="Keyword">import</a> <a id="19631" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="19654" class="Keyword">open</a> <a id="19659" class="Keyword">import</a> <a id="19666" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="19690" class="Keyword">open</a> <a id="19695" class="Keyword">import</a> <a id="19702" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="19742" class="Keyword">open</a> <a id="19747" class="Keyword">import</a> <a id="19754" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="19797" class="Keyword">open</a> <a id="19802" class="Keyword">import</a> <a id="19809" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="19843" class="Keyword">open</a> <a id="19848" class="Keyword">import</a> <a id="19855" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="19887" class="Keyword">open</a> <a id="19892" class="Keyword">import</a> <a id="19899" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="19929" class="Keyword">open</a> <a id="19934" class="Keyword">import</a> <a id="19941" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="19975" class="Keyword">open</a> <a id="19980" class="Keyword">import</a> <a id="19987" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20022" class="Keyword">open</a> <a id="20027" class="Keyword">import</a> <a id="20034" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20071" class="Keyword">open</a> <a id="20076" class="Keyword">import</a> <a id="20083" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20110" class="Keyword">open</a> <a id="20115" class="Keyword">import</a> <a id="20122" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20150" class="Keyword">open</a> <a id="20155" class="Keyword">import</a> <a id="20162" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20211" class="Keyword">open</a> <a id="20216" class="Keyword">import</a> <a id="20223" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20269" class="Keyword">open</a> <a id="20274" class="Keyword">import</a> <a id="20281" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20321" class="Keyword">open</a> <a id="20326" class="Keyword">import</a> <a id="20333" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20371" class="Keyword">open</a> <a id="20376" class="Keyword">import</a> <a id="20383" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20412" class="Keyword">open</a> <a id="20417" class="Keyword">import</a> <a id="20424" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20454" class="Keyword">open</a> <a id="20459" class="Keyword">import</a> <a id="20466" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20497" class="Keyword">open</a> <a id="20502" class="Keyword">import</a> <a id="20509" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="20549" class="Keyword">open</a> <a id="20554" class="Keyword">import</a> <a id="20561" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="20587" class="Keyword">open</a> <a id="20592" class="Keyword">import</a> <a id="20599" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="20654" class="Keyword">open</a> <a id="20659" class="Keyword">import</a> <a id="20666" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="20717" class="Keyword">open</a> <a id="20722" class="Keyword">import</a> <a id="20729" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="20774" class="Keyword">open</a> <a id="20779" class="Keyword">import</a> <a id="20786" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="20840" class="Keyword">open</a> <a id="20845" class="Keyword">import</a> <a id="20852" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="20879" class="Keyword">open</a> <a id="20884" class="Keyword">import</a> <a id="20891" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="20924" class="Keyword">open</a> <a id="20929" class="Keyword">import</a> <a id="20936" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="20967" class="Keyword">open</a> <a id="20972" class="Keyword">import</a> <a id="20979" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21016" class="Keyword">open</a> <a id="21021" class="Keyword">import</a> <a id="21028" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21053" class="Keyword">open</a> <a id="21058" class="Keyword">import</a> <a id="21065" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21097" class="Keyword">open</a> <a id="21102" class="Keyword">import</a> <a id="21109" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21144" class="Keyword">open</a> <a id="21149" class="Keyword">import</a> <a id="21156" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21185" class="Keyword">open</a> <a id="21190" class="Keyword">import</a> <a id="21197" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21223" class="Keyword">open</a> <a id="21228" class="Keyword">import</a> <a id="21235" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21263" class="Keyword">open</a> <a id="21268" class="Keyword">import</a> <a id="21275" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21300" class="Keyword">open</a> <a id="21305" class="Keyword">import</a> <a id="21312" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21333" class="Keyword">open</a> <a id="21338" class="Keyword">import</a> <a id="21345" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21381" class="Keyword">open</a> <a id="21386" class="Keyword">import</a> <a id="21393" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21436" class="Keyword">open</a> <a id="21441" class="Keyword">import</a> <a id="21448" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21473" class="Keyword">open</a> <a id="21478" class="Keyword">import</a> <a id="21485" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21516" class="Keyword">open</a> <a id="21521" class="Keyword">import</a> <a id="21528" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21560" class="Keyword">open</a> <a id="21565" class="Keyword">import</a> <a id="21572" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="21606" class="Keyword">open</a> <a id="21611" class="Keyword">import</a> <a id="21618" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="21674" class="Keyword">open</a> <a id="21679" class="Keyword">import</a> <a id="21686" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="21739" class="Keyword">open</a> <a id="21744" class="Keyword">import</a> <a id="21751" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="21778" class="Keyword">open</a> <a id="21783" class="Keyword">import</a> <a id="21790" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="21835" class="Keyword">open</a> <a id="21840" class="Keyword">import</a> <a id="21847" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="21909" class="Keyword">open</a> <a id="21914" class="Keyword">import</a> <a id="21921" href="graph-theory.html" class="Module">graph-theory</a>
<a id="21934" class="Keyword">open</a> <a id="21939" class="Keyword">import</a> <a id="21946" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="21987" class="Keyword">open</a> <a id="21992" class="Keyword">import</a> <a id="21999" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22028" class="Keyword">open</a> <a id="22033" class="Keyword">import</a> <a id="22040" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22085" class="Keyword">open</a> <a id="22090" class="Keyword">import</a> <a id="22097" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22141" class="Keyword">open</a> <a id="22146" class="Keyword">import</a> <a id="22153" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="22180" class="Keyword">open</a> <a id="22185" class="Keyword">import</a> <a id="22192" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="22233" class="Keyword">open</a> <a id="22238" class="Keyword">import</a> <a id="22245" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="22268" class="Keyword">open</a> <a id="22273" class="Keyword">import</a> <a id="22280" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="22329" class="Keyword">open</a> <a id="22334" class="Keyword">import</a> <a id="22341" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="22380" class="Keyword">open</a> <a id="22385" class="Keyword">import</a> <a id="22392" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="22433" class="Keyword">open</a> <a id="22438" class="Keyword">import</a> <a id="22445" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22489" class="Keyword">open</a> <a id="22494" class="Keyword">import</a> <a id="22501" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22538" class="Keyword">open</a> <a id="22543" class="Keyword">import</a> <a id="22550" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="22572" class="Keyword">open</a> <a id="22577" class="Keyword">import</a> <a id="22584" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="22614" class="Keyword">open</a> <a id="22619" class="Keyword">import</a> <a id="22626" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="22665" class="Keyword">open</a> <a id="22670" class="Keyword">import</a> <a id="22677" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="22715" class="Keyword">open</a> <a id="22720" class="Keyword">import</a> <a id="22727" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="22758" class="Keyword">open</a> <a id="22763" class="Keyword">import</a> <a id="22770" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="22797" class="Keyword">open</a> <a id="22802" class="Keyword">import</a> <a id="22809" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="22867" class="Keyword">open</a> <a id="22872" class="Keyword">import</a> <a id="22879" href="group-theory.html" class="Module">group-theory</a>
<a id="22892" class="Keyword">open</a> <a id="22897" class="Keyword">import</a> <a id="22904" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="22932" class="Keyword">open</a> <a id="22937" class="Keyword">import</a> <a id="22944" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="22975" class="Keyword">open</a> <a id="22980" class="Keyword">import</a> <a id="22987" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="23023" class="Keyword">open</a> <a id="23028" class="Keyword">import</a> <a id="23035" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="23086" class="Keyword">open</a> <a id="23091" class="Keyword">import</a> <a id="23098" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="23131" class="Keyword">open</a> <a id="23136" class="Keyword">import</a> <a id="23143" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="23175" class="Keyword">open</a> <a id="23180" class="Keyword">import</a> <a id="23187" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="23223" class="Keyword">open</a> <a id="23228" class="Keyword">import</a> <a id="23235" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="23264" class="Keyword">open</a> <a id="23269" class="Keyword">import</a> <a id="23276" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="23312" class="Keyword">open</a> <a id="23317" class="Keyword">import</a> <a id="23324" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="23353" class="Keyword">open</a> <a id="23358" class="Keyword">import</a> <a id="23365" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="23397" class="Keyword">open</a> <a id="23402" class="Keyword">import</a> <a id="23409" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="23434" class="Keyword">open</a> <a id="23439" class="Keyword">import</a> <a id="23446" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="23477" class="Keyword">open</a> <a id="23482" class="Keyword">import</a> <a id="23489" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="23536" class="Keyword">open</a> <a id="23541" class="Keyword">import</a> <a id="23548" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="23581" class="Keyword">open</a> <a id="23586" class="Keyword">import</a> <a id="23593" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="23633" class="Keyword">open</a> <a id="23638" class="Keyword">import</a> <a id="23645" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="23682" class="Keyword">open</a> <a id="23687" class="Keyword">import</a> <a id="23694" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="23730" class="Keyword">open</a> <a id="23735" class="Keyword">import</a> <a id="23742" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="23774" class="Keyword">open</a> <a id="23779" class="Keyword">import</a> <a id="23786" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="23813" class="Keyword">open</a> <a id="23818" class="Keyword">import</a> <a id="23825" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="23845" class="Keyword">open</a> <a id="23850" class="Keyword">import</a> <a id="23857" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="23884" class="Keyword">open</a> <a id="23889" class="Keyword">import</a> <a id="23896" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="23938" class="Keyword">open</a> <a id="23943" class="Keyword">import</a> <a id="23950" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="23997" class="Keyword">open</a> <a id="24002" class="Keyword">import</a> <a id="24009" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="24050" class="Keyword">open</a> <a id="24055" class="Keyword">import</a> <a id="24062" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="24096" class="Keyword">open</a> <a id="24101" class="Keyword">import</a> <a id="24108" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="24143" class="Keyword">open</a> <a id="24148" class="Keyword">import</a> <a id="24155" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="24193" class="Keyword">open</a> <a id="24198" class="Keyword">import</a> <a id="24205" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="24237" class="Keyword">open</a> <a id="24242" class="Keyword">import</a> <a id="24249" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="24290" class="Keyword">open</a> <a id="24295" class="Keyword">import</a> <a id="24302" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="24343" class="Keyword">open</a> <a id="24348" class="Keyword">import</a> <a id="24355" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="24395" class="Keyword">open</a> <a id="24400" class="Keyword">import</a> <a id="24407" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="24440" class="Keyword">open</a> <a id="24445" class="Keyword">import</a> <a id="24452" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="24489" class="Keyword">open</a> <a id="24494" class="Keyword">import</a> <a id="24501" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="24546" class="Keyword">open</a> <a id="24551" class="Keyword">import</a> <a id="24558" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="24586" class="Keyword">open</a> <a id="24591" class="Keyword">import</a> <a id="24598" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="24619" class="Keyword">open</a> <a id="24624" class="Keyword">import</a> <a id="24631" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="24665" class="Keyword">open</a> <a id="24670" class="Keyword">import</a> <a id="24677" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="24711" class="Keyword">open</a> <a id="24716" class="Keyword">import</a> <a id="24723" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="24758" class="Keyword">open</a> <a id="24763" class="Keyword">import</a> <a id="24770" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="24812" class="Keyword">open</a> <a id="24817" class="Keyword">import</a> <a id="24824" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="24859" class="Keyword">open</a> <a id="24864" class="Keyword">import</a> <a id="24871" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="24910" class="Keyword">open</a> <a id="24915" class="Keyword">import</a> <a id="24922" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="24959" class="Keyword">open</a> <a id="24964" class="Keyword">import</a> <a id="24971" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="24995" class="Keyword">open</a> <a id="25000" class="Keyword">import</a> <a id="25007" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="25032" class="Keyword">open</a> <a id="25037" class="Keyword">import</a> <a id="25044" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="25075" class="Keyword">open</a> <a id="25080" class="Keyword">import</a> <a id="25087" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="25138" class="Keyword">open</a> <a id="25143" class="Keyword">import</a> <a id="25150" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="25173" class="Keyword">open</a> <a id="25178" class="Keyword">import</a> <a id="25185" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="25233" class="Keyword">open</a> <a id="25238" class="Keyword">import</a> <a id="25245" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="25275" class="Keyword">open</a> <a id="25280" class="Keyword">import</a> <a id="25287" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="25357" class="Keyword">open</a> <a id="25362" class="Keyword">import</a> <a id="25369" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="25384" class="Keyword">open</a> <a id="25389" class="Keyword">import</a> <a id="25396" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="25429" class="Keyword">open</a> <a id="25434" class="Keyword">import</a> <a id="25441" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="25473" class="Keyword">open</a> <a id="25478" class="Keyword">import</a> <a id="25485" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="25527" class="Keyword">open</a> <a id="25532" class="Keyword">import</a> <a id="25539" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="25577" class="Keyword">open</a> <a id="25582" class="Keyword">import</a> <a id="25589" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="25626" class="Keyword">open</a> <a id="25631" class="Keyword">import</a> <a id="25638" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="25671" class="Keyword">open</a> <a id="25676" class="Keyword">import</a> <a id="25683" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="25707" class="Keyword">open</a> <a id="25712" class="Keyword">import</a> <a id="25719" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="25758" class="Keyword">open</a> <a id="25763" class="Keyword">import</a> <a id="25770" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="25816" class="Keyword">open</a> <a id="25821" class="Keyword">import</a> <a id="25828" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="25873" class="Keyword">open</a> <a id="25878" class="Keyword">import</a> <a id="25885" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="25923" class="Keyword">open</a> <a id="25928" class="Keyword">import</a> <a id="25935" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="25967" class="Keyword">open</a> <a id="25972" class="Keyword">import</a> <a id="25979" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="26032" class="Keyword">open</a> <a id="26037" class="Keyword">import</a> <a id="26044" href="order-theory.html" class="Module">order-theory</a>
<a id="26057" class="Keyword">open</a> <a id="26062" class="Keyword">import</a> <a id="26069" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="26096" class="Keyword">open</a> <a id="26101" class="Keyword">import</a> <a id="26108" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="26138" class="Keyword">open</a> <a id="26143" class="Keyword">import</a> <a id="26150" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="26183" class="Keyword">open</a> <a id="26188" class="Keyword">import</a> <a id="26195" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="26231" class="Keyword">open</a> <a id="26236" class="Keyword">import</a> <a id="26243" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="26270" class="Keyword">open</a> <a id="26275" class="Keyword">import</a> <a id="26282" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="26312" class="Keyword">open</a> <a id="26317" class="Keyword">import</a> <a id="26324" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="26360" class="Keyword">open</a> <a id="26365" class="Keyword">import</a> <a id="26372" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="26414" class="Keyword">open</a> <a id="26419" class="Keyword">import</a> <a id="26426" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="26458" class="Keyword">open</a> <a id="26463" class="Keyword">import</a> <a id="26470" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="26501" class="Keyword">open</a> <a id="26506" class="Keyword">import</a> <a id="26513" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="26539" class="Keyword">open</a> <a id="26544" class="Keyword">import</a> <a id="26551" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="26580" class="Keyword">open</a> <a id="26585" class="Keyword">import</a> <a id="26592" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="26629" class="Keyword">open</a> <a id="26634" class="Keyword">import</a> <a id="26641" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="26681" class="Keyword">open</a> <a id="26686" class="Keyword">import</a> <a id="26693" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="26715" class="Keyword">open</a> <a id="26720" class="Keyword">import</a> <a id="26727" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="26762" class="Keyword">open</a> <a id="26767" class="Keyword">import</a> <a id="26774" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="26812" class="Keyword">open</a> <a id="26817" class="Keyword">import</a> <a id="26824" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="26863" class="Keyword">open</a> <a id="26868" class="Keyword">import</a> <a id="26875" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="26910" class="Keyword">open</a> <a id="26915" class="Keyword">import</a> <a id="26922" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="26957" class="Keyword">open</a> <a id="26962" class="Keyword">import</a> <a id="26969" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="27007" class="Keyword">open</a> <a id="27012" class="Keyword">import</a> <a id="27019" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="27050" class="Keyword">open</a> <a id="27055" class="Keyword">import</a> <a id="27062" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="27104" class="Keyword">open</a> <a id="27109" class="Keyword">import</a> <a id="27116" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="27161" class="Keyword">open</a> <a id="27166" class="Keyword">import</a> <a id="27173" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="27206" class="Keyword">open</a> <a id="27211" class="Keyword">import</a> <a id="27218" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="27238" class="Keyword">open</a> <a id="27243" class="Keyword">import</a> <a id="27250" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="27273" class="Keyword">open</a> <a id="27278" class="Keyword">import</a> <a id="27285" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="27308" class="Keyword">open</a> <a id="27313" class="Keyword">import</a> <a id="27320" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="27346" class="Keyword">open</a> <a id="27351" class="Keyword">import</a> <a id="27358" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="27384" class="Keyword">open</a> <a id="27389" class="Keyword">import</a> <a id="27396" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="27452" class="Keyword">open</a> <a id="27457" class="Keyword">import</a> <a id="27464" href="polytopes.html" class="Module">polytopes</a>
<a id="27474" class="Keyword">open</a> <a id="27479" class="Keyword">import</a> <a id="27486" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="27544" class="Keyword">open</a> <a id="27549" class="Keyword">import</a> <a id="27556" href="ring-theory.html" class="Module">ring-theory</a>
<a id="27568" class="Keyword">open</a> <a id="27573" class="Keyword">import</a> <a id="27580" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="27617" class="Keyword">open</a> <a id="27622" class="Keyword">import</a> <a id="27629" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="27656" class="Keyword">open</a> <a id="27661" class="Keyword">import</a> <a id="27668" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="27700" class="Keyword">open</a> <a id="27705" class="Keyword">import</a> <a id="27712" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="27758" class="Keyword">open</a> <a id="27763" class="Keyword">import</a> <a id="27770" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="27795" class="Keyword">open</a> <a id="27800" class="Keyword">import</a> <a id="27807" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="27850" class="Keyword">open</a> <a id="27855" class="Keyword">import</a> <a id="27862" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="27900" class="Keyword">open</a> <a id="27905" class="Keyword">import</a> <a id="27912" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="27943" class="Keyword">open</a> <a id="27948" class="Keyword">import</a> <a id="27955" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="27987" class="Keyword">open</a> <a id="27992" class="Keyword">import</a> <a id="27999" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="28028" class="Keyword">open</a> <a id="28033" class="Keyword">import</a> <a id="28040" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="28077" class="Keyword">open</a> <a id="28082" class="Keyword">import</a> <a id="28089" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="28118" class="Keyword">open</a> <a id="28123" class="Keyword">import</a> <a id="28130" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="28157" class="Keyword">open</a> <a id="28162" class="Keyword">import</a> <a id="28169" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="28206" class="Keyword">open</a> <a id="28211" class="Keyword">import</a> <a id="28218" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="28245" class="Keyword">open</a> <a id="28250" class="Keyword">import</a> <a id="28257" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="28290" class="Keyword">open</a> <a id="28295" class="Keyword">import</a> <a id="28302" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="28320" class="Keyword">open</a> <a id="28325" class="Keyword">import</a> <a id="28332" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="28386" class="Keyword">open</a> <a id="28391" class="Keyword">import</a> <a id="28398" href="set-theory.html" class="Module">set-theory</a>
<a id="28409" class="Keyword">open</a> <a id="28414" class="Keyword">import</a> <a id="28421" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="28447" class="Keyword">open</a> <a id="28452" class="Keyword">import</a> <a id="28459" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="28521" class="Keyword">open</a> <a id="28526" class="Keyword">import</a> <a id="28533" href="structured-types.html" class="Module">structured-types</a>
<a id="28550" class="Keyword">open</a> <a id="28555" class="Keyword">import</a> <a id="28562" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="28606" class="Keyword">open</a> <a id="28611" class="Keyword">import</a> <a id="28618" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="28682" class="Keyword">open</a> <a id="28687" class="Keyword">import</a> <a id="28694" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="28740" class="Keyword">open</a> <a id="28745" class="Keyword">import</a> <a id="28752" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="28776" class="Keyword">open</a> <a id="28781" class="Keyword">import</a> <a id="28788" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="28857" class="Keyword">open</a> <a id="28862" class="Keyword">import</a> <a id="28869" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="28903" class="Keyword">open</a> <a id="28908" class="Keyword">import</a> <a id="28915" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="28976" class="Keyword">open</a> <a id="28981" class="Keyword">import</a> <a id="28988" href="structured-types.morphisms-wild-unital-magmas.html" class="Module">structured-types.morphisms-wild-unital-magmas</a>
<a id="29034" class="Keyword">open</a> <a id="29039" class="Keyword">import</a> <a id="29046" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="29091" class="Keyword">open</a> <a id="29096" class="Keyword">import</a> <a id="29103" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="29141" class="Keyword">open</a> <a id="29146" class="Keyword">import</a> <a id="29153" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="29196" class="Keyword">open</a> <a id="29201" class="Keyword">import</a> <a id="29208" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="29244" class="Keyword">open</a> <a id="29249" class="Keyword">import</a> <a id="29256" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="29286" class="Keyword">open</a> <a id="29291" class="Keyword">import</a> <a id="29298" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="29329" class="Keyword">open</a> <a id="29334" class="Keyword">import</a> <a id="29341" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="29392" class="Keyword">open</a> <a id="29397" class="Keyword">import</a> <a id="29404" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="29459" class="Keyword">open</a> <a id="29464" class="Keyword">import</a> <a id="29471" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="29500" class="Keyword">open</a> <a id="29505" class="Keyword">import</a> <a id="29512" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="29540" class="Keyword">open</a> <a id="29545" class="Keyword">import</a> <a id="29552" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="29582" class="Keyword">open</a> <a id="29587" class="Keyword">import</a> <a id="29594" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="29628" class="Keyword">open</a> <a id="29633" class="Keyword">import</a> <a id="29640" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
<a id="29673" class="Keyword">open</a> <a id="29678" class="Keyword">import</a> <a id="29685" href="structured-types.wild-unital-magmas.html" class="Module">structured-types.wild-unital-magmas</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="29764" class="Keyword">open</a> <a id="29769" class="Keyword">import</a> <a id="29776" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="29802" class="Keyword">open</a> <a id="29807" class="Keyword">import</a> <a id="29814" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="29853" class="Keyword">open</a> <a id="29858" class="Keyword">import</a> <a id="29865" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="29903" class="Keyword">open</a> <a id="29908" class="Keyword">import</a> <a id="29915" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="29961" class="Keyword">open</a> <a id="29966" class="Keyword">import</a> <a id="29973" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="30010" class="Keyword">open</a> <a id="30015" class="Keyword">import</a> <a id="30022" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="30062" class="Keyword">open</a> <a id="30067" class="Keyword">import</a> <a id="30074" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="30113" class="Keyword">open</a> <a id="30118" class="Keyword">import</a> <a id="30125" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="30158" class="Keyword">open</a> <a id="30163" class="Keyword">import</a> <a id="30170" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="30205" class="Keyword">open</a> <a id="30210" class="Keyword">import</a> <a id="30217" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="30256" class="Keyword">open</a> <a id="30261" class="Keyword">import</a> <a id="30268" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="30313" class="Keyword">open</a> <a id="30318" class="Keyword">import</a> <a id="30325" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="30377" class="Keyword">open</a> <a id="30382" class="Keyword">import</a> <a id="30389" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="30442" class="Keyword">open</a> <a id="30447" class="Keyword">import</a> <a id="30454" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="30502" class="Keyword">open</a> <a id="30507" class="Keyword">import</a> <a id="30514" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="30554" class="Keyword">open</a> <a id="30559" class="Keyword">import</a> <a id="30566" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="30613" class="Keyword">open</a> <a id="30618" class="Keyword">import</a> <a id="30625" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="30666" class="Keyword">open</a> <a id="30671" class="Keyword">import</a> <a id="30678" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="30716" class="Keyword">open</a> <a id="30721" class="Keyword">import</a> <a id="30728" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="30773" class="Keyword">open</a> <a id="30778" class="Keyword">import</a> <a id="30785" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="30834" class="Keyword">open</a> <a id="30839" class="Keyword">import</a> <a id="30846" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="30923" class="Keyword">open</a> <a id="30928" class="Keyword">import</a> <a id="30935" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="30987" class="Keyword">open</a> <a id="30992" class="Keyword">import</a> <a id="30999" href="type-theories.html" class="Module">type-theories</a>
<a id="31013" class="Keyword">open</a> <a id="31018" class="Keyword">import</a> <a id="31025" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="31067" class="Keyword">open</a> <a id="31072" class="Keyword">import</a> <a id="31079" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="31117" class="Keyword">open</a> <a id="31122" class="Keyword">import</a> <a id="31129" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="31175" class="Keyword">open</a> <a id="31180" class="Keyword">import</a> <a id="31187" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="31234" class="Keyword">open</a> <a id="31239" class="Keyword">import</a> <a id="31246" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="31281" class="Keyword">open</a> <a id="31286" class="Keyword">import</a> <a id="31293" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="31371" class="Keyword">open</a> <a id="31376" class="Keyword">import</a> <a id="31383" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="31407" class="Keyword">open</a> <a id="31412" class="Keyword">import</a> <a id="31419" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="31472" class="Keyword">open</a> <a id="31477" class="Keyword">import</a> <a id="31484" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="31527" class="Keyword">open</a> <a id="31532" class="Keyword">import</a> <a id="31539" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="31579" class="Keyword">open</a> <a id="31584" class="Keyword">import</a> <a id="31591" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="31630" class="Keyword">open</a> <a id="31635" class="Keyword">import</a> <a id="31642" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="31690" class="Keyword">open</a> <a id="31695" class="Keyword">import</a> <a id="31702" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="31749" class="Keyword">open</a> <a id="31754" class="Keyword">import</a> <a id="31761" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="31813" class="Keyword">open</a> <a id="31818" class="Keyword">import</a> <a id="31825" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="31869" class="Keyword">open</a> <a id="31874" class="Keyword">import</a> <a id="31881" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="31921" class="Keyword">open</a> <a id="31926" class="Keyword">import</a> <a id="31933" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="31985" class="Keyword">open</a> <a id="31990" class="Keyword">import</a> <a id="31997" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="32051" class="Keyword">open</a> <a id="32056" class="Keyword">import</a> <a id="32063" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="32111" class="Keyword">open</a> <a id="32116" class="Keyword">import</a> <a id="32123" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="32162" class="Keyword">open</a> <a id="32167" class="Keyword">import</a> <a id="32174" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="32207" class="Keyword">open</a> <a id="32212" class="Keyword">import</a> <a id="32219" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="32249" class="Keyword">open</a> <a id="32254" class="Keyword">import</a> <a id="32261" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="32320" class="Keyword">open</a> <a id="32325" class="Keyword">import</a> <a id="32332" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="32387" class="Keyword">open</a> <a id="32392" class="Keyword">import</a> <a id="32399" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="32446" class="Keyword">open</a> <a id="32451" class="Keyword">import</a> <a id="32458" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="32501" class="Keyword">open</a> <a id="32506" class="Keyword">import</a> <a id="32513" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="32558" class="Keyword">open</a> <a id="32563" class="Keyword">import</a> <a id="32570" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="32619" class="Keyword">open</a> <a id="32624" class="Keyword">import</a> <a id="32631" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="32682" class="Keyword">open</a> <a id="32687" class="Keyword">import</a> <a id="32694" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="32772" class="Keyword">open</a> <a id="32777" class="Keyword">import</a> <a id="32784" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="32824" class="Keyword">open</a> <a id="32829" class="Keyword">import</a> <a id="32836" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="32893" class="Keyword">open</a> <a id="32898" class="Keyword">import</a> <a id="32905" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="32940" class="Keyword">open</a> <a id="32945" class="Keyword">import</a> <a id="32952" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="32998" class="Keyword">open</a> <a id="33003" class="Keyword">import</a> <a id="33010" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="33065" class="Keyword">open</a> <a id="33070" class="Keyword">import</a> <a id="33077" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="33120" class="Keyword">open</a> <a id="33125" class="Keyword">import</a> <a id="33132" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="33191" class="Keyword">open</a> <a id="33196" class="Keyword">import</a> <a id="33203" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="33240" class="Keyword">open</a> <a id="33245" class="Keyword">import</a> <a id="33252" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="33293" class="Keyword">open</a> <a id="33298" class="Keyword">import</a> <a id="33305" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="33344" class="Keyword">open</a> <a id="33349" class="Keyword">import</a> <a id="33356" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="33394" class="Keyword">open</a> <a id="33399" class="Keyword">import</a> <a id="33406" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="33458" class="Keyword">open</a> <a id="33463" class="Keyword">import</a> <a id="33470" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="33515" class="Keyword">open</a> <a id="33520" class="Keyword">import</a> <a id="33527" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="33564" class="Keyword">open</a> <a id="33569" class="Keyword">import</a> <a id="33576" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="33625" class="Keyword">open</a> <a id="33630" class="Keyword">import</a> <a id="33637" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="33676" class="Keyword">open</a> <a id="33681" class="Keyword">import</a> <a id="33688" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="33726" class="Keyword">open</a> <a id="33731" class="Keyword">import</a> <a id="33738" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="33793" class="Keyword">open</a> <a id="33798" class="Keyword">import</a> <a id="33805" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="33844" class="Keyword">open</a> <a id="33849" class="Keyword">import</a> <a id="33856" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="33904" class="Keyword">open</a> <a id="33909" class="Keyword">import</a> <a id="33916" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="33963" class="Keyword">open</a> <a id="33968" class="Keyword">import</a> <a id="33975" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="34013" class="Keyword">open</a> <a id="34018" class="Keyword">import</a> <a id="34025" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="34055" class="Keyword">open</a> <a id="34060" class="Keyword">import</a> <a id="34067" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="34124" class="Keyword">open</a> <a id="34129" class="Keyword">import</a> <a id="34136" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="34190" class="Keyword">open</a> <a id="34195" class="Keyword">import</a> <a id="34202" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="34232" class="Keyword">open</a> <a id="34237" class="Keyword">import</a> <a id="34244" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="34307" class="Keyword">open</a> <a id="34312" class="Keyword">import</a> <a id="34319" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="34362" class="Keyword">open</a> <a id="34367" class="Keyword">import</a> <a id="34374" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="34409" class="Keyword">open</a> <a id="34414" class="Keyword">import</a> <a id="34421" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="34461" class="Keyword">open</a> <a id="34466" class="Keyword">import</a> <a id="34473" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="34518" class="Keyword">open</a> <a id="34523" class="Keyword">import</a> <a id="34530" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="34580" class="Keyword">open</a> <a id="34585" class="Keyword">import</a> <a id="34592" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="34630" class="Keyword">open</a> <a id="34635" class="Keyword">import</a> <a id="34642" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="34691" class="Keyword">open</a> <a id="34696" class="Keyword">import</a> <a id="34703" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="34750" class="Keyword">open</a> <a id="34755" class="Keyword">import</a> <a id="34762" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="34825" class="Keyword">open</a> <a id="34830" class="Keyword">import</a> <a id="34837" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="34869" class="Keyword">open</a> <a id="34874" class="Keyword">import</a> <a id="34881" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="34934" class="Keyword">open</a> <a id="34939" class="Keyword">import</a> <a id="34946" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="34992" class="Keyword">open</a> <a id="34997" class="Keyword">import</a> <a id="35004" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="35050" class="Keyword">open</a> <a id="35055" class="Keyword">import</a> <a id="35062" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="35110" class="Keyword">open</a> <a id="35115" class="Keyword">import</a> <a id="35122" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="35162" class="Keyword">open</a> <a id="35167" class="Keyword">import</a> <a id="35174" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="35219" class="Keyword">open</a> <a id="35224" class="Keyword">import</a> <a id="35231" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>