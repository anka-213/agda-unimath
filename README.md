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
<a id="14901" class="Keyword">open</a> <a id="14906" class="Keyword">import</a> <a id="14913" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="14953" class="Keyword">open</a> <a id="14958" class="Keyword">import</a> <a id="14965" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15005" class="Keyword">open</a> <a id="15010" class="Keyword">import</a> <a id="15017" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15067" class="Keyword">open</a> <a id="15072" class="Keyword">import</a> <a id="15079" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15118" class="Keyword">open</a> <a id="15123" class="Keyword">import</a> <a id="15130" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15170" class="Keyword">open</a> <a id="15175" class="Keyword">import</a> <a id="15182" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15215" class="Keyword">open</a> <a id="15220" class="Keyword">import</a> <a id="15227" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15276" class="Keyword">open</a> <a id="15281" class="Keyword">import</a> <a id="15288" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15313" class="Keyword">open</a> <a id="15318" class="Keyword">import</a> <a id="15325" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15363" class="Keyword">open</a> <a id="15368" class="Keyword">import</a> <a id="15375" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15397" class="Keyword">open</a> <a id="15402" class="Keyword">import</a> <a id="15409" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15437" class="Keyword">open</a> <a id="15442" class="Keyword">import</a> <a id="15449" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15485" class="Keyword">open</a> <a id="15490" class="Keyword">import</a> <a id="15497" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15523" class="Keyword">open</a> <a id="15528" class="Keyword">import</a> <a id="15535" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15553" class="Keyword">open</a> <a id="15558" class="Keyword">import</a> <a id="15565" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15600" class="Keyword">open</a> <a id="15605" class="Keyword">import</a> <a id="15612" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15647" class="Keyword">open</a> <a id="15652" class="Keyword">import</a> <a id="15659" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15686" class="Keyword">open</a> <a id="15691" class="Keyword">import</a> <a id="15698" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15754" class="Keyword">open</a> <a id="15759" class="Keyword">import</a> <a id="15766" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15795" class="Keyword">open</a> <a id="15800" class="Keyword">import</a> <a id="15807" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15837" class="Keyword">open</a> <a id="15842" class="Keyword">import</a> <a id="15849" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15876" class="Keyword">open</a> <a id="15881" class="Keyword">import</a> <a id="15888" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15914" class="Keyword">open</a> <a id="15919" class="Keyword">import</a> <a id="15926" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15953" class="Keyword">open</a> <a id="15958" class="Keyword">import</a> <a id="15965" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15989" class="Keyword">open</a> <a id="15994" class="Keyword">import</a> <a id="16001" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16024" class="Keyword">open</a> <a id="16029" class="Keyword">import</a> <a id="16036" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16063" class="Keyword">open</a> <a id="16068" class="Keyword">import</a> <a id="16075" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16107" class="Keyword">open</a> <a id="16112" class="Keyword">import</a> <a id="16119" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16154" class="Keyword">open</a> <a id="16159" class="Keyword">import</a> <a id="16166" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16197" class="Keyword">open</a> <a id="16202" class="Keyword">import</a> <a id="16209" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16242" class="Keyword">open</a> <a id="16247" class="Keyword">import</a> <a id="16254" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16288" class="Keyword">open</a> <a id="16293" class="Keyword">import</a> <a id="16300" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16340" class="Keyword">open</a> <a id="16345" class="Keyword">import</a> <a id="16352" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16383" class="Keyword">open</a> <a id="16388" class="Keyword">import</a> <a id="16395" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16427" class="Keyword">open</a> <a id="16432" class="Keyword">import</a> <a id="16439" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16470" class="Keyword">open</a> <a id="16475" class="Keyword">import</a> <a id="16482" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16499" class="Keyword">open</a> <a id="16504" class="Keyword">import</a> <a id="16511" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16536" class="Keyword">open</a> <a id="16541" class="Keyword">import</a> <a id="16548" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16577" class="Keyword">open</a> <a id="16582" class="Keyword">import</a> <a id="16589" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16614" class="Keyword">open</a> <a id="16619" class="Keyword">import</a> <a id="16626" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="16655" class="Keyword">open</a> <a id="16660" class="Keyword">import</a> <a id="16667" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16688" class="Keyword">open</a> <a id="16693" class="Keyword">import</a> <a id="16700" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16724" class="Keyword">open</a> <a id="16729" class="Keyword">import</a> <a id="16736" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16756" class="Keyword">open</a> <a id="16761" class="Keyword">import</a> <a id="16768" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16802" class="Keyword">open</a> <a id="16807" class="Keyword">import</a> <a id="16814" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16852" class="Keyword">open</a> <a id="16857" class="Keyword">import</a> <a id="16864" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16892" class="Keyword">open</a> <a id="16897" class="Keyword">import</a> <a id="16904" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16928" class="Keyword">open</a> <a id="16933" class="Keyword">import</a> <a id="16940" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16967" class="Keyword">open</a> <a id="16972" class="Keyword">import</a> <a id="16979" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17014" class="Keyword">open</a> <a id="17019" class="Keyword">import</a> <a id="17026" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17047" class="Keyword">open</a> <a id="17052" class="Keyword">import</a> <a id="17059" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17095" class="Keyword">open</a> <a id="17100" class="Keyword">import</a> <a id="17107" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17152" class="Keyword">open</a> <a id="17157" class="Keyword">import</a> <a id="17164" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17210" class="Keyword">open</a> <a id="17215" class="Keyword">import</a> <a id="17222" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17262" class="Keyword">open</a> <a id="17267" class="Keyword">import</a> <a id="17274" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17304" class="Keyword">open</a> <a id="17309" class="Keyword">import</a> <a id="17316" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17350" class="Keyword">open</a> <a id="17355" class="Keyword">import</a> <a id="17362" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17399" class="Keyword">open</a> <a id="17404" class="Keyword">import</a> <a id="17411" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17435" class="Keyword">open</a> <a id="17440" class="Keyword">import</a> <a id="17447" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17468" class="Keyword">open</a> <a id="17473" class="Keyword">import</a> <a id="17480" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17515" class="Keyword">open</a> <a id="17520" class="Keyword">import</a> <a id="17527" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17564" class="Keyword">open</a> <a id="17569" class="Keyword">import</a> <a id="17576" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17625" class="Keyword">open</a> <a id="17630" class="Keyword">import</a> <a id="17637" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17670" class="Keyword">open</a> <a id="17675" class="Keyword">import</a> <a id="17682" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17705" class="Keyword">open</a> <a id="17710" class="Keyword">import</a> <a id="17717" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17740" class="Keyword">open</a> <a id="17745" class="Keyword">import</a> <a id="17752" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17775" class="Keyword">open</a> <a id="17780" class="Keyword">import</a> <a id="17787" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17815" class="Keyword">open</a> <a id="17820" class="Keyword">import</a> <a id="17827" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17847" class="Keyword">open</a> <a id="17852" class="Keyword">import</a> <a id="17859" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17880" class="Keyword">open</a> <a id="17885" class="Keyword">import</a> <a id="17892" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17923" class="Keyword">open</a> <a id="17928" class="Keyword">import</a> <a id="17935" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17962" class="Keyword">open</a> <a id="17967" class="Keyword">import</a> <a id="17974" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17990" class="Keyword">open</a> <a id="17995" class="Keyword">import</a> <a id="18002" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18033" class="Keyword">open</a> <a id="18038" class="Keyword">import</a> <a id="18045" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18062" class="Keyword">open</a> <a id="18067" class="Keyword">import</a> <a id="18074" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18096" class="Keyword">open</a> <a id="18101" class="Keyword">import</a> <a id="18108" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18135" class="Keyword">open</a> <a id="18140" class="Keyword">import</a> <a id="18147" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18170" class="Keyword">open</a> <a id="18175" class="Keyword">import</a> <a id="18182" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18209" class="Keyword">open</a> <a id="18214" class="Keyword">import</a> <a id="18221" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18254" class="Keyword">open</a> <a id="18259" class="Keyword">import</a> <a id="18266" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18306" class="Keyword">open</a> <a id="18311" class="Keyword">import</a> <a id="18318" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18339" class="Keyword">open</a> <a id="18344" class="Keyword">import</a> <a id="18351" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18380" class="Keyword">open</a> <a id="18385" class="Keyword">import</a> <a id="18392" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18430" class="Keyword">open</a> <a id="18435" class="Keyword">import</a> <a id="18442" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18462" class="Keyword">open</a> <a id="18467" class="Keyword">import</a> <a id="18474" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18498" class="Keyword">open</a> <a id="18503" class="Keyword">import</a> <a id="18510" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18537" class="Keyword">open</a> <a id="18542" class="Keyword">import</a> <a id="18549" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18581" class="Keyword">open</a> <a id="18586" class="Keyword">import</a> <a id="18593" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18623" class="Keyword">open</a> <a id="18628" class="Keyword">import</a> <a id="18635" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18661" class="Keyword">open</a> <a id="18666" class="Keyword">import</a> <a id="18673" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18700" class="Keyword">open</a> <a id="18705" class="Keyword">import</a> <a id="18712" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="18749" class="Keyword">open</a> <a id="18754" class="Keyword">import</a> <a id="18761" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18790" class="Keyword">open</a> <a id="18795" class="Keyword">import</a> <a id="18802" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18825" class="Keyword">open</a> <a id="18830" class="Keyword">import</a> <a id="18837" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18888" class="Keyword">open</a> <a id="18893" class="Keyword">import</a> <a id="18900" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18943" class="Keyword">open</a> <a id="18948" class="Keyword">import</a> <a id="18955" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19007" class="Keyword">open</a> <a id="19012" class="Keyword">import</a> <a id="19019" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19067" class="Keyword">open</a> <a id="19072" class="Keyword">import</a> <a id="19079" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19117" class="Keyword">open</a> <a id="19122" class="Keyword">import</a> <a id="19129" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19166" class="Keyword">open</a> <a id="19171" class="Keyword">import</a> <a id="19178" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19224" class="Keyword">open</a> <a id="19229" class="Keyword">import</a> <a id="19236" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19253" class="Keyword">open</a> <a id="19258" class="Keyword">import</a> <a id="19265" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19293" class="Keyword">open</a> <a id="19298" class="Keyword">import</a> <a id="19305" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19333" class="Keyword">open</a> <a id="19338" class="Keyword">import</a> <a id="19345" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19381" class="Keyword">open</a> <a id="19386" class="Keyword">import</a> <a id="19393" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19431" class="Keyword">open</a> <a id="19436" class="Keyword">import</a> <a id="19443" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19476" class="Keyword">open</a> <a id="19481" class="Keyword">import</a> <a id="19488" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19509" class="Keyword">open</a> <a id="19514" class="Keyword">import</a> <a id="19521" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19557" class="Keyword">open</a> <a id="19562" class="Keyword">import</a> <a id="19569" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19623" class="Keyword">open</a> <a id="19628" class="Keyword">import</a> <a id="19635" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19657" class="Keyword">open</a> <a id="19662" class="Keyword">import</a> <a id="19669" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19704" class="Keyword">open</a> <a id="19709" class="Keyword">import</a> <a id="19716" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19746" class="Keyword">open</a> <a id="19751" class="Keyword">import</a> <a id="19758" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19797" class="Keyword">open</a> <a id="19802" class="Keyword">import</a> <a id="19809" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19863" class="Keyword">open</a> <a id="19868" class="Keyword">import</a> <a id="19875" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19921" class="Keyword">open</a> <a id="19926" class="Keyword">import</a> <a id="19933" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19984" class="Keyword">open</a> <a id="19989" class="Keyword">import</a> <a id="19996" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20037" class="Keyword">open</a> <a id="20042" class="Keyword">import</a> <a id="20049" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20094" class="Keyword">open</a> <a id="20099" class="Keyword">import</a> <a id="20106" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20151" class="Keyword">open</a> <a id="20156" class="Keyword">import</a> <a id="20163" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20199" class="Keyword">open</a> <a id="20204" class="Keyword">import</a> <a id="20211" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20247" class="Keyword">open</a> <a id="20252" class="Keyword">import</a> <a id="20259" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20324" class="Keyword">open</a> <a id="20329" class="Keyword">import</a> <a id="20336" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20391" class="Keyword">open</a> <a id="20396" class="Keyword">import</a> <a id="20403" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20443" class="Keyword">open</a> <a id="20448" class="Keyword">import</a> <a id="20455" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20499" class="Keyword">open</a> <a id="20504" class="Keyword">import</a> <a id="20511" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20556" class="Keyword">open</a> <a id="20561" class="Keyword">import</a> <a id="20568" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20609" class="Keyword">open</a> <a id="20614" class="Keyword">import</a> <a id="20621" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20661" class="Keyword">open</a> <a id="20666" class="Keyword">import</a> <a id="20673" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20700" class="Keyword">open</a> <a id="20705" class="Keyword">import</a> <a id="20712" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20748" class="Keyword">open</a> <a id="20753" class="Keyword">import</a> <a id="20760" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20787" class="Keyword">open</a> <a id="20792" class="Keyword">import</a> <a id="20799" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20836" class="Keyword">open</a> <a id="20841" class="Keyword">import</a> <a id="20848" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20876" class="Keyword">open</a> <a id="20881" class="Keyword">import</a> <a id="20888" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20907" class="Keyword">open</a> <a id="20912" class="Keyword">import</a> <a id="20919" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20959" class="Keyword">open</a> <a id="20964" class="Keyword">import</a> <a id="20971" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21003" class="Keyword">open</a> <a id="21008" class="Keyword">import</a> <a id="21015" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21063" class="Keyword">open</a> <a id="21068" class="Keyword">import</a> <a id="21075" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21098" class="Keyword">open</a> <a id="21103" class="Keyword">import</a> <a id="21110" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21134" class="Keyword">open</a> <a id="21139" class="Keyword">import</a> <a id="21146" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21186" class="Keyword">open</a> <a id="21191" class="Keyword">import</a> <a id="21198" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="21241" class="Keyword">open</a> <a id="21246" class="Keyword">import</a> <a id="21253" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21287" class="Keyword">open</a> <a id="21292" class="Keyword">import</a> <a id="21299" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21331" class="Keyword">open</a> <a id="21336" class="Keyword">import</a> <a id="21343" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21373" class="Keyword">open</a> <a id="21378" class="Keyword">import</a> <a id="21385" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21419" class="Keyword">open</a> <a id="21424" class="Keyword">import</a> <a id="21431" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21466" class="Keyword">open</a> <a id="21471" class="Keyword">import</a> <a id="21478" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21515" class="Keyword">open</a> <a id="21520" class="Keyword">import</a> <a id="21527" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21554" class="Keyword">open</a> <a id="21559" class="Keyword">import</a> <a id="21566" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21594" class="Keyword">open</a> <a id="21599" class="Keyword">import</a> <a id="21606" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21655" class="Keyword">open</a> <a id="21660" class="Keyword">import</a> <a id="21667" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21713" class="Keyword">open</a> <a id="21718" class="Keyword">import</a> <a id="21725" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21765" class="Keyword">open</a> <a id="21770" class="Keyword">import</a> <a id="21777" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21815" class="Keyword">open</a> <a id="21820" class="Keyword">import</a> <a id="21827" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21856" class="Keyword">open</a> <a id="21861" class="Keyword">import</a> <a id="21868" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21898" class="Keyword">open</a> <a id="21903" class="Keyword">import</a> <a id="21910" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21941" class="Keyword">open</a> <a id="21946" class="Keyword">import</a> <a id="21953" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21993" class="Keyword">open</a> <a id="21998" class="Keyword">import</a> <a id="22005" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22031" class="Keyword">open</a> <a id="22036" class="Keyword">import</a> <a id="22043" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="22098" class="Keyword">open</a> <a id="22103" class="Keyword">import</a> <a id="22110" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="22161" class="Keyword">open</a> <a id="22166" class="Keyword">import</a> <a id="22173" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="22218" class="Keyword">open</a> <a id="22223" class="Keyword">import</a> <a id="22230" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="22275" class="Keyword">open</a> <a id="22280" class="Keyword">import</a> <a id="22287" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22341" class="Keyword">open</a> <a id="22346" class="Keyword">import</a> <a id="22353" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22380" class="Keyword">open</a> <a id="22385" class="Keyword">import</a> <a id="22392" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22425" class="Keyword">open</a> <a id="22430" class="Keyword">import</a> <a id="22437" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22468" class="Keyword">open</a> <a id="22473" class="Keyword">import</a> <a id="22480" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22517" class="Keyword">open</a> <a id="22522" class="Keyword">import</a> <a id="22529" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="22563" class="Keyword">open</a> <a id="22568" class="Keyword">import</a> <a id="22575" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22600" class="Keyword">open</a> <a id="22605" class="Keyword">import</a> <a id="22612" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22644" class="Keyword">open</a> <a id="22649" class="Keyword">import</a> <a id="22656" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22691" class="Keyword">open</a> <a id="22696" class="Keyword">import</a> <a id="22703" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22732" class="Keyword">open</a> <a id="22737" class="Keyword">import</a> <a id="22744" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22770" class="Keyword">open</a> <a id="22775" class="Keyword">import</a> <a id="22782" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22810" class="Keyword">open</a> <a id="22815" class="Keyword">import</a> <a id="22822" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22847" class="Keyword">open</a> <a id="22852" class="Keyword">import</a> <a id="22859" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22880" class="Keyword">open</a> <a id="22885" class="Keyword">import</a> <a id="22892" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22928" class="Keyword">open</a> <a id="22933" class="Keyword">import</a> <a id="22940" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22983" class="Keyword">open</a> <a id="22988" class="Keyword">import</a> <a id="22995" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23020" class="Keyword">open</a> <a id="23025" class="Keyword">import</a> <a id="23032" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23063" class="Keyword">open</a> <a id="23068" class="Keyword">import</a> <a id="23075" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="23107" class="Keyword">open</a> <a id="23112" class="Keyword">import</a> <a id="23119" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="23153" class="Keyword">open</a> <a id="23158" class="Keyword">import</a> <a id="23165" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="23221" class="Keyword">open</a> <a id="23226" class="Keyword">import</a> <a id="23233" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="23286" class="Keyword">open</a> <a id="23291" class="Keyword">import</a> <a id="23298" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="23325" class="Keyword">open</a> <a id="23330" class="Keyword">import</a> <a id="23337" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23382" class="Keyword">open</a> <a id="23387" class="Keyword">import</a> <a id="23394" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23456" class="Keyword">open</a> <a id="23461" class="Keyword">import</a> <a id="23468" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23481" class="Keyword">open</a> <a id="23486" class="Keyword">import</a> <a id="23493" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23533" class="Keyword">open</a> <a id="23538" class="Keyword">import</a> <a id="23545" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23589" class="Keyword">open</a> <a id="23594" class="Keyword">import</a> <a id="23601" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23640" class="Keyword">open</a> <a id="23645" class="Keyword">import</a> <a id="23652" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23694" class="Keyword">open</a> <a id="23699" class="Keyword">import</a> <a id="23706" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23746" class="Keyword">open</a> <a id="23751" class="Keyword">import</a> <a id="23758" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23799" class="Keyword">open</a> <a id="23804" class="Keyword">import</a> <a id="23811" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23849" class="Keyword">open</a> <a id="23854" class="Keyword">import</a> <a id="23861" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23924" class="Keyword">open</a> <a id="23929" class="Keyword">import</a> <a id="23936" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23965" class="Keyword">open</a> <a id="23970" class="Keyword">import</a> <a id="23977" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24022" class="Keyword">open</a> <a id="24027" class="Keyword">import</a> <a id="24034" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24076" class="Keyword">open</a> <a id="24081" class="Keyword">import</a> <a id="24088" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="24132" class="Keyword">open</a> <a id="24137" class="Keyword">import</a> <a id="24144" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="24193" class="Keyword">open</a> <a id="24198" class="Keyword">import</a> <a id="24205" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="24255" class="Keyword">open</a> <a id="24260" class="Keyword">import</a> <a id="24267" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="24294" class="Keyword">open</a> <a id="24299" class="Keyword">import</a> <a id="24306" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="24331" class="Keyword">open</a> <a id="24336" class="Keyword">import</a> <a id="24343" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24384" class="Keyword">open</a> <a id="24389" class="Keyword">import</a> <a id="24396" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24419" class="Keyword">open</a> <a id="24424" class="Keyword">import</a> <a id="24431" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24480" class="Keyword">open</a> <a id="24485" class="Keyword">import</a> <a id="24492" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24531" class="Keyword">open</a> <a id="24536" class="Keyword">import</a> <a id="24543" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24584" class="Keyword">open</a> <a id="24589" class="Keyword">import</a> <a id="24596" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24640" class="Keyword">open</a> <a id="24645" class="Keyword">import</a> <a id="24652" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24689" class="Keyword">open</a> <a id="24694" class="Keyword">import</a> <a id="24701" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24723" class="Keyword">open</a> <a id="24728" class="Keyword">import</a> <a id="24735" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24765" class="Keyword">open</a> <a id="24770" class="Keyword">import</a> <a id="24777" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24816" class="Keyword">open</a> <a id="24821" class="Keyword">import</a> <a id="24828" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24866" class="Keyword">open</a> <a id="24871" class="Keyword">import</a> <a id="24878" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24936" class="Keyword">open</a> <a id="24941" class="Keyword">import</a> <a id="24948" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="25013" class="Keyword">open</a> <a id="25018" class="Keyword">import</a> <a id="25025" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="25056" class="Keyword">open</a> <a id="25061" class="Keyword">import</a> <a id="25068" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="25095" class="Keyword">open</a> <a id="25100" class="Keyword">import</a> <a id="25107" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="25165" class="Keyword">open</a> <a id="25170" class="Keyword">import</a> <a id="25177" href="group-theory.html" class="Module">group-theory</a>
<a id="25190" class="Keyword">open</a> <a id="25195" class="Keyword">import</a> <a id="25202" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="25230" class="Keyword">open</a> <a id="25235" class="Keyword">import</a> <a id="25242" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25293" class="Keyword">open</a> <a id="25298" class="Keyword">import</a> <a id="25305" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25338" class="Keyword">open</a> <a id="25343" class="Keyword">import</a> <a id="25350" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="25397" class="Keyword">open</a> <a id="25402" class="Keyword">import</a> <a id="25409" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="25448" class="Keyword">open</a> <a id="25453" class="Keyword">import</a> <a id="25460" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25500" class="Keyword">open</a> <a id="25505" class="Keyword">import</a> <a id="25512" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25555" class="Keyword">open</a> <a id="25560" class="Keyword">import</a> <a id="25567" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25599" class="Keyword">open</a> <a id="25604" class="Keyword">import</a> <a id="25611" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25647" class="Keyword">open</a> <a id="25652" class="Keyword">import</a> <a id="25659" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25688" class="Keyword">open</a> <a id="25693" class="Keyword">import</a> <a id="25700" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25728" class="Keyword">open</a> <a id="25733" class="Keyword">import</a> <a id="25740" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25773" class="Keyword">open</a> <a id="25778" class="Keyword">import</a> <a id="25785" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25821" class="Keyword">open</a> <a id="25826" class="Keyword">import</a> <a id="25833" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25862" class="Keyword">open</a> <a id="25867" class="Keyword">import</a> <a id="25874" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25899" class="Keyword">open</a> <a id="25904" class="Keyword">import</a> <a id="25911" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25973" class="Keyword">open</a> <a id="25978" class="Keyword">import</a> <a id="25985" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="26016" class="Keyword">open</a> <a id="26021" class="Keyword">import</a> <a id="26028" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="26075" class="Keyword">open</a> <a id="26080" class="Keyword">import</a> <a id="26087" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="26120" class="Keyword">open</a> <a id="26125" class="Keyword">import</a> <a id="26132" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="26181" class="Keyword">open</a> <a id="26186" class="Keyword">import</a> <a id="26193" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="26233" class="Keyword">open</a> <a id="26238" class="Keyword">import</a> <a id="26245" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="26282" class="Keyword">open</a> <a id="26287" class="Keyword">import</a> <a id="26294" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="26341" class="Keyword">open</a> <a id="26346" class="Keyword">import</a> <a id="26353" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="26394" class="Keyword">open</a> <a id="26399" class="Keyword">import</a> <a id="26406" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="26445" class="Keyword">open</a> <a id="26450" class="Keyword">import</a> <a id="26457" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="26489" class="Keyword">open</a> <a id="26494" class="Keyword">import</a> <a id="26501" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="26528" class="Keyword">open</a> <a id="26533" class="Keyword">import</a> <a id="26540" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26560" class="Keyword">open</a> <a id="26565" class="Keyword">import</a> <a id="26572" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26606" class="Keyword">open</a> <a id="26611" class="Keyword">import</a> <a id="26618" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26645" class="Keyword">open</a> <a id="26650" class="Keyword">import</a> <a id="26657" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26699" class="Keyword">open</a> <a id="26704" class="Keyword">import</a> <a id="26711" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26761" class="Keyword">open</a> <a id="26766" class="Keyword">import</a> <a id="26773" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26820" class="Keyword">open</a> <a id="26825" class="Keyword">import</a> <a id="26832" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="26873" class="Keyword">open</a> <a id="26878" class="Keyword">import</a> <a id="26885" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26919" class="Keyword">open</a> <a id="26924" class="Keyword">import</a> <a id="26931" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="26972" class="Keyword">open</a> <a id="26977" class="Keyword">import</a> <a id="26984" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="27019" class="Keyword">open</a> <a id="27024" class="Keyword">import</a> <a id="27031" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="27069" class="Keyword">open</a> <a id="27074" class="Keyword">import</a> <a id="27081" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="27116" class="Keyword">open</a> <a id="27121" class="Keyword">import</a> <a id="27128" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="27160" class="Keyword">open</a> <a id="27165" class="Keyword">import</a> <a id="27172" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="27213" class="Keyword">open</a> <a id="27218" class="Keyword">import</a> <a id="27225" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="27266" class="Keyword">open</a> <a id="27271" class="Keyword">import</a> <a id="27278" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="27318" class="Keyword">open</a> <a id="27323" class="Keyword">import</a> <a id="27330" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="27363" class="Keyword">open</a> <a id="27368" class="Keyword">import</a> <a id="27375" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="27412" class="Keyword">open</a> <a id="27417" class="Keyword">import</a> <a id="27424" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="27454" class="Keyword">open</a> <a id="27459" class="Keyword">import</a> <a id="27466" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="27487" class="Keyword">open</a> <a id="27492" class="Keyword">import</a> <a id="27499" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="27553" class="Keyword">open</a> <a id="27558" class="Keyword">import</a> <a id="27565" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27610" class="Keyword">open</a> <a id="27615" class="Keyword">import</a> <a id="27622" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27650" class="Keyword">open</a> <a id="27655" class="Keyword">import</a> <a id="27662" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27683" class="Keyword">open</a> <a id="27688" class="Keyword">import</a> <a id="27695" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27738" class="Keyword">open</a> <a id="27743" class="Keyword">import</a> <a id="27750" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27784" class="Keyword">open</a> <a id="27789" class="Keyword">import</a> <a id="27796" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27826" class="Keyword">open</a> <a id="27831" class="Keyword">import</a> <a id="27838" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="27884" class="Keyword">open</a> <a id="27889" class="Keyword">import</a> <a id="27896" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="27950" class="Keyword">open</a> <a id="27955" class="Keyword">import</a> <a id="27962" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="28005" class="Keyword">open</a> <a id="28010" class="Keyword">import</a> <a id="28017" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="28051" class="Keyword">open</a> <a id="28056" class="Keyword">import</a> <a id="28063" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="28104" class="Keyword">open</a> <a id="28109" class="Keyword">import</a> <a id="28116" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="28151" class="Keyword">open</a> <a id="28156" class="Keyword">import</a> <a id="28163" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="28205" class="Keyword">open</a> <a id="28210" class="Keyword">import</a> <a id="28217" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="28252" class="Keyword">open</a> <a id="28257" class="Keyword">import</a> <a id="28264" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="28303" class="Keyword">open</a> <a id="28308" class="Keyword">import</a> <a id="28315" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="28352" class="Keyword">open</a> <a id="28357" class="Keyword">import</a> <a id="28364" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="28411" class="Keyword">open</a> <a id="28416" class="Keyword">import</a> <a id="28423" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="28487" class="Keyword">open</a> <a id="28492" class="Keyword">import</a> <a id="28499" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="28544" class="Keyword">open</a> <a id="28549" class="Keyword">import</a> <a id="28556" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="28580" class="Keyword">open</a> <a id="28585" class="Keyword">import</a> <a id="28592" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="28617" class="Keyword">open</a> <a id="28622" class="Keyword">import</a> <a id="28629" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28672" class="Keyword">open</a> <a id="28677" class="Keyword">import</a> <a id="28684" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28715" class="Keyword">open</a> <a id="28720" class="Keyword">import</a> <a id="28727" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28781" class="Keyword">open</a> <a id="28786" class="Keyword">import</a> <a id="28793" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28816" class="Keyword">open</a> <a id="28821" class="Keyword">import</a> <a id="28828" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="28866" class="Keyword">open</a> <a id="28871" class="Keyword">import</a> <a id="28878" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="28917" class="Keyword">open</a> <a id="28922" class="Keyword">import</a> <a id="28929" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="28980" class="Keyword">open</a> <a id="28985" class="Keyword">import</a> <a id="28992" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="29029" class="Keyword">open</a> <a id="29034" class="Keyword">import</a> <a id="29041" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="29098" class="Keyword">open</a> <a id="29103" class="Keyword">import</a> <a id="29110" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="29158" class="Keyword">open</a> <a id="29163" class="Keyword">import</a> <a id="29170" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="29200" class="Keyword">open</a> <a id="29205" class="Keyword">import</a> <a id="29212" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="29249" class="Keyword">open</a> <a id="29254" class="Keyword">import</a> <a id="29261" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="29282" class="Keyword">open</a> <a id="29287" class="Keyword">import</a> <a id="29294" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="29341" class="Keyword">open</a> <a id="29346" class="Keyword">import</a> <a id="29353" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="29391" class="Keyword">open</a> <a id="29396" class="Keyword">import</a> <a id="29403" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="29497" class="Keyword">open</a> <a id="29502" class="Keyword">import</a> <a id="29509" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="29524" class="Keyword">open</a> <a id="29529" class="Keyword">import</a> <a id="29536" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="29569" class="Keyword">open</a> <a id="29574" class="Keyword">import</a> <a id="29581" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="29613" class="Keyword">open</a> <a id="29618" class="Keyword">import</a> <a id="29625" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29667" class="Keyword">open</a> <a id="29672" class="Keyword">import</a> <a id="29679" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29717" class="Keyword">open</a> <a id="29722" class="Keyword">import</a> <a id="29729" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29766" class="Keyword">open</a> <a id="29771" class="Keyword">import</a> <a id="29778" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29811" class="Keyword">open</a> <a id="29816" class="Keyword">import</a> <a id="29823" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="29847" class="Keyword">open</a> <a id="29852" class="Keyword">import</a> <a id="29859" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="29898" class="Keyword">open</a> <a id="29903" class="Keyword">import</a> <a id="29910" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="29956" class="Keyword">open</a> <a id="29961" class="Keyword">import</a> <a id="29968" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="30013" class="Keyword">open</a> <a id="30018" class="Keyword">import</a> <a id="30025" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="30063" class="Keyword">open</a> <a id="30068" class="Keyword">import</a> <a id="30075" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="30107" class="Keyword">open</a> <a id="30112" class="Keyword">import</a> <a id="30119" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="30172" class="Keyword">open</a> <a id="30177" class="Keyword">import</a> <a id="30184" href="order-theory.html" class="Module">order-theory</a>
<a id="30197" class="Keyword">open</a> <a id="30202" class="Keyword">import</a> <a id="30209" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="30236" class="Keyword">open</a> <a id="30241" class="Keyword">import</a> <a id="30248" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="30278" class="Keyword">open</a> <a id="30283" class="Keyword">import</a> <a id="30290" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="30323" class="Keyword">open</a> <a id="30328" class="Keyword">import</a> <a id="30335" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="30371" class="Keyword">open</a> <a id="30376" class="Keyword">import</a> <a id="30383" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="30418" class="Keyword">open</a> <a id="30423" class="Keyword">import</a> <a id="30430" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="30457" class="Keyword">open</a> <a id="30462" class="Keyword">import</a> <a id="30469" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="30499" class="Keyword">open</a> <a id="30504" class="Keyword">import</a> <a id="30511" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="30547" class="Keyword">open</a> <a id="30552" class="Keyword">import</a> <a id="30559" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="30601" class="Keyword">open</a> <a id="30606" class="Keyword">import</a> <a id="30613" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="30645" class="Keyword">open</a> <a id="30650" class="Keyword">import</a> <a id="30657" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30688" class="Keyword">open</a> <a id="30693" class="Keyword">import</a> <a id="30700" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30726" class="Keyword">open</a> <a id="30731" class="Keyword">import</a> <a id="30738" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30767" class="Keyword">open</a> <a id="30772" class="Keyword">import</a> <a id="30779" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30816" class="Keyword">open</a> <a id="30821" class="Keyword">import</a> <a id="30828" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="30868" class="Keyword">open</a> <a id="30873" class="Keyword">import</a> <a id="30880" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="30902" class="Keyword">open</a> <a id="30907" class="Keyword">import</a> <a id="30914" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="30949" class="Keyword">open</a> <a id="30954" class="Keyword">import</a> <a id="30961" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="30999" class="Keyword">open</a> <a id="31004" class="Keyword">import</a> <a id="31011" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="31050" class="Keyword">open</a> <a id="31055" class="Keyword">import</a> <a id="31062" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="31097" class="Keyword">open</a> <a id="31102" class="Keyword">import</a> <a id="31109" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="31144" class="Keyword">open</a> <a id="31149" class="Keyword">import</a> <a id="31156" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="31194" class="Keyword">open</a> <a id="31199" class="Keyword">import</a> <a id="31206" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="31237" class="Keyword">open</a> <a id="31242" class="Keyword">import</a> <a id="31249" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="31291" class="Keyword">open</a> <a id="31296" class="Keyword">import</a> <a id="31303" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="31348" class="Keyword">open</a> <a id="31353" class="Keyword">import</a> <a id="31360" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="31393" class="Keyword">open</a> <a id="31398" class="Keyword">import</a> <a id="31405" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="31425" class="Keyword">open</a> <a id="31430" class="Keyword">import</a> <a id="31437" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="31460" class="Keyword">open</a> <a id="31465" class="Keyword">import</a> <a id="31472" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="31495" class="Keyword">open</a> <a id="31500" class="Keyword">import</a> <a id="31507" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="31533" class="Keyword">open</a> <a id="31538" class="Keyword">import</a> <a id="31545" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="31571" class="Keyword">open</a> <a id="31576" class="Keyword">import</a> <a id="31583" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="31647" class="Keyword">open</a> <a id="31652" class="Keyword">import</a> <a id="31659" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31677" class="Keyword">open</a> <a id="31682" class="Keyword">import</a> <a id="31689" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31716" class="Keyword">open</a> <a id="31721" class="Keyword">import</a> <a id="31728" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31754" class="Keyword">open</a> <a id="31759" class="Keyword">import</a> <a id="31766" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31792" class="Keyword">open</a> <a id="31797" class="Keyword">import</a> <a id="31804" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31830" class="Keyword">open</a> <a id="31835" class="Keyword">import</a> <a id="31842" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="31873" class="Keyword">open</a> <a id="31878" class="Keyword">import</a> <a id="31885" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="31948" class="Keyword">open</a> <a id="31953" class="Keyword">import</a> <a id="31960" href="polytopes.html" class="Module">polytopes</a>
<a id="31970" class="Keyword">open</a> <a id="31975" class="Keyword">import</a> <a id="31982" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="32040" class="Keyword">open</a> <a id="32045" class="Keyword">import</a> <a id="32052" href="ring-theory.html" class="Module">ring-theory</a>
<a id="32064" class="Keyword">open</a> <a id="32069" class="Keyword">import</a> <a id="32076" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="32113" class="Keyword">open</a> <a id="32118" class="Keyword">import</a> <a id="32125" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="32152" class="Keyword">open</a> <a id="32157" class="Keyword">import</a> <a id="32164" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="32196" class="Keyword">open</a> <a id="32201" class="Keyword">import</a> <a id="32208" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="32254" class="Keyword">open</a> <a id="32259" class="Keyword">import</a> <a id="32266" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="32291" class="Keyword">open</a> <a id="32296" class="Keyword">import</a> <a id="32303" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="32346" class="Keyword">open</a> <a id="32351" class="Keyword">import</a> <a id="32358" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="32396" class="Keyword">open</a> <a id="32401" class="Keyword">import</a> <a id="32408" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="32439" class="Keyword">open</a> <a id="32444" class="Keyword">import</a> <a id="32451" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="32475" class="Keyword">open</a> <a id="32480" class="Keyword">import</a> <a id="32487" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="32519" class="Keyword">open</a> <a id="32524" class="Keyword">import</a> <a id="32531" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="32557" class="Keyword">open</a> <a id="32562" class="Keyword">import</a> <a id="32569" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="32598" class="Keyword">open</a> <a id="32603" class="Keyword">import</a> <a id="32610" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="32647" class="Keyword">open</a> <a id="32652" class="Keyword">import</a> <a id="32659" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32688" class="Keyword">open</a> <a id="32693" class="Keyword">import</a> <a id="32700" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32727" class="Keyword">open</a> <a id="32732" class="Keyword">import</a> <a id="32739" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32776" class="Keyword">open</a> <a id="32781" class="Keyword">import</a> <a id="32788" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32815" class="Keyword">open</a> <a id="32820" class="Keyword">import</a> <a id="32827" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="32860" class="Keyword">open</a> <a id="32865" class="Keyword">import</a> <a id="32872" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="32890" class="Keyword">open</a> <a id="32895" class="Keyword">import</a> <a id="32902" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="32956" class="Keyword">open</a> <a id="32961" class="Keyword">import</a> <a id="32968" href="set-theory.html" class="Module">set-theory</a>
<a id="32979" class="Keyword">open</a> <a id="32984" class="Keyword">import</a> <a id="32991" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="33014" class="Keyword">open</a> <a id="33019" class="Keyword">import</a> <a id="33026" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="33050" class="Keyword">open</a> <a id="33055" class="Keyword">import</a> <a id="33062" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="33088" class="Keyword">open</a> <a id="33093" class="Keyword">import</a> <a id="33100" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="33162" class="Keyword">open</a> <a id="33167" class="Keyword">import</a> <a id="33174" href="structured-types.html" class="Module">structured-types</a>
<a id="33191" class="Keyword">open</a> <a id="33196" class="Keyword">import</a> <a id="33203" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="33238" class="Keyword">open</a> <a id="33243" class="Keyword">import</a> <a id="33250" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="33294" class="Keyword">open</a> <a id="33299" class="Keyword">import</a> <a id="33306" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="33370" class="Keyword">open</a> <a id="33375" class="Keyword">import</a> <a id="33382" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="33421" class="Keyword">open</a> <a id="33426" class="Keyword">import</a> <a id="33433" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="33479" class="Keyword">open</a> <a id="33484" class="Keyword">import</a> <a id="33491" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="33515" class="Keyword">open</a> <a id="33520" class="Keyword">import</a> <a id="33527" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="33596" class="Keyword">open</a> <a id="33601" class="Keyword">import</a> <a id="33608" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="33653" class="Keyword">open</a> <a id="33658" class="Keyword">import</a> <a id="33665" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33699" class="Keyword">open</a> <a id="33704" class="Keyword">import</a> <a id="33711" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33772" class="Keyword">open</a> <a id="33777" class="Keyword">import</a> <a id="33784" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33829" class="Keyword">open</a> <a id="33834" class="Keyword">import</a> <a id="33841" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="33879" class="Keyword">open</a> <a id="33884" class="Keyword">import</a> <a id="33891" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="33934" class="Keyword">open</a> <a id="33939" class="Keyword">import</a> <a id="33946" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="33982" class="Keyword">open</a> <a id="33987" class="Keyword">import</a> <a id="33994" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="34024" class="Keyword">open</a> <a id="34029" class="Keyword">import</a> <a id="34036" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="34067" class="Keyword">open</a> <a id="34072" class="Keyword">import</a> <a id="34079" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="34138" class="Keyword">open</a> <a id="34143" class="Keyword">import</a> <a id="34150" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="34201" class="Keyword">open</a> <a id="34206" class="Keyword">import</a> <a id="34213" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="34264" class="Keyword">open</a> <a id="34269" class="Keyword">import</a> <a id="34276" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="34331" class="Keyword">open</a> <a id="34336" class="Keyword">import</a> <a id="34343" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="34372" class="Keyword">open</a> <a id="34377" class="Keyword">import</a> <a id="34384" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="34412" class="Keyword">open</a> <a id="34417" class="Keyword">import</a> <a id="34424" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="34454" class="Keyword">open</a> <a id="34459" class="Keyword">import</a> <a id="34466" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="34500" class="Keyword">open</a> <a id="34505" class="Keyword">import</a> <a id="34512" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="34588" class="Keyword">open</a> <a id="34593" class="Keyword">import</a> <a id="34600" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="34626" class="Keyword">open</a> <a id="34631" class="Keyword">import</a> <a id="34638" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34676" class="Keyword">open</a> <a id="34681" class="Keyword">import</a> <a id="34688" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34734" class="Keyword">open</a> <a id="34739" class="Keyword">import</a> <a id="34746" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34783" class="Keyword">open</a> <a id="34788" class="Keyword">import</a> <a id="34795" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34835" class="Keyword">open</a> <a id="34840" class="Keyword">import</a> <a id="34847" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="34886" class="Keyword">open</a> <a id="34891" class="Keyword">import</a> <a id="34898" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="34931" class="Keyword">open</a> <a id="34936" class="Keyword">import</a> <a id="34943" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="34978" class="Keyword">open</a> <a id="34983" class="Keyword">import</a> <a id="34990" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="35035" class="Keyword">open</a> <a id="35040" class="Keyword">import</a> <a id="35047" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="35099" class="Keyword">open</a> <a id="35104" class="Keyword">import</a> <a id="35111" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="35164" class="Keyword">open</a> <a id="35169" class="Keyword">import</a> <a id="35176" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="35236" class="Keyword">open</a> <a id="35241" class="Keyword">import</a> <a id="35248" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="35296" class="Keyword">open</a> <a id="35301" class="Keyword">import</a> <a id="35308" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="35348" class="Keyword">open</a> <a id="35353" class="Keyword">import</a> <a id="35360" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="35407" class="Keyword">open</a> <a id="35412" class="Keyword">import</a> <a id="35419" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="35460" class="Keyword">open</a> <a id="35465" class="Keyword">import</a> <a id="35472" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="35510" class="Keyword">open</a> <a id="35515" class="Keyword">import</a> <a id="35522" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="35570" class="Keyword">open</a> <a id="35575" class="Keyword">import</a> <a id="35582" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35619" class="Keyword">open</a> <a id="35624" class="Keyword">import</a> <a id="35631" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35665" class="Keyword">open</a> <a id="35670" class="Keyword">import</a> <a id="35677" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35724" class="Keyword">open</a> <a id="35729" class="Keyword">import</a> <a id="35736" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35781" class="Keyword">open</a> <a id="35786" class="Keyword">import</a> <a id="35793" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35842" class="Keyword">open</a> <a id="35847" class="Keyword">import</a> <a id="35854" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="35931" class="Keyword">open</a> <a id="35936" class="Keyword">import</a> <a id="35943" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="35995" class="Keyword">open</a> <a id="36000" class="Keyword">import</a> <a id="36007" href="type-theories.html" class="Module">type-theories</a>
<a id="36021" class="Keyword">open</a> <a id="36026" class="Keyword">import</a> <a id="36033" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="36075" class="Keyword">open</a> <a id="36080" class="Keyword">import</a> <a id="36087" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="36125" class="Keyword">open</a> <a id="36130" class="Keyword">import</a> <a id="36137" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="36183" class="Keyword">open</a> <a id="36188" class="Keyword">import</a> <a id="36195" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="36242" class="Keyword">open</a> <a id="36247" class="Keyword">import</a> <a id="36254" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="36289" class="Keyword">open</a> <a id="36294" class="Keyword">import</a> <a id="36301" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="36379" class="Keyword">open</a> <a id="36384" class="Keyword">import</a> <a id="36391" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="36415" class="Keyword">open</a> <a id="36420" class="Keyword">import</a> <a id="36427" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="36480" class="Keyword">open</a> <a id="36485" class="Keyword">import</a> <a id="36492" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="36535" class="Keyword">open</a> <a id="36540" class="Keyword">import</a> <a id="36547" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="36587" class="Keyword">open</a> <a id="36592" class="Keyword">import</a> <a id="36599" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36638" class="Keyword">open</a> <a id="36643" class="Keyword">import</a> <a id="36650" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36684" class="Keyword">open</a> <a id="36689" class="Keyword">import</a> <a id="36696" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36744" class="Keyword">open</a> <a id="36749" class="Keyword">import</a> <a id="36756" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36807" class="Keyword">open</a> <a id="36812" class="Keyword">import</a> <a id="36819" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="36866" class="Keyword">open</a> <a id="36871" class="Keyword">import</a> <a id="36878" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="36930" class="Keyword">open</a> <a id="36935" class="Keyword">import</a> <a id="36942" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="36986" class="Keyword">open</a> <a id="36991" class="Keyword">import</a> <a id="36998" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="37038" class="Keyword">open</a> <a id="37043" class="Keyword">import</a> <a id="37050" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="37093" class="Keyword">open</a> <a id="37098" class="Keyword">import</a> <a id="37105" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="37157" class="Keyword">open</a> <a id="37162" class="Keyword">import</a> <a id="37169" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="37223" class="Keyword">open</a> <a id="37228" class="Keyword">import</a> <a id="37235" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="37283" class="Keyword">open</a> <a id="37288" class="Keyword">import</a> <a id="37295" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="37334" class="Keyword">open</a> <a id="37339" class="Keyword">import</a> <a id="37346" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="37379" class="Keyword">open</a> <a id="37384" class="Keyword">import</a> <a id="37391" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="37421" class="Keyword">open</a> <a id="37426" class="Keyword">import</a> <a id="37433" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="37484" class="Keyword">open</a> <a id="37489" class="Keyword">import</a> <a id="37496" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="37537" class="Keyword">open</a> <a id="37542" class="Keyword">import</a> <a id="37549" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="37586" class="Keyword">open</a> <a id="37591" class="Keyword">import</a> <a id="37598" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="37657" class="Keyword">open</a> <a id="37662" class="Keyword">import</a> <a id="37669" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37724" class="Keyword">open</a> <a id="37729" class="Keyword">import</a> <a id="37736" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37792" class="Keyword">open</a> <a id="37797" class="Keyword">import</a> <a id="37804" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="37851" class="Keyword">open</a> <a id="37856" class="Keyword">import</a> <a id="37863" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="37906" class="Keyword">open</a> <a id="37911" class="Keyword">import</a> <a id="37918" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="37963" class="Keyword">open</a> <a id="37968" class="Keyword">import</a> <a id="37975" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="38024" class="Keyword">open</a> <a id="38029" class="Keyword">import</a> <a id="38036" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="38087" class="Keyword">open</a> <a id="38092" class="Keyword">import</a> <a id="38099" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="38143" class="Keyword">open</a> <a id="38148" class="Keyword">import</a> <a id="38155" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="38233" class="Keyword">open</a> <a id="38238" class="Keyword">import</a> <a id="38245" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="38285" class="Keyword">open</a> <a id="38290" class="Keyword">import</a> <a id="38297" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="38354" class="Keyword">open</a> <a id="38359" class="Keyword">import</a> <a id="38366" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="38401" class="Keyword">open</a> <a id="38406" class="Keyword">import</a> <a id="38413" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="38459" class="Keyword">open</a> <a id="38464" class="Keyword">import</a> <a id="38471" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="38526" class="Keyword">open</a> <a id="38531" class="Keyword">import</a> <a id="38538" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="38581" class="Keyword">open</a> <a id="38586" class="Keyword">import</a> <a id="38593" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38638" class="Keyword">open</a> <a id="38643" class="Keyword">import</a> <a id="38650" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38709" class="Keyword">open</a> <a id="38714" class="Keyword">import</a> <a id="38721" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38758" class="Keyword">open</a> <a id="38763" class="Keyword">import</a> <a id="38770" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38812" class="Keyword">open</a> <a id="38817" class="Keyword">import</a> <a id="38824" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="38865" class="Keyword">open</a> <a id="38870" class="Keyword">import</a> <a id="38877" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="38916" class="Keyword">open</a> <a id="38921" class="Keyword">import</a> <a id="38928" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="38966" class="Keyword">open</a> <a id="38971" class="Keyword">import</a> <a id="38978" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="39030" class="Keyword">open</a> <a id="39035" class="Keyword">import</a> <a id="39042" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="39087" class="Keyword">open</a> <a id="39092" class="Keyword">import</a> <a id="39099" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="39138" class="Keyword">open</a> <a id="39143" class="Keyword">import</a> <a id="39150" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="39187" class="Keyword">open</a> <a id="39192" class="Keyword">import</a> <a id="39199" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="39248" class="Keyword">open</a> <a id="39253" class="Keyword">import</a> <a id="39260" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="39299" class="Keyword">open</a> <a id="39304" class="Keyword">import</a> <a id="39311" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="39349" class="Keyword">open</a> <a id="39354" class="Keyword">import</a> <a id="39361" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="39416" class="Keyword">open</a> <a id="39421" class="Keyword">import</a> <a id="39428" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="39467" class="Keyword">open</a> <a id="39472" class="Keyword">import</a> <a id="39479" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="39527" class="Keyword">open</a> <a id="39532" class="Keyword">import</a> <a id="39539" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="39586" class="Keyword">open</a> <a id="39591" class="Keyword">import</a> <a id="39598" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39636" class="Keyword">open</a> <a id="39641" class="Keyword">import</a> <a id="39648" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="39678" class="Keyword">open</a> <a id="39683" class="Keyword">import</a> <a id="39690" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39747" class="Keyword">open</a> <a id="39752" class="Keyword">import</a> <a id="39759" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39813" class="Keyword">open</a> <a id="39818" class="Keyword">import</a> <a id="39825" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="39855" class="Keyword">open</a> <a id="39860" class="Keyword">import</a> <a id="39867" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="39916" class="Keyword">open</a> <a id="39921" class="Keyword">import</a> <a id="39928" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="39970" class="Keyword">open</a> <a id="39975" class="Keyword">import</a> <a id="39982" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="40016" class="Keyword">open</a> <a id="40021" class="Keyword">import</a> <a id="40028" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="40091" class="Keyword">open</a> <a id="40096" class="Keyword">import</a> <a id="40103" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="40146" class="Keyword">open</a> <a id="40151" class="Keyword">import</a> <a id="40158" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="40193" class="Keyword">open</a> <a id="40198" class="Keyword">import</a> <a id="40205" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="40240" class="Keyword">open</a> <a id="40245" class="Keyword">import</a> <a id="40252" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="40292" class="Keyword">open</a> <a id="40297" class="Keyword">import</a> <a id="40304" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="40349" class="Keyword">open</a> <a id="40354" class="Keyword">import</a> <a id="40361" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="40402" class="Keyword">open</a> <a id="40407" class="Keyword">import</a> <a id="40414" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="40468" class="Keyword">open</a> <a id="40473" class="Keyword">import</a> <a id="40480" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="40530" class="Keyword">open</a> <a id="40535" class="Keyword">import</a> <a id="40542" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="40589" class="Keyword">open</a> <a id="40594" class="Keyword">import</a> <a id="40601" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40639" class="Keyword">open</a> <a id="40644" class="Keyword">import</a> <a id="40651" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40700" class="Keyword">open</a> <a id="40705" class="Keyword">import</a> <a id="40712" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40759" class="Keyword">open</a> <a id="40764" class="Keyword">import</a> <a id="40771" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40834" class="Keyword">open</a> <a id="40839" class="Keyword">import</a> <a id="40846" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="40878" class="Keyword">open</a> <a id="40883" class="Keyword">import</a> <a id="40890" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="40943" class="Keyword">open</a> <a id="40948" class="Keyword">import</a> <a id="40955" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="41001" class="Keyword">open</a> <a id="41006" class="Keyword">import</a> <a id="41013" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="41059" class="Keyword">open</a> <a id="41064" class="Keyword">import</a> <a id="41071" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="41111" class="Keyword">open</a> <a id="41116" class="Keyword">import</a> <a id="41123" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="41170" class="Keyword">open</a> <a id="41175" class="Keyword">import</a> <a id="41182" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="41230" class="Keyword">open</a> <a id="41235" class="Keyword">import</a> <a id="41242" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="41282" class="Keyword">open</a> <a id="41287" class="Keyword">import</a> <a id="41294" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="41339" class="Keyword">open</a> <a id="41344" class="Keyword">import</a> <a id="41351" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="41416" class="Keyword">open</a> <a id="41421" class="Keyword">import</a> <a id="41428" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="41473" class="Keyword">open</a> <a id="41478" class="Keyword">import</a> <a id="41485" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="41532" class="Keyword">open</a> <a id="41537" class="Keyword">import</a> <a id="41544" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="41597" class="Keyword">open</a> <a id="41602" class="Keyword">import</a> <a id="41609" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>