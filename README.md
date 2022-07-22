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
<a id="12090" class="Keyword">open</a> <a id="12095" class="Keyword">import</a> <a id="12102" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12131" class="Keyword">open</a> <a id="12136" class="Keyword">import</a> <a id="12143" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12166" class="Keyword">open</a> <a id="12171" class="Keyword">import</a> <a id="12178" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12205" class="Keyword">open</a> <a id="12210" class="Keyword">import</a> <a id="12217" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12240" class="Keyword">open</a> <a id="12245" class="Keyword">import</a> <a id="12252" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12294" class="Keyword">open</a> <a id="12299" class="Keyword">import</a> <a id="12306" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12338" class="Keyword">open</a> <a id="12343" class="Keyword">import</a> <a id="12350" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="12376" class="Keyword">open</a> <a id="12381" class="Keyword">import</a> <a id="12388" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12415" class="Keyword">open</a> <a id="12420" class="Keyword">import</a> <a id="12427" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12452" class="Keyword">open</a> <a id="12457" class="Keyword">import</a> <a id="12464" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12493" class="Keyword">open</a> <a id="12498" class="Keyword">import</a> <a id="12505" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12535" class="Keyword">open</a> <a id="12540" class="Keyword">import</a> <a id="12547" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12574" class="Keyword">open</a> <a id="12579" class="Keyword">import</a> <a id="12586" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12605" class="Keyword">open</a> <a id="12610" class="Keyword">import</a> <a id="12617" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12663" class="Keyword">open</a> <a id="12668" class="Keyword">import</a> <a id="12675" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12717" class="Keyword">open</a> <a id="12722" class="Keyword">import</a> <a id="12729" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12761" class="Keyword">open</a> <a id="12766" class="Keyword">import</a> <a id="12773" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12803" class="Keyword">open</a> <a id="12808" class="Keyword">import</a> <a id="12815" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="12858" class="Keyword">open</a> <a id="12863" class="Keyword">import</a> <a id="12870" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12896" class="Keyword">open</a> <a id="12901" class="Keyword">import</a> <a id="12908" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12942" class="Keyword">open</a> <a id="12947" class="Keyword">import</a> <a id="12954" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="12985" class="Keyword">open</a> <a id="12990" class="Keyword">import</a> <a id="12997" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13027" class="Keyword">open</a> <a id="13032" class="Keyword">import</a> <a id="13039" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13066" class="Keyword">open</a> <a id="13071" class="Keyword">import</a> <a id="13078" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13116" class="Keyword">open</a> <a id="13121" class="Keyword">import</a> <a id="13128" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13160" class="Keyword">open</a> <a id="13165" class="Keyword">import</a> <a id="13172" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13207" class="Keyword">open</a> <a id="13212" class="Keyword">import</a> <a id="13219" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13259" class="Keyword">open</a> <a id="13264" class="Keyword">import</a> <a id="13271" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13302" class="Keyword">open</a> <a id="13307" class="Keyword">import</a> <a id="13314" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13348" class="Keyword">open</a> <a id="13353" class="Keyword">import</a> <a id="13360" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="13389" class="Keyword">open</a> <a id="13394" class="Keyword">import</a> <a id="13401" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13424" class="Keyword">open</a> <a id="13429" class="Keyword">import</a> <a id="13436" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13463" class="Keyword">open</a> <a id="13468" class="Keyword">import</a> <a id="13475" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13503" class="Keyword">open</a> <a id="13508" class="Keyword">import</a> <a id="13515" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13552" class="Keyword">open</a> <a id="13557" class="Keyword">import</a> <a id="13564" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13612" class="Keyword">open</a> <a id="13617" class="Keyword">import</a> <a id="13624" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13664" class="Keyword">open</a> <a id="13669" class="Keyword">import</a> <a id="13676" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13698" class="Keyword">open</a> <a id="13703" class="Keyword">import</a> <a id="13710" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13733" class="Keyword">open</a> <a id="13738" class="Keyword">import</a> <a id="13745" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13770" class="Keyword">open</a> <a id="13775" class="Keyword">import</a> <a id="13782" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13827" class="Keyword">open</a> <a id="13832" class="Keyword">import</a> <a id="13839" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13883" class="Keyword">open</a> <a id="13888" class="Keyword">import</a> <a id="13895" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13931" class="Keyword">open</a> <a id="13936" class="Keyword">import</a> <a id="13943" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13988" class="Keyword">open</a> <a id="13993" class="Keyword">import</a> <a id="14000" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14041" class="Keyword">open</a> <a id="14046" class="Keyword">import</a> <a id="14053" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14088" class="Keyword">open</a> <a id="14093" class="Keyword">import</a> <a id="14100" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14132" class="Keyword">open</a> <a id="14137" class="Keyword">import</a> <a id="14144" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14175" class="Keyword">open</a> <a id="14180" class="Keyword">import</a> <a id="14187" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14220" class="Keyword">open</a> <a id="14225" class="Keyword">import</a> <a id="14232" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14265" class="Keyword">open</a> <a id="14270" class="Keyword">import</a> <a id="14277" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14307" class="Keyword">open</a> <a id="14312" class="Keyword">import</a> <a id="14319" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14343" class="Keyword">open</a> <a id="14348" class="Keyword">import</a> <a id="14355" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14393" class="Keyword">open</a> <a id="14398" class="Keyword">import</a> <a id="14405" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14436" class="Keyword">open</a> <a id="14441" class="Keyword">import</a> <a id="14448" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14473" class="Keyword">open</a> <a id="14478" class="Keyword">import</a> <a id="14485" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14513" class="Keyword">open</a> <a id="14518" class="Keyword">import</a> <a id="14525" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14549" class="Keyword">open</a> <a id="14554" class="Keyword">import</a> <a id="14561" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14587" class="Keyword">open</a> <a id="14592" class="Keyword">import</a> <a id="14599" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14634" class="Keyword">open</a> <a id="14639" class="Keyword">import</a> <a id="14646" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14667" class="Keyword">open</a> <a id="14672" class="Keyword">import</a> <a id="14679" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14728" class="Keyword">open</a> <a id="14733" class="Keyword">import</a> <a id="14740" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14781" class="Keyword">open</a> <a id="14786" class="Keyword">import</a> <a id="14793" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14843" class="Keyword">open</a> <a id="14848" class="Keyword">import</a> <a id="14855" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14901" class="Keyword">open</a> <a id="14906" class="Keyword">import</a> <a id="14913" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14953" class="Keyword">open</a> <a id="14958" class="Keyword">import</a> <a id="14965" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15015" class="Keyword">open</a> <a id="15020" class="Keyword">import</a> <a id="15027" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15066" class="Keyword">open</a> <a id="15071" class="Keyword">import</a> <a id="15078" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15118" class="Keyword">open</a> <a id="15123" class="Keyword">import</a> <a id="15130" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15163" class="Keyword">open</a> <a id="15168" class="Keyword">import</a> <a id="15175" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15224" class="Keyword">open</a> <a id="15229" class="Keyword">import</a> <a id="15236" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15261" class="Keyword">open</a> <a id="15266" class="Keyword">import</a> <a id="15273" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15311" class="Keyword">open</a> <a id="15316" class="Keyword">import</a> <a id="15323" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15345" class="Keyword">open</a> <a id="15350" class="Keyword">import</a> <a id="15357" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15385" class="Keyword">open</a> <a id="15390" class="Keyword">import</a> <a id="15397" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15433" class="Keyword">open</a> <a id="15438" class="Keyword">import</a> <a id="15445" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15471" class="Keyword">open</a> <a id="15476" class="Keyword">import</a> <a id="15483" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15501" class="Keyword">open</a> <a id="15506" class="Keyword">import</a> <a id="15513" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15548" class="Keyword">open</a> <a id="15553" class="Keyword">import</a> <a id="15560" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15595" class="Keyword">open</a> <a id="15600" class="Keyword">import</a> <a id="15607" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15634" class="Keyword">open</a> <a id="15639" class="Keyword">import</a> <a id="15646" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15702" class="Keyword">open</a> <a id="15707" class="Keyword">import</a> <a id="15714" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15743" class="Keyword">open</a> <a id="15748" class="Keyword">import</a> <a id="15755" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15785" class="Keyword">open</a> <a id="15790" class="Keyword">import</a> <a id="15797" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15824" class="Keyword">open</a> <a id="15829" class="Keyword">import</a> <a id="15836" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15862" class="Keyword">open</a> <a id="15867" class="Keyword">import</a> <a id="15874" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15901" class="Keyword">open</a> <a id="15906" class="Keyword">import</a> <a id="15913" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15937" class="Keyword">open</a> <a id="15942" class="Keyword">import</a> <a id="15949" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15972" class="Keyword">open</a> <a id="15977" class="Keyword">import</a> <a id="15984" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16011" class="Keyword">open</a> <a id="16016" class="Keyword">import</a> <a id="16023" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16055" class="Keyword">open</a> <a id="16060" class="Keyword">import</a> <a id="16067" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16102" class="Keyword">open</a> <a id="16107" class="Keyword">import</a> <a id="16114" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16145" class="Keyword">open</a> <a id="16150" class="Keyword">import</a> <a id="16157" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16190" class="Keyword">open</a> <a id="16195" class="Keyword">import</a> <a id="16202" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16236" class="Keyword">open</a> <a id="16241" class="Keyword">import</a> <a id="16248" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16288" class="Keyword">open</a> <a id="16293" class="Keyword">import</a> <a id="16300" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16331" class="Keyword">open</a> <a id="16336" class="Keyword">import</a> <a id="16343" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16375" class="Keyword">open</a> <a id="16380" class="Keyword">import</a> <a id="16387" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16418" class="Keyword">open</a> <a id="16423" class="Keyword">import</a> <a id="16430" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16447" class="Keyword">open</a> <a id="16452" class="Keyword">import</a> <a id="16459" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16484" class="Keyword">open</a> <a id="16489" class="Keyword">import</a> <a id="16496" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16525" class="Keyword">open</a> <a id="16530" class="Keyword">import</a> <a id="16537" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16562" class="Keyword">open</a> <a id="16567" class="Keyword">import</a> <a id="16574" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16595" class="Keyword">open</a> <a id="16600" class="Keyword">import</a> <a id="16607" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16631" class="Keyword">open</a> <a id="16636" class="Keyword">import</a> <a id="16643" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16663" class="Keyword">open</a> <a id="16668" class="Keyword">import</a> <a id="16675" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16709" class="Keyword">open</a> <a id="16714" class="Keyword">import</a> <a id="16721" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16759" class="Keyword">open</a> <a id="16764" class="Keyword">import</a> <a id="16771" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16799" class="Keyword">open</a> <a id="16804" class="Keyword">import</a> <a id="16811" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16835" class="Keyword">open</a> <a id="16840" class="Keyword">import</a> <a id="16847" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16874" class="Keyword">open</a> <a id="16879" class="Keyword">import</a> <a id="16886" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16921" class="Keyword">open</a> <a id="16926" class="Keyword">import</a> <a id="16933" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16954" class="Keyword">open</a> <a id="16959" class="Keyword">import</a> <a id="16966" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17002" class="Keyword">open</a> <a id="17007" class="Keyword">import</a> <a id="17014" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17059" class="Keyword">open</a> <a id="17064" class="Keyword">import</a> <a id="17071" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17117" class="Keyword">open</a> <a id="17122" class="Keyword">import</a> <a id="17129" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17169" class="Keyword">open</a> <a id="17174" class="Keyword">import</a> <a id="17181" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17211" class="Keyword">open</a> <a id="17216" class="Keyword">import</a> <a id="17223" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17257" class="Keyword">open</a> <a id="17262" class="Keyword">import</a> <a id="17269" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17306" class="Keyword">open</a> <a id="17311" class="Keyword">import</a> <a id="17318" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17342" class="Keyword">open</a> <a id="17347" class="Keyword">import</a> <a id="17354" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17375" class="Keyword">open</a> <a id="17380" class="Keyword">import</a> <a id="17387" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17422" class="Keyword">open</a> <a id="17427" class="Keyword">import</a> <a id="17434" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17471" class="Keyword">open</a> <a id="17476" class="Keyword">import</a> <a id="17483" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17532" class="Keyword">open</a> <a id="17537" class="Keyword">import</a> <a id="17544" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17577" class="Keyword">open</a> <a id="17582" class="Keyword">import</a> <a id="17589" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17612" class="Keyword">open</a> <a id="17617" class="Keyword">import</a> <a id="17624" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17647" class="Keyword">open</a> <a id="17652" class="Keyword">import</a> <a id="17659" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17682" class="Keyword">open</a> <a id="17687" class="Keyword">import</a> <a id="17694" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17722" class="Keyword">open</a> <a id="17727" class="Keyword">import</a> <a id="17734" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17754" class="Keyword">open</a> <a id="17759" class="Keyword">import</a> <a id="17766" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17787" class="Keyword">open</a> <a id="17792" class="Keyword">import</a> <a id="17799" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17830" class="Keyword">open</a> <a id="17835" class="Keyword">import</a> <a id="17842" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17869" class="Keyword">open</a> <a id="17874" class="Keyword">import</a> <a id="17881" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17897" class="Keyword">open</a> <a id="17902" class="Keyword">import</a> <a id="17909" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17940" class="Keyword">open</a> <a id="17945" class="Keyword">import</a> <a id="17952" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17969" class="Keyword">open</a> <a id="17974" class="Keyword">import</a> <a id="17981" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18003" class="Keyword">open</a> <a id="18008" class="Keyword">import</a> <a id="18015" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18042" class="Keyword">open</a> <a id="18047" class="Keyword">import</a> <a id="18054" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18077" class="Keyword">open</a> <a id="18082" class="Keyword">import</a> <a id="18089" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18116" class="Keyword">open</a> <a id="18121" class="Keyword">import</a> <a id="18128" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18161" class="Keyword">open</a> <a id="18166" class="Keyword">import</a> <a id="18173" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18213" class="Keyword">open</a> <a id="18218" class="Keyword">import</a> <a id="18225" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18246" class="Keyword">open</a> <a id="18251" class="Keyword">import</a> <a id="18258" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18287" class="Keyword">open</a> <a id="18292" class="Keyword">import</a> <a id="18299" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18337" class="Keyword">open</a> <a id="18342" class="Keyword">import</a> <a id="18349" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18369" class="Keyword">open</a> <a id="18374" class="Keyword">import</a> <a id="18381" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18405" class="Keyword">open</a> <a id="18410" class="Keyword">import</a> <a id="18417" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18444" class="Keyword">open</a> <a id="18449" class="Keyword">import</a> <a id="18456" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18488" class="Keyword">open</a> <a id="18493" class="Keyword">import</a> <a id="18500" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18530" class="Keyword">open</a> <a id="18535" class="Keyword">import</a> <a id="18542" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18568" class="Keyword">open</a> <a id="18573" class="Keyword">import</a> <a id="18580" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18607" class="Keyword">open</a> <a id="18612" class="Keyword">import</a> <a id="18619" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="18656" class="Keyword">open</a> <a id="18661" class="Keyword">import</a> <a id="18668" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18697" class="Keyword">open</a> <a id="18702" class="Keyword">import</a> <a id="18709" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18732" class="Keyword">open</a> <a id="18737" class="Keyword">import</a> <a id="18744" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18795" class="Keyword">open</a> <a id="18800" class="Keyword">import</a> <a id="18807" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18850" class="Keyword">open</a> <a id="18855" class="Keyword">import</a> <a id="18862" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="18914" class="Keyword">open</a> <a id="18919" class="Keyword">import</a> <a id="18926" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18974" class="Keyword">open</a> <a id="18979" class="Keyword">import</a> <a id="18986" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19024" class="Keyword">open</a> <a id="19029" class="Keyword">import</a> <a id="19036" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19073" class="Keyword">open</a> <a id="19078" class="Keyword">import</a> <a id="19085" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19131" class="Keyword">open</a> <a id="19136" class="Keyword">import</a> <a id="19143" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19160" class="Keyword">open</a> <a id="19165" class="Keyword">import</a> <a id="19172" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19200" class="Keyword">open</a> <a id="19205" class="Keyword">import</a> <a id="19212" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19240" class="Keyword">open</a> <a id="19245" class="Keyword">import</a> <a id="19252" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19288" class="Keyword">open</a> <a id="19293" class="Keyword">import</a> <a id="19300" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19338" class="Keyword">open</a> <a id="19343" class="Keyword">import</a> <a id="19350" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19383" class="Keyword">open</a> <a id="19388" class="Keyword">import</a> <a id="19395" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19416" class="Keyword">open</a> <a id="19421" class="Keyword">import</a> <a id="19428" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19464" class="Keyword">open</a> <a id="19469" class="Keyword">import</a> <a id="19476" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19530" class="Keyword">open</a> <a id="19535" class="Keyword">import</a> <a id="19542" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19564" class="Keyword">open</a> <a id="19569" class="Keyword">import</a> <a id="19576" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19611" class="Keyword">open</a> <a id="19616" class="Keyword">import</a> <a id="19623" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19653" class="Keyword">open</a> <a id="19658" class="Keyword">import</a> <a id="19665" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19704" class="Keyword">open</a> <a id="19709" class="Keyword">import</a> <a id="19716" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19770" class="Keyword">open</a> <a id="19775" class="Keyword">import</a> <a id="19782" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19828" class="Keyword">open</a> <a id="19833" class="Keyword">import</a> <a id="19840" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19891" class="Keyword">open</a> <a id="19896" class="Keyword">import</a> <a id="19903" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19944" class="Keyword">open</a> <a id="19949" class="Keyword">import</a> <a id="19956" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20001" class="Keyword">open</a> <a id="20006" class="Keyword">import</a> <a id="20013" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20058" class="Keyword">open</a> <a id="20063" class="Keyword">import</a> <a id="20070" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20106" class="Keyword">open</a> <a id="20111" class="Keyword">import</a> <a id="20118" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20154" class="Keyword">open</a> <a id="20159" class="Keyword">import</a> <a id="20166" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20231" class="Keyword">open</a> <a id="20236" class="Keyword">import</a> <a id="20243" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20298" class="Keyword">open</a> <a id="20303" class="Keyword">import</a> <a id="20310" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20350" class="Keyword">open</a> <a id="20355" class="Keyword">import</a> <a id="20362" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20406" class="Keyword">open</a> <a id="20411" class="Keyword">import</a> <a id="20418" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20463" class="Keyword">open</a> <a id="20468" class="Keyword">import</a> <a id="20475" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20516" class="Keyword">open</a> <a id="20521" class="Keyword">import</a> <a id="20528" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20568" class="Keyword">open</a> <a id="20573" class="Keyword">import</a> <a id="20580" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20607" class="Keyword">open</a> <a id="20612" class="Keyword">import</a> <a id="20619" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20655" class="Keyword">open</a> <a id="20660" class="Keyword">import</a> <a id="20667" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20694" class="Keyword">open</a> <a id="20699" class="Keyword">import</a> <a id="20706" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20743" class="Keyword">open</a> <a id="20748" class="Keyword">import</a> <a id="20755" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20783" class="Keyword">open</a> <a id="20788" class="Keyword">import</a> <a id="20795" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20814" class="Keyword">open</a> <a id="20819" class="Keyword">import</a> <a id="20826" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20866" class="Keyword">open</a> <a id="20871" class="Keyword">import</a> <a id="20878" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20910" class="Keyword">open</a> <a id="20915" class="Keyword">import</a> <a id="20922" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20970" class="Keyword">open</a> <a id="20975" class="Keyword">import</a> <a id="20982" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21005" class="Keyword">open</a> <a id="21010" class="Keyword">import</a> <a id="21017" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21041" class="Keyword">open</a> <a id="21046" class="Keyword">import</a> <a id="21053" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21093" class="Keyword">open</a> <a id="21098" class="Keyword">import</a> <a id="21105" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="21148" class="Keyword">open</a> <a id="21153" class="Keyword">import</a> <a id="21160" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21194" class="Keyword">open</a> <a id="21199" class="Keyword">import</a> <a id="21206" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21238" class="Keyword">open</a> <a id="21243" class="Keyword">import</a> <a id="21250" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21280" class="Keyword">open</a> <a id="21285" class="Keyword">import</a> <a id="21292" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21326" class="Keyword">open</a> <a id="21331" class="Keyword">import</a> <a id="21338" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21373" class="Keyword">open</a> <a id="21378" class="Keyword">import</a> <a id="21385" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21422" class="Keyword">open</a> <a id="21427" class="Keyword">import</a> <a id="21434" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21461" class="Keyword">open</a> <a id="21466" class="Keyword">import</a> <a id="21473" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21501" class="Keyword">open</a> <a id="21506" class="Keyword">import</a> <a id="21513" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21562" class="Keyword">open</a> <a id="21567" class="Keyword">import</a> <a id="21574" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21620" class="Keyword">open</a> <a id="21625" class="Keyword">import</a> <a id="21632" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21672" class="Keyword">open</a> <a id="21677" class="Keyword">import</a> <a id="21684" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21722" class="Keyword">open</a> <a id="21727" class="Keyword">import</a> <a id="21734" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21763" class="Keyword">open</a> <a id="21768" class="Keyword">import</a> <a id="21775" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21805" class="Keyword">open</a> <a id="21810" class="Keyword">import</a> <a id="21817" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21848" class="Keyword">open</a> <a id="21853" class="Keyword">import</a> <a id="21860" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21900" class="Keyword">open</a> <a id="21905" class="Keyword">import</a> <a id="21912" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21938" class="Keyword">open</a> <a id="21943" class="Keyword">import</a> <a id="21950" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="22005" class="Keyword">open</a> <a id="22010" class="Keyword">import</a> <a id="22017" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="22068" class="Keyword">open</a> <a id="22073" class="Keyword">import</a> <a id="22080" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="22125" class="Keyword">open</a> <a id="22130" class="Keyword">import</a> <a id="22137" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22191" class="Keyword">open</a> <a id="22196" class="Keyword">import</a> <a id="22203" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22230" class="Keyword">open</a> <a id="22235" class="Keyword">import</a> <a id="22242" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22275" class="Keyword">open</a> <a id="22280" class="Keyword">import</a> <a id="22287" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22318" class="Keyword">open</a> <a id="22323" class="Keyword">import</a> <a id="22330" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22367" class="Keyword">open</a> <a id="22372" class="Keyword">import</a> <a id="22379" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22404" class="Keyword">open</a> <a id="22409" class="Keyword">import</a> <a id="22416" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22448" class="Keyword">open</a> <a id="22453" class="Keyword">import</a> <a id="22460" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22495" class="Keyword">open</a> <a id="22500" class="Keyword">import</a> <a id="22507" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22536" class="Keyword">open</a> <a id="22541" class="Keyword">import</a> <a id="22548" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22574" class="Keyword">open</a> <a id="22579" class="Keyword">import</a> <a id="22586" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22614" class="Keyword">open</a> <a id="22619" class="Keyword">import</a> <a id="22626" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22651" class="Keyword">open</a> <a id="22656" class="Keyword">import</a> <a id="22663" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22684" class="Keyword">open</a> <a id="22689" class="Keyword">import</a> <a id="22696" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22732" class="Keyword">open</a> <a id="22737" class="Keyword">import</a> <a id="22744" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22787" class="Keyword">open</a> <a id="22792" class="Keyword">import</a> <a id="22799" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22824" class="Keyword">open</a> <a id="22829" class="Keyword">import</a> <a id="22836" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22867" class="Keyword">open</a> <a id="22872" class="Keyword">import</a> <a id="22879" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22911" class="Keyword">open</a> <a id="22916" class="Keyword">import</a> <a id="22923" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22957" class="Keyword">open</a> <a id="22962" class="Keyword">import</a> <a id="22969" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="23025" class="Keyword">open</a> <a id="23030" class="Keyword">import</a> <a id="23037" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="23090" class="Keyword">open</a> <a id="23095" class="Keyword">import</a> <a id="23102" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="23129" class="Keyword">open</a> <a id="23134" class="Keyword">import</a> <a id="23141" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23186" class="Keyword">open</a> <a id="23191" class="Keyword">import</a> <a id="23198" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23260" class="Keyword">open</a> <a id="23265" class="Keyword">import</a> <a id="23272" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23285" class="Keyword">open</a> <a id="23290" class="Keyword">import</a> <a id="23297" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23337" class="Keyword">open</a> <a id="23342" class="Keyword">import</a> <a id="23349" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23393" class="Keyword">open</a> <a id="23398" class="Keyword">import</a> <a id="23405" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23444" class="Keyword">open</a> <a id="23449" class="Keyword">import</a> <a id="23456" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23498" class="Keyword">open</a> <a id="23503" class="Keyword">import</a> <a id="23510" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23550" class="Keyword">open</a> <a id="23555" class="Keyword">import</a> <a id="23562" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23603" class="Keyword">open</a> <a id="23608" class="Keyword">import</a> <a id="23615" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23653" class="Keyword">open</a> <a id="23658" class="Keyword">import</a> <a id="23665" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23728" class="Keyword">open</a> <a id="23733" class="Keyword">import</a> <a id="23740" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23769" class="Keyword">open</a> <a id="23774" class="Keyword">import</a> <a id="23781" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23826" class="Keyword">open</a> <a id="23831" class="Keyword">import</a> <a id="23838" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23880" class="Keyword">open</a> <a id="23885" class="Keyword">import</a> <a id="23892" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23936" class="Keyword">open</a> <a id="23941" class="Keyword">import</a> <a id="23948" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23997" class="Keyword">open</a> <a id="24002" class="Keyword">import</a> <a id="24009" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="24059" class="Keyword">open</a> <a id="24064" class="Keyword">import</a> <a id="24071" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="24098" class="Keyword">open</a> <a id="24103" class="Keyword">import</a> <a id="24110" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="24135" class="Keyword">open</a> <a id="24140" class="Keyword">import</a> <a id="24147" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24188" class="Keyword">open</a> <a id="24193" class="Keyword">import</a> <a id="24200" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24223" class="Keyword">open</a> <a id="24228" class="Keyword">import</a> <a id="24235" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24284" class="Keyword">open</a> <a id="24289" class="Keyword">import</a> <a id="24296" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24335" class="Keyword">open</a> <a id="24340" class="Keyword">import</a> <a id="24347" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24388" class="Keyword">open</a> <a id="24393" class="Keyword">import</a> <a id="24400" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24444" class="Keyword">open</a> <a id="24449" class="Keyword">import</a> <a id="24456" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24493" class="Keyword">open</a> <a id="24498" class="Keyword">import</a> <a id="24505" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24527" class="Keyword">open</a> <a id="24532" class="Keyword">import</a> <a id="24539" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24569" class="Keyword">open</a> <a id="24574" class="Keyword">import</a> <a id="24581" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24620" class="Keyword">open</a> <a id="24625" class="Keyword">import</a> <a id="24632" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24670" class="Keyword">open</a> <a id="24675" class="Keyword">import</a> <a id="24682" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24740" class="Keyword">open</a> <a id="24745" class="Keyword">import</a> <a id="24752" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24817" class="Keyword">open</a> <a id="24822" class="Keyword">import</a> <a id="24829" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24860" class="Keyword">open</a> <a id="24865" class="Keyword">import</a> <a id="24872" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24899" class="Keyword">open</a> <a id="24904" class="Keyword">import</a> <a id="24911" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24969" class="Keyword">open</a> <a id="24974" class="Keyword">import</a> <a id="24981" href="group-theory.html" class="Module">group-theory</a>
<a id="24994" class="Keyword">open</a> <a id="24999" class="Keyword">import</a> <a id="25006" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="25034" class="Keyword">open</a> <a id="25039" class="Keyword">import</a> <a id="25046" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25097" class="Keyword">open</a> <a id="25102" class="Keyword">import</a> <a id="25109" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25142" class="Keyword">open</a> <a id="25147" class="Keyword">import</a> <a id="25154" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="25201" class="Keyword">open</a> <a id="25206" class="Keyword">import</a> <a id="25213" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="25252" class="Keyword">open</a> <a id="25257" class="Keyword">import</a> <a id="25264" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25304" class="Keyword">open</a> <a id="25309" class="Keyword">import</a> <a id="25316" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25359" class="Keyword">open</a> <a id="25364" class="Keyword">import</a> <a id="25371" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25403" class="Keyword">open</a> <a id="25408" class="Keyword">import</a> <a id="25415" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25451" class="Keyword">open</a> <a id="25456" class="Keyword">import</a> <a id="25463" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25492" class="Keyword">open</a> <a id="25497" class="Keyword">import</a> <a id="25504" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25532" class="Keyword">open</a> <a id="25537" class="Keyword">import</a> <a id="25544" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25577" class="Keyword">open</a> <a id="25582" class="Keyword">import</a> <a id="25589" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25625" class="Keyword">open</a> <a id="25630" class="Keyword">import</a> <a id="25637" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25666" class="Keyword">open</a> <a id="25671" class="Keyword">import</a> <a id="25678" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25703" class="Keyword">open</a> <a id="25708" class="Keyword">import</a> <a id="25715" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25777" class="Keyword">open</a> <a id="25782" class="Keyword">import</a> <a id="25789" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25820" class="Keyword">open</a> <a id="25825" class="Keyword">import</a> <a id="25832" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25879" class="Keyword">open</a> <a id="25884" class="Keyword">import</a> <a id="25891" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25924" class="Keyword">open</a> <a id="25929" class="Keyword">import</a> <a id="25936" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="25985" class="Keyword">open</a> <a id="25990" class="Keyword">import</a> <a id="25997" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="26037" class="Keyword">open</a> <a id="26042" class="Keyword">import</a> <a id="26049" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="26086" class="Keyword">open</a> <a id="26091" class="Keyword">import</a> <a id="26098" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="26145" class="Keyword">open</a> <a id="26150" class="Keyword">import</a> <a id="26157" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="26198" class="Keyword">open</a> <a id="26203" class="Keyword">import</a> <a id="26210" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="26249" class="Keyword">open</a> <a id="26254" class="Keyword">import</a> <a id="26261" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="26293" class="Keyword">open</a> <a id="26298" class="Keyword">import</a> <a id="26305" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="26332" class="Keyword">open</a> <a id="26337" class="Keyword">import</a> <a id="26344" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26364" class="Keyword">open</a> <a id="26369" class="Keyword">import</a> <a id="26376" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26410" class="Keyword">open</a> <a id="26415" class="Keyword">import</a> <a id="26422" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26449" class="Keyword">open</a> <a id="26454" class="Keyword">import</a> <a id="26461" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26503" class="Keyword">open</a> <a id="26508" class="Keyword">import</a> <a id="26515" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26565" class="Keyword">open</a> <a id="26570" class="Keyword">import</a> <a id="26577" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26624" class="Keyword">open</a> <a id="26629" class="Keyword">import</a> <a id="26636" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="26677" class="Keyword">open</a> <a id="26682" class="Keyword">import</a> <a id="26689" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26723" class="Keyword">open</a> <a id="26728" class="Keyword">import</a> <a id="26735" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="26776" class="Keyword">open</a> <a id="26781" class="Keyword">import</a> <a id="26788" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="26823" class="Keyword">open</a> <a id="26828" class="Keyword">import</a> <a id="26835" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="26873" class="Keyword">open</a> <a id="26878" class="Keyword">import</a> <a id="26885" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="26920" class="Keyword">open</a> <a id="26925" class="Keyword">import</a> <a id="26932" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26964" class="Keyword">open</a> <a id="26969" class="Keyword">import</a> <a id="26976" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="27017" class="Keyword">open</a> <a id="27022" class="Keyword">import</a> <a id="27029" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="27070" class="Keyword">open</a> <a id="27075" class="Keyword">import</a> <a id="27082" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="27122" class="Keyword">open</a> <a id="27127" class="Keyword">import</a> <a id="27134" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="27167" class="Keyword">open</a> <a id="27172" class="Keyword">import</a> <a id="27179" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="27216" class="Keyword">open</a> <a id="27221" class="Keyword">import</a> <a id="27228" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="27258" class="Keyword">open</a> <a id="27263" class="Keyword">import</a> <a id="27270" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="27291" class="Keyword">open</a> <a id="27296" class="Keyword">import</a> <a id="27303" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="27357" class="Keyword">open</a> <a id="27362" class="Keyword">import</a> <a id="27369" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27414" class="Keyword">open</a> <a id="27419" class="Keyword">import</a> <a id="27426" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27454" class="Keyword">open</a> <a id="27459" class="Keyword">import</a> <a id="27466" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27487" class="Keyword">open</a> <a id="27492" class="Keyword">import</a> <a id="27499" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27542" class="Keyword">open</a> <a id="27547" class="Keyword">import</a> <a id="27554" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27588" class="Keyword">open</a> <a id="27593" class="Keyword">import</a> <a id="27600" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27630" class="Keyword">open</a> <a id="27635" class="Keyword">import</a> <a id="27642" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="27688" class="Keyword">open</a> <a id="27693" class="Keyword">import</a> <a id="27700" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="27754" class="Keyword">open</a> <a id="27759" class="Keyword">import</a> <a id="27766" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="27809" class="Keyword">open</a> <a id="27814" class="Keyword">import</a> <a id="27821" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="27855" class="Keyword">open</a> <a id="27860" class="Keyword">import</a> <a id="27867" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="27908" class="Keyword">open</a> <a id="27913" class="Keyword">import</a> <a id="27920" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="27955" class="Keyword">open</a> <a id="27960" class="Keyword">import</a> <a id="27967" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="28009" class="Keyword">open</a> <a id="28014" class="Keyword">import</a> <a id="28021" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="28056" class="Keyword">open</a> <a id="28061" class="Keyword">import</a> <a id="28068" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="28107" class="Keyword">open</a> <a id="28112" class="Keyword">import</a> <a id="28119" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="28156" class="Keyword">open</a> <a id="28161" class="Keyword">import</a> <a id="28168" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="28215" class="Keyword">open</a> <a id="28220" class="Keyword">import</a> <a id="28227" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="28291" class="Keyword">open</a> <a id="28296" class="Keyword">import</a> <a id="28303" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="28348" class="Keyword">open</a> <a id="28353" class="Keyword">import</a> <a id="28360" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="28384" class="Keyword">open</a> <a id="28389" class="Keyword">import</a> <a id="28396" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="28421" class="Keyword">open</a> <a id="28426" class="Keyword">import</a> <a id="28433" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28476" class="Keyword">open</a> <a id="28481" class="Keyword">import</a> <a id="28488" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28519" class="Keyword">open</a> <a id="28524" class="Keyword">import</a> <a id="28531" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28585" class="Keyword">open</a> <a id="28590" class="Keyword">import</a> <a id="28597" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28620" class="Keyword">open</a> <a id="28625" class="Keyword">import</a> <a id="28632" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="28670" class="Keyword">open</a> <a id="28675" class="Keyword">import</a> <a id="28682" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="28721" class="Keyword">open</a> <a id="28726" class="Keyword">import</a> <a id="28733" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="28784" class="Keyword">open</a> <a id="28789" class="Keyword">import</a> <a id="28796" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="28833" class="Keyword">open</a> <a id="28838" class="Keyword">import</a> <a id="28845" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="28902" class="Keyword">open</a> <a id="28907" class="Keyword">import</a> <a id="28914" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="28962" class="Keyword">open</a> <a id="28967" class="Keyword">import</a> <a id="28974" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="29004" class="Keyword">open</a> <a id="29009" class="Keyword">import</a> <a id="29016" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="29053" class="Keyword">open</a> <a id="29058" class="Keyword">import</a> <a id="29065" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="29086" class="Keyword">open</a> <a id="29091" class="Keyword">import</a> <a id="29098" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="29145" class="Keyword">open</a> <a id="29150" class="Keyword">import</a> <a id="29157" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="29195" class="Keyword">open</a> <a id="29200" class="Keyword">import</a> <a id="29207" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="29301" class="Keyword">open</a> <a id="29306" class="Keyword">import</a> <a id="29313" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="29328" class="Keyword">open</a> <a id="29333" class="Keyword">import</a> <a id="29340" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="29373" class="Keyword">open</a> <a id="29378" class="Keyword">import</a> <a id="29385" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="29417" class="Keyword">open</a> <a id="29422" class="Keyword">import</a> <a id="29429" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29471" class="Keyword">open</a> <a id="29476" class="Keyword">import</a> <a id="29483" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29521" class="Keyword">open</a> <a id="29526" class="Keyword">import</a> <a id="29533" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29570" class="Keyword">open</a> <a id="29575" class="Keyword">import</a> <a id="29582" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29615" class="Keyword">open</a> <a id="29620" class="Keyword">import</a> <a id="29627" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="29651" class="Keyword">open</a> <a id="29656" class="Keyword">import</a> <a id="29663" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="29702" class="Keyword">open</a> <a id="29707" class="Keyword">import</a> <a id="29714" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="29760" class="Keyword">open</a> <a id="29765" class="Keyword">import</a> <a id="29772" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="29817" class="Keyword">open</a> <a id="29822" class="Keyword">import</a> <a id="29829" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="29867" class="Keyword">open</a> <a id="29872" class="Keyword">import</a> <a id="29879" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="29911" class="Keyword">open</a> <a id="29916" class="Keyword">import</a> <a id="29923" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="29976" class="Keyword">open</a> <a id="29981" class="Keyword">import</a> <a id="29988" href="order-theory.html" class="Module">order-theory</a>
<a id="30001" class="Keyword">open</a> <a id="30006" class="Keyword">import</a> <a id="30013" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="30040" class="Keyword">open</a> <a id="30045" class="Keyword">import</a> <a id="30052" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="30082" class="Keyword">open</a> <a id="30087" class="Keyword">import</a> <a id="30094" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="30127" class="Keyword">open</a> <a id="30132" class="Keyword">import</a> <a id="30139" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="30175" class="Keyword">open</a> <a id="30180" class="Keyword">import</a> <a id="30187" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="30222" class="Keyword">open</a> <a id="30227" class="Keyword">import</a> <a id="30234" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="30261" class="Keyword">open</a> <a id="30266" class="Keyword">import</a> <a id="30273" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="30303" class="Keyword">open</a> <a id="30308" class="Keyword">import</a> <a id="30315" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="30351" class="Keyword">open</a> <a id="30356" class="Keyword">import</a> <a id="30363" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="30405" class="Keyword">open</a> <a id="30410" class="Keyword">import</a> <a id="30417" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="30449" class="Keyword">open</a> <a id="30454" class="Keyword">import</a> <a id="30461" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30492" class="Keyword">open</a> <a id="30497" class="Keyword">import</a> <a id="30504" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30530" class="Keyword">open</a> <a id="30535" class="Keyword">import</a> <a id="30542" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30571" class="Keyword">open</a> <a id="30576" class="Keyword">import</a> <a id="30583" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30620" class="Keyword">open</a> <a id="30625" class="Keyword">import</a> <a id="30632" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="30672" class="Keyword">open</a> <a id="30677" class="Keyword">import</a> <a id="30684" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="30706" class="Keyword">open</a> <a id="30711" class="Keyword">import</a> <a id="30718" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="30753" class="Keyword">open</a> <a id="30758" class="Keyword">import</a> <a id="30765" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="30803" class="Keyword">open</a> <a id="30808" class="Keyword">import</a> <a id="30815" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="30854" class="Keyword">open</a> <a id="30859" class="Keyword">import</a> <a id="30866" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="30901" class="Keyword">open</a> <a id="30906" class="Keyword">import</a> <a id="30913" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="30948" class="Keyword">open</a> <a id="30953" class="Keyword">import</a> <a id="30960" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="30998" class="Keyword">open</a> <a id="31003" class="Keyword">import</a> <a id="31010" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="31041" class="Keyword">open</a> <a id="31046" class="Keyword">import</a> <a id="31053" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="31095" class="Keyword">open</a> <a id="31100" class="Keyword">import</a> <a id="31107" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="31152" class="Keyword">open</a> <a id="31157" class="Keyword">import</a> <a id="31164" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="31197" class="Keyword">open</a> <a id="31202" class="Keyword">import</a> <a id="31209" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="31229" class="Keyword">open</a> <a id="31234" class="Keyword">import</a> <a id="31241" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="31264" class="Keyword">open</a> <a id="31269" class="Keyword">import</a> <a id="31276" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="31299" class="Keyword">open</a> <a id="31304" class="Keyword">import</a> <a id="31311" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="31337" class="Keyword">open</a> <a id="31342" class="Keyword">import</a> <a id="31349" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="31375" class="Keyword">open</a> <a id="31380" class="Keyword">import</a> <a id="31387" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="31451" class="Keyword">open</a> <a id="31456" class="Keyword">import</a> <a id="31463" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31481" class="Keyword">open</a> <a id="31486" class="Keyword">import</a> <a id="31493" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31520" class="Keyword">open</a> <a id="31525" class="Keyword">import</a> <a id="31532" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31558" class="Keyword">open</a> <a id="31563" class="Keyword">import</a> <a id="31570" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31596" class="Keyword">open</a> <a id="31601" class="Keyword">import</a> <a id="31608" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31634" class="Keyword">open</a> <a id="31639" class="Keyword">import</a> <a id="31646" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="31677" class="Keyword">open</a> <a id="31682" class="Keyword">import</a> <a id="31689" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="31752" class="Keyword">open</a> <a id="31757" class="Keyword">import</a> <a id="31764" href="polytopes.html" class="Module">polytopes</a>
<a id="31774" class="Keyword">open</a> <a id="31779" class="Keyword">import</a> <a id="31786" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="31844" class="Keyword">open</a> <a id="31849" class="Keyword">import</a> <a id="31856" href="ring-theory.html" class="Module">ring-theory</a>
<a id="31868" class="Keyword">open</a> <a id="31873" class="Keyword">import</a> <a id="31880" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="31917" class="Keyword">open</a> <a id="31922" class="Keyword">import</a> <a id="31929" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="31956" class="Keyword">open</a> <a id="31961" class="Keyword">import</a> <a id="31968" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="32000" class="Keyword">open</a> <a id="32005" class="Keyword">import</a> <a id="32012" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="32058" class="Keyword">open</a> <a id="32063" class="Keyword">import</a> <a id="32070" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="32095" class="Keyword">open</a> <a id="32100" class="Keyword">import</a> <a id="32107" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="32150" class="Keyword">open</a> <a id="32155" class="Keyword">import</a> <a id="32162" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="32200" class="Keyword">open</a> <a id="32205" class="Keyword">import</a> <a id="32212" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="32243" class="Keyword">open</a> <a id="32248" class="Keyword">import</a> <a id="32255" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="32279" class="Keyword">open</a> <a id="32284" class="Keyword">import</a> <a id="32291" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="32323" class="Keyword">open</a> <a id="32328" class="Keyword">import</a> <a id="32335" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="32361" class="Keyword">open</a> <a id="32366" class="Keyword">import</a> <a id="32373" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="32402" class="Keyword">open</a> <a id="32407" class="Keyword">import</a> <a id="32414" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="32451" class="Keyword">open</a> <a id="32456" class="Keyword">import</a> <a id="32463" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32492" class="Keyword">open</a> <a id="32497" class="Keyword">import</a> <a id="32504" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32531" class="Keyword">open</a> <a id="32536" class="Keyword">import</a> <a id="32543" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32580" class="Keyword">open</a> <a id="32585" class="Keyword">import</a> <a id="32592" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32619" class="Keyword">open</a> <a id="32624" class="Keyword">import</a> <a id="32631" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="32664" class="Keyword">open</a> <a id="32669" class="Keyword">import</a> <a id="32676" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="32694" class="Keyword">open</a> <a id="32699" class="Keyword">import</a> <a id="32706" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="32760" class="Keyword">open</a> <a id="32765" class="Keyword">import</a> <a id="32772" href="set-theory.html" class="Module">set-theory</a>
<a id="32783" class="Keyword">open</a> <a id="32788" class="Keyword">import</a> <a id="32795" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="32818" class="Keyword">open</a> <a id="32823" class="Keyword">import</a> <a id="32830" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="32854" class="Keyword">open</a> <a id="32859" class="Keyword">import</a> <a id="32866" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="32892" class="Keyword">open</a> <a id="32897" class="Keyword">import</a> <a id="32904" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="32966" class="Keyword">open</a> <a id="32971" class="Keyword">import</a> <a id="32978" href="structured-types.html" class="Module">structured-types</a>
<a id="32995" class="Keyword">open</a> <a id="33000" class="Keyword">import</a> <a id="33007" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="33042" class="Keyword">open</a> <a id="33047" class="Keyword">import</a> <a id="33054" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="33098" class="Keyword">open</a> <a id="33103" class="Keyword">import</a> <a id="33110" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="33174" class="Keyword">open</a> <a id="33179" class="Keyword">import</a> <a id="33186" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="33225" class="Keyword">open</a> <a id="33230" class="Keyword">import</a> <a id="33237" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="33283" class="Keyword">open</a> <a id="33288" class="Keyword">import</a> <a id="33295" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="33319" class="Keyword">open</a> <a id="33324" class="Keyword">import</a> <a id="33331" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="33400" class="Keyword">open</a> <a id="33405" class="Keyword">import</a> <a id="33412" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="33457" class="Keyword">open</a> <a id="33462" class="Keyword">import</a> <a id="33469" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33503" class="Keyword">open</a> <a id="33508" class="Keyword">import</a> <a id="33515" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33576" class="Keyword">open</a> <a id="33581" class="Keyword">import</a> <a id="33588" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33633" class="Keyword">open</a> <a id="33638" class="Keyword">import</a> <a id="33645" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="33683" class="Keyword">open</a> <a id="33688" class="Keyword">import</a> <a id="33695" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="33738" class="Keyword">open</a> <a id="33743" class="Keyword">import</a> <a id="33750" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="33786" class="Keyword">open</a> <a id="33791" class="Keyword">import</a> <a id="33798" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="33828" class="Keyword">open</a> <a id="33833" class="Keyword">import</a> <a id="33840" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="33871" class="Keyword">open</a> <a id="33876" class="Keyword">import</a> <a id="33883" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="33942" class="Keyword">open</a> <a id="33947" class="Keyword">import</a> <a id="33954" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="34005" class="Keyword">open</a> <a id="34010" class="Keyword">import</a> <a id="34017" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="34068" class="Keyword">open</a> <a id="34073" class="Keyword">import</a> <a id="34080" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="34135" class="Keyword">open</a> <a id="34140" class="Keyword">import</a> <a id="34147" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="34176" class="Keyword">open</a> <a id="34181" class="Keyword">import</a> <a id="34188" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="34216" class="Keyword">open</a> <a id="34221" class="Keyword">import</a> <a id="34228" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="34258" class="Keyword">open</a> <a id="34263" class="Keyword">import</a> <a id="34270" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="34304" class="Keyword">open</a> <a id="34309" class="Keyword">import</a> <a id="34316" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="34392" class="Keyword">open</a> <a id="34397" class="Keyword">import</a> <a id="34404" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="34430" class="Keyword">open</a> <a id="34435" class="Keyword">import</a> <a id="34442" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="34481" class="Keyword">open</a> <a id="34486" class="Keyword">import</a> <a id="34493" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34531" class="Keyword">open</a> <a id="34536" class="Keyword">import</a> <a id="34543" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34589" class="Keyword">open</a> <a id="34594" class="Keyword">import</a> <a id="34601" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34638" class="Keyword">open</a> <a id="34643" class="Keyword">import</a> <a id="34650" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34690" class="Keyword">open</a> <a id="34695" class="Keyword">import</a> <a id="34702" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="34741" class="Keyword">open</a> <a id="34746" class="Keyword">import</a> <a id="34753" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="34786" class="Keyword">open</a> <a id="34791" class="Keyword">import</a> <a id="34798" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="34833" class="Keyword">open</a> <a id="34838" class="Keyword">import</a> <a id="34845" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="34890" class="Keyword">open</a> <a id="34895" class="Keyword">import</a> <a id="34902" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="34954" class="Keyword">open</a> <a id="34959" class="Keyword">import</a> <a id="34966" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="35019" class="Keyword">open</a> <a id="35024" class="Keyword">import</a> <a id="35031" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="35091" class="Keyword">open</a> <a id="35096" class="Keyword">import</a> <a id="35103" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="35151" class="Keyword">open</a> <a id="35156" class="Keyword">import</a> <a id="35163" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="35203" class="Keyword">open</a> <a id="35208" class="Keyword">import</a> <a id="35215" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="35262" class="Keyword">open</a> <a id="35267" class="Keyword">import</a> <a id="35274" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="35315" class="Keyword">open</a> <a id="35320" class="Keyword">import</a> <a id="35327" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="35365" class="Keyword">open</a> <a id="35370" class="Keyword">import</a> <a id="35377" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="35425" class="Keyword">open</a> <a id="35430" class="Keyword">import</a> <a id="35437" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35474" class="Keyword">open</a> <a id="35479" class="Keyword">import</a> <a id="35486" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35520" class="Keyword">open</a> <a id="35525" class="Keyword">import</a> <a id="35532" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35579" class="Keyword">open</a> <a id="35584" class="Keyword">import</a> <a id="35591" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35636" class="Keyword">open</a> <a id="35641" class="Keyword">import</a> <a id="35648" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35697" class="Keyword">open</a> <a id="35702" class="Keyword">import</a> <a id="35709" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="35786" class="Keyword">open</a> <a id="35791" class="Keyword">import</a> <a id="35798" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="35850" class="Keyword">open</a> <a id="35855" class="Keyword">import</a> <a id="35862" href="type-theories.html" class="Module">type-theories</a>
<a id="35876" class="Keyword">open</a> <a id="35881" class="Keyword">import</a> <a id="35888" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="35930" class="Keyword">open</a> <a id="35935" class="Keyword">import</a> <a id="35942" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="35980" class="Keyword">open</a> <a id="35985" class="Keyword">import</a> <a id="35992" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="36038" class="Keyword">open</a> <a id="36043" class="Keyword">import</a> <a id="36050" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="36097" class="Keyword">open</a> <a id="36102" class="Keyword">import</a> <a id="36109" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="36144" class="Keyword">open</a> <a id="36149" class="Keyword">import</a> <a id="36156" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="36234" class="Keyword">open</a> <a id="36239" class="Keyword">import</a> <a id="36246" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="36270" class="Keyword">open</a> <a id="36275" class="Keyword">import</a> <a id="36282" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="36335" class="Keyword">open</a> <a id="36340" class="Keyword">import</a> <a id="36347" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="36390" class="Keyword">open</a> <a id="36395" class="Keyword">import</a> <a id="36402" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="36442" class="Keyword">open</a> <a id="36447" class="Keyword">import</a> <a id="36454" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36493" class="Keyword">open</a> <a id="36498" class="Keyword">import</a> <a id="36505" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36539" class="Keyword">open</a> <a id="36544" class="Keyword">import</a> <a id="36551" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36599" class="Keyword">open</a> <a id="36604" class="Keyword">import</a> <a id="36611" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36662" class="Keyword">open</a> <a id="36667" class="Keyword">import</a> <a id="36674" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="36721" class="Keyword">open</a> <a id="36726" class="Keyword">import</a> <a id="36733" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="36785" class="Keyword">open</a> <a id="36790" class="Keyword">import</a> <a id="36797" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="36841" class="Keyword">open</a> <a id="36846" class="Keyword">import</a> <a id="36853" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="36893" class="Keyword">open</a> <a id="36898" class="Keyword">import</a> <a id="36905" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="36948" class="Keyword">open</a> <a id="36953" class="Keyword">import</a> <a id="36960" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="37012" class="Keyword">open</a> <a id="37017" class="Keyword">import</a> <a id="37024" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="37078" class="Keyword">open</a> <a id="37083" class="Keyword">import</a> <a id="37090" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="37138" class="Keyword">open</a> <a id="37143" class="Keyword">import</a> <a id="37150" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="37189" class="Keyword">open</a> <a id="37194" class="Keyword">import</a> <a id="37201" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="37234" class="Keyword">open</a> <a id="37239" class="Keyword">import</a> <a id="37246" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="37276" class="Keyword">open</a> <a id="37281" class="Keyword">import</a> <a id="37288" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="37339" class="Keyword">open</a> <a id="37344" class="Keyword">import</a> <a id="37351" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="37392" class="Keyword">open</a> <a id="37397" class="Keyword">import</a> <a id="37404" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="37441" class="Keyword">open</a> <a id="37446" class="Keyword">import</a> <a id="37453" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="37512" class="Keyword">open</a> <a id="37517" class="Keyword">import</a> <a id="37524" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37579" class="Keyword">open</a> <a id="37584" class="Keyword">import</a> <a id="37591" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37647" class="Keyword">open</a> <a id="37652" class="Keyword">import</a> <a id="37659" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="37706" class="Keyword">open</a> <a id="37711" class="Keyword">import</a> <a id="37718" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="37761" class="Keyword">open</a> <a id="37766" class="Keyword">import</a> <a id="37773" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="37818" class="Keyword">open</a> <a id="37823" class="Keyword">import</a> <a id="37830" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="37879" class="Keyword">open</a> <a id="37884" class="Keyword">import</a> <a id="37891" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="37942" class="Keyword">open</a> <a id="37947" class="Keyword">import</a> <a id="37954" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="37998" class="Keyword">open</a> <a id="38003" class="Keyword">import</a> <a id="38010" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="38088" class="Keyword">open</a> <a id="38093" class="Keyword">import</a> <a id="38100" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="38140" class="Keyword">open</a> <a id="38145" class="Keyword">import</a> <a id="38152" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="38209" class="Keyword">open</a> <a id="38214" class="Keyword">import</a> <a id="38221" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="38256" class="Keyword">open</a> <a id="38261" class="Keyword">import</a> <a id="38268" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="38314" class="Keyword">open</a> <a id="38319" class="Keyword">import</a> <a id="38326" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="38381" class="Keyword">open</a> <a id="38386" class="Keyword">import</a> <a id="38393" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="38436" class="Keyword">open</a> <a id="38441" class="Keyword">import</a> <a id="38448" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38493" class="Keyword">open</a> <a id="38498" class="Keyword">import</a> <a id="38505" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38564" class="Keyword">open</a> <a id="38569" class="Keyword">import</a> <a id="38576" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38613" class="Keyword">open</a> <a id="38618" class="Keyword">import</a> <a id="38625" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38667" class="Keyword">open</a> <a id="38672" class="Keyword">import</a> <a id="38679" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="38720" class="Keyword">open</a> <a id="38725" class="Keyword">import</a> <a id="38732" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="38771" class="Keyword">open</a> <a id="38776" class="Keyword">import</a> <a id="38783" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="38821" class="Keyword">open</a> <a id="38826" class="Keyword">import</a> <a id="38833" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="38885" class="Keyword">open</a> <a id="38890" class="Keyword">import</a> <a id="38897" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="38942" class="Keyword">open</a> <a id="38947" class="Keyword">import</a> <a id="38954" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="38993" class="Keyword">open</a> <a id="38998" class="Keyword">import</a> <a id="39005" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="39042" class="Keyword">open</a> <a id="39047" class="Keyword">import</a> <a id="39054" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="39103" class="Keyword">open</a> <a id="39108" class="Keyword">import</a> <a id="39115" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="39154" class="Keyword">open</a> <a id="39159" class="Keyword">import</a> <a id="39166" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="39204" class="Keyword">open</a> <a id="39209" class="Keyword">import</a> <a id="39216" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="39271" class="Keyword">open</a> <a id="39276" class="Keyword">import</a> <a id="39283" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="39322" class="Keyword">open</a> <a id="39327" class="Keyword">import</a> <a id="39334" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="39382" class="Keyword">open</a> <a id="39387" class="Keyword">import</a> <a id="39394" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="39441" class="Keyword">open</a> <a id="39446" class="Keyword">import</a> <a id="39453" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39491" class="Keyword">open</a> <a id="39496" class="Keyword">import</a> <a id="39503" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="39533" class="Keyword">open</a> <a id="39538" class="Keyword">import</a> <a id="39545" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39602" class="Keyword">open</a> <a id="39607" class="Keyword">import</a> <a id="39614" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39668" class="Keyword">open</a> <a id="39673" class="Keyword">import</a> <a id="39680" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="39710" class="Keyword">open</a> <a id="39715" class="Keyword">import</a> <a id="39722" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="39771" class="Keyword">open</a> <a id="39776" class="Keyword">import</a> <a id="39783" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="39825" class="Keyword">open</a> <a id="39830" class="Keyword">import</a> <a id="39837" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="39871" class="Keyword">open</a> <a id="39876" class="Keyword">import</a> <a id="39883" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="39946" class="Keyword">open</a> <a id="39951" class="Keyword">import</a> <a id="39958" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="40001" class="Keyword">open</a> <a id="40006" class="Keyword">import</a> <a id="40013" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="40048" class="Keyword">open</a> <a id="40053" class="Keyword">import</a> <a id="40060" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="40095" class="Keyword">open</a> <a id="40100" class="Keyword">import</a> <a id="40107" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="40147" class="Keyword">open</a> <a id="40152" class="Keyword">import</a> <a id="40159" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="40204" class="Keyword">open</a> <a id="40209" class="Keyword">import</a> <a id="40216" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="40257" class="Keyword">open</a> <a id="40262" class="Keyword">import</a> <a id="40269" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="40323" class="Keyword">open</a> <a id="40328" class="Keyword">import</a> <a id="40335" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="40385" class="Keyword">open</a> <a id="40390" class="Keyword">import</a> <a id="40397" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="40444" class="Keyword">open</a> <a id="40449" class="Keyword">import</a> <a id="40456" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40494" class="Keyword">open</a> <a id="40499" class="Keyword">import</a> <a id="40506" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40555" class="Keyword">open</a> <a id="40560" class="Keyword">import</a> <a id="40567" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40614" class="Keyword">open</a> <a id="40619" class="Keyword">import</a> <a id="40626" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40689" class="Keyword">open</a> <a id="40694" class="Keyword">import</a> <a id="40701" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="40733" class="Keyword">open</a> <a id="40738" class="Keyword">import</a> <a id="40745" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="40798" class="Keyword">open</a> <a id="40803" class="Keyword">import</a> <a id="40810" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="40856" class="Keyword">open</a> <a id="40861" class="Keyword">import</a> <a id="40868" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="40914" class="Keyword">open</a> <a id="40919" class="Keyword">import</a> <a id="40926" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="40966" class="Keyword">open</a> <a id="40971" class="Keyword">import</a> <a id="40978" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="41025" class="Keyword">open</a> <a id="41030" class="Keyword">import</a> <a id="41037" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="41085" class="Keyword">open</a> <a id="41090" class="Keyword">import</a> <a id="41097" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="41137" class="Keyword">open</a> <a id="41142" class="Keyword">import</a> <a id="41149" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="41194" class="Keyword">open</a> <a id="41199" class="Keyword">import</a> <a id="41206" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="41271" class="Keyword">open</a> <a id="41276" class="Keyword">import</a> <a id="41283" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="41328" class="Keyword">open</a> <a id="41333" class="Keyword">import</a> <a id="41340" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="41387" class="Keyword">open</a> <a id="41392" class="Keyword">import</a> <a id="41399" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="41452" class="Keyword">open</a> <a id="41457" class="Keyword">import</a> <a id="41464" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>