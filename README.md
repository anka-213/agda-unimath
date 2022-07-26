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
<a id="7746" class="Keyword">open</a> <a id="7751" class="Keyword">import</a> <a id="7758" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7803" class="Keyword">open</a> <a id="7808" class="Keyword">import</a> <a id="7815" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7867" class="Keyword">open</a> <a id="7872" class="Keyword">import</a> <a id="7879" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7937" class="Keyword">open</a> <a id="7942" class="Keyword">import</a> <a id="7949" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="7995" class="Keyword">open</a> <a id="8000" class="Keyword">import</a> <a id="8007" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="8051" class="Keyword">open</a> <a id="8056" class="Keyword">import</a> <a id="8063" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="8097" class="Keyword">open</a> <a id="8102" class="Keyword">import</a> <a id="8109" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="8163" class="Keyword">open</a> <a id="8168" class="Keyword">import</a> <a id="8175" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="8224" class="Keyword">open</a> <a id="8229" class="Keyword">import</a> <a id="8236" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="8277" class="Keyword">open</a> <a id="8282" class="Keyword">import</a> <a id="8289" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8338" class="Keyword">open</a> <a id="8343" class="Keyword">import</a> <a id="8350" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8416" class="Keyword">open</a> <a id="8421" class="Keyword">import</a> <a id="8428" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8472" class="Keyword">open</a> <a id="8477" class="Keyword">import</a> <a id="8484" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8533" class="Keyword">open</a> <a id="8538" class="Keyword">import</a> <a id="8545" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8601" class="Keyword">open</a> <a id="8606" class="Keyword">import</a> <a id="8613" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8654" class="Keyword">open</a> <a id="8659" class="Keyword">import</a> <a id="8666" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8715" class="Keyword">open</a> <a id="8720" class="Keyword">import</a> <a id="8727" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8786" class="Keyword">open</a> <a id="8791" class="Keyword">import</a> <a id="8798" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8837" class="Keyword">open</a> <a id="8842" class="Keyword">import</a> <a id="8849" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8902" class="Keyword">open</a> <a id="8907" class="Keyword">import</a> <a id="8914" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="8971" class="Keyword">open</a> <a id="8976" class="Keyword">import</a> <a id="8983" href="elementary-number-theory.pythagorean-triples.html" class="Module">elementary-number-theory.pythagorean-triples</a>
<a id="9028" class="Keyword">open</a> <a id="9033" class="Keyword">import</a> <a id="9040" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="9082" class="Keyword">open</a> <a id="9087" class="Keyword">import</a> <a id="9094" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="9145" class="Keyword">open</a> <a id="9150" class="Keyword">import</a> <a id="9157" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9215" class="Keyword">open</a> <a id="9220" class="Keyword">import</a> <a id="9227" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9291" class="Keyword">open</a> <a id="9296" class="Keyword">import</a> <a id="9303" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9356" class="Keyword">open</a> <a id="9361" class="Keyword">import</a> <a id="9368" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9421" class="Keyword">open</a> <a id="9426" class="Keyword">import</a> <a id="9433" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9494" class="Keyword">open</a> <a id="9499" class="Keyword">import</a> <a id="9506" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9564" class="Keyword">open</a> <a id="9569" class="Keyword">import</a> <a id="9576" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9625" class="Keyword">open</a> <a id="9630" class="Keyword">import</a> <a id="9637" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9680" class="Keyword">open</a> <a id="9685" class="Keyword">import</a> <a id="9692" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9736" class="Keyword">open</a> <a id="9741" class="Keyword">import</a> <a id="9748" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9795" class="Keyword">open</a> <a id="9800" class="Keyword">import</a> <a id="9807" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9868" class="Keyword">open</a> <a id="9873" class="Keyword">import</a> <a id="9880" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9943" class="Keyword">open</a> <a id="9948" class="Keyword">import</a> <a id="9955" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="10015" class="Keyword">open</a> <a id="10020" class="Keyword">import</a> <a id="10027" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="10081" class="Keyword">open</a> <a id="10086" class="Keyword">import</a> <a id="10093" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="10158" class="Keyword">open</a> <a id="10163" class="Keyword">import</a> <a id="10170" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10278" class="Keyword">open</a> <a id="10283" class="Keyword">import</a> <a id="10290" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10310" class="Keyword">open</a> <a id="10315" class="Keyword">import</a> <a id="10322" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10368" class="Keyword">open</a> <a id="10373" class="Keyword">import</a> <a id="10380" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a>
<a id="10419" class="Keyword">open</a> <a id="10424" class="Keyword">import</a> <a id="10431" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10487" class="Keyword">open</a> <a id="10492" class="Keyword">import</a> <a id="10499" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10545" class="Keyword">open</a> <a id="10550" class="Keyword">import</a> <a id="10557" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10591" class="Keyword">open</a> <a id="10596" class="Keyword">import</a> <a id="10603" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10638" class="Keyword">open</a> <a id="10643" class="Keyword">import</a> <a id="10650" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10688" class="Keyword">open</a> <a id="10693" class="Keyword">import</a> <a id="10700" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10738" class="Keyword">open</a> <a id="10743" class="Keyword">import</a> <a id="10750" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10790" class="Keyword">open</a> <a id="10795" class="Keyword">import</a> <a id="10802" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10835" class="Keyword">open</a> <a id="10840" class="Keyword">import</a> <a id="10847" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10885" class="Keyword">open</a> <a id="10890" class="Keyword">import</a> <a id="10897" href="finite-group-theory.simpson-delooping-sign-homomorphism.html" class="Module">finite-group-theory.simpson-delooping-sign-homomorphism</a>
<a id="10953" class="Keyword">open</a> <a id="10958" class="Keyword">import</a> <a id="10965" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="11007" class="Keyword">open</a> <a id="11012" class="Keyword">import</a> <a id="11019" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="11082" class="Keyword">open</a> <a id="11087" class="Keyword">import</a> <a id="11094" href="foundation.html" class="Module">foundation</a>
<a id="11105" class="Keyword">open</a> <a id="11110" class="Keyword">import</a> <a id="11117" href="foundation.0-connected-types.html" class="Module">foundation.0-connected-types</a>
<a id="11146" class="Keyword">open</a> <a id="11151" class="Keyword">import</a> <a id="11158" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a>
<a id="11186" class="Keyword">open</a> <a id="11191" class="Keyword">import</a> <a id="11198" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11216" class="Keyword">open</a> <a id="11221" class="Keyword">import</a> <a id="11228" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11247" class="Keyword">open</a> <a id="11252" class="Keyword">import</a> <a id="11259" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11278" class="Keyword">open</a> <a id="11283" class="Keyword">import</a> <a id="11290" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11334" class="Keyword">open</a> <a id="11339" class="Keyword">import</a> <a id="11346" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11371" class="Keyword">open</a> <a id="11376" class="Keyword">import</a> <a id="11383" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11410" class="Keyword">open</a> <a id="11415" class="Keyword">import</a> <a id="11422" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11439" class="Keyword">open</a> <a id="11444" class="Keyword">import</a> <a id="11451" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11480" class="Keyword">open</a> <a id="11485" class="Keyword">import</a> <a id="11492" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11548" class="Keyword">open</a> <a id="11553" class="Keyword">import</a> <a id="11560" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11591" class="Keyword">open</a> <a id="11596" class="Keyword">import</a> <a id="11603" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11657" class="Keyword">open</a> <a id="11662" class="Keyword">import</a> <a id="11669" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11697" class="Keyword">open</a> <a id="11702" class="Keyword">import</a> <a id="11709" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11739" class="Keyword">open</a> <a id="11744" class="Keyword">import</a> <a id="11751" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11771" class="Keyword">open</a> <a id="11776" class="Keyword">import</a> <a id="11783" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11828" class="Keyword">open</a> <a id="11833" class="Keyword">import</a> <a id="11840" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11877" class="Keyword">open</a> <a id="11882" class="Keyword">import</a> <a id="11889" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11924" class="Keyword">open</a> <a id="11929" class="Keyword">import</a> <a id="11936" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11994" class="Keyword">open</a> <a id="11999" class="Keyword">import</a> <a id="12006" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12044" class="Keyword">open</a> <a id="12049" class="Keyword">import</a> <a id="12056" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12090" class="Keyword">open</a> <a id="12095" class="Keyword">import</a> <a id="12102" href="foundation.commuting-cubes.html" class="Module">foundation.commuting-cubes</a>
<a id="12129" class="Keyword">open</a> <a id="12134" class="Keyword">import</a> <a id="12141" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12170" class="Keyword">open</a> <a id="12175" class="Keyword">import</a> <a id="12182" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12205" class="Keyword">open</a> <a id="12210" class="Keyword">import</a> <a id="12217" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12244" class="Keyword">open</a> <a id="12249" class="Keyword">import</a> <a id="12256" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12279" class="Keyword">open</a> <a id="12284" class="Keyword">import</a> <a id="12291" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12333" class="Keyword">open</a> <a id="12338" class="Keyword">import</a> <a id="12345" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12377" class="Keyword">open</a> <a id="12382" class="Keyword">import</a> <a id="12389" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="12415" class="Keyword">open</a> <a id="12420" class="Keyword">import</a> <a id="12427" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12454" class="Keyword">open</a> <a id="12459" class="Keyword">import</a> <a id="12466" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12491" class="Keyword">open</a> <a id="12496" class="Keyword">import</a> <a id="12503" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12532" class="Keyword">open</a> <a id="12537" class="Keyword">import</a> <a id="12544" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12574" class="Keyword">open</a> <a id="12579" class="Keyword">import</a> <a id="12586" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12613" class="Keyword">open</a> <a id="12618" class="Keyword">import</a> <a id="12625" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12644" class="Keyword">open</a> <a id="12649" class="Keyword">import</a> <a id="12656" href="foundation.cospans.html" class="Module">foundation.cospans</a>
<a id="12675" class="Keyword">open</a> <a id="12680" class="Keyword">import</a> <a id="12687" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12733" class="Keyword">open</a> <a id="12738" class="Keyword">import</a> <a id="12745" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12787" class="Keyword">open</a> <a id="12792" class="Keyword">import</a> <a id="12799" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12831" class="Keyword">open</a> <a id="12836" class="Keyword">import</a> <a id="12843" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12873" class="Keyword">open</a> <a id="12878" class="Keyword">import</a> <a id="12885" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="12928" class="Keyword">open</a> <a id="12933" class="Keyword">import</a> <a id="12940" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12966" class="Keyword">open</a> <a id="12971" class="Keyword">import</a> <a id="12978" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="13012" class="Keyword">open</a> <a id="13017" class="Keyword">import</a> <a id="13024" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="13055" class="Keyword">open</a> <a id="13060" class="Keyword">import</a> <a id="13067" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13097" class="Keyword">open</a> <a id="13102" class="Keyword">import</a> <a id="13109" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13136" class="Keyword">open</a> <a id="13141" class="Keyword">import</a> <a id="13148" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13186" class="Keyword">open</a> <a id="13191" class="Keyword">import</a> <a id="13198" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13230" class="Keyword">open</a> <a id="13235" class="Keyword">import</a> <a id="13242" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13277" class="Keyword">open</a> <a id="13282" class="Keyword">import</a> <a id="13289" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13329" class="Keyword">open</a> <a id="13334" class="Keyword">import</a> <a id="13341" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13372" class="Keyword">open</a> <a id="13377" class="Keyword">import</a> <a id="13384" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13418" class="Keyword">open</a> <a id="13423" class="Keyword">import</a> <a id="13430" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="13459" class="Keyword">open</a> <a id="13464" class="Keyword">import</a> <a id="13471" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13494" class="Keyword">open</a> <a id="13499" class="Keyword">import</a> <a id="13506" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13533" class="Keyword">open</a> <a id="13538" class="Keyword">import</a> <a id="13545" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13573" class="Keyword">open</a> <a id="13578" class="Keyword">import</a> <a id="13585" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13622" class="Keyword">open</a> <a id="13627" class="Keyword">import</a> <a id="13634" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13682" class="Keyword">open</a> <a id="13687" class="Keyword">import</a> <a id="13694" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13734" class="Keyword">open</a> <a id="13739" class="Keyword">import</a> <a id="13746" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13768" class="Keyword">open</a> <a id="13773" class="Keyword">import</a> <a id="13780" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13803" class="Keyword">open</a> <a id="13808" class="Keyword">import</a> <a id="13815" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13840" class="Keyword">open</a> <a id="13845" class="Keyword">import</a> <a id="13852" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13897" class="Keyword">open</a> <a id="13902" class="Keyword">import</a> <a id="13909" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13953" class="Keyword">open</a> <a id="13958" class="Keyword">import</a> <a id="13965" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14001" class="Keyword">open</a> <a id="14006" class="Keyword">import</a> <a id="14013" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14058" class="Keyword">open</a> <a id="14063" class="Keyword">import</a> <a id="14070" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14111" class="Keyword">open</a> <a id="14116" class="Keyword">import</a> <a id="14123" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14158" class="Keyword">open</a> <a id="14163" class="Keyword">import</a> <a id="14170" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14202" class="Keyword">open</a> <a id="14207" class="Keyword">import</a> <a id="14214" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14245" class="Keyword">open</a> <a id="14250" class="Keyword">import</a> <a id="14257" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14290" class="Keyword">open</a> <a id="14295" class="Keyword">import</a> <a id="14302" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14335" class="Keyword">open</a> <a id="14340" class="Keyword">import</a> <a id="14347" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14377" class="Keyword">open</a> <a id="14382" class="Keyword">import</a> <a id="14389" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14413" class="Keyword">open</a> <a id="14418" class="Keyword">import</a> <a id="14425" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14463" class="Keyword">open</a> <a id="14468" class="Keyword">import</a> <a id="14475" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14506" class="Keyword">open</a> <a id="14511" class="Keyword">import</a> <a id="14518" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14543" class="Keyword">open</a> <a id="14548" class="Keyword">import</a> <a id="14555" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14583" class="Keyword">open</a> <a id="14588" class="Keyword">import</a> <a id="14595" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14619" class="Keyword">open</a> <a id="14624" class="Keyword">import</a> <a id="14631" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14657" class="Keyword">open</a> <a id="14662" class="Keyword">import</a> <a id="14669" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14704" class="Keyword">open</a> <a id="14709" class="Keyword">import</a> <a id="14716" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14737" class="Keyword">open</a> <a id="14742" class="Keyword">import</a> <a id="14749" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14798" class="Keyword">open</a> <a id="14803" class="Keyword">import</a> <a id="14810" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14851" class="Keyword">open</a> <a id="14856" class="Keyword">import</a> <a id="14863" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14913" class="Keyword">open</a> <a id="14918" class="Keyword">import</a> <a id="14925" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14971" class="Keyword">open</a> <a id="14976" class="Keyword">import</a> <a id="14983" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15023" class="Keyword">open</a> <a id="15028" class="Keyword">import</a> <a id="15035" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15075" class="Keyword">open</a> <a id="15080" class="Keyword">import</a> <a id="15087" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15137" class="Keyword">open</a> <a id="15142" class="Keyword">import</a> <a id="15149" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15188" class="Keyword">open</a> <a id="15193" class="Keyword">import</a> <a id="15200" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15240" class="Keyword">open</a> <a id="15245" class="Keyword">import</a> <a id="15252" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15285" class="Keyword">open</a> <a id="15290" class="Keyword">import</a> <a id="15297" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15346" class="Keyword">open</a> <a id="15351" class="Keyword">import</a> <a id="15358" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15383" class="Keyword">open</a> <a id="15388" class="Keyword">import</a> <a id="15395" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="15434" class="Keyword">open</a> <a id="15439" class="Keyword">import</a> <a id="15446" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15484" class="Keyword">open</a> <a id="15489" class="Keyword">import</a> <a id="15496" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15518" class="Keyword">open</a> <a id="15523" class="Keyword">import</a> <a id="15530" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15558" class="Keyword">open</a> <a id="15563" class="Keyword">import</a> <a id="15570" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15606" class="Keyword">open</a> <a id="15611" class="Keyword">import</a> <a id="15618" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15644" class="Keyword">open</a> <a id="15649" class="Keyword">import</a> <a id="15656" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15674" class="Keyword">open</a> <a id="15679" class="Keyword">import</a> <a id="15686" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15721" class="Keyword">open</a> <a id="15726" class="Keyword">import</a> <a id="15733" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15768" class="Keyword">open</a> <a id="15773" class="Keyword">import</a> <a id="15780" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15807" class="Keyword">open</a> <a id="15812" class="Keyword">import</a> <a id="15819" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15875" class="Keyword">open</a> <a id="15880" class="Keyword">import</a> <a id="15887" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15916" class="Keyword">open</a> <a id="15921" class="Keyword">import</a> <a id="15928" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15958" class="Keyword">open</a> <a id="15963" class="Keyword">import</a> <a id="15970" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15997" class="Keyword">open</a> <a id="16002" class="Keyword">import</a> <a id="16009" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16035" class="Keyword">open</a> <a id="16040" class="Keyword">import</a> <a id="16047" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16074" class="Keyword">open</a> <a id="16079" class="Keyword">import</a> <a id="16086" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16110" class="Keyword">open</a> <a id="16115" class="Keyword">import</a> <a id="16122" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16145" class="Keyword">open</a> <a id="16150" class="Keyword">import</a> <a id="16157" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16184" class="Keyword">open</a> <a id="16189" class="Keyword">import</a> <a id="16196" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16228" class="Keyword">open</a> <a id="16233" class="Keyword">import</a> <a id="16240" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16275" class="Keyword">open</a> <a id="16280" class="Keyword">import</a> <a id="16287" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16318" class="Keyword">open</a> <a id="16323" class="Keyword">import</a> <a id="16330" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16363" class="Keyword">open</a> <a id="16368" class="Keyword">import</a> <a id="16375" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16409" class="Keyword">open</a> <a id="16414" class="Keyword">import</a> <a id="16421" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16461" class="Keyword">open</a> <a id="16466" class="Keyword">import</a> <a id="16473" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16504" class="Keyword">open</a> <a id="16509" class="Keyword">import</a> <a id="16516" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16548" class="Keyword">open</a> <a id="16553" class="Keyword">import</a> <a id="16560" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16591" class="Keyword">open</a> <a id="16596" class="Keyword">import</a> <a id="16603" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16620" class="Keyword">open</a> <a id="16625" class="Keyword">import</a> <a id="16632" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16657" class="Keyword">open</a> <a id="16662" class="Keyword">import</a> <a id="16669" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16698" class="Keyword">open</a> <a id="16703" class="Keyword">import</a> <a id="16710" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16735" class="Keyword">open</a> <a id="16740" class="Keyword">import</a> <a id="16747" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="16776" class="Keyword">open</a> <a id="16781" class="Keyword">import</a> <a id="16788" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16809" class="Keyword">open</a> <a id="16814" class="Keyword">import</a> <a id="16821" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16845" class="Keyword">open</a> <a id="16850" class="Keyword">import</a> <a id="16857" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16877" class="Keyword">open</a> <a id="16882" class="Keyword">import</a> <a id="16889" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16923" class="Keyword">open</a> <a id="16928" class="Keyword">import</a> <a id="16935" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16973" class="Keyword">open</a> <a id="16978" class="Keyword">import</a> <a id="16985" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17013" class="Keyword">open</a> <a id="17018" class="Keyword">import</a> <a id="17025" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17049" class="Keyword">open</a> <a id="17054" class="Keyword">import</a> <a id="17061" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17088" class="Keyword">open</a> <a id="17093" class="Keyword">import</a> <a id="17100" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17135" class="Keyword">open</a> <a id="17140" class="Keyword">import</a> <a id="17147" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17168" class="Keyword">open</a> <a id="17173" class="Keyword">import</a> <a id="17180" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17216" class="Keyword">open</a> <a id="17221" class="Keyword">import</a> <a id="17228" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17273" class="Keyword">open</a> <a id="17278" class="Keyword">import</a> <a id="17285" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17331" class="Keyword">open</a> <a id="17336" class="Keyword">import</a> <a id="17343" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17383" class="Keyword">open</a> <a id="17388" class="Keyword">import</a> <a id="17395" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17425" class="Keyword">open</a> <a id="17430" class="Keyword">import</a> <a id="17437" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17471" class="Keyword">open</a> <a id="17476" class="Keyword">import</a> <a id="17483" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17520" class="Keyword">open</a> <a id="17525" class="Keyword">import</a> <a id="17532" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17556" class="Keyword">open</a> <a id="17561" class="Keyword">import</a> <a id="17568" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17589" class="Keyword">open</a> <a id="17594" class="Keyword">import</a> <a id="17601" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17636" class="Keyword">open</a> <a id="17641" class="Keyword">import</a> <a id="17648" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17685" class="Keyword">open</a> <a id="17690" class="Keyword">import</a> <a id="17697" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17746" class="Keyword">open</a> <a id="17751" class="Keyword">import</a> <a id="17758" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17791" class="Keyword">open</a> <a id="17796" class="Keyword">import</a> <a id="17803" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17826" class="Keyword">open</a> <a id="17831" class="Keyword">import</a> <a id="17838" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17861" class="Keyword">open</a> <a id="17866" class="Keyword">import</a> <a id="17873" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17896" class="Keyword">open</a> <a id="17901" class="Keyword">import</a> <a id="17908" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17936" class="Keyword">open</a> <a id="17941" class="Keyword">import</a> <a id="17948" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17968" class="Keyword">open</a> <a id="17973" class="Keyword">import</a> <a id="17980" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18001" class="Keyword">open</a> <a id="18006" class="Keyword">import</a> <a id="18013" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18044" class="Keyword">open</a> <a id="18049" class="Keyword">import</a> <a id="18056" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18083" class="Keyword">open</a> <a id="18088" class="Keyword">import</a> <a id="18095" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18111" class="Keyword">open</a> <a id="18116" class="Keyword">import</a> <a id="18123" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18154" class="Keyword">open</a> <a id="18159" class="Keyword">import</a> <a id="18166" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18183" class="Keyword">open</a> <a id="18188" class="Keyword">import</a> <a id="18195" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18217" class="Keyword">open</a> <a id="18222" class="Keyword">import</a> <a id="18229" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18256" class="Keyword">open</a> <a id="18261" class="Keyword">import</a> <a id="18268" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18291" class="Keyword">open</a> <a id="18296" class="Keyword">import</a> <a id="18303" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18330" class="Keyword">open</a> <a id="18335" class="Keyword">import</a> <a id="18342" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18375" class="Keyword">open</a> <a id="18380" class="Keyword">import</a> <a id="18387" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18427" class="Keyword">open</a> <a id="18432" class="Keyword">import</a> <a id="18439" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18460" class="Keyword">open</a> <a id="18465" class="Keyword">import</a> <a id="18472" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18501" class="Keyword">open</a> <a id="18506" class="Keyword">import</a> <a id="18513" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18551" class="Keyword">open</a> <a id="18556" class="Keyword">import</a> <a id="18563" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18583" class="Keyword">open</a> <a id="18588" class="Keyword">import</a> <a id="18595" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18619" class="Keyword">open</a> <a id="18624" class="Keyword">import</a> <a id="18631" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18658" class="Keyword">open</a> <a id="18663" class="Keyword">import</a> <a id="18670" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18702" class="Keyword">open</a> <a id="18707" class="Keyword">import</a> <a id="18714" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18744" class="Keyword">open</a> <a id="18749" class="Keyword">import</a> <a id="18756" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18782" class="Keyword">open</a> <a id="18787" class="Keyword">import</a> <a id="18794" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18821" class="Keyword">open</a> <a id="18826" class="Keyword">import</a> <a id="18833" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="18870" class="Keyword">open</a> <a id="18875" class="Keyword">import</a> <a id="18882" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18911" class="Keyword">open</a> <a id="18916" class="Keyword">import</a> <a id="18923" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18946" class="Keyword">open</a> <a id="18951" class="Keyword">import</a> <a id="18958" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19009" class="Keyword">open</a> <a id="19014" class="Keyword">import</a> <a id="19021" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19064" class="Keyword">open</a> <a id="19069" class="Keyword">import</a> <a id="19076" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19128" class="Keyword">open</a> <a id="19133" class="Keyword">import</a> <a id="19140" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19188" class="Keyword">open</a> <a id="19193" class="Keyword">import</a> <a id="19200" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19238" class="Keyword">open</a> <a id="19243" class="Keyword">import</a> <a id="19250" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19287" class="Keyword">open</a> <a id="19292" class="Keyword">import</a> <a id="19299" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19345" class="Keyword">open</a> <a id="19350" class="Keyword">import</a> <a id="19357" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19374" class="Keyword">open</a> <a id="19379" class="Keyword">import</a> <a id="19386" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19414" class="Keyword">open</a> <a id="19419" class="Keyword">import</a> <a id="19426" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19454" class="Keyword">open</a> <a id="19459" class="Keyword">import</a> <a id="19466" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19502" class="Keyword">open</a> <a id="19507" class="Keyword">import</a> <a id="19514" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19552" class="Keyword">open</a> <a id="19557" class="Keyword">import</a> <a id="19564" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19597" class="Keyword">open</a> <a id="19602" class="Keyword">import</a> <a id="19609" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19630" class="Keyword">open</a> <a id="19635" class="Keyword">import</a> <a id="19642" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19678" class="Keyword">open</a> <a id="19683" class="Keyword">import</a> <a id="19690" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19744" class="Keyword">open</a> <a id="19749" class="Keyword">import</a> <a id="19756" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19778" class="Keyword">open</a> <a id="19783" class="Keyword">import</a> <a id="19790" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19825" class="Keyword">open</a> <a id="19830" class="Keyword">import</a> <a id="19837" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19867" class="Keyword">open</a> <a id="19872" class="Keyword">import</a> <a id="19879" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19918" class="Keyword">open</a> <a id="19923" class="Keyword">import</a> <a id="19930" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19984" class="Keyword">open</a> <a id="19989" class="Keyword">import</a> <a id="19996" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20042" class="Keyword">open</a> <a id="20047" class="Keyword">import</a> <a id="20054" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20105" class="Keyword">open</a> <a id="20110" class="Keyword">import</a> <a id="20117" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20158" class="Keyword">open</a> <a id="20163" class="Keyword">import</a> <a id="20170" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20215" class="Keyword">open</a> <a id="20220" class="Keyword">import</a> <a id="20227" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20272" class="Keyword">open</a> <a id="20277" class="Keyword">import</a> <a id="20284" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20320" class="Keyword">open</a> <a id="20325" class="Keyword">import</a> <a id="20332" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20368" class="Keyword">open</a> <a id="20373" class="Keyword">import</a> <a id="20380" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20445" class="Keyword">open</a> <a id="20450" class="Keyword">import</a> <a id="20457" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20512" class="Keyword">open</a> <a id="20517" class="Keyword">import</a> <a id="20524" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20564" class="Keyword">open</a> <a id="20569" class="Keyword">import</a> <a id="20576" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20620" class="Keyword">open</a> <a id="20625" class="Keyword">import</a> <a id="20632" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20677" class="Keyword">open</a> <a id="20682" class="Keyword">import</a> <a id="20689" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20730" class="Keyword">open</a> <a id="20735" class="Keyword">import</a> <a id="20742" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20782" class="Keyword">open</a> <a id="20787" class="Keyword">import</a> <a id="20794" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20821" class="Keyword">open</a> <a id="20826" class="Keyword">import</a> <a id="20833" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20869" class="Keyword">open</a> <a id="20874" class="Keyword">import</a> <a id="20881" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20908" class="Keyword">open</a> <a id="20913" class="Keyword">import</a> <a id="20920" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20957" class="Keyword">open</a> <a id="20962" class="Keyword">import</a> <a id="20969" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20997" class="Keyword">open</a> <a id="21002" class="Keyword">import</a> <a id="21009" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21028" class="Keyword">open</a> <a id="21033" class="Keyword">import</a> <a id="21040" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21080" class="Keyword">open</a> <a id="21085" class="Keyword">import</a> <a id="21092" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21124" class="Keyword">open</a> <a id="21129" class="Keyword">import</a> <a id="21136" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21184" class="Keyword">open</a> <a id="21189" class="Keyword">import</a> <a id="21196" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21219" class="Keyword">open</a> <a id="21224" class="Keyword">import</a> <a id="21231" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21255" class="Keyword">open</a> <a id="21260" class="Keyword">import</a> <a id="21267" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21307" class="Keyword">open</a> <a id="21312" class="Keyword">import</a> <a id="21319" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="21362" class="Keyword">open</a> <a id="21367" class="Keyword">import</a> <a id="21374" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21408" class="Keyword">open</a> <a id="21413" class="Keyword">import</a> <a id="21420" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21452" class="Keyword">open</a> <a id="21457" class="Keyword">import</a> <a id="21464" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21494" class="Keyword">open</a> <a id="21499" class="Keyword">import</a> <a id="21506" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21540" class="Keyword">open</a> <a id="21545" class="Keyword">import</a> <a id="21552" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21587" class="Keyword">open</a> <a id="21592" class="Keyword">import</a> <a id="21599" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="21623" class="Keyword">open</a> <a id="21628" class="Keyword">import</a> <a id="21635" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21672" class="Keyword">open</a> <a id="21677" class="Keyword">import</a> <a id="21684" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21711" class="Keyword">open</a> <a id="21716" class="Keyword">import</a> <a id="21723" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21751" class="Keyword">open</a> <a id="21756" class="Keyword">import</a> <a id="21763" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21812" class="Keyword">open</a> <a id="21817" class="Keyword">import</a> <a id="21824" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21870" class="Keyword">open</a> <a id="21875" class="Keyword">import</a> <a id="21882" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21922" class="Keyword">open</a> <a id="21927" class="Keyword">import</a> <a id="21934" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21972" class="Keyword">open</a> <a id="21977" class="Keyword">import</a> <a id="21984" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22013" class="Keyword">open</a> <a id="22018" class="Keyword">import</a> <a id="22025" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22055" class="Keyword">open</a> <a id="22060" class="Keyword">import</a> <a id="22067" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22098" class="Keyword">open</a> <a id="22103" class="Keyword">import</a> <a id="22110" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="22150" class="Keyword">open</a> <a id="22155" class="Keyword">import</a> <a id="22162" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22188" class="Keyword">open</a> <a id="22193" class="Keyword">import</a> <a id="22200" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="22255" class="Keyword">open</a> <a id="22260" class="Keyword">import</a> <a id="22267" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="22318" class="Keyword">open</a> <a id="22323" class="Keyword">import</a> <a id="22330" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="22375" class="Keyword">open</a> <a id="22380" class="Keyword">import</a> <a id="22387" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="22432" class="Keyword">open</a> <a id="22437" class="Keyword">import</a> <a id="22444" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22498" class="Keyword">open</a> <a id="22503" class="Keyword">import</a> <a id="22510" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22537" class="Keyword">open</a> <a id="22542" class="Keyword">import</a> <a id="22549" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22582" class="Keyword">open</a> <a id="22587" class="Keyword">import</a> <a id="22594" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22625" class="Keyword">open</a> <a id="22630" class="Keyword">import</a> <a id="22637" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22674" class="Keyword">open</a> <a id="22679" class="Keyword">import</a> <a id="22686" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="22720" class="Keyword">open</a> <a id="22725" class="Keyword">import</a> <a id="22732" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22757" class="Keyword">open</a> <a id="22762" class="Keyword">import</a> <a id="22769" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22801" class="Keyword">open</a> <a id="22806" class="Keyword">import</a> <a id="22813" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22848" class="Keyword">open</a> <a id="22853" class="Keyword">import</a> <a id="22860" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22889" class="Keyword">open</a> <a id="22894" class="Keyword">import</a> <a id="22901" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22927" class="Keyword">open</a> <a id="22932" class="Keyword">import</a> <a id="22939" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22967" class="Keyword">open</a> <a id="22972" class="Keyword">import</a> <a id="22979" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23004" class="Keyword">open</a> <a id="23009" class="Keyword">import</a> <a id="23016" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23037" class="Keyword">open</a> <a id="23042" class="Keyword">import</a> <a id="23049" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23085" class="Keyword">open</a> <a id="23090" class="Keyword">import</a> <a id="23097" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="23140" class="Keyword">open</a> <a id="23145" class="Keyword">import</a> <a id="23152" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23177" class="Keyword">open</a> <a id="23182" class="Keyword">import</a> <a id="23189" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23220" class="Keyword">open</a> <a id="23225" class="Keyword">import</a> <a id="23232" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="23264" class="Keyword">open</a> <a id="23269" class="Keyword">import</a> <a id="23276" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="23310" class="Keyword">open</a> <a id="23315" class="Keyword">import</a> <a id="23322" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="23378" class="Keyword">open</a> <a id="23383" class="Keyword">import</a> <a id="23390" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="23443" class="Keyword">open</a> <a id="23448" class="Keyword">import</a> <a id="23455" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="23482" class="Keyword">open</a> <a id="23487" class="Keyword">import</a> <a id="23494" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23539" class="Keyword">open</a> <a id="23544" class="Keyword">import</a> <a id="23551" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23613" class="Keyword">open</a> <a id="23618" class="Keyword">import</a> <a id="23625" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23638" class="Keyword">open</a> <a id="23643" class="Keyword">import</a> <a id="23650" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23690" class="Keyword">open</a> <a id="23695" class="Keyword">import</a> <a id="23702" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23746" class="Keyword">open</a> <a id="23751" class="Keyword">import</a> <a id="23758" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23797" class="Keyword">open</a> <a id="23802" class="Keyword">import</a> <a id="23809" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23851" class="Keyword">open</a> <a id="23856" class="Keyword">import</a> <a id="23863" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23903" class="Keyword">open</a> <a id="23908" class="Keyword">import</a> <a id="23915" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23956" class="Keyword">open</a> <a id="23961" class="Keyword">import</a> <a id="23968" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24006" class="Keyword">open</a> <a id="24011" class="Keyword">import</a> <a id="24018" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24081" class="Keyword">open</a> <a id="24086" class="Keyword">import</a> <a id="24093" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="24122" class="Keyword">open</a> <a id="24127" class="Keyword">import</a> <a id="24134" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24179" class="Keyword">open</a> <a id="24184" class="Keyword">import</a> <a id="24191" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24233" class="Keyword">open</a> <a id="24238" class="Keyword">import</a> <a id="24245" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="24289" class="Keyword">open</a> <a id="24294" class="Keyword">import</a> <a id="24301" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="24350" class="Keyword">open</a> <a id="24355" class="Keyword">import</a> <a id="24362" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="24412" class="Keyword">open</a> <a id="24417" class="Keyword">import</a> <a id="24424" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="24451" class="Keyword">open</a> <a id="24456" class="Keyword">import</a> <a id="24463" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="24488" class="Keyword">open</a> <a id="24493" class="Keyword">import</a> <a id="24500" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24541" class="Keyword">open</a> <a id="24546" class="Keyword">import</a> <a id="24553" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24576" class="Keyword">open</a> <a id="24581" class="Keyword">import</a> <a id="24588" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24637" class="Keyword">open</a> <a id="24642" class="Keyword">import</a> <a id="24649" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24688" class="Keyword">open</a> <a id="24693" class="Keyword">import</a> <a id="24700" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24741" class="Keyword">open</a> <a id="24746" class="Keyword">import</a> <a id="24753" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24797" class="Keyword">open</a> <a id="24802" class="Keyword">import</a> <a id="24809" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24846" class="Keyword">open</a> <a id="24851" class="Keyword">import</a> <a id="24858" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24880" class="Keyword">open</a> <a id="24885" class="Keyword">import</a> <a id="24892" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24922" class="Keyword">open</a> <a id="24927" class="Keyword">import</a> <a id="24934" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24973" class="Keyword">open</a> <a id="24978" class="Keyword">import</a> <a id="24985" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25023" class="Keyword">open</a> <a id="25028" class="Keyword">import</a> <a id="25035" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="25093" class="Keyword">open</a> <a id="25098" class="Keyword">import</a> <a id="25105" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="25170" class="Keyword">open</a> <a id="25175" class="Keyword">import</a> <a id="25182" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="25213" class="Keyword">open</a> <a id="25218" class="Keyword">import</a> <a id="25225" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="25252" class="Keyword">open</a> <a id="25257" class="Keyword">import</a> <a id="25264" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="25322" class="Keyword">open</a> <a id="25327" class="Keyword">import</a> <a id="25334" href="group-theory.html" class="Module">group-theory</a>
<a id="25347" class="Keyword">open</a> <a id="25352" class="Keyword">import</a> <a id="25359" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="25387" class="Keyword">open</a> <a id="25392" class="Keyword">import</a> <a id="25399" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25450" class="Keyword">open</a> <a id="25455" class="Keyword">import</a> <a id="25462" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25495" class="Keyword">open</a> <a id="25500" class="Keyword">import</a> <a id="25507" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="25554" class="Keyword">open</a> <a id="25559" class="Keyword">import</a> <a id="25566" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="25605" class="Keyword">open</a> <a id="25610" class="Keyword">import</a> <a id="25617" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25657" class="Keyword">open</a> <a id="25662" class="Keyword">import</a> <a id="25669" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25712" class="Keyword">open</a> <a id="25717" class="Keyword">import</a> <a id="25724" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25756" class="Keyword">open</a> <a id="25761" class="Keyword">import</a> <a id="25768" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25804" class="Keyword">open</a> <a id="25809" class="Keyword">import</a> <a id="25816" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25845" class="Keyword">open</a> <a id="25850" class="Keyword">import</a> <a id="25857" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25885" class="Keyword">open</a> <a id="25890" class="Keyword">import</a> <a id="25897" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25930" class="Keyword">open</a> <a id="25935" class="Keyword">import</a> <a id="25942" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25978" class="Keyword">open</a> <a id="25983" class="Keyword">import</a> <a id="25990" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="26019" class="Keyword">open</a> <a id="26024" class="Keyword">import</a> <a id="26031" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="26056" class="Keyword">open</a> <a id="26061" class="Keyword">import</a> <a id="26068" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="26130" class="Keyword">open</a> <a id="26135" class="Keyword">import</a> <a id="26142" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="26173" class="Keyword">open</a> <a id="26178" class="Keyword">import</a> <a id="26185" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="26232" class="Keyword">open</a> <a id="26237" class="Keyword">import</a> <a id="26244" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="26277" class="Keyword">open</a> <a id="26282" class="Keyword">import</a> <a id="26289" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="26338" class="Keyword">open</a> <a id="26343" class="Keyword">import</a> <a id="26350" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="26390" class="Keyword">open</a> <a id="26395" class="Keyword">import</a> <a id="26402" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="26439" class="Keyword">open</a> <a id="26444" class="Keyword">import</a> <a id="26451" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="26498" class="Keyword">open</a> <a id="26503" class="Keyword">import</a> <a id="26510" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="26551" class="Keyword">open</a> <a id="26556" class="Keyword">import</a> <a id="26563" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="26602" class="Keyword">open</a> <a id="26607" class="Keyword">import</a> <a id="26614" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="26646" class="Keyword">open</a> <a id="26651" class="Keyword">import</a> <a id="26658" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="26685" class="Keyword">open</a> <a id="26690" class="Keyword">import</a> <a id="26697" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26717" class="Keyword">open</a> <a id="26722" class="Keyword">import</a> <a id="26729" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26763" class="Keyword">open</a> <a id="26768" class="Keyword">import</a> <a id="26775" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26802" class="Keyword">open</a> <a id="26807" class="Keyword">import</a> <a id="26814" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26856" class="Keyword">open</a> <a id="26861" class="Keyword">import</a> <a id="26868" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26918" class="Keyword">open</a> <a id="26923" class="Keyword">import</a> <a id="26930" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26977" class="Keyword">open</a> <a id="26982" class="Keyword">import</a> <a id="26989" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="27030" class="Keyword">open</a> <a id="27035" class="Keyword">import</a> <a id="27042" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="27076" class="Keyword">open</a> <a id="27081" class="Keyword">import</a> <a id="27088" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="27129" class="Keyword">open</a> <a id="27134" class="Keyword">import</a> <a id="27141" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="27176" class="Keyword">open</a> <a id="27181" class="Keyword">import</a> <a id="27188" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="27226" class="Keyword">open</a> <a id="27231" class="Keyword">import</a> <a id="27238" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="27273" class="Keyword">open</a> <a id="27278" class="Keyword">import</a> <a id="27285" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="27317" class="Keyword">open</a> <a id="27322" class="Keyword">import</a> <a id="27329" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="27370" class="Keyword">open</a> <a id="27375" class="Keyword">import</a> <a id="27382" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="27423" class="Keyword">open</a> <a id="27428" class="Keyword">import</a> <a id="27435" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="27475" class="Keyword">open</a> <a id="27480" class="Keyword">import</a> <a id="27487" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="27520" class="Keyword">open</a> <a id="27525" class="Keyword">import</a> <a id="27532" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="27569" class="Keyword">open</a> <a id="27574" class="Keyword">import</a> <a id="27581" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="27611" class="Keyword">open</a> <a id="27616" class="Keyword">import</a> <a id="27623" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="27644" class="Keyword">open</a> <a id="27649" class="Keyword">import</a> <a id="27656" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="27710" class="Keyword">open</a> <a id="27715" class="Keyword">import</a> <a id="27722" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27767" class="Keyword">open</a> <a id="27772" class="Keyword">import</a> <a id="27779" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27807" class="Keyword">open</a> <a id="27812" class="Keyword">import</a> <a id="27819" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27840" class="Keyword">open</a> <a id="27845" class="Keyword">import</a> <a id="27852" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27895" class="Keyword">open</a> <a id="27900" class="Keyword">import</a> <a id="27907" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27941" class="Keyword">open</a> <a id="27946" class="Keyword">import</a> <a id="27953" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27983" class="Keyword">open</a> <a id="27988" class="Keyword">import</a> <a id="27995" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="28041" class="Keyword">open</a> <a id="28046" class="Keyword">import</a> <a id="28053" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="28107" class="Keyword">open</a> <a id="28112" class="Keyword">import</a> <a id="28119" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="28162" class="Keyword">open</a> <a id="28167" class="Keyword">import</a> <a id="28174" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="28208" class="Keyword">open</a> <a id="28213" class="Keyword">import</a> <a id="28220" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="28261" class="Keyword">open</a> <a id="28266" class="Keyword">import</a> <a id="28273" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="28308" class="Keyword">open</a> <a id="28313" class="Keyword">import</a> <a id="28320" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="28362" class="Keyword">open</a> <a id="28367" class="Keyword">import</a> <a id="28374" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="28409" class="Keyword">open</a> <a id="28414" class="Keyword">import</a> <a id="28421" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="28460" class="Keyword">open</a> <a id="28465" class="Keyword">import</a> <a id="28472" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="28509" class="Keyword">open</a> <a id="28514" class="Keyword">import</a> <a id="28521" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="28568" class="Keyword">open</a> <a id="28573" class="Keyword">import</a> <a id="28580" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="28644" class="Keyword">open</a> <a id="28649" class="Keyword">import</a> <a id="28656" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="28701" class="Keyword">open</a> <a id="28706" class="Keyword">import</a> <a id="28713" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="28737" class="Keyword">open</a> <a id="28742" class="Keyword">import</a> <a id="28749" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="28774" class="Keyword">open</a> <a id="28779" class="Keyword">import</a> <a id="28786" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28829" class="Keyword">open</a> <a id="28834" class="Keyword">import</a> <a id="28841" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28872" class="Keyword">open</a> <a id="28877" class="Keyword">import</a> <a id="28884" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28938" class="Keyword">open</a> <a id="28943" class="Keyword">import</a> <a id="28950" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28973" class="Keyword">open</a> <a id="28978" class="Keyword">import</a> <a id="28985" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="29023" class="Keyword">open</a> <a id="29028" class="Keyword">import</a> <a id="29035" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="29074" class="Keyword">open</a> <a id="29079" class="Keyword">import</a> <a id="29086" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="29137" class="Keyword">open</a> <a id="29142" class="Keyword">import</a> <a id="29149" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="29186" class="Keyword">open</a> <a id="29191" class="Keyword">import</a> <a id="29198" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="29255" class="Keyword">open</a> <a id="29260" class="Keyword">import</a> <a id="29267" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="29315" class="Keyword">open</a> <a id="29320" class="Keyword">import</a> <a id="29327" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="29357" class="Keyword">open</a> <a id="29362" class="Keyword">import</a> <a id="29369" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="29406" class="Keyword">open</a> <a id="29411" class="Keyword">import</a> <a id="29418" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="29439" class="Keyword">open</a> <a id="29444" class="Keyword">import</a> <a id="29451" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="29498" class="Keyword">open</a> <a id="29503" class="Keyword">import</a> <a id="29510" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="29548" class="Keyword">open</a> <a id="29553" class="Keyword">import</a> <a id="29560" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="29654" class="Keyword">open</a> <a id="29659" class="Keyword">import</a> <a id="29666" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="29681" class="Keyword">open</a> <a id="29686" class="Keyword">import</a> <a id="29693" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="29726" class="Keyword">open</a> <a id="29731" class="Keyword">import</a> <a id="29738" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="29770" class="Keyword">open</a> <a id="29775" class="Keyword">import</a> <a id="29782" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29824" class="Keyword">open</a> <a id="29829" class="Keyword">import</a> <a id="29836" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29874" class="Keyword">open</a> <a id="29879" class="Keyword">import</a> <a id="29886" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29923" class="Keyword">open</a> <a id="29928" class="Keyword">import</a> <a id="29935" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29968" class="Keyword">open</a> <a id="29973" class="Keyword">import</a> <a id="29980" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="30004" class="Keyword">open</a> <a id="30009" class="Keyword">import</a> <a id="30016" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="30055" class="Keyword">open</a> <a id="30060" class="Keyword">import</a> <a id="30067" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="30113" class="Keyword">open</a> <a id="30118" class="Keyword">import</a> <a id="30125" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="30170" class="Keyword">open</a> <a id="30175" class="Keyword">import</a> <a id="30182" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="30220" class="Keyword">open</a> <a id="30225" class="Keyword">import</a> <a id="30232" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="30264" class="Keyword">open</a> <a id="30269" class="Keyword">import</a> <a id="30276" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="30329" class="Keyword">open</a> <a id="30334" class="Keyword">import</a> <a id="30341" href="order-theory.html" class="Module">order-theory</a>
<a id="30354" class="Keyword">open</a> <a id="30359" class="Keyword">import</a> <a id="30366" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="30393" class="Keyword">open</a> <a id="30398" class="Keyword">import</a> <a id="30405" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="30435" class="Keyword">open</a> <a id="30440" class="Keyword">import</a> <a id="30447" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="30480" class="Keyword">open</a> <a id="30485" class="Keyword">import</a> <a id="30492" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="30528" class="Keyword">open</a> <a id="30533" class="Keyword">import</a> <a id="30540" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="30575" class="Keyword">open</a> <a id="30580" class="Keyword">import</a> <a id="30587" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="30614" class="Keyword">open</a> <a id="30619" class="Keyword">import</a> <a id="30626" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="30656" class="Keyword">open</a> <a id="30661" class="Keyword">import</a> <a id="30668" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="30704" class="Keyword">open</a> <a id="30709" class="Keyword">import</a> <a id="30716" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="30758" class="Keyword">open</a> <a id="30763" class="Keyword">import</a> <a id="30770" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="30802" class="Keyword">open</a> <a id="30807" class="Keyword">import</a> <a id="30814" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30845" class="Keyword">open</a> <a id="30850" class="Keyword">import</a> <a id="30857" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30883" class="Keyword">open</a> <a id="30888" class="Keyword">import</a> <a id="30895" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30924" class="Keyword">open</a> <a id="30929" class="Keyword">import</a> <a id="30936" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30973" class="Keyword">open</a> <a id="30978" class="Keyword">import</a> <a id="30985" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="31025" class="Keyword">open</a> <a id="31030" class="Keyword">import</a> <a id="31037" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="31059" class="Keyword">open</a> <a id="31064" class="Keyword">import</a> <a id="31071" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="31106" class="Keyword">open</a> <a id="31111" class="Keyword">import</a> <a id="31118" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="31156" class="Keyword">open</a> <a id="31161" class="Keyword">import</a> <a id="31168" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="31207" class="Keyword">open</a> <a id="31212" class="Keyword">import</a> <a id="31219" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="31254" class="Keyword">open</a> <a id="31259" class="Keyword">import</a> <a id="31266" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="31301" class="Keyword">open</a> <a id="31306" class="Keyword">import</a> <a id="31313" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="31351" class="Keyword">open</a> <a id="31356" class="Keyword">import</a> <a id="31363" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="31394" class="Keyword">open</a> <a id="31399" class="Keyword">import</a> <a id="31406" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="31448" class="Keyword">open</a> <a id="31453" class="Keyword">import</a> <a id="31460" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="31505" class="Keyword">open</a> <a id="31510" class="Keyword">import</a> <a id="31517" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="31550" class="Keyword">open</a> <a id="31555" class="Keyword">import</a> <a id="31562" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="31582" class="Keyword">open</a> <a id="31587" class="Keyword">import</a> <a id="31594" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="31617" class="Keyword">open</a> <a id="31622" class="Keyword">import</a> <a id="31629" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="31652" class="Keyword">open</a> <a id="31657" class="Keyword">import</a> <a id="31664" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="31690" class="Keyword">open</a> <a id="31695" class="Keyword">import</a> <a id="31702" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="31728" class="Keyword">open</a> <a id="31733" class="Keyword">import</a> <a id="31740" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="31804" class="Keyword">open</a> <a id="31809" class="Keyword">import</a> <a id="31816" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31834" class="Keyword">open</a> <a id="31839" class="Keyword">import</a> <a id="31846" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31873" class="Keyword">open</a> <a id="31878" class="Keyword">import</a> <a id="31885" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31911" class="Keyword">open</a> <a id="31916" class="Keyword">import</a> <a id="31923" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31949" class="Keyword">open</a> <a id="31954" class="Keyword">import</a> <a id="31961" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31987" class="Keyword">open</a> <a id="31992" class="Keyword">import</a> <a id="31999" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="32030" class="Keyword">open</a> <a id="32035" class="Keyword">import</a> <a id="32042" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="32105" class="Keyword">open</a> <a id="32110" class="Keyword">import</a> <a id="32117" href="polytopes.html" class="Module">polytopes</a>
<a id="32127" class="Keyword">open</a> <a id="32132" class="Keyword">import</a> <a id="32139" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="32197" class="Keyword">open</a> <a id="32202" class="Keyword">import</a> <a id="32209" href="ring-theory.html" class="Module">ring-theory</a>
<a id="32221" class="Keyword">open</a> <a id="32226" class="Keyword">import</a> <a id="32233" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="32270" class="Keyword">open</a> <a id="32275" class="Keyword">import</a> <a id="32282" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="32309" class="Keyword">open</a> <a id="32314" class="Keyword">import</a> <a id="32321" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="32353" class="Keyword">open</a> <a id="32358" class="Keyword">import</a> <a id="32365" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="32411" class="Keyword">open</a> <a id="32416" class="Keyword">import</a> <a id="32423" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="32448" class="Keyword">open</a> <a id="32453" class="Keyword">import</a> <a id="32460" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="32503" class="Keyword">open</a> <a id="32508" class="Keyword">import</a> <a id="32515" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="32553" class="Keyword">open</a> <a id="32558" class="Keyword">import</a> <a id="32565" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="32596" class="Keyword">open</a> <a id="32601" class="Keyword">import</a> <a id="32608" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="32632" class="Keyword">open</a> <a id="32637" class="Keyword">import</a> <a id="32644" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="32676" class="Keyword">open</a> <a id="32681" class="Keyword">import</a> <a id="32688" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="32714" class="Keyword">open</a> <a id="32719" class="Keyword">import</a> <a id="32726" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="32755" class="Keyword">open</a> <a id="32760" class="Keyword">import</a> <a id="32767" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="32804" class="Keyword">open</a> <a id="32809" class="Keyword">import</a> <a id="32816" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32845" class="Keyword">open</a> <a id="32850" class="Keyword">import</a> <a id="32857" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32884" class="Keyword">open</a> <a id="32889" class="Keyword">import</a> <a id="32896" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32933" class="Keyword">open</a> <a id="32938" class="Keyword">import</a> <a id="32945" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32972" class="Keyword">open</a> <a id="32977" class="Keyword">import</a> <a id="32984" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="33017" class="Keyword">open</a> <a id="33022" class="Keyword">import</a> <a id="33029" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="33047" class="Keyword">open</a> <a id="33052" class="Keyword">import</a> <a id="33059" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="33113" class="Keyword">open</a> <a id="33118" class="Keyword">import</a> <a id="33125" href="set-theory.html" class="Module">set-theory</a>
<a id="33136" class="Keyword">open</a> <a id="33141" class="Keyword">import</a> <a id="33148" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="33171" class="Keyword">open</a> <a id="33176" class="Keyword">import</a> <a id="33183" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="33207" class="Keyword">open</a> <a id="33212" class="Keyword">import</a> <a id="33219" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="33245" class="Keyword">open</a> <a id="33250" class="Keyword">import</a> <a id="33257" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="33319" class="Keyword">open</a> <a id="33324" class="Keyword">import</a> <a id="33331" href="structured-types.html" class="Module">structured-types</a>
<a id="33348" class="Keyword">open</a> <a id="33353" class="Keyword">import</a> <a id="33360" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="33395" class="Keyword">open</a> <a id="33400" class="Keyword">import</a> <a id="33407" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="33451" class="Keyword">open</a> <a id="33456" class="Keyword">import</a> <a id="33463" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="33527" class="Keyword">open</a> <a id="33532" class="Keyword">import</a> <a id="33539" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="33578" class="Keyword">open</a> <a id="33583" class="Keyword">import</a> <a id="33590" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="33636" class="Keyword">open</a> <a id="33641" class="Keyword">import</a> <a id="33648" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="33672" class="Keyword">open</a> <a id="33677" class="Keyword">import</a> <a id="33684" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="33753" class="Keyword">open</a> <a id="33758" class="Keyword">import</a> <a id="33765" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="33810" class="Keyword">open</a> <a id="33815" class="Keyword">import</a> <a id="33822" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33856" class="Keyword">open</a> <a id="33861" class="Keyword">import</a> <a id="33868" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33929" class="Keyword">open</a> <a id="33934" class="Keyword">import</a> <a id="33941" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33986" class="Keyword">open</a> <a id="33991" class="Keyword">import</a> <a id="33998" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="34036" class="Keyword">open</a> <a id="34041" class="Keyword">import</a> <a id="34048" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="34091" class="Keyword">open</a> <a id="34096" class="Keyword">import</a> <a id="34103" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="34139" class="Keyword">open</a> <a id="34144" class="Keyword">import</a> <a id="34151" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="34181" class="Keyword">open</a> <a id="34186" class="Keyword">import</a> <a id="34193" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="34224" class="Keyword">open</a> <a id="34229" class="Keyword">import</a> <a id="34236" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="34295" class="Keyword">open</a> <a id="34300" class="Keyword">import</a> <a id="34307" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="34358" class="Keyword">open</a> <a id="34363" class="Keyword">import</a> <a id="34370" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="34421" class="Keyword">open</a> <a id="34426" class="Keyword">import</a> <a id="34433" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="34488" class="Keyword">open</a> <a id="34493" class="Keyword">import</a> <a id="34500" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="34529" class="Keyword">open</a> <a id="34534" class="Keyword">import</a> <a id="34541" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="34569" class="Keyword">open</a> <a id="34574" class="Keyword">import</a> <a id="34581" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="34611" class="Keyword">open</a> <a id="34616" class="Keyword">import</a> <a id="34623" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="34657" class="Keyword">open</a> <a id="34662" class="Keyword">import</a> <a id="34669" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="34745" class="Keyword">open</a> <a id="34750" class="Keyword">import</a> <a id="34757" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="34783" class="Keyword">open</a> <a id="34788" class="Keyword">import</a> <a id="34795" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34833" class="Keyword">open</a> <a id="34838" class="Keyword">import</a> <a id="34845" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34891" class="Keyword">open</a> <a id="34896" class="Keyword">import</a> <a id="34903" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34940" class="Keyword">open</a> <a id="34945" class="Keyword">import</a> <a id="34952" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34992" class="Keyword">open</a> <a id="34997" class="Keyword">import</a> <a id="35004" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="35043" class="Keyword">open</a> <a id="35048" class="Keyword">import</a> <a id="35055" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="35088" class="Keyword">open</a> <a id="35093" class="Keyword">import</a> <a id="35100" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="35135" class="Keyword">open</a> <a id="35140" class="Keyword">import</a> <a id="35147" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="35192" class="Keyword">open</a> <a id="35197" class="Keyword">import</a> <a id="35204" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="35256" class="Keyword">open</a> <a id="35261" class="Keyword">import</a> <a id="35268" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="35321" class="Keyword">open</a> <a id="35326" class="Keyword">import</a> <a id="35333" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="35393" class="Keyword">open</a> <a id="35398" class="Keyword">import</a> <a id="35405" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="35453" class="Keyword">open</a> <a id="35458" class="Keyword">import</a> <a id="35465" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="35505" class="Keyword">open</a> <a id="35510" class="Keyword">import</a> <a id="35517" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="35564" class="Keyword">open</a> <a id="35569" class="Keyword">import</a> <a id="35576" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="35617" class="Keyword">open</a> <a id="35622" class="Keyword">import</a> <a id="35629" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="35667" class="Keyword">open</a> <a id="35672" class="Keyword">import</a> <a id="35679" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="35727" class="Keyword">open</a> <a id="35732" class="Keyword">import</a> <a id="35739" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35776" class="Keyword">open</a> <a id="35781" class="Keyword">import</a> <a id="35788" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35822" class="Keyword">open</a> <a id="35827" class="Keyword">import</a> <a id="35834" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35881" class="Keyword">open</a> <a id="35886" class="Keyword">import</a> <a id="35893" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35938" class="Keyword">open</a> <a id="35943" class="Keyword">import</a> <a id="35950" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35999" class="Keyword">open</a> <a id="36004" class="Keyword">import</a> <a id="36011" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="36088" class="Keyword">open</a> <a id="36093" class="Keyword">import</a> <a id="36100" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="36152" class="Keyword">open</a> <a id="36157" class="Keyword">import</a> <a id="36164" href="type-theories.html" class="Module">type-theories</a>
<a id="36178" class="Keyword">open</a> <a id="36183" class="Keyword">import</a> <a id="36190" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="36232" class="Keyword">open</a> <a id="36237" class="Keyword">import</a> <a id="36244" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="36282" class="Keyword">open</a> <a id="36287" class="Keyword">import</a> <a id="36294" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="36340" class="Keyword">open</a> <a id="36345" class="Keyword">import</a> <a id="36352" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="36399" class="Keyword">open</a> <a id="36404" class="Keyword">import</a> <a id="36411" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="36446" class="Keyword">open</a> <a id="36451" class="Keyword">import</a> <a id="36458" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="36536" class="Keyword">open</a> <a id="36541" class="Keyword">import</a> <a id="36548" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="36572" class="Keyword">open</a> <a id="36577" class="Keyword">import</a> <a id="36584" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="36637" class="Keyword">open</a> <a id="36642" class="Keyword">import</a> <a id="36649" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="36692" class="Keyword">open</a> <a id="36697" class="Keyword">import</a> <a id="36704" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="36744" class="Keyword">open</a> <a id="36749" class="Keyword">import</a> <a id="36756" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36795" class="Keyword">open</a> <a id="36800" class="Keyword">import</a> <a id="36807" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36841" class="Keyword">open</a> <a id="36846" class="Keyword">import</a> <a id="36853" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36901" class="Keyword">open</a> <a id="36906" class="Keyword">import</a> <a id="36913" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36964" class="Keyword">open</a> <a id="36969" class="Keyword">import</a> <a id="36976" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="37023" class="Keyword">open</a> <a id="37028" class="Keyword">import</a> <a id="37035" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="37087" class="Keyword">open</a> <a id="37092" class="Keyword">import</a> <a id="37099" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="37143" class="Keyword">open</a> <a id="37148" class="Keyword">import</a> <a id="37155" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="37195" class="Keyword">open</a> <a id="37200" class="Keyword">import</a> <a id="37207" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="37250" class="Keyword">open</a> <a id="37255" class="Keyword">import</a> <a id="37262" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="37314" class="Keyword">open</a> <a id="37319" class="Keyword">import</a> <a id="37326" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="37380" class="Keyword">open</a> <a id="37385" class="Keyword">import</a> <a id="37392" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="37440" class="Keyword">open</a> <a id="37445" class="Keyword">import</a> <a id="37452" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="37491" class="Keyword">open</a> <a id="37496" class="Keyword">import</a> <a id="37503" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="37536" class="Keyword">open</a> <a id="37541" class="Keyword">import</a> <a id="37548" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="37578" class="Keyword">open</a> <a id="37583" class="Keyword">import</a> <a id="37590" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="37641" class="Keyword">open</a> <a id="37646" class="Keyword">import</a> <a id="37653" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="37694" class="Keyword">open</a> <a id="37699" class="Keyword">import</a> <a id="37706" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="37743" class="Keyword">open</a> <a id="37748" class="Keyword">import</a> <a id="37755" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="37814" class="Keyword">open</a> <a id="37819" class="Keyword">import</a> <a id="37826" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37881" class="Keyword">open</a> <a id="37886" class="Keyword">import</a> <a id="37893" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37949" class="Keyword">open</a> <a id="37954" class="Keyword">import</a> <a id="37961" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="38008" class="Keyword">open</a> <a id="38013" class="Keyword">import</a> <a id="38020" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="38063" class="Keyword">open</a> <a id="38068" class="Keyword">import</a> <a id="38075" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="38120" class="Keyword">open</a> <a id="38125" class="Keyword">import</a> <a id="38132" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="38181" class="Keyword">open</a> <a id="38186" class="Keyword">import</a> <a id="38193" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="38244" class="Keyword">open</a> <a id="38249" class="Keyword">import</a> <a id="38256" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="38300" class="Keyword">open</a> <a id="38305" class="Keyword">import</a> <a id="38312" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="38390" class="Keyword">open</a> <a id="38395" class="Keyword">import</a> <a id="38402" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="38442" class="Keyword">open</a> <a id="38447" class="Keyword">import</a> <a id="38454" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="38511" class="Keyword">open</a> <a id="38516" class="Keyword">import</a> <a id="38523" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="38558" class="Keyword">open</a> <a id="38563" class="Keyword">import</a> <a id="38570" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="38616" class="Keyword">open</a> <a id="38621" class="Keyword">import</a> <a id="38628" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="38683" class="Keyword">open</a> <a id="38688" class="Keyword">import</a> <a id="38695" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="38738" class="Keyword">open</a> <a id="38743" class="Keyword">import</a> <a id="38750" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38795" class="Keyword">open</a> <a id="38800" class="Keyword">import</a> <a id="38807" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38866" class="Keyword">open</a> <a id="38871" class="Keyword">import</a> <a id="38878" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38915" class="Keyword">open</a> <a id="38920" class="Keyword">import</a> <a id="38927" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38969" class="Keyword">open</a> <a id="38974" class="Keyword">import</a> <a id="38981" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="39022" class="Keyword">open</a> <a id="39027" class="Keyword">import</a> <a id="39034" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="39073" class="Keyword">open</a> <a id="39078" class="Keyword">import</a> <a id="39085" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="39123" class="Keyword">open</a> <a id="39128" class="Keyword">import</a> <a id="39135" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="39187" class="Keyword">open</a> <a id="39192" class="Keyword">import</a> <a id="39199" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="39244" class="Keyword">open</a> <a id="39249" class="Keyword">import</a> <a id="39256" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="39295" class="Keyword">open</a> <a id="39300" class="Keyword">import</a> <a id="39307" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="39344" class="Keyword">open</a> <a id="39349" class="Keyword">import</a> <a id="39356" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="39405" class="Keyword">open</a> <a id="39410" class="Keyword">import</a> <a id="39417" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="39456" class="Keyword">open</a> <a id="39461" class="Keyword">import</a> <a id="39468" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="39506" class="Keyword">open</a> <a id="39511" class="Keyword">import</a> <a id="39518" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="39573" class="Keyword">open</a> <a id="39578" class="Keyword">import</a> <a id="39585" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="39624" class="Keyword">open</a> <a id="39629" class="Keyword">import</a> <a id="39636" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="39684" class="Keyword">open</a> <a id="39689" class="Keyword">import</a> <a id="39696" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="39743" class="Keyword">open</a> <a id="39748" class="Keyword">import</a> <a id="39755" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39793" class="Keyword">open</a> <a id="39798" class="Keyword">import</a> <a id="39805" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="39835" class="Keyword">open</a> <a id="39840" class="Keyword">import</a> <a id="39847" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39904" class="Keyword">open</a> <a id="39909" class="Keyword">import</a> <a id="39916" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39970" class="Keyword">open</a> <a id="39975" class="Keyword">import</a> <a id="39982" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="40012" class="Keyword">open</a> <a id="40017" class="Keyword">import</a> <a id="40024" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="40073" class="Keyword">open</a> <a id="40078" class="Keyword">import</a> <a id="40085" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="40127" class="Keyword">open</a> <a id="40132" class="Keyword">import</a> <a id="40139" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="40173" class="Keyword">open</a> <a id="40178" class="Keyword">import</a> <a id="40185" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="40248" class="Keyword">open</a> <a id="40253" class="Keyword">import</a> <a id="40260" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="40303" class="Keyword">open</a> <a id="40308" class="Keyword">import</a> <a id="40315" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="40350" class="Keyword">open</a> <a id="40355" class="Keyword">import</a> <a id="40362" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="40397" class="Keyword">open</a> <a id="40402" class="Keyword">import</a> <a id="40409" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="40449" class="Keyword">open</a> <a id="40454" class="Keyword">import</a> <a id="40461" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="40506" class="Keyword">open</a> <a id="40511" class="Keyword">import</a> <a id="40518" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="40559" class="Keyword">open</a> <a id="40564" class="Keyword">import</a> <a id="40571" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="40625" class="Keyword">open</a> <a id="40630" class="Keyword">import</a> <a id="40637" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="40687" class="Keyword">open</a> <a id="40692" class="Keyword">import</a> <a id="40699" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="40746" class="Keyword">open</a> <a id="40751" class="Keyword">import</a> <a id="40758" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40796" class="Keyword">open</a> <a id="40801" class="Keyword">import</a> <a id="40808" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40857" class="Keyword">open</a> <a id="40862" class="Keyword">import</a> <a id="40869" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40916" class="Keyword">open</a> <a id="40921" class="Keyword">import</a> <a id="40928" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40991" class="Keyword">open</a> <a id="40996" class="Keyword">import</a> <a id="41003" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="41035" class="Keyword">open</a> <a id="41040" class="Keyword">import</a> <a id="41047" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="41100" class="Keyword">open</a> <a id="41105" class="Keyword">import</a> <a id="41112" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="41158" class="Keyword">open</a> <a id="41163" class="Keyword">import</a> <a id="41170" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="41216" class="Keyword">open</a> <a id="41221" class="Keyword">import</a> <a id="41228" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="41268" class="Keyword">open</a> <a id="41273" class="Keyword">import</a> <a id="41280" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="41327" class="Keyword">open</a> <a id="41332" class="Keyword">import</a> <a id="41339" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="41387" class="Keyword">open</a> <a id="41392" class="Keyword">import</a> <a id="41399" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="41439" class="Keyword">open</a> <a id="41444" class="Keyword">import</a> <a id="41451" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="41496" class="Keyword">open</a> <a id="41501" class="Keyword">import</a> <a id="41508" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="41573" class="Keyword">open</a> <a id="41578" class="Keyword">import</a> <a id="41585" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="41630" class="Keyword">open</a> <a id="41635" class="Keyword">import</a> <a id="41642" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="41689" class="Keyword">open</a> <a id="41694" class="Keyword">import</a> <a id="41701" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="41754" class="Keyword">open</a> <a id="41759" class="Keyword">import</a> <a id="41766" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>