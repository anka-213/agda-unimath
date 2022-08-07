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
<a id="16571" class="Keyword">open</a> <a id="16576" class="Keyword">import</a> <a id="16583" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16614" class="Keyword">open</a> <a id="16619" class="Keyword">import</a> <a id="16626" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16658" class="Keyword">open</a> <a id="16663" class="Keyword">import</a> <a id="16670" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16701" class="Keyword">open</a> <a id="16706" class="Keyword">import</a> <a id="16713" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16730" class="Keyword">open</a> <a id="16735" class="Keyword">import</a> <a id="16742" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16767" class="Keyword">open</a> <a id="16772" class="Keyword">import</a> <a id="16779" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16808" class="Keyword">open</a> <a id="16813" class="Keyword">import</a> <a id="16820" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16845" class="Keyword">open</a> <a id="16850" class="Keyword">import</a> <a id="16857" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="16886" class="Keyword">open</a> <a id="16891" class="Keyword">import</a> <a id="16898" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16919" class="Keyword">open</a> <a id="16924" class="Keyword">import</a> <a id="16931" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16955" class="Keyword">open</a> <a id="16960" class="Keyword">import</a> <a id="16967" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16987" class="Keyword">open</a> <a id="16992" class="Keyword">import</a> <a id="16999" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="17033" class="Keyword">open</a> <a id="17038" class="Keyword">import</a> <a id="17045" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17083" class="Keyword">open</a> <a id="17088" class="Keyword">import</a> <a id="17095" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17123" class="Keyword">open</a> <a id="17128" class="Keyword">import</a> <a id="17135" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17159" class="Keyword">open</a> <a id="17164" class="Keyword">import</a> <a id="17171" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17198" class="Keyword">open</a> <a id="17203" class="Keyword">import</a> <a id="17210" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17245" class="Keyword">open</a> <a id="17250" class="Keyword">import</a> <a id="17257" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17278" class="Keyword">open</a> <a id="17283" class="Keyword">import</a> <a id="17290" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17326" class="Keyword">open</a> <a id="17331" class="Keyword">import</a> <a id="17338" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17383" class="Keyword">open</a> <a id="17388" class="Keyword">import</a> <a id="17395" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17441" class="Keyword">open</a> <a id="17446" class="Keyword">import</a> <a id="17453" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17493" class="Keyword">open</a> <a id="17498" class="Keyword">import</a> <a id="17505" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17535" class="Keyword">open</a> <a id="17540" class="Keyword">import</a> <a id="17547" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17581" class="Keyword">open</a> <a id="17586" class="Keyword">import</a> <a id="17593" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17630" class="Keyword">open</a> <a id="17635" class="Keyword">import</a> <a id="17642" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17666" class="Keyword">open</a> <a id="17671" class="Keyword">import</a> <a id="17678" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17699" class="Keyword">open</a> <a id="17704" class="Keyword">import</a> <a id="17711" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17746" class="Keyword">open</a> <a id="17751" class="Keyword">import</a> <a id="17758" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17795" class="Keyword">open</a> <a id="17800" class="Keyword">import</a> <a id="17807" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17856" class="Keyword">open</a> <a id="17861" class="Keyword">import</a> <a id="17868" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17901" class="Keyword">open</a> <a id="17906" class="Keyword">import</a> <a id="17913" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17936" class="Keyword">open</a> <a id="17941" class="Keyword">import</a> <a id="17948" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17971" class="Keyword">open</a> <a id="17976" class="Keyword">import</a> <a id="17983" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18006" class="Keyword">open</a> <a id="18011" class="Keyword">import</a> <a id="18018" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18046" class="Keyword">open</a> <a id="18051" class="Keyword">import</a> <a id="18058" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18078" class="Keyword">open</a> <a id="18083" class="Keyword">import</a> <a id="18090" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18111" class="Keyword">open</a> <a id="18116" class="Keyword">import</a> <a id="18123" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18154" class="Keyword">open</a> <a id="18159" class="Keyword">import</a> <a id="18166" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18193" class="Keyword">open</a> <a id="18198" class="Keyword">import</a> <a id="18205" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18221" class="Keyword">open</a> <a id="18226" class="Keyword">import</a> <a id="18233" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18264" class="Keyword">open</a> <a id="18269" class="Keyword">import</a> <a id="18276" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18293" class="Keyword">open</a> <a id="18298" class="Keyword">import</a> <a id="18305" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18327" class="Keyword">open</a> <a id="18332" class="Keyword">import</a> <a id="18339" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18366" class="Keyword">open</a> <a id="18371" class="Keyword">import</a> <a id="18378" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18401" class="Keyword">open</a> <a id="18406" class="Keyword">import</a> <a id="18413" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18440" class="Keyword">open</a> <a id="18445" class="Keyword">import</a> <a id="18452" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18485" class="Keyword">open</a> <a id="18490" class="Keyword">import</a> <a id="18497" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18537" class="Keyword">open</a> <a id="18542" class="Keyword">import</a> <a id="18549" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18570" class="Keyword">open</a> <a id="18575" class="Keyword">import</a> <a id="18582" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18611" class="Keyword">open</a> <a id="18616" class="Keyword">import</a> <a id="18623" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18661" class="Keyword">open</a> <a id="18666" class="Keyword">import</a> <a id="18673" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18693" class="Keyword">open</a> <a id="18698" class="Keyword">import</a> <a id="18705" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18729" class="Keyword">open</a> <a id="18734" class="Keyword">import</a> <a id="18741" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18768" class="Keyword">open</a> <a id="18773" class="Keyword">import</a> <a id="18780" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18812" class="Keyword">open</a> <a id="18817" class="Keyword">import</a> <a id="18824" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18854" class="Keyword">open</a> <a id="18859" class="Keyword">import</a> <a id="18866" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18892" class="Keyword">open</a> <a id="18897" class="Keyword">import</a> <a id="18904" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18931" class="Keyword">open</a> <a id="18936" class="Keyword">import</a> <a id="18943" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="18980" class="Keyword">open</a> <a id="18985" class="Keyword">import</a> <a id="18992" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19021" class="Keyword">open</a> <a id="19026" class="Keyword">import</a> <a id="19033" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19056" class="Keyword">open</a> <a id="19061" class="Keyword">import</a> <a id="19068" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19119" class="Keyword">open</a> <a id="19124" class="Keyword">import</a> <a id="19131" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19174" class="Keyword">open</a> <a id="19179" class="Keyword">import</a> <a id="19186" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19238" class="Keyword">open</a> <a id="19243" class="Keyword">import</a> <a id="19250" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19298" class="Keyword">open</a> <a id="19303" class="Keyword">import</a> <a id="19310" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19348" class="Keyword">open</a> <a id="19353" class="Keyword">import</a> <a id="19360" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19397" class="Keyword">open</a> <a id="19402" class="Keyword">import</a> <a id="19409" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19455" class="Keyword">open</a> <a id="19460" class="Keyword">import</a> <a id="19467" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19484" class="Keyword">open</a> <a id="19489" class="Keyword">import</a> <a id="19496" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19524" class="Keyword">open</a> <a id="19529" class="Keyword">import</a> <a id="19536" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19564" class="Keyword">open</a> <a id="19569" class="Keyword">import</a> <a id="19576" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19612" class="Keyword">open</a> <a id="19617" class="Keyword">import</a> <a id="19624" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19662" class="Keyword">open</a> <a id="19667" class="Keyword">import</a> <a id="19674" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19707" class="Keyword">open</a> <a id="19712" class="Keyword">import</a> <a id="19719" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19740" class="Keyword">open</a> <a id="19745" class="Keyword">import</a> <a id="19752" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19788" class="Keyword">open</a> <a id="19793" class="Keyword">import</a> <a id="19800" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19854" class="Keyword">open</a> <a id="19859" class="Keyword">import</a> <a id="19866" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19888" class="Keyword">open</a> <a id="19893" class="Keyword">import</a> <a id="19900" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19935" class="Keyword">open</a> <a id="19940" class="Keyword">import</a> <a id="19947" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19977" class="Keyword">open</a> <a id="19982" class="Keyword">import</a> <a id="19989" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20028" class="Keyword">open</a> <a id="20033" class="Keyword">import</a> <a id="20040" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20094" class="Keyword">open</a> <a id="20099" class="Keyword">import</a> <a id="20106" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20152" class="Keyword">open</a> <a id="20157" class="Keyword">import</a> <a id="20164" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20215" class="Keyword">open</a> <a id="20220" class="Keyword">import</a> <a id="20227" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20268" class="Keyword">open</a> <a id="20273" class="Keyword">import</a> <a id="20280" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20325" class="Keyword">open</a> <a id="20330" class="Keyword">import</a> <a id="20337" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20382" class="Keyword">open</a> <a id="20387" class="Keyword">import</a> <a id="20394" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20430" class="Keyword">open</a> <a id="20435" class="Keyword">import</a> <a id="20442" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20478" class="Keyword">open</a> <a id="20483" class="Keyword">import</a> <a id="20490" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20555" class="Keyword">open</a> <a id="20560" class="Keyword">import</a> <a id="20567" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20622" class="Keyword">open</a> <a id="20627" class="Keyword">import</a> <a id="20634" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20674" class="Keyword">open</a> <a id="20679" class="Keyword">import</a> <a id="20686" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20730" class="Keyword">open</a> <a id="20735" class="Keyword">import</a> <a id="20742" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20787" class="Keyword">open</a> <a id="20792" class="Keyword">import</a> <a id="20799" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20840" class="Keyword">open</a> <a id="20845" class="Keyword">import</a> <a id="20852" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20892" class="Keyword">open</a> <a id="20897" class="Keyword">import</a> <a id="20904" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20931" class="Keyword">open</a> <a id="20936" class="Keyword">import</a> <a id="20943" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20979" class="Keyword">open</a> <a id="20984" class="Keyword">import</a> <a id="20991" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21018" class="Keyword">open</a> <a id="21023" class="Keyword">import</a> <a id="21030" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21067" class="Keyword">open</a> <a id="21072" class="Keyword">import</a> <a id="21079" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21107" class="Keyword">open</a> <a id="21112" class="Keyword">import</a> <a id="21119" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21138" class="Keyword">open</a> <a id="21143" class="Keyword">import</a> <a id="21150" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21190" class="Keyword">open</a> <a id="21195" class="Keyword">import</a> <a id="21202" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21234" class="Keyword">open</a> <a id="21239" class="Keyword">import</a> <a id="21246" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21294" class="Keyword">open</a> <a id="21299" class="Keyword">import</a> <a id="21306" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21329" class="Keyword">open</a> <a id="21334" class="Keyword">import</a> <a id="21341" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21365" class="Keyword">open</a> <a id="21370" class="Keyword">import</a> <a id="21377" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21417" class="Keyword">open</a> <a id="21422" class="Keyword">import</a> <a id="21429" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="21472" class="Keyword">open</a> <a id="21477" class="Keyword">import</a> <a id="21484" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21518" class="Keyword">open</a> <a id="21523" class="Keyword">import</a> <a id="21530" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21562" class="Keyword">open</a> <a id="21567" class="Keyword">import</a> <a id="21574" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21604" class="Keyword">open</a> <a id="21609" class="Keyword">import</a> <a id="21616" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21650" class="Keyword">open</a> <a id="21655" class="Keyword">import</a> <a id="21662" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21697" class="Keyword">open</a> <a id="21702" class="Keyword">import</a> <a id="21709" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="21733" class="Keyword">open</a> <a id="21738" class="Keyword">import</a> <a id="21745" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21782" class="Keyword">open</a> <a id="21787" class="Keyword">import</a> <a id="21794" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21821" class="Keyword">open</a> <a id="21826" class="Keyword">import</a> <a id="21833" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21861" class="Keyword">open</a> <a id="21866" class="Keyword">import</a> <a id="21873" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21922" class="Keyword">open</a> <a id="21927" class="Keyword">import</a> <a id="21934" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21980" class="Keyword">open</a> <a id="21985" class="Keyword">import</a> <a id="21992" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22032" class="Keyword">open</a> <a id="22037" class="Keyword">import</a> <a id="22044" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22082" class="Keyword">open</a> <a id="22087" class="Keyword">import</a> <a id="22094" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22123" class="Keyword">open</a> <a id="22128" class="Keyword">import</a> <a id="22135" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22165" class="Keyword">open</a> <a id="22170" class="Keyword">import</a> <a id="22177" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22208" class="Keyword">open</a> <a id="22213" class="Keyword">import</a> <a id="22220" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="22260" class="Keyword">open</a> <a id="22265" class="Keyword">import</a> <a id="22272" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22298" class="Keyword">open</a> <a id="22303" class="Keyword">import</a> <a id="22310" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="22365" class="Keyword">open</a> <a id="22370" class="Keyword">import</a> <a id="22377" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="22428" class="Keyword">open</a> <a id="22433" class="Keyword">import</a> <a id="22440" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="22485" class="Keyword">open</a> <a id="22490" class="Keyword">import</a> <a id="22497" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="22542" class="Keyword">open</a> <a id="22547" class="Keyword">import</a> <a id="22554" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22608" class="Keyword">open</a> <a id="22613" class="Keyword">import</a> <a id="22620" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22647" class="Keyword">open</a> <a id="22652" class="Keyword">import</a> <a id="22659" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22692" class="Keyword">open</a> <a id="22697" class="Keyword">import</a> <a id="22704" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22735" class="Keyword">open</a> <a id="22740" class="Keyword">import</a> <a id="22747" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22784" class="Keyword">open</a> <a id="22789" class="Keyword">import</a> <a id="22796" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="22830" class="Keyword">open</a> <a id="22835" class="Keyword">import</a> <a id="22842" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22867" class="Keyword">open</a> <a id="22872" class="Keyword">import</a> <a id="22879" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22911" class="Keyword">open</a> <a id="22916" class="Keyword">import</a> <a id="22923" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22958" class="Keyword">open</a> <a id="22963" class="Keyword">import</a> <a id="22970" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22999" class="Keyword">open</a> <a id="23004" class="Keyword">import</a> <a id="23011" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23037" class="Keyword">open</a> <a id="23042" class="Keyword">import</a> <a id="23049" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23077" class="Keyword">open</a> <a id="23082" class="Keyword">import</a> <a id="23089" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23114" class="Keyword">open</a> <a id="23119" class="Keyword">import</a> <a id="23126" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23147" class="Keyword">open</a> <a id="23152" class="Keyword">import</a> <a id="23159" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23195" class="Keyword">open</a> <a id="23200" class="Keyword">import</a> <a id="23207" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="23250" class="Keyword">open</a> <a id="23255" class="Keyword">import</a> <a id="23262" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23287" class="Keyword">open</a> <a id="23292" class="Keyword">import</a> <a id="23299" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23330" class="Keyword">open</a> <a id="23335" class="Keyword">import</a> <a id="23342" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="23374" class="Keyword">open</a> <a id="23379" class="Keyword">import</a> <a id="23386" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="23420" class="Keyword">open</a> <a id="23425" class="Keyword">import</a> <a id="23432" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="23488" class="Keyword">open</a> <a id="23493" class="Keyword">import</a> <a id="23500" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="23553" class="Keyword">open</a> <a id="23558" class="Keyword">import</a> <a id="23565" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="23592" class="Keyword">open</a> <a id="23597" class="Keyword">import</a> <a id="23604" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23649" class="Keyword">open</a> <a id="23654" class="Keyword">import</a> <a id="23661" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23723" class="Keyword">open</a> <a id="23728" class="Keyword">import</a> <a id="23735" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23748" class="Keyword">open</a> <a id="23753" class="Keyword">import</a> <a id="23760" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23800" class="Keyword">open</a> <a id="23805" class="Keyword">import</a> <a id="23812" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23856" class="Keyword">open</a> <a id="23861" class="Keyword">import</a> <a id="23868" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23907" class="Keyword">open</a> <a id="23912" class="Keyword">import</a> <a id="23919" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23961" class="Keyword">open</a> <a id="23966" class="Keyword">import</a> <a id="23973" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24013" class="Keyword">open</a> <a id="24018" class="Keyword">import</a> <a id="24025" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24066" class="Keyword">open</a> <a id="24071" class="Keyword">import</a> <a id="24078" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24116" class="Keyword">open</a> <a id="24121" class="Keyword">import</a> <a id="24128" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24191" class="Keyword">open</a> <a id="24196" class="Keyword">import</a> <a id="24203" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="24232" class="Keyword">open</a> <a id="24237" class="Keyword">import</a> <a id="24244" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24289" class="Keyword">open</a> <a id="24294" class="Keyword">import</a> <a id="24301" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24343" class="Keyword">open</a> <a id="24348" class="Keyword">import</a> <a id="24355" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="24399" class="Keyword">open</a> <a id="24404" class="Keyword">import</a> <a id="24411" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="24460" class="Keyword">open</a> <a id="24465" class="Keyword">import</a> <a id="24472" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="24522" class="Keyword">open</a> <a id="24527" class="Keyword">import</a> <a id="24534" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="24561" class="Keyword">open</a> <a id="24566" class="Keyword">import</a> <a id="24573" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="24598" class="Keyword">open</a> <a id="24603" class="Keyword">import</a> <a id="24610" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24651" class="Keyword">open</a> <a id="24656" class="Keyword">import</a> <a id="24663" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24686" class="Keyword">open</a> <a id="24691" class="Keyword">import</a> <a id="24698" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24747" class="Keyword">open</a> <a id="24752" class="Keyword">import</a> <a id="24759" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24798" class="Keyword">open</a> <a id="24803" class="Keyword">import</a> <a id="24810" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24851" class="Keyword">open</a> <a id="24856" class="Keyword">import</a> <a id="24863" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24907" class="Keyword">open</a> <a id="24912" class="Keyword">import</a> <a id="24919" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24956" class="Keyword">open</a> <a id="24961" class="Keyword">import</a> <a id="24968" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24990" class="Keyword">open</a> <a id="24995" class="Keyword">import</a> <a id="25002" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="25032" class="Keyword">open</a> <a id="25037" class="Keyword">import</a> <a id="25044" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="25083" class="Keyword">open</a> <a id="25088" class="Keyword">import</a> <a id="25095" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="25121" class="Keyword">open</a> <a id="25126" class="Keyword">import</a> <a id="25133" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25171" class="Keyword">open</a> <a id="25176" class="Keyword">import</a> <a id="25183" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="25241" class="Keyword">open</a> <a id="25246" class="Keyword">import</a> <a id="25253" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="25291" class="Keyword">open</a> <a id="25296" class="Keyword">import</a> <a id="25303" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="25322" class="Keyword">open</a> <a id="25327" class="Keyword">import</a> <a id="25334" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="25399" class="Keyword">open</a> <a id="25404" class="Keyword">import</a> <a id="25411" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="25442" class="Keyword">open</a> <a id="25447" class="Keyword">import</a> <a id="25454" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="25481" class="Keyword">open</a> <a id="25486" class="Keyword">import</a> <a id="25493" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="25521" class="Keyword">open</a> <a id="25526" class="Keyword">import</a> <a id="25533" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="25600" class="Keyword">open</a> <a id="25605" class="Keyword">import</a> <a id="25612" href="group-theory.html" class="Module">group-theory</a>
<a id="25625" class="Keyword">open</a> <a id="25630" class="Keyword">import</a> <a id="25637" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="25665" class="Keyword">open</a> <a id="25670" class="Keyword">import</a> <a id="25677" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25728" class="Keyword">open</a> <a id="25733" class="Keyword">import</a> <a id="25740" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25773" class="Keyword">open</a> <a id="25778" class="Keyword">import</a> <a id="25785" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="25832" class="Keyword">open</a> <a id="25837" class="Keyword">import</a> <a id="25844" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="25883" class="Keyword">open</a> <a id="25888" class="Keyword">import</a> <a id="25895" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25935" class="Keyword">open</a> <a id="25940" class="Keyword">import</a> <a id="25947" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25990" class="Keyword">open</a> <a id="25995" class="Keyword">import</a> <a id="26002" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="26034" class="Keyword">open</a> <a id="26039" class="Keyword">import</a> <a id="26046" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="26082" class="Keyword">open</a> <a id="26087" class="Keyword">import</a> <a id="26094" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="26123" class="Keyword">open</a> <a id="26128" class="Keyword">import</a> <a id="26135" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="26163" class="Keyword">open</a> <a id="26168" class="Keyword">import</a> <a id="26175" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="26208" class="Keyword">open</a> <a id="26213" class="Keyword">import</a> <a id="26220" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="26256" class="Keyword">open</a> <a id="26261" class="Keyword">import</a> <a id="26268" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="26297" class="Keyword">open</a> <a id="26302" class="Keyword">import</a> <a id="26309" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="26334" class="Keyword">open</a> <a id="26339" class="Keyword">import</a> <a id="26346" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="26408" class="Keyword">open</a> <a id="26413" class="Keyword">import</a> <a id="26420" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="26461" class="Keyword">open</a> <a id="26466" class="Keyword">import</a> <a id="26473" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="26502" class="Keyword">open</a> <a id="26507" class="Keyword">import</a> <a id="26514" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="26538" class="Keyword">open</a> <a id="26543" class="Keyword">import</a> <a id="26550" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="26581" class="Keyword">open</a> <a id="26586" class="Keyword">import</a> <a id="26593" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="26640" class="Keyword">open</a> <a id="26645" class="Keyword">import</a> <a id="26652" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="26685" class="Keyword">open</a> <a id="26690" class="Keyword">import</a> <a id="26697" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="26746" class="Keyword">open</a> <a id="26751" class="Keyword">import</a> <a id="26758" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="26798" class="Keyword">open</a> <a id="26803" class="Keyword">import</a> <a id="26810" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="26847" class="Keyword">open</a> <a id="26852" class="Keyword">import</a> <a id="26859" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="26906" class="Keyword">open</a> <a id="26911" class="Keyword">import</a> <a id="26918" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="26959" class="Keyword">open</a> <a id="26964" class="Keyword">import</a> <a id="26971" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="27010" class="Keyword">open</a> <a id="27015" class="Keyword">import</a> <a id="27022" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="27054" class="Keyword">open</a> <a id="27059" class="Keyword">import</a> <a id="27066" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="27093" class="Keyword">open</a> <a id="27098" class="Keyword">import</a> <a id="27105" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="27125" class="Keyword">open</a> <a id="27130" class="Keyword">import</a> <a id="27137" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="27171" class="Keyword">open</a> <a id="27176" class="Keyword">import</a> <a id="27183" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="27210" class="Keyword">open</a> <a id="27215" class="Keyword">import</a> <a id="27222" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="27264" class="Keyword">open</a> <a id="27269" class="Keyword">import</a> <a id="27276" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="27326" class="Keyword">open</a> <a id="27331" class="Keyword">import</a> <a id="27338" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="27385" class="Keyword">open</a> <a id="27390" class="Keyword">import</a> <a id="27397" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="27438" class="Keyword">open</a> <a id="27443" class="Keyword">import</a> <a id="27450" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="27484" class="Keyword">open</a> <a id="27489" class="Keyword">import</a> <a id="27496" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="27537" class="Keyword">open</a> <a id="27542" class="Keyword">import</a> <a id="27549" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="27584" class="Keyword">open</a> <a id="27589" class="Keyword">import</a> <a id="27596" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="27634" class="Keyword">open</a> <a id="27639" class="Keyword">import</a> <a id="27646" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="27681" class="Keyword">open</a> <a id="27686" class="Keyword">import</a> <a id="27693" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="27725" class="Keyword">open</a> <a id="27730" class="Keyword">import</a> <a id="27737" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="27778" class="Keyword">open</a> <a id="27783" class="Keyword">import</a> <a id="27790" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="27831" class="Keyword">open</a> <a id="27836" class="Keyword">import</a> <a id="27843" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="27883" class="Keyword">open</a> <a id="27888" class="Keyword">import</a> <a id="27895" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="27928" class="Keyword">open</a> <a id="27933" class="Keyword">import</a> <a id="27940" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="27977" class="Keyword">open</a> <a id="27982" class="Keyword">import</a> <a id="27989" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="28019" class="Keyword">open</a> <a id="28024" class="Keyword">import</a> <a id="28031" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="28052" class="Keyword">open</a> <a id="28057" class="Keyword">import</a> <a id="28064" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="28118" class="Keyword">open</a> <a id="28123" class="Keyword">import</a> <a id="28130" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="28175" class="Keyword">open</a> <a id="28180" class="Keyword">import</a> <a id="28187" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="28215" class="Keyword">open</a> <a id="28220" class="Keyword">import</a> <a id="28227" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="28248" class="Keyword">open</a> <a id="28253" class="Keyword">import</a> <a id="28260" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="28303" class="Keyword">open</a> <a id="28308" class="Keyword">import</a> <a id="28315" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="28349" class="Keyword">open</a> <a id="28354" class="Keyword">import</a> <a id="28361" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="28391" class="Keyword">open</a> <a id="28396" class="Keyword">import</a> <a id="28403" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="28449" class="Keyword">open</a> <a id="28454" class="Keyword">import</a> <a id="28461" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="28515" class="Keyword">open</a> <a id="28520" class="Keyword">import</a> <a id="28527" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="28570" class="Keyword">open</a> <a id="28575" class="Keyword">import</a> <a id="28582" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="28616" class="Keyword">open</a> <a id="28621" class="Keyword">import</a> <a id="28628" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="28669" class="Keyword">open</a> <a id="28674" class="Keyword">import</a> <a id="28681" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="28716" class="Keyword">open</a> <a id="28721" class="Keyword">import</a> <a id="28728" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="28770" class="Keyword">open</a> <a id="28775" class="Keyword">import</a> <a id="28782" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="28817" class="Keyword">open</a> <a id="28822" class="Keyword">import</a> <a id="28829" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="28868" class="Keyword">open</a> <a id="28873" class="Keyword">import</a> <a id="28880" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="28917" class="Keyword">open</a> <a id="28922" class="Keyword">import</a> <a id="28929" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="28976" class="Keyword">open</a> <a id="28981" class="Keyword">import</a> <a id="28988" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="29052" class="Keyword">open</a> <a id="29057" class="Keyword">import</a> <a id="29064" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="29109" class="Keyword">open</a> <a id="29114" class="Keyword">import</a> <a id="29121" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="29145" class="Keyword">open</a> <a id="29150" class="Keyword">import</a> <a id="29157" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="29182" class="Keyword">open</a> <a id="29187" class="Keyword">import</a> <a id="29194" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="29237" class="Keyword">open</a> <a id="29242" class="Keyword">import</a> <a id="29249" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="29280" class="Keyword">open</a> <a id="29285" class="Keyword">import</a> <a id="29292" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="29346" class="Keyword">open</a> <a id="29351" class="Keyword">import</a> <a id="29358" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="29381" class="Keyword">open</a> <a id="29386" class="Keyword">import</a> <a id="29393" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="29431" class="Keyword">open</a> <a id="29436" class="Keyword">import</a> <a id="29443" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="29482" class="Keyword">open</a> <a id="29487" class="Keyword">import</a> <a id="29494" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="29545" class="Keyword">open</a> <a id="29550" class="Keyword">import</a> <a id="29557" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="29594" class="Keyword">open</a> <a id="29599" class="Keyword">import</a> <a id="29606" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="29663" class="Keyword">open</a> <a id="29668" class="Keyword">import</a> <a id="29675" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="29723" class="Keyword">open</a> <a id="29728" class="Keyword">import</a> <a id="29735" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="29765" class="Keyword">open</a> <a id="29770" class="Keyword">import</a> <a id="29777" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="29814" class="Keyword">open</a> <a id="29819" class="Keyword">import</a> <a id="29826" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="29847" class="Keyword">open</a> <a id="29852" class="Keyword">import</a> <a id="29859" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="29906" class="Keyword">open</a> <a id="29911" class="Keyword">import</a> <a id="29918" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="29956" class="Keyword">open</a> <a id="29961" class="Keyword">import</a> <a id="29968" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="30062" class="Keyword">open</a> <a id="30067" class="Keyword">import</a> <a id="30074" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="30089" class="Keyword">open</a> <a id="30094" class="Keyword">import</a> <a id="30101" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="30134" class="Keyword">open</a> <a id="30139" class="Keyword">import</a> <a id="30146" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="30178" class="Keyword">open</a> <a id="30183" class="Keyword">import</a> <a id="30190" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="30232" class="Keyword">open</a> <a id="30237" class="Keyword">import</a> <a id="30244" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="30282" class="Keyword">open</a> <a id="30287" class="Keyword">import</a> <a id="30294" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="30331" class="Keyword">open</a> <a id="30336" class="Keyword">import</a> <a id="30343" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="30376" class="Keyword">open</a> <a id="30381" class="Keyword">import</a> <a id="30388" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="30412" class="Keyword">open</a> <a id="30417" class="Keyword">import</a> <a id="30424" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="30463" class="Keyword">open</a> <a id="30468" class="Keyword">import</a> <a id="30475" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="30521" class="Keyword">open</a> <a id="30526" class="Keyword">import</a> <a id="30533" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="30578" class="Keyword">open</a> <a id="30583" class="Keyword">import</a> <a id="30590" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="30628" class="Keyword">open</a> <a id="30633" class="Keyword">import</a> <a id="30640" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="30672" class="Keyword">open</a> <a id="30677" class="Keyword">import</a> <a id="30684" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="30737" class="Keyword">open</a> <a id="30742" class="Keyword">import</a> <a id="30749" href="order-theory.html" class="Module">order-theory</a>
<a id="30762" class="Keyword">open</a> <a id="30767" class="Keyword">import</a> <a id="30774" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="30801" class="Keyword">open</a> <a id="30806" class="Keyword">import</a> <a id="30813" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="30843" class="Keyword">open</a> <a id="30848" class="Keyword">import</a> <a id="30855" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="30888" class="Keyword">open</a> <a id="30893" class="Keyword">import</a> <a id="30900" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="30936" class="Keyword">open</a> <a id="30941" class="Keyword">import</a> <a id="30948" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="30983" class="Keyword">open</a> <a id="30988" class="Keyword">import</a> <a id="30995" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="31022" class="Keyword">open</a> <a id="31027" class="Keyword">import</a> <a id="31034" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="31064" class="Keyword">open</a> <a id="31069" class="Keyword">import</a> <a id="31076" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="31112" class="Keyword">open</a> <a id="31117" class="Keyword">import</a> <a id="31124" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="31166" class="Keyword">open</a> <a id="31171" class="Keyword">import</a> <a id="31178" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="31210" class="Keyword">open</a> <a id="31215" class="Keyword">import</a> <a id="31222" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="31253" class="Keyword">open</a> <a id="31258" class="Keyword">import</a> <a id="31265" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="31291" class="Keyword">open</a> <a id="31296" class="Keyword">import</a> <a id="31303" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="31332" class="Keyword">open</a> <a id="31337" class="Keyword">import</a> <a id="31344" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="31381" class="Keyword">open</a> <a id="31386" class="Keyword">import</a> <a id="31393" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="31433" class="Keyword">open</a> <a id="31438" class="Keyword">import</a> <a id="31445" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="31467" class="Keyword">open</a> <a id="31472" class="Keyword">import</a> <a id="31479" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="31514" class="Keyword">open</a> <a id="31519" class="Keyword">import</a> <a id="31526" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="31564" class="Keyword">open</a> <a id="31569" class="Keyword">import</a> <a id="31576" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="31615" class="Keyword">open</a> <a id="31620" class="Keyword">import</a> <a id="31627" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="31662" class="Keyword">open</a> <a id="31667" class="Keyword">import</a> <a id="31674" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="31709" class="Keyword">open</a> <a id="31714" class="Keyword">import</a> <a id="31721" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="31759" class="Keyword">open</a> <a id="31764" class="Keyword">import</a> <a id="31771" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="31802" class="Keyword">open</a> <a id="31807" class="Keyword">import</a> <a id="31814" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="31856" class="Keyword">open</a> <a id="31861" class="Keyword">import</a> <a id="31868" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="31913" class="Keyword">open</a> <a id="31918" class="Keyword">import</a> <a id="31925" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="31958" class="Keyword">open</a> <a id="31963" class="Keyword">import</a> <a id="31970" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="31990" class="Keyword">open</a> <a id="31995" class="Keyword">import</a> <a id="32002" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="32025" class="Keyword">open</a> <a id="32030" class="Keyword">import</a> <a id="32037" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="32060" class="Keyword">open</a> <a id="32065" class="Keyword">import</a> <a id="32072" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="32098" class="Keyword">open</a> <a id="32103" class="Keyword">import</a> <a id="32110" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="32136" class="Keyword">open</a> <a id="32141" class="Keyword">import</a> <a id="32148" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="32212" class="Keyword">open</a> <a id="32217" class="Keyword">import</a> <a id="32224" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="32242" class="Keyword">open</a> <a id="32247" class="Keyword">import</a> <a id="32254" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="32281" class="Keyword">open</a> <a id="32286" class="Keyword">import</a> <a id="32293" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="32319" class="Keyword">open</a> <a id="32324" class="Keyword">import</a> <a id="32331" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="32357" class="Keyword">open</a> <a id="32362" class="Keyword">import</a> <a id="32369" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="32395" class="Keyword">open</a> <a id="32400" class="Keyword">import</a> <a id="32407" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="32438" class="Keyword">open</a> <a id="32443" class="Keyword">import</a> <a id="32450" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="32513" class="Keyword">open</a> <a id="32518" class="Keyword">import</a> <a id="32525" href="polytopes.html" class="Module">polytopes</a>
<a id="32535" class="Keyword">open</a> <a id="32540" class="Keyword">import</a> <a id="32547" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="32605" class="Keyword">open</a> <a id="32610" class="Keyword">import</a> <a id="32617" href="ring-theory.html" class="Module">ring-theory</a>
<a id="32629" class="Keyword">open</a> <a id="32634" class="Keyword">import</a> <a id="32641" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="32678" class="Keyword">open</a> <a id="32683" class="Keyword">import</a> <a id="32690" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="32717" class="Keyword">open</a> <a id="32722" class="Keyword">import</a> <a id="32729" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="32761" class="Keyword">open</a> <a id="32766" class="Keyword">import</a> <a id="32773" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="32819" class="Keyword">open</a> <a id="32824" class="Keyword">import</a> <a id="32831" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="32856" class="Keyword">open</a> <a id="32861" class="Keyword">import</a> <a id="32868" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="32911" class="Keyword">open</a> <a id="32916" class="Keyword">import</a> <a id="32923" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="32961" class="Keyword">open</a> <a id="32966" class="Keyword">import</a> <a id="32973" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="33004" class="Keyword">open</a> <a id="33009" class="Keyword">import</a> <a id="33016" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="33040" class="Keyword">open</a> <a id="33045" class="Keyword">import</a> <a id="33052" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="33084" class="Keyword">open</a> <a id="33089" class="Keyword">import</a> <a id="33096" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="33122" class="Keyword">open</a> <a id="33127" class="Keyword">import</a> <a id="33134" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="33163" class="Keyword">open</a> <a id="33168" class="Keyword">import</a> <a id="33175" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="33212" class="Keyword">open</a> <a id="33217" class="Keyword">import</a> <a id="33224" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="33253" class="Keyword">open</a> <a id="33258" class="Keyword">import</a> <a id="33265" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="33292" class="Keyword">open</a> <a id="33297" class="Keyword">import</a> <a id="33304" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="33341" class="Keyword">open</a> <a id="33346" class="Keyword">import</a> <a id="33353" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="33380" class="Keyword">open</a> <a id="33385" class="Keyword">import</a> <a id="33392" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="33425" class="Keyword">open</a> <a id="33430" class="Keyword">import</a> <a id="33437" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="33455" class="Keyword">open</a> <a id="33460" class="Keyword">import</a> <a id="33467" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="33521" class="Keyword">open</a> <a id="33526" class="Keyword">import</a> <a id="33533" href="set-theory.html" class="Module">set-theory</a>
<a id="33544" class="Keyword">open</a> <a id="33549" class="Keyword">import</a> <a id="33556" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="33579" class="Keyword">open</a> <a id="33584" class="Keyword">import</a> <a id="33591" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="33615" class="Keyword">open</a> <a id="33620" class="Keyword">import</a> <a id="33627" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="33653" class="Keyword">open</a> <a id="33658" class="Keyword">import</a> <a id="33665" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="33727" class="Keyword">open</a> <a id="33732" class="Keyword">import</a> <a id="33739" href="structured-types.html" class="Module">structured-types</a>
<a id="33756" class="Keyword">open</a> <a id="33761" class="Keyword">import</a> <a id="33768" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="33803" class="Keyword">open</a> <a id="33808" class="Keyword">import</a> <a id="33815" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="33859" class="Keyword">open</a> <a id="33864" class="Keyword">import</a> <a id="33871" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="33935" class="Keyword">open</a> <a id="33940" class="Keyword">import</a> <a id="33947" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="33986" class="Keyword">open</a> <a id="33991" class="Keyword">import</a> <a id="33998" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="34044" class="Keyword">open</a> <a id="34049" class="Keyword">import</a> <a id="34056" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="34080" class="Keyword">open</a> <a id="34085" class="Keyword">import</a> <a id="34092" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="34161" class="Keyword">open</a> <a id="34166" class="Keyword">import</a> <a id="34173" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="34218" class="Keyword">open</a> <a id="34223" class="Keyword">import</a> <a id="34230" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="34264" class="Keyword">open</a> <a id="34269" class="Keyword">import</a> <a id="34276" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="34337" class="Keyword">open</a> <a id="34342" class="Keyword">import</a> <a id="34349" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="34394" class="Keyword">open</a> <a id="34399" class="Keyword">import</a> <a id="34406" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="34444" class="Keyword">open</a> <a id="34449" class="Keyword">import</a> <a id="34456" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="34499" class="Keyword">open</a> <a id="34504" class="Keyword">import</a> <a id="34511" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="34547" class="Keyword">open</a> <a id="34552" class="Keyword">import</a> <a id="34559" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="34589" class="Keyword">open</a> <a id="34594" class="Keyword">import</a> <a id="34601" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="34632" class="Keyword">open</a> <a id="34637" class="Keyword">import</a> <a id="34644" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="34703" class="Keyword">open</a> <a id="34708" class="Keyword">import</a> <a id="34715" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="34766" class="Keyword">open</a> <a id="34771" class="Keyword">import</a> <a id="34778" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="34829" class="Keyword">open</a> <a id="34834" class="Keyword">import</a> <a id="34841" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="34896" class="Keyword">open</a> <a id="34901" class="Keyword">import</a> <a id="34908" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="34937" class="Keyword">open</a> <a id="34942" class="Keyword">import</a> <a id="34949" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="34977" class="Keyword">open</a> <a id="34982" class="Keyword">import</a> <a id="34989" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="35019" class="Keyword">open</a> <a id="35024" class="Keyword">import</a> <a id="35031" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="35065" class="Keyword">open</a> <a id="35070" class="Keyword">import</a> <a id="35077" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="35153" class="Keyword">open</a> <a id="35158" class="Keyword">import</a> <a id="35165" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="35191" class="Keyword">open</a> <a id="35196" class="Keyword">import</a> <a id="35203" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="35241" class="Keyword">open</a> <a id="35246" class="Keyword">import</a> <a id="35253" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="35290" class="Keyword">open</a> <a id="35295" class="Keyword">import</a> <a id="35302" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="35342" class="Keyword">open</a> <a id="35347" class="Keyword">import</a> <a id="35354" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="35393" class="Keyword">open</a> <a id="35398" class="Keyword">import</a> <a id="35405" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="35438" class="Keyword">open</a> <a id="35443" class="Keyword">import</a> <a id="35450" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="35493" class="Keyword">open</a> <a id="35498" class="Keyword">import</a> <a id="35505" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="35540" class="Keyword">open</a> <a id="35545" class="Keyword">import</a> <a id="35552" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="35597" class="Keyword">open</a> <a id="35602" class="Keyword">import</a> <a id="35609" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="35646" class="Keyword">open</a> <a id="35651" class="Keyword">import</a> <a id="35658" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="35710" class="Keyword">open</a> <a id="35715" class="Keyword">import</a> <a id="35722" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="35775" class="Keyword">open</a> <a id="35780" class="Keyword">import</a> <a id="35787" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="35847" class="Keyword">open</a> <a id="35852" class="Keyword">import</a> <a id="35859" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="35907" class="Keyword">open</a> <a id="35912" class="Keyword">import</a> <a id="35919" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="35959" class="Keyword">open</a> <a id="35964" class="Keyword">import</a> <a id="35971" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="36018" class="Keyword">open</a> <a id="36023" class="Keyword">import</a> <a id="36030" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="36071" class="Keyword">open</a> <a id="36076" class="Keyword">import</a> <a id="36083" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="36121" class="Keyword">open</a> <a id="36126" class="Keyword">import</a> <a id="36133" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="36181" class="Keyword">open</a> <a id="36186" class="Keyword">import</a> <a id="36193" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="36230" class="Keyword">open</a> <a id="36235" class="Keyword">import</a> <a id="36242" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="36277" class="Keyword">open</a> <a id="36282" class="Keyword">import</a> <a id="36289" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="36323" class="Keyword">open</a> <a id="36328" class="Keyword">import</a> <a id="36335" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="36382" class="Keyword">open</a> <a id="36387" class="Keyword">import</a> <a id="36394" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="36439" class="Keyword">open</a> <a id="36444" class="Keyword">import</a> <a id="36451" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="36500" class="Keyword">open</a> <a id="36505" class="Keyword">import</a> <a id="36512" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="36564" class="Keyword">open</a> <a id="36569" class="Keyword">import</a> <a id="36576" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="36630" class="Keyword">open</a> <a id="36635" class="Keyword">import</a> <a id="36642" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="36719" class="Keyword">open</a> <a id="36724" class="Keyword">import</a> <a id="36731" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="36783" class="Keyword">open</a> <a id="36788" class="Keyword">import</a> <a id="36795" href="type-theories.html" class="Module">type-theories</a>
<a id="36809" class="Keyword">open</a> <a id="36814" class="Keyword">import</a> <a id="36821" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="36863" class="Keyword">open</a> <a id="36868" class="Keyword">import</a> <a id="36875" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="36913" class="Keyword">open</a> <a id="36918" class="Keyword">import</a> <a id="36925" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="36971" class="Keyword">open</a> <a id="36976" class="Keyword">import</a> <a id="36983" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="37030" class="Keyword">open</a> <a id="37035" class="Keyword">import</a> <a id="37042" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="37077" class="Keyword">open</a> <a id="37082" class="Keyword">import</a> <a id="37089" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="37167" class="Keyword">open</a> <a id="37172" class="Keyword">import</a> <a id="37179" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="37203" class="Keyword">open</a> <a id="37208" class="Keyword">import</a> <a id="37215" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="37268" class="Keyword">open</a> <a id="37273" class="Keyword">import</a> <a id="37280" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="37323" class="Keyword">open</a> <a id="37328" class="Keyword">import</a> <a id="37335" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="37375" class="Keyword">open</a> <a id="37380" class="Keyword">import</a> <a id="37387" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="37426" class="Keyword">open</a> <a id="37431" class="Keyword">import</a> <a id="37438" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="37472" class="Keyword">open</a> <a id="37477" class="Keyword">import</a> <a id="37484" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="37532" class="Keyword">open</a> <a id="37537" class="Keyword">import</a> <a id="37544" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="37595" class="Keyword">open</a> <a id="37600" class="Keyword">import</a> <a id="37607" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="37654" class="Keyword">open</a> <a id="37659" class="Keyword">import</a> <a id="37666" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="37718" class="Keyword">open</a> <a id="37723" class="Keyword">import</a> <a id="37730" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="37774" class="Keyword">open</a> <a id="37779" class="Keyword">import</a> <a id="37786" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="37826" class="Keyword">open</a> <a id="37831" class="Keyword">import</a> <a id="37838" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="37881" class="Keyword">open</a> <a id="37886" class="Keyword">import</a> <a id="37893" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="37945" class="Keyword">open</a> <a id="37950" class="Keyword">import</a> <a id="37957" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="38011" class="Keyword">open</a> <a id="38016" class="Keyword">import</a> <a id="38023" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="38071" class="Keyword">open</a> <a id="38076" class="Keyword">import</a> <a id="38083" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="38122" class="Keyword">open</a> <a id="38127" class="Keyword">import</a> <a id="38134" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="38167" class="Keyword">open</a> <a id="38172" class="Keyword">import</a> <a id="38179" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="38209" class="Keyword">open</a> <a id="38214" class="Keyword">import</a> <a id="38221" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="38272" class="Keyword">open</a> <a id="38277" class="Keyword">import</a> <a id="38284" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="38325" class="Keyword">open</a> <a id="38330" class="Keyword">import</a> <a id="38337" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="38374" class="Keyword">open</a> <a id="38379" class="Keyword">import</a> <a id="38386" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="38445" class="Keyword">open</a> <a id="38450" class="Keyword">import</a> <a id="38457" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="38512" class="Keyword">open</a> <a id="38517" class="Keyword">import</a> <a id="38524" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="38580" class="Keyword">open</a> <a id="38585" class="Keyword">import</a> <a id="38592" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="38639" class="Keyword">open</a> <a id="38644" class="Keyword">import</a> <a id="38651" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="38694" class="Keyword">open</a> <a id="38699" class="Keyword">import</a> <a id="38706" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="38751" class="Keyword">open</a> <a id="38756" class="Keyword">import</a> <a id="38763" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="38812" class="Keyword">open</a> <a id="38817" class="Keyword">import</a> <a id="38824" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="38875" class="Keyword">open</a> <a id="38880" class="Keyword">import</a> <a id="38887" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="38931" class="Keyword">open</a> <a id="38936" class="Keyword">import</a> <a id="38943" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="39021" class="Keyword">open</a> <a id="39026" class="Keyword">import</a> <a id="39033" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="39073" class="Keyword">open</a> <a id="39078" class="Keyword">import</a> <a id="39085" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="39142" class="Keyword">open</a> <a id="39147" class="Keyword">import</a> <a id="39154" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="39189" class="Keyword">open</a> <a id="39194" class="Keyword">import</a> <a id="39201" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="39247" class="Keyword">open</a> <a id="39252" class="Keyword">import</a> <a id="39259" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="39314" class="Keyword">open</a> <a id="39319" class="Keyword">import</a> <a id="39326" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="39369" class="Keyword">open</a> <a id="39374" class="Keyword">import</a> <a id="39381" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="39426" class="Keyword">open</a> <a id="39431" class="Keyword">import</a> <a id="39438" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="39497" class="Keyword">open</a> <a id="39502" class="Keyword">import</a> <a id="39509" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="39546" class="Keyword">open</a> <a id="39551" class="Keyword">import</a> <a id="39558" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="39600" class="Keyword">open</a> <a id="39605" class="Keyword">import</a> <a id="39612" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="39653" class="Keyword">open</a> <a id="39658" class="Keyword">import</a> <a id="39665" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="39704" class="Keyword">open</a> <a id="39709" class="Keyword">import</a> <a id="39716" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="39754" class="Keyword">open</a> <a id="39759" class="Keyword">import</a> <a id="39766" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="39818" class="Keyword">open</a> <a id="39823" class="Keyword">import</a> <a id="39830" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="39875" class="Keyword">open</a> <a id="39880" class="Keyword">import</a> <a id="39887" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="39926" class="Keyword">open</a> <a id="39931" class="Keyword">import</a> <a id="39938" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="39975" class="Keyword">open</a> <a id="39980" class="Keyword">import</a> <a id="39987" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="40036" class="Keyword">open</a> <a id="40041" class="Keyword">import</a> <a id="40048" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="40087" class="Keyword">open</a> <a id="40092" class="Keyword">import</a> <a id="40099" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="40137" class="Keyword">open</a> <a id="40142" class="Keyword">import</a> <a id="40149" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="40204" class="Keyword">open</a> <a id="40209" class="Keyword">import</a> <a id="40216" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="40255" class="Keyword">open</a> <a id="40260" class="Keyword">import</a> <a id="40267" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="40315" class="Keyword">open</a> <a id="40320" class="Keyword">import</a> <a id="40327" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="40374" class="Keyword">open</a> <a id="40379" class="Keyword">import</a> <a id="40386" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="40424" class="Keyword">open</a> <a id="40429" class="Keyword">import</a> <a id="40436" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="40466" class="Keyword">open</a> <a id="40471" class="Keyword">import</a> <a id="40478" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="40535" class="Keyword">open</a> <a id="40540" class="Keyword">import</a> <a id="40547" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="40601" class="Keyword">open</a> <a id="40606" class="Keyword">import</a> <a id="40613" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="40643" class="Keyword">open</a> <a id="40648" class="Keyword">import</a> <a id="40655" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="40704" class="Keyword">open</a> <a id="40709" class="Keyword">import</a> <a id="40716" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="40758" class="Keyword">open</a> <a id="40763" class="Keyword">import</a> <a id="40770" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="40804" class="Keyword">open</a> <a id="40809" class="Keyword">import</a> <a id="40816" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="40879" class="Keyword">open</a> <a id="40884" class="Keyword">import</a> <a id="40891" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="40934" class="Keyword">open</a> <a id="40939" class="Keyword">import</a> <a id="40946" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="40981" class="Keyword">open</a> <a id="40986" class="Keyword">import</a> <a id="40993" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="41028" class="Keyword">open</a> <a id="41033" class="Keyword">import</a> <a id="41040" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="41080" class="Keyword">open</a> <a id="41085" class="Keyword">import</a> <a id="41092" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="41137" class="Keyword">open</a> <a id="41142" class="Keyword">import</a> <a id="41149" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="41190" class="Keyword">open</a> <a id="41195" class="Keyword">import</a> <a id="41202" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="41256" class="Keyword">open</a> <a id="41261" class="Keyword">import</a> <a id="41268" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="41318" class="Keyword">open</a> <a id="41323" class="Keyword">import</a> <a id="41330" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="41377" class="Keyword">open</a> <a id="41382" class="Keyword">import</a> <a id="41389" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="41427" class="Keyword">open</a> <a id="41432" class="Keyword">import</a> <a id="41439" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="41488" class="Keyword">open</a> <a id="41493" class="Keyword">import</a> <a id="41500" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="41547" class="Keyword">open</a> <a id="41552" class="Keyword">import</a> <a id="41559" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="41622" class="Keyword">open</a> <a id="41627" class="Keyword">import</a> <a id="41634" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="41666" class="Keyword">open</a> <a id="41671" class="Keyword">import</a> <a id="41678" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="41731" class="Keyword">open</a> <a id="41736" class="Keyword">import</a> <a id="41743" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="41789" class="Keyword">open</a> <a id="41794" class="Keyword">import</a> <a id="41801" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="41847" class="Keyword">open</a> <a id="41852" class="Keyword">import</a> <a id="41859" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="41899" class="Keyword">open</a> <a id="41904" class="Keyword">import</a> <a id="41911" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="41958" class="Keyword">open</a> <a id="41963" class="Keyword">import</a> <a id="41970" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="42018" class="Keyword">open</a> <a id="42023" class="Keyword">import</a> <a id="42030" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="42070" class="Keyword">open</a> <a id="42075" class="Keyword">import</a> <a id="42082" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="42127" class="Keyword">open</a> <a id="42132" class="Keyword">import</a> <a id="42139" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="42204" class="Keyword">open</a> <a id="42209" class="Keyword">import</a> <a id="42216" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="42261" class="Keyword">open</a> <a id="42266" class="Keyword">import</a> <a id="42273" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="42320" class="Keyword">open</a> <a id="42325" class="Keyword">import</a> <a id="42332" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="42385" class="Keyword">open</a> <a id="42390" class="Keyword">import</a> <a id="42397" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>