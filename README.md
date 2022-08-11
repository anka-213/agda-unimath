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
<a id="8652" class="Keyword">open</a> <a id="8657" class="Keyword">import</a> <a id="8664" href="elementary-number-theory.multiset-coefficients.html" class="Module">elementary-number-theory.multiset-coefficients</a>
<a id="8711" class="Keyword">open</a> <a id="8716" class="Keyword">import</a> <a id="8723" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8764" class="Keyword">open</a> <a id="8769" class="Keyword">import</a> <a id="8776" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8825" class="Keyword">open</a> <a id="8830" class="Keyword">import</a> <a id="8837" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8896" class="Keyword">open</a> <a id="8901" class="Keyword">import</a> <a id="8908" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8947" class="Keyword">open</a> <a id="8952" class="Keyword">import</a> <a id="8959" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="9012" class="Keyword">open</a> <a id="9017" class="Keyword">import</a> <a id="9024" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="9081" class="Keyword">open</a> <a id="9086" class="Keyword">import</a> <a id="9093" href="elementary-number-theory.pythagorean-triples.html" class="Module">elementary-number-theory.pythagorean-triples</a>
<a id="9138" class="Keyword">open</a> <a id="9143" class="Keyword">import</a> <a id="9150" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="9192" class="Keyword">open</a> <a id="9197" class="Keyword">import</a> <a id="9204" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="9255" class="Keyword">open</a> <a id="9260" class="Keyword">import</a> <a id="9267" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9325" class="Keyword">open</a> <a id="9330" class="Keyword">import</a> <a id="9337" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9401" class="Keyword">open</a> <a id="9406" class="Keyword">import</a> <a id="9413" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9466" class="Keyword">open</a> <a id="9471" class="Keyword">import</a> <a id="9478" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9531" class="Keyword">open</a> <a id="9536" class="Keyword">import</a> <a id="9543" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9604" class="Keyword">open</a> <a id="9609" class="Keyword">import</a> <a id="9616" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9674" class="Keyword">open</a> <a id="9679" class="Keyword">import</a> <a id="9686" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9735" class="Keyword">open</a> <a id="9740" class="Keyword">import</a> <a id="9747" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9790" class="Keyword">open</a> <a id="9795" class="Keyword">import</a> <a id="9802" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9846" class="Keyword">open</a> <a id="9851" class="Keyword">import</a> <a id="9858" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9905" class="Keyword">open</a> <a id="9910" class="Keyword">import</a> <a id="9917" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9978" class="Keyword">open</a> <a id="9983" class="Keyword">import</a> <a id="9990" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="10053" class="Keyword">open</a> <a id="10058" class="Keyword">import</a> <a id="10065" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="10125" class="Keyword">open</a> <a id="10130" class="Keyword">import</a> <a id="10137" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="10191" class="Keyword">open</a> <a id="10196" class="Keyword">import</a> <a id="10203" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="10268" class="Keyword">open</a> <a id="10273" class="Keyword">import</a> <a id="10280" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10388" class="Keyword">open</a> <a id="10393" class="Keyword">import</a> <a id="10400" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10420" class="Keyword">open</a> <a id="10425" class="Keyword">import</a> <a id="10432" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10478" class="Keyword">open</a> <a id="10483" class="Keyword">import</a> <a id="10490" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a>
<a id="10529" class="Keyword">open</a> <a id="10534" class="Keyword">import</a> <a id="10541" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10597" class="Keyword">open</a> <a id="10602" class="Keyword">import</a> <a id="10609" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10655" class="Keyword">open</a> <a id="10660" class="Keyword">import</a> <a id="10667" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10701" class="Keyword">open</a> <a id="10706" class="Keyword">import</a> <a id="10713" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10748" class="Keyword">open</a> <a id="10753" class="Keyword">import</a> <a id="10760" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10798" class="Keyword">open</a> <a id="10803" class="Keyword">import</a> <a id="10810" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10848" class="Keyword">open</a> <a id="10853" class="Keyword">import</a> <a id="10860" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10900" class="Keyword">open</a> <a id="10905" class="Keyword">import</a> <a id="10912" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10945" class="Keyword">open</a> <a id="10950" class="Keyword">import</a> <a id="10957" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10995" class="Keyword">open</a> <a id="11000" class="Keyword">import</a> <a id="11007" href="finite-group-theory.simpson-delooping-sign-homomorphism.html" class="Module">finite-group-theory.simpson-delooping-sign-homomorphism</a>
<a id="11063" class="Keyword">open</a> <a id="11068" class="Keyword">import</a> <a id="11075" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="11117" class="Keyword">open</a> <a id="11122" class="Keyword">import</a> <a id="11129" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="11192" class="Keyword">open</a> <a id="11197" class="Keyword">import</a> <a id="11204" href="foundation.html" class="Module">foundation</a>
<a id="11215" class="Keyword">open</a> <a id="11220" class="Keyword">import</a> <a id="11227" href="foundation.0-connected-types.html" class="Module">foundation.0-connected-types</a>
<a id="11256" class="Keyword">open</a> <a id="11261" class="Keyword">import</a> <a id="11268" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a>
<a id="11296" class="Keyword">open</a> <a id="11301" class="Keyword">import</a> <a id="11308" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11326" class="Keyword">open</a> <a id="11331" class="Keyword">import</a> <a id="11338" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11357" class="Keyword">open</a> <a id="11362" class="Keyword">import</a> <a id="11369" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11388" class="Keyword">open</a> <a id="11393" class="Keyword">import</a> <a id="11400" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11444" class="Keyword">open</a> <a id="11449" class="Keyword">import</a> <a id="11456" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11481" class="Keyword">open</a> <a id="11486" class="Keyword">import</a> <a id="11493" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11520" class="Keyword">open</a> <a id="11525" class="Keyword">import</a> <a id="11532" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11549" class="Keyword">open</a> <a id="11554" class="Keyword">import</a> <a id="11561" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11590" class="Keyword">open</a> <a id="11595" class="Keyword">import</a> <a id="11602" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11658" class="Keyword">open</a> <a id="11663" class="Keyword">import</a> <a id="11670" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11701" class="Keyword">open</a> <a id="11706" class="Keyword">import</a> <a id="11713" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11767" class="Keyword">open</a> <a id="11772" class="Keyword">import</a> <a id="11779" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11807" class="Keyword">open</a> <a id="11812" class="Keyword">import</a> <a id="11819" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11849" class="Keyword">open</a> <a id="11854" class="Keyword">import</a> <a id="11861" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11881" class="Keyword">open</a> <a id="11886" class="Keyword">import</a> <a id="11893" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11938" class="Keyword">open</a> <a id="11943" class="Keyword">import</a> <a id="11950" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11987" class="Keyword">open</a> <a id="11992" class="Keyword">import</a> <a id="11999" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="12034" class="Keyword">open</a> <a id="12039" class="Keyword">import</a> <a id="12046" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="12104" class="Keyword">open</a> <a id="12109" class="Keyword">import</a> <a id="12116" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12154" class="Keyword">open</a> <a id="12159" class="Keyword">import</a> <a id="12166" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12200" class="Keyword">open</a> <a id="12205" class="Keyword">import</a> <a id="12212" href="foundation.commuting-cubes.html" class="Module">foundation.commuting-cubes</a>
<a id="12239" class="Keyword">open</a> <a id="12244" class="Keyword">import</a> <a id="12251" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12280" class="Keyword">open</a> <a id="12285" class="Keyword">import</a> <a id="12292" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12315" class="Keyword">open</a> <a id="12320" class="Keyword">import</a> <a id="12327" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12354" class="Keyword">open</a> <a id="12359" class="Keyword">import</a> <a id="12366" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12389" class="Keyword">open</a> <a id="12394" class="Keyword">import</a> <a id="12401" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12443" class="Keyword">open</a> <a id="12448" class="Keyword">import</a> <a id="12455" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12487" class="Keyword">open</a> <a id="12492" class="Keyword">import</a> <a id="12499" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="12525" class="Keyword">open</a> <a id="12530" class="Keyword">import</a> <a id="12537" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12564" class="Keyword">open</a> <a id="12569" class="Keyword">import</a> <a id="12576" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12601" class="Keyword">open</a> <a id="12606" class="Keyword">import</a> <a id="12613" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12642" class="Keyword">open</a> <a id="12647" class="Keyword">import</a> <a id="12654" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12684" class="Keyword">open</a> <a id="12689" class="Keyword">import</a> <a id="12696" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12723" class="Keyword">open</a> <a id="12728" class="Keyword">import</a> <a id="12735" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12754" class="Keyword">open</a> <a id="12759" class="Keyword">import</a> <a id="12766" href="foundation.cospans.html" class="Module">foundation.cospans</a>
<a id="12785" class="Keyword">open</a> <a id="12790" class="Keyword">import</a> <a id="12797" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12843" class="Keyword">open</a> <a id="12848" class="Keyword">import</a> <a id="12855" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12897" class="Keyword">open</a> <a id="12902" class="Keyword">import</a> <a id="12909" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12941" class="Keyword">open</a> <a id="12946" class="Keyword">import</a> <a id="12953" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12983" class="Keyword">open</a> <a id="12988" class="Keyword">import</a> <a id="12995" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="13038" class="Keyword">open</a> <a id="13043" class="Keyword">import</a> <a id="13050" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="13076" class="Keyword">open</a> <a id="13081" class="Keyword">import</a> <a id="13088" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="13122" class="Keyword">open</a> <a id="13127" class="Keyword">import</a> <a id="13134" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="13165" class="Keyword">open</a> <a id="13170" class="Keyword">import</a> <a id="13177" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13207" class="Keyword">open</a> <a id="13212" class="Keyword">import</a> <a id="13219" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13246" class="Keyword">open</a> <a id="13251" class="Keyword">import</a> <a id="13258" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13296" class="Keyword">open</a> <a id="13301" class="Keyword">import</a> <a id="13308" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13340" class="Keyword">open</a> <a id="13345" class="Keyword">import</a> <a id="13352" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13387" class="Keyword">open</a> <a id="13392" class="Keyword">import</a> <a id="13399" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13439" class="Keyword">open</a> <a id="13444" class="Keyword">import</a> <a id="13451" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13482" class="Keyword">open</a> <a id="13487" class="Keyword">import</a> <a id="13494" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13528" class="Keyword">open</a> <a id="13533" class="Keyword">import</a> <a id="13540" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="13569" class="Keyword">open</a> <a id="13574" class="Keyword">import</a> <a id="13581" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13604" class="Keyword">open</a> <a id="13609" class="Keyword">import</a> <a id="13616" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13643" class="Keyword">open</a> <a id="13648" class="Keyword">import</a> <a id="13655" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13683" class="Keyword">open</a> <a id="13688" class="Keyword">import</a> <a id="13695" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13732" class="Keyword">open</a> <a id="13737" class="Keyword">import</a> <a id="13744" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13792" class="Keyword">open</a> <a id="13797" class="Keyword">import</a> <a id="13804" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13844" class="Keyword">open</a> <a id="13849" class="Keyword">import</a> <a id="13856" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13878" class="Keyword">open</a> <a id="13883" class="Keyword">import</a> <a id="13890" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13913" class="Keyword">open</a> <a id="13918" class="Keyword">import</a> <a id="13925" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13950" class="Keyword">open</a> <a id="13955" class="Keyword">import</a> <a id="13962" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="14007" class="Keyword">open</a> <a id="14012" class="Keyword">import</a> <a id="14019" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="14063" class="Keyword">open</a> <a id="14068" class="Keyword">import</a> <a id="14075" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14111" class="Keyword">open</a> <a id="14116" class="Keyword">import</a> <a id="14123" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14168" class="Keyword">open</a> <a id="14173" class="Keyword">import</a> <a id="14180" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14221" class="Keyword">open</a> <a id="14226" class="Keyword">import</a> <a id="14233" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14268" class="Keyword">open</a> <a id="14273" class="Keyword">import</a> <a id="14280" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14312" class="Keyword">open</a> <a id="14317" class="Keyword">import</a> <a id="14324" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14355" class="Keyword">open</a> <a id="14360" class="Keyword">import</a> <a id="14367" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14400" class="Keyword">open</a> <a id="14405" class="Keyword">import</a> <a id="14412" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14445" class="Keyword">open</a> <a id="14450" class="Keyword">import</a> <a id="14457" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14487" class="Keyword">open</a> <a id="14492" class="Keyword">import</a> <a id="14499" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14523" class="Keyword">open</a> <a id="14528" class="Keyword">import</a> <a id="14535" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14573" class="Keyword">open</a> <a id="14578" class="Keyword">import</a> <a id="14585" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14616" class="Keyword">open</a> <a id="14621" class="Keyword">import</a> <a id="14628" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14653" class="Keyword">open</a> <a id="14658" class="Keyword">import</a> <a id="14665" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14693" class="Keyword">open</a> <a id="14698" class="Keyword">import</a> <a id="14705" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14729" class="Keyword">open</a> <a id="14734" class="Keyword">import</a> <a id="14741" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14767" class="Keyword">open</a> <a id="14772" class="Keyword">import</a> <a id="14779" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14814" class="Keyword">open</a> <a id="14819" class="Keyword">import</a> <a id="14826" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14847" class="Keyword">open</a> <a id="14852" class="Keyword">import</a> <a id="14859" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14908" class="Keyword">open</a> <a id="14913" class="Keyword">import</a> <a id="14920" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14961" class="Keyword">open</a> <a id="14966" class="Keyword">import</a> <a id="14973" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="15023" class="Keyword">open</a> <a id="15028" class="Keyword">import</a> <a id="15035" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="15081" class="Keyword">open</a> <a id="15086" class="Keyword">import</a> <a id="15093" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15133" class="Keyword">open</a> <a id="15138" class="Keyword">import</a> <a id="15145" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15185" class="Keyword">open</a> <a id="15190" class="Keyword">import</a> <a id="15197" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15247" class="Keyword">open</a> <a id="15252" class="Keyword">import</a> <a id="15259" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15298" class="Keyword">open</a> <a id="15303" class="Keyword">import</a> <a id="15310" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15350" class="Keyword">open</a> <a id="15355" class="Keyword">import</a> <a id="15362" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15395" class="Keyword">open</a> <a id="15400" class="Keyword">import</a> <a id="15407" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15456" class="Keyword">open</a> <a id="15461" class="Keyword">import</a> <a id="15468" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15493" class="Keyword">open</a> <a id="15498" class="Keyword">import</a> <a id="15505" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="15544" class="Keyword">open</a> <a id="15549" class="Keyword">import</a> <a id="15556" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15594" class="Keyword">open</a> <a id="15599" class="Keyword">import</a> <a id="15606" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15628" class="Keyword">open</a> <a id="15633" class="Keyword">import</a> <a id="15640" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15668" class="Keyword">open</a> <a id="15673" class="Keyword">import</a> <a id="15680" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15716" class="Keyword">open</a> <a id="15721" class="Keyword">import</a> <a id="15728" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15754" class="Keyword">open</a> <a id="15759" class="Keyword">import</a> <a id="15766" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15784" class="Keyword">open</a> <a id="15789" class="Keyword">import</a> <a id="15796" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15831" class="Keyword">open</a> <a id="15836" class="Keyword">import</a> <a id="15843" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15878" class="Keyword">open</a> <a id="15883" class="Keyword">import</a> <a id="15890" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15917" class="Keyword">open</a> <a id="15922" class="Keyword">import</a> <a id="15929" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15985" class="Keyword">open</a> <a id="15990" class="Keyword">import</a> <a id="15997" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="16026" class="Keyword">open</a> <a id="16031" class="Keyword">import</a> <a id="16038" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="16068" class="Keyword">open</a> <a id="16073" class="Keyword">import</a> <a id="16080" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="16107" class="Keyword">open</a> <a id="16112" class="Keyword">import</a> <a id="16119" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16145" class="Keyword">open</a> <a id="16150" class="Keyword">import</a> <a id="16157" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16184" class="Keyword">open</a> <a id="16189" class="Keyword">import</a> <a id="16196" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16220" class="Keyword">open</a> <a id="16225" class="Keyword">import</a> <a id="16232" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16255" class="Keyword">open</a> <a id="16260" class="Keyword">import</a> <a id="16267" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16294" class="Keyword">open</a> <a id="16299" class="Keyword">import</a> <a id="16306" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16338" class="Keyword">open</a> <a id="16343" class="Keyword">import</a> <a id="16350" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16385" class="Keyword">open</a> <a id="16390" class="Keyword">import</a> <a id="16397" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16428" class="Keyword">open</a> <a id="16433" class="Keyword">import</a> <a id="16440" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16473" class="Keyword">open</a> <a id="16478" class="Keyword">import</a> <a id="16485" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16519" class="Keyword">open</a> <a id="16524" class="Keyword">import</a> <a id="16531" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16571" class="Keyword">open</a> <a id="16576" class="Keyword">import</a> <a id="16583" href="foundation.lesser-limited-principle-of-omniscience.html" class="Module">foundation.lesser-limited-principle-of-omniscience</a>
<a id="16634" class="Keyword">open</a> <a id="16639" class="Keyword">import</a> <a id="16646" href="foundation.limited-principle-of-omniscience.html" class="Module">foundation.limited-principle-of-omniscience</a>
<a id="16690" class="Keyword">open</a> <a id="16695" class="Keyword">import</a> <a id="16702" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16733" class="Keyword">open</a> <a id="16738" class="Keyword">import</a> <a id="16745" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16777" class="Keyword">open</a> <a id="16782" class="Keyword">import</a> <a id="16789" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16820" class="Keyword">open</a> <a id="16825" class="Keyword">import</a> <a id="16832" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16849" class="Keyword">open</a> <a id="16854" class="Keyword">import</a> <a id="16861" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16886" class="Keyword">open</a> <a id="16891" class="Keyword">import</a> <a id="16898" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16927" class="Keyword">open</a> <a id="16932" class="Keyword">import</a> <a id="16939" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16964" class="Keyword">open</a> <a id="16969" class="Keyword">import</a> <a id="16976" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="17005" class="Keyword">open</a> <a id="17010" class="Keyword">import</a> <a id="17017" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="17038" class="Keyword">open</a> <a id="17043" class="Keyword">import</a> <a id="17050" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="17074" class="Keyword">open</a> <a id="17079" class="Keyword">import</a> <a id="17086" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="17106" class="Keyword">open</a> <a id="17111" class="Keyword">import</a> <a id="17118" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="17152" class="Keyword">open</a> <a id="17157" class="Keyword">import</a> <a id="17164" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17202" class="Keyword">open</a> <a id="17207" class="Keyword">import</a> <a id="17214" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17242" class="Keyword">open</a> <a id="17247" class="Keyword">import</a> <a id="17254" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17278" class="Keyword">open</a> <a id="17283" class="Keyword">import</a> <a id="17290" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17317" class="Keyword">open</a> <a id="17322" class="Keyword">import</a> <a id="17329" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17364" class="Keyword">open</a> <a id="17369" class="Keyword">import</a> <a id="17376" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17397" class="Keyword">open</a> <a id="17402" class="Keyword">import</a> <a id="17409" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17445" class="Keyword">open</a> <a id="17450" class="Keyword">import</a> <a id="17457" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17502" class="Keyword">open</a> <a id="17507" class="Keyword">import</a> <a id="17514" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17560" class="Keyword">open</a> <a id="17565" class="Keyword">import</a> <a id="17572" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17612" class="Keyword">open</a> <a id="17617" class="Keyword">import</a> <a id="17624" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17654" class="Keyword">open</a> <a id="17659" class="Keyword">import</a> <a id="17666" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17700" class="Keyword">open</a> <a id="17705" class="Keyword">import</a> <a id="17712" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17749" class="Keyword">open</a> <a id="17754" class="Keyword">import</a> <a id="17761" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17785" class="Keyword">open</a> <a id="17790" class="Keyword">import</a> <a id="17797" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17818" class="Keyword">open</a> <a id="17823" class="Keyword">import</a> <a id="17830" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17865" class="Keyword">open</a> <a id="17870" class="Keyword">import</a> <a id="17877" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17914" class="Keyword">open</a> <a id="17919" class="Keyword">import</a> <a id="17926" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17975" class="Keyword">open</a> <a id="17980" class="Keyword">import</a> <a id="17987" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="18020" class="Keyword">open</a> <a id="18025" class="Keyword">import</a> <a id="18032" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="18055" class="Keyword">open</a> <a id="18060" class="Keyword">import</a> <a id="18067" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="18090" class="Keyword">open</a> <a id="18095" class="Keyword">import</a> <a id="18102" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18125" class="Keyword">open</a> <a id="18130" class="Keyword">import</a> <a id="18137" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18165" class="Keyword">open</a> <a id="18170" class="Keyword">import</a> <a id="18177" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18197" class="Keyword">open</a> <a id="18202" class="Keyword">import</a> <a id="18209" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18230" class="Keyword">open</a> <a id="18235" class="Keyword">import</a> <a id="18242" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18273" class="Keyword">open</a> <a id="18278" class="Keyword">import</a> <a id="18285" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18312" class="Keyword">open</a> <a id="18317" class="Keyword">import</a> <a id="18324" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18340" class="Keyword">open</a> <a id="18345" class="Keyword">import</a> <a id="18352" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18383" class="Keyword">open</a> <a id="18388" class="Keyword">import</a> <a id="18395" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18412" class="Keyword">open</a> <a id="18417" class="Keyword">import</a> <a id="18424" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18446" class="Keyword">open</a> <a id="18451" class="Keyword">import</a> <a id="18458" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18485" class="Keyword">open</a> <a id="18490" class="Keyword">import</a> <a id="18497" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18520" class="Keyword">open</a> <a id="18525" class="Keyword">import</a> <a id="18532" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18559" class="Keyword">open</a> <a id="18564" class="Keyword">import</a> <a id="18571" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18604" class="Keyword">open</a> <a id="18609" class="Keyword">import</a> <a id="18616" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18656" class="Keyword">open</a> <a id="18661" class="Keyword">import</a> <a id="18668" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18689" class="Keyword">open</a> <a id="18694" class="Keyword">import</a> <a id="18701" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18730" class="Keyword">open</a> <a id="18735" class="Keyword">import</a> <a id="18742" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18780" class="Keyword">open</a> <a id="18785" class="Keyword">import</a> <a id="18792" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18812" class="Keyword">open</a> <a id="18817" class="Keyword">import</a> <a id="18824" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18848" class="Keyword">open</a> <a id="18853" class="Keyword">import</a> <a id="18860" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18887" class="Keyword">open</a> <a id="18892" class="Keyword">import</a> <a id="18899" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18931" class="Keyword">open</a> <a id="18936" class="Keyword">import</a> <a id="18943" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18973" class="Keyword">open</a> <a id="18978" class="Keyword">import</a> <a id="18985" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19011" class="Keyword">open</a> <a id="19016" class="Keyword">import</a> <a id="19023" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19050" class="Keyword">open</a> <a id="19055" class="Keyword">import</a> <a id="19062" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19099" class="Keyword">open</a> <a id="19104" class="Keyword">import</a> <a id="19111" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19140" class="Keyword">open</a> <a id="19145" class="Keyword">import</a> <a id="19152" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19175" class="Keyword">open</a> <a id="19180" class="Keyword">import</a> <a id="19187" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19238" class="Keyword">open</a> <a id="19243" class="Keyword">import</a> <a id="19250" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19293" class="Keyword">open</a> <a id="19298" class="Keyword">import</a> <a id="19305" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19357" class="Keyword">open</a> <a id="19362" class="Keyword">import</a> <a id="19369" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19417" class="Keyword">open</a> <a id="19422" class="Keyword">import</a> <a id="19429" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19467" class="Keyword">open</a> <a id="19472" class="Keyword">import</a> <a id="19479" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19516" class="Keyword">open</a> <a id="19521" class="Keyword">import</a> <a id="19528" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19574" class="Keyword">open</a> <a id="19579" class="Keyword">import</a> <a id="19586" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19603" class="Keyword">open</a> <a id="19608" class="Keyword">import</a> <a id="19615" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19643" class="Keyword">open</a> <a id="19648" class="Keyword">import</a> <a id="19655" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19683" class="Keyword">open</a> <a id="19688" class="Keyword">import</a> <a id="19695" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19731" class="Keyword">open</a> <a id="19736" class="Keyword">import</a> <a id="19743" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19781" class="Keyword">open</a> <a id="19786" class="Keyword">import</a> <a id="19793" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19826" class="Keyword">open</a> <a id="19831" class="Keyword">import</a> <a id="19838" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19859" class="Keyword">open</a> <a id="19864" class="Keyword">import</a> <a id="19871" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19907" class="Keyword">open</a> <a id="19912" class="Keyword">import</a> <a id="19919" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19973" class="Keyword">open</a> <a id="19978" class="Keyword">import</a> <a id="19985" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20007" class="Keyword">open</a> <a id="20012" class="Keyword">import</a> <a id="20019" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20054" class="Keyword">open</a> <a id="20059" class="Keyword">import</a> <a id="20066" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20096" class="Keyword">open</a> <a id="20101" class="Keyword">import</a> <a id="20108" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20147" class="Keyword">open</a> <a id="20152" class="Keyword">import</a> <a id="20159" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20213" class="Keyword">open</a> <a id="20218" class="Keyword">import</a> <a id="20225" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20271" class="Keyword">open</a> <a id="20276" class="Keyword">import</a> <a id="20283" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20334" class="Keyword">open</a> <a id="20339" class="Keyword">import</a> <a id="20346" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20387" class="Keyword">open</a> <a id="20392" class="Keyword">import</a> <a id="20399" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20444" class="Keyword">open</a> <a id="20449" class="Keyword">import</a> <a id="20456" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20501" class="Keyword">open</a> <a id="20506" class="Keyword">import</a> <a id="20513" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20549" class="Keyword">open</a> <a id="20554" class="Keyword">import</a> <a id="20561" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20597" class="Keyword">open</a> <a id="20602" class="Keyword">import</a> <a id="20609" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20674" class="Keyword">open</a> <a id="20679" class="Keyword">import</a> <a id="20686" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20741" class="Keyword">open</a> <a id="20746" class="Keyword">import</a> <a id="20753" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20793" class="Keyword">open</a> <a id="20798" class="Keyword">import</a> <a id="20805" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20849" class="Keyword">open</a> <a id="20854" class="Keyword">import</a> <a id="20861" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20906" class="Keyword">open</a> <a id="20911" class="Keyword">import</a> <a id="20918" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20959" class="Keyword">open</a> <a id="20964" class="Keyword">import</a> <a id="20971" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21011" class="Keyword">open</a> <a id="21016" class="Keyword">import</a> <a id="21023" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21050" class="Keyword">open</a> <a id="21055" class="Keyword">import</a> <a id="21062" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21098" class="Keyword">open</a> <a id="21103" class="Keyword">import</a> <a id="21110" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21137" class="Keyword">open</a> <a id="21142" class="Keyword">import</a> <a id="21149" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21186" class="Keyword">open</a> <a id="21191" class="Keyword">import</a> <a id="21198" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21226" class="Keyword">open</a> <a id="21231" class="Keyword">import</a> <a id="21238" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21257" class="Keyword">open</a> <a id="21262" class="Keyword">import</a> <a id="21269" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21309" class="Keyword">open</a> <a id="21314" class="Keyword">import</a> <a id="21321" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="21370" class="Keyword">open</a> <a id="21375" class="Keyword">import</a> <a id="21382" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21414" class="Keyword">open</a> <a id="21419" class="Keyword">import</a> <a id="21426" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21474" class="Keyword">open</a> <a id="21479" class="Keyword">import</a> <a id="21486" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21509" class="Keyword">open</a> <a id="21514" class="Keyword">import</a> <a id="21521" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21545" class="Keyword">open</a> <a id="21550" class="Keyword">import</a> <a id="21557" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21597" class="Keyword">open</a> <a id="21602" class="Keyword">import</a> <a id="21609" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="21652" class="Keyword">open</a> <a id="21657" class="Keyword">import</a> <a id="21664" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21698" class="Keyword">open</a> <a id="21703" class="Keyword">import</a> <a id="21710" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21742" class="Keyword">open</a> <a id="21747" class="Keyword">import</a> <a id="21754" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21784" class="Keyword">open</a> <a id="21789" class="Keyword">import</a> <a id="21796" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21830" class="Keyword">open</a> <a id="21835" class="Keyword">import</a> <a id="21842" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21877" class="Keyword">open</a> <a id="21882" class="Keyword">import</a> <a id="21889" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="21913" class="Keyword">open</a> <a id="21918" class="Keyword">import</a> <a id="21925" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21962" class="Keyword">open</a> <a id="21967" class="Keyword">import</a> <a id="21974" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22001" class="Keyword">open</a> <a id="22006" class="Keyword">import</a> <a id="22013" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22041" class="Keyword">open</a> <a id="22046" class="Keyword">import</a> <a id="22053" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22102" class="Keyword">open</a> <a id="22107" class="Keyword">import</a> <a id="22114" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22160" class="Keyword">open</a> <a id="22165" class="Keyword">import</a> <a id="22172" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22212" class="Keyword">open</a> <a id="22217" class="Keyword">import</a> <a id="22224" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22262" class="Keyword">open</a> <a id="22267" class="Keyword">import</a> <a id="22274" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22303" class="Keyword">open</a> <a id="22308" class="Keyword">import</a> <a id="22315" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22345" class="Keyword">open</a> <a id="22350" class="Keyword">import</a> <a id="22357" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22388" class="Keyword">open</a> <a id="22393" class="Keyword">import</a> <a id="22400" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="22440" class="Keyword">open</a> <a id="22445" class="Keyword">import</a> <a id="22452" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22478" class="Keyword">open</a> <a id="22483" class="Keyword">import</a> <a id="22490" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="22545" class="Keyword">open</a> <a id="22550" class="Keyword">import</a> <a id="22557" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="22608" class="Keyword">open</a> <a id="22613" class="Keyword">import</a> <a id="22620" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="22665" class="Keyword">open</a> <a id="22670" class="Keyword">import</a> <a id="22677" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="22722" class="Keyword">open</a> <a id="22727" class="Keyword">import</a> <a id="22734" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22788" class="Keyword">open</a> <a id="22793" class="Keyword">import</a> <a id="22800" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22827" class="Keyword">open</a> <a id="22832" class="Keyword">import</a> <a id="22839" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22872" class="Keyword">open</a> <a id="22877" class="Keyword">import</a> <a id="22884" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22915" class="Keyword">open</a> <a id="22920" class="Keyword">import</a> <a id="22927" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22964" class="Keyword">open</a> <a id="22969" class="Keyword">import</a> <a id="22976" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23010" class="Keyword">open</a> <a id="23015" class="Keyword">import</a> <a id="23022" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23047" class="Keyword">open</a> <a id="23052" class="Keyword">import</a> <a id="23059" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23091" class="Keyword">open</a> <a id="23096" class="Keyword">import</a> <a id="23103" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23138" class="Keyword">open</a> <a id="23143" class="Keyword">import</a> <a id="23150" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23179" class="Keyword">open</a> <a id="23184" class="Keyword">import</a> <a id="23191" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23217" class="Keyword">open</a> <a id="23222" class="Keyword">import</a> <a id="23229" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23257" class="Keyword">open</a> <a id="23262" class="Keyword">import</a> <a id="23269" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23294" class="Keyword">open</a> <a id="23299" class="Keyword">import</a> <a id="23306" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23327" class="Keyword">open</a> <a id="23332" class="Keyword">import</a> <a id="23339" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23375" class="Keyword">open</a> <a id="23380" class="Keyword">import</a> <a id="23387" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="23430" class="Keyword">open</a> <a id="23435" class="Keyword">import</a> <a id="23442" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23467" class="Keyword">open</a> <a id="23472" class="Keyword">import</a> <a id="23479" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23510" class="Keyword">open</a> <a id="23515" class="Keyword">import</a> <a id="23522" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="23554" class="Keyword">open</a> <a id="23559" class="Keyword">import</a> <a id="23566" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="23600" class="Keyword">open</a> <a id="23605" class="Keyword">import</a> <a id="23612" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="23668" class="Keyword">open</a> <a id="23673" class="Keyword">import</a> <a id="23680" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="23733" class="Keyword">open</a> <a id="23738" class="Keyword">import</a> <a id="23745" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="23772" class="Keyword">open</a> <a id="23777" class="Keyword">import</a> <a id="23784" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23829" class="Keyword">open</a> <a id="23834" class="Keyword">import</a> <a id="23841" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23903" class="Keyword">open</a> <a id="23908" class="Keyword">import</a> <a id="23915" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23928" class="Keyword">open</a> <a id="23933" class="Keyword">import</a> <a id="23940" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23980" class="Keyword">open</a> <a id="23985" class="Keyword">import</a> <a id="23992" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24036" class="Keyword">open</a> <a id="24041" class="Keyword">import</a> <a id="24048" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24087" class="Keyword">open</a> <a id="24092" class="Keyword">import</a> <a id="24099" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24141" class="Keyword">open</a> <a id="24146" class="Keyword">import</a> <a id="24153" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24193" class="Keyword">open</a> <a id="24198" class="Keyword">import</a> <a id="24205" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24246" class="Keyword">open</a> <a id="24251" class="Keyword">import</a> <a id="24258" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24296" class="Keyword">open</a> <a id="24301" class="Keyword">import</a> <a id="24308" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24371" class="Keyword">open</a> <a id="24376" class="Keyword">import</a> <a id="24383" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="24412" class="Keyword">open</a> <a id="24417" class="Keyword">import</a> <a id="24424" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24469" class="Keyword">open</a> <a id="24474" class="Keyword">import</a> <a id="24481" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24523" class="Keyword">open</a> <a id="24528" class="Keyword">import</a> <a id="24535" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="24579" class="Keyword">open</a> <a id="24584" class="Keyword">import</a> <a id="24591" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="24640" class="Keyword">open</a> <a id="24645" class="Keyword">import</a> <a id="24652" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="24702" class="Keyword">open</a> <a id="24707" class="Keyword">import</a> <a id="24714" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="24741" class="Keyword">open</a> <a id="24746" class="Keyword">import</a> <a id="24753" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="24778" class="Keyword">open</a> <a id="24783" class="Keyword">import</a> <a id="24790" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24831" class="Keyword">open</a> <a id="24836" class="Keyword">import</a> <a id="24843" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24866" class="Keyword">open</a> <a id="24871" class="Keyword">import</a> <a id="24878" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24927" class="Keyword">open</a> <a id="24932" class="Keyword">import</a> <a id="24939" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24978" class="Keyword">open</a> <a id="24983" class="Keyword">import</a> <a id="24990" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25031" class="Keyword">open</a> <a id="25036" class="Keyword">import</a> <a id="25043" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25087" class="Keyword">open</a> <a id="25092" class="Keyword">import</a> <a id="25099" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25136" class="Keyword">open</a> <a id="25141" class="Keyword">import</a> <a id="25148" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="25170" class="Keyword">open</a> <a id="25175" class="Keyword">import</a> <a id="25182" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="25212" class="Keyword">open</a> <a id="25217" class="Keyword">import</a> <a id="25224" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="25263" class="Keyword">open</a> <a id="25268" class="Keyword">import</a> <a id="25275" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="25306" class="Keyword">open</a> <a id="25311" class="Keyword">import</a> <a id="25318" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="25344" class="Keyword">open</a> <a id="25349" class="Keyword">import</a> <a id="25356" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25394" class="Keyword">open</a> <a id="25399" class="Keyword">import</a> <a id="25406" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="25464" class="Keyword">open</a> <a id="25469" class="Keyword">import</a> <a id="25476" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="25514" class="Keyword">open</a> <a id="25519" class="Keyword">import</a> <a id="25526" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="25545" class="Keyword">open</a> <a id="25550" class="Keyword">import</a> <a id="25557" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="25622" class="Keyword">open</a> <a id="25627" class="Keyword">import</a> <a id="25634" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="25665" class="Keyword">open</a> <a id="25670" class="Keyword">import</a> <a id="25677" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="25704" class="Keyword">open</a> <a id="25709" class="Keyword">import</a> <a id="25716" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="25744" class="Keyword">open</a> <a id="25749" class="Keyword">import</a> <a id="25756" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="25823" class="Keyword">open</a> <a id="25828" class="Keyword">import</a> <a id="25835" href="group-theory.html" class="Module">group-theory</a>
<a id="25848" class="Keyword">open</a> <a id="25853" class="Keyword">import</a> <a id="25860" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="25888" class="Keyword">open</a> <a id="25893" class="Keyword">import</a> <a id="25900" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25951" class="Keyword">open</a> <a id="25956" class="Keyword">import</a> <a id="25963" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25996" class="Keyword">open</a> <a id="26001" class="Keyword">import</a> <a id="26008" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26055" class="Keyword">open</a> <a id="26060" class="Keyword">import</a> <a id="26067" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26106" class="Keyword">open</a> <a id="26111" class="Keyword">import</a> <a id="26118" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="26158" class="Keyword">open</a> <a id="26163" class="Keyword">import</a> <a id="26170" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="26213" class="Keyword">open</a> <a id="26218" class="Keyword">import</a> <a id="26225" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="26257" class="Keyword">open</a> <a id="26262" class="Keyword">import</a> <a id="26269" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="26305" class="Keyword">open</a> <a id="26310" class="Keyword">import</a> <a id="26317" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="26346" class="Keyword">open</a> <a id="26351" class="Keyword">import</a> <a id="26358" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="26386" class="Keyword">open</a> <a id="26391" class="Keyword">import</a> <a id="26398" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="26431" class="Keyword">open</a> <a id="26436" class="Keyword">import</a> <a id="26443" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="26479" class="Keyword">open</a> <a id="26484" class="Keyword">import</a> <a id="26491" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="26520" class="Keyword">open</a> <a id="26525" class="Keyword">import</a> <a id="26532" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="26557" class="Keyword">open</a> <a id="26562" class="Keyword">import</a> <a id="26569" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="26631" class="Keyword">open</a> <a id="26636" class="Keyword">import</a> <a id="26643" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="26684" class="Keyword">open</a> <a id="26689" class="Keyword">import</a> <a id="26696" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="26725" class="Keyword">open</a> <a id="26730" class="Keyword">import</a> <a id="26737" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="26761" class="Keyword">open</a> <a id="26766" class="Keyword">import</a> <a id="26773" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="26804" class="Keyword">open</a> <a id="26809" class="Keyword">import</a> <a id="26816" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="26863" class="Keyword">open</a> <a id="26868" class="Keyword">import</a> <a id="26875" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="26908" class="Keyword">open</a> <a id="26913" class="Keyword">import</a> <a id="26920" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="26969" class="Keyword">open</a> <a id="26974" class="Keyword">import</a> <a id="26981" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="27021" class="Keyword">open</a> <a id="27026" class="Keyword">import</a> <a id="27033" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="27070" class="Keyword">open</a> <a id="27075" class="Keyword">import</a> <a id="27082" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="27129" class="Keyword">open</a> <a id="27134" class="Keyword">import</a> <a id="27141" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="27182" class="Keyword">open</a> <a id="27187" class="Keyword">import</a> <a id="27194" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="27233" class="Keyword">open</a> <a id="27238" class="Keyword">import</a> <a id="27245" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="27277" class="Keyword">open</a> <a id="27282" class="Keyword">import</a> <a id="27289" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="27316" class="Keyword">open</a> <a id="27321" class="Keyword">import</a> <a id="27328" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="27348" class="Keyword">open</a> <a id="27353" class="Keyword">import</a> <a id="27360" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="27394" class="Keyword">open</a> <a id="27399" class="Keyword">import</a> <a id="27406" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="27433" class="Keyword">open</a> <a id="27438" class="Keyword">import</a> <a id="27445" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="27487" class="Keyword">open</a> <a id="27492" class="Keyword">import</a> <a id="27499" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="27549" class="Keyword">open</a> <a id="27554" class="Keyword">import</a> <a id="27561" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="27608" class="Keyword">open</a> <a id="27613" class="Keyword">import</a> <a id="27620" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="27661" class="Keyword">open</a> <a id="27666" class="Keyword">import</a> <a id="27673" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="27707" class="Keyword">open</a> <a id="27712" class="Keyword">import</a> <a id="27719" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="27760" class="Keyword">open</a> <a id="27765" class="Keyword">import</a> <a id="27772" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="27807" class="Keyword">open</a> <a id="27812" class="Keyword">import</a> <a id="27819" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="27857" class="Keyword">open</a> <a id="27862" class="Keyword">import</a> <a id="27869" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="27904" class="Keyword">open</a> <a id="27909" class="Keyword">import</a> <a id="27916" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="27948" class="Keyword">open</a> <a id="27953" class="Keyword">import</a> <a id="27960" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="28001" class="Keyword">open</a> <a id="28006" class="Keyword">import</a> <a id="28013" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="28054" class="Keyword">open</a> <a id="28059" class="Keyword">import</a> <a id="28066" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="28106" class="Keyword">open</a> <a id="28111" class="Keyword">import</a> <a id="28118" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="28151" class="Keyword">open</a> <a id="28156" class="Keyword">import</a> <a id="28163" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="28200" class="Keyword">open</a> <a id="28205" class="Keyword">import</a> <a id="28212" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="28242" class="Keyword">open</a> <a id="28247" class="Keyword">import</a> <a id="28254" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="28275" class="Keyword">open</a> <a id="28280" class="Keyword">import</a> <a id="28287" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="28341" class="Keyword">open</a> <a id="28346" class="Keyword">import</a> <a id="28353" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="28398" class="Keyword">open</a> <a id="28403" class="Keyword">import</a> <a id="28410" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="28438" class="Keyword">open</a> <a id="28443" class="Keyword">import</a> <a id="28450" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="28471" class="Keyword">open</a> <a id="28476" class="Keyword">import</a> <a id="28483" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="28526" class="Keyword">open</a> <a id="28531" class="Keyword">import</a> <a id="28538" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="28572" class="Keyword">open</a> <a id="28577" class="Keyword">import</a> <a id="28584" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="28614" class="Keyword">open</a> <a id="28619" class="Keyword">import</a> <a id="28626" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="28672" class="Keyword">open</a> <a id="28677" class="Keyword">import</a> <a id="28684" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="28738" class="Keyword">open</a> <a id="28743" class="Keyword">import</a> <a id="28750" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="28793" class="Keyword">open</a> <a id="28798" class="Keyword">import</a> <a id="28805" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="28839" class="Keyword">open</a> <a id="28844" class="Keyword">import</a> <a id="28851" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="28892" class="Keyword">open</a> <a id="28897" class="Keyword">import</a> <a id="28904" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="28939" class="Keyword">open</a> <a id="28944" class="Keyword">import</a> <a id="28951" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="28993" class="Keyword">open</a> <a id="28998" class="Keyword">import</a> <a id="29005" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="29040" class="Keyword">open</a> <a id="29045" class="Keyword">import</a> <a id="29052" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="29091" class="Keyword">open</a> <a id="29096" class="Keyword">import</a> <a id="29103" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="29140" class="Keyword">open</a> <a id="29145" class="Keyword">import</a> <a id="29152" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="29199" class="Keyword">open</a> <a id="29204" class="Keyword">import</a> <a id="29211" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="29275" class="Keyword">open</a> <a id="29280" class="Keyword">import</a> <a id="29287" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="29332" class="Keyword">open</a> <a id="29337" class="Keyword">import</a> <a id="29344" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="29368" class="Keyword">open</a> <a id="29373" class="Keyword">import</a> <a id="29380" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="29405" class="Keyword">open</a> <a id="29410" class="Keyword">import</a> <a id="29417" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="29460" class="Keyword">open</a> <a id="29465" class="Keyword">import</a> <a id="29472" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="29503" class="Keyword">open</a> <a id="29508" class="Keyword">import</a> <a id="29515" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="29569" class="Keyword">open</a> <a id="29574" class="Keyword">import</a> <a id="29581" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="29604" class="Keyword">open</a> <a id="29609" class="Keyword">import</a> <a id="29616" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="29654" class="Keyword">open</a> <a id="29659" class="Keyword">import</a> <a id="29666" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="29705" class="Keyword">open</a> <a id="29710" class="Keyword">import</a> <a id="29717" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="29768" class="Keyword">open</a> <a id="29773" class="Keyword">import</a> <a id="29780" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="29817" class="Keyword">open</a> <a id="29822" class="Keyword">import</a> <a id="29829" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="29886" class="Keyword">open</a> <a id="29891" class="Keyword">import</a> <a id="29898" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="29946" class="Keyword">open</a> <a id="29951" class="Keyword">import</a> <a id="29958" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="29988" class="Keyword">open</a> <a id="29993" class="Keyword">import</a> <a id="30000" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="30037" class="Keyword">open</a> <a id="30042" class="Keyword">import</a> <a id="30049" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="30070" class="Keyword">open</a> <a id="30075" class="Keyword">import</a> <a id="30082" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="30129" class="Keyword">open</a> <a id="30134" class="Keyword">import</a> <a id="30141" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="30179" class="Keyword">open</a> <a id="30184" class="Keyword">import</a> <a id="30191" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="30285" class="Keyword">open</a> <a id="30290" class="Keyword">import</a> <a id="30297" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="30312" class="Keyword">open</a> <a id="30317" class="Keyword">import</a> <a id="30324" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="30357" class="Keyword">open</a> <a id="30362" class="Keyword">import</a> <a id="30369" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="30401" class="Keyword">open</a> <a id="30406" class="Keyword">import</a> <a id="30413" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="30455" class="Keyword">open</a> <a id="30460" class="Keyword">import</a> <a id="30467" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="30505" class="Keyword">open</a> <a id="30510" class="Keyword">import</a> <a id="30517" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="30554" class="Keyword">open</a> <a id="30559" class="Keyword">import</a> <a id="30566" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="30599" class="Keyword">open</a> <a id="30604" class="Keyword">import</a> <a id="30611" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="30635" class="Keyword">open</a> <a id="30640" class="Keyword">import</a> <a id="30647" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="30686" class="Keyword">open</a> <a id="30691" class="Keyword">import</a> <a id="30698" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="30744" class="Keyword">open</a> <a id="30749" class="Keyword">import</a> <a id="30756" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="30801" class="Keyword">open</a> <a id="30806" class="Keyword">import</a> <a id="30813" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="30851" class="Keyword">open</a> <a id="30856" class="Keyword">import</a> <a id="30863" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="30895" class="Keyword">open</a> <a id="30900" class="Keyword">import</a> <a id="30907" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="30960" class="Keyword">open</a> <a id="30965" class="Keyword">import</a> <a id="30972" href="order-theory.html" class="Module">order-theory</a>
<a id="30985" class="Keyword">open</a> <a id="30990" class="Keyword">import</a> <a id="30997" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="31024" class="Keyword">open</a> <a id="31029" class="Keyword">import</a> <a id="31036" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="31066" class="Keyword">open</a> <a id="31071" class="Keyword">import</a> <a id="31078" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="31111" class="Keyword">open</a> <a id="31116" class="Keyword">import</a> <a id="31123" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="31159" class="Keyword">open</a> <a id="31164" class="Keyword">import</a> <a id="31171" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="31206" class="Keyword">open</a> <a id="31211" class="Keyword">import</a> <a id="31218" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="31245" class="Keyword">open</a> <a id="31250" class="Keyword">import</a> <a id="31257" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="31287" class="Keyword">open</a> <a id="31292" class="Keyword">import</a> <a id="31299" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="31335" class="Keyword">open</a> <a id="31340" class="Keyword">import</a> <a id="31347" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="31389" class="Keyword">open</a> <a id="31394" class="Keyword">import</a> <a id="31401" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="31431" class="Keyword">open</a> <a id="31436" class="Keyword">import</a> <a id="31443" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="31475" class="Keyword">open</a> <a id="31480" class="Keyword">import</a> <a id="31487" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="31518" class="Keyword">open</a> <a id="31523" class="Keyword">import</a> <a id="31530" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="31556" class="Keyword">open</a> <a id="31561" class="Keyword">import</a> <a id="31568" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="31597" class="Keyword">open</a> <a id="31602" class="Keyword">import</a> <a id="31609" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="31646" class="Keyword">open</a> <a id="31651" class="Keyword">import</a> <a id="31658" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="31698" class="Keyword">open</a> <a id="31703" class="Keyword">import</a> <a id="31710" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="31732" class="Keyword">open</a> <a id="31737" class="Keyword">import</a> <a id="31744" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="31779" class="Keyword">open</a> <a id="31784" class="Keyword">import</a> <a id="31791" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="31829" class="Keyword">open</a> <a id="31834" class="Keyword">import</a> <a id="31841" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="31880" class="Keyword">open</a> <a id="31885" class="Keyword">import</a> <a id="31892" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="31927" class="Keyword">open</a> <a id="31932" class="Keyword">import</a> <a id="31939" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="31974" class="Keyword">open</a> <a id="31979" class="Keyword">import</a> <a id="31986" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="32021" class="Keyword">open</a> <a id="32026" class="Keyword">import</a> <a id="32033" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="32071" class="Keyword">open</a> <a id="32076" class="Keyword">import</a> <a id="32083" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="32114" class="Keyword">open</a> <a id="32119" class="Keyword">import</a> <a id="32126" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="32168" class="Keyword">open</a> <a id="32173" class="Keyword">import</a> <a id="32180" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="32225" class="Keyword">open</a> <a id="32230" class="Keyword">import</a> <a id="32237" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="32270" class="Keyword">open</a> <a id="32275" class="Keyword">import</a> <a id="32282" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="32302" class="Keyword">open</a> <a id="32307" class="Keyword">import</a> <a id="32314" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="32337" class="Keyword">open</a> <a id="32342" class="Keyword">import</a> <a id="32349" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="32372" class="Keyword">open</a> <a id="32377" class="Keyword">import</a> <a id="32384" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="32410" class="Keyword">open</a> <a id="32415" class="Keyword">import</a> <a id="32422" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="32448" class="Keyword">open</a> <a id="32453" class="Keyword">import</a> <a id="32460" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="32524" class="Keyword">open</a> <a id="32529" class="Keyword">import</a> <a id="32536" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="32554" class="Keyword">open</a> <a id="32559" class="Keyword">import</a> <a id="32566" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="32593" class="Keyword">open</a> <a id="32598" class="Keyword">import</a> <a id="32605" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="32631" class="Keyword">open</a> <a id="32636" class="Keyword">import</a> <a id="32643" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="32669" class="Keyword">open</a> <a id="32674" class="Keyword">import</a> <a id="32681" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="32707" class="Keyword">open</a> <a id="32712" class="Keyword">import</a> <a id="32719" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="32750" class="Keyword">open</a> <a id="32755" class="Keyword">import</a> <a id="32762" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="32825" class="Keyword">open</a> <a id="32830" class="Keyword">import</a> <a id="32837" href="polytopes.html" class="Module">polytopes</a>
<a id="32847" class="Keyword">open</a> <a id="32852" class="Keyword">import</a> <a id="32859" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="32917" class="Keyword">open</a> <a id="32922" class="Keyword">import</a> <a id="32929" href="ring-theory.html" class="Module">ring-theory</a>
<a id="32941" class="Keyword">open</a> <a id="32946" class="Keyword">import</a> <a id="32953" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="32990" class="Keyword">open</a> <a id="32995" class="Keyword">import</a> <a id="33002" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="33029" class="Keyword">open</a> <a id="33034" class="Keyword">import</a> <a id="33041" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="33073" class="Keyword">open</a> <a id="33078" class="Keyword">import</a> <a id="33085" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="33131" class="Keyword">open</a> <a id="33136" class="Keyword">import</a> <a id="33143" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="33168" class="Keyword">open</a> <a id="33173" class="Keyword">import</a> <a id="33180" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="33223" class="Keyword">open</a> <a id="33228" class="Keyword">import</a> <a id="33235" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="33273" class="Keyword">open</a> <a id="33278" class="Keyword">import</a> <a id="33285" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="33316" class="Keyword">open</a> <a id="33321" class="Keyword">import</a> <a id="33328" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="33352" class="Keyword">open</a> <a id="33357" class="Keyword">import</a> <a id="33364" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="33396" class="Keyword">open</a> <a id="33401" class="Keyword">import</a> <a id="33408" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="33434" class="Keyword">open</a> <a id="33439" class="Keyword">import</a> <a id="33446" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="33475" class="Keyword">open</a> <a id="33480" class="Keyword">import</a> <a id="33487" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="33524" class="Keyword">open</a> <a id="33529" class="Keyword">import</a> <a id="33536" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="33565" class="Keyword">open</a> <a id="33570" class="Keyword">import</a> <a id="33577" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="33604" class="Keyword">open</a> <a id="33609" class="Keyword">import</a> <a id="33616" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="33653" class="Keyword">open</a> <a id="33658" class="Keyword">import</a> <a id="33665" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="33692" class="Keyword">open</a> <a id="33697" class="Keyword">import</a> <a id="33704" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="33737" class="Keyword">open</a> <a id="33742" class="Keyword">import</a> <a id="33749" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="33767" class="Keyword">open</a> <a id="33772" class="Keyword">import</a> <a id="33779" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="33833" class="Keyword">open</a> <a id="33838" class="Keyword">import</a> <a id="33845" href="set-theory.html" class="Module">set-theory</a>
<a id="33856" class="Keyword">open</a> <a id="33861" class="Keyword">import</a> <a id="33868" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="33891" class="Keyword">open</a> <a id="33896" class="Keyword">import</a> <a id="33903" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="33927" class="Keyword">open</a> <a id="33932" class="Keyword">import</a> <a id="33939" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="33965" class="Keyword">open</a> <a id="33970" class="Keyword">import</a> <a id="33977" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="34039" class="Keyword">open</a> <a id="34044" class="Keyword">import</a> <a id="34051" href="structured-types.html" class="Module">structured-types</a>
<a id="34068" class="Keyword">open</a> <a id="34073" class="Keyword">import</a> <a id="34080" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="34115" class="Keyword">open</a> <a id="34120" class="Keyword">import</a> <a id="34127" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="34171" class="Keyword">open</a> <a id="34176" class="Keyword">import</a> <a id="34183" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="34247" class="Keyword">open</a> <a id="34252" class="Keyword">import</a> <a id="34259" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="34298" class="Keyword">open</a> <a id="34303" class="Keyword">import</a> <a id="34310" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="34356" class="Keyword">open</a> <a id="34361" class="Keyword">import</a> <a id="34368" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="34392" class="Keyword">open</a> <a id="34397" class="Keyword">import</a> <a id="34404" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="34473" class="Keyword">open</a> <a id="34478" class="Keyword">import</a> <a id="34485" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="34530" class="Keyword">open</a> <a id="34535" class="Keyword">import</a> <a id="34542" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="34576" class="Keyword">open</a> <a id="34581" class="Keyword">import</a> <a id="34588" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="34649" class="Keyword">open</a> <a id="34654" class="Keyword">import</a> <a id="34661" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="34706" class="Keyword">open</a> <a id="34711" class="Keyword">import</a> <a id="34718" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="34756" class="Keyword">open</a> <a id="34761" class="Keyword">import</a> <a id="34768" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="34811" class="Keyword">open</a> <a id="34816" class="Keyword">import</a> <a id="34823" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="34859" class="Keyword">open</a> <a id="34864" class="Keyword">import</a> <a id="34871" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="34901" class="Keyword">open</a> <a id="34906" class="Keyword">import</a> <a id="34913" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="34944" class="Keyword">open</a> <a id="34949" class="Keyword">import</a> <a id="34956" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="35015" class="Keyword">open</a> <a id="35020" class="Keyword">import</a> <a id="35027" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="35078" class="Keyword">open</a> <a id="35083" class="Keyword">import</a> <a id="35090" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="35141" class="Keyword">open</a> <a id="35146" class="Keyword">import</a> <a id="35153" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="35208" class="Keyword">open</a> <a id="35213" class="Keyword">import</a> <a id="35220" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="35249" class="Keyword">open</a> <a id="35254" class="Keyword">import</a> <a id="35261" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="35289" class="Keyword">open</a> <a id="35294" class="Keyword">import</a> <a id="35301" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="35331" class="Keyword">open</a> <a id="35336" class="Keyword">import</a> <a id="35343" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="35377" class="Keyword">open</a> <a id="35382" class="Keyword">import</a> <a id="35389" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="35465" class="Keyword">open</a> <a id="35470" class="Keyword">import</a> <a id="35477" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="35503" class="Keyword">open</a> <a id="35508" class="Keyword">import</a> <a id="35515" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="35553" class="Keyword">open</a> <a id="35558" class="Keyword">import</a> <a id="35565" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="35602" class="Keyword">open</a> <a id="35607" class="Keyword">import</a> <a id="35614" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="35654" class="Keyword">open</a> <a id="35659" class="Keyword">import</a> <a id="35666" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="35705" class="Keyword">open</a> <a id="35710" class="Keyword">import</a> <a id="35717" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="35750" class="Keyword">open</a> <a id="35755" class="Keyword">import</a> <a id="35762" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="35805" class="Keyword">open</a> <a id="35810" class="Keyword">import</a> <a id="35817" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="35852" class="Keyword">open</a> <a id="35857" class="Keyword">import</a> <a id="35864" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="35909" class="Keyword">open</a> <a id="35914" class="Keyword">import</a> <a id="35921" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="35958" class="Keyword">open</a> <a id="35963" class="Keyword">import</a> <a id="35970" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="36022" class="Keyword">open</a> <a id="36027" class="Keyword">import</a> <a id="36034" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="36087" class="Keyword">open</a> <a id="36092" class="Keyword">import</a> <a id="36099" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="36159" class="Keyword">open</a> <a id="36164" class="Keyword">import</a> <a id="36171" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="36219" class="Keyword">open</a> <a id="36224" class="Keyword">import</a> <a id="36231" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="36271" class="Keyword">open</a> <a id="36276" class="Keyword">import</a> <a id="36283" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="36330" class="Keyword">open</a> <a id="36335" class="Keyword">import</a> <a id="36342" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="36383" class="Keyword">open</a> <a id="36388" class="Keyword">import</a> <a id="36395" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="36433" class="Keyword">open</a> <a id="36438" class="Keyword">import</a> <a id="36445" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="36493" class="Keyword">open</a> <a id="36498" class="Keyword">import</a> <a id="36505" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="36542" class="Keyword">open</a> <a id="36547" class="Keyword">import</a> <a id="36554" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="36589" class="Keyword">open</a> <a id="36594" class="Keyword">import</a> <a id="36601" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="36635" class="Keyword">open</a> <a id="36640" class="Keyword">import</a> <a id="36647" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="36694" class="Keyword">open</a> <a id="36699" class="Keyword">import</a> <a id="36706" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="36751" class="Keyword">open</a> <a id="36756" class="Keyword">import</a> <a id="36763" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="36812" class="Keyword">open</a> <a id="36817" class="Keyword">import</a> <a id="36824" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="36876" class="Keyword">open</a> <a id="36881" class="Keyword">import</a> <a id="36888" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="36942" class="Keyword">open</a> <a id="36947" class="Keyword">import</a> <a id="36954" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="37031" class="Keyword">open</a> <a id="37036" class="Keyword">import</a> <a id="37043" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="37095" class="Keyword">open</a> <a id="37100" class="Keyword">import</a> <a id="37107" href="type-theories.html" class="Module">type-theories</a>
<a id="37121" class="Keyword">open</a> <a id="37126" class="Keyword">import</a> <a id="37133" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="37175" class="Keyword">open</a> <a id="37180" class="Keyword">import</a> <a id="37187" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="37225" class="Keyword">open</a> <a id="37230" class="Keyword">import</a> <a id="37237" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="37283" class="Keyword">open</a> <a id="37288" class="Keyword">import</a> <a id="37295" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="37342" class="Keyword">open</a> <a id="37347" class="Keyword">import</a> <a id="37354" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="37389" class="Keyword">open</a> <a id="37394" class="Keyword">import</a> <a id="37401" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="37479" class="Keyword">open</a> <a id="37484" class="Keyword">import</a> <a id="37491" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="37515" class="Keyword">open</a> <a id="37520" class="Keyword">import</a> <a id="37527" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="37580" class="Keyword">open</a> <a id="37585" class="Keyword">import</a> <a id="37592" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="37635" class="Keyword">open</a> <a id="37640" class="Keyword">import</a> <a id="37647" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="37687" class="Keyword">open</a> <a id="37692" class="Keyword">import</a> <a id="37699" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="37738" class="Keyword">open</a> <a id="37743" class="Keyword">import</a> <a id="37750" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="37784" class="Keyword">open</a> <a id="37789" class="Keyword">import</a> <a id="37796" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="37844" class="Keyword">open</a> <a id="37849" class="Keyword">import</a> <a id="37856" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="37907" class="Keyword">open</a> <a id="37912" class="Keyword">import</a> <a id="37919" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="37966" class="Keyword">open</a> <a id="37971" class="Keyword">import</a> <a id="37978" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="38030" class="Keyword">open</a> <a id="38035" class="Keyword">import</a> <a id="38042" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="38086" class="Keyword">open</a> <a id="38091" class="Keyword">import</a> <a id="38098" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="38138" class="Keyword">open</a> <a id="38143" class="Keyword">import</a> <a id="38150" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="38193" class="Keyword">open</a> <a id="38198" class="Keyword">import</a> <a id="38205" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="38257" class="Keyword">open</a> <a id="38262" class="Keyword">import</a> <a id="38269" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="38323" class="Keyword">open</a> <a id="38328" class="Keyword">import</a> <a id="38335" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="38383" class="Keyword">open</a> <a id="38388" class="Keyword">import</a> <a id="38395" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="38434" class="Keyword">open</a> <a id="38439" class="Keyword">import</a> <a id="38446" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="38479" class="Keyword">open</a> <a id="38484" class="Keyword">import</a> <a id="38491" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="38521" class="Keyword">open</a> <a id="38526" class="Keyword">import</a> <a id="38533" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="38584" class="Keyword">open</a> <a id="38589" class="Keyword">import</a> <a id="38596" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="38637" class="Keyword">open</a> <a id="38642" class="Keyword">import</a> <a id="38649" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="38686" class="Keyword">open</a> <a id="38691" class="Keyword">import</a> <a id="38698" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="38757" class="Keyword">open</a> <a id="38762" class="Keyword">import</a> <a id="38769" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="38824" class="Keyword">open</a> <a id="38829" class="Keyword">import</a> <a id="38836" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="38892" class="Keyword">open</a> <a id="38897" class="Keyword">import</a> <a id="38904" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="38951" class="Keyword">open</a> <a id="38956" class="Keyword">import</a> <a id="38963" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="39006" class="Keyword">open</a> <a id="39011" class="Keyword">import</a> <a id="39018" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="39063" class="Keyword">open</a> <a id="39068" class="Keyword">import</a> <a id="39075" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="39124" class="Keyword">open</a> <a id="39129" class="Keyword">import</a> <a id="39136" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="39187" class="Keyword">open</a> <a id="39192" class="Keyword">import</a> <a id="39199" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="39243" class="Keyword">open</a> <a id="39248" class="Keyword">import</a> <a id="39255" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="39333" class="Keyword">open</a> <a id="39338" class="Keyword">import</a> <a id="39345" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="39385" class="Keyword">open</a> <a id="39390" class="Keyword">import</a> <a id="39397" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="39454" class="Keyword">open</a> <a id="39459" class="Keyword">import</a> <a id="39466" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="39501" class="Keyword">open</a> <a id="39506" class="Keyword">import</a> <a id="39513" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="39559" class="Keyword">open</a> <a id="39564" class="Keyword">import</a> <a id="39571" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="39626" class="Keyword">open</a> <a id="39631" class="Keyword">import</a> <a id="39638" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="39681" class="Keyword">open</a> <a id="39686" class="Keyword">import</a> <a id="39693" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="39738" class="Keyword">open</a> <a id="39743" class="Keyword">import</a> <a id="39750" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="39809" class="Keyword">open</a> <a id="39814" class="Keyword">import</a> <a id="39821" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="39858" class="Keyword">open</a> <a id="39863" class="Keyword">import</a> <a id="39870" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="39912" class="Keyword">open</a> <a id="39917" class="Keyword">import</a> <a id="39924" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="39965" class="Keyword">open</a> <a id="39970" class="Keyword">import</a> <a id="39977" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="40016" class="Keyword">open</a> <a id="40021" class="Keyword">import</a> <a id="40028" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="40066" class="Keyword">open</a> <a id="40071" class="Keyword">import</a> <a id="40078" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="40130" class="Keyword">open</a> <a id="40135" class="Keyword">import</a> <a id="40142" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="40187" class="Keyword">open</a> <a id="40192" class="Keyword">import</a> <a id="40199" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="40238" class="Keyword">open</a> <a id="40243" class="Keyword">import</a> <a id="40250" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="40287" class="Keyword">open</a> <a id="40292" class="Keyword">import</a> <a id="40299" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="40348" class="Keyword">open</a> <a id="40353" class="Keyword">import</a> <a id="40360" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="40399" class="Keyword">open</a> <a id="40404" class="Keyword">import</a> <a id="40411" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="40449" class="Keyword">open</a> <a id="40454" class="Keyword">import</a> <a id="40461" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="40516" class="Keyword">open</a> <a id="40521" class="Keyword">import</a> <a id="40528" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="40567" class="Keyword">open</a> <a id="40572" class="Keyword">import</a> <a id="40579" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="40627" class="Keyword">open</a> <a id="40632" class="Keyword">import</a> <a id="40639" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="40686" class="Keyword">open</a> <a id="40691" class="Keyword">import</a> <a id="40698" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="40736" class="Keyword">open</a> <a id="40741" class="Keyword">import</a> <a id="40748" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="40778" class="Keyword">open</a> <a id="40783" class="Keyword">import</a> <a id="40790" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="40847" class="Keyword">open</a> <a id="40852" class="Keyword">import</a> <a id="40859" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="40913" class="Keyword">open</a> <a id="40918" class="Keyword">import</a> <a id="40925" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="40955" class="Keyword">open</a> <a id="40960" class="Keyword">import</a> <a id="40967" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="41016" class="Keyword">open</a> <a id="41021" class="Keyword">import</a> <a id="41028" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="41070" class="Keyword">open</a> <a id="41075" class="Keyword">import</a> <a id="41082" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="41116" class="Keyword">open</a> <a id="41121" class="Keyword">import</a> <a id="41128" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="41191" class="Keyword">open</a> <a id="41196" class="Keyword">import</a> <a id="41203" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="41246" class="Keyword">open</a> <a id="41251" class="Keyword">import</a> <a id="41258" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="41293" class="Keyword">open</a> <a id="41298" class="Keyword">import</a> <a id="41305" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="41340" class="Keyword">open</a> <a id="41345" class="Keyword">import</a> <a id="41352" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="41392" class="Keyword">open</a> <a id="41397" class="Keyword">import</a> <a id="41404" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="41449" class="Keyword">open</a> <a id="41454" class="Keyword">import</a> <a id="41461" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="41502" class="Keyword">open</a> <a id="41507" class="Keyword">import</a> <a id="41514" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="41568" class="Keyword">open</a> <a id="41573" class="Keyword">import</a> <a id="41580" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="41630" class="Keyword">open</a> <a id="41635" class="Keyword">import</a> <a id="41642" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="41689" class="Keyword">open</a> <a id="41694" class="Keyword">import</a> <a id="41701" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="41739" class="Keyword">open</a> <a id="41744" class="Keyword">import</a> <a id="41751" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="41800" class="Keyword">open</a> <a id="41805" class="Keyword">import</a> <a id="41812" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="41859" class="Keyword">open</a> <a id="41864" class="Keyword">import</a> <a id="41871" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="41934" class="Keyword">open</a> <a id="41939" class="Keyword">import</a> <a id="41946" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="41978" class="Keyword">open</a> <a id="41983" class="Keyword">import</a> <a id="41990" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="42043" class="Keyword">open</a> <a id="42048" class="Keyword">import</a> <a id="42055" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="42101" class="Keyword">open</a> <a id="42106" class="Keyword">import</a> <a id="42113" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="42159" class="Keyword">open</a> <a id="42164" class="Keyword">import</a> <a id="42171" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="42211" class="Keyword">open</a> <a id="42216" class="Keyword">import</a> <a id="42223" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="42270" class="Keyword">open</a> <a id="42275" class="Keyword">import</a> <a id="42282" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="42330" class="Keyword">open</a> <a id="42335" class="Keyword">import</a> <a id="42342" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="42382" class="Keyword">open</a> <a id="42387" class="Keyword">import</a> <a id="42394" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="42439" class="Keyword">open</a> <a id="42444" class="Keyword">import</a> <a id="42451" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="42516" class="Keyword">open</a> <a id="42521" class="Keyword">import</a> <a id="42528" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="42573" class="Keyword">open</a> <a id="42578" class="Keyword">import</a> <a id="42585" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="42632" class="Keyword">open</a> <a id="42637" class="Keyword">import</a> <a id="42644" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="42697" class="Keyword">open</a> <a id="42702" class="Keyword">import</a> <a id="42709" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>