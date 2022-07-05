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
<a id="10834" class="Keyword">open</a> <a id="10839" class="Keyword">import</a> <a id="10846" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="10888" class="Keyword">open</a> <a id="10893" class="Keyword">import</a> <a id="10900" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10963" class="Keyword">open</a> <a id="10968" class="Keyword">import</a> <a id="10975" href="foundation.html" class="Module">foundation</a>
<a id="10986" class="Keyword">open</a> <a id="10991" class="Keyword">import</a> <a id="10998" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11016" class="Keyword">open</a> <a id="11021" class="Keyword">import</a> <a id="11028" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11047" class="Keyword">open</a> <a id="11052" class="Keyword">import</a> <a id="11059" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11078" class="Keyword">open</a> <a id="11083" class="Keyword">import</a> <a id="11090" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11134" class="Keyword">open</a> <a id="11139" class="Keyword">import</a> <a id="11146" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11171" class="Keyword">open</a> <a id="11176" class="Keyword">import</a> <a id="11183" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11210" class="Keyword">open</a> <a id="11215" class="Keyword">import</a> <a id="11222" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11239" class="Keyword">open</a> <a id="11244" class="Keyword">import</a> <a id="11251" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11280" class="Keyword">open</a> <a id="11285" class="Keyword">import</a> <a id="11292" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11348" class="Keyword">open</a> <a id="11353" class="Keyword">import</a> <a id="11360" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11391" class="Keyword">open</a> <a id="11396" class="Keyword">import</a> <a id="11403" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11457" class="Keyword">open</a> <a id="11462" class="Keyword">import</a> <a id="11469" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11497" class="Keyword">open</a> <a id="11502" class="Keyword">import</a> <a id="11509" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11539" class="Keyword">open</a> <a id="11544" class="Keyword">import</a> <a id="11551" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11571" class="Keyword">open</a> <a id="11576" class="Keyword">import</a> <a id="11583" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11628" class="Keyword">open</a> <a id="11633" class="Keyword">import</a> <a id="11640" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11677" class="Keyword">open</a> <a id="11682" class="Keyword">import</a> <a id="11689" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11724" class="Keyword">open</a> <a id="11729" class="Keyword">import</a> <a id="11736" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11794" class="Keyword">open</a> <a id="11799" class="Keyword">import</a> <a id="11806" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11844" class="Keyword">open</a> <a id="11849" class="Keyword">import</a> <a id="11856" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11890" class="Keyword">open</a> <a id="11895" class="Keyword">import</a> <a id="11902" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11931" class="Keyword">open</a> <a id="11936" class="Keyword">import</a> <a id="11943" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11966" class="Keyword">open</a> <a id="11971" class="Keyword">import</a> <a id="11978" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12005" class="Keyword">open</a> <a id="12010" class="Keyword">import</a> <a id="12017" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12040" class="Keyword">open</a> <a id="12045" class="Keyword">import</a> <a id="12052" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12094" class="Keyword">open</a> <a id="12099" class="Keyword">import</a> <a id="12106" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12138" class="Keyword">open</a> <a id="12143" class="Keyword">import</a> <a id="12150" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12177" class="Keyword">open</a> <a id="12182" class="Keyword">import</a> <a id="12189" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12214" class="Keyword">open</a> <a id="12219" class="Keyword">import</a> <a id="12226" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12255" class="Keyword">open</a> <a id="12260" class="Keyword">import</a> <a id="12267" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12297" class="Keyword">open</a> <a id="12302" class="Keyword">import</a> <a id="12309" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12336" class="Keyword">open</a> <a id="12341" class="Keyword">import</a> <a id="12348" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12367" class="Keyword">open</a> <a id="12372" class="Keyword">import</a> <a id="12379" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12425" class="Keyword">open</a> <a id="12430" class="Keyword">import</a> <a id="12437" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12479" class="Keyword">open</a> <a id="12484" class="Keyword">import</a> <a id="12491" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12523" class="Keyword">open</a> <a id="12528" class="Keyword">import</a> <a id="12535" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12565" class="Keyword">open</a> <a id="12570" class="Keyword">import</a> <a id="12577" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12603" class="Keyword">open</a> <a id="12608" class="Keyword">import</a> <a id="12615" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12649" class="Keyword">open</a> <a id="12654" class="Keyword">import</a> <a id="12661" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12691" class="Keyword">open</a> <a id="12696" class="Keyword">import</a> <a id="12703" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12730" class="Keyword">open</a> <a id="12735" class="Keyword">import</a> <a id="12742" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="12780" class="Keyword">open</a> <a id="12785" class="Keyword">import</a> <a id="12792" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12824" class="Keyword">open</a> <a id="12829" class="Keyword">import</a> <a id="12836" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12870" class="Keyword">open</a> <a id="12875" class="Keyword">import</a> <a id="12882" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12905" class="Keyword">open</a> <a id="12910" class="Keyword">import</a> <a id="12917" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12944" class="Keyword">open</a> <a id="12949" class="Keyword">import</a> <a id="12956" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12984" class="Keyword">open</a> <a id="12989" class="Keyword">import</a> <a id="12996" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13033" class="Keyword">open</a> <a id="13038" class="Keyword">import</a> <a id="13045" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13093" class="Keyword">open</a> <a id="13098" class="Keyword">import</a> <a id="13105" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13145" class="Keyword">open</a> <a id="13150" class="Keyword">import</a> <a id="13157" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13179" class="Keyword">open</a> <a id="13184" class="Keyword">import</a> <a id="13191" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13214" class="Keyword">open</a> <a id="13219" class="Keyword">import</a> <a id="13226" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13251" class="Keyword">open</a> <a id="13256" class="Keyword">import</a> <a id="13263" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13308" class="Keyword">open</a> <a id="13313" class="Keyword">import</a> <a id="13320" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13364" class="Keyword">open</a> <a id="13369" class="Keyword">import</a> <a id="13376" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13412" class="Keyword">open</a> <a id="13417" class="Keyword">import</a> <a id="13424" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13469" class="Keyword">open</a> <a id="13474" class="Keyword">import</a> <a id="13481" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13522" class="Keyword">open</a> <a id="13527" class="Keyword">import</a> <a id="13534" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13569" class="Keyword">open</a> <a id="13574" class="Keyword">import</a> <a id="13581" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13613" class="Keyword">open</a> <a id="13618" class="Keyword">import</a> <a id="13625" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13656" class="Keyword">open</a> <a id="13661" class="Keyword">import</a> <a id="13668" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13701" class="Keyword">open</a> <a id="13706" class="Keyword">import</a> <a id="13713" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13746" class="Keyword">open</a> <a id="13751" class="Keyword">import</a> <a id="13758" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13788" class="Keyword">open</a> <a id="13793" class="Keyword">import</a> <a id="13800" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13824" class="Keyword">open</a> <a id="13829" class="Keyword">import</a> <a id="13836" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13874" class="Keyword">open</a> <a id="13879" class="Keyword">import</a> <a id="13886" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13917" class="Keyword">open</a> <a id="13922" class="Keyword">import</a> <a id="13929" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13954" class="Keyword">open</a> <a id="13959" class="Keyword">import</a> <a id="13966" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13994" class="Keyword">open</a> <a id="13999" class="Keyword">import</a> <a id="14006" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14030" class="Keyword">open</a> <a id="14035" class="Keyword">import</a> <a id="14042" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14068" class="Keyword">open</a> <a id="14073" class="Keyword">import</a> <a id="14080" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14115" class="Keyword">open</a> <a id="14120" class="Keyword">import</a> <a id="14127" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14148" class="Keyword">open</a> <a id="14153" class="Keyword">import</a> <a id="14160" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14209" class="Keyword">open</a> <a id="14214" class="Keyword">import</a> <a id="14221" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14262" class="Keyword">open</a> <a id="14267" class="Keyword">import</a> <a id="14274" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14324" class="Keyword">open</a> <a id="14329" class="Keyword">import</a> <a id="14336" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14382" class="Keyword">open</a> <a id="14387" class="Keyword">import</a> <a id="14394" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14434" class="Keyword">open</a> <a id="14439" class="Keyword">import</a> <a id="14446" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14496" class="Keyword">open</a> <a id="14501" class="Keyword">import</a> <a id="14508" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14547" class="Keyword">open</a> <a id="14552" class="Keyword">import</a> <a id="14559" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14599" class="Keyword">open</a> <a id="14604" class="Keyword">import</a> <a id="14611" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14644" class="Keyword">open</a> <a id="14649" class="Keyword">import</a> <a id="14656" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14705" class="Keyword">open</a> <a id="14710" class="Keyword">import</a> <a id="14717" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14742" class="Keyword">open</a> <a id="14747" class="Keyword">import</a> <a id="14754" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14792" class="Keyword">open</a> <a id="14797" class="Keyword">import</a> <a id="14804" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14826" class="Keyword">open</a> <a id="14831" class="Keyword">import</a> <a id="14838" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14866" class="Keyword">open</a> <a id="14871" class="Keyword">import</a> <a id="14878" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="14914" class="Keyword">open</a> <a id="14919" class="Keyword">import</a> <a id="14926" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14952" class="Keyword">open</a> <a id="14957" class="Keyword">import</a> <a id="14964" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14982" class="Keyword">open</a> <a id="14987" class="Keyword">import</a> <a id="14994" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15029" class="Keyword">open</a> <a id="15034" class="Keyword">import</a> <a id="15041" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15076" class="Keyword">open</a> <a id="15081" class="Keyword">import</a> <a id="15088" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15115" class="Keyword">open</a> <a id="15120" class="Keyword">import</a> <a id="15127" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15183" class="Keyword">open</a> <a id="15188" class="Keyword">import</a> <a id="15195" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15224" class="Keyword">open</a> <a id="15229" class="Keyword">import</a> <a id="15236" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15266" class="Keyword">open</a> <a id="15271" class="Keyword">import</a> <a id="15278" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15305" class="Keyword">open</a> <a id="15310" class="Keyword">import</a> <a id="15317" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15343" class="Keyword">open</a> <a id="15348" class="Keyword">import</a> <a id="15355" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15382" class="Keyword">open</a> <a id="15387" class="Keyword">import</a> <a id="15394" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15418" class="Keyword">open</a> <a id="15423" class="Keyword">import</a> <a id="15430" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15453" class="Keyword">open</a> <a id="15458" class="Keyword">import</a> <a id="15465" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15492" class="Keyword">open</a> <a id="15497" class="Keyword">import</a> <a id="15504" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15536" class="Keyword">open</a> <a id="15541" class="Keyword">import</a> <a id="15548" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15583" class="Keyword">open</a> <a id="15588" class="Keyword">import</a> <a id="15595" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15626" class="Keyword">open</a> <a id="15631" class="Keyword">import</a> <a id="15638" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15671" class="Keyword">open</a> <a id="15676" class="Keyword">import</a> <a id="15683" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15717" class="Keyword">open</a> <a id="15722" class="Keyword">import</a> <a id="15729" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15769" class="Keyword">open</a> <a id="15774" class="Keyword">import</a> <a id="15781" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15812" class="Keyword">open</a> <a id="15817" class="Keyword">import</a> <a id="15824" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15856" class="Keyword">open</a> <a id="15861" class="Keyword">import</a> <a id="15868" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15899" class="Keyword">open</a> <a id="15904" class="Keyword">import</a> <a id="15911" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15928" class="Keyword">open</a> <a id="15933" class="Keyword">import</a> <a id="15940" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15965" class="Keyword">open</a> <a id="15970" class="Keyword">import</a> <a id="15977" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16006" class="Keyword">open</a> <a id="16011" class="Keyword">import</a> <a id="16018" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16043" class="Keyword">open</a> <a id="16048" class="Keyword">import</a> <a id="16055" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16076" class="Keyword">open</a> <a id="16081" class="Keyword">import</a> <a id="16088" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16112" class="Keyword">open</a> <a id="16117" class="Keyword">import</a> <a id="16124" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16144" class="Keyword">open</a> <a id="16149" class="Keyword">import</a> <a id="16156" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16190" class="Keyword">open</a> <a id="16195" class="Keyword">import</a> <a id="16202" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16240" class="Keyword">open</a> <a id="16245" class="Keyword">import</a> <a id="16252" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16280" class="Keyword">open</a> <a id="16285" class="Keyword">import</a> <a id="16292" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16316" class="Keyword">open</a> <a id="16321" class="Keyword">import</a> <a id="16328" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16355" class="Keyword">open</a> <a id="16360" class="Keyword">import</a> <a id="16367" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16402" class="Keyword">open</a> <a id="16407" class="Keyword">import</a> <a id="16414" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16435" class="Keyword">open</a> <a id="16440" class="Keyword">import</a> <a id="16447" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16483" class="Keyword">open</a> <a id="16488" class="Keyword">import</a> <a id="16495" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16540" class="Keyword">open</a> <a id="16545" class="Keyword">import</a> <a id="16552" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16598" class="Keyword">open</a> <a id="16603" class="Keyword">import</a> <a id="16610" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16650" class="Keyword">open</a> <a id="16655" class="Keyword">import</a> <a id="16662" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16692" class="Keyword">open</a> <a id="16697" class="Keyword">import</a> <a id="16704" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="16738" class="Keyword">open</a> <a id="16743" class="Keyword">import</a> <a id="16750" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16787" class="Keyword">open</a> <a id="16792" class="Keyword">import</a> <a id="16799" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16823" class="Keyword">open</a> <a id="16828" class="Keyword">import</a> <a id="16835" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16856" class="Keyword">open</a> <a id="16861" class="Keyword">import</a> <a id="16868" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16903" class="Keyword">open</a> <a id="16908" class="Keyword">import</a> <a id="16915" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16952" class="Keyword">open</a> <a id="16957" class="Keyword">import</a> <a id="16964" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17013" class="Keyword">open</a> <a id="17018" class="Keyword">import</a> <a id="17025" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17058" class="Keyword">open</a> <a id="17063" class="Keyword">import</a> <a id="17070" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17093" class="Keyword">open</a> <a id="17098" class="Keyword">import</a> <a id="17105" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17128" class="Keyword">open</a> <a id="17133" class="Keyword">import</a> <a id="17140" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17163" class="Keyword">open</a> <a id="17168" class="Keyword">import</a> <a id="17175" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17203" class="Keyword">open</a> <a id="17208" class="Keyword">import</a> <a id="17215" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17235" class="Keyword">open</a> <a id="17240" class="Keyword">import</a> <a id="17247" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17268" class="Keyword">open</a> <a id="17273" class="Keyword">import</a> <a id="17280" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17311" class="Keyword">open</a> <a id="17316" class="Keyword">import</a> <a id="17323" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17350" class="Keyword">open</a> <a id="17355" class="Keyword">import</a> <a id="17362" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17378" class="Keyword">open</a> <a id="17383" class="Keyword">import</a> <a id="17390" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17421" class="Keyword">open</a> <a id="17426" class="Keyword">import</a> <a id="17433" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17450" class="Keyword">open</a> <a id="17455" class="Keyword">import</a> <a id="17462" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17484" class="Keyword">open</a> <a id="17489" class="Keyword">import</a> <a id="17496" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17523" class="Keyword">open</a> <a id="17528" class="Keyword">import</a> <a id="17535" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17558" class="Keyword">open</a> <a id="17563" class="Keyword">import</a> <a id="17570" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17597" class="Keyword">open</a> <a id="17602" class="Keyword">import</a> <a id="17609" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17642" class="Keyword">open</a> <a id="17647" class="Keyword">import</a> <a id="17654" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17694" class="Keyword">open</a> <a id="17699" class="Keyword">import</a> <a id="17706" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17727" class="Keyword">open</a> <a id="17732" class="Keyword">import</a> <a id="17739" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17768" class="Keyword">open</a> <a id="17773" class="Keyword">import</a> <a id="17780" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17818" class="Keyword">open</a> <a id="17823" class="Keyword">import</a> <a id="17830" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17850" class="Keyword">open</a> <a id="17855" class="Keyword">import</a> <a id="17862" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17886" class="Keyword">open</a> <a id="17891" class="Keyword">import</a> <a id="17898" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17925" class="Keyword">open</a> <a id="17930" class="Keyword">import</a> <a id="17937" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17969" class="Keyword">open</a> <a id="17974" class="Keyword">import</a> <a id="17981" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18011" class="Keyword">open</a> <a id="18016" class="Keyword">import</a> <a id="18023" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18049" class="Keyword">open</a> <a id="18054" class="Keyword">import</a> <a id="18061" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18088" class="Keyword">open</a> <a id="18093" class="Keyword">import</a> <a id="18100" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18129" class="Keyword">open</a> <a id="18134" class="Keyword">import</a> <a id="18141" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18164" class="Keyword">open</a> <a id="18169" class="Keyword">import</a> <a id="18176" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18227" class="Keyword">open</a> <a id="18232" class="Keyword">import</a> <a id="18239" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18282" class="Keyword">open</a> <a id="18287" class="Keyword">import</a> <a id="18294" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18342" class="Keyword">open</a> <a id="18347" class="Keyword">import</a> <a id="18354" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18392" class="Keyword">open</a> <a id="18397" class="Keyword">import</a> <a id="18404" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18441" class="Keyword">open</a> <a id="18446" class="Keyword">import</a> <a id="18453" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18499" class="Keyword">open</a> <a id="18504" class="Keyword">import</a> <a id="18511" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18528" class="Keyword">open</a> <a id="18533" class="Keyword">import</a> <a id="18540" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18568" class="Keyword">open</a> <a id="18573" class="Keyword">import</a> <a id="18580" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18608" class="Keyword">open</a> <a id="18613" class="Keyword">import</a> <a id="18620" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18656" class="Keyword">open</a> <a id="18661" class="Keyword">import</a> <a id="18668" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18706" class="Keyword">open</a> <a id="18711" class="Keyword">import</a> <a id="18718" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18751" class="Keyword">open</a> <a id="18756" class="Keyword">import</a> <a id="18763" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18784" class="Keyword">open</a> <a id="18789" class="Keyword">import</a> <a id="18796" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="18832" class="Keyword">open</a> <a id="18837" class="Keyword">import</a> <a id="18844" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18898" class="Keyword">open</a> <a id="18903" class="Keyword">import</a> <a id="18910" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18932" class="Keyword">open</a> <a id="18937" class="Keyword">import</a> <a id="18944" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18979" class="Keyword">open</a> <a id="18984" class="Keyword">import</a> <a id="18991" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19021" class="Keyword">open</a> <a id="19026" class="Keyword">import</a> <a id="19033" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19072" class="Keyword">open</a> <a id="19077" class="Keyword">import</a> <a id="19084" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19138" class="Keyword">open</a> <a id="19143" class="Keyword">import</a> <a id="19150" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19196" class="Keyword">open</a> <a id="19201" class="Keyword">import</a> <a id="19208" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19259" class="Keyword">open</a> <a id="19264" class="Keyword">import</a> <a id="19271" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19312" class="Keyword">open</a> <a id="19317" class="Keyword">import</a> <a id="19324" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19369" class="Keyword">open</a> <a id="19374" class="Keyword">import</a> <a id="19381" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19426" class="Keyword">open</a> <a id="19431" class="Keyword">import</a> <a id="19438" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19474" class="Keyword">open</a> <a id="19479" class="Keyword">import</a> <a id="19486" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19522" class="Keyword">open</a> <a id="19527" class="Keyword">import</a> <a id="19534" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19599" class="Keyword">open</a> <a id="19604" class="Keyword">import</a> <a id="19611" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19666" class="Keyword">open</a> <a id="19671" class="Keyword">import</a> <a id="19678" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19718" class="Keyword">open</a> <a id="19723" class="Keyword">import</a> <a id="19730" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19774" class="Keyword">open</a> <a id="19779" class="Keyword">import</a> <a id="19786" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19831" class="Keyword">open</a> <a id="19836" class="Keyword">import</a> <a id="19843" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19884" class="Keyword">open</a> <a id="19889" class="Keyword">import</a> <a id="19896" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19936" class="Keyword">open</a> <a id="19941" class="Keyword">import</a> <a id="19948" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19975" class="Keyword">open</a> <a id="19980" class="Keyword">import</a> <a id="19987" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20023" class="Keyword">open</a> <a id="20028" class="Keyword">import</a> <a id="20035" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20062" class="Keyword">open</a> <a id="20067" class="Keyword">import</a> <a id="20074" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20111" class="Keyword">open</a> <a id="20116" class="Keyword">import</a> <a id="20123" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20151" class="Keyword">open</a> <a id="20156" class="Keyword">import</a> <a id="20163" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20182" class="Keyword">open</a> <a id="20187" class="Keyword">import</a> <a id="20194" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20234" class="Keyword">open</a> <a id="20239" class="Keyword">import</a> <a id="20246" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20278" class="Keyword">open</a> <a id="20283" class="Keyword">import</a> <a id="20290" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20338" class="Keyword">open</a> <a id="20343" class="Keyword">import</a> <a id="20350" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20373" class="Keyword">open</a> <a id="20378" class="Keyword">import</a> <a id="20385" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20409" class="Keyword">open</a> <a id="20414" class="Keyword">import</a> <a id="20421" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20461" class="Keyword">open</a> <a id="20466" class="Keyword">import</a> <a id="20473" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20516" class="Keyword">open</a> <a id="20521" class="Keyword">import</a> <a id="20528" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20562" class="Keyword">open</a> <a id="20567" class="Keyword">import</a> <a id="20574" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20606" class="Keyword">open</a> <a id="20611" class="Keyword">import</a> <a id="20618" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20648" class="Keyword">open</a> <a id="20653" class="Keyword">import</a> <a id="20660" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20694" class="Keyword">open</a> <a id="20699" class="Keyword">import</a> <a id="20706" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20741" class="Keyword">open</a> <a id="20746" class="Keyword">import</a> <a id="20753" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20790" class="Keyword">open</a> <a id="20795" class="Keyword">import</a> <a id="20802" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20829" class="Keyword">open</a> <a id="20834" class="Keyword">import</a> <a id="20841" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20869" class="Keyword">open</a> <a id="20874" class="Keyword">import</a> <a id="20881" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20930" class="Keyword">open</a> <a id="20935" class="Keyword">import</a> <a id="20942" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20988" class="Keyword">open</a> <a id="20993" class="Keyword">import</a> <a id="21000" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21040" class="Keyword">open</a> <a id="21045" class="Keyword">import</a> <a id="21052" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21090" class="Keyword">open</a> <a id="21095" class="Keyword">import</a> <a id="21102" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21131" class="Keyword">open</a> <a id="21136" class="Keyword">import</a> <a id="21143" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21173" class="Keyword">open</a> <a id="21178" class="Keyword">import</a> <a id="21185" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21216" class="Keyword">open</a> <a id="21221" class="Keyword">import</a> <a id="21228" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21268" class="Keyword">open</a> <a id="21273" class="Keyword">import</a> <a id="21280" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21306" class="Keyword">open</a> <a id="21311" class="Keyword">import</a> <a id="21318" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21373" class="Keyword">open</a> <a id="21378" class="Keyword">import</a> <a id="21385" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21436" class="Keyword">open</a> <a id="21441" class="Keyword">import</a> <a id="21448" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21493" class="Keyword">open</a> <a id="21498" class="Keyword">import</a> <a id="21505" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21559" class="Keyword">open</a> <a id="21564" class="Keyword">import</a> <a id="21571" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21598" class="Keyword">open</a> <a id="21603" class="Keyword">import</a> <a id="21610" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21643" class="Keyword">open</a> <a id="21648" class="Keyword">import</a> <a id="21655" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21686" class="Keyword">open</a> <a id="21691" class="Keyword">import</a> <a id="21698" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21735" class="Keyword">open</a> <a id="21740" class="Keyword">import</a> <a id="21747" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21772" class="Keyword">open</a> <a id="21777" class="Keyword">import</a> <a id="21784" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21816" class="Keyword">open</a> <a id="21821" class="Keyword">import</a> <a id="21828" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21863" class="Keyword">open</a> <a id="21868" class="Keyword">import</a> <a id="21875" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21904" class="Keyword">open</a> <a id="21909" class="Keyword">import</a> <a id="21916" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21942" class="Keyword">open</a> <a id="21947" class="Keyword">import</a> <a id="21954" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21982" class="Keyword">open</a> <a id="21987" class="Keyword">import</a> <a id="21994" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22019" class="Keyword">open</a> <a id="22024" class="Keyword">import</a> <a id="22031" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22052" class="Keyword">open</a> <a id="22057" class="Keyword">import</a> <a id="22064" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22100" class="Keyword">open</a> <a id="22105" class="Keyword">import</a> <a id="22112" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22155" class="Keyword">open</a> <a id="22160" class="Keyword">import</a> <a id="22167" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22192" class="Keyword">open</a> <a id="22197" class="Keyword">import</a> <a id="22204" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22235" class="Keyword">open</a> <a id="22240" class="Keyword">import</a> <a id="22247" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22279" class="Keyword">open</a> <a id="22284" class="Keyword">import</a> <a id="22291" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22325" class="Keyword">open</a> <a id="22330" class="Keyword">import</a> <a id="22337" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22393" class="Keyword">open</a> <a id="22398" class="Keyword">import</a> <a id="22405" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22458" class="Keyword">open</a> <a id="22463" class="Keyword">import</a> <a id="22470" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22497" class="Keyword">open</a> <a id="22502" class="Keyword">import</a> <a id="22509" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22554" class="Keyword">open</a> <a id="22559" class="Keyword">import</a> <a id="22566" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22628" class="Keyword">open</a> <a id="22633" class="Keyword">import</a> <a id="22640" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22653" class="Keyword">open</a> <a id="22658" class="Keyword">import</a> <a id="22665" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="22705" class="Keyword">open</a> <a id="22710" class="Keyword">import</a> <a id="22717" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="22761" class="Keyword">open</a> <a id="22766" class="Keyword">import</a> <a id="22773" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="22812" class="Keyword">open</a> <a id="22817" class="Keyword">import</a> <a id="22824" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="22866" class="Keyword">open</a> <a id="22871" class="Keyword">import</a> <a id="22878" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="22918" class="Keyword">open</a> <a id="22923" class="Keyword">import</a> <a id="22930" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22971" class="Keyword">open</a> <a id="22976" class="Keyword">import</a> <a id="22983" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23021" class="Keyword">open</a> <a id="23026" class="Keyword">import</a> <a id="23033" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23096" class="Keyword">open</a> <a id="23101" class="Keyword">import</a> <a id="23108" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23137" class="Keyword">open</a> <a id="23142" class="Keyword">import</a> <a id="23149" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23194" class="Keyword">open</a> <a id="23199" class="Keyword">import</a> <a id="23206" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23248" class="Keyword">open</a> <a id="23253" class="Keyword">import</a> <a id="23260" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23304" class="Keyword">open</a> <a id="23309" class="Keyword">import</a> <a id="23316" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23365" class="Keyword">open</a> <a id="23370" class="Keyword">import</a> <a id="23377" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23427" class="Keyword">open</a> <a id="23432" class="Keyword">import</a> <a id="23439" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23466" class="Keyword">open</a> <a id="23471" class="Keyword">import</a> <a id="23478" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23519" class="Keyword">open</a> <a id="23524" class="Keyword">import</a> <a id="23531" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23554" class="Keyword">open</a> <a id="23559" class="Keyword">import</a> <a id="23566" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23615" class="Keyword">open</a> <a id="23620" class="Keyword">import</a> <a id="23627" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23666" class="Keyword">open</a> <a id="23671" class="Keyword">import</a> <a id="23678" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="23719" class="Keyword">open</a> <a id="23724" class="Keyword">import</a> <a id="23731" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="23775" class="Keyword">open</a> <a id="23780" class="Keyword">import</a> <a id="23787" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="23824" class="Keyword">open</a> <a id="23829" class="Keyword">import</a> <a id="23836" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="23858" class="Keyword">open</a> <a id="23863" class="Keyword">import</a> <a id="23870" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23900" class="Keyword">open</a> <a id="23905" class="Keyword">import</a> <a id="23912" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="23951" class="Keyword">open</a> <a id="23956" class="Keyword">import</a> <a id="23963" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24001" class="Keyword">open</a> <a id="24006" class="Keyword">import</a> <a id="24013" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24071" class="Keyword">open</a> <a id="24076" class="Keyword">import</a> <a id="24083" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24148" class="Keyword">open</a> <a id="24153" class="Keyword">import</a> <a id="24160" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24191" class="Keyword">open</a> <a id="24196" class="Keyword">import</a> <a id="24203" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24230" class="Keyword">open</a> <a id="24235" class="Keyword">import</a> <a id="24242" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24300" class="Keyword">open</a> <a id="24305" class="Keyword">import</a> <a id="24312" href="group-theory.html" class="Module">group-theory</a>
<a id="24325" class="Keyword">open</a> <a id="24330" class="Keyword">import</a> <a id="24337" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24365" class="Keyword">open</a> <a id="24370" class="Keyword">import</a> <a id="24377" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="24408" class="Keyword">open</a> <a id="24413" class="Keyword">import</a> <a id="24420" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="24456" class="Keyword">open</a> <a id="24461" class="Keyword">import</a> <a id="24468" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24519" class="Keyword">open</a> <a id="24524" class="Keyword">import</a> <a id="24531" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24564" class="Keyword">open</a> <a id="24569" class="Keyword">import</a> <a id="24576" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24623" class="Keyword">open</a> <a id="24628" class="Keyword">import</a> <a id="24635" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24674" class="Keyword">open</a> <a id="24679" class="Keyword">import</a> <a id="24686" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24726" class="Keyword">open</a> <a id="24731" class="Keyword">import</a> <a id="24738" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="24781" class="Keyword">open</a> <a id="24786" class="Keyword">import</a> <a id="24793" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="24825" class="Keyword">open</a> <a id="24830" class="Keyword">import</a> <a id="24837" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="24873" class="Keyword">open</a> <a id="24878" class="Keyword">import</a> <a id="24885" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="24914" class="Keyword">open</a> <a id="24919" class="Keyword">import</a> <a id="24926" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="24959" class="Keyword">open</a> <a id="24964" class="Keyword">import</a> <a id="24971" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25007" class="Keyword">open</a> <a id="25012" class="Keyword">import</a> <a id="25019" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25048" class="Keyword">open</a> <a id="25053" class="Keyword">import</a> <a id="25060" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="25092" class="Keyword">open</a> <a id="25097" class="Keyword">import</a> <a id="25104" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25129" class="Keyword">open</a> <a id="25134" class="Keyword">import</a> <a id="25141" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25172" class="Keyword">open</a> <a id="25177" class="Keyword">import</a> <a id="25184" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25231" class="Keyword">open</a> <a id="25236" class="Keyword">import</a> <a id="25243" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25276" class="Keyword">open</a> <a id="25281" class="Keyword">import</a> <a id="25288" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25328" class="Keyword">open</a> <a id="25333" class="Keyword">import</a> <a id="25340" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25377" class="Keyword">open</a> <a id="25382" class="Keyword">import</a> <a id="25389" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="25425" class="Keyword">open</a> <a id="25430" class="Keyword">import</a> <a id="25437" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25469" class="Keyword">open</a> <a id="25474" class="Keyword">import</a> <a id="25481" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25508" class="Keyword">open</a> <a id="25513" class="Keyword">import</a> <a id="25520" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="25540" class="Keyword">open</a> <a id="25545" class="Keyword">import</a> <a id="25552" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="25579" class="Keyword">open</a> <a id="25584" class="Keyword">import</a> <a id="25591" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="25633" class="Keyword">open</a> <a id="25638" class="Keyword">import</a> <a id="25645" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="25692" class="Keyword">open</a> <a id="25697" class="Keyword">import</a> <a id="25704" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="25745" class="Keyword">open</a> <a id="25750" class="Keyword">import</a> <a id="25757" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="25791" class="Keyword">open</a> <a id="25796" class="Keyword">import</a> <a id="25803" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="25838" class="Keyword">open</a> <a id="25843" class="Keyword">import</a> <a id="25850" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="25888" class="Keyword">open</a> <a id="25893" class="Keyword">import</a> <a id="25900" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="25932" class="Keyword">open</a> <a id="25937" class="Keyword">import</a> <a id="25944" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="25985" class="Keyword">open</a> <a id="25990" class="Keyword">import</a> <a id="25997" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="26038" class="Keyword">open</a> <a id="26043" class="Keyword">import</a> <a id="26050" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26090" class="Keyword">open</a> <a id="26095" class="Keyword">import</a> <a id="26102" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26135" class="Keyword">open</a> <a id="26140" class="Keyword">import</a> <a id="26147" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="26184" class="Keyword">open</a> <a id="26189" class="Keyword">import</a> <a id="26196" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="26226" class="Keyword">open</a> <a id="26231" class="Keyword">import</a> <a id="26238" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="26283" class="Keyword">open</a> <a id="26288" class="Keyword">import</a> <a id="26295" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="26323" class="Keyword">open</a> <a id="26328" class="Keyword">import</a> <a id="26335" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="26356" class="Keyword">open</a> <a id="26361" class="Keyword">import</a> <a id="26368" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="26402" class="Keyword">open</a> <a id="26407" class="Keyword">import</a> <a id="26414" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="26448" class="Keyword">open</a> <a id="26453" class="Keyword">import</a> <a id="26460" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="26495" class="Keyword">open</a> <a id="26500" class="Keyword">import</a> <a id="26507" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="26549" class="Keyword">open</a> <a id="26554" class="Keyword">import</a> <a id="26561" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="26596" class="Keyword">open</a> <a id="26601" class="Keyword">import</a> <a id="26608" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="26647" class="Keyword">open</a> <a id="26652" class="Keyword">import</a> <a id="26659" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="26696" class="Keyword">open</a> <a id="26701" class="Keyword">import</a> <a id="26708" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="26732" class="Keyword">open</a> <a id="26737" class="Keyword">import</a> <a id="26744" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="26769" class="Keyword">open</a> <a id="26774" class="Keyword">import</a> <a id="26781" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="26812" class="Keyword">open</a> <a id="26817" class="Keyword">import</a> <a id="26824" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="26875" class="Keyword">open</a> <a id="26880" class="Keyword">import</a> <a id="26887" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="26910" class="Keyword">open</a> <a id="26915" class="Keyword">import</a> <a id="26922" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="26970" class="Keyword">open</a> <a id="26975" class="Keyword">import</a> <a id="26982" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="27012" class="Keyword">open</a> <a id="27017" class="Keyword">import</a> <a id="27024" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="27094" class="Keyword">open</a> <a id="27099" class="Keyword">import</a> <a id="27106" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="27121" class="Keyword">open</a> <a id="27126" class="Keyword">import</a> <a id="27133" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="27166" class="Keyword">open</a> <a id="27171" class="Keyword">import</a> <a id="27178" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="27210" class="Keyword">open</a> <a id="27215" class="Keyword">import</a> <a id="27222" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="27264" class="Keyword">open</a> <a id="27269" class="Keyword">import</a> <a id="27276" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="27314" class="Keyword">open</a> <a id="27319" class="Keyword">import</a> <a id="27326" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="27363" class="Keyword">open</a> <a id="27368" class="Keyword">import</a> <a id="27375" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="27408" class="Keyword">open</a> <a id="27413" class="Keyword">import</a> <a id="27420" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="27444" class="Keyword">open</a> <a id="27449" class="Keyword">import</a> <a id="27456" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="27495" class="Keyword">open</a> <a id="27500" class="Keyword">import</a> <a id="27507" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="27553" class="Keyword">open</a> <a id="27558" class="Keyword">import</a> <a id="27565" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="27610" class="Keyword">open</a> <a id="27615" class="Keyword">import</a> <a id="27622" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="27660" class="Keyword">open</a> <a id="27665" class="Keyword">import</a> <a id="27672" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="27704" class="Keyword">open</a> <a id="27709" class="Keyword">import</a> <a id="27716" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="27769" class="Keyword">open</a> <a id="27774" class="Keyword">import</a> <a id="27781" href="order-theory.html" class="Module">order-theory</a>
<a id="27794" class="Keyword">open</a> <a id="27799" class="Keyword">import</a> <a id="27806" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="27833" class="Keyword">open</a> <a id="27838" class="Keyword">import</a> <a id="27845" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="27875" class="Keyword">open</a> <a id="27880" class="Keyword">import</a> <a id="27887" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="27920" class="Keyword">open</a> <a id="27925" class="Keyword">import</a> <a id="27932" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="27968" class="Keyword">open</a> <a id="27973" class="Keyword">import</a> <a id="27980" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="28015" class="Keyword">open</a> <a id="28020" class="Keyword">import</a> <a id="28027" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="28054" class="Keyword">open</a> <a id="28059" class="Keyword">import</a> <a id="28066" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="28096" class="Keyword">open</a> <a id="28101" class="Keyword">import</a> <a id="28108" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="28144" class="Keyword">open</a> <a id="28149" class="Keyword">import</a> <a id="28156" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="28198" class="Keyword">open</a> <a id="28203" class="Keyword">import</a> <a id="28210" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="28242" class="Keyword">open</a> <a id="28247" class="Keyword">import</a> <a id="28254" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="28285" class="Keyword">open</a> <a id="28290" class="Keyword">import</a> <a id="28297" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="28323" class="Keyword">open</a> <a id="28328" class="Keyword">import</a> <a id="28335" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="28364" class="Keyword">open</a> <a id="28369" class="Keyword">import</a> <a id="28376" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="28413" class="Keyword">open</a> <a id="28418" class="Keyword">import</a> <a id="28425" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="28465" class="Keyword">open</a> <a id="28470" class="Keyword">import</a> <a id="28477" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="28499" class="Keyword">open</a> <a id="28504" class="Keyword">import</a> <a id="28511" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="28546" class="Keyword">open</a> <a id="28551" class="Keyword">import</a> <a id="28558" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="28596" class="Keyword">open</a> <a id="28601" class="Keyword">import</a> <a id="28608" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="28647" class="Keyword">open</a> <a id="28652" class="Keyword">import</a> <a id="28659" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="28694" class="Keyword">open</a> <a id="28699" class="Keyword">import</a> <a id="28706" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="28741" class="Keyword">open</a> <a id="28746" class="Keyword">import</a> <a id="28753" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="28791" class="Keyword">open</a> <a id="28796" class="Keyword">import</a> <a id="28803" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="28834" class="Keyword">open</a> <a id="28839" class="Keyword">import</a> <a id="28846" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="28888" class="Keyword">open</a> <a id="28893" class="Keyword">import</a> <a id="28900" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="28945" class="Keyword">open</a> <a id="28950" class="Keyword">import</a> <a id="28957" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="28990" class="Keyword">open</a> <a id="28995" class="Keyword">import</a> <a id="29002" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="29022" class="Keyword">open</a> <a id="29027" class="Keyword">import</a> <a id="29034" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="29057" class="Keyword">open</a> <a id="29062" class="Keyword">import</a> <a id="29069" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="29092" class="Keyword">open</a> <a id="29097" class="Keyword">import</a> <a id="29104" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="29130" class="Keyword">open</a> <a id="29135" class="Keyword">import</a> <a id="29142" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="29168" class="Keyword">open</a> <a id="29173" class="Keyword">import</a> <a id="29180" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="29244" class="Keyword">open</a> <a id="29249" class="Keyword">import</a> <a id="29256" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="29274" class="Keyword">open</a> <a id="29279" class="Keyword">import</a> <a id="29286" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="29313" class="Keyword">open</a> <a id="29318" class="Keyword">import</a> <a id="29325" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="29383" class="Keyword">open</a> <a id="29388" class="Keyword">import</a> <a id="29395" href="polytopes.html" class="Module">polytopes</a>
<a id="29405" class="Keyword">open</a> <a id="29410" class="Keyword">import</a> <a id="29417" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="29475" class="Keyword">open</a> <a id="29480" class="Keyword">import</a> <a id="29487" href="ring-theory.html" class="Module">ring-theory</a>
<a id="29499" class="Keyword">open</a> <a id="29504" class="Keyword">import</a> <a id="29511" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="29548" class="Keyword">open</a> <a id="29553" class="Keyword">import</a> <a id="29560" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="29587" class="Keyword">open</a> <a id="29592" class="Keyword">import</a> <a id="29599" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="29631" class="Keyword">open</a> <a id="29636" class="Keyword">import</a> <a id="29643" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="29689" class="Keyword">open</a> <a id="29694" class="Keyword">import</a> <a id="29701" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="29726" class="Keyword">open</a> <a id="29731" class="Keyword">import</a> <a id="29738" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="29781" class="Keyword">open</a> <a id="29786" class="Keyword">import</a> <a id="29793" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="29831" class="Keyword">open</a> <a id="29836" class="Keyword">import</a> <a id="29843" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="29874" class="Keyword">open</a> <a id="29879" class="Keyword">import</a> <a id="29886" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="29910" class="Keyword">open</a> <a id="29915" class="Keyword">import</a> <a id="29922" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="29954" class="Keyword">open</a> <a id="29959" class="Keyword">import</a> <a id="29966" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="29992" class="Keyword">open</a> <a id="29997" class="Keyword">import</a> <a id="30004" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="30033" class="Keyword">open</a> <a id="30038" class="Keyword">import</a> <a id="30045" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="30082" class="Keyword">open</a> <a id="30087" class="Keyword">import</a> <a id="30094" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="30123" class="Keyword">open</a> <a id="30128" class="Keyword">import</a> <a id="30135" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="30162" class="Keyword">open</a> <a id="30167" class="Keyword">import</a> <a id="30174" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="30211" class="Keyword">open</a> <a id="30216" class="Keyword">import</a> <a id="30223" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="30250" class="Keyword">open</a> <a id="30255" class="Keyword">import</a> <a id="30262" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="30295" class="Keyword">open</a> <a id="30300" class="Keyword">import</a> <a id="30307" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="30325" class="Keyword">open</a> <a id="30330" class="Keyword">import</a> <a id="30337" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="30391" class="Keyword">open</a> <a id="30396" class="Keyword">import</a> <a id="30403" href="set-theory.html" class="Module">set-theory</a>
<a id="30414" class="Keyword">open</a> <a id="30419" class="Keyword">import</a> <a id="30426" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="30449" class="Keyword">open</a> <a id="30454" class="Keyword">import</a> <a id="30461" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="30485" class="Keyword">open</a> <a id="30490" class="Keyword">import</a> <a id="30497" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="30523" class="Keyword">open</a> <a id="30528" class="Keyword">import</a> <a id="30535" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="30597" class="Keyword">open</a> <a id="30602" class="Keyword">import</a> <a id="30609" href="structured-types.html" class="Module">structured-types</a>
<a id="30626" class="Keyword">open</a> <a id="30631" class="Keyword">import</a> <a id="30638" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="30673" class="Keyword">open</a> <a id="30678" class="Keyword">import</a> <a id="30685" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="30729" class="Keyword">open</a> <a id="30734" class="Keyword">import</a> <a id="30741" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="30805" class="Keyword">open</a> <a id="30810" class="Keyword">import</a> <a id="30817" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="30863" class="Keyword">open</a> <a id="30868" class="Keyword">import</a> <a id="30875" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="30899" class="Keyword">open</a> <a id="30904" class="Keyword">import</a> <a id="30911" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="30980" class="Keyword">open</a> <a id="30985" class="Keyword">import</a> <a id="30992" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="31037" class="Keyword">open</a> <a id="31042" class="Keyword">import</a> <a id="31049" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="31083" class="Keyword">open</a> <a id="31088" class="Keyword">import</a> <a id="31095" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="31156" class="Keyword">open</a> <a id="31161" class="Keyword">import</a> <a id="31168" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="31213" class="Keyword">open</a> <a id="31218" class="Keyword">import</a> <a id="31225" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="31263" class="Keyword">open</a> <a id="31268" class="Keyword">import</a> <a id="31275" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="31318" class="Keyword">open</a> <a id="31323" class="Keyword">import</a> <a id="31330" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="31366" class="Keyword">open</a> <a id="31371" class="Keyword">import</a> <a id="31378" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="31408" class="Keyword">open</a> <a id="31413" class="Keyword">import</a> <a id="31420" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="31451" class="Keyword">open</a> <a id="31456" class="Keyword">import</a> <a id="31463" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="31522" class="Keyword">open</a> <a id="31527" class="Keyword">import</a> <a id="31534" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="31585" class="Keyword">open</a> <a id="31590" class="Keyword">import</a> <a id="31597" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="31648" class="Keyword">open</a> <a id="31653" class="Keyword">import</a> <a id="31660" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="31715" class="Keyword">open</a> <a id="31720" class="Keyword">import</a> <a id="31727" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="31756" class="Keyword">open</a> <a id="31761" class="Keyword">import</a> <a id="31768" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="31796" class="Keyword">open</a> <a id="31801" class="Keyword">import</a> <a id="31808" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="31838" class="Keyword">open</a> <a id="31843" class="Keyword">import</a> <a id="31850" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="31884" class="Keyword">open</a> <a id="31889" class="Keyword">import</a> <a id="31896" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="31972" class="Keyword">open</a> <a id="31977" class="Keyword">import</a> <a id="31984" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="32010" class="Keyword">open</a> <a id="32015" class="Keyword">import</a> <a id="32022" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="32061" class="Keyword">open</a> <a id="32066" class="Keyword">import</a> <a id="32073" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="32111" class="Keyword">open</a> <a id="32116" class="Keyword">import</a> <a id="32123" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="32169" class="Keyword">open</a> <a id="32174" class="Keyword">import</a> <a id="32181" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="32218" class="Keyword">open</a> <a id="32223" class="Keyword">import</a> <a id="32230" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="32270" class="Keyword">open</a> <a id="32275" class="Keyword">import</a> <a id="32282" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="32321" class="Keyword">open</a> <a id="32326" class="Keyword">import</a> <a id="32333" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="32366" class="Keyword">open</a> <a id="32371" class="Keyword">import</a> <a id="32378" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="32413" class="Keyword">open</a> <a id="32418" class="Keyword">import</a> <a id="32425" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="32470" class="Keyword">open</a> <a id="32475" class="Keyword">import</a> <a id="32482" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="32534" class="Keyword">open</a> <a id="32539" class="Keyword">import</a> <a id="32546" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="32599" class="Keyword">open</a> <a id="32604" class="Keyword">import</a> <a id="32611" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="32659" class="Keyword">open</a> <a id="32664" class="Keyword">import</a> <a id="32671" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="32711" class="Keyword">open</a> <a id="32716" class="Keyword">import</a> <a id="32723" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="32770" class="Keyword">open</a> <a id="32775" class="Keyword">import</a> <a id="32782" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="32823" class="Keyword">open</a> <a id="32828" class="Keyword">import</a> <a id="32835" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="32873" class="Keyword">open</a> <a id="32878" class="Keyword">import</a> <a id="32885" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="32933" class="Keyword">open</a> <a id="32938" class="Keyword">import</a> <a id="32945" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="32990" class="Keyword">open</a> <a id="32995" class="Keyword">import</a> <a id="33002" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="33051" class="Keyword">open</a> <a id="33056" class="Keyword">import</a> <a id="33063" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="33140" class="Keyword">open</a> <a id="33145" class="Keyword">import</a> <a id="33152" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="33204" class="Keyword">open</a> <a id="33209" class="Keyword">import</a> <a id="33216" href="type-theories.html" class="Module">type-theories</a>
<a id="33230" class="Keyword">open</a> <a id="33235" class="Keyword">import</a> <a id="33242" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="33284" class="Keyword">open</a> <a id="33289" class="Keyword">import</a> <a id="33296" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="33334" class="Keyword">open</a> <a id="33339" class="Keyword">import</a> <a id="33346" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="33392" class="Keyword">open</a> <a id="33397" class="Keyword">import</a> <a id="33404" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="33451" class="Keyword">open</a> <a id="33456" class="Keyword">import</a> <a id="33463" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="33498" class="Keyword">open</a> <a id="33503" class="Keyword">import</a> <a id="33510" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="33588" class="Keyword">open</a> <a id="33593" class="Keyword">import</a> <a id="33600" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="33624" class="Keyword">open</a> <a id="33629" class="Keyword">import</a> <a id="33636" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="33689" class="Keyword">open</a> <a id="33694" class="Keyword">import</a> <a id="33701" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="33744" class="Keyword">open</a> <a id="33749" class="Keyword">import</a> <a id="33756" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="33796" class="Keyword">open</a> <a id="33801" class="Keyword">import</a> <a id="33808" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="33847" class="Keyword">open</a> <a id="33852" class="Keyword">import</a> <a id="33859" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="33893" class="Keyword">open</a> <a id="33898" class="Keyword">import</a> <a id="33905" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="33953" class="Keyword">open</a> <a id="33958" class="Keyword">import</a> <a id="33965" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="34016" class="Keyword">open</a> <a id="34021" class="Keyword">import</a> <a id="34028" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="34075" class="Keyword">open</a> <a id="34080" class="Keyword">import</a> <a id="34087" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="34139" class="Keyword">open</a> <a id="34144" class="Keyword">import</a> <a id="34151" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="34195" class="Keyword">open</a> <a id="34200" class="Keyword">import</a> <a id="34207" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="34247" class="Keyword">open</a> <a id="34252" class="Keyword">import</a> <a id="34259" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="34302" class="Keyword">open</a> <a id="34307" class="Keyword">import</a> <a id="34314" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="34366" class="Keyword">open</a> <a id="34371" class="Keyword">import</a> <a id="34378" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="34432" class="Keyword">open</a> <a id="34437" class="Keyword">import</a> <a id="34444" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="34492" class="Keyword">open</a> <a id="34497" class="Keyword">import</a> <a id="34504" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="34543" class="Keyword">open</a> <a id="34548" class="Keyword">import</a> <a id="34555" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="34588" class="Keyword">open</a> <a id="34593" class="Keyword">import</a> <a id="34600" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="34630" class="Keyword">open</a> <a id="34635" class="Keyword">import</a> <a id="34642" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="34693" class="Keyword">open</a> <a id="34698" class="Keyword">import</a> <a id="34705" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="34746" class="Keyword">open</a> <a id="34751" class="Keyword">import</a> <a id="34758" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="34795" class="Keyword">open</a> <a id="34800" class="Keyword">import</a> <a id="34807" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="34866" class="Keyword">open</a> <a id="34871" class="Keyword">import</a> <a id="34878" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="34933" class="Keyword">open</a> <a id="34938" class="Keyword">import</a> <a id="34945" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="34992" class="Keyword">open</a> <a id="34997" class="Keyword">import</a> <a id="35004" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="35047" class="Keyword">open</a> <a id="35052" class="Keyword">import</a> <a id="35059" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="35104" class="Keyword">open</a> <a id="35109" class="Keyword">import</a> <a id="35116" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="35165" class="Keyword">open</a> <a id="35170" class="Keyword">import</a> <a id="35177" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="35228" class="Keyword">open</a> <a id="35233" class="Keyword">import</a> <a id="35240" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="35284" class="Keyword">open</a> <a id="35289" class="Keyword">import</a> <a id="35296" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="35374" class="Keyword">open</a> <a id="35379" class="Keyword">import</a> <a id="35386" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="35426" class="Keyword">open</a> <a id="35431" class="Keyword">import</a> <a id="35438" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="35495" class="Keyword">open</a> <a id="35500" class="Keyword">import</a> <a id="35507" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="35542" class="Keyword">open</a> <a id="35547" class="Keyword">import</a> <a id="35554" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="35600" class="Keyword">open</a> <a id="35605" class="Keyword">import</a> <a id="35612" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="35667" class="Keyword">open</a> <a id="35672" class="Keyword">import</a> <a id="35679" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="35722" class="Keyword">open</a> <a id="35727" class="Keyword">import</a> <a id="35734" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="35779" class="Keyword">open</a> <a id="35784" class="Keyword">import</a> <a id="35791" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="35850" class="Keyword">open</a> <a id="35855" class="Keyword">import</a> <a id="35862" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="35899" class="Keyword">open</a> <a id="35904" class="Keyword">import</a> <a id="35911" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="35953" class="Keyword">open</a> <a id="35958" class="Keyword">import</a> <a id="35965" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="36006" class="Keyword">open</a> <a id="36011" class="Keyword">import</a> <a id="36018" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="36057" class="Keyword">open</a> <a id="36062" class="Keyword">import</a> <a id="36069" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="36107" class="Keyword">open</a> <a id="36112" class="Keyword">import</a> <a id="36119" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="36171" class="Keyword">open</a> <a id="36176" class="Keyword">import</a> <a id="36183" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="36228" class="Keyword">open</a> <a id="36233" class="Keyword">import</a> <a id="36240" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="36279" class="Keyword">open</a> <a id="36284" class="Keyword">import</a> <a id="36291" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="36328" class="Keyword">open</a> <a id="36333" class="Keyword">import</a> <a id="36340" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="36389" class="Keyword">open</a> <a id="36394" class="Keyword">import</a> <a id="36401" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="36440" class="Keyword">open</a> <a id="36445" class="Keyword">import</a> <a id="36452" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="36490" class="Keyword">open</a> <a id="36495" class="Keyword">import</a> <a id="36502" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="36557" class="Keyword">open</a> <a id="36562" class="Keyword">import</a> <a id="36569" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="36608" class="Keyword">open</a> <a id="36613" class="Keyword">import</a> <a id="36620" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="36668" class="Keyword">open</a> <a id="36673" class="Keyword">import</a> <a id="36680" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="36727" class="Keyword">open</a> <a id="36732" class="Keyword">import</a> <a id="36739" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="36777" class="Keyword">open</a> <a id="36782" class="Keyword">import</a> <a id="36789" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="36819" class="Keyword">open</a> <a id="36824" class="Keyword">import</a> <a id="36831" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="36888" class="Keyword">open</a> <a id="36893" class="Keyword">import</a> <a id="36900" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="36954" class="Keyword">open</a> <a id="36959" class="Keyword">import</a> <a id="36966" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="36996" class="Keyword">open</a> <a id="37001" class="Keyword">import</a> <a id="37008" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="37057" class="Keyword">open</a> <a id="37062" class="Keyword">import</a> <a id="37069" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="37111" class="Keyword">open</a> <a id="37116" class="Keyword">import</a> <a id="37123" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="37157" class="Keyword">open</a> <a id="37162" class="Keyword">import</a> <a id="37169" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="37232" class="Keyword">open</a> <a id="37237" class="Keyword">import</a> <a id="37244" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="37287" class="Keyword">open</a> <a id="37292" class="Keyword">import</a> <a id="37299" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="37334" class="Keyword">open</a> <a id="37339" class="Keyword">import</a> <a id="37346" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="37381" class="Keyword">open</a> <a id="37386" class="Keyword">import</a> <a id="37393" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="37433" class="Keyword">open</a> <a id="37438" class="Keyword">import</a> <a id="37445" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="37490" class="Keyword">open</a> <a id="37495" class="Keyword">import</a> <a id="37502" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="37543" class="Keyword">open</a> <a id="37548" class="Keyword">import</a> <a id="37555" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="37609" class="Keyword">open</a> <a id="37614" class="Keyword">import</a> <a id="37621" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="37671" class="Keyword">open</a> <a id="37676" class="Keyword">import</a> <a id="37683" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="37721" class="Keyword">open</a> <a id="37726" class="Keyword">import</a> <a id="37733" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="37782" class="Keyword">open</a> <a id="37787" class="Keyword">import</a> <a id="37794" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="37841" class="Keyword">open</a> <a id="37846" class="Keyword">import</a> <a id="37853" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="37916" class="Keyword">open</a> <a id="37921" class="Keyword">import</a> <a id="37928" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="37960" class="Keyword">open</a> <a id="37965" class="Keyword">import</a> <a id="37972" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="38025" class="Keyword">open</a> <a id="38030" class="Keyword">import</a> <a id="38037" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="38083" class="Keyword">open</a> <a id="38088" class="Keyword">import</a> <a id="38095" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="38141" class="Keyword">open</a> <a id="38146" class="Keyword">import</a> <a id="38153" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="38201" class="Keyword">open</a> <a id="38206" class="Keyword">import</a> <a id="38213" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="38253" class="Keyword">open</a> <a id="38258" class="Keyword">import</a> <a id="38265" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="38310" class="Keyword">open</a> <a id="38315" class="Keyword">import</a> <a id="38322" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="38387" class="Keyword">open</a> <a id="38392" class="Keyword">import</a> <a id="38399" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="38444" class="Keyword">open</a> <a id="38449" class="Keyword">import</a> <a id="38456" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="38503" class="Keyword">open</a> <a id="38508" class="Keyword">import</a> <a id="38515" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="38568" class="Keyword">open</a> <a id="38573" class="Keyword">import</a> <a id="38580" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>