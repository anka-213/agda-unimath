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
<a id="13259" class="Keyword">open</a> <a id="13264" class="Keyword">import</a> <a id="13271" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13305" class="Keyword">open</a> <a id="13310" class="Keyword">import</a> <a id="13317" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="13346" class="Keyword">open</a> <a id="13351" class="Keyword">import</a> <a id="13358" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13381" class="Keyword">open</a> <a id="13386" class="Keyword">import</a> <a id="13393" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13420" class="Keyword">open</a> <a id="13425" class="Keyword">import</a> <a id="13432" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13460" class="Keyword">open</a> <a id="13465" class="Keyword">import</a> <a id="13472" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13509" class="Keyword">open</a> <a id="13514" class="Keyword">import</a> <a id="13521" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13569" class="Keyword">open</a> <a id="13574" class="Keyword">import</a> <a id="13581" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13621" class="Keyword">open</a> <a id="13626" class="Keyword">import</a> <a id="13633" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13655" class="Keyword">open</a> <a id="13660" class="Keyword">import</a> <a id="13667" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13690" class="Keyword">open</a> <a id="13695" class="Keyword">import</a> <a id="13702" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13727" class="Keyword">open</a> <a id="13732" class="Keyword">import</a> <a id="13739" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13784" class="Keyword">open</a> <a id="13789" class="Keyword">import</a> <a id="13796" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13840" class="Keyword">open</a> <a id="13845" class="Keyword">import</a> <a id="13852" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13888" class="Keyword">open</a> <a id="13893" class="Keyword">import</a> <a id="13900" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13945" class="Keyword">open</a> <a id="13950" class="Keyword">import</a> <a id="13957" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13998" class="Keyword">open</a> <a id="14003" class="Keyword">import</a> <a id="14010" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14045" class="Keyword">open</a> <a id="14050" class="Keyword">import</a> <a id="14057" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14089" class="Keyword">open</a> <a id="14094" class="Keyword">import</a> <a id="14101" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14132" class="Keyword">open</a> <a id="14137" class="Keyword">import</a> <a id="14144" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14177" class="Keyword">open</a> <a id="14182" class="Keyword">import</a> <a id="14189" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14222" class="Keyword">open</a> <a id="14227" class="Keyword">import</a> <a id="14234" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14264" class="Keyword">open</a> <a id="14269" class="Keyword">import</a> <a id="14276" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14300" class="Keyword">open</a> <a id="14305" class="Keyword">import</a> <a id="14312" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14350" class="Keyword">open</a> <a id="14355" class="Keyword">import</a> <a id="14362" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14393" class="Keyword">open</a> <a id="14398" class="Keyword">import</a> <a id="14405" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14430" class="Keyword">open</a> <a id="14435" class="Keyword">import</a> <a id="14442" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14470" class="Keyword">open</a> <a id="14475" class="Keyword">import</a> <a id="14482" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14506" class="Keyword">open</a> <a id="14511" class="Keyword">import</a> <a id="14518" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14544" class="Keyword">open</a> <a id="14549" class="Keyword">import</a> <a id="14556" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14591" class="Keyword">open</a> <a id="14596" class="Keyword">import</a> <a id="14603" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14624" class="Keyword">open</a> <a id="14629" class="Keyword">import</a> <a id="14636" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14685" class="Keyword">open</a> <a id="14690" class="Keyword">import</a> <a id="14697" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14738" class="Keyword">open</a> <a id="14743" class="Keyword">import</a> <a id="14750" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14800" class="Keyword">open</a> <a id="14805" class="Keyword">import</a> <a id="14812" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14858" class="Keyword">open</a> <a id="14863" class="Keyword">import</a> <a id="14870" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14910" class="Keyword">open</a> <a id="14915" class="Keyword">import</a> <a id="14922" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14972" class="Keyword">open</a> <a id="14977" class="Keyword">import</a> <a id="14984" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15023" class="Keyword">open</a> <a id="15028" class="Keyword">import</a> <a id="15035" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15075" class="Keyword">open</a> <a id="15080" class="Keyword">import</a> <a id="15087" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15120" class="Keyword">open</a> <a id="15125" class="Keyword">import</a> <a id="15132" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15181" class="Keyword">open</a> <a id="15186" class="Keyword">import</a> <a id="15193" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15218" class="Keyword">open</a> <a id="15223" class="Keyword">import</a> <a id="15230" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15268" class="Keyword">open</a> <a id="15273" class="Keyword">import</a> <a id="15280" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15302" class="Keyword">open</a> <a id="15307" class="Keyword">import</a> <a id="15314" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15342" class="Keyword">open</a> <a id="15347" class="Keyword">import</a> <a id="15354" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15390" class="Keyword">open</a> <a id="15395" class="Keyword">import</a> <a id="15402" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15428" class="Keyword">open</a> <a id="15433" class="Keyword">import</a> <a id="15440" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15458" class="Keyword">open</a> <a id="15463" class="Keyword">import</a> <a id="15470" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15505" class="Keyword">open</a> <a id="15510" class="Keyword">import</a> <a id="15517" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15552" class="Keyword">open</a> <a id="15557" class="Keyword">import</a> <a id="15564" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15591" class="Keyword">open</a> <a id="15596" class="Keyword">import</a> <a id="15603" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15659" class="Keyword">open</a> <a id="15664" class="Keyword">import</a> <a id="15671" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15700" class="Keyword">open</a> <a id="15705" class="Keyword">import</a> <a id="15712" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15742" class="Keyword">open</a> <a id="15747" class="Keyword">import</a> <a id="15754" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15781" class="Keyword">open</a> <a id="15786" class="Keyword">import</a> <a id="15793" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15819" class="Keyword">open</a> <a id="15824" class="Keyword">import</a> <a id="15831" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15858" class="Keyword">open</a> <a id="15863" class="Keyword">import</a> <a id="15870" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15894" class="Keyword">open</a> <a id="15899" class="Keyword">import</a> <a id="15906" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15929" class="Keyword">open</a> <a id="15934" class="Keyword">import</a> <a id="15941" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15968" class="Keyword">open</a> <a id="15973" class="Keyword">import</a> <a id="15980" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16012" class="Keyword">open</a> <a id="16017" class="Keyword">import</a> <a id="16024" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16059" class="Keyword">open</a> <a id="16064" class="Keyword">import</a> <a id="16071" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16102" class="Keyword">open</a> <a id="16107" class="Keyword">import</a> <a id="16114" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16147" class="Keyword">open</a> <a id="16152" class="Keyword">import</a> <a id="16159" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16193" class="Keyword">open</a> <a id="16198" class="Keyword">import</a> <a id="16205" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16245" class="Keyword">open</a> <a id="16250" class="Keyword">import</a> <a id="16257" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16288" class="Keyword">open</a> <a id="16293" class="Keyword">import</a> <a id="16300" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16332" class="Keyword">open</a> <a id="16337" class="Keyword">import</a> <a id="16344" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16375" class="Keyword">open</a> <a id="16380" class="Keyword">import</a> <a id="16387" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16404" class="Keyword">open</a> <a id="16409" class="Keyword">import</a> <a id="16416" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16441" class="Keyword">open</a> <a id="16446" class="Keyword">import</a> <a id="16453" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16482" class="Keyword">open</a> <a id="16487" class="Keyword">import</a> <a id="16494" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16519" class="Keyword">open</a> <a id="16524" class="Keyword">import</a> <a id="16531" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16552" class="Keyword">open</a> <a id="16557" class="Keyword">import</a> <a id="16564" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16588" class="Keyword">open</a> <a id="16593" class="Keyword">import</a> <a id="16600" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16620" class="Keyword">open</a> <a id="16625" class="Keyword">import</a> <a id="16632" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16666" class="Keyword">open</a> <a id="16671" class="Keyword">import</a> <a id="16678" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16716" class="Keyword">open</a> <a id="16721" class="Keyword">import</a> <a id="16728" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16756" class="Keyword">open</a> <a id="16761" class="Keyword">import</a> <a id="16768" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16792" class="Keyword">open</a> <a id="16797" class="Keyword">import</a> <a id="16804" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16831" class="Keyword">open</a> <a id="16836" class="Keyword">import</a> <a id="16843" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16878" class="Keyword">open</a> <a id="16883" class="Keyword">import</a> <a id="16890" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16911" class="Keyword">open</a> <a id="16916" class="Keyword">import</a> <a id="16923" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16959" class="Keyword">open</a> <a id="16964" class="Keyword">import</a> <a id="16971" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17016" class="Keyword">open</a> <a id="17021" class="Keyword">import</a> <a id="17028" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17074" class="Keyword">open</a> <a id="17079" class="Keyword">import</a> <a id="17086" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17126" class="Keyword">open</a> <a id="17131" class="Keyword">import</a> <a id="17138" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17168" class="Keyword">open</a> <a id="17173" class="Keyword">import</a> <a id="17180" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17214" class="Keyword">open</a> <a id="17219" class="Keyword">import</a> <a id="17226" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17263" class="Keyword">open</a> <a id="17268" class="Keyword">import</a> <a id="17275" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17299" class="Keyword">open</a> <a id="17304" class="Keyword">import</a> <a id="17311" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17332" class="Keyword">open</a> <a id="17337" class="Keyword">import</a> <a id="17344" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17379" class="Keyword">open</a> <a id="17384" class="Keyword">import</a> <a id="17391" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17428" class="Keyword">open</a> <a id="17433" class="Keyword">import</a> <a id="17440" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17489" class="Keyword">open</a> <a id="17494" class="Keyword">import</a> <a id="17501" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17534" class="Keyword">open</a> <a id="17539" class="Keyword">import</a> <a id="17546" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17569" class="Keyword">open</a> <a id="17574" class="Keyword">import</a> <a id="17581" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17604" class="Keyword">open</a> <a id="17609" class="Keyword">import</a> <a id="17616" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17639" class="Keyword">open</a> <a id="17644" class="Keyword">import</a> <a id="17651" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17679" class="Keyword">open</a> <a id="17684" class="Keyword">import</a> <a id="17691" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17711" class="Keyword">open</a> <a id="17716" class="Keyword">import</a> <a id="17723" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17744" class="Keyword">open</a> <a id="17749" class="Keyword">import</a> <a id="17756" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17787" class="Keyword">open</a> <a id="17792" class="Keyword">import</a> <a id="17799" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17826" class="Keyword">open</a> <a id="17831" class="Keyword">import</a> <a id="17838" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17854" class="Keyword">open</a> <a id="17859" class="Keyword">import</a> <a id="17866" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17897" class="Keyword">open</a> <a id="17902" class="Keyword">import</a> <a id="17909" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17926" class="Keyword">open</a> <a id="17931" class="Keyword">import</a> <a id="17938" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17960" class="Keyword">open</a> <a id="17965" class="Keyword">import</a> <a id="17972" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17999" class="Keyword">open</a> <a id="18004" class="Keyword">import</a> <a id="18011" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18034" class="Keyword">open</a> <a id="18039" class="Keyword">import</a> <a id="18046" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18073" class="Keyword">open</a> <a id="18078" class="Keyword">import</a> <a id="18085" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18118" class="Keyword">open</a> <a id="18123" class="Keyword">import</a> <a id="18130" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18170" class="Keyword">open</a> <a id="18175" class="Keyword">import</a> <a id="18182" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18203" class="Keyword">open</a> <a id="18208" class="Keyword">import</a> <a id="18215" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18244" class="Keyword">open</a> <a id="18249" class="Keyword">import</a> <a id="18256" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18294" class="Keyword">open</a> <a id="18299" class="Keyword">import</a> <a id="18306" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18326" class="Keyword">open</a> <a id="18331" class="Keyword">import</a> <a id="18338" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18362" class="Keyword">open</a> <a id="18367" class="Keyword">import</a> <a id="18374" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18401" class="Keyword">open</a> <a id="18406" class="Keyword">import</a> <a id="18413" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18445" class="Keyword">open</a> <a id="18450" class="Keyword">import</a> <a id="18457" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18487" class="Keyword">open</a> <a id="18492" class="Keyword">import</a> <a id="18499" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18525" class="Keyword">open</a> <a id="18530" class="Keyword">import</a> <a id="18537" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18564" class="Keyword">open</a> <a id="18569" class="Keyword">import</a> <a id="18576" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="18613" class="Keyword">open</a> <a id="18618" class="Keyword">import</a> <a id="18625" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18654" class="Keyword">open</a> <a id="18659" class="Keyword">import</a> <a id="18666" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18689" class="Keyword">open</a> <a id="18694" class="Keyword">import</a> <a id="18701" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18752" class="Keyword">open</a> <a id="18757" class="Keyword">import</a> <a id="18764" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18807" class="Keyword">open</a> <a id="18812" class="Keyword">import</a> <a id="18819" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="18871" class="Keyword">open</a> <a id="18876" class="Keyword">import</a> <a id="18883" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18931" class="Keyword">open</a> <a id="18936" class="Keyword">import</a> <a id="18943" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18981" class="Keyword">open</a> <a id="18986" class="Keyword">import</a> <a id="18993" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19030" class="Keyword">open</a> <a id="19035" class="Keyword">import</a> <a id="19042" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19088" class="Keyword">open</a> <a id="19093" class="Keyword">import</a> <a id="19100" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19117" class="Keyword">open</a> <a id="19122" class="Keyword">import</a> <a id="19129" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19157" class="Keyword">open</a> <a id="19162" class="Keyword">import</a> <a id="19169" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19197" class="Keyword">open</a> <a id="19202" class="Keyword">import</a> <a id="19209" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19245" class="Keyword">open</a> <a id="19250" class="Keyword">import</a> <a id="19257" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19295" class="Keyword">open</a> <a id="19300" class="Keyword">import</a> <a id="19307" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19340" class="Keyword">open</a> <a id="19345" class="Keyword">import</a> <a id="19352" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19373" class="Keyword">open</a> <a id="19378" class="Keyword">import</a> <a id="19385" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19421" class="Keyword">open</a> <a id="19426" class="Keyword">import</a> <a id="19433" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19487" class="Keyword">open</a> <a id="19492" class="Keyword">import</a> <a id="19499" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19521" class="Keyword">open</a> <a id="19526" class="Keyword">import</a> <a id="19533" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19568" class="Keyword">open</a> <a id="19573" class="Keyword">import</a> <a id="19580" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19610" class="Keyword">open</a> <a id="19615" class="Keyword">import</a> <a id="19622" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19661" class="Keyword">open</a> <a id="19666" class="Keyword">import</a> <a id="19673" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19727" class="Keyword">open</a> <a id="19732" class="Keyword">import</a> <a id="19739" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19785" class="Keyword">open</a> <a id="19790" class="Keyword">import</a> <a id="19797" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19848" class="Keyword">open</a> <a id="19853" class="Keyword">import</a> <a id="19860" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19901" class="Keyword">open</a> <a id="19906" class="Keyword">import</a> <a id="19913" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19958" class="Keyword">open</a> <a id="19963" class="Keyword">import</a> <a id="19970" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20015" class="Keyword">open</a> <a id="20020" class="Keyword">import</a> <a id="20027" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20063" class="Keyword">open</a> <a id="20068" class="Keyword">import</a> <a id="20075" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20111" class="Keyword">open</a> <a id="20116" class="Keyword">import</a> <a id="20123" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20188" class="Keyword">open</a> <a id="20193" class="Keyword">import</a> <a id="20200" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20255" class="Keyword">open</a> <a id="20260" class="Keyword">import</a> <a id="20267" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20307" class="Keyword">open</a> <a id="20312" class="Keyword">import</a> <a id="20319" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20363" class="Keyword">open</a> <a id="20368" class="Keyword">import</a> <a id="20375" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20420" class="Keyword">open</a> <a id="20425" class="Keyword">import</a> <a id="20432" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20473" class="Keyword">open</a> <a id="20478" class="Keyword">import</a> <a id="20485" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20525" class="Keyword">open</a> <a id="20530" class="Keyword">import</a> <a id="20537" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20564" class="Keyword">open</a> <a id="20569" class="Keyword">import</a> <a id="20576" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20612" class="Keyword">open</a> <a id="20617" class="Keyword">import</a> <a id="20624" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20651" class="Keyword">open</a> <a id="20656" class="Keyword">import</a> <a id="20663" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20700" class="Keyword">open</a> <a id="20705" class="Keyword">import</a> <a id="20712" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20740" class="Keyword">open</a> <a id="20745" class="Keyword">import</a> <a id="20752" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20771" class="Keyword">open</a> <a id="20776" class="Keyword">import</a> <a id="20783" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20823" class="Keyword">open</a> <a id="20828" class="Keyword">import</a> <a id="20835" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20867" class="Keyword">open</a> <a id="20872" class="Keyword">import</a> <a id="20879" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20927" class="Keyword">open</a> <a id="20932" class="Keyword">import</a> <a id="20939" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20962" class="Keyword">open</a> <a id="20967" class="Keyword">import</a> <a id="20974" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20998" class="Keyword">open</a> <a id="21003" class="Keyword">import</a> <a id="21010" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21050" class="Keyword">open</a> <a id="21055" class="Keyword">import</a> <a id="21062" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="21105" class="Keyword">open</a> <a id="21110" class="Keyword">import</a> <a id="21117" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21151" class="Keyword">open</a> <a id="21156" class="Keyword">import</a> <a id="21163" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21195" class="Keyword">open</a> <a id="21200" class="Keyword">import</a> <a id="21207" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21237" class="Keyword">open</a> <a id="21242" class="Keyword">import</a> <a id="21249" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21283" class="Keyword">open</a> <a id="21288" class="Keyword">import</a> <a id="21295" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21330" class="Keyword">open</a> <a id="21335" class="Keyword">import</a> <a id="21342" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21379" class="Keyword">open</a> <a id="21384" class="Keyword">import</a> <a id="21391" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21418" class="Keyword">open</a> <a id="21423" class="Keyword">import</a> <a id="21430" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21458" class="Keyword">open</a> <a id="21463" class="Keyword">import</a> <a id="21470" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21519" class="Keyword">open</a> <a id="21524" class="Keyword">import</a> <a id="21531" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21577" class="Keyword">open</a> <a id="21582" class="Keyword">import</a> <a id="21589" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21629" class="Keyword">open</a> <a id="21634" class="Keyword">import</a> <a id="21641" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21679" class="Keyword">open</a> <a id="21684" class="Keyword">import</a> <a id="21691" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21720" class="Keyword">open</a> <a id="21725" class="Keyword">import</a> <a id="21732" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21762" class="Keyword">open</a> <a id="21767" class="Keyword">import</a> <a id="21774" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21805" class="Keyword">open</a> <a id="21810" class="Keyword">import</a> <a id="21817" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21857" class="Keyword">open</a> <a id="21862" class="Keyword">import</a> <a id="21869" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21895" class="Keyword">open</a> <a id="21900" class="Keyword">import</a> <a id="21907" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21962" class="Keyword">open</a> <a id="21967" class="Keyword">import</a> <a id="21974" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="22025" class="Keyword">open</a> <a id="22030" class="Keyword">import</a> <a id="22037" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="22082" class="Keyword">open</a> <a id="22087" class="Keyword">import</a> <a id="22094" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22148" class="Keyword">open</a> <a id="22153" class="Keyword">import</a> <a id="22160" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22187" class="Keyword">open</a> <a id="22192" class="Keyword">import</a> <a id="22199" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22232" class="Keyword">open</a> <a id="22237" class="Keyword">import</a> <a id="22244" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22275" class="Keyword">open</a> <a id="22280" class="Keyword">import</a> <a id="22287" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22324" class="Keyword">open</a> <a id="22329" class="Keyword">import</a> <a id="22336" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22361" class="Keyword">open</a> <a id="22366" class="Keyword">import</a> <a id="22373" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22405" class="Keyword">open</a> <a id="22410" class="Keyword">import</a> <a id="22417" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22452" class="Keyword">open</a> <a id="22457" class="Keyword">import</a> <a id="22464" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22493" class="Keyword">open</a> <a id="22498" class="Keyword">import</a> <a id="22505" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22531" class="Keyword">open</a> <a id="22536" class="Keyword">import</a> <a id="22543" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22571" class="Keyword">open</a> <a id="22576" class="Keyword">import</a> <a id="22583" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22608" class="Keyword">open</a> <a id="22613" class="Keyword">import</a> <a id="22620" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22641" class="Keyword">open</a> <a id="22646" class="Keyword">import</a> <a id="22653" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22689" class="Keyword">open</a> <a id="22694" class="Keyword">import</a> <a id="22701" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22744" class="Keyword">open</a> <a id="22749" class="Keyword">import</a> <a id="22756" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22781" class="Keyword">open</a> <a id="22786" class="Keyword">import</a> <a id="22793" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22824" class="Keyword">open</a> <a id="22829" class="Keyword">import</a> <a id="22836" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22868" class="Keyword">open</a> <a id="22873" class="Keyword">import</a> <a id="22880" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22914" class="Keyword">open</a> <a id="22919" class="Keyword">import</a> <a id="22926" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22982" class="Keyword">open</a> <a id="22987" class="Keyword">import</a> <a id="22994" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="23047" class="Keyword">open</a> <a id="23052" class="Keyword">import</a> <a id="23059" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="23086" class="Keyword">open</a> <a id="23091" class="Keyword">import</a> <a id="23098" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23143" class="Keyword">open</a> <a id="23148" class="Keyword">import</a> <a id="23155" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23217" class="Keyword">open</a> <a id="23222" class="Keyword">import</a> <a id="23229" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23242" class="Keyword">open</a> <a id="23247" class="Keyword">import</a> <a id="23254" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23294" class="Keyword">open</a> <a id="23299" class="Keyword">import</a> <a id="23306" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23350" class="Keyword">open</a> <a id="23355" class="Keyword">import</a> <a id="23362" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23401" class="Keyword">open</a> <a id="23406" class="Keyword">import</a> <a id="23413" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23455" class="Keyword">open</a> <a id="23460" class="Keyword">import</a> <a id="23467" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23507" class="Keyword">open</a> <a id="23512" class="Keyword">import</a> <a id="23519" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23560" class="Keyword">open</a> <a id="23565" class="Keyword">import</a> <a id="23572" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23610" class="Keyword">open</a> <a id="23615" class="Keyword">import</a> <a id="23622" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23685" class="Keyword">open</a> <a id="23690" class="Keyword">import</a> <a id="23697" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23726" class="Keyword">open</a> <a id="23731" class="Keyword">import</a> <a id="23738" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23783" class="Keyword">open</a> <a id="23788" class="Keyword">import</a> <a id="23795" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23837" class="Keyword">open</a> <a id="23842" class="Keyword">import</a> <a id="23849" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23893" class="Keyword">open</a> <a id="23898" class="Keyword">import</a> <a id="23905" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23954" class="Keyword">open</a> <a id="23959" class="Keyword">import</a> <a id="23966" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="24016" class="Keyword">open</a> <a id="24021" class="Keyword">import</a> <a id="24028" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="24055" class="Keyword">open</a> <a id="24060" class="Keyword">import</a> <a id="24067" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="24092" class="Keyword">open</a> <a id="24097" class="Keyword">import</a> <a id="24104" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24145" class="Keyword">open</a> <a id="24150" class="Keyword">import</a> <a id="24157" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24180" class="Keyword">open</a> <a id="24185" class="Keyword">import</a> <a id="24192" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24241" class="Keyword">open</a> <a id="24246" class="Keyword">import</a> <a id="24253" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24292" class="Keyword">open</a> <a id="24297" class="Keyword">import</a> <a id="24304" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24345" class="Keyword">open</a> <a id="24350" class="Keyword">import</a> <a id="24357" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24401" class="Keyword">open</a> <a id="24406" class="Keyword">import</a> <a id="24413" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24450" class="Keyword">open</a> <a id="24455" class="Keyword">import</a> <a id="24462" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24484" class="Keyword">open</a> <a id="24489" class="Keyword">import</a> <a id="24496" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24526" class="Keyword">open</a> <a id="24531" class="Keyword">import</a> <a id="24538" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24577" class="Keyword">open</a> <a id="24582" class="Keyword">import</a> <a id="24589" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24627" class="Keyword">open</a> <a id="24632" class="Keyword">import</a> <a id="24639" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24697" class="Keyword">open</a> <a id="24702" class="Keyword">import</a> <a id="24709" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24774" class="Keyword">open</a> <a id="24779" class="Keyword">import</a> <a id="24786" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24817" class="Keyword">open</a> <a id="24822" class="Keyword">import</a> <a id="24829" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24856" class="Keyword">open</a> <a id="24861" class="Keyword">import</a> <a id="24868" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24926" class="Keyword">open</a> <a id="24931" class="Keyword">import</a> <a id="24938" href="group-theory.html" class="Module">group-theory</a>
<a id="24951" class="Keyword">open</a> <a id="24956" class="Keyword">import</a> <a id="24963" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24991" class="Keyword">open</a> <a id="24996" class="Keyword">import</a> <a id="25003" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="25054" class="Keyword">open</a> <a id="25059" class="Keyword">import</a> <a id="25066" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="25099" class="Keyword">open</a> <a id="25104" class="Keyword">import</a> <a id="25111" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="25158" class="Keyword">open</a> <a id="25163" class="Keyword">import</a> <a id="25170" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="25209" class="Keyword">open</a> <a id="25214" class="Keyword">import</a> <a id="25221" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25261" class="Keyword">open</a> <a id="25266" class="Keyword">import</a> <a id="25273" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25316" class="Keyword">open</a> <a id="25321" class="Keyword">import</a> <a id="25328" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25360" class="Keyword">open</a> <a id="25365" class="Keyword">import</a> <a id="25372" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25408" class="Keyword">open</a> <a id="25413" class="Keyword">import</a> <a id="25420" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25449" class="Keyword">open</a> <a id="25454" class="Keyword">import</a> <a id="25461" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25489" class="Keyword">open</a> <a id="25494" class="Keyword">import</a> <a id="25501" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25534" class="Keyword">open</a> <a id="25539" class="Keyword">import</a> <a id="25546" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25582" class="Keyword">open</a> <a id="25587" class="Keyword">import</a> <a id="25594" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25623" class="Keyword">open</a> <a id="25628" class="Keyword">import</a> <a id="25635" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25660" class="Keyword">open</a> <a id="25665" class="Keyword">import</a> <a id="25672" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25734" class="Keyword">open</a> <a id="25739" class="Keyword">import</a> <a id="25746" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25777" class="Keyword">open</a> <a id="25782" class="Keyword">import</a> <a id="25789" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25836" class="Keyword">open</a> <a id="25841" class="Keyword">import</a> <a id="25848" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25881" class="Keyword">open</a> <a id="25886" class="Keyword">import</a> <a id="25893" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="25942" class="Keyword">open</a> <a id="25947" class="Keyword">import</a> <a id="25954" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25994" class="Keyword">open</a> <a id="25999" class="Keyword">import</a> <a id="26006" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="26043" class="Keyword">open</a> <a id="26048" class="Keyword">import</a> <a id="26055" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="26102" class="Keyword">open</a> <a id="26107" class="Keyword">import</a> <a id="26114" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="26155" class="Keyword">open</a> <a id="26160" class="Keyword">import</a> <a id="26167" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="26206" class="Keyword">open</a> <a id="26211" class="Keyword">import</a> <a id="26218" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="26250" class="Keyword">open</a> <a id="26255" class="Keyword">import</a> <a id="26262" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="26289" class="Keyword">open</a> <a id="26294" class="Keyword">import</a> <a id="26301" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26321" class="Keyword">open</a> <a id="26326" class="Keyword">import</a> <a id="26333" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26367" class="Keyword">open</a> <a id="26372" class="Keyword">import</a> <a id="26379" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26406" class="Keyword">open</a> <a id="26411" class="Keyword">import</a> <a id="26418" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26460" class="Keyword">open</a> <a id="26465" class="Keyword">import</a> <a id="26472" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26522" class="Keyword">open</a> <a id="26527" class="Keyword">import</a> <a id="26534" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26581" class="Keyword">open</a> <a id="26586" class="Keyword">import</a> <a id="26593" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="26634" class="Keyword">open</a> <a id="26639" class="Keyword">import</a> <a id="26646" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26680" class="Keyword">open</a> <a id="26685" class="Keyword">import</a> <a id="26692" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="26733" class="Keyword">open</a> <a id="26738" class="Keyword">import</a> <a id="26745" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="26780" class="Keyword">open</a> <a id="26785" class="Keyword">import</a> <a id="26792" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="26830" class="Keyword">open</a> <a id="26835" class="Keyword">import</a> <a id="26842" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="26877" class="Keyword">open</a> <a id="26882" class="Keyword">import</a> <a id="26889" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26921" class="Keyword">open</a> <a id="26926" class="Keyword">import</a> <a id="26933" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="26974" class="Keyword">open</a> <a id="26979" class="Keyword">import</a> <a id="26986" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="27027" class="Keyword">open</a> <a id="27032" class="Keyword">import</a> <a id="27039" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="27079" class="Keyword">open</a> <a id="27084" class="Keyword">import</a> <a id="27091" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="27124" class="Keyword">open</a> <a id="27129" class="Keyword">import</a> <a id="27136" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="27173" class="Keyword">open</a> <a id="27178" class="Keyword">import</a> <a id="27185" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="27215" class="Keyword">open</a> <a id="27220" class="Keyword">import</a> <a id="27227" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="27248" class="Keyword">open</a> <a id="27253" class="Keyword">import</a> <a id="27260" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="27314" class="Keyword">open</a> <a id="27319" class="Keyword">import</a> <a id="27326" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27371" class="Keyword">open</a> <a id="27376" class="Keyword">import</a> <a id="27383" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27411" class="Keyword">open</a> <a id="27416" class="Keyword">import</a> <a id="27423" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27444" class="Keyword">open</a> <a id="27449" class="Keyword">import</a> <a id="27456" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27499" class="Keyword">open</a> <a id="27504" class="Keyword">import</a> <a id="27511" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27545" class="Keyword">open</a> <a id="27550" class="Keyword">import</a> <a id="27557" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27587" class="Keyword">open</a> <a id="27592" class="Keyword">import</a> <a id="27599" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="27645" class="Keyword">open</a> <a id="27650" class="Keyword">import</a> <a id="27657" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="27711" class="Keyword">open</a> <a id="27716" class="Keyword">import</a> <a id="27723" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="27766" class="Keyword">open</a> <a id="27771" class="Keyword">import</a> <a id="27778" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="27812" class="Keyword">open</a> <a id="27817" class="Keyword">import</a> <a id="27824" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="27865" class="Keyword">open</a> <a id="27870" class="Keyword">import</a> <a id="27877" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="27912" class="Keyword">open</a> <a id="27917" class="Keyword">import</a> <a id="27924" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="27966" class="Keyword">open</a> <a id="27971" class="Keyword">import</a> <a id="27978" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="28013" class="Keyword">open</a> <a id="28018" class="Keyword">import</a> <a id="28025" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="28064" class="Keyword">open</a> <a id="28069" class="Keyword">import</a> <a id="28076" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="28113" class="Keyword">open</a> <a id="28118" class="Keyword">import</a> <a id="28125" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="28172" class="Keyword">open</a> <a id="28177" class="Keyword">import</a> <a id="28184" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="28248" class="Keyword">open</a> <a id="28253" class="Keyword">import</a> <a id="28260" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="28305" class="Keyword">open</a> <a id="28310" class="Keyword">import</a> <a id="28317" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="28341" class="Keyword">open</a> <a id="28346" class="Keyword">import</a> <a id="28353" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="28378" class="Keyword">open</a> <a id="28383" class="Keyword">import</a> <a id="28390" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28433" class="Keyword">open</a> <a id="28438" class="Keyword">import</a> <a id="28445" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28476" class="Keyword">open</a> <a id="28481" class="Keyword">import</a> <a id="28488" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28542" class="Keyword">open</a> <a id="28547" class="Keyword">import</a> <a id="28554" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28577" class="Keyword">open</a> <a id="28582" class="Keyword">import</a> <a id="28589" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="28627" class="Keyword">open</a> <a id="28632" class="Keyword">import</a> <a id="28639" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="28678" class="Keyword">open</a> <a id="28683" class="Keyword">import</a> <a id="28690" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="28741" class="Keyword">open</a> <a id="28746" class="Keyword">import</a> <a id="28753" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="28790" class="Keyword">open</a> <a id="28795" class="Keyword">import</a> <a id="28802" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="28859" class="Keyword">open</a> <a id="28864" class="Keyword">import</a> <a id="28871" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="28919" class="Keyword">open</a> <a id="28924" class="Keyword">import</a> <a id="28931" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="28961" class="Keyword">open</a> <a id="28966" class="Keyword">import</a> <a id="28973" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="29010" class="Keyword">open</a> <a id="29015" class="Keyword">import</a> <a id="29022" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="29043" class="Keyword">open</a> <a id="29048" class="Keyword">import</a> <a id="29055" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="29102" class="Keyword">open</a> <a id="29107" class="Keyword">import</a> <a id="29114" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="29152" class="Keyword">open</a> <a id="29157" class="Keyword">import</a> <a id="29164" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="29258" class="Keyword">open</a> <a id="29263" class="Keyword">import</a> <a id="29270" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="29285" class="Keyword">open</a> <a id="29290" class="Keyword">import</a> <a id="29297" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="29330" class="Keyword">open</a> <a id="29335" class="Keyword">import</a> <a id="29342" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="29374" class="Keyword">open</a> <a id="29379" class="Keyword">import</a> <a id="29386" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29428" class="Keyword">open</a> <a id="29433" class="Keyword">import</a> <a id="29440" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29478" class="Keyword">open</a> <a id="29483" class="Keyword">import</a> <a id="29490" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29527" class="Keyword">open</a> <a id="29532" class="Keyword">import</a> <a id="29539" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29572" class="Keyword">open</a> <a id="29577" class="Keyword">import</a> <a id="29584" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="29608" class="Keyword">open</a> <a id="29613" class="Keyword">import</a> <a id="29620" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="29659" class="Keyword">open</a> <a id="29664" class="Keyword">import</a> <a id="29671" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="29717" class="Keyword">open</a> <a id="29722" class="Keyword">import</a> <a id="29729" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="29774" class="Keyword">open</a> <a id="29779" class="Keyword">import</a> <a id="29786" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="29824" class="Keyword">open</a> <a id="29829" class="Keyword">import</a> <a id="29836" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="29868" class="Keyword">open</a> <a id="29873" class="Keyword">import</a> <a id="29880" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="29933" class="Keyword">open</a> <a id="29938" class="Keyword">import</a> <a id="29945" href="order-theory.html" class="Module">order-theory</a>
<a id="29958" class="Keyword">open</a> <a id="29963" class="Keyword">import</a> <a id="29970" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="29997" class="Keyword">open</a> <a id="30002" class="Keyword">import</a> <a id="30009" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="30039" class="Keyword">open</a> <a id="30044" class="Keyword">import</a> <a id="30051" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="30084" class="Keyword">open</a> <a id="30089" class="Keyword">import</a> <a id="30096" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="30132" class="Keyword">open</a> <a id="30137" class="Keyword">import</a> <a id="30144" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="30179" class="Keyword">open</a> <a id="30184" class="Keyword">import</a> <a id="30191" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="30218" class="Keyword">open</a> <a id="30223" class="Keyword">import</a> <a id="30230" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="30260" class="Keyword">open</a> <a id="30265" class="Keyword">import</a> <a id="30272" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="30308" class="Keyword">open</a> <a id="30313" class="Keyword">import</a> <a id="30320" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="30362" class="Keyword">open</a> <a id="30367" class="Keyword">import</a> <a id="30374" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="30406" class="Keyword">open</a> <a id="30411" class="Keyword">import</a> <a id="30418" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30449" class="Keyword">open</a> <a id="30454" class="Keyword">import</a> <a id="30461" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30487" class="Keyword">open</a> <a id="30492" class="Keyword">import</a> <a id="30499" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30528" class="Keyword">open</a> <a id="30533" class="Keyword">import</a> <a id="30540" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30577" class="Keyword">open</a> <a id="30582" class="Keyword">import</a> <a id="30589" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="30629" class="Keyword">open</a> <a id="30634" class="Keyword">import</a> <a id="30641" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="30663" class="Keyword">open</a> <a id="30668" class="Keyword">import</a> <a id="30675" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="30710" class="Keyword">open</a> <a id="30715" class="Keyword">import</a> <a id="30722" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="30760" class="Keyword">open</a> <a id="30765" class="Keyword">import</a> <a id="30772" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="30811" class="Keyword">open</a> <a id="30816" class="Keyword">import</a> <a id="30823" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="30858" class="Keyword">open</a> <a id="30863" class="Keyword">import</a> <a id="30870" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="30905" class="Keyword">open</a> <a id="30910" class="Keyword">import</a> <a id="30917" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="30955" class="Keyword">open</a> <a id="30960" class="Keyword">import</a> <a id="30967" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="30998" class="Keyword">open</a> <a id="31003" class="Keyword">import</a> <a id="31010" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="31052" class="Keyword">open</a> <a id="31057" class="Keyword">import</a> <a id="31064" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="31109" class="Keyword">open</a> <a id="31114" class="Keyword">import</a> <a id="31121" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="31154" class="Keyword">open</a> <a id="31159" class="Keyword">import</a> <a id="31166" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="31186" class="Keyword">open</a> <a id="31191" class="Keyword">import</a> <a id="31198" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="31221" class="Keyword">open</a> <a id="31226" class="Keyword">import</a> <a id="31233" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="31256" class="Keyword">open</a> <a id="31261" class="Keyword">import</a> <a id="31268" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="31294" class="Keyword">open</a> <a id="31299" class="Keyword">import</a> <a id="31306" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="31332" class="Keyword">open</a> <a id="31337" class="Keyword">import</a> <a id="31344" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="31408" class="Keyword">open</a> <a id="31413" class="Keyword">import</a> <a id="31420" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31438" class="Keyword">open</a> <a id="31443" class="Keyword">import</a> <a id="31450" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31477" class="Keyword">open</a> <a id="31482" class="Keyword">import</a> <a id="31489" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31515" class="Keyword">open</a> <a id="31520" class="Keyword">import</a> <a id="31527" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31553" class="Keyword">open</a> <a id="31558" class="Keyword">import</a> <a id="31565" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31591" class="Keyword">open</a> <a id="31596" class="Keyword">import</a> <a id="31603" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="31634" class="Keyword">open</a> <a id="31639" class="Keyword">import</a> <a id="31646" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="31709" class="Keyword">open</a> <a id="31714" class="Keyword">import</a> <a id="31721" href="polytopes.html" class="Module">polytopes</a>
<a id="31731" class="Keyword">open</a> <a id="31736" class="Keyword">import</a> <a id="31743" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="31801" class="Keyword">open</a> <a id="31806" class="Keyword">import</a> <a id="31813" href="ring-theory.html" class="Module">ring-theory</a>
<a id="31825" class="Keyword">open</a> <a id="31830" class="Keyword">import</a> <a id="31837" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="31874" class="Keyword">open</a> <a id="31879" class="Keyword">import</a> <a id="31886" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="31913" class="Keyword">open</a> <a id="31918" class="Keyword">import</a> <a id="31925" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="31957" class="Keyword">open</a> <a id="31962" class="Keyword">import</a> <a id="31969" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="32015" class="Keyword">open</a> <a id="32020" class="Keyword">import</a> <a id="32027" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="32052" class="Keyword">open</a> <a id="32057" class="Keyword">import</a> <a id="32064" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="32107" class="Keyword">open</a> <a id="32112" class="Keyword">import</a> <a id="32119" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="32157" class="Keyword">open</a> <a id="32162" class="Keyword">import</a> <a id="32169" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="32200" class="Keyword">open</a> <a id="32205" class="Keyword">import</a> <a id="32212" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="32236" class="Keyword">open</a> <a id="32241" class="Keyword">import</a> <a id="32248" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="32280" class="Keyword">open</a> <a id="32285" class="Keyword">import</a> <a id="32292" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="32318" class="Keyword">open</a> <a id="32323" class="Keyword">import</a> <a id="32330" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="32359" class="Keyword">open</a> <a id="32364" class="Keyword">import</a> <a id="32371" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="32408" class="Keyword">open</a> <a id="32413" class="Keyword">import</a> <a id="32420" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32449" class="Keyword">open</a> <a id="32454" class="Keyword">import</a> <a id="32461" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32488" class="Keyword">open</a> <a id="32493" class="Keyword">import</a> <a id="32500" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32537" class="Keyword">open</a> <a id="32542" class="Keyword">import</a> <a id="32549" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32576" class="Keyword">open</a> <a id="32581" class="Keyword">import</a> <a id="32588" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="32621" class="Keyword">open</a> <a id="32626" class="Keyword">import</a> <a id="32633" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="32651" class="Keyword">open</a> <a id="32656" class="Keyword">import</a> <a id="32663" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="32717" class="Keyword">open</a> <a id="32722" class="Keyword">import</a> <a id="32729" href="set-theory.html" class="Module">set-theory</a>
<a id="32740" class="Keyword">open</a> <a id="32745" class="Keyword">import</a> <a id="32752" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="32775" class="Keyword">open</a> <a id="32780" class="Keyword">import</a> <a id="32787" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="32811" class="Keyword">open</a> <a id="32816" class="Keyword">import</a> <a id="32823" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="32849" class="Keyword">open</a> <a id="32854" class="Keyword">import</a> <a id="32861" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="32923" class="Keyword">open</a> <a id="32928" class="Keyword">import</a> <a id="32935" href="structured-types.html" class="Module">structured-types</a>
<a id="32952" class="Keyword">open</a> <a id="32957" class="Keyword">import</a> <a id="32964" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="32999" class="Keyword">open</a> <a id="33004" class="Keyword">import</a> <a id="33011" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="33055" class="Keyword">open</a> <a id="33060" class="Keyword">import</a> <a id="33067" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="33131" class="Keyword">open</a> <a id="33136" class="Keyword">import</a> <a id="33143" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="33182" class="Keyword">open</a> <a id="33187" class="Keyword">import</a> <a id="33194" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="33240" class="Keyword">open</a> <a id="33245" class="Keyword">import</a> <a id="33252" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="33276" class="Keyword">open</a> <a id="33281" class="Keyword">import</a> <a id="33288" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="33357" class="Keyword">open</a> <a id="33362" class="Keyword">import</a> <a id="33369" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="33414" class="Keyword">open</a> <a id="33419" class="Keyword">import</a> <a id="33426" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33460" class="Keyword">open</a> <a id="33465" class="Keyword">import</a> <a id="33472" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33533" class="Keyword">open</a> <a id="33538" class="Keyword">import</a> <a id="33545" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33590" class="Keyword">open</a> <a id="33595" class="Keyword">import</a> <a id="33602" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="33640" class="Keyword">open</a> <a id="33645" class="Keyword">import</a> <a id="33652" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="33695" class="Keyword">open</a> <a id="33700" class="Keyword">import</a> <a id="33707" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="33743" class="Keyword">open</a> <a id="33748" class="Keyword">import</a> <a id="33755" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="33785" class="Keyword">open</a> <a id="33790" class="Keyword">import</a> <a id="33797" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="33828" class="Keyword">open</a> <a id="33833" class="Keyword">import</a> <a id="33840" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="33899" class="Keyword">open</a> <a id="33904" class="Keyword">import</a> <a id="33911" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="33962" class="Keyword">open</a> <a id="33967" class="Keyword">import</a> <a id="33974" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="34025" class="Keyword">open</a> <a id="34030" class="Keyword">import</a> <a id="34037" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="34092" class="Keyword">open</a> <a id="34097" class="Keyword">import</a> <a id="34104" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="34133" class="Keyword">open</a> <a id="34138" class="Keyword">import</a> <a id="34145" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="34173" class="Keyword">open</a> <a id="34178" class="Keyword">import</a> <a id="34185" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="34215" class="Keyword">open</a> <a id="34220" class="Keyword">import</a> <a id="34227" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="34261" class="Keyword">open</a> <a id="34266" class="Keyword">import</a> <a id="34273" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="34349" class="Keyword">open</a> <a id="34354" class="Keyword">import</a> <a id="34361" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="34387" class="Keyword">open</a> <a id="34392" class="Keyword">import</a> <a id="34399" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="34438" class="Keyword">open</a> <a id="34443" class="Keyword">import</a> <a id="34450" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34488" class="Keyword">open</a> <a id="34493" class="Keyword">import</a> <a id="34500" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34546" class="Keyword">open</a> <a id="34551" class="Keyword">import</a> <a id="34558" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34595" class="Keyword">open</a> <a id="34600" class="Keyword">import</a> <a id="34607" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34647" class="Keyword">open</a> <a id="34652" class="Keyword">import</a> <a id="34659" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="34698" class="Keyword">open</a> <a id="34703" class="Keyword">import</a> <a id="34710" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="34743" class="Keyword">open</a> <a id="34748" class="Keyword">import</a> <a id="34755" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="34790" class="Keyword">open</a> <a id="34795" class="Keyword">import</a> <a id="34802" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="34847" class="Keyword">open</a> <a id="34852" class="Keyword">import</a> <a id="34859" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="34911" class="Keyword">open</a> <a id="34916" class="Keyword">import</a> <a id="34923" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="34976" class="Keyword">open</a> <a id="34981" class="Keyword">import</a> <a id="34988" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="35048" class="Keyword">open</a> <a id="35053" class="Keyword">import</a> <a id="35060" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="35108" class="Keyword">open</a> <a id="35113" class="Keyword">import</a> <a id="35120" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="35160" class="Keyword">open</a> <a id="35165" class="Keyword">import</a> <a id="35172" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="35219" class="Keyword">open</a> <a id="35224" class="Keyword">import</a> <a id="35231" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="35272" class="Keyword">open</a> <a id="35277" class="Keyword">import</a> <a id="35284" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="35322" class="Keyword">open</a> <a id="35327" class="Keyword">import</a> <a id="35334" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="35382" class="Keyword">open</a> <a id="35387" class="Keyword">import</a> <a id="35394" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35431" class="Keyword">open</a> <a id="35436" class="Keyword">import</a> <a id="35443" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35477" class="Keyword">open</a> <a id="35482" class="Keyword">import</a> <a id="35489" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35536" class="Keyword">open</a> <a id="35541" class="Keyword">import</a> <a id="35548" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35593" class="Keyword">open</a> <a id="35598" class="Keyword">import</a> <a id="35605" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35654" class="Keyword">open</a> <a id="35659" class="Keyword">import</a> <a id="35666" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="35743" class="Keyword">open</a> <a id="35748" class="Keyword">import</a> <a id="35755" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="35807" class="Keyword">open</a> <a id="35812" class="Keyword">import</a> <a id="35819" href="type-theories.html" class="Module">type-theories</a>
<a id="35833" class="Keyword">open</a> <a id="35838" class="Keyword">import</a> <a id="35845" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="35887" class="Keyword">open</a> <a id="35892" class="Keyword">import</a> <a id="35899" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="35937" class="Keyword">open</a> <a id="35942" class="Keyword">import</a> <a id="35949" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="35995" class="Keyword">open</a> <a id="36000" class="Keyword">import</a> <a id="36007" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="36054" class="Keyword">open</a> <a id="36059" class="Keyword">import</a> <a id="36066" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="36101" class="Keyword">open</a> <a id="36106" class="Keyword">import</a> <a id="36113" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="36191" class="Keyword">open</a> <a id="36196" class="Keyword">import</a> <a id="36203" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="36227" class="Keyword">open</a> <a id="36232" class="Keyword">import</a> <a id="36239" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="36292" class="Keyword">open</a> <a id="36297" class="Keyword">import</a> <a id="36304" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="36347" class="Keyword">open</a> <a id="36352" class="Keyword">import</a> <a id="36359" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="36399" class="Keyword">open</a> <a id="36404" class="Keyword">import</a> <a id="36411" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36450" class="Keyword">open</a> <a id="36455" class="Keyword">import</a> <a id="36462" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36496" class="Keyword">open</a> <a id="36501" class="Keyword">import</a> <a id="36508" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36556" class="Keyword">open</a> <a id="36561" class="Keyword">import</a> <a id="36568" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36619" class="Keyword">open</a> <a id="36624" class="Keyword">import</a> <a id="36631" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="36678" class="Keyword">open</a> <a id="36683" class="Keyword">import</a> <a id="36690" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="36742" class="Keyword">open</a> <a id="36747" class="Keyword">import</a> <a id="36754" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="36798" class="Keyword">open</a> <a id="36803" class="Keyword">import</a> <a id="36810" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="36850" class="Keyword">open</a> <a id="36855" class="Keyword">import</a> <a id="36862" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="36905" class="Keyword">open</a> <a id="36910" class="Keyword">import</a> <a id="36917" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="36969" class="Keyword">open</a> <a id="36974" class="Keyword">import</a> <a id="36981" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="37035" class="Keyword">open</a> <a id="37040" class="Keyword">import</a> <a id="37047" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="37095" class="Keyword">open</a> <a id="37100" class="Keyword">import</a> <a id="37107" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="37146" class="Keyword">open</a> <a id="37151" class="Keyword">import</a> <a id="37158" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="37191" class="Keyword">open</a> <a id="37196" class="Keyword">import</a> <a id="37203" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="37233" class="Keyword">open</a> <a id="37238" class="Keyword">import</a> <a id="37245" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="37296" class="Keyword">open</a> <a id="37301" class="Keyword">import</a> <a id="37308" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="37349" class="Keyword">open</a> <a id="37354" class="Keyword">import</a> <a id="37361" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="37398" class="Keyword">open</a> <a id="37403" class="Keyword">import</a> <a id="37410" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="37469" class="Keyword">open</a> <a id="37474" class="Keyword">import</a> <a id="37481" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37536" class="Keyword">open</a> <a id="37541" class="Keyword">import</a> <a id="37548" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37604" class="Keyword">open</a> <a id="37609" class="Keyword">import</a> <a id="37616" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="37663" class="Keyword">open</a> <a id="37668" class="Keyword">import</a> <a id="37675" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="37718" class="Keyword">open</a> <a id="37723" class="Keyword">import</a> <a id="37730" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="37775" class="Keyword">open</a> <a id="37780" class="Keyword">import</a> <a id="37787" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="37836" class="Keyword">open</a> <a id="37841" class="Keyword">import</a> <a id="37848" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="37899" class="Keyword">open</a> <a id="37904" class="Keyword">import</a> <a id="37911" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="37955" class="Keyword">open</a> <a id="37960" class="Keyword">import</a> <a id="37967" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="38045" class="Keyword">open</a> <a id="38050" class="Keyword">import</a> <a id="38057" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="38097" class="Keyword">open</a> <a id="38102" class="Keyword">import</a> <a id="38109" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="38166" class="Keyword">open</a> <a id="38171" class="Keyword">import</a> <a id="38178" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="38213" class="Keyword">open</a> <a id="38218" class="Keyword">import</a> <a id="38225" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="38271" class="Keyword">open</a> <a id="38276" class="Keyword">import</a> <a id="38283" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="38338" class="Keyword">open</a> <a id="38343" class="Keyword">import</a> <a id="38350" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="38393" class="Keyword">open</a> <a id="38398" class="Keyword">import</a> <a id="38405" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38450" class="Keyword">open</a> <a id="38455" class="Keyword">import</a> <a id="38462" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38521" class="Keyword">open</a> <a id="38526" class="Keyword">import</a> <a id="38533" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38570" class="Keyword">open</a> <a id="38575" class="Keyword">import</a> <a id="38582" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38624" class="Keyword">open</a> <a id="38629" class="Keyword">import</a> <a id="38636" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="38677" class="Keyword">open</a> <a id="38682" class="Keyword">import</a> <a id="38689" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="38728" class="Keyword">open</a> <a id="38733" class="Keyword">import</a> <a id="38740" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="38778" class="Keyword">open</a> <a id="38783" class="Keyword">import</a> <a id="38790" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="38842" class="Keyword">open</a> <a id="38847" class="Keyword">import</a> <a id="38854" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="38899" class="Keyword">open</a> <a id="38904" class="Keyword">import</a> <a id="38911" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="38950" class="Keyword">open</a> <a id="38955" class="Keyword">import</a> <a id="38962" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="38999" class="Keyword">open</a> <a id="39004" class="Keyword">import</a> <a id="39011" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="39060" class="Keyword">open</a> <a id="39065" class="Keyword">import</a> <a id="39072" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="39111" class="Keyword">open</a> <a id="39116" class="Keyword">import</a> <a id="39123" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="39161" class="Keyword">open</a> <a id="39166" class="Keyword">import</a> <a id="39173" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="39228" class="Keyword">open</a> <a id="39233" class="Keyword">import</a> <a id="39240" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="39279" class="Keyword">open</a> <a id="39284" class="Keyword">import</a> <a id="39291" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="39339" class="Keyword">open</a> <a id="39344" class="Keyword">import</a> <a id="39351" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="39398" class="Keyword">open</a> <a id="39403" class="Keyword">import</a> <a id="39410" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39448" class="Keyword">open</a> <a id="39453" class="Keyword">import</a> <a id="39460" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="39490" class="Keyword">open</a> <a id="39495" class="Keyword">import</a> <a id="39502" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39559" class="Keyword">open</a> <a id="39564" class="Keyword">import</a> <a id="39571" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39625" class="Keyword">open</a> <a id="39630" class="Keyword">import</a> <a id="39637" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="39667" class="Keyword">open</a> <a id="39672" class="Keyword">import</a> <a id="39679" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="39728" class="Keyword">open</a> <a id="39733" class="Keyword">import</a> <a id="39740" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="39782" class="Keyword">open</a> <a id="39787" class="Keyword">import</a> <a id="39794" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="39828" class="Keyword">open</a> <a id="39833" class="Keyword">import</a> <a id="39840" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="39903" class="Keyword">open</a> <a id="39908" class="Keyword">import</a> <a id="39915" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="39958" class="Keyword">open</a> <a id="39963" class="Keyword">import</a> <a id="39970" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="40005" class="Keyword">open</a> <a id="40010" class="Keyword">import</a> <a id="40017" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="40052" class="Keyword">open</a> <a id="40057" class="Keyword">import</a> <a id="40064" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="40104" class="Keyword">open</a> <a id="40109" class="Keyword">import</a> <a id="40116" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="40161" class="Keyword">open</a> <a id="40166" class="Keyword">import</a> <a id="40173" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="40214" class="Keyword">open</a> <a id="40219" class="Keyword">import</a> <a id="40226" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="40280" class="Keyword">open</a> <a id="40285" class="Keyword">import</a> <a id="40292" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="40342" class="Keyword">open</a> <a id="40347" class="Keyword">import</a> <a id="40354" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="40401" class="Keyword">open</a> <a id="40406" class="Keyword">import</a> <a id="40413" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40451" class="Keyword">open</a> <a id="40456" class="Keyword">import</a> <a id="40463" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40512" class="Keyword">open</a> <a id="40517" class="Keyword">import</a> <a id="40524" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40571" class="Keyword">open</a> <a id="40576" class="Keyword">import</a> <a id="40583" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40646" class="Keyword">open</a> <a id="40651" class="Keyword">import</a> <a id="40658" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="40690" class="Keyword">open</a> <a id="40695" class="Keyword">import</a> <a id="40702" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="40755" class="Keyword">open</a> <a id="40760" class="Keyword">import</a> <a id="40767" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="40813" class="Keyword">open</a> <a id="40818" class="Keyword">import</a> <a id="40825" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="40871" class="Keyword">open</a> <a id="40876" class="Keyword">import</a> <a id="40883" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="40923" class="Keyword">open</a> <a id="40928" class="Keyword">import</a> <a id="40935" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="40982" class="Keyword">open</a> <a id="40987" class="Keyword">import</a> <a id="40994" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="41042" class="Keyword">open</a> <a id="41047" class="Keyword">import</a> <a id="41054" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="41094" class="Keyword">open</a> <a id="41099" class="Keyword">import</a> <a id="41106" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="41151" class="Keyword">open</a> <a id="41156" class="Keyword">import</a> <a id="41163" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="41228" class="Keyword">open</a> <a id="41233" class="Keyword">import</a> <a id="41240" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="41285" class="Keyword">open</a> <a id="41290" class="Keyword">import</a> <a id="41297" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="41344" class="Keyword">open</a> <a id="41349" class="Keyword">import</a> <a id="41356" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="41409" class="Keyword">open</a> <a id="41414" class="Keyword">import</a> <a id="41421" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>