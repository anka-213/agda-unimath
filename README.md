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

<pre class="Agda"><a id="2976" class="Symbol">{-#</a> <a id="2980" class="Keyword">OPTIONS</a> <a id="2988" class="Pragma">--without-K</a> <a id="3000" class="Pragma">--exact-split</a> <a id="3014" class="Pragma">--guardedness</a> <a id="3028" class="Symbol">#-}</a>
</pre>
See the list of all Agda modules [here](everything.html).

## Category theory

<pre class="Agda"><a id="3124" class="Keyword">open</a> <a id="3129" class="Keyword">import</a> <a id="3136" href="category-theory.html" class="Module">category-theory</a>
<a id="3152" class="Keyword">open</a> <a id="3157" class="Keyword">import</a> <a id="3164" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="3212" class="Keyword">open</a> <a id="3217" class="Keyword">import</a> <a id="3224" href="category-theory.anafunctors.html" class="Module">category-theory.anafunctors</a>
<a id="3252" class="Keyword">open</a> <a id="3257" class="Keyword">import</a> <a id="3264" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="3291" class="Keyword">open</a> <a id="3296" class="Keyword">import</a> <a id="3303" href="category-theory.epimorphisms-large-precategories.html" class="Module">category-theory.epimorphisms-large-precategories</a>
<a id="3352" class="Keyword">open</a> <a id="3357" class="Keyword">import</a> <a id="3364" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="3404" class="Keyword">open</a> <a id="3409" class="Keyword">import</a> <a id="3416" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="3465" class="Keyword">open</a> <a id="3470" class="Keyword">import</a> <a id="3477" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="3520" class="Keyword">open</a> <a id="3525" class="Keyword">import</a> <a id="3532" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="3568" class="Keyword">open</a> <a id="3573" class="Keyword">import</a> <a id="3580" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="3625" class="Keyword">open</a> <a id="3630" class="Keyword">import</a> <a id="3637" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="3676" class="Keyword">open</a> <a id="3681" class="Keyword">import</a> <a id="3688" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="3759" class="Keyword">open</a> <a id="3764" class="Keyword">import</a> <a id="3771" href="category-theory.initial-objects-precategories.html" class="Module">category-theory.initial-objects-precategories</a>
<a id="3817" class="Keyword">open</a> <a id="3822" class="Keyword">import</a> <a id="3829" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="3869" class="Keyword">open</a> <a id="3874" class="Keyword">import</a> <a id="3881" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="3930" class="Keyword">open</a> <a id="3935" class="Keyword">import</a> <a id="3942" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="3985" class="Keyword">open</a> <a id="3990" class="Keyword">import</a> <a id="3997" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="4030" class="Keyword">open</a> <a id="4035" class="Keyword">import</a> <a id="4042" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="4078" class="Keyword">open</a> <a id="4083" class="Keyword">import</a> <a id="4090" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="4140" class="Keyword">open</a> <a id="4145" class="Keyword">import</a> <a id="4152" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="4200" class="Keyword">open</a> <a id="4205" class="Keyword">import</a> <a id="4212" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="4269" class="Keyword">open</a> <a id="4274" class="Keyword">import</a> <a id="4281" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="4332" class="Keyword">open</a> <a id="4337" class="Keyword">import</a> <a id="4344" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="4395" class="Keyword">open</a> <a id="4400" class="Keyword">import</a> <a id="4407" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="4467" class="Keyword">open</a> <a id="4472" class="Keyword">import</a> <a id="4479" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="4533" class="Keyword">open</a> <a id="4538" class="Keyword">import</a> <a id="4545" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
<a id="4575" class="Keyword">open</a> <a id="4580" class="Keyword">import</a> <a id="4587" href="category-theory.slice-precategories.html" class="Module">category-theory.slice-precategories</a>
<a id="4623" class="Keyword">open</a> <a id="4628" class="Keyword">import</a> <a id="4635" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Commutative algebra

<pre class="Agda"><a id="4719" class="Keyword">open</a> <a id="4724" class="Keyword">import</a> <a id="4731" href="commutative-algebra.html" class="Module">commutative-algebra</a>
<a id="4751" class="Keyword">open</a> <a id="4756" class="Keyword">import</a> <a id="4763" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>
<a id="4801" class="Keyword">open</a> <a id="4806" class="Keyword">import</a> <a id="4813" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a>
<a id="4849" class="Keyword">open</a> <a id="4854" class="Keyword">import</a> <a id="4861" href="commutative-algebra.eisenstein-integers.html" class="Module">commutative-algebra.eisenstein-integers</a>
<a id="4901" class="Keyword">open</a> <a id="4906" class="Keyword">import</a> <a id="4913" href="commutative-algebra.gaussian-integers.html" class="Module">commutative-algebra.gaussian-integers</a>
<a id="4951" class="Keyword">open</a> <a id="4956" class="Keyword">import</a> <a id="4963" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a>
<a id="5015" class="Keyword">open</a> <a id="5020" class="Keyword">import</a> <a id="5027" href="commutative-algebra.ideals-commutative-rings.html" class="Module">commutative-algebra.ideals-commutative-rings</a>
<a id="5072" class="Keyword">open</a> <a id="5077" class="Keyword">import</a> <a id="5084" href="commutative-algebra.integral-domains.html" class="Module">commutative-algebra.integral-domains</a>
<a id="5121" class="Keyword">open</a> <a id="5126" class="Keyword">import</a> <a id="5133" href="commutative-algebra.invertible-elements-commutative-rings.html" class="Module">commutative-algebra.invertible-elements-commutative-rings</a>
<a id="5191" class="Keyword">open</a> <a id="5196" class="Keyword">import</a> <a id="5203" href="commutative-algebra.isomorphisms-commutative-rings.html" class="Module">commutative-algebra.isomorphisms-commutative-rings</a>
<a id="5254" class="Keyword">open</a> <a id="5259" class="Keyword">import</a> <a id="5266" href="commutative-algebra.local-commutative-rings.html" class="Module">commutative-algebra.local-commutative-rings</a>
<a id="5310" class="Keyword">open</a> <a id="5315" class="Keyword">import</a> <a id="5322" href="commutative-algebra.prime-ideals-commutative-rings.html" class="Module">commutative-algebra.prime-ideals-commutative-rings</a>
<a id="5373" class="Keyword">open</a> <a id="5378" class="Keyword">import</a> <a id="5385" href="commutative-algebra.zariski-topology.html" class="Module">commutative-algebra.zariski-topology</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="5464" class="Keyword">open</a> <a id="5469" class="Keyword">import</a> <a id="5476" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5501" class="Keyword">open</a> <a id="5506" class="Keyword">import</a> <a id="5513" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5562" class="Keyword">open</a> <a id="5567" class="Keyword">import</a> <a id="5574" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5617" class="Keyword">open</a> <a id="5622" class="Keyword">import</a> <a id="5629" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5679" class="Keyword">open</a> <a id="5684" class="Keyword">import</a> <a id="5691" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5737" class="Keyword">open</a> <a id="5742" class="Keyword">import</a> <a id="5749" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5796" class="Keyword">open</a> <a id="5801" class="Keyword">import</a> <a id="5808" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5867" class="Keyword">open</a> <a id="5872" class="Keyword">import</a> <a id="5879" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="5920" class="Keyword">open</a> <a id="5925" class="Keyword">import</a> <a id="5932" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="5975" class="Keyword">open</a> <a id="5980" class="Keyword">import</a> <a id="5987" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="6031" class="Keyword">open</a> <a id="6036" class="Keyword">import</a> <a id="6043" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="6088" class="Keyword">open</a> <a id="6093" class="Keyword">import</a> <a id="6100" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="6152" class="Keyword">open</a> <a id="6157" class="Keyword">import</a> <a id="6164" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="6224" class="Keyword">open</a> <a id="6229" class="Keyword">import</a> <a id="6236" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="6277" class="Keyword">open</a> <a id="6282" class="Keyword">import</a> <a id="6289" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6334" class="Keyword">open</a> <a id="6339" class="Keyword">import</a> <a id="6346" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6393" class="Keyword">open</a> <a id="6398" class="Keyword">import</a> <a id="6405" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6448" class="Keyword">open</a> <a id="6453" class="Keyword">import</a> <a id="6460" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6510" class="Keyword">open</a> <a id="6515" class="Keyword">import</a> <a id="6522" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6569" class="Keyword">open</a> <a id="6574" class="Keyword">import</a> <a id="6581" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6638" class="Keyword">open</a> <a id="6643" class="Keyword">import</a> <a id="6650" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6704" class="Keyword">open</a> <a id="6709" class="Keyword">import</a> <a id="6716" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6776" class="Keyword">open</a> <a id="6781" class="Keyword">import</a> <a id="6788" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6831" class="Keyword">open</a> <a id="6836" class="Keyword">import</a> <a id="6843" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="6893" class="Keyword">open</a> <a id="6898" class="Keyword">import</a> <a id="6905" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="6965" class="Keyword">open</a> <a id="6970" class="Keyword">import</a> <a id="6977" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="7026" class="Keyword">open</a> <a id="7031" class="Keyword">import</a> <a id="7038" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="7094" class="Keyword">open</a> <a id="7099" class="Keyword">import</a> <a id="7106" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="7142" class="Keyword">open</a> <a id="7147" class="Keyword">import</a> <a id="7154" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="7198" class="Keyword">open</a> <a id="7203" class="Keyword">import</a> <a id="7210" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="7254" class="Keyword">open</a> <a id="7259" class="Keyword">import</a> <a id="7266" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7316" class="Keyword">open</a> <a id="7321" class="Keyword">import</a> <a id="7328" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7374" class="Keyword">open</a> <a id="7379" class="Keyword">import</a> <a id="7386" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7421" class="Keyword">open</a> <a id="7426" class="Keyword">import</a> <a id="7433" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7478" class="Keyword">open</a> <a id="7483" class="Keyword">import</a> <a id="7490" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7548" class="Keyword">open</a> <a id="7553" class="Keyword">import</a> <a id="7560" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7625" class="Keyword">open</a> <a id="7630" class="Keyword">import</a> <a id="7637" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7680" class="Keyword">open</a> <a id="7685" class="Keyword">import</a> <a id="7692" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7746" class="Keyword">open</a> <a id="7751" class="Keyword">import</a> <a id="7758" href="elementary-number-theory.half-integers.html" class="Module">elementary-number-theory.half-integers</a>
<a id="7797" class="Keyword">open</a> <a id="7802" class="Keyword">import</a> <a id="7809" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7854" class="Keyword">open</a> <a id="7859" class="Keyword">import</a> <a id="7866" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7918" class="Keyword">open</a> <a id="7923" class="Keyword">import</a> <a id="7930" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7988" class="Keyword">open</a> <a id="7993" class="Keyword">import</a> <a id="8000" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="8046" class="Keyword">open</a> <a id="8051" class="Keyword">import</a> <a id="8058" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="8102" class="Keyword">open</a> <a id="8107" class="Keyword">import</a> <a id="8114" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="8148" class="Keyword">open</a> <a id="8153" class="Keyword">import</a> <a id="8160" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="8214" class="Keyword">open</a> <a id="8219" class="Keyword">import</a> <a id="8226" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="8275" class="Keyword">open</a> <a id="8280" class="Keyword">import</a> <a id="8287" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="8328" class="Keyword">open</a> <a id="8333" class="Keyword">import</a> <a id="8340" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8389" class="Keyword">open</a> <a id="8394" class="Keyword">import</a> <a id="8401" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8467" class="Keyword">open</a> <a id="8472" class="Keyword">import</a> <a id="8479" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8523" class="Keyword">open</a> <a id="8528" class="Keyword">import</a> <a id="8535" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8584" class="Keyword">open</a> <a id="8589" class="Keyword">import</a> <a id="8596" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8652" class="Keyword">open</a> <a id="8657" class="Keyword">import</a> <a id="8664" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8705" class="Keyword">open</a> <a id="8710" class="Keyword">import</a> <a id="8717" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8766" class="Keyword">open</a> <a id="8771" class="Keyword">import</a> <a id="8778" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8837" class="Keyword">open</a> <a id="8842" class="Keyword">import</a> <a id="8849" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8888" class="Keyword">open</a> <a id="8893" class="Keyword">import</a> <a id="8900" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8953" class="Keyword">open</a> <a id="8958" class="Keyword">import</a> <a id="8965" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="9022" class="Keyword">open</a> <a id="9027" class="Keyword">import</a> <a id="9034" href="elementary-number-theory.pythagorean-triples.html" class="Module">elementary-number-theory.pythagorean-triples</a>
<a id="9079" class="Keyword">open</a> <a id="9084" class="Keyword">import</a> <a id="9091" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="9133" class="Keyword">open</a> <a id="9138" class="Keyword">import</a> <a id="9145" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="9196" class="Keyword">open</a> <a id="9201" class="Keyword">import</a> <a id="9208" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9266" class="Keyword">open</a> <a id="9271" class="Keyword">import</a> <a id="9278" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9342" class="Keyword">open</a> <a id="9347" class="Keyword">import</a> <a id="9354" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9407" class="Keyword">open</a> <a id="9412" class="Keyword">import</a> <a id="9419" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9472" class="Keyword">open</a> <a id="9477" class="Keyword">import</a> <a id="9484" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9545" class="Keyword">open</a> <a id="9550" class="Keyword">import</a> <a id="9557" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9615" class="Keyword">open</a> <a id="9620" class="Keyword">import</a> <a id="9627" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9676" class="Keyword">open</a> <a id="9681" class="Keyword">import</a> <a id="9688" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9731" class="Keyword">open</a> <a id="9736" class="Keyword">import</a> <a id="9743" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9787" class="Keyword">open</a> <a id="9792" class="Keyword">import</a> <a id="9799" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9846" class="Keyword">open</a> <a id="9851" class="Keyword">import</a> <a id="9858" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9919" class="Keyword">open</a> <a id="9924" class="Keyword">import</a> <a id="9931" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9994" class="Keyword">open</a> <a id="9999" class="Keyword">import</a> <a id="10006" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="10066" class="Keyword">open</a> <a id="10071" class="Keyword">import</a> <a id="10078" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="10132" class="Keyword">open</a> <a id="10137" class="Keyword">import</a> <a id="10144" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="10209" class="Keyword">open</a> <a id="10214" class="Keyword">import</a> <a id="10221" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10329" class="Keyword">open</a> <a id="10334" class="Keyword">import</a> <a id="10341" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10361" class="Keyword">open</a> <a id="10366" class="Keyword">import</a> <a id="10373" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10419" class="Keyword">open</a> <a id="10424" class="Keyword">import</a> <a id="10431" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a>
<a id="10470" class="Keyword">open</a> <a id="10475" class="Keyword">import</a> <a id="10482" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10538" class="Keyword">open</a> <a id="10543" class="Keyword">import</a> <a id="10550" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10596" class="Keyword">open</a> <a id="10601" class="Keyword">import</a> <a id="10608" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10642" class="Keyword">open</a> <a id="10647" class="Keyword">import</a> <a id="10654" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10689" class="Keyword">open</a> <a id="10694" class="Keyword">import</a> <a id="10701" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10739" class="Keyword">open</a> <a id="10744" class="Keyword">import</a> <a id="10751" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10789" class="Keyword">open</a> <a id="10794" class="Keyword">import</a> <a id="10801" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10841" class="Keyword">open</a> <a id="10846" class="Keyword">import</a> <a id="10853" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10886" class="Keyword">open</a> <a id="10891" class="Keyword">import</a> <a id="10898" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10936" class="Keyword">open</a> <a id="10941" class="Keyword">import</a> <a id="10948" href="finite-group-theory.simpson-delooping-sign-homomorphism.html" class="Module">finite-group-theory.simpson-delooping-sign-homomorphism</a>
<a id="11004" class="Keyword">open</a> <a id="11009" class="Keyword">import</a> <a id="11016" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="11058" class="Keyword">open</a> <a id="11063" class="Keyword">import</a> <a id="11070" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="11133" class="Keyword">open</a> <a id="11138" class="Keyword">import</a> <a id="11145" href="foundation.html" class="Module">foundation</a>
<a id="11156" class="Keyword">open</a> <a id="11161" class="Keyword">import</a> <a id="11168" href="foundation.0-connected-types.html" class="Module">foundation.0-connected-types</a>
<a id="11197" class="Keyword">open</a> <a id="11202" class="Keyword">import</a> <a id="11209" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a>
<a id="11237" class="Keyword">open</a> <a id="11242" class="Keyword">import</a> <a id="11249" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11267" class="Keyword">open</a> <a id="11272" class="Keyword">import</a> <a id="11279" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11298" class="Keyword">open</a> <a id="11303" class="Keyword">import</a> <a id="11310" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11329" class="Keyword">open</a> <a id="11334" class="Keyword">import</a> <a id="11341" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11385" class="Keyword">open</a> <a id="11390" class="Keyword">import</a> <a id="11397" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11422" class="Keyword">open</a> <a id="11427" class="Keyword">import</a> <a id="11434" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11461" class="Keyword">open</a> <a id="11466" class="Keyword">import</a> <a id="11473" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11490" class="Keyword">open</a> <a id="11495" class="Keyword">import</a> <a id="11502" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11531" class="Keyword">open</a> <a id="11536" class="Keyword">import</a> <a id="11543" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11599" class="Keyword">open</a> <a id="11604" class="Keyword">import</a> <a id="11611" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11642" class="Keyword">open</a> <a id="11647" class="Keyword">import</a> <a id="11654" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11708" class="Keyword">open</a> <a id="11713" class="Keyword">import</a> <a id="11720" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11748" class="Keyword">open</a> <a id="11753" class="Keyword">import</a> <a id="11760" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11790" class="Keyword">open</a> <a id="11795" class="Keyword">import</a> <a id="11802" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11822" class="Keyword">open</a> <a id="11827" class="Keyword">import</a> <a id="11834" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11879" class="Keyword">open</a> <a id="11884" class="Keyword">import</a> <a id="11891" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11928" class="Keyword">open</a> <a id="11933" class="Keyword">import</a> <a id="11940" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11975" class="Keyword">open</a> <a id="11980" class="Keyword">import</a> <a id="11987" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="12045" class="Keyword">open</a> <a id="12050" class="Keyword">import</a> <a id="12057" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12095" class="Keyword">open</a> <a id="12100" class="Keyword">import</a> <a id="12107" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12141" class="Keyword">open</a> <a id="12146" class="Keyword">import</a> <a id="12153" href="foundation.commuting-cubes.html" class="Module">foundation.commuting-cubes</a>
<a id="12180" class="Keyword">open</a> <a id="12185" class="Keyword">import</a> <a id="12192" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12221" class="Keyword">open</a> <a id="12226" class="Keyword">import</a> <a id="12233" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12256" class="Keyword">open</a> <a id="12261" class="Keyword">import</a> <a id="12268" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12295" class="Keyword">open</a> <a id="12300" class="Keyword">import</a> <a id="12307" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12330" class="Keyword">open</a> <a id="12335" class="Keyword">import</a> <a id="12342" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12384" class="Keyword">open</a> <a id="12389" class="Keyword">import</a> <a id="12396" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12428" class="Keyword">open</a> <a id="12433" class="Keyword">import</a> <a id="12440" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="12466" class="Keyword">open</a> <a id="12471" class="Keyword">import</a> <a id="12478" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12505" class="Keyword">open</a> <a id="12510" class="Keyword">import</a> <a id="12517" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12542" class="Keyword">open</a> <a id="12547" class="Keyword">import</a> <a id="12554" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12583" class="Keyword">open</a> <a id="12588" class="Keyword">import</a> <a id="12595" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12625" class="Keyword">open</a> <a id="12630" class="Keyword">import</a> <a id="12637" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12664" class="Keyword">open</a> <a id="12669" class="Keyword">import</a> <a id="12676" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12695" class="Keyword">open</a> <a id="12700" class="Keyword">import</a> <a id="12707" href="foundation.cospans.html" class="Module">foundation.cospans</a>
<a id="12726" class="Keyword">open</a> <a id="12731" class="Keyword">import</a> <a id="12738" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12784" class="Keyword">open</a> <a id="12789" class="Keyword">import</a> <a id="12796" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12838" class="Keyword">open</a> <a id="12843" class="Keyword">import</a> <a id="12850" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12882" class="Keyword">open</a> <a id="12887" class="Keyword">import</a> <a id="12894" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12924" class="Keyword">open</a> <a id="12929" class="Keyword">import</a> <a id="12936" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="12979" class="Keyword">open</a> <a id="12984" class="Keyword">import</a> <a id="12991" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="13017" class="Keyword">open</a> <a id="13022" class="Keyword">import</a> <a id="13029" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="13063" class="Keyword">open</a> <a id="13068" class="Keyword">import</a> <a id="13075" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="13106" class="Keyword">open</a> <a id="13111" class="Keyword">import</a> <a id="13118" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13148" class="Keyword">open</a> <a id="13153" class="Keyword">import</a> <a id="13160" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13187" class="Keyword">open</a> <a id="13192" class="Keyword">import</a> <a id="13199" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13237" class="Keyword">open</a> <a id="13242" class="Keyword">import</a> <a id="13249" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13281" class="Keyword">open</a> <a id="13286" class="Keyword">import</a> <a id="13293" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13328" class="Keyword">open</a> <a id="13333" class="Keyword">import</a> <a id="13340" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13380" class="Keyword">open</a> <a id="13385" class="Keyword">import</a> <a id="13392" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13423" class="Keyword">open</a> <a id="13428" class="Keyword">import</a> <a id="13435" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13469" class="Keyword">open</a> <a id="13474" class="Keyword">import</a> <a id="13481" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="13510" class="Keyword">open</a> <a id="13515" class="Keyword">import</a> <a id="13522" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13545" class="Keyword">open</a> <a id="13550" class="Keyword">import</a> <a id="13557" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13584" class="Keyword">open</a> <a id="13589" class="Keyword">import</a> <a id="13596" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13624" class="Keyword">open</a> <a id="13629" class="Keyword">import</a> <a id="13636" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13673" class="Keyword">open</a> <a id="13678" class="Keyword">import</a> <a id="13685" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13733" class="Keyword">open</a> <a id="13738" class="Keyword">import</a> <a id="13745" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13785" class="Keyword">open</a> <a id="13790" class="Keyword">import</a> <a id="13797" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13819" class="Keyword">open</a> <a id="13824" class="Keyword">import</a> <a id="13831" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13854" class="Keyword">open</a> <a id="13859" class="Keyword">import</a> <a id="13866" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13891" class="Keyword">open</a> <a id="13896" class="Keyword">import</a> <a id="13903" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13948" class="Keyword">open</a> <a id="13953" class="Keyword">import</a> <a id="13960" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="14004" class="Keyword">open</a> <a id="14009" class="Keyword">import</a> <a id="14016" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14052" class="Keyword">open</a> <a id="14057" class="Keyword">import</a> <a id="14064" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14109" class="Keyword">open</a> <a id="14114" class="Keyword">import</a> <a id="14121" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14162" class="Keyword">open</a> <a id="14167" class="Keyword">import</a> <a id="14174" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14209" class="Keyword">open</a> <a id="14214" class="Keyword">import</a> <a id="14221" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14253" class="Keyword">open</a> <a id="14258" class="Keyword">import</a> <a id="14265" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14296" class="Keyword">open</a> <a id="14301" class="Keyword">import</a> <a id="14308" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14341" class="Keyword">open</a> <a id="14346" class="Keyword">import</a> <a id="14353" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14386" class="Keyword">open</a> <a id="14391" class="Keyword">import</a> <a id="14398" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14428" class="Keyword">open</a> <a id="14433" class="Keyword">import</a> <a id="14440" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14464" class="Keyword">open</a> <a id="14469" class="Keyword">import</a> <a id="14476" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14514" class="Keyword">open</a> <a id="14519" class="Keyword">import</a> <a id="14526" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14557" class="Keyword">open</a> <a id="14562" class="Keyword">import</a> <a id="14569" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14594" class="Keyword">open</a> <a id="14599" class="Keyword">import</a> <a id="14606" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14634" class="Keyword">open</a> <a id="14639" class="Keyword">import</a> <a id="14646" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14670" class="Keyword">open</a> <a id="14675" class="Keyword">import</a> <a id="14682" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14708" class="Keyword">open</a> <a id="14713" class="Keyword">import</a> <a id="14720" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14755" class="Keyword">open</a> <a id="14760" class="Keyword">import</a> <a id="14767" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14788" class="Keyword">open</a> <a id="14793" class="Keyword">import</a> <a id="14800" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14849" class="Keyword">open</a> <a id="14854" class="Keyword">import</a> <a id="14861" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14902" class="Keyword">open</a> <a id="14907" class="Keyword">import</a> <a id="14914" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14964" class="Keyword">open</a> <a id="14969" class="Keyword">import</a> <a id="14976" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="15022" class="Keyword">open</a> <a id="15027" class="Keyword">import</a> <a id="15034" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15074" class="Keyword">open</a> <a id="15079" class="Keyword">import</a> <a id="15086" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15126" class="Keyword">open</a> <a id="15131" class="Keyword">import</a> <a id="15138" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15188" class="Keyword">open</a> <a id="15193" class="Keyword">import</a> <a id="15200" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15239" class="Keyword">open</a> <a id="15244" class="Keyword">import</a> <a id="15251" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15291" class="Keyword">open</a> <a id="15296" class="Keyword">import</a> <a id="15303" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15336" class="Keyword">open</a> <a id="15341" class="Keyword">import</a> <a id="15348" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15397" class="Keyword">open</a> <a id="15402" class="Keyword">import</a> <a id="15409" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15434" class="Keyword">open</a> <a id="15439" class="Keyword">import</a> <a id="15446" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="15485" class="Keyword">open</a> <a id="15490" class="Keyword">import</a> <a id="15497" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15535" class="Keyword">open</a> <a id="15540" class="Keyword">import</a> <a id="15547" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15569" class="Keyword">open</a> <a id="15574" class="Keyword">import</a> <a id="15581" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15609" class="Keyword">open</a> <a id="15614" class="Keyword">import</a> <a id="15621" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15657" class="Keyword">open</a> <a id="15662" class="Keyword">import</a> <a id="15669" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15695" class="Keyword">open</a> <a id="15700" class="Keyword">import</a> <a id="15707" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15725" class="Keyword">open</a> <a id="15730" class="Keyword">import</a> <a id="15737" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15772" class="Keyword">open</a> <a id="15777" class="Keyword">import</a> <a id="15784" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15819" class="Keyword">open</a> <a id="15824" class="Keyword">import</a> <a id="15831" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15858" class="Keyword">open</a> <a id="15863" class="Keyword">import</a> <a id="15870" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15926" class="Keyword">open</a> <a id="15931" class="Keyword">import</a> <a id="15938" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15967" class="Keyword">open</a> <a id="15972" class="Keyword">import</a> <a id="15979" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="16009" class="Keyword">open</a> <a id="16014" class="Keyword">import</a> <a id="16021" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="16048" class="Keyword">open</a> <a id="16053" class="Keyword">import</a> <a id="16060" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16086" class="Keyword">open</a> <a id="16091" class="Keyword">import</a> <a id="16098" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16125" class="Keyword">open</a> <a id="16130" class="Keyword">import</a> <a id="16137" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16161" class="Keyword">open</a> <a id="16166" class="Keyword">import</a> <a id="16173" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16196" class="Keyword">open</a> <a id="16201" class="Keyword">import</a> <a id="16208" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16235" class="Keyword">open</a> <a id="16240" class="Keyword">import</a> <a id="16247" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16279" class="Keyword">open</a> <a id="16284" class="Keyword">import</a> <a id="16291" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16326" class="Keyword">open</a> <a id="16331" class="Keyword">import</a> <a id="16338" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16369" class="Keyword">open</a> <a id="16374" class="Keyword">import</a> <a id="16381" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16414" class="Keyword">open</a> <a id="16419" class="Keyword">import</a> <a id="16426" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16460" class="Keyword">open</a> <a id="16465" class="Keyword">import</a> <a id="16472" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16512" class="Keyword">open</a> <a id="16517" class="Keyword">import</a> <a id="16524" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16555" class="Keyword">open</a> <a id="16560" class="Keyword">import</a> <a id="16567" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16599" class="Keyword">open</a> <a id="16604" class="Keyword">import</a> <a id="16611" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16642" class="Keyword">open</a> <a id="16647" class="Keyword">import</a> <a id="16654" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16671" class="Keyword">open</a> <a id="16676" class="Keyword">import</a> <a id="16683" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16708" class="Keyword">open</a> <a id="16713" class="Keyword">import</a> <a id="16720" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16749" class="Keyword">open</a> <a id="16754" class="Keyword">import</a> <a id="16761" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16786" class="Keyword">open</a> <a id="16791" class="Keyword">import</a> <a id="16798" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="16827" class="Keyword">open</a> <a id="16832" class="Keyword">import</a> <a id="16839" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16860" class="Keyword">open</a> <a id="16865" class="Keyword">import</a> <a id="16872" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16896" class="Keyword">open</a> <a id="16901" class="Keyword">import</a> <a id="16908" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16928" class="Keyword">open</a> <a id="16933" class="Keyword">import</a> <a id="16940" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16974" class="Keyword">open</a> <a id="16979" class="Keyword">import</a> <a id="16986" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17024" class="Keyword">open</a> <a id="17029" class="Keyword">import</a> <a id="17036" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17064" class="Keyword">open</a> <a id="17069" class="Keyword">import</a> <a id="17076" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17100" class="Keyword">open</a> <a id="17105" class="Keyword">import</a> <a id="17112" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17139" class="Keyword">open</a> <a id="17144" class="Keyword">import</a> <a id="17151" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17186" class="Keyword">open</a> <a id="17191" class="Keyword">import</a> <a id="17198" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17219" class="Keyword">open</a> <a id="17224" class="Keyword">import</a> <a id="17231" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17267" class="Keyword">open</a> <a id="17272" class="Keyword">import</a> <a id="17279" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17324" class="Keyword">open</a> <a id="17329" class="Keyword">import</a> <a id="17336" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17382" class="Keyword">open</a> <a id="17387" class="Keyword">import</a> <a id="17394" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17434" class="Keyword">open</a> <a id="17439" class="Keyword">import</a> <a id="17446" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17476" class="Keyword">open</a> <a id="17481" class="Keyword">import</a> <a id="17488" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17522" class="Keyword">open</a> <a id="17527" class="Keyword">import</a> <a id="17534" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17571" class="Keyword">open</a> <a id="17576" class="Keyword">import</a> <a id="17583" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17607" class="Keyword">open</a> <a id="17612" class="Keyword">import</a> <a id="17619" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17640" class="Keyword">open</a> <a id="17645" class="Keyword">import</a> <a id="17652" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17687" class="Keyword">open</a> <a id="17692" class="Keyword">import</a> <a id="17699" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17736" class="Keyword">open</a> <a id="17741" class="Keyword">import</a> <a id="17748" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17797" class="Keyword">open</a> <a id="17802" class="Keyword">import</a> <a id="17809" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17842" class="Keyword">open</a> <a id="17847" class="Keyword">import</a> <a id="17854" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17877" class="Keyword">open</a> <a id="17882" class="Keyword">import</a> <a id="17889" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17912" class="Keyword">open</a> <a id="17917" class="Keyword">import</a> <a id="17924" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17947" class="Keyword">open</a> <a id="17952" class="Keyword">import</a> <a id="17959" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17987" class="Keyword">open</a> <a id="17992" class="Keyword">import</a> <a id="17999" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18019" class="Keyword">open</a> <a id="18024" class="Keyword">import</a> <a id="18031" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18052" class="Keyword">open</a> <a id="18057" class="Keyword">import</a> <a id="18064" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18095" class="Keyword">open</a> <a id="18100" class="Keyword">import</a> <a id="18107" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18134" class="Keyword">open</a> <a id="18139" class="Keyword">import</a> <a id="18146" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18162" class="Keyword">open</a> <a id="18167" class="Keyword">import</a> <a id="18174" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18205" class="Keyword">open</a> <a id="18210" class="Keyword">import</a> <a id="18217" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18234" class="Keyword">open</a> <a id="18239" class="Keyword">import</a> <a id="18246" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18268" class="Keyword">open</a> <a id="18273" class="Keyword">import</a> <a id="18280" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18307" class="Keyword">open</a> <a id="18312" class="Keyword">import</a> <a id="18319" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18342" class="Keyword">open</a> <a id="18347" class="Keyword">import</a> <a id="18354" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18381" class="Keyword">open</a> <a id="18386" class="Keyword">import</a> <a id="18393" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18426" class="Keyword">open</a> <a id="18431" class="Keyword">import</a> <a id="18438" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18478" class="Keyword">open</a> <a id="18483" class="Keyword">import</a> <a id="18490" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18511" class="Keyword">open</a> <a id="18516" class="Keyword">import</a> <a id="18523" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18552" class="Keyword">open</a> <a id="18557" class="Keyword">import</a> <a id="18564" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18602" class="Keyword">open</a> <a id="18607" class="Keyword">import</a> <a id="18614" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18634" class="Keyword">open</a> <a id="18639" class="Keyword">import</a> <a id="18646" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18670" class="Keyword">open</a> <a id="18675" class="Keyword">import</a> <a id="18682" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18709" class="Keyword">open</a> <a id="18714" class="Keyword">import</a> <a id="18721" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18753" class="Keyword">open</a> <a id="18758" class="Keyword">import</a> <a id="18765" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18795" class="Keyword">open</a> <a id="18800" class="Keyword">import</a> <a id="18807" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18833" class="Keyword">open</a> <a id="18838" class="Keyword">import</a> <a id="18845" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18872" class="Keyword">open</a> <a id="18877" class="Keyword">import</a> <a id="18884" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="18921" class="Keyword">open</a> <a id="18926" class="Keyword">import</a> <a id="18933" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18962" class="Keyword">open</a> <a id="18967" class="Keyword">import</a> <a id="18974" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18997" class="Keyword">open</a> <a id="19002" class="Keyword">import</a> <a id="19009" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19060" class="Keyword">open</a> <a id="19065" class="Keyword">import</a> <a id="19072" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19115" class="Keyword">open</a> <a id="19120" class="Keyword">import</a> <a id="19127" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19179" class="Keyword">open</a> <a id="19184" class="Keyword">import</a> <a id="19191" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19239" class="Keyword">open</a> <a id="19244" class="Keyword">import</a> <a id="19251" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19289" class="Keyword">open</a> <a id="19294" class="Keyword">import</a> <a id="19301" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19338" class="Keyword">open</a> <a id="19343" class="Keyword">import</a> <a id="19350" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19396" class="Keyword">open</a> <a id="19401" class="Keyword">import</a> <a id="19408" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19425" class="Keyword">open</a> <a id="19430" class="Keyword">import</a> <a id="19437" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19465" class="Keyword">open</a> <a id="19470" class="Keyword">import</a> <a id="19477" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19505" class="Keyword">open</a> <a id="19510" class="Keyword">import</a> <a id="19517" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19553" class="Keyword">open</a> <a id="19558" class="Keyword">import</a> <a id="19565" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19603" class="Keyword">open</a> <a id="19608" class="Keyword">import</a> <a id="19615" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19648" class="Keyword">open</a> <a id="19653" class="Keyword">import</a> <a id="19660" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19681" class="Keyword">open</a> <a id="19686" class="Keyword">import</a> <a id="19693" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19729" class="Keyword">open</a> <a id="19734" class="Keyword">import</a> <a id="19741" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19795" class="Keyword">open</a> <a id="19800" class="Keyword">import</a> <a id="19807" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19829" class="Keyword">open</a> <a id="19834" class="Keyword">import</a> <a id="19841" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19876" class="Keyword">open</a> <a id="19881" class="Keyword">import</a> <a id="19888" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19918" class="Keyword">open</a> <a id="19923" class="Keyword">import</a> <a id="19930" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19969" class="Keyword">open</a> <a id="19974" class="Keyword">import</a> <a id="19981" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20035" class="Keyword">open</a> <a id="20040" class="Keyword">import</a> <a id="20047" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20093" class="Keyword">open</a> <a id="20098" class="Keyword">import</a> <a id="20105" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20156" class="Keyword">open</a> <a id="20161" class="Keyword">import</a> <a id="20168" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20209" class="Keyword">open</a> <a id="20214" class="Keyword">import</a> <a id="20221" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20266" class="Keyword">open</a> <a id="20271" class="Keyword">import</a> <a id="20278" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20323" class="Keyword">open</a> <a id="20328" class="Keyword">import</a> <a id="20335" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20371" class="Keyword">open</a> <a id="20376" class="Keyword">import</a> <a id="20383" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20419" class="Keyword">open</a> <a id="20424" class="Keyword">import</a> <a id="20431" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20496" class="Keyword">open</a> <a id="20501" class="Keyword">import</a> <a id="20508" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20563" class="Keyword">open</a> <a id="20568" class="Keyword">import</a> <a id="20575" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20615" class="Keyword">open</a> <a id="20620" class="Keyword">import</a> <a id="20627" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20671" class="Keyword">open</a> <a id="20676" class="Keyword">import</a> <a id="20683" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20728" class="Keyword">open</a> <a id="20733" class="Keyword">import</a> <a id="20740" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20781" class="Keyword">open</a> <a id="20786" class="Keyword">import</a> <a id="20793" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20833" class="Keyword">open</a> <a id="20838" class="Keyword">import</a> <a id="20845" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20872" class="Keyword">open</a> <a id="20877" class="Keyword">import</a> <a id="20884" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20920" class="Keyword">open</a> <a id="20925" class="Keyword">import</a> <a id="20932" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20959" class="Keyword">open</a> <a id="20964" class="Keyword">import</a> <a id="20971" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21008" class="Keyword">open</a> <a id="21013" class="Keyword">import</a> <a id="21020" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21048" class="Keyword">open</a> <a id="21053" class="Keyword">import</a> <a id="21060" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21079" class="Keyword">open</a> <a id="21084" class="Keyword">import</a> <a id="21091" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21131" class="Keyword">open</a> <a id="21136" class="Keyword">import</a> <a id="21143" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21175" class="Keyword">open</a> <a id="21180" class="Keyword">import</a> <a id="21187" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21235" class="Keyword">open</a> <a id="21240" class="Keyword">import</a> <a id="21247" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21270" class="Keyword">open</a> <a id="21275" class="Keyword">import</a> <a id="21282" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21306" class="Keyword">open</a> <a id="21311" class="Keyword">import</a> <a id="21318" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21358" class="Keyword">open</a> <a id="21363" class="Keyword">import</a> <a id="21370" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="21413" class="Keyword">open</a> <a id="21418" class="Keyword">import</a> <a id="21425" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21459" class="Keyword">open</a> <a id="21464" class="Keyword">import</a> <a id="21471" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21503" class="Keyword">open</a> <a id="21508" class="Keyword">import</a> <a id="21515" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21545" class="Keyword">open</a> <a id="21550" class="Keyword">import</a> <a id="21557" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21591" class="Keyword">open</a> <a id="21596" class="Keyword">import</a> <a id="21603" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21638" class="Keyword">open</a> <a id="21643" class="Keyword">import</a> <a id="21650" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="21674" class="Keyword">open</a> <a id="21679" class="Keyword">import</a> <a id="21686" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21723" class="Keyword">open</a> <a id="21728" class="Keyword">import</a> <a id="21735" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21762" class="Keyword">open</a> <a id="21767" class="Keyword">import</a> <a id="21774" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21802" class="Keyword">open</a> <a id="21807" class="Keyword">import</a> <a id="21814" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21863" class="Keyword">open</a> <a id="21868" class="Keyword">import</a> <a id="21875" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21921" class="Keyword">open</a> <a id="21926" class="Keyword">import</a> <a id="21933" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21973" class="Keyword">open</a> <a id="21978" class="Keyword">import</a> <a id="21985" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22023" class="Keyword">open</a> <a id="22028" class="Keyword">import</a> <a id="22035" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22064" class="Keyword">open</a> <a id="22069" class="Keyword">import</a> <a id="22076" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22106" class="Keyword">open</a> <a id="22111" class="Keyword">import</a> <a id="22118" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22149" class="Keyword">open</a> <a id="22154" class="Keyword">import</a> <a id="22161" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="22201" class="Keyword">open</a> <a id="22206" class="Keyword">import</a> <a id="22213" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22239" class="Keyword">open</a> <a id="22244" class="Keyword">import</a> <a id="22251" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="22306" class="Keyword">open</a> <a id="22311" class="Keyword">import</a> <a id="22318" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="22369" class="Keyword">open</a> <a id="22374" class="Keyword">import</a> <a id="22381" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="22426" class="Keyword">open</a> <a id="22431" class="Keyword">import</a> <a id="22438" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="22483" class="Keyword">open</a> <a id="22488" class="Keyword">import</a> <a id="22495" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22549" class="Keyword">open</a> <a id="22554" class="Keyword">import</a> <a id="22561" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22588" class="Keyword">open</a> <a id="22593" class="Keyword">import</a> <a id="22600" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22633" class="Keyword">open</a> <a id="22638" class="Keyword">import</a> <a id="22645" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22676" class="Keyword">open</a> <a id="22681" class="Keyword">import</a> <a id="22688" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22725" class="Keyword">open</a> <a id="22730" class="Keyword">import</a> <a id="22737" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="22771" class="Keyword">open</a> <a id="22776" class="Keyword">import</a> <a id="22783" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22808" class="Keyword">open</a> <a id="22813" class="Keyword">import</a> <a id="22820" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22852" class="Keyword">open</a> <a id="22857" class="Keyword">import</a> <a id="22864" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22899" class="Keyword">open</a> <a id="22904" class="Keyword">import</a> <a id="22911" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22940" class="Keyword">open</a> <a id="22945" class="Keyword">import</a> <a id="22952" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22978" class="Keyword">open</a> <a id="22983" class="Keyword">import</a> <a id="22990" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23018" class="Keyword">open</a> <a id="23023" class="Keyword">import</a> <a id="23030" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23055" class="Keyword">open</a> <a id="23060" class="Keyword">import</a> <a id="23067" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23088" class="Keyword">open</a> <a id="23093" class="Keyword">import</a> <a id="23100" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23136" class="Keyword">open</a> <a id="23141" class="Keyword">import</a> <a id="23148" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="23191" class="Keyword">open</a> <a id="23196" class="Keyword">import</a> <a id="23203" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23228" class="Keyword">open</a> <a id="23233" class="Keyword">import</a> <a id="23240" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23271" class="Keyword">open</a> <a id="23276" class="Keyword">import</a> <a id="23283" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="23315" class="Keyword">open</a> <a id="23320" class="Keyword">import</a> <a id="23327" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="23361" class="Keyword">open</a> <a id="23366" class="Keyword">import</a> <a id="23373" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="23429" class="Keyword">open</a> <a id="23434" class="Keyword">import</a> <a id="23441" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="23494" class="Keyword">open</a> <a id="23499" class="Keyword">import</a> <a id="23506" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="23533" class="Keyword">open</a> <a id="23538" class="Keyword">import</a> <a id="23545" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23590" class="Keyword">open</a> <a id="23595" class="Keyword">import</a> <a id="23602" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23664" class="Keyword">open</a> <a id="23669" class="Keyword">import</a> <a id="23676" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23689" class="Keyword">open</a> <a id="23694" class="Keyword">import</a> <a id="23701" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23741" class="Keyword">open</a> <a id="23746" class="Keyword">import</a> <a id="23753" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23797" class="Keyword">open</a> <a id="23802" class="Keyword">import</a> <a id="23809" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23848" class="Keyword">open</a> <a id="23853" class="Keyword">import</a> <a id="23860" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23902" class="Keyword">open</a> <a id="23907" class="Keyword">import</a> <a id="23914" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23954" class="Keyword">open</a> <a id="23959" class="Keyword">import</a> <a id="23966" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24007" class="Keyword">open</a> <a id="24012" class="Keyword">import</a> <a id="24019" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24057" class="Keyword">open</a> <a id="24062" class="Keyword">import</a> <a id="24069" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24132" class="Keyword">open</a> <a id="24137" class="Keyword">import</a> <a id="24144" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="24173" class="Keyword">open</a> <a id="24178" class="Keyword">import</a> <a id="24185" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24230" class="Keyword">open</a> <a id="24235" class="Keyword">import</a> <a id="24242" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24284" class="Keyword">open</a> <a id="24289" class="Keyword">import</a> <a id="24296" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="24340" class="Keyword">open</a> <a id="24345" class="Keyword">import</a> <a id="24352" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="24401" class="Keyword">open</a> <a id="24406" class="Keyword">import</a> <a id="24413" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="24463" class="Keyword">open</a> <a id="24468" class="Keyword">import</a> <a id="24475" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="24502" class="Keyword">open</a> <a id="24507" class="Keyword">import</a> <a id="24514" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="24539" class="Keyword">open</a> <a id="24544" class="Keyword">import</a> <a id="24551" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24592" class="Keyword">open</a> <a id="24597" class="Keyword">import</a> <a id="24604" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24627" class="Keyword">open</a> <a id="24632" class="Keyword">import</a> <a id="24639" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24688" class="Keyword">open</a> <a id="24693" class="Keyword">import</a> <a id="24700" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24739" class="Keyword">open</a> <a id="24744" class="Keyword">import</a> <a id="24751" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24792" class="Keyword">open</a> <a id="24797" class="Keyword">import</a> <a id="24804" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24848" class="Keyword">open</a> <a id="24853" class="Keyword">import</a> <a id="24860" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24897" class="Keyword">open</a> <a id="24902" class="Keyword">import</a> <a id="24909" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24931" class="Keyword">open</a> <a id="24936" class="Keyword">import</a> <a id="24943" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24973" class="Keyword">open</a> <a id="24978" class="Keyword">import</a> <a id="24985" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="25024" class="Keyword">open</a> <a id="25029" class="Keyword">import</a> <a id="25036" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25074" class="Keyword">open</a> <a id="25079" class="Keyword">import</a> <a id="25086" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="25144" class="Keyword">open</a> <a id="25149" class="Keyword">import</a> <a id="25156" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="25221" class="Keyword">open</a> <a id="25226" class="Keyword">import</a> <a id="25233" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="25264" class="Keyword">open</a> <a id="25269" class="Keyword">import</a> <a id="25276" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="25303" class="Keyword">open</a> <a id="25308" class="Keyword">import</a> <a id="25315" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="25373" class="Keyword">open</a> <a id="25378" class="Keyword">import</a> <a id="25385" href="group-theory.html" class="Module">group-theory</a>
<a id="25398" class="Keyword">open</a> <a id="25403" class="Keyword">import</a> <a id="25410" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="25438" class="Keyword">open</a> <a id="25443" class="Keyword">import</a> <a id="25450" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25501" class="Keyword">open</a> <a id="25506" class="Keyword">import</a> <a id="25513" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25546" class="Keyword">open</a> <a id="25551" class="Keyword">import</a> <a id="25558" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="25605" class="Keyword">open</a> <a id="25610" class="Keyword">import</a> <a id="25617" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="25656" class="Keyword">open</a> <a id="25661" class="Keyword">import</a> <a id="25668" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25708" class="Keyword">open</a> <a id="25713" class="Keyword">import</a> <a id="25720" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25763" class="Keyword">open</a> <a id="25768" class="Keyword">import</a> <a id="25775" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25807" class="Keyword">open</a> <a id="25812" class="Keyword">import</a> <a id="25819" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25855" class="Keyword">open</a> <a id="25860" class="Keyword">import</a> <a id="25867" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25896" class="Keyword">open</a> <a id="25901" class="Keyword">import</a> <a id="25908" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25936" class="Keyword">open</a> <a id="25941" class="Keyword">import</a> <a id="25948" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25981" class="Keyword">open</a> <a id="25986" class="Keyword">import</a> <a id="25993" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="26029" class="Keyword">open</a> <a id="26034" class="Keyword">import</a> <a id="26041" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="26070" class="Keyword">open</a> <a id="26075" class="Keyword">import</a> <a id="26082" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="26107" class="Keyword">open</a> <a id="26112" class="Keyword">import</a> <a id="26119" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="26181" class="Keyword">open</a> <a id="26186" class="Keyword">import</a> <a id="26193" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="26217" class="Keyword">open</a> <a id="26222" class="Keyword">import</a> <a id="26229" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="26260" class="Keyword">open</a> <a id="26265" class="Keyword">import</a> <a id="26272" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="26319" class="Keyword">open</a> <a id="26324" class="Keyword">import</a> <a id="26331" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="26364" class="Keyword">open</a> <a id="26369" class="Keyword">import</a> <a id="26376" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="26425" class="Keyword">open</a> <a id="26430" class="Keyword">import</a> <a id="26437" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="26477" class="Keyword">open</a> <a id="26482" class="Keyword">import</a> <a id="26489" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="26526" class="Keyword">open</a> <a id="26531" class="Keyword">import</a> <a id="26538" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="26585" class="Keyword">open</a> <a id="26590" class="Keyword">import</a> <a id="26597" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="26638" class="Keyword">open</a> <a id="26643" class="Keyword">import</a> <a id="26650" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="26689" class="Keyword">open</a> <a id="26694" class="Keyword">import</a> <a id="26701" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="26733" class="Keyword">open</a> <a id="26738" class="Keyword">import</a> <a id="26745" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="26772" class="Keyword">open</a> <a id="26777" class="Keyword">import</a> <a id="26784" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26804" class="Keyword">open</a> <a id="26809" class="Keyword">import</a> <a id="26816" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26850" class="Keyword">open</a> <a id="26855" class="Keyword">import</a> <a id="26862" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26889" class="Keyword">open</a> <a id="26894" class="Keyword">import</a> <a id="26901" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26943" class="Keyword">open</a> <a id="26948" class="Keyword">import</a> <a id="26955" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="27005" class="Keyword">open</a> <a id="27010" class="Keyword">import</a> <a id="27017" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="27064" class="Keyword">open</a> <a id="27069" class="Keyword">import</a> <a id="27076" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="27117" class="Keyword">open</a> <a id="27122" class="Keyword">import</a> <a id="27129" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="27163" class="Keyword">open</a> <a id="27168" class="Keyword">import</a> <a id="27175" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="27216" class="Keyword">open</a> <a id="27221" class="Keyword">import</a> <a id="27228" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="27263" class="Keyword">open</a> <a id="27268" class="Keyword">import</a> <a id="27275" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="27313" class="Keyword">open</a> <a id="27318" class="Keyword">import</a> <a id="27325" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="27360" class="Keyword">open</a> <a id="27365" class="Keyword">import</a> <a id="27372" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="27404" class="Keyword">open</a> <a id="27409" class="Keyword">import</a> <a id="27416" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="27457" class="Keyword">open</a> <a id="27462" class="Keyword">import</a> <a id="27469" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="27510" class="Keyword">open</a> <a id="27515" class="Keyword">import</a> <a id="27522" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="27562" class="Keyword">open</a> <a id="27567" class="Keyword">import</a> <a id="27574" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="27607" class="Keyword">open</a> <a id="27612" class="Keyword">import</a> <a id="27619" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="27656" class="Keyword">open</a> <a id="27661" class="Keyword">import</a> <a id="27668" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="27698" class="Keyword">open</a> <a id="27703" class="Keyword">import</a> <a id="27710" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="27731" class="Keyword">open</a> <a id="27736" class="Keyword">import</a> <a id="27743" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="27797" class="Keyword">open</a> <a id="27802" class="Keyword">import</a> <a id="27809" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27854" class="Keyword">open</a> <a id="27859" class="Keyword">import</a> <a id="27866" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27894" class="Keyword">open</a> <a id="27899" class="Keyword">import</a> <a id="27906" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27927" class="Keyword">open</a> <a id="27932" class="Keyword">import</a> <a id="27939" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27982" class="Keyword">open</a> <a id="27987" class="Keyword">import</a> <a id="27994" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="28028" class="Keyword">open</a> <a id="28033" class="Keyword">import</a> <a id="28040" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="28070" class="Keyword">open</a> <a id="28075" class="Keyword">import</a> <a id="28082" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="28128" class="Keyword">open</a> <a id="28133" class="Keyword">import</a> <a id="28140" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="28194" class="Keyword">open</a> <a id="28199" class="Keyword">import</a> <a id="28206" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="28249" class="Keyword">open</a> <a id="28254" class="Keyword">import</a> <a id="28261" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="28295" class="Keyword">open</a> <a id="28300" class="Keyword">import</a> <a id="28307" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="28348" class="Keyword">open</a> <a id="28353" class="Keyword">import</a> <a id="28360" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="28395" class="Keyword">open</a> <a id="28400" class="Keyword">import</a> <a id="28407" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="28449" class="Keyword">open</a> <a id="28454" class="Keyword">import</a> <a id="28461" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="28496" class="Keyword">open</a> <a id="28501" class="Keyword">import</a> <a id="28508" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="28547" class="Keyword">open</a> <a id="28552" class="Keyword">import</a> <a id="28559" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="28596" class="Keyword">open</a> <a id="28601" class="Keyword">import</a> <a id="28608" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="28655" class="Keyword">open</a> <a id="28660" class="Keyword">import</a> <a id="28667" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="28731" class="Keyword">open</a> <a id="28736" class="Keyword">import</a> <a id="28743" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="28788" class="Keyword">open</a> <a id="28793" class="Keyword">import</a> <a id="28800" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="28824" class="Keyword">open</a> <a id="28829" class="Keyword">import</a> <a id="28836" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="28861" class="Keyword">open</a> <a id="28866" class="Keyword">import</a> <a id="28873" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28916" class="Keyword">open</a> <a id="28921" class="Keyword">import</a> <a id="28928" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28959" class="Keyword">open</a> <a id="28964" class="Keyword">import</a> <a id="28971" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="29025" class="Keyword">open</a> <a id="29030" class="Keyword">import</a> <a id="29037" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="29060" class="Keyword">open</a> <a id="29065" class="Keyword">import</a> <a id="29072" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="29110" class="Keyword">open</a> <a id="29115" class="Keyword">import</a> <a id="29122" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="29161" class="Keyword">open</a> <a id="29166" class="Keyword">import</a> <a id="29173" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="29224" class="Keyword">open</a> <a id="29229" class="Keyword">import</a> <a id="29236" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="29273" class="Keyword">open</a> <a id="29278" class="Keyword">import</a> <a id="29285" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="29342" class="Keyword">open</a> <a id="29347" class="Keyword">import</a> <a id="29354" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="29402" class="Keyword">open</a> <a id="29407" class="Keyword">import</a> <a id="29414" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="29444" class="Keyword">open</a> <a id="29449" class="Keyword">import</a> <a id="29456" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="29493" class="Keyword">open</a> <a id="29498" class="Keyword">import</a> <a id="29505" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="29526" class="Keyword">open</a> <a id="29531" class="Keyword">import</a> <a id="29538" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="29585" class="Keyword">open</a> <a id="29590" class="Keyword">import</a> <a id="29597" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="29635" class="Keyword">open</a> <a id="29640" class="Keyword">import</a> <a id="29647" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="29741" class="Keyword">open</a> <a id="29746" class="Keyword">import</a> <a id="29753" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="29768" class="Keyword">open</a> <a id="29773" class="Keyword">import</a> <a id="29780" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="29813" class="Keyword">open</a> <a id="29818" class="Keyword">import</a> <a id="29825" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="29857" class="Keyword">open</a> <a id="29862" class="Keyword">import</a> <a id="29869" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29911" class="Keyword">open</a> <a id="29916" class="Keyword">import</a> <a id="29923" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29961" class="Keyword">open</a> <a id="29966" class="Keyword">import</a> <a id="29973" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="30010" class="Keyword">open</a> <a id="30015" class="Keyword">import</a> <a id="30022" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="30055" class="Keyword">open</a> <a id="30060" class="Keyword">import</a> <a id="30067" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="30091" class="Keyword">open</a> <a id="30096" class="Keyword">import</a> <a id="30103" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="30142" class="Keyword">open</a> <a id="30147" class="Keyword">import</a> <a id="30154" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="30200" class="Keyword">open</a> <a id="30205" class="Keyword">import</a> <a id="30212" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="30257" class="Keyword">open</a> <a id="30262" class="Keyword">import</a> <a id="30269" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="30307" class="Keyword">open</a> <a id="30312" class="Keyword">import</a> <a id="30319" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="30351" class="Keyword">open</a> <a id="30356" class="Keyword">import</a> <a id="30363" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="30416" class="Keyword">open</a> <a id="30421" class="Keyword">import</a> <a id="30428" href="order-theory.html" class="Module">order-theory</a>
<a id="30441" class="Keyword">open</a> <a id="30446" class="Keyword">import</a> <a id="30453" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="30480" class="Keyword">open</a> <a id="30485" class="Keyword">import</a> <a id="30492" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="30522" class="Keyword">open</a> <a id="30527" class="Keyword">import</a> <a id="30534" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="30567" class="Keyword">open</a> <a id="30572" class="Keyword">import</a> <a id="30579" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="30615" class="Keyword">open</a> <a id="30620" class="Keyword">import</a> <a id="30627" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="30662" class="Keyword">open</a> <a id="30667" class="Keyword">import</a> <a id="30674" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="30701" class="Keyword">open</a> <a id="30706" class="Keyword">import</a> <a id="30713" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="30743" class="Keyword">open</a> <a id="30748" class="Keyword">import</a> <a id="30755" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="30791" class="Keyword">open</a> <a id="30796" class="Keyword">import</a> <a id="30803" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="30845" class="Keyword">open</a> <a id="30850" class="Keyword">import</a> <a id="30857" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="30889" class="Keyword">open</a> <a id="30894" class="Keyword">import</a> <a id="30901" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30932" class="Keyword">open</a> <a id="30937" class="Keyword">import</a> <a id="30944" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30970" class="Keyword">open</a> <a id="30975" class="Keyword">import</a> <a id="30982" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="31011" class="Keyword">open</a> <a id="31016" class="Keyword">import</a> <a id="31023" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="31060" class="Keyword">open</a> <a id="31065" class="Keyword">import</a> <a id="31072" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="31112" class="Keyword">open</a> <a id="31117" class="Keyword">import</a> <a id="31124" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="31146" class="Keyword">open</a> <a id="31151" class="Keyword">import</a> <a id="31158" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="31193" class="Keyword">open</a> <a id="31198" class="Keyword">import</a> <a id="31205" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="31243" class="Keyword">open</a> <a id="31248" class="Keyword">import</a> <a id="31255" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="31294" class="Keyword">open</a> <a id="31299" class="Keyword">import</a> <a id="31306" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="31341" class="Keyword">open</a> <a id="31346" class="Keyword">import</a> <a id="31353" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="31388" class="Keyword">open</a> <a id="31393" class="Keyword">import</a> <a id="31400" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="31438" class="Keyword">open</a> <a id="31443" class="Keyword">import</a> <a id="31450" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="31481" class="Keyword">open</a> <a id="31486" class="Keyword">import</a> <a id="31493" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="31535" class="Keyword">open</a> <a id="31540" class="Keyword">import</a> <a id="31547" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="31592" class="Keyword">open</a> <a id="31597" class="Keyword">import</a> <a id="31604" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="31637" class="Keyword">open</a> <a id="31642" class="Keyword">import</a> <a id="31649" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="31669" class="Keyword">open</a> <a id="31674" class="Keyword">import</a> <a id="31681" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="31704" class="Keyword">open</a> <a id="31709" class="Keyword">import</a> <a id="31716" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="31739" class="Keyword">open</a> <a id="31744" class="Keyword">import</a> <a id="31751" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="31777" class="Keyword">open</a> <a id="31782" class="Keyword">import</a> <a id="31789" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="31815" class="Keyword">open</a> <a id="31820" class="Keyword">import</a> <a id="31827" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="31891" class="Keyword">open</a> <a id="31896" class="Keyword">import</a> <a id="31903" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31921" class="Keyword">open</a> <a id="31926" class="Keyword">import</a> <a id="31933" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31960" class="Keyword">open</a> <a id="31965" class="Keyword">import</a> <a id="31972" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31998" class="Keyword">open</a> <a id="32003" class="Keyword">import</a> <a id="32010" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="32036" class="Keyword">open</a> <a id="32041" class="Keyword">import</a> <a id="32048" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="32074" class="Keyword">open</a> <a id="32079" class="Keyword">import</a> <a id="32086" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="32117" class="Keyword">open</a> <a id="32122" class="Keyword">import</a> <a id="32129" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="32192" class="Keyword">open</a> <a id="32197" class="Keyword">import</a> <a id="32204" href="polytopes.html" class="Module">polytopes</a>
<a id="32214" class="Keyword">open</a> <a id="32219" class="Keyword">import</a> <a id="32226" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="32284" class="Keyword">open</a> <a id="32289" class="Keyword">import</a> <a id="32296" href="ring-theory.html" class="Module">ring-theory</a>
<a id="32308" class="Keyword">open</a> <a id="32313" class="Keyword">import</a> <a id="32320" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="32357" class="Keyword">open</a> <a id="32362" class="Keyword">import</a> <a id="32369" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="32396" class="Keyword">open</a> <a id="32401" class="Keyword">import</a> <a id="32408" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="32440" class="Keyword">open</a> <a id="32445" class="Keyword">import</a> <a id="32452" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="32498" class="Keyword">open</a> <a id="32503" class="Keyword">import</a> <a id="32510" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="32535" class="Keyword">open</a> <a id="32540" class="Keyword">import</a> <a id="32547" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="32590" class="Keyword">open</a> <a id="32595" class="Keyword">import</a> <a id="32602" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="32640" class="Keyword">open</a> <a id="32645" class="Keyword">import</a> <a id="32652" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="32683" class="Keyword">open</a> <a id="32688" class="Keyword">import</a> <a id="32695" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="32719" class="Keyword">open</a> <a id="32724" class="Keyword">import</a> <a id="32731" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="32763" class="Keyword">open</a> <a id="32768" class="Keyword">import</a> <a id="32775" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="32801" class="Keyword">open</a> <a id="32806" class="Keyword">import</a> <a id="32813" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="32842" class="Keyword">open</a> <a id="32847" class="Keyword">import</a> <a id="32854" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="32891" class="Keyword">open</a> <a id="32896" class="Keyword">import</a> <a id="32903" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32932" class="Keyword">open</a> <a id="32937" class="Keyword">import</a> <a id="32944" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32971" class="Keyword">open</a> <a id="32976" class="Keyword">import</a> <a id="32983" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="33020" class="Keyword">open</a> <a id="33025" class="Keyword">import</a> <a id="33032" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="33059" class="Keyword">open</a> <a id="33064" class="Keyword">import</a> <a id="33071" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="33104" class="Keyword">open</a> <a id="33109" class="Keyword">import</a> <a id="33116" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="33134" class="Keyword">open</a> <a id="33139" class="Keyword">import</a> <a id="33146" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="33200" class="Keyword">open</a> <a id="33205" class="Keyword">import</a> <a id="33212" href="set-theory.html" class="Module">set-theory</a>
<a id="33223" class="Keyword">open</a> <a id="33228" class="Keyword">import</a> <a id="33235" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="33258" class="Keyword">open</a> <a id="33263" class="Keyword">import</a> <a id="33270" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="33294" class="Keyword">open</a> <a id="33299" class="Keyword">import</a> <a id="33306" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="33332" class="Keyword">open</a> <a id="33337" class="Keyword">import</a> <a id="33344" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="33406" class="Keyword">open</a> <a id="33411" class="Keyword">import</a> <a id="33418" href="structured-types.html" class="Module">structured-types</a>
<a id="33435" class="Keyword">open</a> <a id="33440" class="Keyword">import</a> <a id="33447" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="33482" class="Keyword">open</a> <a id="33487" class="Keyword">import</a> <a id="33494" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="33538" class="Keyword">open</a> <a id="33543" class="Keyword">import</a> <a id="33550" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="33614" class="Keyword">open</a> <a id="33619" class="Keyword">import</a> <a id="33626" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="33665" class="Keyword">open</a> <a id="33670" class="Keyword">import</a> <a id="33677" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="33723" class="Keyword">open</a> <a id="33728" class="Keyword">import</a> <a id="33735" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="33759" class="Keyword">open</a> <a id="33764" class="Keyword">import</a> <a id="33771" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="33840" class="Keyword">open</a> <a id="33845" class="Keyword">import</a> <a id="33852" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="33897" class="Keyword">open</a> <a id="33902" class="Keyword">import</a> <a id="33909" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33943" class="Keyword">open</a> <a id="33948" class="Keyword">import</a> <a id="33955" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="34016" class="Keyword">open</a> <a id="34021" class="Keyword">import</a> <a id="34028" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="34073" class="Keyword">open</a> <a id="34078" class="Keyword">import</a> <a id="34085" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="34123" class="Keyword">open</a> <a id="34128" class="Keyword">import</a> <a id="34135" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="34178" class="Keyword">open</a> <a id="34183" class="Keyword">import</a> <a id="34190" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="34226" class="Keyword">open</a> <a id="34231" class="Keyword">import</a> <a id="34238" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="34268" class="Keyword">open</a> <a id="34273" class="Keyword">import</a> <a id="34280" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="34311" class="Keyword">open</a> <a id="34316" class="Keyword">import</a> <a id="34323" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="34382" class="Keyword">open</a> <a id="34387" class="Keyword">import</a> <a id="34394" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="34445" class="Keyword">open</a> <a id="34450" class="Keyword">import</a> <a id="34457" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="34508" class="Keyword">open</a> <a id="34513" class="Keyword">import</a> <a id="34520" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="34575" class="Keyword">open</a> <a id="34580" class="Keyword">import</a> <a id="34587" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="34616" class="Keyword">open</a> <a id="34621" class="Keyword">import</a> <a id="34628" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="34656" class="Keyword">open</a> <a id="34661" class="Keyword">import</a> <a id="34668" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="34698" class="Keyword">open</a> <a id="34703" class="Keyword">import</a> <a id="34710" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="34744" class="Keyword">open</a> <a id="34749" class="Keyword">import</a> <a id="34756" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="34832" class="Keyword">open</a> <a id="34837" class="Keyword">import</a> <a id="34844" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="34870" class="Keyword">open</a> <a id="34875" class="Keyword">import</a> <a id="34882" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34920" class="Keyword">open</a> <a id="34925" class="Keyword">import</a> <a id="34932" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34969" class="Keyword">open</a> <a id="34974" class="Keyword">import</a> <a id="34981" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="35021" class="Keyword">open</a> <a id="35026" class="Keyword">import</a> <a id="35033" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="35072" class="Keyword">open</a> <a id="35077" class="Keyword">import</a> <a id="35084" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="35117" class="Keyword">open</a> <a id="35122" class="Keyword">import</a> <a id="35129" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="35172" class="Keyword">open</a> <a id="35177" class="Keyword">import</a> <a id="35184" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="35219" class="Keyword">open</a> <a id="35224" class="Keyword">import</a> <a id="35231" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="35276" class="Keyword">open</a> <a id="35281" class="Keyword">import</a> <a id="35288" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="35340" class="Keyword">open</a> <a id="35345" class="Keyword">import</a> <a id="35352" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="35405" class="Keyword">open</a> <a id="35410" class="Keyword">import</a> <a id="35417" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="35477" class="Keyword">open</a> <a id="35482" class="Keyword">import</a> <a id="35489" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="35537" class="Keyword">open</a> <a id="35542" class="Keyword">import</a> <a id="35549" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="35589" class="Keyword">open</a> <a id="35594" class="Keyword">import</a> <a id="35601" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="35648" class="Keyword">open</a> <a id="35653" class="Keyword">import</a> <a id="35660" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="35701" class="Keyword">open</a> <a id="35706" class="Keyword">import</a> <a id="35713" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="35751" class="Keyword">open</a> <a id="35756" class="Keyword">import</a> <a id="35763" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="35811" class="Keyword">open</a> <a id="35816" class="Keyword">import</a> <a id="35823" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35860" class="Keyword">open</a> <a id="35865" class="Keyword">import</a> <a id="35872" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="35907" class="Keyword">open</a> <a id="35912" class="Keyword">import</a> <a id="35919" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35953" class="Keyword">open</a> <a id="35958" class="Keyword">import</a> <a id="35965" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="36012" class="Keyword">open</a> <a id="36017" class="Keyword">import</a> <a id="36024" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="36069" class="Keyword">open</a> <a id="36074" class="Keyword">import</a> <a id="36081" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="36130" class="Keyword">open</a> <a id="36135" class="Keyword">import</a> <a id="36142" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="36196" class="Keyword">open</a> <a id="36201" class="Keyword">import</a> <a id="36208" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="36285" class="Keyword">open</a> <a id="36290" class="Keyword">import</a> <a id="36297" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="36349" class="Keyword">open</a> <a id="36354" class="Keyword">import</a> <a id="36361" href="type-theories.html" class="Module">type-theories</a>
<a id="36375" class="Keyword">open</a> <a id="36380" class="Keyword">import</a> <a id="36387" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="36429" class="Keyword">open</a> <a id="36434" class="Keyword">import</a> <a id="36441" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="36479" class="Keyword">open</a> <a id="36484" class="Keyword">import</a> <a id="36491" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="36537" class="Keyword">open</a> <a id="36542" class="Keyword">import</a> <a id="36549" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="36596" class="Keyword">open</a> <a id="36601" class="Keyword">import</a> <a id="36608" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="36643" class="Keyword">open</a> <a id="36648" class="Keyword">import</a> <a id="36655" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="36733" class="Keyword">open</a> <a id="36738" class="Keyword">import</a> <a id="36745" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="36769" class="Keyword">open</a> <a id="36774" class="Keyword">import</a> <a id="36781" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="36834" class="Keyword">open</a> <a id="36839" class="Keyword">import</a> <a id="36846" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="36889" class="Keyword">open</a> <a id="36894" class="Keyword">import</a> <a id="36901" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="36941" class="Keyword">open</a> <a id="36946" class="Keyword">import</a> <a id="36953" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36992" class="Keyword">open</a> <a id="36997" class="Keyword">import</a> <a id="37004" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="37038" class="Keyword">open</a> <a id="37043" class="Keyword">import</a> <a id="37050" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="37098" class="Keyword">open</a> <a id="37103" class="Keyword">import</a> <a id="37110" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="37161" class="Keyword">open</a> <a id="37166" class="Keyword">import</a> <a id="37173" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="37220" class="Keyword">open</a> <a id="37225" class="Keyword">import</a> <a id="37232" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="37284" class="Keyword">open</a> <a id="37289" class="Keyword">import</a> <a id="37296" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="37340" class="Keyword">open</a> <a id="37345" class="Keyword">import</a> <a id="37352" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="37392" class="Keyword">open</a> <a id="37397" class="Keyword">import</a> <a id="37404" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="37447" class="Keyword">open</a> <a id="37452" class="Keyword">import</a> <a id="37459" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="37511" class="Keyword">open</a> <a id="37516" class="Keyword">import</a> <a id="37523" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="37577" class="Keyword">open</a> <a id="37582" class="Keyword">import</a> <a id="37589" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="37637" class="Keyword">open</a> <a id="37642" class="Keyword">import</a> <a id="37649" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="37688" class="Keyword">open</a> <a id="37693" class="Keyword">import</a> <a id="37700" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="37733" class="Keyword">open</a> <a id="37738" class="Keyword">import</a> <a id="37745" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="37775" class="Keyword">open</a> <a id="37780" class="Keyword">import</a> <a id="37787" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="37838" class="Keyword">open</a> <a id="37843" class="Keyword">import</a> <a id="37850" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="37891" class="Keyword">open</a> <a id="37896" class="Keyword">import</a> <a id="37903" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="37940" class="Keyword">open</a> <a id="37945" class="Keyword">import</a> <a id="37952" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="38011" class="Keyword">open</a> <a id="38016" class="Keyword">import</a> <a id="38023" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="38078" class="Keyword">open</a> <a id="38083" class="Keyword">import</a> <a id="38090" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="38146" class="Keyword">open</a> <a id="38151" class="Keyword">import</a> <a id="38158" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="38205" class="Keyword">open</a> <a id="38210" class="Keyword">import</a> <a id="38217" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="38260" class="Keyword">open</a> <a id="38265" class="Keyword">import</a> <a id="38272" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="38317" class="Keyword">open</a> <a id="38322" class="Keyword">import</a> <a id="38329" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="38378" class="Keyword">open</a> <a id="38383" class="Keyword">import</a> <a id="38390" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="38441" class="Keyword">open</a> <a id="38446" class="Keyword">import</a> <a id="38453" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="38497" class="Keyword">open</a> <a id="38502" class="Keyword">import</a> <a id="38509" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="38587" class="Keyword">open</a> <a id="38592" class="Keyword">import</a> <a id="38599" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="38639" class="Keyword">open</a> <a id="38644" class="Keyword">import</a> <a id="38651" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="38708" class="Keyword">open</a> <a id="38713" class="Keyword">import</a> <a id="38720" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="38755" class="Keyword">open</a> <a id="38760" class="Keyword">import</a> <a id="38767" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="38813" class="Keyword">open</a> <a id="38818" class="Keyword">import</a> <a id="38825" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="38880" class="Keyword">open</a> <a id="38885" class="Keyword">import</a> <a id="38892" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="38935" class="Keyword">open</a> <a id="38940" class="Keyword">import</a> <a id="38947" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38992" class="Keyword">open</a> <a id="38997" class="Keyword">import</a> <a id="39004" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="39063" class="Keyword">open</a> <a id="39068" class="Keyword">import</a> <a id="39075" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="39112" class="Keyword">open</a> <a id="39117" class="Keyword">import</a> <a id="39124" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="39166" class="Keyword">open</a> <a id="39171" class="Keyword">import</a> <a id="39178" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="39219" class="Keyword">open</a> <a id="39224" class="Keyword">import</a> <a id="39231" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="39270" class="Keyword">open</a> <a id="39275" class="Keyword">import</a> <a id="39282" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="39320" class="Keyword">open</a> <a id="39325" class="Keyword">import</a> <a id="39332" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="39384" class="Keyword">open</a> <a id="39389" class="Keyword">import</a> <a id="39396" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="39441" class="Keyword">open</a> <a id="39446" class="Keyword">import</a> <a id="39453" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="39492" class="Keyword">open</a> <a id="39497" class="Keyword">import</a> <a id="39504" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="39541" class="Keyword">open</a> <a id="39546" class="Keyword">import</a> <a id="39553" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="39602" class="Keyword">open</a> <a id="39607" class="Keyword">import</a> <a id="39614" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="39653" class="Keyword">open</a> <a id="39658" class="Keyword">import</a> <a id="39665" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="39703" class="Keyword">open</a> <a id="39708" class="Keyword">import</a> <a id="39715" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="39770" class="Keyword">open</a> <a id="39775" class="Keyword">import</a> <a id="39782" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="39821" class="Keyword">open</a> <a id="39826" class="Keyword">import</a> <a id="39833" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="39881" class="Keyword">open</a> <a id="39886" class="Keyword">import</a> <a id="39893" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="39940" class="Keyword">open</a> <a id="39945" class="Keyword">import</a> <a id="39952" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39990" class="Keyword">open</a> <a id="39995" class="Keyword">import</a> <a id="40002" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="40032" class="Keyword">open</a> <a id="40037" class="Keyword">import</a> <a id="40044" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="40101" class="Keyword">open</a> <a id="40106" class="Keyword">import</a> <a id="40113" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="40167" class="Keyword">open</a> <a id="40172" class="Keyword">import</a> <a id="40179" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="40209" class="Keyword">open</a> <a id="40214" class="Keyword">import</a> <a id="40221" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="40270" class="Keyword">open</a> <a id="40275" class="Keyword">import</a> <a id="40282" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="40324" class="Keyword">open</a> <a id="40329" class="Keyword">import</a> <a id="40336" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="40370" class="Keyword">open</a> <a id="40375" class="Keyword">import</a> <a id="40382" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="40445" class="Keyword">open</a> <a id="40450" class="Keyword">import</a> <a id="40457" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="40500" class="Keyword">open</a> <a id="40505" class="Keyword">import</a> <a id="40512" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="40547" class="Keyword">open</a> <a id="40552" class="Keyword">import</a> <a id="40559" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="40594" class="Keyword">open</a> <a id="40599" class="Keyword">import</a> <a id="40606" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="40646" class="Keyword">open</a> <a id="40651" class="Keyword">import</a> <a id="40658" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="40703" class="Keyword">open</a> <a id="40708" class="Keyword">import</a> <a id="40715" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="40756" class="Keyword">open</a> <a id="40761" class="Keyword">import</a> <a id="40768" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="40822" class="Keyword">open</a> <a id="40827" class="Keyword">import</a> <a id="40834" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="40884" class="Keyword">open</a> <a id="40889" class="Keyword">import</a> <a id="40896" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="40943" class="Keyword">open</a> <a id="40948" class="Keyword">import</a> <a id="40955" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40993" class="Keyword">open</a> <a id="40998" class="Keyword">import</a> <a id="41005" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="41054" class="Keyword">open</a> <a id="41059" class="Keyword">import</a> <a id="41066" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="41113" class="Keyword">open</a> <a id="41118" class="Keyword">import</a> <a id="41125" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="41188" class="Keyword">open</a> <a id="41193" class="Keyword">import</a> <a id="41200" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="41232" class="Keyword">open</a> <a id="41237" class="Keyword">import</a> <a id="41244" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="41297" class="Keyword">open</a> <a id="41302" class="Keyword">import</a> <a id="41309" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="41355" class="Keyword">open</a> <a id="41360" class="Keyword">import</a> <a id="41367" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="41413" class="Keyword">open</a> <a id="41418" class="Keyword">import</a> <a id="41425" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="41465" class="Keyword">open</a> <a id="41470" class="Keyword">import</a> <a id="41477" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="41524" class="Keyword">open</a> <a id="41529" class="Keyword">import</a> <a id="41536" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="41584" class="Keyword">open</a> <a id="41589" class="Keyword">import</a> <a id="41596" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="41636" class="Keyword">open</a> <a id="41641" class="Keyword">import</a> <a id="41648" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="41693" class="Keyword">open</a> <a id="41698" class="Keyword">import</a> <a id="41705" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="41770" class="Keyword">open</a> <a id="41775" class="Keyword">import</a> <a id="41782" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="41827" class="Keyword">open</a> <a id="41832" class="Keyword">import</a> <a id="41839" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="41886" class="Keyword">open</a> <a id="41891" class="Keyword">import</a> <a id="41898" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="41951" class="Keyword">open</a> <a id="41956" class="Keyword">import</a> <a id="41963" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>