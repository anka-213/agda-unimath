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
<a id="11105" class="Keyword">open</a> <a id="11110" class="Keyword">import</a> <a id="11117" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11135" class="Keyword">open</a> <a id="11140" class="Keyword">import</a> <a id="11147" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11166" class="Keyword">open</a> <a id="11171" class="Keyword">import</a> <a id="11178" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11197" class="Keyword">open</a> <a id="11202" class="Keyword">import</a> <a id="11209" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11253" class="Keyword">open</a> <a id="11258" class="Keyword">import</a> <a id="11265" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11290" class="Keyword">open</a> <a id="11295" class="Keyword">import</a> <a id="11302" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11329" class="Keyword">open</a> <a id="11334" class="Keyword">import</a> <a id="11341" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11358" class="Keyword">open</a> <a id="11363" class="Keyword">import</a> <a id="11370" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11399" class="Keyword">open</a> <a id="11404" class="Keyword">import</a> <a id="11411" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11467" class="Keyword">open</a> <a id="11472" class="Keyword">import</a> <a id="11479" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11510" class="Keyword">open</a> <a id="11515" class="Keyword">import</a> <a id="11522" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11576" class="Keyword">open</a> <a id="11581" class="Keyword">import</a> <a id="11588" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11616" class="Keyword">open</a> <a id="11621" class="Keyword">import</a> <a id="11628" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11658" class="Keyword">open</a> <a id="11663" class="Keyword">import</a> <a id="11670" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11690" class="Keyword">open</a> <a id="11695" class="Keyword">import</a> <a id="11702" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11747" class="Keyword">open</a> <a id="11752" class="Keyword">import</a> <a id="11759" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11796" class="Keyword">open</a> <a id="11801" class="Keyword">import</a> <a id="11808" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11843" class="Keyword">open</a> <a id="11848" class="Keyword">import</a> <a id="11855" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11913" class="Keyword">open</a> <a id="11918" class="Keyword">import</a> <a id="11925" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11963" class="Keyword">open</a> <a id="11968" class="Keyword">import</a> <a id="11975" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12009" class="Keyword">open</a> <a id="12014" class="Keyword">import</a> <a id="12021" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12050" class="Keyword">open</a> <a id="12055" class="Keyword">import</a> <a id="12062" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12085" class="Keyword">open</a> <a id="12090" class="Keyword">import</a> <a id="12097" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12124" class="Keyword">open</a> <a id="12129" class="Keyword">import</a> <a id="12136" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12159" class="Keyword">open</a> <a id="12164" class="Keyword">import</a> <a id="12171" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12213" class="Keyword">open</a> <a id="12218" class="Keyword">import</a> <a id="12225" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12257" class="Keyword">open</a> <a id="12262" class="Keyword">import</a> <a id="12269" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12296" class="Keyword">open</a> <a id="12301" class="Keyword">import</a> <a id="12308" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12333" class="Keyword">open</a> <a id="12338" class="Keyword">import</a> <a id="12345" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12374" class="Keyword">open</a> <a id="12379" class="Keyword">import</a> <a id="12386" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12416" class="Keyword">open</a> <a id="12421" class="Keyword">import</a> <a id="12428" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12455" class="Keyword">open</a> <a id="12460" class="Keyword">import</a> <a id="12467" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12486" class="Keyword">open</a> <a id="12491" class="Keyword">import</a> <a id="12498" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12544" class="Keyword">open</a> <a id="12549" class="Keyword">import</a> <a id="12556" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12598" class="Keyword">open</a> <a id="12603" class="Keyword">import</a> <a id="12610" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12642" class="Keyword">open</a> <a id="12647" class="Keyword">import</a> <a id="12654" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12684" class="Keyword">open</a> <a id="12689" class="Keyword">import</a> <a id="12696" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="12739" class="Keyword">open</a> <a id="12744" class="Keyword">import</a> <a id="12751" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12777" class="Keyword">open</a> <a id="12782" class="Keyword">import</a> <a id="12789" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12823" class="Keyword">open</a> <a id="12828" class="Keyword">import</a> <a id="12835" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="12866" class="Keyword">open</a> <a id="12871" class="Keyword">import</a> <a id="12878" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12908" class="Keyword">open</a> <a id="12913" class="Keyword">import</a> <a id="12920" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12947" class="Keyword">open</a> <a id="12952" class="Keyword">import</a> <a id="12959" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="12997" class="Keyword">open</a> <a id="13002" class="Keyword">import</a> <a id="13009" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13041" class="Keyword">open</a> <a id="13046" class="Keyword">import</a> <a id="13053" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13087" class="Keyword">open</a> <a id="13092" class="Keyword">import</a> <a id="13099" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13122" class="Keyword">open</a> <a id="13127" class="Keyword">import</a> <a id="13134" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13161" class="Keyword">open</a> <a id="13166" class="Keyword">import</a> <a id="13173" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13201" class="Keyword">open</a> <a id="13206" class="Keyword">import</a> <a id="13213" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13250" class="Keyword">open</a> <a id="13255" class="Keyword">import</a> <a id="13262" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13310" class="Keyword">open</a> <a id="13315" class="Keyword">import</a> <a id="13322" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13362" class="Keyword">open</a> <a id="13367" class="Keyword">import</a> <a id="13374" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13396" class="Keyword">open</a> <a id="13401" class="Keyword">import</a> <a id="13408" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13431" class="Keyword">open</a> <a id="13436" class="Keyword">import</a> <a id="13443" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13468" class="Keyword">open</a> <a id="13473" class="Keyword">import</a> <a id="13480" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13525" class="Keyword">open</a> <a id="13530" class="Keyword">import</a> <a id="13537" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13581" class="Keyword">open</a> <a id="13586" class="Keyword">import</a> <a id="13593" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13629" class="Keyword">open</a> <a id="13634" class="Keyword">import</a> <a id="13641" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13686" class="Keyword">open</a> <a id="13691" class="Keyword">import</a> <a id="13698" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13739" class="Keyword">open</a> <a id="13744" class="Keyword">import</a> <a id="13751" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13786" class="Keyword">open</a> <a id="13791" class="Keyword">import</a> <a id="13798" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13830" class="Keyword">open</a> <a id="13835" class="Keyword">import</a> <a id="13842" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13873" class="Keyword">open</a> <a id="13878" class="Keyword">import</a> <a id="13885" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13918" class="Keyword">open</a> <a id="13923" class="Keyword">import</a> <a id="13930" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13963" class="Keyword">open</a> <a id="13968" class="Keyword">import</a> <a id="13975" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14005" class="Keyword">open</a> <a id="14010" class="Keyword">import</a> <a id="14017" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14041" class="Keyword">open</a> <a id="14046" class="Keyword">import</a> <a id="14053" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14091" class="Keyword">open</a> <a id="14096" class="Keyword">import</a> <a id="14103" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14134" class="Keyword">open</a> <a id="14139" class="Keyword">import</a> <a id="14146" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14171" class="Keyword">open</a> <a id="14176" class="Keyword">import</a> <a id="14183" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14211" class="Keyword">open</a> <a id="14216" class="Keyword">import</a> <a id="14223" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14247" class="Keyword">open</a> <a id="14252" class="Keyword">import</a> <a id="14259" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14285" class="Keyword">open</a> <a id="14290" class="Keyword">import</a> <a id="14297" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14332" class="Keyword">open</a> <a id="14337" class="Keyword">import</a> <a id="14344" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14365" class="Keyword">open</a> <a id="14370" class="Keyword">import</a> <a id="14377" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14426" class="Keyword">open</a> <a id="14431" class="Keyword">import</a> <a id="14438" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14479" class="Keyword">open</a> <a id="14484" class="Keyword">import</a> <a id="14491" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14541" class="Keyword">open</a> <a id="14546" class="Keyword">import</a> <a id="14553" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14599" class="Keyword">open</a> <a id="14604" class="Keyword">import</a> <a id="14611" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14651" class="Keyword">open</a> <a id="14656" class="Keyword">import</a> <a id="14663" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14713" class="Keyword">open</a> <a id="14718" class="Keyword">import</a> <a id="14725" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14764" class="Keyword">open</a> <a id="14769" class="Keyword">import</a> <a id="14776" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14816" class="Keyword">open</a> <a id="14821" class="Keyword">import</a> <a id="14828" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14861" class="Keyword">open</a> <a id="14866" class="Keyword">import</a> <a id="14873" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14922" class="Keyword">open</a> <a id="14927" class="Keyword">import</a> <a id="14934" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14959" class="Keyword">open</a> <a id="14964" class="Keyword">import</a> <a id="14971" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15009" class="Keyword">open</a> <a id="15014" class="Keyword">import</a> <a id="15021" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15043" class="Keyword">open</a> <a id="15048" class="Keyword">import</a> <a id="15055" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15083" class="Keyword">open</a> <a id="15088" class="Keyword">import</a> <a id="15095" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15131" class="Keyword">open</a> <a id="15136" class="Keyword">import</a> <a id="15143" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15169" class="Keyword">open</a> <a id="15174" class="Keyword">import</a> <a id="15181" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15199" class="Keyword">open</a> <a id="15204" class="Keyword">import</a> <a id="15211" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15246" class="Keyword">open</a> <a id="15251" class="Keyword">import</a> <a id="15258" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15293" class="Keyword">open</a> <a id="15298" class="Keyword">import</a> <a id="15305" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15332" class="Keyword">open</a> <a id="15337" class="Keyword">import</a> <a id="15344" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15400" class="Keyword">open</a> <a id="15405" class="Keyword">import</a> <a id="15412" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15441" class="Keyword">open</a> <a id="15446" class="Keyword">import</a> <a id="15453" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15483" class="Keyword">open</a> <a id="15488" class="Keyword">import</a> <a id="15495" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15522" class="Keyword">open</a> <a id="15527" class="Keyword">import</a> <a id="15534" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15560" class="Keyword">open</a> <a id="15565" class="Keyword">import</a> <a id="15572" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15599" class="Keyword">open</a> <a id="15604" class="Keyword">import</a> <a id="15611" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15635" class="Keyword">open</a> <a id="15640" class="Keyword">import</a> <a id="15647" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15670" class="Keyword">open</a> <a id="15675" class="Keyword">import</a> <a id="15682" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15709" class="Keyword">open</a> <a id="15714" class="Keyword">import</a> <a id="15721" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15753" class="Keyword">open</a> <a id="15758" class="Keyword">import</a> <a id="15765" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15800" class="Keyword">open</a> <a id="15805" class="Keyword">import</a> <a id="15812" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15843" class="Keyword">open</a> <a id="15848" class="Keyword">import</a> <a id="15855" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15888" class="Keyword">open</a> <a id="15893" class="Keyword">import</a> <a id="15900" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15934" class="Keyword">open</a> <a id="15939" class="Keyword">import</a> <a id="15946" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15986" class="Keyword">open</a> <a id="15991" class="Keyword">import</a> <a id="15998" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16029" class="Keyword">open</a> <a id="16034" class="Keyword">import</a> <a id="16041" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16073" class="Keyword">open</a> <a id="16078" class="Keyword">import</a> <a id="16085" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16116" class="Keyword">open</a> <a id="16121" class="Keyword">import</a> <a id="16128" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16145" class="Keyword">open</a> <a id="16150" class="Keyword">import</a> <a id="16157" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16182" class="Keyword">open</a> <a id="16187" class="Keyword">import</a> <a id="16194" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16223" class="Keyword">open</a> <a id="16228" class="Keyword">import</a> <a id="16235" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16260" class="Keyword">open</a> <a id="16265" class="Keyword">import</a> <a id="16272" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16293" class="Keyword">open</a> <a id="16298" class="Keyword">import</a> <a id="16305" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16329" class="Keyword">open</a> <a id="16334" class="Keyword">import</a> <a id="16341" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16361" class="Keyword">open</a> <a id="16366" class="Keyword">import</a> <a id="16373" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16407" class="Keyword">open</a> <a id="16412" class="Keyword">import</a> <a id="16419" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16457" class="Keyword">open</a> <a id="16462" class="Keyword">import</a> <a id="16469" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16497" class="Keyword">open</a> <a id="16502" class="Keyword">import</a> <a id="16509" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16533" class="Keyword">open</a> <a id="16538" class="Keyword">import</a> <a id="16545" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16572" class="Keyword">open</a> <a id="16577" class="Keyword">import</a> <a id="16584" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16619" class="Keyword">open</a> <a id="16624" class="Keyword">import</a> <a id="16631" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16652" class="Keyword">open</a> <a id="16657" class="Keyword">import</a> <a id="16664" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16700" class="Keyword">open</a> <a id="16705" class="Keyword">import</a> <a id="16712" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16757" class="Keyword">open</a> <a id="16762" class="Keyword">import</a> <a id="16769" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16815" class="Keyword">open</a> <a id="16820" class="Keyword">import</a> <a id="16827" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16867" class="Keyword">open</a> <a id="16872" class="Keyword">import</a> <a id="16879" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16909" class="Keyword">open</a> <a id="16914" class="Keyword">import</a> <a id="16921" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="16955" class="Keyword">open</a> <a id="16960" class="Keyword">import</a> <a id="16967" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17004" class="Keyword">open</a> <a id="17009" class="Keyword">import</a> <a id="17016" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17040" class="Keyword">open</a> <a id="17045" class="Keyword">import</a> <a id="17052" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17073" class="Keyword">open</a> <a id="17078" class="Keyword">import</a> <a id="17085" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17120" class="Keyword">open</a> <a id="17125" class="Keyword">import</a> <a id="17132" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17169" class="Keyword">open</a> <a id="17174" class="Keyword">import</a> <a id="17181" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17230" class="Keyword">open</a> <a id="17235" class="Keyword">import</a> <a id="17242" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17275" class="Keyword">open</a> <a id="17280" class="Keyword">import</a> <a id="17287" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17310" class="Keyword">open</a> <a id="17315" class="Keyword">import</a> <a id="17322" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17345" class="Keyword">open</a> <a id="17350" class="Keyword">import</a> <a id="17357" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17380" class="Keyword">open</a> <a id="17385" class="Keyword">import</a> <a id="17392" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17420" class="Keyword">open</a> <a id="17425" class="Keyword">import</a> <a id="17432" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17452" class="Keyword">open</a> <a id="17457" class="Keyword">import</a> <a id="17464" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17485" class="Keyword">open</a> <a id="17490" class="Keyword">import</a> <a id="17497" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17528" class="Keyword">open</a> <a id="17533" class="Keyword">import</a> <a id="17540" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17567" class="Keyword">open</a> <a id="17572" class="Keyword">import</a> <a id="17579" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17595" class="Keyword">open</a> <a id="17600" class="Keyword">import</a> <a id="17607" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17638" class="Keyword">open</a> <a id="17643" class="Keyword">import</a> <a id="17650" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17667" class="Keyword">open</a> <a id="17672" class="Keyword">import</a> <a id="17679" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17701" class="Keyword">open</a> <a id="17706" class="Keyword">import</a> <a id="17713" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17740" class="Keyword">open</a> <a id="17745" class="Keyword">import</a> <a id="17752" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17775" class="Keyword">open</a> <a id="17780" class="Keyword">import</a> <a id="17787" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17814" class="Keyword">open</a> <a id="17819" class="Keyword">import</a> <a id="17826" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17859" class="Keyword">open</a> <a id="17864" class="Keyword">import</a> <a id="17871" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17911" class="Keyword">open</a> <a id="17916" class="Keyword">import</a> <a id="17923" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17944" class="Keyword">open</a> <a id="17949" class="Keyword">import</a> <a id="17956" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17985" class="Keyword">open</a> <a id="17990" class="Keyword">import</a> <a id="17997" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18035" class="Keyword">open</a> <a id="18040" class="Keyword">import</a> <a id="18047" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18067" class="Keyword">open</a> <a id="18072" class="Keyword">import</a> <a id="18079" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18103" class="Keyword">open</a> <a id="18108" class="Keyword">import</a> <a id="18115" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18142" class="Keyword">open</a> <a id="18147" class="Keyword">import</a> <a id="18154" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18186" class="Keyword">open</a> <a id="18191" class="Keyword">import</a> <a id="18198" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18228" class="Keyword">open</a> <a id="18233" class="Keyword">import</a> <a id="18240" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18266" class="Keyword">open</a> <a id="18271" class="Keyword">import</a> <a id="18278" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18305" class="Keyword">open</a> <a id="18310" class="Keyword">import</a> <a id="18317" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18346" class="Keyword">open</a> <a id="18351" class="Keyword">import</a> <a id="18358" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18381" class="Keyword">open</a> <a id="18386" class="Keyword">import</a> <a id="18393" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18444" class="Keyword">open</a> <a id="18449" class="Keyword">import</a> <a id="18456" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18499" class="Keyword">open</a> <a id="18504" class="Keyword">import</a> <a id="18511" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18559" class="Keyword">open</a> <a id="18564" class="Keyword">import</a> <a id="18571" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18609" class="Keyword">open</a> <a id="18614" class="Keyword">import</a> <a id="18621" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18658" class="Keyword">open</a> <a id="18663" class="Keyword">import</a> <a id="18670" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18716" class="Keyword">open</a> <a id="18721" class="Keyword">import</a> <a id="18728" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18745" class="Keyword">open</a> <a id="18750" class="Keyword">import</a> <a id="18757" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18785" class="Keyword">open</a> <a id="18790" class="Keyword">import</a> <a id="18797" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18825" class="Keyword">open</a> <a id="18830" class="Keyword">import</a> <a id="18837" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18873" class="Keyword">open</a> <a id="18878" class="Keyword">import</a> <a id="18885" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18923" class="Keyword">open</a> <a id="18928" class="Keyword">import</a> <a id="18935" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18968" class="Keyword">open</a> <a id="18973" class="Keyword">import</a> <a id="18980" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19001" class="Keyword">open</a> <a id="19006" class="Keyword">import</a> <a id="19013" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19049" class="Keyword">open</a> <a id="19054" class="Keyword">import</a> <a id="19061" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19115" class="Keyword">open</a> <a id="19120" class="Keyword">import</a> <a id="19127" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19149" class="Keyword">open</a> <a id="19154" class="Keyword">import</a> <a id="19161" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19196" class="Keyword">open</a> <a id="19201" class="Keyword">import</a> <a id="19208" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19238" class="Keyword">open</a> <a id="19243" class="Keyword">import</a> <a id="19250" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19289" class="Keyword">open</a> <a id="19294" class="Keyword">import</a> <a id="19301" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19355" class="Keyword">open</a> <a id="19360" class="Keyword">import</a> <a id="19367" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19413" class="Keyword">open</a> <a id="19418" class="Keyword">import</a> <a id="19425" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19476" class="Keyword">open</a> <a id="19481" class="Keyword">import</a> <a id="19488" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19529" class="Keyword">open</a> <a id="19534" class="Keyword">import</a> <a id="19541" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19586" class="Keyword">open</a> <a id="19591" class="Keyword">import</a> <a id="19598" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19643" class="Keyword">open</a> <a id="19648" class="Keyword">import</a> <a id="19655" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19691" class="Keyword">open</a> <a id="19696" class="Keyword">import</a> <a id="19703" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19739" class="Keyword">open</a> <a id="19744" class="Keyword">import</a> <a id="19751" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19816" class="Keyword">open</a> <a id="19821" class="Keyword">import</a> <a id="19828" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19883" class="Keyword">open</a> <a id="19888" class="Keyword">import</a> <a id="19895" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19935" class="Keyword">open</a> <a id="19940" class="Keyword">import</a> <a id="19947" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19991" class="Keyword">open</a> <a id="19996" class="Keyword">import</a> <a id="20003" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20048" class="Keyword">open</a> <a id="20053" class="Keyword">import</a> <a id="20060" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20101" class="Keyword">open</a> <a id="20106" class="Keyword">import</a> <a id="20113" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20153" class="Keyword">open</a> <a id="20158" class="Keyword">import</a> <a id="20165" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20192" class="Keyword">open</a> <a id="20197" class="Keyword">import</a> <a id="20204" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20240" class="Keyword">open</a> <a id="20245" class="Keyword">import</a> <a id="20252" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20279" class="Keyword">open</a> <a id="20284" class="Keyword">import</a> <a id="20291" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20328" class="Keyword">open</a> <a id="20333" class="Keyword">import</a> <a id="20340" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20368" class="Keyword">open</a> <a id="20373" class="Keyword">import</a> <a id="20380" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20399" class="Keyword">open</a> <a id="20404" class="Keyword">import</a> <a id="20411" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20451" class="Keyword">open</a> <a id="20456" class="Keyword">import</a> <a id="20463" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20495" class="Keyword">open</a> <a id="20500" class="Keyword">import</a> <a id="20507" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20555" class="Keyword">open</a> <a id="20560" class="Keyword">import</a> <a id="20567" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20590" class="Keyword">open</a> <a id="20595" class="Keyword">import</a> <a id="20602" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20626" class="Keyword">open</a> <a id="20631" class="Keyword">import</a> <a id="20638" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20678" class="Keyword">open</a> <a id="20683" class="Keyword">import</a> <a id="20690" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20733" class="Keyword">open</a> <a id="20738" class="Keyword">import</a> <a id="20745" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20779" class="Keyword">open</a> <a id="20784" class="Keyword">import</a> <a id="20791" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20823" class="Keyword">open</a> <a id="20828" class="Keyword">import</a> <a id="20835" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20865" class="Keyword">open</a> <a id="20870" class="Keyword">import</a> <a id="20877" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20911" class="Keyword">open</a> <a id="20916" class="Keyword">import</a> <a id="20923" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20958" class="Keyword">open</a> <a id="20963" class="Keyword">import</a> <a id="20970" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21007" class="Keyword">open</a> <a id="21012" class="Keyword">import</a> <a id="21019" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21046" class="Keyword">open</a> <a id="21051" class="Keyword">import</a> <a id="21058" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21086" class="Keyword">open</a> <a id="21091" class="Keyword">import</a> <a id="21098" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21147" class="Keyword">open</a> <a id="21152" class="Keyword">import</a> <a id="21159" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21205" class="Keyword">open</a> <a id="21210" class="Keyword">import</a> <a id="21217" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21257" class="Keyword">open</a> <a id="21262" class="Keyword">import</a> <a id="21269" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21307" class="Keyword">open</a> <a id="21312" class="Keyword">import</a> <a id="21319" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21348" class="Keyword">open</a> <a id="21353" class="Keyword">import</a> <a id="21360" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21390" class="Keyword">open</a> <a id="21395" class="Keyword">import</a> <a id="21402" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21433" class="Keyword">open</a> <a id="21438" class="Keyword">import</a> <a id="21445" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21485" class="Keyword">open</a> <a id="21490" class="Keyword">import</a> <a id="21497" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21523" class="Keyword">open</a> <a id="21528" class="Keyword">import</a> <a id="21535" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21590" class="Keyword">open</a> <a id="21595" class="Keyword">import</a> <a id="21602" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21653" class="Keyword">open</a> <a id="21658" class="Keyword">import</a> <a id="21665" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21710" class="Keyword">open</a> <a id="21715" class="Keyword">import</a> <a id="21722" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21776" class="Keyword">open</a> <a id="21781" class="Keyword">import</a> <a id="21788" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21815" class="Keyword">open</a> <a id="21820" class="Keyword">import</a> <a id="21827" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21860" class="Keyword">open</a> <a id="21865" class="Keyword">import</a> <a id="21872" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21903" class="Keyword">open</a> <a id="21908" class="Keyword">import</a> <a id="21915" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21952" class="Keyword">open</a> <a id="21957" class="Keyword">import</a> <a id="21964" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21989" class="Keyword">open</a> <a id="21994" class="Keyword">import</a> <a id="22001" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22033" class="Keyword">open</a> <a id="22038" class="Keyword">import</a> <a id="22045" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22080" class="Keyword">open</a> <a id="22085" class="Keyword">import</a> <a id="22092" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22121" class="Keyword">open</a> <a id="22126" class="Keyword">import</a> <a id="22133" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22159" class="Keyword">open</a> <a id="22164" class="Keyword">import</a> <a id="22171" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22199" class="Keyword">open</a> <a id="22204" class="Keyword">import</a> <a id="22211" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22236" class="Keyword">open</a> <a id="22241" class="Keyword">import</a> <a id="22248" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22269" class="Keyword">open</a> <a id="22274" class="Keyword">import</a> <a id="22281" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22317" class="Keyword">open</a> <a id="22322" class="Keyword">import</a> <a id="22329" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22372" class="Keyword">open</a> <a id="22377" class="Keyword">import</a> <a id="22384" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22409" class="Keyword">open</a> <a id="22414" class="Keyword">import</a> <a id="22421" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22452" class="Keyword">open</a> <a id="22457" class="Keyword">import</a> <a id="22464" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22496" class="Keyword">open</a> <a id="22501" class="Keyword">import</a> <a id="22508" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22542" class="Keyword">open</a> <a id="22547" class="Keyword">import</a> <a id="22554" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22610" class="Keyword">open</a> <a id="22615" class="Keyword">import</a> <a id="22622" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22675" class="Keyword">open</a> <a id="22680" class="Keyword">import</a> <a id="22687" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22714" class="Keyword">open</a> <a id="22719" class="Keyword">import</a> <a id="22726" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22771" class="Keyword">open</a> <a id="22776" class="Keyword">import</a> <a id="22783" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22845" class="Keyword">open</a> <a id="22850" class="Keyword">import</a> <a id="22857" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22870" class="Keyword">open</a> <a id="22875" class="Keyword">import</a> <a id="22882" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="22922" class="Keyword">open</a> <a id="22927" class="Keyword">import</a> <a id="22934" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="22978" class="Keyword">open</a> <a id="22983" class="Keyword">import</a> <a id="22990" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23029" class="Keyword">open</a> <a id="23034" class="Keyword">import</a> <a id="23041" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23083" class="Keyword">open</a> <a id="23088" class="Keyword">import</a> <a id="23095" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23135" class="Keyword">open</a> <a id="23140" class="Keyword">import</a> <a id="23147" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23188" class="Keyword">open</a> <a id="23193" class="Keyword">import</a> <a id="23200" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23238" class="Keyword">open</a> <a id="23243" class="Keyword">import</a> <a id="23250" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23313" class="Keyword">open</a> <a id="23318" class="Keyword">import</a> <a id="23325" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23354" class="Keyword">open</a> <a id="23359" class="Keyword">import</a> <a id="23366" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23411" class="Keyword">open</a> <a id="23416" class="Keyword">import</a> <a id="23423" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23465" class="Keyword">open</a> <a id="23470" class="Keyword">import</a> <a id="23477" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23521" class="Keyword">open</a> <a id="23526" class="Keyword">import</a> <a id="23533" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23582" class="Keyword">open</a> <a id="23587" class="Keyword">import</a> <a id="23594" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23644" class="Keyword">open</a> <a id="23649" class="Keyword">import</a> <a id="23656" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23683" class="Keyword">open</a> <a id="23688" class="Keyword">import</a> <a id="23695" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="23720" class="Keyword">open</a> <a id="23725" class="Keyword">import</a> <a id="23732" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23773" class="Keyword">open</a> <a id="23778" class="Keyword">import</a> <a id="23785" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23808" class="Keyword">open</a> <a id="23813" class="Keyword">import</a> <a id="23820" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23869" class="Keyword">open</a> <a id="23874" class="Keyword">import</a> <a id="23881" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23920" class="Keyword">open</a> <a id="23925" class="Keyword">import</a> <a id="23932" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="23973" class="Keyword">open</a> <a id="23978" class="Keyword">import</a> <a id="23985" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24029" class="Keyword">open</a> <a id="24034" class="Keyword">import</a> <a id="24041" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24078" class="Keyword">open</a> <a id="24083" class="Keyword">import</a> <a id="24090" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24112" class="Keyword">open</a> <a id="24117" class="Keyword">import</a> <a id="24124" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24154" class="Keyword">open</a> <a id="24159" class="Keyword">import</a> <a id="24166" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24205" class="Keyword">open</a> <a id="24210" class="Keyword">import</a> <a id="24217" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24255" class="Keyword">open</a> <a id="24260" class="Keyword">import</a> <a id="24267" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24325" class="Keyword">open</a> <a id="24330" class="Keyword">import</a> <a id="24337" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24402" class="Keyword">open</a> <a id="24407" class="Keyword">import</a> <a id="24414" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24445" class="Keyword">open</a> <a id="24450" class="Keyword">import</a> <a id="24457" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24484" class="Keyword">open</a> <a id="24489" class="Keyword">import</a> <a id="24496" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24554" class="Keyword">open</a> <a id="24559" class="Keyword">import</a> <a id="24566" href="group-theory.html" class="Module">group-theory</a>
<a id="24579" class="Keyword">open</a> <a id="24584" class="Keyword">import</a> <a id="24591" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24619" class="Keyword">open</a> <a id="24624" class="Keyword">import</a> <a id="24631" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24682" class="Keyword">open</a> <a id="24687" class="Keyword">import</a> <a id="24694" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24727" class="Keyword">open</a> <a id="24732" class="Keyword">import</a> <a id="24739" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24786" class="Keyword">open</a> <a id="24791" class="Keyword">import</a> <a id="24798" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24837" class="Keyword">open</a> <a id="24842" class="Keyword">import</a> <a id="24849" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24889" class="Keyword">open</a> <a id="24894" class="Keyword">import</a> <a id="24901" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="24944" class="Keyword">open</a> <a id="24949" class="Keyword">import</a> <a id="24956" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="24988" class="Keyword">open</a> <a id="24993" class="Keyword">import</a> <a id="25000" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25036" class="Keyword">open</a> <a id="25041" class="Keyword">import</a> <a id="25048" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25077" class="Keyword">open</a> <a id="25082" class="Keyword">import</a> <a id="25089" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25117" class="Keyword">open</a> <a id="25122" class="Keyword">import</a> <a id="25129" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25162" class="Keyword">open</a> <a id="25167" class="Keyword">import</a> <a id="25174" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25210" class="Keyword">open</a> <a id="25215" class="Keyword">import</a> <a id="25222" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25251" class="Keyword">open</a> <a id="25256" class="Keyword">import</a> <a id="25263" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25288" class="Keyword">open</a> <a id="25293" class="Keyword">import</a> <a id="25300" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25362" class="Keyword">open</a> <a id="25367" class="Keyword">import</a> <a id="25374" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25405" class="Keyword">open</a> <a id="25410" class="Keyword">import</a> <a id="25417" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25464" class="Keyword">open</a> <a id="25469" class="Keyword">import</a> <a id="25476" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25509" class="Keyword">open</a> <a id="25514" class="Keyword">import</a> <a id="25521" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="25570" class="Keyword">open</a> <a id="25575" class="Keyword">import</a> <a id="25582" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25622" class="Keyword">open</a> <a id="25627" class="Keyword">import</a> <a id="25634" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25671" class="Keyword">open</a> <a id="25676" class="Keyword">import</a> <a id="25683" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="25730" class="Keyword">open</a> <a id="25735" class="Keyword">import</a> <a id="25742" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="25783" class="Keyword">open</a> <a id="25788" class="Keyword">import</a> <a id="25795" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="25834" class="Keyword">open</a> <a id="25839" class="Keyword">import</a> <a id="25846" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25878" class="Keyword">open</a> <a id="25883" class="Keyword">import</a> <a id="25890" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25917" class="Keyword">open</a> <a id="25922" class="Keyword">import</a> <a id="25929" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="25949" class="Keyword">open</a> <a id="25954" class="Keyword">import</a> <a id="25961" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="25995" class="Keyword">open</a> <a id="26000" class="Keyword">import</a> <a id="26007" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26034" class="Keyword">open</a> <a id="26039" class="Keyword">import</a> <a id="26046" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26088" class="Keyword">open</a> <a id="26093" class="Keyword">import</a> <a id="26100" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26150" class="Keyword">open</a> <a id="26155" class="Keyword">import</a> <a id="26162" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26209" class="Keyword">open</a> <a id="26214" class="Keyword">import</a> <a id="26221" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="26262" class="Keyword">open</a> <a id="26267" class="Keyword">import</a> <a id="26274" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26308" class="Keyword">open</a> <a id="26313" class="Keyword">import</a> <a id="26320" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="26361" class="Keyword">open</a> <a id="26366" class="Keyword">import</a> <a id="26373" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="26408" class="Keyword">open</a> <a id="26413" class="Keyword">import</a> <a id="26420" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="26458" class="Keyword">open</a> <a id="26463" class="Keyword">import</a> <a id="26470" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="26505" class="Keyword">open</a> <a id="26510" class="Keyword">import</a> <a id="26517" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26549" class="Keyword">open</a> <a id="26554" class="Keyword">import</a> <a id="26561" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="26602" class="Keyword">open</a> <a id="26607" class="Keyword">import</a> <a id="26614" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="26655" class="Keyword">open</a> <a id="26660" class="Keyword">import</a> <a id="26667" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26707" class="Keyword">open</a> <a id="26712" class="Keyword">import</a> <a id="26719" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26752" class="Keyword">open</a> <a id="26757" class="Keyword">import</a> <a id="26764" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="26801" class="Keyword">open</a> <a id="26806" class="Keyword">import</a> <a id="26813" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="26843" class="Keyword">open</a> <a id="26848" class="Keyword">import</a> <a id="26855" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="26876" class="Keyword">open</a> <a id="26881" class="Keyword">import</a> <a id="26888" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="26933" class="Keyword">open</a> <a id="26938" class="Keyword">import</a> <a id="26945" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="26973" class="Keyword">open</a> <a id="26978" class="Keyword">import</a> <a id="26985" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27006" class="Keyword">open</a> <a id="27011" class="Keyword">import</a> <a id="27018" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27061" class="Keyword">open</a> <a id="27066" class="Keyword">import</a> <a id="27073" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27107" class="Keyword">open</a> <a id="27112" class="Keyword">import</a> <a id="27119" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27149" class="Keyword">open</a> <a id="27154" class="Keyword">import</a> <a id="27161" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="27207" class="Keyword">open</a> <a id="27212" class="Keyword">import</a> <a id="27219" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="27273" class="Keyword">open</a> <a id="27278" class="Keyword">import</a> <a id="27285" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="27328" class="Keyword">open</a> <a id="27333" class="Keyword">import</a> <a id="27340" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="27374" class="Keyword">open</a> <a id="27379" class="Keyword">import</a> <a id="27386" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="27427" class="Keyword">open</a> <a id="27432" class="Keyword">import</a> <a id="27439" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="27474" class="Keyword">open</a> <a id="27479" class="Keyword">import</a> <a id="27486" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="27528" class="Keyword">open</a> <a id="27533" class="Keyword">import</a> <a id="27540" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="27575" class="Keyword">open</a> <a id="27580" class="Keyword">import</a> <a id="27587" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="27626" class="Keyword">open</a> <a id="27631" class="Keyword">import</a> <a id="27638" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="27675" class="Keyword">open</a> <a id="27680" class="Keyword">import</a> <a id="27687" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="27734" class="Keyword">open</a> <a id="27739" class="Keyword">import</a> <a id="27746" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="27810" class="Keyword">open</a> <a id="27815" class="Keyword">import</a> <a id="27822" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="27846" class="Keyword">open</a> <a id="27851" class="Keyword">import</a> <a id="27858" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="27883" class="Keyword">open</a> <a id="27888" class="Keyword">import</a> <a id="27895" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="27938" class="Keyword">open</a> <a id="27943" class="Keyword">import</a> <a id="27950" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="27981" class="Keyword">open</a> <a id="27986" class="Keyword">import</a> <a id="27993" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28047" class="Keyword">open</a> <a id="28052" class="Keyword">import</a> <a id="28059" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28082" class="Keyword">open</a> <a id="28087" class="Keyword">import</a> <a id="28094" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="28132" class="Keyword">open</a> <a id="28137" class="Keyword">import</a> <a id="28144" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="28183" class="Keyword">open</a> <a id="28188" class="Keyword">import</a> <a id="28195" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="28246" class="Keyword">open</a> <a id="28251" class="Keyword">import</a> <a id="28258" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="28295" class="Keyword">open</a> <a id="28300" class="Keyword">import</a> <a id="28307" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="28364" class="Keyword">open</a> <a id="28369" class="Keyword">import</a> <a id="28376" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="28424" class="Keyword">open</a> <a id="28429" class="Keyword">import</a> <a id="28436" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="28466" class="Keyword">open</a> <a id="28471" class="Keyword">import</a> <a id="28478" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="28515" class="Keyword">open</a> <a id="28520" class="Keyword">import</a> <a id="28527" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="28548" class="Keyword">open</a> <a id="28553" class="Keyword">import</a> <a id="28560" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="28607" class="Keyword">open</a> <a id="28612" class="Keyword">import</a> <a id="28619" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="28657" class="Keyword">open</a> <a id="28662" class="Keyword">import</a> <a id="28669" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="28763" class="Keyword">open</a> <a id="28768" class="Keyword">import</a> <a id="28775" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="28790" class="Keyword">open</a> <a id="28795" class="Keyword">import</a> <a id="28802" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="28835" class="Keyword">open</a> <a id="28840" class="Keyword">import</a> <a id="28847" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="28879" class="Keyword">open</a> <a id="28884" class="Keyword">import</a> <a id="28891" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="28933" class="Keyword">open</a> <a id="28938" class="Keyword">import</a> <a id="28945" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="28983" class="Keyword">open</a> <a id="28988" class="Keyword">import</a> <a id="28995" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29032" class="Keyword">open</a> <a id="29037" class="Keyword">import</a> <a id="29044" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29077" class="Keyword">open</a> <a id="29082" class="Keyword">import</a> <a id="29089" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="29113" class="Keyword">open</a> <a id="29118" class="Keyword">import</a> <a id="29125" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="29164" class="Keyword">open</a> <a id="29169" class="Keyword">import</a> <a id="29176" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="29222" class="Keyword">open</a> <a id="29227" class="Keyword">import</a> <a id="29234" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="29279" class="Keyword">open</a> <a id="29284" class="Keyword">import</a> <a id="29291" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="29329" class="Keyword">open</a> <a id="29334" class="Keyword">import</a> <a id="29341" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="29373" class="Keyword">open</a> <a id="29378" class="Keyword">import</a> <a id="29385" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="29438" class="Keyword">open</a> <a id="29443" class="Keyword">import</a> <a id="29450" href="order-theory.html" class="Module">order-theory</a>
<a id="29463" class="Keyword">open</a> <a id="29468" class="Keyword">import</a> <a id="29475" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="29502" class="Keyword">open</a> <a id="29507" class="Keyword">import</a> <a id="29514" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="29544" class="Keyword">open</a> <a id="29549" class="Keyword">import</a> <a id="29556" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="29589" class="Keyword">open</a> <a id="29594" class="Keyword">import</a> <a id="29601" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="29637" class="Keyword">open</a> <a id="29642" class="Keyword">import</a> <a id="29649" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="29684" class="Keyword">open</a> <a id="29689" class="Keyword">import</a> <a id="29696" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="29723" class="Keyword">open</a> <a id="29728" class="Keyword">import</a> <a id="29735" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="29765" class="Keyword">open</a> <a id="29770" class="Keyword">import</a> <a id="29777" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="29813" class="Keyword">open</a> <a id="29818" class="Keyword">import</a> <a id="29825" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="29867" class="Keyword">open</a> <a id="29872" class="Keyword">import</a> <a id="29879" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="29911" class="Keyword">open</a> <a id="29916" class="Keyword">import</a> <a id="29923" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="29954" class="Keyword">open</a> <a id="29959" class="Keyword">import</a> <a id="29966" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="29992" class="Keyword">open</a> <a id="29997" class="Keyword">import</a> <a id="30004" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30033" class="Keyword">open</a> <a id="30038" class="Keyword">import</a> <a id="30045" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30082" class="Keyword">open</a> <a id="30087" class="Keyword">import</a> <a id="30094" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="30134" class="Keyword">open</a> <a id="30139" class="Keyword">import</a> <a id="30146" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="30168" class="Keyword">open</a> <a id="30173" class="Keyword">import</a> <a id="30180" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="30215" class="Keyword">open</a> <a id="30220" class="Keyword">import</a> <a id="30227" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="30265" class="Keyword">open</a> <a id="30270" class="Keyword">import</a> <a id="30277" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="30316" class="Keyword">open</a> <a id="30321" class="Keyword">import</a> <a id="30328" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="30363" class="Keyword">open</a> <a id="30368" class="Keyword">import</a> <a id="30375" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="30410" class="Keyword">open</a> <a id="30415" class="Keyword">import</a> <a id="30422" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="30460" class="Keyword">open</a> <a id="30465" class="Keyword">import</a> <a id="30472" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="30503" class="Keyword">open</a> <a id="30508" class="Keyword">import</a> <a id="30515" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="30557" class="Keyword">open</a> <a id="30562" class="Keyword">import</a> <a id="30569" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="30614" class="Keyword">open</a> <a id="30619" class="Keyword">import</a> <a id="30626" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="30659" class="Keyword">open</a> <a id="30664" class="Keyword">import</a> <a id="30671" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="30691" class="Keyword">open</a> <a id="30696" class="Keyword">import</a> <a id="30703" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="30726" class="Keyword">open</a> <a id="30731" class="Keyword">import</a> <a id="30738" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="30761" class="Keyword">open</a> <a id="30766" class="Keyword">import</a> <a id="30773" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="30799" class="Keyword">open</a> <a id="30804" class="Keyword">import</a> <a id="30811" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="30837" class="Keyword">open</a> <a id="30842" class="Keyword">import</a> <a id="30849" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="30913" class="Keyword">open</a> <a id="30918" class="Keyword">import</a> <a id="30925" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="30943" class="Keyword">open</a> <a id="30948" class="Keyword">import</a> <a id="30955" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="30982" class="Keyword">open</a> <a id="30987" class="Keyword">import</a> <a id="30994" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31020" class="Keyword">open</a> <a id="31025" class="Keyword">import</a> <a id="31032" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31058" class="Keyword">open</a> <a id="31063" class="Keyword">import</a> <a id="31070" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31096" class="Keyword">open</a> <a id="31101" class="Keyword">import</a> <a id="31108" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="31139" class="Keyword">open</a> <a id="31144" class="Keyword">import</a> <a id="31151" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="31214" class="Keyword">open</a> <a id="31219" class="Keyword">import</a> <a id="31226" href="polytopes.html" class="Module">polytopes</a>
<a id="31236" class="Keyword">open</a> <a id="31241" class="Keyword">import</a> <a id="31248" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="31306" class="Keyword">open</a> <a id="31311" class="Keyword">import</a> <a id="31318" href="ring-theory.html" class="Module">ring-theory</a>
<a id="31330" class="Keyword">open</a> <a id="31335" class="Keyword">import</a> <a id="31342" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="31379" class="Keyword">open</a> <a id="31384" class="Keyword">import</a> <a id="31391" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="31418" class="Keyword">open</a> <a id="31423" class="Keyword">import</a> <a id="31430" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="31462" class="Keyword">open</a> <a id="31467" class="Keyword">import</a> <a id="31474" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="31520" class="Keyword">open</a> <a id="31525" class="Keyword">import</a> <a id="31532" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="31557" class="Keyword">open</a> <a id="31562" class="Keyword">import</a> <a id="31569" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="31612" class="Keyword">open</a> <a id="31617" class="Keyword">import</a> <a id="31624" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="31662" class="Keyword">open</a> <a id="31667" class="Keyword">import</a> <a id="31674" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="31705" class="Keyword">open</a> <a id="31710" class="Keyword">import</a> <a id="31717" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="31741" class="Keyword">open</a> <a id="31746" class="Keyword">import</a> <a id="31753" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="31785" class="Keyword">open</a> <a id="31790" class="Keyword">import</a> <a id="31797" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="31823" class="Keyword">open</a> <a id="31828" class="Keyword">import</a> <a id="31835" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="31864" class="Keyword">open</a> <a id="31869" class="Keyword">import</a> <a id="31876" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="31913" class="Keyword">open</a> <a id="31918" class="Keyword">import</a> <a id="31925" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="31954" class="Keyword">open</a> <a id="31959" class="Keyword">import</a> <a id="31966" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="31993" class="Keyword">open</a> <a id="31998" class="Keyword">import</a> <a id="32005" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32042" class="Keyword">open</a> <a id="32047" class="Keyword">import</a> <a id="32054" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32081" class="Keyword">open</a> <a id="32086" class="Keyword">import</a> <a id="32093" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="32126" class="Keyword">open</a> <a id="32131" class="Keyword">import</a> <a id="32138" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="32156" class="Keyword">open</a> <a id="32161" class="Keyword">import</a> <a id="32168" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="32222" class="Keyword">open</a> <a id="32227" class="Keyword">import</a> <a id="32234" href="set-theory.html" class="Module">set-theory</a>
<a id="32245" class="Keyword">open</a> <a id="32250" class="Keyword">import</a> <a id="32257" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="32280" class="Keyword">open</a> <a id="32285" class="Keyword">import</a> <a id="32292" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="32316" class="Keyword">open</a> <a id="32321" class="Keyword">import</a> <a id="32328" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="32354" class="Keyword">open</a> <a id="32359" class="Keyword">import</a> <a id="32366" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="32428" class="Keyword">open</a> <a id="32433" class="Keyword">import</a> <a id="32440" href="structured-types.html" class="Module">structured-types</a>
<a id="32457" class="Keyword">open</a> <a id="32462" class="Keyword">import</a> <a id="32469" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="32504" class="Keyword">open</a> <a id="32509" class="Keyword">import</a> <a id="32516" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="32560" class="Keyword">open</a> <a id="32565" class="Keyword">import</a> <a id="32572" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="32636" class="Keyword">open</a> <a id="32641" class="Keyword">import</a> <a id="32648" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="32687" class="Keyword">open</a> <a id="32692" class="Keyword">import</a> <a id="32699" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="32745" class="Keyword">open</a> <a id="32750" class="Keyword">import</a> <a id="32757" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="32781" class="Keyword">open</a> <a id="32786" class="Keyword">import</a> <a id="32793" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="32862" class="Keyword">open</a> <a id="32867" class="Keyword">import</a> <a id="32874" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="32919" class="Keyword">open</a> <a id="32924" class="Keyword">import</a> <a id="32931" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="32965" class="Keyword">open</a> <a id="32970" class="Keyword">import</a> <a id="32977" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33038" class="Keyword">open</a> <a id="33043" class="Keyword">import</a> <a id="33050" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33095" class="Keyword">open</a> <a id="33100" class="Keyword">import</a> <a id="33107" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="33145" class="Keyword">open</a> <a id="33150" class="Keyword">import</a> <a id="33157" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="33200" class="Keyword">open</a> <a id="33205" class="Keyword">import</a> <a id="33212" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="33248" class="Keyword">open</a> <a id="33253" class="Keyword">import</a> <a id="33260" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="33290" class="Keyword">open</a> <a id="33295" class="Keyword">import</a> <a id="33302" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="33333" class="Keyword">open</a> <a id="33338" class="Keyword">import</a> <a id="33345" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="33404" class="Keyword">open</a> <a id="33409" class="Keyword">import</a> <a id="33416" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="33467" class="Keyword">open</a> <a id="33472" class="Keyword">import</a> <a id="33479" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="33530" class="Keyword">open</a> <a id="33535" class="Keyword">import</a> <a id="33542" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="33597" class="Keyword">open</a> <a id="33602" class="Keyword">import</a> <a id="33609" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="33638" class="Keyword">open</a> <a id="33643" class="Keyword">import</a> <a id="33650" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="33678" class="Keyword">open</a> <a id="33683" class="Keyword">import</a> <a id="33690" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="33720" class="Keyword">open</a> <a id="33725" class="Keyword">import</a> <a id="33732" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="33766" class="Keyword">open</a> <a id="33771" class="Keyword">import</a> <a id="33778" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="33854" class="Keyword">open</a> <a id="33859" class="Keyword">import</a> <a id="33866" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="33892" class="Keyword">open</a> <a id="33897" class="Keyword">import</a> <a id="33904" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="33943" class="Keyword">open</a> <a id="33948" class="Keyword">import</a> <a id="33955" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="33993" class="Keyword">open</a> <a id="33998" class="Keyword">import</a> <a id="34005" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34051" class="Keyword">open</a> <a id="34056" class="Keyword">import</a> <a id="34063" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34100" class="Keyword">open</a> <a id="34105" class="Keyword">import</a> <a id="34112" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34152" class="Keyword">open</a> <a id="34157" class="Keyword">import</a> <a id="34164" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="34203" class="Keyword">open</a> <a id="34208" class="Keyword">import</a> <a id="34215" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="34248" class="Keyword">open</a> <a id="34253" class="Keyword">import</a> <a id="34260" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="34295" class="Keyword">open</a> <a id="34300" class="Keyword">import</a> <a id="34307" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="34352" class="Keyword">open</a> <a id="34357" class="Keyword">import</a> <a id="34364" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="34416" class="Keyword">open</a> <a id="34421" class="Keyword">import</a> <a id="34428" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="34481" class="Keyword">open</a> <a id="34486" class="Keyword">import</a> <a id="34493" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="34553" class="Keyword">open</a> <a id="34558" class="Keyword">import</a> <a id="34565" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="34613" class="Keyword">open</a> <a id="34618" class="Keyword">import</a> <a id="34625" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="34665" class="Keyword">open</a> <a id="34670" class="Keyword">import</a> <a id="34677" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="34724" class="Keyword">open</a> <a id="34729" class="Keyword">import</a> <a id="34736" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="34777" class="Keyword">open</a> <a id="34782" class="Keyword">import</a> <a id="34789" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="34827" class="Keyword">open</a> <a id="34832" class="Keyword">import</a> <a id="34839" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="34887" class="Keyword">open</a> <a id="34892" class="Keyword">import</a> <a id="34899" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="34936" class="Keyword">open</a> <a id="34941" class="Keyword">import</a> <a id="34948" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="34982" class="Keyword">open</a> <a id="34987" class="Keyword">import</a> <a id="34994" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35041" class="Keyword">open</a> <a id="35046" class="Keyword">import</a> <a id="35053" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35098" class="Keyword">open</a> <a id="35103" class="Keyword">import</a> <a id="35110" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35159" class="Keyword">open</a> <a id="35164" class="Keyword">import</a> <a id="35171" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="35248" class="Keyword">open</a> <a id="35253" class="Keyword">import</a> <a id="35260" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="35312" class="Keyword">open</a> <a id="35317" class="Keyword">import</a> <a id="35324" href="type-theories.html" class="Module">type-theories</a>
<a id="35338" class="Keyword">open</a> <a id="35343" class="Keyword">import</a> <a id="35350" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="35392" class="Keyword">open</a> <a id="35397" class="Keyword">import</a> <a id="35404" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="35442" class="Keyword">open</a> <a id="35447" class="Keyword">import</a> <a id="35454" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="35500" class="Keyword">open</a> <a id="35505" class="Keyword">import</a> <a id="35512" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="35559" class="Keyword">open</a> <a id="35564" class="Keyword">import</a> <a id="35571" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="35606" class="Keyword">open</a> <a id="35611" class="Keyword">import</a> <a id="35618" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="35696" class="Keyword">open</a> <a id="35701" class="Keyword">import</a> <a id="35708" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="35732" class="Keyword">open</a> <a id="35737" class="Keyword">import</a> <a id="35744" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="35797" class="Keyword">open</a> <a id="35802" class="Keyword">import</a> <a id="35809" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="35852" class="Keyword">open</a> <a id="35857" class="Keyword">import</a> <a id="35864" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="35904" class="Keyword">open</a> <a id="35909" class="Keyword">import</a> <a id="35916" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="35955" class="Keyword">open</a> <a id="35960" class="Keyword">import</a> <a id="35967" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36001" class="Keyword">open</a> <a id="36006" class="Keyword">import</a> <a id="36013" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36061" class="Keyword">open</a> <a id="36066" class="Keyword">import</a> <a id="36073" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36124" class="Keyword">open</a> <a id="36129" class="Keyword">import</a> <a id="36136" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="36183" class="Keyword">open</a> <a id="36188" class="Keyword">import</a> <a id="36195" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="36247" class="Keyword">open</a> <a id="36252" class="Keyword">import</a> <a id="36259" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="36303" class="Keyword">open</a> <a id="36308" class="Keyword">import</a> <a id="36315" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="36355" class="Keyword">open</a> <a id="36360" class="Keyword">import</a> <a id="36367" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="36410" class="Keyword">open</a> <a id="36415" class="Keyword">import</a> <a id="36422" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="36474" class="Keyword">open</a> <a id="36479" class="Keyword">import</a> <a id="36486" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="36540" class="Keyword">open</a> <a id="36545" class="Keyword">import</a> <a id="36552" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="36600" class="Keyword">open</a> <a id="36605" class="Keyword">import</a> <a id="36612" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="36651" class="Keyword">open</a> <a id="36656" class="Keyword">import</a> <a id="36663" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="36696" class="Keyword">open</a> <a id="36701" class="Keyword">import</a> <a id="36708" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="36738" class="Keyword">open</a> <a id="36743" class="Keyword">import</a> <a id="36750" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="36801" class="Keyword">open</a> <a id="36806" class="Keyword">import</a> <a id="36813" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="36854" class="Keyword">open</a> <a id="36859" class="Keyword">import</a> <a id="36866" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="36903" class="Keyword">open</a> <a id="36908" class="Keyword">import</a> <a id="36915" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="36974" class="Keyword">open</a> <a id="36979" class="Keyword">import</a> <a id="36986" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37041" class="Keyword">open</a> <a id="37046" class="Keyword">import</a> <a id="37053" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37109" class="Keyword">open</a> <a id="37114" class="Keyword">import</a> <a id="37121" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="37168" class="Keyword">open</a> <a id="37173" class="Keyword">import</a> <a id="37180" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="37223" class="Keyword">open</a> <a id="37228" class="Keyword">import</a> <a id="37235" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="37280" class="Keyword">open</a> <a id="37285" class="Keyword">import</a> <a id="37292" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="37341" class="Keyword">open</a> <a id="37346" class="Keyword">import</a> <a id="37353" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="37404" class="Keyword">open</a> <a id="37409" class="Keyword">import</a> <a id="37416" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="37460" class="Keyword">open</a> <a id="37465" class="Keyword">import</a> <a id="37472" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="37550" class="Keyword">open</a> <a id="37555" class="Keyword">import</a> <a id="37562" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="37602" class="Keyword">open</a> <a id="37607" class="Keyword">import</a> <a id="37614" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="37671" class="Keyword">open</a> <a id="37676" class="Keyword">import</a> <a id="37683" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="37718" class="Keyword">open</a> <a id="37723" class="Keyword">import</a> <a id="37730" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="37776" class="Keyword">open</a> <a id="37781" class="Keyword">import</a> <a id="37788" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="37843" class="Keyword">open</a> <a id="37848" class="Keyword">import</a> <a id="37855" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="37898" class="Keyword">open</a> <a id="37903" class="Keyword">import</a> <a id="37910" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="37955" class="Keyword">open</a> <a id="37960" class="Keyword">import</a> <a id="37967" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38026" class="Keyword">open</a> <a id="38031" class="Keyword">import</a> <a id="38038" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38075" class="Keyword">open</a> <a id="38080" class="Keyword">import</a> <a id="38087" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38129" class="Keyword">open</a> <a id="38134" class="Keyword">import</a> <a id="38141" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="38182" class="Keyword">open</a> <a id="38187" class="Keyword">import</a> <a id="38194" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="38233" class="Keyword">open</a> <a id="38238" class="Keyword">import</a> <a id="38245" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="38283" class="Keyword">open</a> <a id="38288" class="Keyword">import</a> <a id="38295" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="38347" class="Keyword">open</a> <a id="38352" class="Keyword">import</a> <a id="38359" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="38404" class="Keyword">open</a> <a id="38409" class="Keyword">import</a> <a id="38416" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="38455" class="Keyword">open</a> <a id="38460" class="Keyword">import</a> <a id="38467" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="38504" class="Keyword">open</a> <a id="38509" class="Keyword">import</a> <a id="38516" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="38565" class="Keyword">open</a> <a id="38570" class="Keyword">import</a> <a id="38577" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="38616" class="Keyword">open</a> <a id="38621" class="Keyword">import</a> <a id="38628" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="38666" class="Keyword">open</a> <a id="38671" class="Keyword">import</a> <a id="38678" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="38733" class="Keyword">open</a> <a id="38738" class="Keyword">import</a> <a id="38745" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="38784" class="Keyword">open</a> <a id="38789" class="Keyword">import</a> <a id="38796" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="38844" class="Keyword">open</a> <a id="38849" class="Keyword">import</a> <a id="38856" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="38903" class="Keyword">open</a> <a id="38908" class="Keyword">import</a> <a id="38915" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="38953" class="Keyword">open</a> <a id="38958" class="Keyword">import</a> <a id="38965" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="38995" class="Keyword">open</a> <a id="39000" class="Keyword">import</a> <a id="39007" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39064" class="Keyword">open</a> <a id="39069" class="Keyword">import</a> <a id="39076" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39130" class="Keyword">open</a> <a id="39135" class="Keyword">import</a> <a id="39142" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="39172" class="Keyword">open</a> <a id="39177" class="Keyword">import</a> <a id="39184" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="39233" class="Keyword">open</a> <a id="39238" class="Keyword">import</a> <a id="39245" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="39287" class="Keyword">open</a> <a id="39292" class="Keyword">import</a> <a id="39299" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="39333" class="Keyword">open</a> <a id="39338" class="Keyword">import</a> <a id="39345" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="39408" class="Keyword">open</a> <a id="39413" class="Keyword">import</a> <a id="39420" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="39463" class="Keyword">open</a> <a id="39468" class="Keyword">import</a> <a id="39475" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="39510" class="Keyword">open</a> <a id="39515" class="Keyword">import</a> <a id="39522" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="39557" class="Keyword">open</a> <a id="39562" class="Keyword">import</a> <a id="39569" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="39609" class="Keyword">open</a> <a id="39614" class="Keyword">import</a> <a id="39621" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="39666" class="Keyword">open</a> <a id="39671" class="Keyword">import</a> <a id="39678" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="39719" class="Keyword">open</a> <a id="39724" class="Keyword">import</a> <a id="39731" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="39785" class="Keyword">open</a> <a id="39790" class="Keyword">import</a> <a id="39797" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="39847" class="Keyword">open</a> <a id="39852" class="Keyword">import</a> <a id="39859" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="39906" class="Keyword">open</a> <a id="39911" class="Keyword">import</a> <a id="39918" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="39956" class="Keyword">open</a> <a id="39961" class="Keyword">import</a> <a id="39968" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40017" class="Keyword">open</a> <a id="40022" class="Keyword">import</a> <a id="40029" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40076" class="Keyword">open</a> <a id="40081" class="Keyword">import</a> <a id="40088" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40151" class="Keyword">open</a> <a id="40156" class="Keyword">import</a> <a id="40163" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="40195" class="Keyword">open</a> <a id="40200" class="Keyword">import</a> <a id="40207" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="40260" class="Keyword">open</a> <a id="40265" class="Keyword">import</a> <a id="40272" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="40318" class="Keyword">open</a> <a id="40323" class="Keyword">import</a> <a id="40330" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="40376" class="Keyword">open</a> <a id="40381" class="Keyword">import</a> <a id="40388" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="40428" class="Keyword">open</a> <a id="40433" class="Keyword">import</a> <a id="40440" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="40487" class="Keyword">open</a> <a id="40492" class="Keyword">import</a> <a id="40499" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="40547" class="Keyword">open</a> <a id="40552" class="Keyword">import</a> <a id="40559" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="40599" class="Keyword">open</a> <a id="40604" class="Keyword">import</a> <a id="40611" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="40656" class="Keyword">open</a> <a id="40661" class="Keyword">import</a> <a id="40668" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="40733" class="Keyword">open</a> <a id="40738" class="Keyword">import</a> <a id="40745" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="40790" class="Keyword">open</a> <a id="40795" class="Keyword">import</a> <a id="40802" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="40849" class="Keyword">open</a> <a id="40854" class="Keyword">import</a> <a id="40861" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="40914" class="Keyword">open</a> <a id="40919" class="Keyword">import</a> <a id="40926" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>