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
<a id="11146" class="Keyword">open</a> <a id="11151" class="Keyword">import</a> <a id="11158" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11176" class="Keyword">open</a> <a id="11181" class="Keyword">import</a> <a id="11188" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11207" class="Keyword">open</a> <a id="11212" class="Keyword">import</a> <a id="11219" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11238" class="Keyword">open</a> <a id="11243" class="Keyword">import</a> <a id="11250" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11294" class="Keyword">open</a> <a id="11299" class="Keyword">import</a> <a id="11306" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11331" class="Keyword">open</a> <a id="11336" class="Keyword">import</a> <a id="11343" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11370" class="Keyword">open</a> <a id="11375" class="Keyword">import</a> <a id="11382" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11399" class="Keyword">open</a> <a id="11404" class="Keyword">import</a> <a id="11411" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11440" class="Keyword">open</a> <a id="11445" class="Keyword">import</a> <a id="11452" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11508" class="Keyword">open</a> <a id="11513" class="Keyword">import</a> <a id="11520" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11551" class="Keyword">open</a> <a id="11556" class="Keyword">import</a> <a id="11563" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11617" class="Keyword">open</a> <a id="11622" class="Keyword">import</a> <a id="11629" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11657" class="Keyword">open</a> <a id="11662" class="Keyword">import</a> <a id="11669" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11699" class="Keyword">open</a> <a id="11704" class="Keyword">import</a> <a id="11711" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11731" class="Keyword">open</a> <a id="11736" class="Keyword">import</a> <a id="11743" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11788" class="Keyword">open</a> <a id="11793" class="Keyword">import</a> <a id="11800" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11837" class="Keyword">open</a> <a id="11842" class="Keyword">import</a> <a id="11849" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11884" class="Keyword">open</a> <a id="11889" class="Keyword">import</a> <a id="11896" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11954" class="Keyword">open</a> <a id="11959" class="Keyword">import</a> <a id="11966" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12004" class="Keyword">open</a> <a id="12009" class="Keyword">import</a> <a id="12016" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12050" class="Keyword">open</a> <a id="12055" class="Keyword">import</a> <a id="12062" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12091" class="Keyword">open</a> <a id="12096" class="Keyword">import</a> <a id="12103" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12126" class="Keyword">open</a> <a id="12131" class="Keyword">import</a> <a id="12138" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12165" class="Keyword">open</a> <a id="12170" class="Keyword">import</a> <a id="12177" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12200" class="Keyword">open</a> <a id="12205" class="Keyword">import</a> <a id="12212" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12254" class="Keyword">open</a> <a id="12259" class="Keyword">import</a> <a id="12266" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12298" class="Keyword">open</a> <a id="12303" class="Keyword">import</a> <a id="12310" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="12336" class="Keyword">open</a> <a id="12341" class="Keyword">import</a> <a id="12348" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12375" class="Keyword">open</a> <a id="12380" class="Keyword">import</a> <a id="12387" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12412" class="Keyword">open</a> <a id="12417" class="Keyword">import</a> <a id="12424" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12453" class="Keyword">open</a> <a id="12458" class="Keyword">import</a> <a id="12465" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12495" class="Keyword">open</a> <a id="12500" class="Keyword">import</a> <a id="12507" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12534" class="Keyword">open</a> <a id="12539" class="Keyword">import</a> <a id="12546" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12565" class="Keyword">open</a> <a id="12570" class="Keyword">import</a> <a id="12577" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12623" class="Keyword">open</a> <a id="12628" class="Keyword">import</a> <a id="12635" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12677" class="Keyword">open</a> <a id="12682" class="Keyword">import</a> <a id="12689" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12721" class="Keyword">open</a> <a id="12726" class="Keyword">import</a> <a id="12733" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12763" class="Keyword">open</a> <a id="12768" class="Keyword">import</a> <a id="12775" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="12818" class="Keyword">open</a> <a id="12823" class="Keyword">import</a> <a id="12830" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12856" class="Keyword">open</a> <a id="12861" class="Keyword">import</a> <a id="12868" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12902" class="Keyword">open</a> <a id="12907" class="Keyword">import</a> <a id="12914" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="12945" class="Keyword">open</a> <a id="12950" class="Keyword">import</a> <a id="12957" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12987" class="Keyword">open</a> <a id="12992" class="Keyword">import</a> <a id="12999" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13026" class="Keyword">open</a> <a id="13031" class="Keyword">import</a> <a id="13038" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13076" class="Keyword">open</a> <a id="13081" class="Keyword">import</a> <a id="13088" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13120" class="Keyword">open</a> <a id="13125" class="Keyword">import</a> <a id="13132" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13166" class="Keyword">open</a> <a id="13171" class="Keyword">import</a> <a id="13178" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13201" class="Keyword">open</a> <a id="13206" class="Keyword">import</a> <a id="13213" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13240" class="Keyword">open</a> <a id="13245" class="Keyword">import</a> <a id="13252" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13280" class="Keyword">open</a> <a id="13285" class="Keyword">import</a> <a id="13292" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13329" class="Keyword">open</a> <a id="13334" class="Keyword">import</a> <a id="13341" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13389" class="Keyword">open</a> <a id="13394" class="Keyword">import</a> <a id="13401" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13441" class="Keyword">open</a> <a id="13446" class="Keyword">import</a> <a id="13453" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13475" class="Keyword">open</a> <a id="13480" class="Keyword">import</a> <a id="13487" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13510" class="Keyword">open</a> <a id="13515" class="Keyword">import</a> <a id="13522" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13547" class="Keyword">open</a> <a id="13552" class="Keyword">import</a> <a id="13559" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13604" class="Keyword">open</a> <a id="13609" class="Keyword">import</a> <a id="13616" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13660" class="Keyword">open</a> <a id="13665" class="Keyword">import</a> <a id="13672" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13708" class="Keyword">open</a> <a id="13713" class="Keyword">import</a> <a id="13720" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13765" class="Keyword">open</a> <a id="13770" class="Keyword">import</a> <a id="13777" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13818" class="Keyword">open</a> <a id="13823" class="Keyword">import</a> <a id="13830" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13865" class="Keyword">open</a> <a id="13870" class="Keyword">import</a> <a id="13877" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13909" class="Keyword">open</a> <a id="13914" class="Keyword">import</a> <a id="13921" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13952" class="Keyword">open</a> <a id="13957" class="Keyword">import</a> <a id="13964" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13997" class="Keyword">open</a> <a id="14002" class="Keyword">import</a> <a id="14009" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14042" class="Keyword">open</a> <a id="14047" class="Keyword">import</a> <a id="14054" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14084" class="Keyword">open</a> <a id="14089" class="Keyword">import</a> <a id="14096" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14120" class="Keyword">open</a> <a id="14125" class="Keyword">import</a> <a id="14132" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14170" class="Keyword">open</a> <a id="14175" class="Keyword">import</a> <a id="14182" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14213" class="Keyword">open</a> <a id="14218" class="Keyword">import</a> <a id="14225" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14250" class="Keyword">open</a> <a id="14255" class="Keyword">import</a> <a id="14262" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14290" class="Keyword">open</a> <a id="14295" class="Keyword">import</a> <a id="14302" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14326" class="Keyword">open</a> <a id="14331" class="Keyword">import</a> <a id="14338" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14364" class="Keyword">open</a> <a id="14369" class="Keyword">import</a> <a id="14376" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14411" class="Keyword">open</a> <a id="14416" class="Keyword">import</a> <a id="14423" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14444" class="Keyword">open</a> <a id="14449" class="Keyword">import</a> <a id="14456" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14505" class="Keyword">open</a> <a id="14510" class="Keyword">import</a> <a id="14517" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14558" class="Keyword">open</a> <a id="14563" class="Keyword">import</a> <a id="14570" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14620" class="Keyword">open</a> <a id="14625" class="Keyword">import</a> <a id="14632" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14678" class="Keyword">open</a> <a id="14683" class="Keyword">import</a> <a id="14690" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14730" class="Keyword">open</a> <a id="14735" class="Keyword">import</a> <a id="14742" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14792" class="Keyword">open</a> <a id="14797" class="Keyword">import</a> <a id="14804" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14843" class="Keyword">open</a> <a id="14848" class="Keyword">import</a> <a id="14855" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14895" class="Keyword">open</a> <a id="14900" class="Keyword">import</a> <a id="14907" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14940" class="Keyword">open</a> <a id="14945" class="Keyword">import</a> <a id="14952" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15001" class="Keyword">open</a> <a id="15006" class="Keyword">import</a> <a id="15013" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15038" class="Keyword">open</a> <a id="15043" class="Keyword">import</a> <a id="15050" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15088" class="Keyword">open</a> <a id="15093" class="Keyword">import</a> <a id="15100" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15122" class="Keyword">open</a> <a id="15127" class="Keyword">import</a> <a id="15134" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15162" class="Keyword">open</a> <a id="15167" class="Keyword">import</a> <a id="15174" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15210" class="Keyword">open</a> <a id="15215" class="Keyword">import</a> <a id="15222" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15248" class="Keyword">open</a> <a id="15253" class="Keyword">import</a> <a id="15260" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15278" class="Keyword">open</a> <a id="15283" class="Keyword">import</a> <a id="15290" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15325" class="Keyword">open</a> <a id="15330" class="Keyword">import</a> <a id="15337" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15372" class="Keyword">open</a> <a id="15377" class="Keyword">import</a> <a id="15384" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15411" class="Keyword">open</a> <a id="15416" class="Keyword">import</a> <a id="15423" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15479" class="Keyword">open</a> <a id="15484" class="Keyword">import</a> <a id="15491" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15520" class="Keyword">open</a> <a id="15525" class="Keyword">import</a> <a id="15532" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15562" class="Keyword">open</a> <a id="15567" class="Keyword">import</a> <a id="15574" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15601" class="Keyword">open</a> <a id="15606" class="Keyword">import</a> <a id="15613" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15639" class="Keyword">open</a> <a id="15644" class="Keyword">import</a> <a id="15651" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15678" class="Keyword">open</a> <a id="15683" class="Keyword">import</a> <a id="15690" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15714" class="Keyword">open</a> <a id="15719" class="Keyword">import</a> <a id="15726" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15749" class="Keyword">open</a> <a id="15754" class="Keyword">import</a> <a id="15761" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15788" class="Keyword">open</a> <a id="15793" class="Keyword">import</a> <a id="15800" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15832" class="Keyword">open</a> <a id="15837" class="Keyword">import</a> <a id="15844" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15879" class="Keyword">open</a> <a id="15884" class="Keyword">import</a> <a id="15891" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15922" class="Keyword">open</a> <a id="15927" class="Keyword">import</a> <a id="15934" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15967" class="Keyword">open</a> <a id="15972" class="Keyword">import</a> <a id="15979" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16013" class="Keyword">open</a> <a id="16018" class="Keyword">import</a> <a id="16025" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16065" class="Keyword">open</a> <a id="16070" class="Keyword">import</a> <a id="16077" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16108" class="Keyword">open</a> <a id="16113" class="Keyword">import</a> <a id="16120" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16152" class="Keyword">open</a> <a id="16157" class="Keyword">import</a> <a id="16164" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16195" class="Keyword">open</a> <a id="16200" class="Keyword">import</a> <a id="16207" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16224" class="Keyword">open</a> <a id="16229" class="Keyword">import</a> <a id="16236" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16261" class="Keyword">open</a> <a id="16266" class="Keyword">import</a> <a id="16273" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16302" class="Keyword">open</a> <a id="16307" class="Keyword">import</a> <a id="16314" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16339" class="Keyword">open</a> <a id="16344" class="Keyword">import</a> <a id="16351" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16372" class="Keyword">open</a> <a id="16377" class="Keyword">import</a> <a id="16384" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16408" class="Keyword">open</a> <a id="16413" class="Keyword">import</a> <a id="16420" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16440" class="Keyword">open</a> <a id="16445" class="Keyword">import</a> <a id="16452" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16486" class="Keyword">open</a> <a id="16491" class="Keyword">import</a> <a id="16498" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16536" class="Keyword">open</a> <a id="16541" class="Keyword">import</a> <a id="16548" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16576" class="Keyword">open</a> <a id="16581" class="Keyword">import</a> <a id="16588" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16612" class="Keyword">open</a> <a id="16617" class="Keyword">import</a> <a id="16624" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16651" class="Keyword">open</a> <a id="16656" class="Keyword">import</a> <a id="16663" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16698" class="Keyword">open</a> <a id="16703" class="Keyword">import</a> <a id="16710" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16731" class="Keyword">open</a> <a id="16736" class="Keyword">import</a> <a id="16743" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16779" class="Keyword">open</a> <a id="16784" class="Keyword">import</a> <a id="16791" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16836" class="Keyword">open</a> <a id="16841" class="Keyword">import</a> <a id="16848" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16894" class="Keyword">open</a> <a id="16899" class="Keyword">import</a> <a id="16906" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16946" class="Keyword">open</a> <a id="16951" class="Keyword">import</a> <a id="16958" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16988" class="Keyword">open</a> <a id="16993" class="Keyword">import</a> <a id="17000" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17034" class="Keyword">open</a> <a id="17039" class="Keyword">import</a> <a id="17046" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17083" class="Keyword">open</a> <a id="17088" class="Keyword">import</a> <a id="17095" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17119" class="Keyword">open</a> <a id="17124" class="Keyword">import</a> <a id="17131" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17152" class="Keyword">open</a> <a id="17157" class="Keyword">import</a> <a id="17164" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17199" class="Keyword">open</a> <a id="17204" class="Keyword">import</a> <a id="17211" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17248" class="Keyword">open</a> <a id="17253" class="Keyword">import</a> <a id="17260" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17309" class="Keyword">open</a> <a id="17314" class="Keyword">import</a> <a id="17321" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17354" class="Keyword">open</a> <a id="17359" class="Keyword">import</a> <a id="17366" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17389" class="Keyword">open</a> <a id="17394" class="Keyword">import</a> <a id="17401" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17424" class="Keyword">open</a> <a id="17429" class="Keyword">import</a> <a id="17436" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17459" class="Keyword">open</a> <a id="17464" class="Keyword">import</a> <a id="17471" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17499" class="Keyword">open</a> <a id="17504" class="Keyword">import</a> <a id="17511" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17531" class="Keyword">open</a> <a id="17536" class="Keyword">import</a> <a id="17543" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17564" class="Keyword">open</a> <a id="17569" class="Keyword">import</a> <a id="17576" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17607" class="Keyword">open</a> <a id="17612" class="Keyword">import</a> <a id="17619" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17646" class="Keyword">open</a> <a id="17651" class="Keyword">import</a> <a id="17658" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17674" class="Keyword">open</a> <a id="17679" class="Keyword">import</a> <a id="17686" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17717" class="Keyword">open</a> <a id="17722" class="Keyword">import</a> <a id="17729" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17746" class="Keyword">open</a> <a id="17751" class="Keyword">import</a> <a id="17758" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17780" class="Keyword">open</a> <a id="17785" class="Keyword">import</a> <a id="17792" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17819" class="Keyword">open</a> <a id="17824" class="Keyword">import</a> <a id="17831" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17854" class="Keyword">open</a> <a id="17859" class="Keyword">import</a> <a id="17866" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17893" class="Keyword">open</a> <a id="17898" class="Keyword">import</a> <a id="17905" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17938" class="Keyword">open</a> <a id="17943" class="Keyword">import</a> <a id="17950" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17990" class="Keyword">open</a> <a id="17995" class="Keyword">import</a> <a id="18002" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18023" class="Keyword">open</a> <a id="18028" class="Keyword">import</a> <a id="18035" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18064" class="Keyword">open</a> <a id="18069" class="Keyword">import</a> <a id="18076" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18114" class="Keyword">open</a> <a id="18119" class="Keyword">import</a> <a id="18126" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18146" class="Keyword">open</a> <a id="18151" class="Keyword">import</a> <a id="18158" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18182" class="Keyword">open</a> <a id="18187" class="Keyword">import</a> <a id="18194" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18221" class="Keyword">open</a> <a id="18226" class="Keyword">import</a> <a id="18233" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18265" class="Keyword">open</a> <a id="18270" class="Keyword">import</a> <a id="18277" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18307" class="Keyword">open</a> <a id="18312" class="Keyword">import</a> <a id="18319" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18345" class="Keyword">open</a> <a id="18350" class="Keyword">import</a> <a id="18357" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18384" class="Keyword">open</a> <a id="18389" class="Keyword">import</a> <a id="18396" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18425" class="Keyword">open</a> <a id="18430" class="Keyword">import</a> <a id="18437" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18460" class="Keyword">open</a> <a id="18465" class="Keyword">import</a> <a id="18472" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18523" class="Keyword">open</a> <a id="18528" class="Keyword">import</a> <a id="18535" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18578" class="Keyword">open</a> <a id="18583" class="Keyword">import</a> <a id="18590" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="18642" class="Keyword">open</a> <a id="18647" class="Keyword">import</a> <a id="18654" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18702" class="Keyword">open</a> <a id="18707" class="Keyword">import</a> <a id="18714" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18752" class="Keyword">open</a> <a id="18757" class="Keyword">import</a> <a id="18764" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18801" class="Keyword">open</a> <a id="18806" class="Keyword">import</a> <a id="18813" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18859" class="Keyword">open</a> <a id="18864" class="Keyword">import</a> <a id="18871" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18888" class="Keyword">open</a> <a id="18893" class="Keyword">import</a> <a id="18900" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18928" class="Keyword">open</a> <a id="18933" class="Keyword">import</a> <a id="18940" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18968" class="Keyword">open</a> <a id="18973" class="Keyword">import</a> <a id="18980" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19016" class="Keyword">open</a> <a id="19021" class="Keyword">import</a> <a id="19028" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19066" class="Keyword">open</a> <a id="19071" class="Keyword">import</a> <a id="19078" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19111" class="Keyword">open</a> <a id="19116" class="Keyword">import</a> <a id="19123" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19144" class="Keyword">open</a> <a id="19149" class="Keyword">import</a> <a id="19156" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19192" class="Keyword">open</a> <a id="19197" class="Keyword">import</a> <a id="19204" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19258" class="Keyword">open</a> <a id="19263" class="Keyword">import</a> <a id="19270" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19292" class="Keyword">open</a> <a id="19297" class="Keyword">import</a> <a id="19304" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19339" class="Keyword">open</a> <a id="19344" class="Keyword">import</a> <a id="19351" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19381" class="Keyword">open</a> <a id="19386" class="Keyword">import</a> <a id="19393" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19432" class="Keyword">open</a> <a id="19437" class="Keyword">import</a> <a id="19444" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19498" class="Keyword">open</a> <a id="19503" class="Keyword">import</a> <a id="19510" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19556" class="Keyword">open</a> <a id="19561" class="Keyword">import</a> <a id="19568" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19619" class="Keyword">open</a> <a id="19624" class="Keyword">import</a> <a id="19631" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19672" class="Keyword">open</a> <a id="19677" class="Keyword">import</a> <a id="19684" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19729" class="Keyword">open</a> <a id="19734" class="Keyword">import</a> <a id="19741" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19786" class="Keyword">open</a> <a id="19791" class="Keyword">import</a> <a id="19798" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19834" class="Keyword">open</a> <a id="19839" class="Keyword">import</a> <a id="19846" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19882" class="Keyword">open</a> <a id="19887" class="Keyword">import</a> <a id="19894" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19959" class="Keyword">open</a> <a id="19964" class="Keyword">import</a> <a id="19971" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20026" class="Keyword">open</a> <a id="20031" class="Keyword">import</a> <a id="20038" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20078" class="Keyword">open</a> <a id="20083" class="Keyword">import</a> <a id="20090" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20134" class="Keyword">open</a> <a id="20139" class="Keyword">import</a> <a id="20146" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20191" class="Keyword">open</a> <a id="20196" class="Keyword">import</a> <a id="20203" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20244" class="Keyword">open</a> <a id="20249" class="Keyword">import</a> <a id="20256" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20296" class="Keyword">open</a> <a id="20301" class="Keyword">import</a> <a id="20308" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20335" class="Keyword">open</a> <a id="20340" class="Keyword">import</a> <a id="20347" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20383" class="Keyword">open</a> <a id="20388" class="Keyword">import</a> <a id="20395" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20422" class="Keyword">open</a> <a id="20427" class="Keyword">import</a> <a id="20434" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20471" class="Keyword">open</a> <a id="20476" class="Keyword">import</a> <a id="20483" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20511" class="Keyword">open</a> <a id="20516" class="Keyword">import</a> <a id="20523" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20542" class="Keyword">open</a> <a id="20547" class="Keyword">import</a> <a id="20554" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20594" class="Keyword">open</a> <a id="20599" class="Keyword">import</a> <a id="20606" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20638" class="Keyword">open</a> <a id="20643" class="Keyword">import</a> <a id="20650" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20698" class="Keyword">open</a> <a id="20703" class="Keyword">import</a> <a id="20710" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20733" class="Keyword">open</a> <a id="20738" class="Keyword">import</a> <a id="20745" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20769" class="Keyword">open</a> <a id="20774" class="Keyword">import</a> <a id="20781" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20821" class="Keyword">open</a> <a id="20826" class="Keyword">import</a> <a id="20833" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20876" class="Keyword">open</a> <a id="20881" class="Keyword">import</a> <a id="20888" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20922" class="Keyword">open</a> <a id="20927" class="Keyword">import</a> <a id="20934" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20966" class="Keyword">open</a> <a id="20971" class="Keyword">import</a> <a id="20978" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21008" class="Keyword">open</a> <a id="21013" class="Keyword">import</a> <a id="21020" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21054" class="Keyword">open</a> <a id="21059" class="Keyword">import</a> <a id="21066" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21101" class="Keyword">open</a> <a id="21106" class="Keyword">import</a> <a id="21113" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21150" class="Keyword">open</a> <a id="21155" class="Keyword">import</a> <a id="21162" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21189" class="Keyword">open</a> <a id="21194" class="Keyword">import</a> <a id="21201" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21229" class="Keyword">open</a> <a id="21234" class="Keyword">import</a> <a id="21241" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21290" class="Keyword">open</a> <a id="21295" class="Keyword">import</a> <a id="21302" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21348" class="Keyword">open</a> <a id="21353" class="Keyword">import</a> <a id="21360" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21400" class="Keyword">open</a> <a id="21405" class="Keyword">import</a> <a id="21412" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21450" class="Keyword">open</a> <a id="21455" class="Keyword">import</a> <a id="21462" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21491" class="Keyword">open</a> <a id="21496" class="Keyword">import</a> <a id="21503" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21533" class="Keyword">open</a> <a id="21538" class="Keyword">import</a> <a id="21545" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21576" class="Keyword">open</a> <a id="21581" class="Keyword">import</a> <a id="21588" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21628" class="Keyword">open</a> <a id="21633" class="Keyword">import</a> <a id="21640" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21666" class="Keyword">open</a> <a id="21671" class="Keyword">import</a> <a id="21678" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21733" class="Keyword">open</a> <a id="21738" class="Keyword">import</a> <a id="21745" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21796" class="Keyword">open</a> <a id="21801" class="Keyword">import</a> <a id="21808" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21853" class="Keyword">open</a> <a id="21858" class="Keyword">import</a> <a id="21865" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21919" class="Keyword">open</a> <a id="21924" class="Keyword">import</a> <a id="21931" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21958" class="Keyword">open</a> <a id="21963" class="Keyword">import</a> <a id="21970" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22003" class="Keyword">open</a> <a id="22008" class="Keyword">import</a> <a id="22015" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22046" class="Keyword">open</a> <a id="22051" class="Keyword">import</a> <a id="22058" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22095" class="Keyword">open</a> <a id="22100" class="Keyword">import</a> <a id="22107" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22132" class="Keyword">open</a> <a id="22137" class="Keyword">import</a> <a id="22144" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22176" class="Keyword">open</a> <a id="22181" class="Keyword">import</a> <a id="22188" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22223" class="Keyword">open</a> <a id="22228" class="Keyword">import</a> <a id="22235" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22264" class="Keyword">open</a> <a id="22269" class="Keyword">import</a> <a id="22276" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22302" class="Keyword">open</a> <a id="22307" class="Keyword">import</a> <a id="22314" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22342" class="Keyword">open</a> <a id="22347" class="Keyword">import</a> <a id="22354" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22379" class="Keyword">open</a> <a id="22384" class="Keyword">import</a> <a id="22391" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22412" class="Keyword">open</a> <a id="22417" class="Keyword">import</a> <a id="22424" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22460" class="Keyword">open</a> <a id="22465" class="Keyword">import</a> <a id="22472" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22515" class="Keyword">open</a> <a id="22520" class="Keyword">import</a> <a id="22527" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22552" class="Keyword">open</a> <a id="22557" class="Keyword">import</a> <a id="22564" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22595" class="Keyword">open</a> <a id="22600" class="Keyword">import</a> <a id="22607" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22639" class="Keyword">open</a> <a id="22644" class="Keyword">import</a> <a id="22651" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22685" class="Keyword">open</a> <a id="22690" class="Keyword">import</a> <a id="22697" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22753" class="Keyword">open</a> <a id="22758" class="Keyword">import</a> <a id="22765" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22818" class="Keyword">open</a> <a id="22823" class="Keyword">import</a> <a id="22830" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22857" class="Keyword">open</a> <a id="22862" class="Keyword">import</a> <a id="22869" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22914" class="Keyword">open</a> <a id="22919" class="Keyword">import</a> <a id="22926" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22988" class="Keyword">open</a> <a id="22993" class="Keyword">import</a> <a id="23000" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23013" class="Keyword">open</a> <a id="23018" class="Keyword">import</a> <a id="23025" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23065" class="Keyword">open</a> <a id="23070" class="Keyword">import</a> <a id="23077" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23121" class="Keyword">open</a> <a id="23126" class="Keyword">import</a> <a id="23133" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23172" class="Keyword">open</a> <a id="23177" class="Keyword">import</a> <a id="23184" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23226" class="Keyword">open</a> <a id="23231" class="Keyword">import</a> <a id="23238" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23278" class="Keyword">open</a> <a id="23283" class="Keyword">import</a> <a id="23290" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23331" class="Keyword">open</a> <a id="23336" class="Keyword">import</a> <a id="23343" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23381" class="Keyword">open</a> <a id="23386" class="Keyword">import</a> <a id="23393" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23456" class="Keyword">open</a> <a id="23461" class="Keyword">import</a> <a id="23468" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23497" class="Keyword">open</a> <a id="23502" class="Keyword">import</a> <a id="23509" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23554" class="Keyword">open</a> <a id="23559" class="Keyword">import</a> <a id="23566" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23608" class="Keyword">open</a> <a id="23613" class="Keyword">import</a> <a id="23620" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23664" class="Keyword">open</a> <a id="23669" class="Keyword">import</a> <a id="23676" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23725" class="Keyword">open</a> <a id="23730" class="Keyword">import</a> <a id="23737" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23787" class="Keyword">open</a> <a id="23792" class="Keyword">import</a> <a id="23799" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23826" class="Keyword">open</a> <a id="23831" class="Keyword">import</a> <a id="23838" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="23863" class="Keyword">open</a> <a id="23868" class="Keyword">import</a> <a id="23875" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23916" class="Keyword">open</a> <a id="23921" class="Keyword">import</a> <a id="23928" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23951" class="Keyword">open</a> <a id="23956" class="Keyword">import</a> <a id="23963" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24012" class="Keyword">open</a> <a id="24017" class="Keyword">import</a> <a id="24024" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24063" class="Keyword">open</a> <a id="24068" class="Keyword">import</a> <a id="24075" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24116" class="Keyword">open</a> <a id="24121" class="Keyword">import</a> <a id="24128" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24172" class="Keyword">open</a> <a id="24177" class="Keyword">import</a> <a id="24184" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24221" class="Keyword">open</a> <a id="24226" class="Keyword">import</a> <a id="24233" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24255" class="Keyword">open</a> <a id="24260" class="Keyword">import</a> <a id="24267" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24297" class="Keyword">open</a> <a id="24302" class="Keyword">import</a> <a id="24309" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24348" class="Keyword">open</a> <a id="24353" class="Keyword">import</a> <a id="24360" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24398" class="Keyword">open</a> <a id="24403" class="Keyword">import</a> <a id="24410" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24468" class="Keyword">open</a> <a id="24473" class="Keyword">import</a> <a id="24480" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24545" class="Keyword">open</a> <a id="24550" class="Keyword">import</a> <a id="24557" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24588" class="Keyword">open</a> <a id="24593" class="Keyword">import</a> <a id="24600" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24627" class="Keyword">open</a> <a id="24632" class="Keyword">import</a> <a id="24639" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24697" class="Keyword">open</a> <a id="24702" class="Keyword">import</a> <a id="24709" href="group-theory.html" class="Module">group-theory</a>
<a id="24722" class="Keyword">open</a> <a id="24727" class="Keyword">import</a> <a id="24734" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24762" class="Keyword">open</a> <a id="24767" class="Keyword">import</a> <a id="24774" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24825" class="Keyword">open</a> <a id="24830" class="Keyword">import</a> <a id="24837" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24870" class="Keyword">open</a> <a id="24875" class="Keyword">import</a> <a id="24882" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24929" class="Keyword">open</a> <a id="24934" class="Keyword">import</a> <a id="24941" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24980" class="Keyword">open</a> <a id="24985" class="Keyword">import</a> <a id="24992" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25032" class="Keyword">open</a> <a id="25037" class="Keyword">import</a> <a id="25044" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25087" class="Keyword">open</a> <a id="25092" class="Keyword">import</a> <a id="25099" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25131" class="Keyword">open</a> <a id="25136" class="Keyword">import</a> <a id="25143" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25179" class="Keyword">open</a> <a id="25184" class="Keyword">import</a> <a id="25191" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25220" class="Keyword">open</a> <a id="25225" class="Keyword">import</a> <a id="25232" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25260" class="Keyword">open</a> <a id="25265" class="Keyword">import</a> <a id="25272" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25305" class="Keyword">open</a> <a id="25310" class="Keyword">import</a> <a id="25317" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25353" class="Keyword">open</a> <a id="25358" class="Keyword">import</a> <a id="25365" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25394" class="Keyword">open</a> <a id="25399" class="Keyword">import</a> <a id="25406" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25431" class="Keyword">open</a> <a id="25436" class="Keyword">import</a> <a id="25443" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25505" class="Keyword">open</a> <a id="25510" class="Keyword">import</a> <a id="25517" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25548" class="Keyword">open</a> <a id="25553" class="Keyword">import</a> <a id="25560" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25607" class="Keyword">open</a> <a id="25612" class="Keyword">import</a> <a id="25619" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25652" class="Keyword">open</a> <a id="25657" class="Keyword">import</a> <a id="25664" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="25713" class="Keyword">open</a> <a id="25718" class="Keyword">import</a> <a id="25725" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25765" class="Keyword">open</a> <a id="25770" class="Keyword">import</a> <a id="25777" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25814" class="Keyword">open</a> <a id="25819" class="Keyword">import</a> <a id="25826" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="25873" class="Keyword">open</a> <a id="25878" class="Keyword">import</a> <a id="25885" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="25926" class="Keyword">open</a> <a id="25931" class="Keyword">import</a> <a id="25938" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="25977" class="Keyword">open</a> <a id="25982" class="Keyword">import</a> <a id="25989" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="26021" class="Keyword">open</a> <a id="26026" class="Keyword">import</a> <a id="26033" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="26060" class="Keyword">open</a> <a id="26065" class="Keyword">import</a> <a id="26072" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26092" class="Keyword">open</a> <a id="26097" class="Keyword">import</a> <a id="26104" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26138" class="Keyword">open</a> <a id="26143" class="Keyword">import</a> <a id="26150" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26177" class="Keyword">open</a> <a id="26182" class="Keyword">import</a> <a id="26189" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26231" class="Keyword">open</a> <a id="26236" class="Keyword">import</a> <a id="26243" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26293" class="Keyword">open</a> <a id="26298" class="Keyword">import</a> <a id="26305" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26352" class="Keyword">open</a> <a id="26357" class="Keyword">import</a> <a id="26364" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="26405" class="Keyword">open</a> <a id="26410" class="Keyword">import</a> <a id="26417" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26451" class="Keyword">open</a> <a id="26456" class="Keyword">import</a> <a id="26463" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="26504" class="Keyword">open</a> <a id="26509" class="Keyword">import</a> <a id="26516" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="26551" class="Keyword">open</a> <a id="26556" class="Keyword">import</a> <a id="26563" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="26601" class="Keyword">open</a> <a id="26606" class="Keyword">import</a> <a id="26613" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="26648" class="Keyword">open</a> <a id="26653" class="Keyword">import</a> <a id="26660" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26692" class="Keyword">open</a> <a id="26697" class="Keyword">import</a> <a id="26704" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="26745" class="Keyword">open</a> <a id="26750" class="Keyword">import</a> <a id="26757" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="26798" class="Keyword">open</a> <a id="26803" class="Keyword">import</a> <a id="26810" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26850" class="Keyword">open</a> <a id="26855" class="Keyword">import</a> <a id="26862" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26895" class="Keyword">open</a> <a id="26900" class="Keyword">import</a> <a id="26907" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="26944" class="Keyword">open</a> <a id="26949" class="Keyword">import</a> <a id="26956" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="26986" class="Keyword">open</a> <a id="26991" class="Keyword">import</a> <a id="26998" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="27019" class="Keyword">open</a> <a id="27024" class="Keyword">import</a> <a id="27031" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="27085" class="Keyword">open</a> <a id="27090" class="Keyword">import</a> <a id="27097" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27142" class="Keyword">open</a> <a id="27147" class="Keyword">import</a> <a id="27154" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27182" class="Keyword">open</a> <a id="27187" class="Keyword">import</a> <a id="27194" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27215" class="Keyword">open</a> <a id="27220" class="Keyword">import</a> <a id="27227" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27270" class="Keyword">open</a> <a id="27275" class="Keyword">import</a> <a id="27282" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27316" class="Keyword">open</a> <a id="27321" class="Keyword">import</a> <a id="27328" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27358" class="Keyword">open</a> <a id="27363" class="Keyword">import</a> <a id="27370" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="27416" class="Keyword">open</a> <a id="27421" class="Keyword">import</a> <a id="27428" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="27482" class="Keyword">open</a> <a id="27487" class="Keyword">import</a> <a id="27494" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="27537" class="Keyword">open</a> <a id="27542" class="Keyword">import</a> <a id="27549" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="27583" class="Keyword">open</a> <a id="27588" class="Keyword">import</a> <a id="27595" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="27636" class="Keyword">open</a> <a id="27641" class="Keyword">import</a> <a id="27648" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="27683" class="Keyword">open</a> <a id="27688" class="Keyword">import</a> <a id="27695" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="27737" class="Keyword">open</a> <a id="27742" class="Keyword">import</a> <a id="27749" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="27784" class="Keyword">open</a> <a id="27789" class="Keyword">import</a> <a id="27796" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="27835" class="Keyword">open</a> <a id="27840" class="Keyword">import</a> <a id="27847" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="27884" class="Keyword">open</a> <a id="27889" class="Keyword">import</a> <a id="27896" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="27943" class="Keyword">open</a> <a id="27948" class="Keyword">import</a> <a id="27955" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="28019" class="Keyword">open</a> <a id="28024" class="Keyword">import</a> <a id="28031" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="28055" class="Keyword">open</a> <a id="28060" class="Keyword">import</a> <a id="28067" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="28092" class="Keyword">open</a> <a id="28097" class="Keyword">import</a> <a id="28104" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28147" class="Keyword">open</a> <a id="28152" class="Keyword">import</a> <a id="28159" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28190" class="Keyword">open</a> <a id="28195" class="Keyword">import</a> <a id="28202" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28256" class="Keyword">open</a> <a id="28261" class="Keyword">import</a> <a id="28268" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28291" class="Keyword">open</a> <a id="28296" class="Keyword">import</a> <a id="28303" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="28341" class="Keyword">open</a> <a id="28346" class="Keyword">import</a> <a id="28353" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="28392" class="Keyword">open</a> <a id="28397" class="Keyword">import</a> <a id="28404" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="28455" class="Keyword">open</a> <a id="28460" class="Keyword">import</a> <a id="28467" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="28504" class="Keyword">open</a> <a id="28509" class="Keyword">import</a> <a id="28516" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="28573" class="Keyword">open</a> <a id="28578" class="Keyword">import</a> <a id="28585" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="28633" class="Keyword">open</a> <a id="28638" class="Keyword">import</a> <a id="28645" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="28675" class="Keyword">open</a> <a id="28680" class="Keyword">import</a> <a id="28687" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="28724" class="Keyword">open</a> <a id="28729" class="Keyword">import</a> <a id="28736" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="28757" class="Keyword">open</a> <a id="28762" class="Keyword">import</a> <a id="28769" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="28816" class="Keyword">open</a> <a id="28821" class="Keyword">import</a> <a id="28828" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="28866" class="Keyword">open</a> <a id="28871" class="Keyword">import</a> <a id="28878" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="28972" class="Keyword">open</a> <a id="28977" class="Keyword">import</a> <a id="28984" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="28999" class="Keyword">open</a> <a id="29004" class="Keyword">import</a> <a id="29011" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="29044" class="Keyword">open</a> <a id="29049" class="Keyword">import</a> <a id="29056" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="29088" class="Keyword">open</a> <a id="29093" class="Keyword">import</a> <a id="29100" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29142" class="Keyword">open</a> <a id="29147" class="Keyword">import</a> <a id="29154" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29192" class="Keyword">open</a> <a id="29197" class="Keyword">import</a> <a id="29204" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29241" class="Keyword">open</a> <a id="29246" class="Keyword">import</a> <a id="29253" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29286" class="Keyword">open</a> <a id="29291" class="Keyword">import</a> <a id="29298" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="29322" class="Keyword">open</a> <a id="29327" class="Keyword">import</a> <a id="29334" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="29373" class="Keyword">open</a> <a id="29378" class="Keyword">import</a> <a id="29385" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="29431" class="Keyword">open</a> <a id="29436" class="Keyword">import</a> <a id="29443" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="29488" class="Keyword">open</a> <a id="29493" class="Keyword">import</a> <a id="29500" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="29538" class="Keyword">open</a> <a id="29543" class="Keyword">import</a> <a id="29550" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="29582" class="Keyword">open</a> <a id="29587" class="Keyword">import</a> <a id="29594" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="29647" class="Keyword">open</a> <a id="29652" class="Keyword">import</a> <a id="29659" href="order-theory.html" class="Module">order-theory</a>
<a id="29672" class="Keyword">open</a> <a id="29677" class="Keyword">import</a> <a id="29684" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="29711" class="Keyword">open</a> <a id="29716" class="Keyword">import</a> <a id="29723" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="29753" class="Keyword">open</a> <a id="29758" class="Keyword">import</a> <a id="29765" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="29798" class="Keyword">open</a> <a id="29803" class="Keyword">import</a> <a id="29810" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="29846" class="Keyword">open</a> <a id="29851" class="Keyword">import</a> <a id="29858" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="29893" class="Keyword">open</a> <a id="29898" class="Keyword">import</a> <a id="29905" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="29932" class="Keyword">open</a> <a id="29937" class="Keyword">import</a> <a id="29944" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="29974" class="Keyword">open</a> <a id="29979" class="Keyword">import</a> <a id="29986" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="30022" class="Keyword">open</a> <a id="30027" class="Keyword">import</a> <a id="30034" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="30076" class="Keyword">open</a> <a id="30081" class="Keyword">import</a> <a id="30088" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="30120" class="Keyword">open</a> <a id="30125" class="Keyword">import</a> <a id="30132" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30163" class="Keyword">open</a> <a id="30168" class="Keyword">import</a> <a id="30175" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30201" class="Keyword">open</a> <a id="30206" class="Keyword">import</a> <a id="30213" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30242" class="Keyword">open</a> <a id="30247" class="Keyword">import</a> <a id="30254" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30291" class="Keyword">open</a> <a id="30296" class="Keyword">import</a> <a id="30303" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="30343" class="Keyword">open</a> <a id="30348" class="Keyword">import</a> <a id="30355" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="30377" class="Keyword">open</a> <a id="30382" class="Keyword">import</a> <a id="30389" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="30424" class="Keyword">open</a> <a id="30429" class="Keyword">import</a> <a id="30436" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="30474" class="Keyword">open</a> <a id="30479" class="Keyword">import</a> <a id="30486" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="30525" class="Keyword">open</a> <a id="30530" class="Keyword">import</a> <a id="30537" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="30572" class="Keyword">open</a> <a id="30577" class="Keyword">import</a> <a id="30584" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="30619" class="Keyword">open</a> <a id="30624" class="Keyword">import</a> <a id="30631" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="30669" class="Keyword">open</a> <a id="30674" class="Keyword">import</a> <a id="30681" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="30712" class="Keyword">open</a> <a id="30717" class="Keyword">import</a> <a id="30724" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="30766" class="Keyword">open</a> <a id="30771" class="Keyword">import</a> <a id="30778" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="30823" class="Keyword">open</a> <a id="30828" class="Keyword">import</a> <a id="30835" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="30868" class="Keyword">open</a> <a id="30873" class="Keyword">import</a> <a id="30880" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="30900" class="Keyword">open</a> <a id="30905" class="Keyword">import</a> <a id="30912" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="30935" class="Keyword">open</a> <a id="30940" class="Keyword">import</a> <a id="30947" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="30970" class="Keyword">open</a> <a id="30975" class="Keyword">import</a> <a id="30982" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="31008" class="Keyword">open</a> <a id="31013" class="Keyword">import</a> <a id="31020" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="31046" class="Keyword">open</a> <a id="31051" class="Keyword">import</a> <a id="31058" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="31122" class="Keyword">open</a> <a id="31127" class="Keyword">import</a> <a id="31134" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31152" class="Keyword">open</a> <a id="31157" class="Keyword">import</a> <a id="31164" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31191" class="Keyword">open</a> <a id="31196" class="Keyword">import</a> <a id="31203" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31229" class="Keyword">open</a> <a id="31234" class="Keyword">import</a> <a id="31241" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31267" class="Keyword">open</a> <a id="31272" class="Keyword">import</a> <a id="31279" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31305" class="Keyword">open</a> <a id="31310" class="Keyword">import</a> <a id="31317" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="31348" class="Keyword">open</a> <a id="31353" class="Keyword">import</a> <a id="31360" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="31423" class="Keyword">open</a> <a id="31428" class="Keyword">import</a> <a id="31435" href="polytopes.html" class="Module">polytopes</a>
<a id="31445" class="Keyword">open</a> <a id="31450" class="Keyword">import</a> <a id="31457" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="31515" class="Keyword">open</a> <a id="31520" class="Keyword">import</a> <a id="31527" href="ring-theory.html" class="Module">ring-theory</a>
<a id="31539" class="Keyword">open</a> <a id="31544" class="Keyword">import</a> <a id="31551" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="31588" class="Keyword">open</a> <a id="31593" class="Keyword">import</a> <a id="31600" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="31627" class="Keyword">open</a> <a id="31632" class="Keyword">import</a> <a id="31639" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="31671" class="Keyword">open</a> <a id="31676" class="Keyword">import</a> <a id="31683" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="31729" class="Keyword">open</a> <a id="31734" class="Keyword">import</a> <a id="31741" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="31766" class="Keyword">open</a> <a id="31771" class="Keyword">import</a> <a id="31778" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="31821" class="Keyword">open</a> <a id="31826" class="Keyword">import</a> <a id="31833" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="31871" class="Keyword">open</a> <a id="31876" class="Keyword">import</a> <a id="31883" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="31914" class="Keyword">open</a> <a id="31919" class="Keyword">import</a> <a id="31926" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="31950" class="Keyword">open</a> <a id="31955" class="Keyword">import</a> <a id="31962" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="31994" class="Keyword">open</a> <a id="31999" class="Keyword">import</a> <a id="32006" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="32032" class="Keyword">open</a> <a id="32037" class="Keyword">import</a> <a id="32044" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="32073" class="Keyword">open</a> <a id="32078" class="Keyword">import</a> <a id="32085" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="32122" class="Keyword">open</a> <a id="32127" class="Keyword">import</a> <a id="32134" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32163" class="Keyword">open</a> <a id="32168" class="Keyword">import</a> <a id="32175" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32202" class="Keyword">open</a> <a id="32207" class="Keyword">import</a> <a id="32214" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32251" class="Keyword">open</a> <a id="32256" class="Keyword">import</a> <a id="32263" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32290" class="Keyword">open</a> <a id="32295" class="Keyword">import</a> <a id="32302" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="32335" class="Keyword">open</a> <a id="32340" class="Keyword">import</a> <a id="32347" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="32365" class="Keyword">open</a> <a id="32370" class="Keyword">import</a> <a id="32377" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="32431" class="Keyword">open</a> <a id="32436" class="Keyword">import</a> <a id="32443" href="set-theory.html" class="Module">set-theory</a>
<a id="32454" class="Keyword">open</a> <a id="32459" class="Keyword">import</a> <a id="32466" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="32489" class="Keyword">open</a> <a id="32494" class="Keyword">import</a> <a id="32501" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="32525" class="Keyword">open</a> <a id="32530" class="Keyword">import</a> <a id="32537" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="32563" class="Keyword">open</a> <a id="32568" class="Keyword">import</a> <a id="32575" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="32637" class="Keyword">open</a> <a id="32642" class="Keyword">import</a> <a id="32649" href="structured-types.html" class="Module">structured-types</a>
<a id="32666" class="Keyword">open</a> <a id="32671" class="Keyword">import</a> <a id="32678" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="32713" class="Keyword">open</a> <a id="32718" class="Keyword">import</a> <a id="32725" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="32769" class="Keyword">open</a> <a id="32774" class="Keyword">import</a> <a id="32781" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="32845" class="Keyword">open</a> <a id="32850" class="Keyword">import</a> <a id="32857" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="32896" class="Keyword">open</a> <a id="32901" class="Keyword">import</a> <a id="32908" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="32954" class="Keyword">open</a> <a id="32959" class="Keyword">import</a> <a id="32966" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="32990" class="Keyword">open</a> <a id="32995" class="Keyword">import</a> <a id="33002" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="33071" class="Keyword">open</a> <a id="33076" class="Keyword">import</a> <a id="33083" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="33128" class="Keyword">open</a> <a id="33133" class="Keyword">import</a> <a id="33140" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33174" class="Keyword">open</a> <a id="33179" class="Keyword">import</a> <a id="33186" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33247" class="Keyword">open</a> <a id="33252" class="Keyword">import</a> <a id="33259" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33304" class="Keyword">open</a> <a id="33309" class="Keyword">import</a> <a id="33316" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="33354" class="Keyword">open</a> <a id="33359" class="Keyword">import</a> <a id="33366" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="33409" class="Keyword">open</a> <a id="33414" class="Keyword">import</a> <a id="33421" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="33457" class="Keyword">open</a> <a id="33462" class="Keyword">import</a> <a id="33469" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="33499" class="Keyword">open</a> <a id="33504" class="Keyword">import</a> <a id="33511" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="33542" class="Keyword">open</a> <a id="33547" class="Keyword">import</a> <a id="33554" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="33613" class="Keyword">open</a> <a id="33618" class="Keyword">import</a> <a id="33625" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="33676" class="Keyword">open</a> <a id="33681" class="Keyword">import</a> <a id="33688" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="33739" class="Keyword">open</a> <a id="33744" class="Keyword">import</a> <a id="33751" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="33806" class="Keyword">open</a> <a id="33811" class="Keyword">import</a> <a id="33818" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="33847" class="Keyword">open</a> <a id="33852" class="Keyword">import</a> <a id="33859" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="33887" class="Keyword">open</a> <a id="33892" class="Keyword">import</a> <a id="33899" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="33929" class="Keyword">open</a> <a id="33934" class="Keyword">import</a> <a id="33941" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="33975" class="Keyword">open</a> <a id="33980" class="Keyword">import</a> <a id="33987" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="34063" class="Keyword">open</a> <a id="34068" class="Keyword">import</a> <a id="34075" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="34101" class="Keyword">open</a> <a id="34106" class="Keyword">import</a> <a id="34113" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="34152" class="Keyword">open</a> <a id="34157" class="Keyword">import</a> <a id="34164" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34202" class="Keyword">open</a> <a id="34207" class="Keyword">import</a> <a id="34214" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34260" class="Keyword">open</a> <a id="34265" class="Keyword">import</a> <a id="34272" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34309" class="Keyword">open</a> <a id="34314" class="Keyword">import</a> <a id="34321" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34361" class="Keyword">open</a> <a id="34366" class="Keyword">import</a> <a id="34373" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="34412" class="Keyword">open</a> <a id="34417" class="Keyword">import</a> <a id="34424" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="34457" class="Keyword">open</a> <a id="34462" class="Keyword">import</a> <a id="34469" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="34504" class="Keyword">open</a> <a id="34509" class="Keyword">import</a> <a id="34516" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="34561" class="Keyword">open</a> <a id="34566" class="Keyword">import</a> <a id="34573" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="34625" class="Keyword">open</a> <a id="34630" class="Keyword">import</a> <a id="34637" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="34690" class="Keyword">open</a> <a id="34695" class="Keyword">import</a> <a id="34702" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="34762" class="Keyword">open</a> <a id="34767" class="Keyword">import</a> <a id="34774" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="34822" class="Keyword">open</a> <a id="34827" class="Keyword">import</a> <a id="34834" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="34874" class="Keyword">open</a> <a id="34879" class="Keyword">import</a> <a id="34886" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="34933" class="Keyword">open</a> <a id="34938" class="Keyword">import</a> <a id="34945" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="34986" class="Keyword">open</a> <a id="34991" class="Keyword">import</a> <a id="34998" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="35036" class="Keyword">open</a> <a id="35041" class="Keyword">import</a> <a id="35048" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="35096" class="Keyword">open</a> <a id="35101" class="Keyword">import</a> <a id="35108" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35145" class="Keyword">open</a> <a id="35150" class="Keyword">import</a> <a id="35157" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35191" class="Keyword">open</a> <a id="35196" class="Keyword">import</a> <a id="35203" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35250" class="Keyword">open</a> <a id="35255" class="Keyword">import</a> <a id="35262" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35307" class="Keyword">open</a> <a id="35312" class="Keyword">import</a> <a id="35319" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35368" class="Keyword">open</a> <a id="35373" class="Keyword">import</a> <a id="35380" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="35457" class="Keyword">open</a> <a id="35462" class="Keyword">import</a> <a id="35469" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="35521" class="Keyword">open</a> <a id="35526" class="Keyword">import</a> <a id="35533" href="type-theories.html" class="Module">type-theories</a>
<a id="35547" class="Keyword">open</a> <a id="35552" class="Keyword">import</a> <a id="35559" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="35601" class="Keyword">open</a> <a id="35606" class="Keyword">import</a> <a id="35613" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="35651" class="Keyword">open</a> <a id="35656" class="Keyword">import</a> <a id="35663" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="35709" class="Keyword">open</a> <a id="35714" class="Keyword">import</a> <a id="35721" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="35768" class="Keyword">open</a> <a id="35773" class="Keyword">import</a> <a id="35780" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="35815" class="Keyword">open</a> <a id="35820" class="Keyword">import</a> <a id="35827" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="35905" class="Keyword">open</a> <a id="35910" class="Keyword">import</a> <a id="35917" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="35941" class="Keyword">open</a> <a id="35946" class="Keyword">import</a> <a id="35953" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="36006" class="Keyword">open</a> <a id="36011" class="Keyword">import</a> <a id="36018" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="36061" class="Keyword">open</a> <a id="36066" class="Keyword">import</a> <a id="36073" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="36113" class="Keyword">open</a> <a id="36118" class="Keyword">import</a> <a id="36125" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36164" class="Keyword">open</a> <a id="36169" class="Keyword">import</a> <a id="36176" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36210" class="Keyword">open</a> <a id="36215" class="Keyword">import</a> <a id="36222" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36270" class="Keyword">open</a> <a id="36275" class="Keyword">import</a> <a id="36282" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36333" class="Keyword">open</a> <a id="36338" class="Keyword">import</a> <a id="36345" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="36392" class="Keyword">open</a> <a id="36397" class="Keyword">import</a> <a id="36404" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="36456" class="Keyword">open</a> <a id="36461" class="Keyword">import</a> <a id="36468" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="36512" class="Keyword">open</a> <a id="36517" class="Keyword">import</a> <a id="36524" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="36564" class="Keyword">open</a> <a id="36569" class="Keyword">import</a> <a id="36576" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="36619" class="Keyword">open</a> <a id="36624" class="Keyword">import</a> <a id="36631" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="36683" class="Keyword">open</a> <a id="36688" class="Keyword">import</a> <a id="36695" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="36749" class="Keyword">open</a> <a id="36754" class="Keyword">import</a> <a id="36761" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="36809" class="Keyword">open</a> <a id="36814" class="Keyword">import</a> <a id="36821" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="36860" class="Keyword">open</a> <a id="36865" class="Keyword">import</a> <a id="36872" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="36905" class="Keyword">open</a> <a id="36910" class="Keyword">import</a> <a id="36917" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="36947" class="Keyword">open</a> <a id="36952" class="Keyword">import</a> <a id="36959" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="37010" class="Keyword">open</a> <a id="37015" class="Keyword">import</a> <a id="37022" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="37063" class="Keyword">open</a> <a id="37068" class="Keyword">import</a> <a id="37075" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="37112" class="Keyword">open</a> <a id="37117" class="Keyword">import</a> <a id="37124" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="37183" class="Keyword">open</a> <a id="37188" class="Keyword">import</a> <a id="37195" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37250" class="Keyword">open</a> <a id="37255" class="Keyword">import</a> <a id="37262" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37318" class="Keyword">open</a> <a id="37323" class="Keyword">import</a> <a id="37330" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="37377" class="Keyword">open</a> <a id="37382" class="Keyword">import</a> <a id="37389" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="37432" class="Keyword">open</a> <a id="37437" class="Keyword">import</a> <a id="37444" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="37489" class="Keyword">open</a> <a id="37494" class="Keyword">import</a> <a id="37501" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="37550" class="Keyword">open</a> <a id="37555" class="Keyword">import</a> <a id="37562" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="37613" class="Keyword">open</a> <a id="37618" class="Keyword">import</a> <a id="37625" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="37669" class="Keyword">open</a> <a id="37674" class="Keyword">import</a> <a id="37681" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="37759" class="Keyword">open</a> <a id="37764" class="Keyword">import</a> <a id="37771" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="37811" class="Keyword">open</a> <a id="37816" class="Keyword">import</a> <a id="37823" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="37880" class="Keyword">open</a> <a id="37885" class="Keyword">import</a> <a id="37892" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="37927" class="Keyword">open</a> <a id="37932" class="Keyword">import</a> <a id="37939" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="37985" class="Keyword">open</a> <a id="37990" class="Keyword">import</a> <a id="37997" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="38052" class="Keyword">open</a> <a id="38057" class="Keyword">import</a> <a id="38064" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="38107" class="Keyword">open</a> <a id="38112" class="Keyword">import</a> <a id="38119" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38164" class="Keyword">open</a> <a id="38169" class="Keyword">import</a> <a id="38176" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38235" class="Keyword">open</a> <a id="38240" class="Keyword">import</a> <a id="38247" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38284" class="Keyword">open</a> <a id="38289" class="Keyword">import</a> <a id="38296" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38338" class="Keyword">open</a> <a id="38343" class="Keyword">import</a> <a id="38350" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="38391" class="Keyword">open</a> <a id="38396" class="Keyword">import</a> <a id="38403" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="38442" class="Keyword">open</a> <a id="38447" class="Keyword">import</a> <a id="38454" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="38492" class="Keyword">open</a> <a id="38497" class="Keyword">import</a> <a id="38504" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="38556" class="Keyword">open</a> <a id="38561" class="Keyword">import</a> <a id="38568" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="38613" class="Keyword">open</a> <a id="38618" class="Keyword">import</a> <a id="38625" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="38664" class="Keyword">open</a> <a id="38669" class="Keyword">import</a> <a id="38676" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="38713" class="Keyword">open</a> <a id="38718" class="Keyword">import</a> <a id="38725" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="38774" class="Keyword">open</a> <a id="38779" class="Keyword">import</a> <a id="38786" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="38825" class="Keyword">open</a> <a id="38830" class="Keyword">import</a> <a id="38837" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="38875" class="Keyword">open</a> <a id="38880" class="Keyword">import</a> <a id="38887" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="38942" class="Keyword">open</a> <a id="38947" class="Keyword">import</a> <a id="38954" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="38993" class="Keyword">open</a> <a id="38998" class="Keyword">import</a> <a id="39005" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="39053" class="Keyword">open</a> <a id="39058" class="Keyword">import</a> <a id="39065" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="39112" class="Keyword">open</a> <a id="39117" class="Keyword">import</a> <a id="39124" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39162" class="Keyword">open</a> <a id="39167" class="Keyword">import</a> <a id="39174" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="39204" class="Keyword">open</a> <a id="39209" class="Keyword">import</a> <a id="39216" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39273" class="Keyword">open</a> <a id="39278" class="Keyword">import</a> <a id="39285" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39339" class="Keyword">open</a> <a id="39344" class="Keyword">import</a> <a id="39351" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="39381" class="Keyword">open</a> <a id="39386" class="Keyword">import</a> <a id="39393" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="39442" class="Keyword">open</a> <a id="39447" class="Keyword">import</a> <a id="39454" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="39496" class="Keyword">open</a> <a id="39501" class="Keyword">import</a> <a id="39508" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="39542" class="Keyword">open</a> <a id="39547" class="Keyword">import</a> <a id="39554" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="39617" class="Keyword">open</a> <a id="39622" class="Keyword">import</a> <a id="39629" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="39672" class="Keyword">open</a> <a id="39677" class="Keyword">import</a> <a id="39684" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="39719" class="Keyword">open</a> <a id="39724" class="Keyword">import</a> <a id="39731" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="39766" class="Keyword">open</a> <a id="39771" class="Keyword">import</a> <a id="39778" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="39818" class="Keyword">open</a> <a id="39823" class="Keyword">import</a> <a id="39830" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="39875" class="Keyword">open</a> <a id="39880" class="Keyword">import</a> <a id="39887" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="39928" class="Keyword">open</a> <a id="39933" class="Keyword">import</a> <a id="39940" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="39994" class="Keyword">open</a> <a id="39999" class="Keyword">import</a> <a id="40006" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="40056" class="Keyword">open</a> <a id="40061" class="Keyword">import</a> <a id="40068" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="40115" class="Keyword">open</a> <a id="40120" class="Keyword">import</a> <a id="40127" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40165" class="Keyword">open</a> <a id="40170" class="Keyword">import</a> <a id="40177" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40226" class="Keyword">open</a> <a id="40231" class="Keyword">import</a> <a id="40238" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40285" class="Keyword">open</a> <a id="40290" class="Keyword">import</a> <a id="40297" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40360" class="Keyword">open</a> <a id="40365" class="Keyword">import</a> <a id="40372" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="40404" class="Keyword">open</a> <a id="40409" class="Keyword">import</a> <a id="40416" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="40469" class="Keyword">open</a> <a id="40474" class="Keyword">import</a> <a id="40481" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="40527" class="Keyword">open</a> <a id="40532" class="Keyword">import</a> <a id="40539" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="40585" class="Keyword">open</a> <a id="40590" class="Keyword">import</a> <a id="40597" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="40637" class="Keyword">open</a> <a id="40642" class="Keyword">import</a> <a id="40649" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="40696" class="Keyword">open</a> <a id="40701" class="Keyword">import</a> <a id="40708" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="40756" class="Keyword">open</a> <a id="40761" class="Keyword">import</a> <a id="40768" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="40808" class="Keyword">open</a> <a id="40813" class="Keyword">import</a> <a id="40820" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="40865" class="Keyword">open</a> <a id="40870" class="Keyword">import</a> <a id="40877" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="40942" class="Keyword">open</a> <a id="40947" class="Keyword">import</a> <a id="40954" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="40999" class="Keyword">open</a> <a id="41004" class="Keyword">import</a> <a id="41011" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="41058" class="Keyword">open</a> <a id="41063" class="Keyword">import</a> <a id="41070" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="41123" class="Keyword">open</a> <a id="41128" class="Keyword">import</a> <a id="41135" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>