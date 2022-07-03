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
<a id="10368" class="Keyword">open</a> <a id="10373" class="Keyword">import</a> <a id="10380" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10436" class="Keyword">open</a> <a id="10441" class="Keyword">import</a> <a id="10448" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10494" class="Keyword">open</a> <a id="10499" class="Keyword">import</a> <a id="10506" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10540" class="Keyword">open</a> <a id="10545" class="Keyword">import</a> <a id="10552" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10587" class="Keyword">open</a> <a id="10592" class="Keyword">import</a> <a id="10599" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10637" class="Keyword">open</a> <a id="10642" class="Keyword">import</a> <a id="10649" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10687" class="Keyword">open</a> <a id="10692" class="Keyword">import</a> <a id="10699" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10739" class="Keyword">open</a> <a id="10744" class="Keyword">import</a> <a id="10751" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10784" class="Keyword">open</a> <a id="10789" class="Keyword">import</a> <a id="10796" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10834" class="Keyword">open</a> <a id="10839" class="Keyword">import</a> <a id="10846" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10909" class="Keyword">open</a> <a id="10914" class="Keyword">import</a> <a id="10921" href="foundation.html" class="Module">foundation</a>
<a id="10932" class="Keyword">open</a> <a id="10937" class="Keyword">import</a> <a id="10944" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10962" class="Keyword">open</a> <a id="10967" class="Keyword">import</a> <a id="10974" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10993" class="Keyword">open</a> <a id="10998" class="Keyword">import</a> <a id="11005" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11024" class="Keyword">open</a> <a id="11029" class="Keyword">import</a> <a id="11036" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11080" class="Keyword">open</a> <a id="11085" class="Keyword">import</a> <a id="11092" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11117" class="Keyword">open</a> <a id="11122" class="Keyword">import</a> <a id="11129" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11156" class="Keyword">open</a> <a id="11161" class="Keyword">import</a> <a id="11168" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11185" class="Keyword">open</a> <a id="11190" class="Keyword">import</a> <a id="11197" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11226" class="Keyword">open</a> <a id="11231" class="Keyword">import</a> <a id="11238" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11294" class="Keyword">open</a> <a id="11299" class="Keyword">import</a> <a id="11306" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11337" class="Keyword">open</a> <a id="11342" class="Keyword">import</a> <a id="11349" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11403" class="Keyword">open</a> <a id="11408" class="Keyword">import</a> <a id="11415" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11443" class="Keyword">open</a> <a id="11448" class="Keyword">import</a> <a id="11455" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11485" class="Keyword">open</a> <a id="11490" class="Keyword">import</a> <a id="11497" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11517" class="Keyword">open</a> <a id="11522" class="Keyword">import</a> <a id="11529" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11574" class="Keyword">open</a> <a id="11579" class="Keyword">import</a> <a id="11586" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11623" class="Keyword">open</a> <a id="11628" class="Keyword">import</a> <a id="11635" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11670" class="Keyword">open</a> <a id="11675" class="Keyword">import</a> <a id="11682" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11740" class="Keyword">open</a> <a id="11745" class="Keyword">import</a> <a id="11752" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11790" class="Keyword">open</a> <a id="11795" class="Keyword">import</a> <a id="11802" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11836" class="Keyword">open</a> <a id="11841" class="Keyword">import</a> <a id="11848" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11877" class="Keyword">open</a> <a id="11882" class="Keyword">import</a> <a id="11889" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11912" class="Keyword">open</a> <a id="11917" class="Keyword">import</a> <a id="11924" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="11951" class="Keyword">open</a> <a id="11956" class="Keyword">import</a> <a id="11963" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11986" class="Keyword">open</a> <a id="11991" class="Keyword">import</a> <a id="11998" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12040" class="Keyword">open</a> <a id="12045" class="Keyword">import</a> <a id="12052" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12084" class="Keyword">open</a> <a id="12089" class="Keyword">import</a> <a id="12096" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12123" class="Keyword">open</a> <a id="12128" class="Keyword">import</a> <a id="12135" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12160" class="Keyword">open</a> <a id="12165" class="Keyword">import</a> <a id="12172" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12201" class="Keyword">open</a> <a id="12206" class="Keyword">import</a> <a id="12213" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12243" class="Keyword">open</a> <a id="12248" class="Keyword">import</a> <a id="12255" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12282" class="Keyword">open</a> <a id="12287" class="Keyword">import</a> <a id="12294" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12313" class="Keyword">open</a> <a id="12318" class="Keyword">import</a> <a id="12325" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12371" class="Keyword">open</a> <a id="12376" class="Keyword">import</a> <a id="12383" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12425" class="Keyword">open</a> <a id="12430" class="Keyword">import</a> <a id="12437" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12469" class="Keyword">open</a> <a id="12474" class="Keyword">import</a> <a id="12481" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12511" class="Keyword">open</a> <a id="12516" class="Keyword">import</a> <a id="12523" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12549" class="Keyword">open</a> <a id="12554" class="Keyword">import</a> <a id="12561" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12595" class="Keyword">open</a> <a id="12600" class="Keyword">import</a> <a id="12607" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12637" class="Keyword">open</a> <a id="12642" class="Keyword">import</a> <a id="12649" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12676" class="Keyword">open</a> <a id="12681" class="Keyword">import</a> <a id="12688" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="12726" class="Keyword">open</a> <a id="12731" class="Keyword">import</a> <a id="12738" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12770" class="Keyword">open</a> <a id="12775" class="Keyword">import</a> <a id="12782" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12816" class="Keyword">open</a> <a id="12821" class="Keyword">import</a> <a id="12828" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12851" class="Keyword">open</a> <a id="12856" class="Keyword">import</a> <a id="12863" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12890" class="Keyword">open</a> <a id="12895" class="Keyword">import</a> <a id="12902" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12930" class="Keyword">open</a> <a id="12935" class="Keyword">import</a> <a id="12942" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12979" class="Keyword">open</a> <a id="12984" class="Keyword">import</a> <a id="12991" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13039" class="Keyword">open</a> <a id="13044" class="Keyword">import</a> <a id="13051" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13091" class="Keyword">open</a> <a id="13096" class="Keyword">import</a> <a id="13103" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13125" class="Keyword">open</a> <a id="13130" class="Keyword">import</a> <a id="13137" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13160" class="Keyword">open</a> <a id="13165" class="Keyword">import</a> <a id="13172" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13197" class="Keyword">open</a> <a id="13202" class="Keyword">import</a> <a id="13209" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13254" class="Keyword">open</a> <a id="13259" class="Keyword">import</a> <a id="13266" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13310" class="Keyword">open</a> <a id="13315" class="Keyword">import</a> <a id="13322" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13358" class="Keyword">open</a> <a id="13363" class="Keyword">import</a> <a id="13370" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13415" class="Keyword">open</a> <a id="13420" class="Keyword">import</a> <a id="13427" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13468" class="Keyword">open</a> <a id="13473" class="Keyword">import</a> <a id="13480" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13515" class="Keyword">open</a> <a id="13520" class="Keyword">import</a> <a id="13527" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13559" class="Keyword">open</a> <a id="13564" class="Keyword">import</a> <a id="13571" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13602" class="Keyword">open</a> <a id="13607" class="Keyword">import</a> <a id="13614" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13647" class="Keyword">open</a> <a id="13652" class="Keyword">import</a> <a id="13659" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13692" class="Keyword">open</a> <a id="13697" class="Keyword">import</a> <a id="13704" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13734" class="Keyword">open</a> <a id="13739" class="Keyword">import</a> <a id="13746" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13770" class="Keyword">open</a> <a id="13775" class="Keyword">import</a> <a id="13782" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13820" class="Keyword">open</a> <a id="13825" class="Keyword">import</a> <a id="13832" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13863" class="Keyword">open</a> <a id="13868" class="Keyword">import</a> <a id="13875" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13900" class="Keyword">open</a> <a id="13905" class="Keyword">import</a> <a id="13912" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13940" class="Keyword">open</a> <a id="13945" class="Keyword">import</a> <a id="13952" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13976" class="Keyword">open</a> <a id="13981" class="Keyword">import</a> <a id="13988" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14014" class="Keyword">open</a> <a id="14019" class="Keyword">import</a> <a id="14026" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14061" class="Keyword">open</a> <a id="14066" class="Keyword">import</a> <a id="14073" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14094" class="Keyword">open</a> <a id="14099" class="Keyword">import</a> <a id="14106" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14155" class="Keyword">open</a> <a id="14160" class="Keyword">import</a> <a id="14167" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14208" class="Keyword">open</a> <a id="14213" class="Keyword">import</a> <a id="14220" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14270" class="Keyword">open</a> <a id="14275" class="Keyword">import</a> <a id="14282" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14328" class="Keyword">open</a> <a id="14333" class="Keyword">import</a> <a id="14340" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14380" class="Keyword">open</a> <a id="14385" class="Keyword">import</a> <a id="14392" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14442" class="Keyword">open</a> <a id="14447" class="Keyword">import</a> <a id="14454" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14493" class="Keyword">open</a> <a id="14498" class="Keyword">import</a> <a id="14505" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14545" class="Keyword">open</a> <a id="14550" class="Keyword">import</a> <a id="14557" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14590" class="Keyword">open</a> <a id="14595" class="Keyword">import</a> <a id="14602" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14651" class="Keyword">open</a> <a id="14656" class="Keyword">import</a> <a id="14663" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14688" class="Keyword">open</a> <a id="14693" class="Keyword">import</a> <a id="14700" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14738" class="Keyword">open</a> <a id="14743" class="Keyword">import</a> <a id="14750" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14772" class="Keyword">open</a> <a id="14777" class="Keyword">import</a> <a id="14784" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14812" class="Keyword">open</a> <a id="14817" class="Keyword">import</a> <a id="14824" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="14860" class="Keyword">open</a> <a id="14865" class="Keyword">import</a> <a id="14872" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14898" class="Keyword">open</a> <a id="14903" class="Keyword">import</a> <a id="14910" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14928" class="Keyword">open</a> <a id="14933" class="Keyword">import</a> <a id="14940" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14975" class="Keyword">open</a> <a id="14980" class="Keyword">import</a> <a id="14987" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15022" class="Keyword">open</a> <a id="15027" class="Keyword">import</a> <a id="15034" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15061" class="Keyword">open</a> <a id="15066" class="Keyword">import</a> <a id="15073" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15129" class="Keyword">open</a> <a id="15134" class="Keyword">import</a> <a id="15141" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15170" class="Keyword">open</a> <a id="15175" class="Keyword">import</a> <a id="15182" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15212" class="Keyword">open</a> <a id="15217" class="Keyword">import</a> <a id="15224" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15251" class="Keyword">open</a> <a id="15256" class="Keyword">import</a> <a id="15263" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15289" class="Keyword">open</a> <a id="15294" class="Keyword">import</a> <a id="15301" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15328" class="Keyword">open</a> <a id="15333" class="Keyword">import</a> <a id="15340" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15364" class="Keyword">open</a> <a id="15369" class="Keyword">import</a> <a id="15376" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15399" class="Keyword">open</a> <a id="15404" class="Keyword">import</a> <a id="15411" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15438" class="Keyword">open</a> <a id="15443" class="Keyword">import</a> <a id="15450" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15482" class="Keyword">open</a> <a id="15487" class="Keyword">import</a> <a id="15494" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15529" class="Keyword">open</a> <a id="15534" class="Keyword">import</a> <a id="15541" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15572" class="Keyword">open</a> <a id="15577" class="Keyword">import</a> <a id="15584" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15617" class="Keyword">open</a> <a id="15622" class="Keyword">import</a> <a id="15629" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15663" class="Keyword">open</a> <a id="15668" class="Keyword">import</a> <a id="15675" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15715" class="Keyword">open</a> <a id="15720" class="Keyword">import</a> <a id="15727" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15758" class="Keyword">open</a> <a id="15763" class="Keyword">import</a> <a id="15770" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15802" class="Keyword">open</a> <a id="15807" class="Keyword">import</a> <a id="15814" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15845" class="Keyword">open</a> <a id="15850" class="Keyword">import</a> <a id="15857" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15874" class="Keyword">open</a> <a id="15879" class="Keyword">import</a> <a id="15886" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15911" class="Keyword">open</a> <a id="15916" class="Keyword">import</a> <a id="15923" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15952" class="Keyword">open</a> <a id="15957" class="Keyword">import</a> <a id="15964" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15989" class="Keyword">open</a> <a id="15994" class="Keyword">import</a> <a id="16001" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16022" class="Keyword">open</a> <a id="16027" class="Keyword">import</a> <a id="16034" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16058" class="Keyword">open</a> <a id="16063" class="Keyword">import</a> <a id="16070" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16090" class="Keyword">open</a> <a id="16095" class="Keyword">import</a> <a id="16102" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16136" class="Keyword">open</a> <a id="16141" class="Keyword">import</a> <a id="16148" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16186" class="Keyword">open</a> <a id="16191" class="Keyword">import</a> <a id="16198" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16226" class="Keyword">open</a> <a id="16231" class="Keyword">import</a> <a id="16238" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16262" class="Keyword">open</a> <a id="16267" class="Keyword">import</a> <a id="16274" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16301" class="Keyword">open</a> <a id="16306" class="Keyword">import</a> <a id="16313" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16348" class="Keyword">open</a> <a id="16353" class="Keyword">import</a> <a id="16360" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16381" class="Keyword">open</a> <a id="16386" class="Keyword">import</a> <a id="16393" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16429" class="Keyword">open</a> <a id="16434" class="Keyword">import</a> <a id="16441" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16486" class="Keyword">open</a> <a id="16491" class="Keyword">import</a> <a id="16498" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16544" class="Keyword">open</a> <a id="16549" class="Keyword">import</a> <a id="16556" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16596" class="Keyword">open</a> <a id="16601" class="Keyword">import</a> <a id="16608" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16638" class="Keyword">open</a> <a id="16643" class="Keyword">import</a> <a id="16650" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="16684" class="Keyword">open</a> <a id="16689" class="Keyword">import</a> <a id="16696" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16733" class="Keyword">open</a> <a id="16738" class="Keyword">import</a> <a id="16745" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16769" class="Keyword">open</a> <a id="16774" class="Keyword">import</a> <a id="16781" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16802" class="Keyword">open</a> <a id="16807" class="Keyword">import</a> <a id="16814" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16849" class="Keyword">open</a> <a id="16854" class="Keyword">import</a> <a id="16861" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16898" class="Keyword">open</a> <a id="16903" class="Keyword">import</a> <a id="16910" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16959" class="Keyword">open</a> <a id="16964" class="Keyword">import</a> <a id="16971" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17004" class="Keyword">open</a> <a id="17009" class="Keyword">import</a> <a id="17016" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17039" class="Keyword">open</a> <a id="17044" class="Keyword">import</a> <a id="17051" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17074" class="Keyword">open</a> <a id="17079" class="Keyword">import</a> <a id="17086" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17109" class="Keyword">open</a> <a id="17114" class="Keyword">import</a> <a id="17121" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17149" class="Keyword">open</a> <a id="17154" class="Keyword">import</a> <a id="17161" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17181" class="Keyword">open</a> <a id="17186" class="Keyword">import</a> <a id="17193" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17214" class="Keyword">open</a> <a id="17219" class="Keyword">import</a> <a id="17226" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17257" class="Keyword">open</a> <a id="17262" class="Keyword">import</a> <a id="17269" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17296" class="Keyword">open</a> <a id="17301" class="Keyword">import</a> <a id="17308" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17324" class="Keyword">open</a> <a id="17329" class="Keyword">import</a> <a id="17336" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17367" class="Keyword">open</a> <a id="17372" class="Keyword">import</a> <a id="17379" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17396" class="Keyword">open</a> <a id="17401" class="Keyword">import</a> <a id="17408" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17430" class="Keyword">open</a> <a id="17435" class="Keyword">import</a> <a id="17442" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17469" class="Keyword">open</a> <a id="17474" class="Keyword">import</a> <a id="17481" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17504" class="Keyword">open</a> <a id="17509" class="Keyword">import</a> <a id="17516" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17543" class="Keyword">open</a> <a id="17548" class="Keyword">import</a> <a id="17555" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17588" class="Keyword">open</a> <a id="17593" class="Keyword">import</a> <a id="17600" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17640" class="Keyword">open</a> <a id="17645" class="Keyword">import</a> <a id="17652" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17673" class="Keyword">open</a> <a id="17678" class="Keyword">import</a> <a id="17685" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17714" class="Keyword">open</a> <a id="17719" class="Keyword">import</a> <a id="17726" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17764" class="Keyword">open</a> <a id="17769" class="Keyword">import</a> <a id="17776" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17796" class="Keyword">open</a> <a id="17801" class="Keyword">import</a> <a id="17808" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17832" class="Keyword">open</a> <a id="17837" class="Keyword">import</a> <a id="17844" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17871" class="Keyword">open</a> <a id="17876" class="Keyword">import</a> <a id="17883" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17915" class="Keyword">open</a> <a id="17920" class="Keyword">import</a> <a id="17927" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17957" class="Keyword">open</a> <a id="17962" class="Keyword">import</a> <a id="17969" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17995" class="Keyword">open</a> <a id="18000" class="Keyword">import</a> <a id="18007" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18034" class="Keyword">open</a> <a id="18039" class="Keyword">import</a> <a id="18046" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18075" class="Keyword">open</a> <a id="18080" class="Keyword">import</a> <a id="18087" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18110" class="Keyword">open</a> <a id="18115" class="Keyword">import</a> <a id="18122" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18173" class="Keyword">open</a> <a id="18178" class="Keyword">import</a> <a id="18185" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18228" class="Keyword">open</a> <a id="18233" class="Keyword">import</a> <a id="18240" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18288" class="Keyword">open</a> <a id="18293" class="Keyword">import</a> <a id="18300" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18338" class="Keyword">open</a> <a id="18343" class="Keyword">import</a> <a id="18350" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18387" class="Keyword">open</a> <a id="18392" class="Keyword">import</a> <a id="18399" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18445" class="Keyword">open</a> <a id="18450" class="Keyword">import</a> <a id="18457" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18474" class="Keyword">open</a> <a id="18479" class="Keyword">import</a> <a id="18486" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18514" class="Keyword">open</a> <a id="18519" class="Keyword">import</a> <a id="18526" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18554" class="Keyword">open</a> <a id="18559" class="Keyword">import</a> <a id="18566" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18602" class="Keyword">open</a> <a id="18607" class="Keyword">import</a> <a id="18614" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18652" class="Keyword">open</a> <a id="18657" class="Keyword">import</a> <a id="18664" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18697" class="Keyword">open</a> <a id="18702" class="Keyword">import</a> <a id="18709" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18730" class="Keyword">open</a> <a id="18735" class="Keyword">import</a> <a id="18742" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="18778" class="Keyword">open</a> <a id="18783" class="Keyword">import</a> <a id="18790" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18844" class="Keyword">open</a> <a id="18849" class="Keyword">import</a> <a id="18856" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18878" class="Keyword">open</a> <a id="18883" class="Keyword">import</a> <a id="18890" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18925" class="Keyword">open</a> <a id="18930" class="Keyword">import</a> <a id="18937" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18967" class="Keyword">open</a> <a id="18972" class="Keyword">import</a> <a id="18979" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19018" class="Keyword">open</a> <a id="19023" class="Keyword">import</a> <a id="19030" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19084" class="Keyword">open</a> <a id="19089" class="Keyword">import</a> <a id="19096" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19142" class="Keyword">open</a> <a id="19147" class="Keyword">import</a> <a id="19154" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19205" class="Keyword">open</a> <a id="19210" class="Keyword">import</a> <a id="19217" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19258" class="Keyword">open</a> <a id="19263" class="Keyword">import</a> <a id="19270" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19315" class="Keyword">open</a> <a id="19320" class="Keyword">import</a> <a id="19327" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19372" class="Keyword">open</a> <a id="19377" class="Keyword">import</a> <a id="19384" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19420" class="Keyword">open</a> <a id="19425" class="Keyword">import</a> <a id="19432" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19468" class="Keyword">open</a> <a id="19473" class="Keyword">import</a> <a id="19480" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19545" class="Keyword">open</a> <a id="19550" class="Keyword">import</a> <a id="19557" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19612" class="Keyword">open</a> <a id="19617" class="Keyword">import</a> <a id="19624" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19664" class="Keyword">open</a> <a id="19669" class="Keyword">import</a> <a id="19676" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19720" class="Keyword">open</a> <a id="19725" class="Keyword">import</a> <a id="19732" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19777" class="Keyword">open</a> <a id="19782" class="Keyword">import</a> <a id="19789" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19830" class="Keyword">open</a> <a id="19835" class="Keyword">import</a> <a id="19842" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19882" class="Keyword">open</a> <a id="19887" class="Keyword">import</a> <a id="19894" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19921" class="Keyword">open</a> <a id="19926" class="Keyword">import</a> <a id="19933" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19969" class="Keyword">open</a> <a id="19974" class="Keyword">import</a> <a id="19981" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20008" class="Keyword">open</a> <a id="20013" class="Keyword">import</a> <a id="20020" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20057" class="Keyword">open</a> <a id="20062" class="Keyword">import</a> <a id="20069" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20097" class="Keyword">open</a> <a id="20102" class="Keyword">import</a> <a id="20109" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20128" class="Keyword">open</a> <a id="20133" class="Keyword">import</a> <a id="20140" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20180" class="Keyword">open</a> <a id="20185" class="Keyword">import</a> <a id="20192" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20224" class="Keyword">open</a> <a id="20229" class="Keyword">import</a> <a id="20236" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20284" class="Keyword">open</a> <a id="20289" class="Keyword">import</a> <a id="20296" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20319" class="Keyword">open</a> <a id="20324" class="Keyword">import</a> <a id="20331" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20355" class="Keyword">open</a> <a id="20360" class="Keyword">import</a> <a id="20367" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20407" class="Keyword">open</a> <a id="20412" class="Keyword">import</a> <a id="20419" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20462" class="Keyword">open</a> <a id="20467" class="Keyword">import</a> <a id="20474" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20508" class="Keyword">open</a> <a id="20513" class="Keyword">import</a> <a id="20520" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20552" class="Keyword">open</a> <a id="20557" class="Keyword">import</a> <a id="20564" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20594" class="Keyword">open</a> <a id="20599" class="Keyword">import</a> <a id="20606" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20640" class="Keyword">open</a> <a id="20645" class="Keyword">import</a> <a id="20652" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20687" class="Keyword">open</a> <a id="20692" class="Keyword">import</a> <a id="20699" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20736" class="Keyword">open</a> <a id="20741" class="Keyword">import</a> <a id="20748" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20775" class="Keyword">open</a> <a id="20780" class="Keyword">import</a> <a id="20787" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20815" class="Keyword">open</a> <a id="20820" class="Keyword">import</a> <a id="20827" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20876" class="Keyword">open</a> <a id="20881" class="Keyword">import</a> <a id="20888" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20934" class="Keyword">open</a> <a id="20939" class="Keyword">import</a> <a id="20946" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20986" class="Keyword">open</a> <a id="20991" class="Keyword">import</a> <a id="20998" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21036" class="Keyword">open</a> <a id="21041" class="Keyword">import</a> <a id="21048" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21077" class="Keyword">open</a> <a id="21082" class="Keyword">import</a> <a id="21089" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21119" class="Keyword">open</a> <a id="21124" class="Keyword">import</a> <a id="21131" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21162" class="Keyword">open</a> <a id="21167" class="Keyword">import</a> <a id="21174" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21214" class="Keyword">open</a> <a id="21219" class="Keyword">import</a> <a id="21226" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21252" class="Keyword">open</a> <a id="21257" class="Keyword">import</a> <a id="21264" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21319" class="Keyword">open</a> <a id="21324" class="Keyword">import</a> <a id="21331" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21382" class="Keyword">open</a> <a id="21387" class="Keyword">import</a> <a id="21394" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21439" class="Keyword">open</a> <a id="21444" class="Keyword">import</a> <a id="21451" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21505" class="Keyword">open</a> <a id="21510" class="Keyword">import</a> <a id="21517" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21544" class="Keyword">open</a> <a id="21549" class="Keyword">import</a> <a id="21556" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21589" class="Keyword">open</a> <a id="21594" class="Keyword">import</a> <a id="21601" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21632" class="Keyword">open</a> <a id="21637" class="Keyword">import</a> <a id="21644" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21681" class="Keyword">open</a> <a id="21686" class="Keyword">import</a> <a id="21693" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21718" class="Keyword">open</a> <a id="21723" class="Keyword">import</a> <a id="21730" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21762" class="Keyword">open</a> <a id="21767" class="Keyword">import</a> <a id="21774" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21809" class="Keyword">open</a> <a id="21814" class="Keyword">import</a> <a id="21821" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21850" class="Keyword">open</a> <a id="21855" class="Keyword">import</a> <a id="21862" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21888" class="Keyword">open</a> <a id="21893" class="Keyword">import</a> <a id="21900" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21928" class="Keyword">open</a> <a id="21933" class="Keyword">import</a> <a id="21940" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21965" class="Keyword">open</a> <a id="21970" class="Keyword">import</a> <a id="21977" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21998" class="Keyword">open</a> <a id="22003" class="Keyword">import</a> <a id="22010" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22046" class="Keyword">open</a> <a id="22051" class="Keyword">import</a> <a id="22058" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22101" class="Keyword">open</a> <a id="22106" class="Keyword">import</a> <a id="22113" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22138" class="Keyword">open</a> <a id="22143" class="Keyword">import</a> <a id="22150" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22181" class="Keyword">open</a> <a id="22186" class="Keyword">import</a> <a id="22193" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22225" class="Keyword">open</a> <a id="22230" class="Keyword">import</a> <a id="22237" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22271" class="Keyword">open</a> <a id="22276" class="Keyword">import</a> <a id="22283" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22339" class="Keyword">open</a> <a id="22344" class="Keyword">import</a> <a id="22351" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22404" class="Keyword">open</a> <a id="22409" class="Keyword">import</a> <a id="22416" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22443" class="Keyword">open</a> <a id="22448" class="Keyword">import</a> <a id="22455" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22500" class="Keyword">open</a> <a id="22505" class="Keyword">import</a> <a id="22512" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22574" class="Keyword">open</a> <a id="22579" class="Keyword">import</a> <a id="22586" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22599" class="Keyword">open</a> <a id="22604" class="Keyword">import</a> <a id="22611" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="22651" class="Keyword">open</a> <a id="22656" class="Keyword">import</a> <a id="22663" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="22707" class="Keyword">open</a> <a id="22712" class="Keyword">import</a> <a id="22719" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="22758" class="Keyword">open</a> <a id="22763" class="Keyword">import</a> <a id="22770" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="22812" class="Keyword">open</a> <a id="22817" class="Keyword">import</a> <a id="22824" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="22864" class="Keyword">open</a> <a id="22869" class="Keyword">import</a> <a id="22876" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22917" class="Keyword">open</a> <a id="22922" class="Keyword">import</a> <a id="22929" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="22967" class="Keyword">open</a> <a id="22972" class="Keyword">import</a> <a id="22979" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23042" class="Keyword">open</a> <a id="23047" class="Keyword">import</a> <a id="23054" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23083" class="Keyword">open</a> <a id="23088" class="Keyword">import</a> <a id="23095" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23140" class="Keyword">open</a> <a id="23145" class="Keyword">import</a> <a id="23152" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23194" class="Keyword">open</a> <a id="23199" class="Keyword">import</a> <a id="23206" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23250" class="Keyword">open</a> <a id="23255" class="Keyword">import</a> <a id="23262" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23311" class="Keyword">open</a> <a id="23316" class="Keyword">import</a> <a id="23323" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23373" class="Keyword">open</a> <a id="23378" class="Keyword">import</a> <a id="23385" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23412" class="Keyword">open</a> <a id="23417" class="Keyword">import</a> <a id="23424" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23465" class="Keyword">open</a> <a id="23470" class="Keyword">import</a> <a id="23477" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23500" class="Keyword">open</a> <a id="23505" class="Keyword">import</a> <a id="23512" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23561" class="Keyword">open</a> <a id="23566" class="Keyword">import</a> <a id="23573" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23612" class="Keyword">open</a> <a id="23617" class="Keyword">import</a> <a id="23624" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="23665" class="Keyword">open</a> <a id="23670" class="Keyword">import</a> <a id="23677" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="23721" class="Keyword">open</a> <a id="23726" class="Keyword">import</a> <a id="23733" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="23770" class="Keyword">open</a> <a id="23775" class="Keyword">import</a> <a id="23782" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="23804" class="Keyword">open</a> <a id="23809" class="Keyword">import</a> <a id="23816" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23846" class="Keyword">open</a> <a id="23851" class="Keyword">import</a> <a id="23858" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="23897" class="Keyword">open</a> <a id="23902" class="Keyword">import</a> <a id="23909" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="23947" class="Keyword">open</a> <a id="23952" class="Keyword">import</a> <a id="23959" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24017" class="Keyword">open</a> <a id="24022" class="Keyword">import</a> <a id="24029" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24094" class="Keyword">open</a> <a id="24099" class="Keyword">import</a> <a id="24106" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24137" class="Keyword">open</a> <a id="24142" class="Keyword">import</a> <a id="24149" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24176" class="Keyword">open</a> <a id="24181" class="Keyword">import</a> <a id="24188" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24246" class="Keyword">open</a> <a id="24251" class="Keyword">import</a> <a id="24258" href="group-theory.html" class="Module">group-theory</a>
<a id="24271" class="Keyword">open</a> <a id="24276" class="Keyword">import</a> <a id="24283" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24311" class="Keyword">open</a> <a id="24316" class="Keyword">import</a> <a id="24323" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="24354" class="Keyword">open</a> <a id="24359" class="Keyword">import</a> <a id="24366" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="24402" class="Keyword">open</a> <a id="24407" class="Keyword">import</a> <a id="24414" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24465" class="Keyword">open</a> <a id="24470" class="Keyword">import</a> <a id="24477" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24510" class="Keyword">open</a> <a id="24515" class="Keyword">import</a> <a id="24522" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24569" class="Keyword">open</a> <a id="24574" class="Keyword">import</a> <a id="24581" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24620" class="Keyword">open</a> <a id="24625" class="Keyword">import</a> <a id="24632" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24672" class="Keyword">open</a> <a id="24677" class="Keyword">import</a> <a id="24684" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="24727" class="Keyword">open</a> <a id="24732" class="Keyword">import</a> <a id="24739" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="24771" class="Keyword">open</a> <a id="24776" class="Keyword">import</a> <a id="24783" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="24819" class="Keyword">open</a> <a id="24824" class="Keyword">import</a> <a id="24831" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="24860" class="Keyword">open</a> <a id="24865" class="Keyword">import</a> <a id="24872" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="24905" class="Keyword">open</a> <a id="24910" class="Keyword">import</a> <a id="24917" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="24953" class="Keyword">open</a> <a id="24958" class="Keyword">import</a> <a id="24965" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="24994" class="Keyword">open</a> <a id="24999" class="Keyword">import</a> <a id="25006" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="25038" class="Keyword">open</a> <a id="25043" class="Keyword">import</a> <a id="25050" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25075" class="Keyword">open</a> <a id="25080" class="Keyword">import</a> <a id="25087" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25118" class="Keyword">open</a> <a id="25123" class="Keyword">import</a> <a id="25130" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25177" class="Keyword">open</a> <a id="25182" class="Keyword">import</a> <a id="25189" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25222" class="Keyword">open</a> <a id="25227" class="Keyword">import</a> <a id="25234" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25274" class="Keyword">open</a> <a id="25279" class="Keyword">import</a> <a id="25286" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25323" class="Keyword">open</a> <a id="25328" class="Keyword">import</a> <a id="25335" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="25371" class="Keyword">open</a> <a id="25376" class="Keyword">import</a> <a id="25383" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25415" class="Keyword">open</a> <a id="25420" class="Keyword">import</a> <a id="25427" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25454" class="Keyword">open</a> <a id="25459" class="Keyword">import</a> <a id="25466" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="25486" class="Keyword">open</a> <a id="25491" class="Keyword">import</a> <a id="25498" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="25525" class="Keyword">open</a> <a id="25530" class="Keyword">import</a> <a id="25537" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="25579" class="Keyword">open</a> <a id="25584" class="Keyword">import</a> <a id="25591" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="25638" class="Keyword">open</a> <a id="25643" class="Keyword">import</a> <a id="25650" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="25691" class="Keyword">open</a> <a id="25696" class="Keyword">import</a> <a id="25703" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="25737" class="Keyword">open</a> <a id="25742" class="Keyword">import</a> <a id="25749" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="25784" class="Keyword">open</a> <a id="25789" class="Keyword">import</a> <a id="25796" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="25834" class="Keyword">open</a> <a id="25839" class="Keyword">import</a> <a id="25846" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="25878" class="Keyword">open</a> <a id="25883" class="Keyword">import</a> <a id="25890" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="25931" class="Keyword">open</a> <a id="25936" class="Keyword">import</a> <a id="25943" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="25984" class="Keyword">open</a> <a id="25989" class="Keyword">import</a> <a id="25996" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26036" class="Keyword">open</a> <a id="26041" class="Keyword">import</a> <a id="26048" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26081" class="Keyword">open</a> <a id="26086" class="Keyword">import</a> <a id="26093" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="26130" class="Keyword">open</a> <a id="26135" class="Keyword">import</a> <a id="26142" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="26172" class="Keyword">open</a> <a id="26177" class="Keyword">import</a> <a id="26184" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="26229" class="Keyword">open</a> <a id="26234" class="Keyword">import</a> <a id="26241" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="26269" class="Keyword">open</a> <a id="26274" class="Keyword">import</a> <a id="26281" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="26302" class="Keyword">open</a> <a id="26307" class="Keyword">import</a> <a id="26314" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="26348" class="Keyword">open</a> <a id="26353" class="Keyword">import</a> <a id="26360" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="26394" class="Keyword">open</a> <a id="26399" class="Keyword">import</a> <a id="26406" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="26441" class="Keyword">open</a> <a id="26446" class="Keyword">import</a> <a id="26453" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="26495" class="Keyword">open</a> <a id="26500" class="Keyword">import</a> <a id="26507" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="26542" class="Keyword">open</a> <a id="26547" class="Keyword">import</a> <a id="26554" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="26593" class="Keyword">open</a> <a id="26598" class="Keyword">import</a> <a id="26605" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="26642" class="Keyword">open</a> <a id="26647" class="Keyword">import</a> <a id="26654" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="26678" class="Keyword">open</a> <a id="26683" class="Keyword">import</a> <a id="26690" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="26715" class="Keyword">open</a> <a id="26720" class="Keyword">import</a> <a id="26727" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="26758" class="Keyword">open</a> <a id="26763" class="Keyword">import</a> <a id="26770" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="26821" class="Keyword">open</a> <a id="26826" class="Keyword">import</a> <a id="26833" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="26856" class="Keyword">open</a> <a id="26861" class="Keyword">import</a> <a id="26868" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="26916" class="Keyword">open</a> <a id="26921" class="Keyword">import</a> <a id="26928" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="26958" class="Keyword">open</a> <a id="26963" class="Keyword">import</a> <a id="26970" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="27040" class="Keyword">open</a> <a id="27045" class="Keyword">import</a> <a id="27052" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="27067" class="Keyword">open</a> <a id="27072" class="Keyword">import</a> <a id="27079" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="27112" class="Keyword">open</a> <a id="27117" class="Keyword">import</a> <a id="27124" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="27156" class="Keyword">open</a> <a id="27161" class="Keyword">import</a> <a id="27168" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="27210" class="Keyword">open</a> <a id="27215" class="Keyword">import</a> <a id="27222" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="27260" class="Keyword">open</a> <a id="27265" class="Keyword">import</a> <a id="27272" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="27309" class="Keyword">open</a> <a id="27314" class="Keyword">import</a> <a id="27321" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="27354" class="Keyword">open</a> <a id="27359" class="Keyword">import</a> <a id="27366" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="27390" class="Keyword">open</a> <a id="27395" class="Keyword">import</a> <a id="27402" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="27441" class="Keyword">open</a> <a id="27446" class="Keyword">import</a> <a id="27453" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="27499" class="Keyword">open</a> <a id="27504" class="Keyword">import</a> <a id="27511" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="27556" class="Keyword">open</a> <a id="27561" class="Keyword">import</a> <a id="27568" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="27606" class="Keyword">open</a> <a id="27611" class="Keyword">import</a> <a id="27618" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="27650" class="Keyword">open</a> <a id="27655" class="Keyword">import</a> <a id="27662" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="27715" class="Keyword">open</a> <a id="27720" class="Keyword">import</a> <a id="27727" href="order-theory.html" class="Module">order-theory</a>
<a id="27740" class="Keyword">open</a> <a id="27745" class="Keyword">import</a> <a id="27752" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="27779" class="Keyword">open</a> <a id="27784" class="Keyword">import</a> <a id="27791" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="27821" class="Keyword">open</a> <a id="27826" class="Keyword">import</a> <a id="27833" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="27866" class="Keyword">open</a> <a id="27871" class="Keyword">import</a> <a id="27878" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="27914" class="Keyword">open</a> <a id="27919" class="Keyword">import</a> <a id="27926" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="27961" class="Keyword">open</a> <a id="27966" class="Keyword">import</a> <a id="27973" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="28000" class="Keyword">open</a> <a id="28005" class="Keyword">import</a> <a id="28012" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="28042" class="Keyword">open</a> <a id="28047" class="Keyword">import</a> <a id="28054" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="28090" class="Keyword">open</a> <a id="28095" class="Keyword">import</a> <a id="28102" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="28144" class="Keyword">open</a> <a id="28149" class="Keyword">import</a> <a id="28156" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="28188" class="Keyword">open</a> <a id="28193" class="Keyword">import</a> <a id="28200" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="28231" class="Keyword">open</a> <a id="28236" class="Keyword">import</a> <a id="28243" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="28269" class="Keyword">open</a> <a id="28274" class="Keyword">import</a> <a id="28281" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="28310" class="Keyword">open</a> <a id="28315" class="Keyword">import</a> <a id="28322" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="28359" class="Keyword">open</a> <a id="28364" class="Keyword">import</a> <a id="28371" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="28411" class="Keyword">open</a> <a id="28416" class="Keyword">import</a> <a id="28423" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="28445" class="Keyword">open</a> <a id="28450" class="Keyword">import</a> <a id="28457" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="28492" class="Keyword">open</a> <a id="28497" class="Keyword">import</a> <a id="28504" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="28542" class="Keyword">open</a> <a id="28547" class="Keyword">import</a> <a id="28554" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="28593" class="Keyword">open</a> <a id="28598" class="Keyword">import</a> <a id="28605" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="28640" class="Keyword">open</a> <a id="28645" class="Keyword">import</a> <a id="28652" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="28687" class="Keyword">open</a> <a id="28692" class="Keyword">import</a> <a id="28699" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="28737" class="Keyword">open</a> <a id="28742" class="Keyword">import</a> <a id="28749" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="28780" class="Keyword">open</a> <a id="28785" class="Keyword">import</a> <a id="28792" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="28834" class="Keyword">open</a> <a id="28839" class="Keyword">import</a> <a id="28846" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="28891" class="Keyword">open</a> <a id="28896" class="Keyword">import</a> <a id="28903" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="28936" class="Keyword">open</a> <a id="28941" class="Keyword">import</a> <a id="28948" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="28968" class="Keyword">open</a> <a id="28973" class="Keyword">import</a> <a id="28980" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="29003" class="Keyword">open</a> <a id="29008" class="Keyword">import</a> <a id="29015" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="29038" class="Keyword">open</a> <a id="29043" class="Keyword">import</a> <a id="29050" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="29076" class="Keyword">open</a> <a id="29081" class="Keyword">import</a> <a id="29088" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="29114" class="Keyword">open</a> <a id="29119" class="Keyword">import</a> <a id="29126" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="29182" class="Keyword">open</a> <a id="29187" class="Keyword">import</a> <a id="29194" href="polytopes.html" class="Module">polytopes</a>
<a id="29204" class="Keyword">open</a> <a id="29209" class="Keyword">import</a> <a id="29216" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="29274" class="Keyword">open</a> <a id="29279" class="Keyword">import</a> <a id="29286" href="ring-theory.html" class="Module">ring-theory</a>
<a id="29298" class="Keyword">open</a> <a id="29303" class="Keyword">import</a> <a id="29310" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="29347" class="Keyword">open</a> <a id="29352" class="Keyword">import</a> <a id="29359" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="29386" class="Keyword">open</a> <a id="29391" class="Keyword">import</a> <a id="29398" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="29430" class="Keyword">open</a> <a id="29435" class="Keyword">import</a> <a id="29442" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="29488" class="Keyword">open</a> <a id="29493" class="Keyword">import</a> <a id="29500" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="29525" class="Keyword">open</a> <a id="29530" class="Keyword">import</a> <a id="29537" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="29580" class="Keyword">open</a> <a id="29585" class="Keyword">import</a> <a id="29592" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="29630" class="Keyword">open</a> <a id="29635" class="Keyword">import</a> <a id="29642" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="29673" class="Keyword">open</a> <a id="29678" class="Keyword">import</a> <a id="29685" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="29709" class="Keyword">open</a> <a id="29714" class="Keyword">import</a> <a id="29721" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="29753" class="Keyword">open</a> <a id="29758" class="Keyword">import</a> <a id="29765" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="29791" class="Keyword">open</a> <a id="29796" class="Keyword">import</a> <a id="29803" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="29832" class="Keyword">open</a> <a id="29837" class="Keyword">import</a> <a id="29844" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="29881" class="Keyword">open</a> <a id="29886" class="Keyword">import</a> <a id="29893" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="29922" class="Keyword">open</a> <a id="29927" class="Keyword">import</a> <a id="29934" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="29961" class="Keyword">open</a> <a id="29966" class="Keyword">import</a> <a id="29973" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="30010" class="Keyword">open</a> <a id="30015" class="Keyword">import</a> <a id="30022" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="30049" class="Keyword">open</a> <a id="30054" class="Keyword">import</a> <a id="30061" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="30094" class="Keyword">open</a> <a id="30099" class="Keyword">import</a> <a id="30106" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="30124" class="Keyword">open</a> <a id="30129" class="Keyword">import</a> <a id="30136" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="30190" class="Keyword">open</a> <a id="30195" class="Keyword">import</a> <a id="30202" href="set-theory.html" class="Module">set-theory</a>
<a id="30213" class="Keyword">open</a> <a id="30218" class="Keyword">import</a> <a id="30225" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="30248" class="Keyword">open</a> <a id="30253" class="Keyword">import</a> <a id="30260" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="30284" class="Keyword">open</a> <a id="30289" class="Keyword">import</a> <a id="30296" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="30322" class="Keyword">open</a> <a id="30327" class="Keyword">import</a> <a id="30334" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="30396" class="Keyword">open</a> <a id="30401" class="Keyword">import</a> <a id="30408" href="structured-types.html" class="Module">structured-types</a>
<a id="30425" class="Keyword">open</a> <a id="30430" class="Keyword">import</a> <a id="30437" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="30472" class="Keyword">open</a> <a id="30477" class="Keyword">import</a> <a id="30484" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="30528" class="Keyword">open</a> <a id="30533" class="Keyword">import</a> <a id="30540" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="30604" class="Keyword">open</a> <a id="30609" class="Keyword">import</a> <a id="30616" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="30662" class="Keyword">open</a> <a id="30667" class="Keyword">import</a> <a id="30674" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="30698" class="Keyword">open</a> <a id="30703" class="Keyword">import</a> <a id="30710" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="30779" class="Keyword">open</a> <a id="30784" class="Keyword">import</a> <a id="30791" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="30836" class="Keyword">open</a> <a id="30841" class="Keyword">import</a> <a id="30848" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="30882" class="Keyword">open</a> <a id="30887" class="Keyword">import</a> <a id="30894" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="30955" class="Keyword">open</a> <a id="30960" class="Keyword">import</a> <a id="30967" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="31012" class="Keyword">open</a> <a id="31017" class="Keyword">import</a> <a id="31024" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="31062" class="Keyword">open</a> <a id="31067" class="Keyword">import</a> <a id="31074" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="31117" class="Keyword">open</a> <a id="31122" class="Keyword">import</a> <a id="31129" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="31165" class="Keyword">open</a> <a id="31170" class="Keyword">import</a> <a id="31177" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="31207" class="Keyword">open</a> <a id="31212" class="Keyword">import</a> <a id="31219" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="31250" class="Keyword">open</a> <a id="31255" class="Keyword">import</a> <a id="31262" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="31321" class="Keyword">open</a> <a id="31326" class="Keyword">import</a> <a id="31333" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="31384" class="Keyword">open</a> <a id="31389" class="Keyword">import</a> <a id="31396" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="31447" class="Keyword">open</a> <a id="31452" class="Keyword">import</a> <a id="31459" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="31514" class="Keyword">open</a> <a id="31519" class="Keyword">import</a> <a id="31526" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="31555" class="Keyword">open</a> <a id="31560" class="Keyword">import</a> <a id="31567" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="31595" class="Keyword">open</a> <a id="31600" class="Keyword">import</a> <a id="31607" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="31637" class="Keyword">open</a> <a id="31642" class="Keyword">import</a> <a id="31649" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="31683" class="Keyword">open</a> <a id="31688" class="Keyword">import</a> <a id="31695" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="31771" class="Keyword">open</a> <a id="31776" class="Keyword">import</a> <a id="31783" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="31809" class="Keyword">open</a> <a id="31814" class="Keyword">import</a> <a id="31821" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="31860" class="Keyword">open</a> <a id="31865" class="Keyword">import</a> <a id="31872" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="31910" class="Keyword">open</a> <a id="31915" class="Keyword">import</a> <a id="31922" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="31968" class="Keyword">open</a> <a id="31973" class="Keyword">import</a> <a id="31980" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="32017" class="Keyword">open</a> <a id="32022" class="Keyword">import</a> <a id="32029" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="32069" class="Keyword">open</a> <a id="32074" class="Keyword">import</a> <a id="32081" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="32120" class="Keyword">open</a> <a id="32125" class="Keyword">import</a> <a id="32132" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="32165" class="Keyword">open</a> <a id="32170" class="Keyword">import</a> <a id="32177" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="32212" class="Keyword">open</a> <a id="32217" class="Keyword">import</a> <a id="32224" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="32269" class="Keyword">open</a> <a id="32274" class="Keyword">import</a> <a id="32281" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="32333" class="Keyword">open</a> <a id="32338" class="Keyword">import</a> <a id="32345" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="32398" class="Keyword">open</a> <a id="32403" class="Keyword">import</a> <a id="32410" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="32458" class="Keyword">open</a> <a id="32463" class="Keyword">import</a> <a id="32470" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="32510" class="Keyword">open</a> <a id="32515" class="Keyword">import</a> <a id="32522" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="32569" class="Keyword">open</a> <a id="32574" class="Keyword">import</a> <a id="32581" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="32622" class="Keyword">open</a> <a id="32627" class="Keyword">import</a> <a id="32634" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="32672" class="Keyword">open</a> <a id="32677" class="Keyword">import</a> <a id="32684" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="32732" class="Keyword">open</a> <a id="32737" class="Keyword">import</a> <a id="32744" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="32789" class="Keyword">open</a> <a id="32794" class="Keyword">import</a> <a id="32801" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="32850" class="Keyword">open</a> <a id="32855" class="Keyword">import</a> <a id="32862" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="32939" class="Keyword">open</a> <a id="32944" class="Keyword">import</a> <a id="32951" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="33003" class="Keyword">open</a> <a id="33008" class="Keyword">import</a> <a id="33015" href="type-theories.html" class="Module">type-theories</a>
<a id="33029" class="Keyword">open</a> <a id="33034" class="Keyword">import</a> <a id="33041" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="33083" class="Keyword">open</a> <a id="33088" class="Keyword">import</a> <a id="33095" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="33133" class="Keyword">open</a> <a id="33138" class="Keyword">import</a> <a id="33145" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="33191" class="Keyword">open</a> <a id="33196" class="Keyword">import</a> <a id="33203" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="33250" class="Keyword">open</a> <a id="33255" class="Keyword">import</a> <a id="33262" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="33297" class="Keyword">open</a> <a id="33302" class="Keyword">import</a> <a id="33309" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="33387" class="Keyword">open</a> <a id="33392" class="Keyword">import</a> <a id="33399" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="33423" class="Keyword">open</a> <a id="33428" class="Keyword">import</a> <a id="33435" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="33488" class="Keyword">open</a> <a id="33493" class="Keyword">import</a> <a id="33500" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="33543" class="Keyword">open</a> <a id="33548" class="Keyword">import</a> <a id="33555" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="33595" class="Keyword">open</a> <a id="33600" class="Keyword">import</a> <a id="33607" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="33646" class="Keyword">open</a> <a id="33651" class="Keyword">import</a> <a id="33658" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="33692" class="Keyword">open</a> <a id="33697" class="Keyword">import</a> <a id="33704" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="33752" class="Keyword">open</a> <a id="33757" class="Keyword">import</a> <a id="33764" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="33815" class="Keyword">open</a> <a id="33820" class="Keyword">import</a> <a id="33827" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="33874" class="Keyword">open</a> <a id="33879" class="Keyword">import</a> <a id="33886" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="33938" class="Keyword">open</a> <a id="33943" class="Keyword">import</a> <a id="33950" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="33994" class="Keyword">open</a> <a id="33999" class="Keyword">import</a> <a id="34006" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="34046" class="Keyword">open</a> <a id="34051" class="Keyword">import</a> <a id="34058" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="34101" class="Keyword">open</a> <a id="34106" class="Keyword">import</a> <a id="34113" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="34165" class="Keyword">open</a> <a id="34170" class="Keyword">import</a> <a id="34177" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="34231" class="Keyword">open</a> <a id="34236" class="Keyword">import</a> <a id="34243" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="34291" class="Keyword">open</a> <a id="34296" class="Keyword">import</a> <a id="34303" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="34342" class="Keyword">open</a> <a id="34347" class="Keyword">import</a> <a id="34354" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="34387" class="Keyword">open</a> <a id="34392" class="Keyword">import</a> <a id="34399" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="34429" class="Keyword">open</a> <a id="34434" class="Keyword">import</a> <a id="34441" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="34492" class="Keyword">open</a> <a id="34497" class="Keyword">import</a> <a id="34504" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="34545" class="Keyword">open</a> <a id="34550" class="Keyword">import</a> <a id="34557" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="34594" class="Keyword">open</a> <a id="34599" class="Keyword">import</a> <a id="34606" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="34665" class="Keyword">open</a> <a id="34670" class="Keyword">import</a> <a id="34677" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="34732" class="Keyword">open</a> <a id="34737" class="Keyword">import</a> <a id="34744" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="34791" class="Keyword">open</a> <a id="34796" class="Keyword">import</a> <a id="34803" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="34846" class="Keyword">open</a> <a id="34851" class="Keyword">import</a> <a id="34858" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="34903" class="Keyword">open</a> <a id="34908" class="Keyword">import</a> <a id="34915" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="34964" class="Keyword">open</a> <a id="34969" class="Keyword">import</a> <a id="34976" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="35027" class="Keyword">open</a> <a id="35032" class="Keyword">import</a> <a id="35039" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="35083" class="Keyword">open</a> <a id="35088" class="Keyword">import</a> <a id="35095" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="35173" class="Keyword">open</a> <a id="35178" class="Keyword">import</a> <a id="35185" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="35225" class="Keyword">open</a> <a id="35230" class="Keyword">import</a> <a id="35237" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="35294" class="Keyword">open</a> <a id="35299" class="Keyword">import</a> <a id="35306" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="35341" class="Keyword">open</a> <a id="35346" class="Keyword">import</a> <a id="35353" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="35399" class="Keyword">open</a> <a id="35404" class="Keyword">import</a> <a id="35411" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="35466" class="Keyword">open</a> <a id="35471" class="Keyword">import</a> <a id="35478" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="35521" class="Keyword">open</a> <a id="35526" class="Keyword">import</a> <a id="35533" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="35578" class="Keyword">open</a> <a id="35583" class="Keyword">import</a> <a id="35590" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="35649" class="Keyword">open</a> <a id="35654" class="Keyword">import</a> <a id="35661" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="35698" class="Keyword">open</a> <a id="35703" class="Keyword">import</a> <a id="35710" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="35752" class="Keyword">open</a> <a id="35757" class="Keyword">import</a> <a id="35764" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="35805" class="Keyword">open</a> <a id="35810" class="Keyword">import</a> <a id="35817" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="35856" class="Keyword">open</a> <a id="35861" class="Keyword">import</a> <a id="35868" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="35906" class="Keyword">open</a> <a id="35911" class="Keyword">import</a> <a id="35918" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="35970" class="Keyword">open</a> <a id="35975" class="Keyword">import</a> <a id="35982" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="36027" class="Keyword">open</a> <a id="36032" class="Keyword">import</a> <a id="36039" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="36078" class="Keyword">open</a> <a id="36083" class="Keyword">import</a> <a id="36090" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="36127" class="Keyword">open</a> <a id="36132" class="Keyword">import</a> <a id="36139" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="36188" class="Keyword">open</a> <a id="36193" class="Keyword">import</a> <a id="36200" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="36239" class="Keyword">open</a> <a id="36244" class="Keyword">import</a> <a id="36251" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="36289" class="Keyword">open</a> <a id="36294" class="Keyword">import</a> <a id="36301" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="36356" class="Keyword">open</a> <a id="36361" class="Keyword">import</a> <a id="36368" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="36407" class="Keyword">open</a> <a id="36412" class="Keyword">import</a> <a id="36419" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="36467" class="Keyword">open</a> <a id="36472" class="Keyword">import</a> <a id="36479" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="36526" class="Keyword">open</a> <a id="36531" class="Keyword">import</a> <a id="36538" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="36576" class="Keyword">open</a> <a id="36581" class="Keyword">import</a> <a id="36588" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="36618" class="Keyword">open</a> <a id="36623" class="Keyword">import</a> <a id="36630" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="36687" class="Keyword">open</a> <a id="36692" class="Keyword">import</a> <a id="36699" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="36753" class="Keyword">open</a> <a id="36758" class="Keyword">import</a> <a id="36765" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="36795" class="Keyword">open</a> <a id="36800" class="Keyword">import</a> <a id="36807" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="36856" class="Keyword">open</a> <a id="36861" class="Keyword">import</a> <a id="36868" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="36910" class="Keyword">open</a> <a id="36915" class="Keyword">import</a> <a id="36922" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="36956" class="Keyword">open</a> <a id="36961" class="Keyword">import</a> <a id="36968" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="37031" class="Keyword">open</a> <a id="37036" class="Keyword">import</a> <a id="37043" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="37086" class="Keyword">open</a> <a id="37091" class="Keyword">import</a> <a id="37098" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="37133" class="Keyword">open</a> <a id="37138" class="Keyword">import</a> <a id="37145" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="37180" class="Keyword">open</a> <a id="37185" class="Keyword">import</a> <a id="37192" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="37232" class="Keyword">open</a> <a id="37237" class="Keyword">import</a> <a id="37244" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="37289" class="Keyword">open</a> <a id="37294" class="Keyword">import</a> <a id="37301" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="37342" class="Keyword">open</a> <a id="37347" class="Keyword">import</a> <a id="37354" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="37408" class="Keyword">open</a> <a id="37413" class="Keyword">import</a> <a id="37420" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="37470" class="Keyword">open</a> <a id="37475" class="Keyword">import</a> <a id="37482" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="37520" class="Keyword">open</a> <a id="37525" class="Keyword">import</a> <a id="37532" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="37581" class="Keyword">open</a> <a id="37586" class="Keyword">import</a> <a id="37593" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="37640" class="Keyword">open</a> <a id="37645" class="Keyword">import</a> <a id="37652" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="37715" class="Keyword">open</a> <a id="37720" class="Keyword">import</a> <a id="37727" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="37759" class="Keyword">open</a> <a id="37764" class="Keyword">import</a> <a id="37771" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="37824" class="Keyword">open</a> <a id="37829" class="Keyword">import</a> <a id="37836" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="37882" class="Keyword">open</a> <a id="37887" class="Keyword">import</a> <a id="37894" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="37940" class="Keyword">open</a> <a id="37945" class="Keyword">import</a> <a id="37952" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="38000" class="Keyword">open</a> <a id="38005" class="Keyword">import</a> <a id="38012" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="38052" class="Keyword">open</a> <a id="38057" class="Keyword">import</a> <a id="38064" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="38109" class="Keyword">open</a> <a id="38114" class="Keyword">import</a> <a id="38121" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="38186" class="Keyword">open</a> <a id="38191" class="Keyword">import</a> <a id="38198" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="38243" class="Keyword">open</a> <a id="38248" class="Keyword">import</a> <a id="38255" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="38302" class="Keyword">open</a> <a id="38307" class="Keyword">import</a> <a id="38314" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="38367" class="Keyword">open</a> <a id="38372" class="Keyword">import</a> <a id="38379" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>