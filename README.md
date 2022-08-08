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
<a id="25263" class="Keyword">open</a> <a id="25268" class="Keyword">import</a> <a id="25275" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="25301" class="Keyword">open</a> <a id="25306" class="Keyword">import</a> <a id="25313" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25351" class="Keyword">open</a> <a id="25356" class="Keyword">import</a> <a id="25363" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="25421" class="Keyword">open</a> <a id="25426" class="Keyword">import</a> <a id="25433" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="25471" class="Keyword">open</a> <a id="25476" class="Keyword">import</a> <a id="25483" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="25502" class="Keyword">open</a> <a id="25507" class="Keyword">import</a> <a id="25514" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="25579" class="Keyword">open</a> <a id="25584" class="Keyword">import</a> <a id="25591" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="25622" class="Keyword">open</a> <a id="25627" class="Keyword">import</a> <a id="25634" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="25661" class="Keyword">open</a> <a id="25666" class="Keyword">import</a> <a id="25673" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="25701" class="Keyword">open</a> <a id="25706" class="Keyword">import</a> <a id="25713" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="25780" class="Keyword">open</a> <a id="25785" class="Keyword">import</a> <a id="25792" href="group-theory.html" class="Module">group-theory</a>
<a id="25805" class="Keyword">open</a> <a id="25810" class="Keyword">import</a> <a id="25817" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="25845" class="Keyword">open</a> <a id="25850" class="Keyword">import</a> <a id="25857" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25908" class="Keyword">open</a> <a id="25913" class="Keyword">import</a> <a id="25920" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25953" class="Keyword">open</a> <a id="25958" class="Keyword">import</a> <a id="25965" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26012" class="Keyword">open</a> <a id="26017" class="Keyword">import</a> <a id="26024" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26063" class="Keyword">open</a> <a id="26068" class="Keyword">import</a> <a id="26075" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="26115" class="Keyword">open</a> <a id="26120" class="Keyword">import</a> <a id="26127" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="26170" class="Keyword">open</a> <a id="26175" class="Keyword">import</a> <a id="26182" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="26214" class="Keyword">open</a> <a id="26219" class="Keyword">import</a> <a id="26226" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="26262" class="Keyword">open</a> <a id="26267" class="Keyword">import</a> <a id="26274" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="26303" class="Keyword">open</a> <a id="26308" class="Keyword">import</a> <a id="26315" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="26343" class="Keyword">open</a> <a id="26348" class="Keyword">import</a> <a id="26355" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="26388" class="Keyword">open</a> <a id="26393" class="Keyword">import</a> <a id="26400" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="26436" class="Keyword">open</a> <a id="26441" class="Keyword">import</a> <a id="26448" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="26477" class="Keyword">open</a> <a id="26482" class="Keyword">import</a> <a id="26489" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="26514" class="Keyword">open</a> <a id="26519" class="Keyword">import</a> <a id="26526" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="26588" class="Keyword">open</a> <a id="26593" class="Keyword">import</a> <a id="26600" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="26641" class="Keyword">open</a> <a id="26646" class="Keyword">import</a> <a id="26653" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="26682" class="Keyword">open</a> <a id="26687" class="Keyword">import</a> <a id="26694" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="26718" class="Keyword">open</a> <a id="26723" class="Keyword">import</a> <a id="26730" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="26761" class="Keyword">open</a> <a id="26766" class="Keyword">import</a> <a id="26773" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="26820" class="Keyword">open</a> <a id="26825" class="Keyword">import</a> <a id="26832" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="26865" class="Keyword">open</a> <a id="26870" class="Keyword">import</a> <a id="26877" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="26926" class="Keyword">open</a> <a id="26931" class="Keyword">import</a> <a id="26938" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="26978" class="Keyword">open</a> <a id="26983" class="Keyword">import</a> <a id="26990" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="27027" class="Keyword">open</a> <a id="27032" class="Keyword">import</a> <a id="27039" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="27086" class="Keyword">open</a> <a id="27091" class="Keyword">import</a> <a id="27098" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="27139" class="Keyword">open</a> <a id="27144" class="Keyword">import</a> <a id="27151" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="27190" class="Keyword">open</a> <a id="27195" class="Keyword">import</a> <a id="27202" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="27234" class="Keyword">open</a> <a id="27239" class="Keyword">import</a> <a id="27246" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="27273" class="Keyword">open</a> <a id="27278" class="Keyword">import</a> <a id="27285" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="27305" class="Keyword">open</a> <a id="27310" class="Keyword">import</a> <a id="27317" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="27351" class="Keyword">open</a> <a id="27356" class="Keyword">import</a> <a id="27363" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="27390" class="Keyword">open</a> <a id="27395" class="Keyword">import</a> <a id="27402" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="27444" class="Keyword">open</a> <a id="27449" class="Keyword">import</a> <a id="27456" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="27506" class="Keyword">open</a> <a id="27511" class="Keyword">import</a> <a id="27518" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="27565" class="Keyword">open</a> <a id="27570" class="Keyword">import</a> <a id="27577" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="27618" class="Keyword">open</a> <a id="27623" class="Keyword">import</a> <a id="27630" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="27664" class="Keyword">open</a> <a id="27669" class="Keyword">import</a> <a id="27676" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="27717" class="Keyword">open</a> <a id="27722" class="Keyword">import</a> <a id="27729" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="27764" class="Keyword">open</a> <a id="27769" class="Keyword">import</a> <a id="27776" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="27814" class="Keyword">open</a> <a id="27819" class="Keyword">import</a> <a id="27826" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="27861" class="Keyword">open</a> <a id="27866" class="Keyword">import</a> <a id="27873" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="27905" class="Keyword">open</a> <a id="27910" class="Keyword">import</a> <a id="27917" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="27958" class="Keyword">open</a> <a id="27963" class="Keyword">import</a> <a id="27970" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="28011" class="Keyword">open</a> <a id="28016" class="Keyword">import</a> <a id="28023" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="28063" class="Keyword">open</a> <a id="28068" class="Keyword">import</a> <a id="28075" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="28108" class="Keyword">open</a> <a id="28113" class="Keyword">import</a> <a id="28120" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="28157" class="Keyword">open</a> <a id="28162" class="Keyword">import</a> <a id="28169" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="28199" class="Keyword">open</a> <a id="28204" class="Keyword">import</a> <a id="28211" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="28232" class="Keyword">open</a> <a id="28237" class="Keyword">import</a> <a id="28244" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="28298" class="Keyword">open</a> <a id="28303" class="Keyword">import</a> <a id="28310" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="28355" class="Keyword">open</a> <a id="28360" class="Keyword">import</a> <a id="28367" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="28395" class="Keyword">open</a> <a id="28400" class="Keyword">import</a> <a id="28407" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="28428" class="Keyword">open</a> <a id="28433" class="Keyword">import</a> <a id="28440" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="28483" class="Keyword">open</a> <a id="28488" class="Keyword">import</a> <a id="28495" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="28529" class="Keyword">open</a> <a id="28534" class="Keyword">import</a> <a id="28541" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="28571" class="Keyword">open</a> <a id="28576" class="Keyword">import</a> <a id="28583" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="28629" class="Keyword">open</a> <a id="28634" class="Keyword">import</a> <a id="28641" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="28695" class="Keyword">open</a> <a id="28700" class="Keyword">import</a> <a id="28707" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="28750" class="Keyword">open</a> <a id="28755" class="Keyword">import</a> <a id="28762" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="28796" class="Keyword">open</a> <a id="28801" class="Keyword">import</a> <a id="28808" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="28849" class="Keyword">open</a> <a id="28854" class="Keyword">import</a> <a id="28861" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="28896" class="Keyword">open</a> <a id="28901" class="Keyword">import</a> <a id="28908" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="28950" class="Keyword">open</a> <a id="28955" class="Keyword">import</a> <a id="28962" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="28997" class="Keyword">open</a> <a id="29002" class="Keyword">import</a> <a id="29009" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="29048" class="Keyword">open</a> <a id="29053" class="Keyword">import</a> <a id="29060" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="29097" class="Keyword">open</a> <a id="29102" class="Keyword">import</a> <a id="29109" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="29156" class="Keyword">open</a> <a id="29161" class="Keyword">import</a> <a id="29168" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="29232" class="Keyword">open</a> <a id="29237" class="Keyword">import</a> <a id="29244" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="29289" class="Keyword">open</a> <a id="29294" class="Keyword">import</a> <a id="29301" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="29325" class="Keyword">open</a> <a id="29330" class="Keyword">import</a> <a id="29337" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="29362" class="Keyword">open</a> <a id="29367" class="Keyword">import</a> <a id="29374" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="29417" class="Keyword">open</a> <a id="29422" class="Keyword">import</a> <a id="29429" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="29460" class="Keyword">open</a> <a id="29465" class="Keyword">import</a> <a id="29472" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="29526" class="Keyword">open</a> <a id="29531" class="Keyword">import</a> <a id="29538" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="29561" class="Keyword">open</a> <a id="29566" class="Keyword">import</a> <a id="29573" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="29611" class="Keyword">open</a> <a id="29616" class="Keyword">import</a> <a id="29623" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="29662" class="Keyword">open</a> <a id="29667" class="Keyword">import</a> <a id="29674" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="29725" class="Keyword">open</a> <a id="29730" class="Keyword">import</a> <a id="29737" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="29774" class="Keyword">open</a> <a id="29779" class="Keyword">import</a> <a id="29786" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="29843" class="Keyword">open</a> <a id="29848" class="Keyword">import</a> <a id="29855" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="29903" class="Keyword">open</a> <a id="29908" class="Keyword">import</a> <a id="29915" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="29945" class="Keyword">open</a> <a id="29950" class="Keyword">import</a> <a id="29957" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="29994" class="Keyword">open</a> <a id="29999" class="Keyword">import</a> <a id="30006" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="30027" class="Keyword">open</a> <a id="30032" class="Keyword">import</a> <a id="30039" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="30086" class="Keyword">open</a> <a id="30091" class="Keyword">import</a> <a id="30098" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="30136" class="Keyword">open</a> <a id="30141" class="Keyword">import</a> <a id="30148" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="30242" class="Keyword">open</a> <a id="30247" class="Keyword">import</a> <a id="30254" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="30269" class="Keyword">open</a> <a id="30274" class="Keyword">import</a> <a id="30281" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="30314" class="Keyword">open</a> <a id="30319" class="Keyword">import</a> <a id="30326" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="30358" class="Keyword">open</a> <a id="30363" class="Keyword">import</a> <a id="30370" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="30412" class="Keyword">open</a> <a id="30417" class="Keyword">import</a> <a id="30424" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="30462" class="Keyword">open</a> <a id="30467" class="Keyword">import</a> <a id="30474" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="30511" class="Keyword">open</a> <a id="30516" class="Keyword">import</a> <a id="30523" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="30556" class="Keyword">open</a> <a id="30561" class="Keyword">import</a> <a id="30568" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="30592" class="Keyword">open</a> <a id="30597" class="Keyword">import</a> <a id="30604" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="30643" class="Keyword">open</a> <a id="30648" class="Keyword">import</a> <a id="30655" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="30701" class="Keyword">open</a> <a id="30706" class="Keyword">import</a> <a id="30713" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="30758" class="Keyword">open</a> <a id="30763" class="Keyword">import</a> <a id="30770" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="30808" class="Keyword">open</a> <a id="30813" class="Keyword">import</a> <a id="30820" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="30852" class="Keyword">open</a> <a id="30857" class="Keyword">import</a> <a id="30864" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="30917" class="Keyword">open</a> <a id="30922" class="Keyword">import</a> <a id="30929" href="order-theory.html" class="Module">order-theory</a>
<a id="30942" class="Keyword">open</a> <a id="30947" class="Keyword">import</a> <a id="30954" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="30981" class="Keyword">open</a> <a id="30986" class="Keyword">import</a> <a id="30993" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="31023" class="Keyword">open</a> <a id="31028" class="Keyword">import</a> <a id="31035" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="31068" class="Keyword">open</a> <a id="31073" class="Keyword">import</a> <a id="31080" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="31116" class="Keyword">open</a> <a id="31121" class="Keyword">import</a> <a id="31128" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="31163" class="Keyword">open</a> <a id="31168" class="Keyword">import</a> <a id="31175" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="31202" class="Keyword">open</a> <a id="31207" class="Keyword">import</a> <a id="31214" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="31244" class="Keyword">open</a> <a id="31249" class="Keyword">import</a> <a id="31256" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="31292" class="Keyword">open</a> <a id="31297" class="Keyword">import</a> <a id="31304" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="31346" class="Keyword">open</a> <a id="31351" class="Keyword">import</a> <a id="31358" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="31390" class="Keyword">open</a> <a id="31395" class="Keyword">import</a> <a id="31402" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="31433" class="Keyword">open</a> <a id="31438" class="Keyword">import</a> <a id="31445" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="31471" class="Keyword">open</a> <a id="31476" class="Keyword">import</a> <a id="31483" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="31512" class="Keyword">open</a> <a id="31517" class="Keyword">import</a> <a id="31524" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="31561" class="Keyword">open</a> <a id="31566" class="Keyword">import</a> <a id="31573" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="31613" class="Keyword">open</a> <a id="31618" class="Keyword">import</a> <a id="31625" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="31647" class="Keyword">open</a> <a id="31652" class="Keyword">import</a> <a id="31659" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="31694" class="Keyword">open</a> <a id="31699" class="Keyword">import</a> <a id="31706" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="31744" class="Keyword">open</a> <a id="31749" class="Keyword">import</a> <a id="31756" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="31795" class="Keyword">open</a> <a id="31800" class="Keyword">import</a> <a id="31807" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="31842" class="Keyword">open</a> <a id="31847" class="Keyword">import</a> <a id="31854" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="31889" class="Keyword">open</a> <a id="31894" class="Keyword">import</a> <a id="31901" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="31939" class="Keyword">open</a> <a id="31944" class="Keyword">import</a> <a id="31951" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="31982" class="Keyword">open</a> <a id="31987" class="Keyword">import</a> <a id="31994" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="32036" class="Keyword">open</a> <a id="32041" class="Keyword">import</a> <a id="32048" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="32093" class="Keyword">open</a> <a id="32098" class="Keyword">import</a> <a id="32105" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="32138" class="Keyword">open</a> <a id="32143" class="Keyword">import</a> <a id="32150" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="32170" class="Keyword">open</a> <a id="32175" class="Keyword">import</a> <a id="32182" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="32205" class="Keyword">open</a> <a id="32210" class="Keyword">import</a> <a id="32217" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="32240" class="Keyword">open</a> <a id="32245" class="Keyword">import</a> <a id="32252" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="32278" class="Keyword">open</a> <a id="32283" class="Keyword">import</a> <a id="32290" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="32316" class="Keyword">open</a> <a id="32321" class="Keyword">import</a> <a id="32328" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="32392" class="Keyword">open</a> <a id="32397" class="Keyword">import</a> <a id="32404" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="32422" class="Keyword">open</a> <a id="32427" class="Keyword">import</a> <a id="32434" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="32461" class="Keyword">open</a> <a id="32466" class="Keyword">import</a> <a id="32473" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="32499" class="Keyword">open</a> <a id="32504" class="Keyword">import</a> <a id="32511" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="32537" class="Keyword">open</a> <a id="32542" class="Keyword">import</a> <a id="32549" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="32575" class="Keyword">open</a> <a id="32580" class="Keyword">import</a> <a id="32587" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="32618" class="Keyword">open</a> <a id="32623" class="Keyword">import</a> <a id="32630" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="32693" class="Keyword">open</a> <a id="32698" class="Keyword">import</a> <a id="32705" href="polytopes.html" class="Module">polytopes</a>
<a id="32715" class="Keyword">open</a> <a id="32720" class="Keyword">import</a> <a id="32727" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="32785" class="Keyword">open</a> <a id="32790" class="Keyword">import</a> <a id="32797" href="ring-theory.html" class="Module">ring-theory</a>
<a id="32809" class="Keyword">open</a> <a id="32814" class="Keyword">import</a> <a id="32821" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="32858" class="Keyword">open</a> <a id="32863" class="Keyword">import</a> <a id="32870" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="32897" class="Keyword">open</a> <a id="32902" class="Keyword">import</a> <a id="32909" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="32941" class="Keyword">open</a> <a id="32946" class="Keyword">import</a> <a id="32953" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="32999" class="Keyword">open</a> <a id="33004" class="Keyword">import</a> <a id="33011" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="33036" class="Keyword">open</a> <a id="33041" class="Keyword">import</a> <a id="33048" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="33091" class="Keyword">open</a> <a id="33096" class="Keyword">import</a> <a id="33103" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="33141" class="Keyword">open</a> <a id="33146" class="Keyword">import</a> <a id="33153" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="33184" class="Keyword">open</a> <a id="33189" class="Keyword">import</a> <a id="33196" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="33220" class="Keyword">open</a> <a id="33225" class="Keyword">import</a> <a id="33232" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="33264" class="Keyword">open</a> <a id="33269" class="Keyword">import</a> <a id="33276" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="33302" class="Keyword">open</a> <a id="33307" class="Keyword">import</a> <a id="33314" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="33343" class="Keyword">open</a> <a id="33348" class="Keyword">import</a> <a id="33355" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="33392" class="Keyword">open</a> <a id="33397" class="Keyword">import</a> <a id="33404" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="33433" class="Keyword">open</a> <a id="33438" class="Keyword">import</a> <a id="33445" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="33472" class="Keyword">open</a> <a id="33477" class="Keyword">import</a> <a id="33484" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="33521" class="Keyword">open</a> <a id="33526" class="Keyword">import</a> <a id="33533" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="33560" class="Keyword">open</a> <a id="33565" class="Keyword">import</a> <a id="33572" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="33605" class="Keyword">open</a> <a id="33610" class="Keyword">import</a> <a id="33617" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="33635" class="Keyword">open</a> <a id="33640" class="Keyword">import</a> <a id="33647" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="33701" class="Keyword">open</a> <a id="33706" class="Keyword">import</a> <a id="33713" href="set-theory.html" class="Module">set-theory</a>
<a id="33724" class="Keyword">open</a> <a id="33729" class="Keyword">import</a> <a id="33736" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="33759" class="Keyword">open</a> <a id="33764" class="Keyword">import</a> <a id="33771" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="33795" class="Keyword">open</a> <a id="33800" class="Keyword">import</a> <a id="33807" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="33833" class="Keyword">open</a> <a id="33838" class="Keyword">import</a> <a id="33845" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="33907" class="Keyword">open</a> <a id="33912" class="Keyword">import</a> <a id="33919" href="structured-types.html" class="Module">structured-types</a>
<a id="33936" class="Keyword">open</a> <a id="33941" class="Keyword">import</a> <a id="33948" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="33983" class="Keyword">open</a> <a id="33988" class="Keyword">import</a> <a id="33995" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="34039" class="Keyword">open</a> <a id="34044" class="Keyword">import</a> <a id="34051" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="34115" class="Keyword">open</a> <a id="34120" class="Keyword">import</a> <a id="34127" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="34166" class="Keyword">open</a> <a id="34171" class="Keyword">import</a> <a id="34178" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="34224" class="Keyword">open</a> <a id="34229" class="Keyword">import</a> <a id="34236" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="34260" class="Keyword">open</a> <a id="34265" class="Keyword">import</a> <a id="34272" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="34341" class="Keyword">open</a> <a id="34346" class="Keyword">import</a> <a id="34353" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="34398" class="Keyword">open</a> <a id="34403" class="Keyword">import</a> <a id="34410" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="34444" class="Keyword">open</a> <a id="34449" class="Keyword">import</a> <a id="34456" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="34517" class="Keyword">open</a> <a id="34522" class="Keyword">import</a> <a id="34529" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="34574" class="Keyword">open</a> <a id="34579" class="Keyword">import</a> <a id="34586" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="34624" class="Keyword">open</a> <a id="34629" class="Keyword">import</a> <a id="34636" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="34679" class="Keyword">open</a> <a id="34684" class="Keyword">import</a> <a id="34691" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="34727" class="Keyword">open</a> <a id="34732" class="Keyword">import</a> <a id="34739" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="34769" class="Keyword">open</a> <a id="34774" class="Keyword">import</a> <a id="34781" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="34812" class="Keyword">open</a> <a id="34817" class="Keyword">import</a> <a id="34824" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="34883" class="Keyword">open</a> <a id="34888" class="Keyword">import</a> <a id="34895" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="34946" class="Keyword">open</a> <a id="34951" class="Keyword">import</a> <a id="34958" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="35009" class="Keyword">open</a> <a id="35014" class="Keyword">import</a> <a id="35021" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="35076" class="Keyword">open</a> <a id="35081" class="Keyword">import</a> <a id="35088" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="35117" class="Keyword">open</a> <a id="35122" class="Keyword">import</a> <a id="35129" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="35157" class="Keyword">open</a> <a id="35162" class="Keyword">import</a> <a id="35169" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="35199" class="Keyword">open</a> <a id="35204" class="Keyword">import</a> <a id="35211" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="35245" class="Keyword">open</a> <a id="35250" class="Keyword">import</a> <a id="35257" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="35333" class="Keyword">open</a> <a id="35338" class="Keyword">import</a> <a id="35345" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="35371" class="Keyword">open</a> <a id="35376" class="Keyword">import</a> <a id="35383" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="35421" class="Keyword">open</a> <a id="35426" class="Keyword">import</a> <a id="35433" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="35470" class="Keyword">open</a> <a id="35475" class="Keyword">import</a> <a id="35482" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="35522" class="Keyword">open</a> <a id="35527" class="Keyword">import</a> <a id="35534" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="35573" class="Keyword">open</a> <a id="35578" class="Keyword">import</a> <a id="35585" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="35618" class="Keyword">open</a> <a id="35623" class="Keyword">import</a> <a id="35630" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="35673" class="Keyword">open</a> <a id="35678" class="Keyword">import</a> <a id="35685" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="35720" class="Keyword">open</a> <a id="35725" class="Keyword">import</a> <a id="35732" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="35777" class="Keyword">open</a> <a id="35782" class="Keyword">import</a> <a id="35789" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="35826" class="Keyword">open</a> <a id="35831" class="Keyword">import</a> <a id="35838" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="35890" class="Keyword">open</a> <a id="35895" class="Keyword">import</a> <a id="35902" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="35955" class="Keyword">open</a> <a id="35960" class="Keyword">import</a> <a id="35967" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="36027" class="Keyword">open</a> <a id="36032" class="Keyword">import</a> <a id="36039" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="36087" class="Keyword">open</a> <a id="36092" class="Keyword">import</a> <a id="36099" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="36139" class="Keyword">open</a> <a id="36144" class="Keyword">import</a> <a id="36151" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="36198" class="Keyword">open</a> <a id="36203" class="Keyword">import</a> <a id="36210" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="36251" class="Keyword">open</a> <a id="36256" class="Keyword">import</a> <a id="36263" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="36301" class="Keyword">open</a> <a id="36306" class="Keyword">import</a> <a id="36313" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="36361" class="Keyword">open</a> <a id="36366" class="Keyword">import</a> <a id="36373" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="36410" class="Keyword">open</a> <a id="36415" class="Keyword">import</a> <a id="36422" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="36457" class="Keyword">open</a> <a id="36462" class="Keyword">import</a> <a id="36469" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="36503" class="Keyword">open</a> <a id="36508" class="Keyword">import</a> <a id="36515" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="36562" class="Keyword">open</a> <a id="36567" class="Keyword">import</a> <a id="36574" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="36619" class="Keyword">open</a> <a id="36624" class="Keyword">import</a> <a id="36631" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="36680" class="Keyword">open</a> <a id="36685" class="Keyword">import</a> <a id="36692" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="36744" class="Keyword">open</a> <a id="36749" class="Keyword">import</a> <a id="36756" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="36810" class="Keyword">open</a> <a id="36815" class="Keyword">import</a> <a id="36822" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="36899" class="Keyword">open</a> <a id="36904" class="Keyword">import</a> <a id="36911" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="36963" class="Keyword">open</a> <a id="36968" class="Keyword">import</a> <a id="36975" href="type-theories.html" class="Module">type-theories</a>
<a id="36989" class="Keyword">open</a> <a id="36994" class="Keyword">import</a> <a id="37001" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="37043" class="Keyword">open</a> <a id="37048" class="Keyword">import</a> <a id="37055" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="37093" class="Keyword">open</a> <a id="37098" class="Keyword">import</a> <a id="37105" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="37151" class="Keyword">open</a> <a id="37156" class="Keyword">import</a> <a id="37163" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="37210" class="Keyword">open</a> <a id="37215" class="Keyword">import</a> <a id="37222" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="37257" class="Keyword">open</a> <a id="37262" class="Keyword">import</a> <a id="37269" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="37347" class="Keyword">open</a> <a id="37352" class="Keyword">import</a> <a id="37359" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="37383" class="Keyword">open</a> <a id="37388" class="Keyword">import</a> <a id="37395" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="37448" class="Keyword">open</a> <a id="37453" class="Keyword">import</a> <a id="37460" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="37503" class="Keyword">open</a> <a id="37508" class="Keyword">import</a> <a id="37515" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="37555" class="Keyword">open</a> <a id="37560" class="Keyword">import</a> <a id="37567" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="37606" class="Keyword">open</a> <a id="37611" class="Keyword">import</a> <a id="37618" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="37652" class="Keyword">open</a> <a id="37657" class="Keyword">import</a> <a id="37664" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="37712" class="Keyword">open</a> <a id="37717" class="Keyword">import</a> <a id="37724" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="37775" class="Keyword">open</a> <a id="37780" class="Keyword">import</a> <a id="37787" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="37834" class="Keyword">open</a> <a id="37839" class="Keyword">import</a> <a id="37846" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="37898" class="Keyword">open</a> <a id="37903" class="Keyword">import</a> <a id="37910" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="37954" class="Keyword">open</a> <a id="37959" class="Keyword">import</a> <a id="37966" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="38006" class="Keyword">open</a> <a id="38011" class="Keyword">import</a> <a id="38018" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="38061" class="Keyword">open</a> <a id="38066" class="Keyword">import</a> <a id="38073" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="38125" class="Keyword">open</a> <a id="38130" class="Keyword">import</a> <a id="38137" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="38191" class="Keyword">open</a> <a id="38196" class="Keyword">import</a> <a id="38203" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="38251" class="Keyword">open</a> <a id="38256" class="Keyword">import</a> <a id="38263" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="38302" class="Keyword">open</a> <a id="38307" class="Keyword">import</a> <a id="38314" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="38347" class="Keyword">open</a> <a id="38352" class="Keyword">import</a> <a id="38359" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="38389" class="Keyword">open</a> <a id="38394" class="Keyword">import</a> <a id="38401" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="38452" class="Keyword">open</a> <a id="38457" class="Keyword">import</a> <a id="38464" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="38505" class="Keyword">open</a> <a id="38510" class="Keyword">import</a> <a id="38517" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="38554" class="Keyword">open</a> <a id="38559" class="Keyword">import</a> <a id="38566" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="38625" class="Keyword">open</a> <a id="38630" class="Keyword">import</a> <a id="38637" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="38692" class="Keyword">open</a> <a id="38697" class="Keyword">import</a> <a id="38704" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="38760" class="Keyword">open</a> <a id="38765" class="Keyword">import</a> <a id="38772" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="38819" class="Keyword">open</a> <a id="38824" class="Keyword">import</a> <a id="38831" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="38874" class="Keyword">open</a> <a id="38879" class="Keyword">import</a> <a id="38886" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="38931" class="Keyword">open</a> <a id="38936" class="Keyword">import</a> <a id="38943" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="38992" class="Keyword">open</a> <a id="38997" class="Keyword">import</a> <a id="39004" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="39055" class="Keyword">open</a> <a id="39060" class="Keyword">import</a> <a id="39067" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="39111" class="Keyword">open</a> <a id="39116" class="Keyword">import</a> <a id="39123" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="39201" class="Keyword">open</a> <a id="39206" class="Keyword">import</a> <a id="39213" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="39253" class="Keyword">open</a> <a id="39258" class="Keyword">import</a> <a id="39265" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="39322" class="Keyword">open</a> <a id="39327" class="Keyword">import</a> <a id="39334" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="39369" class="Keyword">open</a> <a id="39374" class="Keyword">import</a> <a id="39381" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="39427" class="Keyword">open</a> <a id="39432" class="Keyword">import</a> <a id="39439" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="39494" class="Keyword">open</a> <a id="39499" class="Keyword">import</a> <a id="39506" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="39549" class="Keyword">open</a> <a id="39554" class="Keyword">import</a> <a id="39561" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="39606" class="Keyword">open</a> <a id="39611" class="Keyword">import</a> <a id="39618" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="39677" class="Keyword">open</a> <a id="39682" class="Keyword">import</a> <a id="39689" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="39726" class="Keyword">open</a> <a id="39731" class="Keyword">import</a> <a id="39738" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="39780" class="Keyword">open</a> <a id="39785" class="Keyword">import</a> <a id="39792" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="39833" class="Keyword">open</a> <a id="39838" class="Keyword">import</a> <a id="39845" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="39884" class="Keyword">open</a> <a id="39889" class="Keyword">import</a> <a id="39896" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="39934" class="Keyword">open</a> <a id="39939" class="Keyword">import</a> <a id="39946" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="39998" class="Keyword">open</a> <a id="40003" class="Keyword">import</a> <a id="40010" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="40055" class="Keyword">open</a> <a id="40060" class="Keyword">import</a> <a id="40067" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="40106" class="Keyword">open</a> <a id="40111" class="Keyword">import</a> <a id="40118" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="40155" class="Keyword">open</a> <a id="40160" class="Keyword">import</a> <a id="40167" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="40216" class="Keyword">open</a> <a id="40221" class="Keyword">import</a> <a id="40228" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="40267" class="Keyword">open</a> <a id="40272" class="Keyword">import</a> <a id="40279" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="40317" class="Keyword">open</a> <a id="40322" class="Keyword">import</a> <a id="40329" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="40384" class="Keyword">open</a> <a id="40389" class="Keyword">import</a> <a id="40396" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="40435" class="Keyword">open</a> <a id="40440" class="Keyword">import</a> <a id="40447" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="40495" class="Keyword">open</a> <a id="40500" class="Keyword">import</a> <a id="40507" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="40554" class="Keyword">open</a> <a id="40559" class="Keyword">import</a> <a id="40566" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="40604" class="Keyword">open</a> <a id="40609" class="Keyword">import</a> <a id="40616" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="40646" class="Keyword">open</a> <a id="40651" class="Keyword">import</a> <a id="40658" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="40715" class="Keyword">open</a> <a id="40720" class="Keyword">import</a> <a id="40727" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="40781" class="Keyword">open</a> <a id="40786" class="Keyword">import</a> <a id="40793" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="40823" class="Keyword">open</a> <a id="40828" class="Keyword">import</a> <a id="40835" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="40884" class="Keyword">open</a> <a id="40889" class="Keyword">import</a> <a id="40896" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="40938" class="Keyword">open</a> <a id="40943" class="Keyword">import</a> <a id="40950" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="40984" class="Keyword">open</a> <a id="40989" class="Keyword">import</a> <a id="40996" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="41059" class="Keyword">open</a> <a id="41064" class="Keyword">import</a> <a id="41071" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="41114" class="Keyword">open</a> <a id="41119" class="Keyword">import</a> <a id="41126" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="41161" class="Keyword">open</a> <a id="41166" class="Keyword">import</a> <a id="41173" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="41208" class="Keyword">open</a> <a id="41213" class="Keyword">import</a> <a id="41220" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="41260" class="Keyword">open</a> <a id="41265" class="Keyword">import</a> <a id="41272" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="41317" class="Keyword">open</a> <a id="41322" class="Keyword">import</a> <a id="41329" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="41370" class="Keyword">open</a> <a id="41375" class="Keyword">import</a> <a id="41382" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="41436" class="Keyword">open</a> <a id="41441" class="Keyword">import</a> <a id="41448" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="41498" class="Keyword">open</a> <a id="41503" class="Keyword">import</a> <a id="41510" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="41557" class="Keyword">open</a> <a id="41562" class="Keyword">import</a> <a id="41569" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="41607" class="Keyword">open</a> <a id="41612" class="Keyword">import</a> <a id="41619" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="41668" class="Keyword">open</a> <a id="41673" class="Keyword">import</a> <a id="41680" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="41727" class="Keyword">open</a> <a id="41732" class="Keyword">import</a> <a id="41739" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="41802" class="Keyword">open</a> <a id="41807" class="Keyword">import</a> <a id="41814" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="41846" class="Keyword">open</a> <a id="41851" class="Keyword">import</a> <a id="41858" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="41911" class="Keyword">open</a> <a id="41916" class="Keyword">import</a> <a id="41923" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="41969" class="Keyword">open</a> <a id="41974" class="Keyword">import</a> <a id="41981" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="42027" class="Keyword">open</a> <a id="42032" class="Keyword">import</a> <a id="42039" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="42079" class="Keyword">open</a> <a id="42084" class="Keyword">import</a> <a id="42091" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="42138" class="Keyword">open</a> <a id="42143" class="Keyword">import</a> <a id="42150" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="42198" class="Keyword">open</a> <a id="42203" class="Keyword">import</a> <a id="42210" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="42250" class="Keyword">open</a> <a id="42255" class="Keyword">import</a> <a id="42262" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="42307" class="Keyword">open</a> <a id="42312" class="Keyword">import</a> <a id="42319" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="42384" class="Keyword">open</a> <a id="42389" class="Keyword">import</a> <a id="42396" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="42441" class="Keyword">open</a> <a id="42446" class="Keyword">import</a> <a id="42453" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="42500" class="Keyword">open</a> <a id="42505" class="Keyword">import</a> <a id="42512" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="42565" class="Keyword">open</a> <a id="42570" class="Keyword">import</a> <a id="42577" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>