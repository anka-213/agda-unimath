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
<a id="12565" class="Keyword">open</a> <a id="12570" class="Keyword">import</a> <a id="12577" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="12620" class="Keyword">open</a> <a id="12625" class="Keyword">import</a> <a id="12632" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12658" class="Keyword">open</a> <a id="12663" class="Keyword">import</a> <a id="12670" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12704" class="Keyword">open</a> <a id="12709" class="Keyword">import</a> <a id="12716" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="12747" class="Keyword">open</a> <a id="12752" class="Keyword">import</a> <a id="12759" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12789" class="Keyword">open</a> <a id="12794" class="Keyword">import</a> <a id="12801" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12828" class="Keyword">open</a> <a id="12833" class="Keyword">import</a> <a id="12840" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="12878" class="Keyword">open</a> <a id="12883" class="Keyword">import</a> <a id="12890" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12922" class="Keyword">open</a> <a id="12927" class="Keyword">import</a> <a id="12934" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12968" class="Keyword">open</a> <a id="12973" class="Keyword">import</a> <a id="12980" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13003" class="Keyword">open</a> <a id="13008" class="Keyword">import</a> <a id="13015" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13042" class="Keyword">open</a> <a id="13047" class="Keyword">import</a> <a id="13054" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13082" class="Keyword">open</a> <a id="13087" class="Keyword">import</a> <a id="13094" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13131" class="Keyword">open</a> <a id="13136" class="Keyword">import</a> <a id="13143" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13191" class="Keyword">open</a> <a id="13196" class="Keyword">import</a> <a id="13203" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13243" class="Keyword">open</a> <a id="13248" class="Keyword">import</a> <a id="13255" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13277" class="Keyword">open</a> <a id="13282" class="Keyword">import</a> <a id="13289" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13312" class="Keyword">open</a> <a id="13317" class="Keyword">import</a> <a id="13324" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13349" class="Keyword">open</a> <a id="13354" class="Keyword">import</a> <a id="13361" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13406" class="Keyword">open</a> <a id="13411" class="Keyword">import</a> <a id="13418" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13462" class="Keyword">open</a> <a id="13467" class="Keyword">import</a> <a id="13474" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13510" class="Keyword">open</a> <a id="13515" class="Keyword">import</a> <a id="13522" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13567" class="Keyword">open</a> <a id="13572" class="Keyword">import</a> <a id="13579" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13620" class="Keyword">open</a> <a id="13625" class="Keyword">import</a> <a id="13632" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13667" class="Keyword">open</a> <a id="13672" class="Keyword">import</a> <a id="13679" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13711" class="Keyword">open</a> <a id="13716" class="Keyword">import</a> <a id="13723" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13754" class="Keyword">open</a> <a id="13759" class="Keyword">import</a> <a id="13766" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13799" class="Keyword">open</a> <a id="13804" class="Keyword">import</a> <a id="13811" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13844" class="Keyword">open</a> <a id="13849" class="Keyword">import</a> <a id="13856" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13886" class="Keyword">open</a> <a id="13891" class="Keyword">import</a> <a id="13898" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13922" class="Keyword">open</a> <a id="13927" class="Keyword">import</a> <a id="13934" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13972" class="Keyword">open</a> <a id="13977" class="Keyword">import</a> <a id="13984" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14015" class="Keyword">open</a> <a id="14020" class="Keyword">import</a> <a id="14027" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14052" class="Keyword">open</a> <a id="14057" class="Keyword">import</a> <a id="14064" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14092" class="Keyword">open</a> <a id="14097" class="Keyword">import</a> <a id="14104" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14128" class="Keyword">open</a> <a id="14133" class="Keyword">import</a> <a id="14140" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14166" class="Keyword">open</a> <a id="14171" class="Keyword">import</a> <a id="14178" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14213" class="Keyword">open</a> <a id="14218" class="Keyword">import</a> <a id="14225" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14246" class="Keyword">open</a> <a id="14251" class="Keyword">import</a> <a id="14258" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14307" class="Keyword">open</a> <a id="14312" class="Keyword">import</a> <a id="14319" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14360" class="Keyword">open</a> <a id="14365" class="Keyword">import</a> <a id="14372" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14422" class="Keyword">open</a> <a id="14427" class="Keyword">import</a> <a id="14434" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14480" class="Keyword">open</a> <a id="14485" class="Keyword">import</a> <a id="14492" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14532" class="Keyword">open</a> <a id="14537" class="Keyword">import</a> <a id="14544" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14594" class="Keyword">open</a> <a id="14599" class="Keyword">import</a> <a id="14606" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14645" class="Keyword">open</a> <a id="14650" class="Keyword">import</a> <a id="14657" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14697" class="Keyword">open</a> <a id="14702" class="Keyword">import</a> <a id="14709" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14742" class="Keyword">open</a> <a id="14747" class="Keyword">import</a> <a id="14754" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14803" class="Keyword">open</a> <a id="14808" class="Keyword">import</a> <a id="14815" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14840" class="Keyword">open</a> <a id="14845" class="Keyword">import</a> <a id="14852" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14890" class="Keyword">open</a> <a id="14895" class="Keyword">import</a> <a id="14902" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14924" class="Keyword">open</a> <a id="14929" class="Keyword">import</a> <a id="14936" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14964" class="Keyword">open</a> <a id="14969" class="Keyword">import</a> <a id="14976" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15012" class="Keyword">open</a> <a id="15017" class="Keyword">import</a> <a id="15024" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15050" class="Keyword">open</a> <a id="15055" class="Keyword">import</a> <a id="15062" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15080" class="Keyword">open</a> <a id="15085" class="Keyword">import</a> <a id="15092" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15127" class="Keyword">open</a> <a id="15132" class="Keyword">import</a> <a id="15139" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15174" class="Keyword">open</a> <a id="15179" class="Keyword">import</a> <a id="15186" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15213" class="Keyword">open</a> <a id="15218" class="Keyword">import</a> <a id="15225" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15281" class="Keyword">open</a> <a id="15286" class="Keyword">import</a> <a id="15293" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15322" class="Keyword">open</a> <a id="15327" class="Keyword">import</a> <a id="15334" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15364" class="Keyword">open</a> <a id="15369" class="Keyword">import</a> <a id="15376" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15403" class="Keyword">open</a> <a id="15408" class="Keyword">import</a> <a id="15415" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15441" class="Keyword">open</a> <a id="15446" class="Keyword">import</a> <a id="15453" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15480" class="Keyword">open</a> <a id="15485" class="Keyword">import</a> <a id="15492" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15516" class="Keyword">open</a> <a id="15521" class="Keyword">import</a> <a id="15528" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15551" class="Keyword">open</a> <a id="15556" class="Keyword">import</a> <a id="15563" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15590" class="Keyword">open</a> <a id="15595" class="Keyword">import</a> <a id="15602" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15634" class="Keyword">open</a> <a id="15639" class="Keyword">import</a> <a id="15646" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15681" class="Keyword">open</a> <a id="15686" class="Keyword">import</a> <a id="15693" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15724" class="Keyword">open</a> <a id="15729" class="Keyword">import</a> <a id="15736" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15769" class="Keyword">open</a> <a id="15774" class="Keyword">import</a> <a id="15781" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15815" class="Keyword">open</a> <a id="15820" class="Keyword">import</a> <a id="15827" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15867" class="Keyword">open</a> <a id="15872" class="Keyword">import</a> <a id="15879" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15910" class="Keyword">open</a> <a id="15915" class="Keyword">import</a> <a id="15922" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15954" class="Keyword">open</a> <a id="15959" class="Keyword">import</a> <a id="15966" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15997" class="Keyword">open</a> <a id="16002" class="Keyword">import</a> <a id="16009" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16026" class="Keyword">open</a> <a id="16031" class="Keyword">import</a> <a id="16038" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16063" class="Keyword">open</a> <a id="16068" class="Keyword">import</a> <a id="16075" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16104" class="Keyword">open</a> <a id="16109" class="Keyword">import</a> <a id="16116" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16141" class="Keyword">open</a> <a id="16146" class="Keyword">import</a> <a id="16153" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16174" class="Keyword">open</a> <a id="16179" class="Keyword">import</a> <a id="16186" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16210" class="Keyword">open</a> <a id="16215" class="Keyword">import</a> <a id="16222" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16242" class="Keyword">open</a> <a id="16247" class="Keyword">import</a> <a id="16254" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16288" class="Keyword">open</a> <a id="16293" class="Keyword">import</a> <a id="16300" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16338" class="Keyword">open</a> <a id="16343" class="Keyword">import</a> <a id="16350" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16378" class="Keyword">open</a> <a id="16383" class="Keyword">import</a> <a id="16390" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16414" class="Keyword">open</a> <a id="16419" class="Keyword">import</a> <a id="16426" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16453" class="Keyword">open</a> <a id="16458" class="Keyword">import</a> <a id="16465" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16500" class="Keyword">open</a> <a id="16505" class="Keyword">import</a> <a id="16512" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16533" class="Keyword">open</a> <a id="16538" class="Keyword">import</a> <a id="16545" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16581" class="Keyword">open</a> <a id="16586" class="Keyword">import</a> <a id="16593" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16638" class="Keyword">open</a> <a id="16643" class="Keyword">import</a> <a id="16650" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16696" class="Keyword">open</a> <a id="16701" class="Keyword">import</a> <a id="16708" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16748" class="Keyword">open</a> <a id="16753" class="Keyword">import</a> <a id="16760" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16790" class="Keyword">open</a> <a id="16795" class="Keyword">import</a> <a id="16802" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="16836" class="Keyword">open</a> <a id="16841" class="Keyword">import</a> <a id="16848" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16885" class="Keyword">open</a> <a id="16890" class="Keyword">import</a> <a id="16897" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16921" class="Keyword">open</a> <a id="16926" class="Keyword">import</a> <a id="16933" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16954" class="Keyword">open</a> <a id="16959" class="Keyword">import</a> <a id="16966" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17001" class="Keyword">open</a> <a id="17006" class="Keyword">import</a> <a id="17013" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17050" class="Keyword">open</a> <a id="17055" class="Keyword">import</a> <a id="17062" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17111" class="Keyword">open</a> <a id="17116" class="Keyword">import</a> <a id="17123" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17156" class="Keyword">open</a> <a id="17161" class="Keyword">import</a> <a id="17168" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17191" class="Keyword">open</a> <a id="17196" class="Keyword">import</a> <a id="17203" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17226" class="Keyword">open</a> <a id="17231" class="Keyword">import</a> <a id="17238" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17261" class="Keyword">open</a> <a id="17266" class="Keyword">import</a> <a id="17273" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17301" class="Keyword">open</a> <a id="17306" class="Keyword">import</a> <a id="17313" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17333" class="Keyword">open</a> <a id="17338" class="Keyword">import</a> <a id="17345" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17366" class="Keyword">open</a> <a id="17371" class="Keyword">import</a> <a id="17378" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17409" class="Keyword">open</a> <a id="17414" class="Keyword">import</a> <a id="17421" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17448" class="Keyword">open</a> <a id="17453" class="Keyword">import</a> <a id="17460" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17476" class="Keyword">open</a> <a id="17481" class="Keyword">import</a> <a id="17488" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17519" class="Keyword">open</a> <a id="17524" class="Keyword">import</a> <a id="17531" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17548" class="Keyword">open</a> <a id="17553" class="Keyword">import</a> <a id="17560" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17582" class="Keyword">open</a> <a id="17587" class="Keyword">import</a> <a id="17594" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17621" class="Keyword">open</a> <a id="17626" class="Keyword">import</a> <a id="17633" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17656" class="Keyword">open</a> <a id="17661" class="Keyword">import</a> <a id="17668" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17695" class="Keyword">open</a> <a id="17700" class="Keyword">import</a> <a id="17707" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17740" class="Keyword">open</a> <a id="17745" class="Keyword">import</a> <a id="17752" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17792" class="Keyword">open</a> <a id="17797" class="Keyword">import</a> <a id="17804" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17825" class="Keyword">open</a> <a id="17830" class="Keyword">import</a> <a id="17837" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17866" class="Keyword">open</a> <a id="17871" class="Keyword">import</a> <a id="17878" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17916" class="Keyword">open</a> <a id="17921" class="Keyword">import</a> <a id="17928" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17948" class="Keyword">open</a> <a id="17953" class="Keyword">import</a> <a id="17960" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17984" class="Keyword">open</a> <a id="17989" class="Keyword">import</a> <a id="17996" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18023" class="Keyword">open</a> <a id="18028" class="Keyword">import</a> <a id="18035" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18067" class="Keyword">open</a> <a id="18072" class="Keyword">import</a> <a id="18079" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18109" class="Keyword">open</a> <a id="18114" class="Keyword">import</a> <a id="18121" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18147" class="Keyword">open</a> <a id="18152" class="Keyword">import</a> <a id="18159" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18186" class="Keyword">open</a> <a id="18191" class="Keyword">import</a> <a id="18198" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18227" class="Keyword">open</a> <a id="18232" class="Keyword">import</a> <a id="18239" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18262" class="Keyword">open</a> <a id="18267" class="Keyword">import</a> <a id="18274" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18325" class="Keyword">open</a> <a id="18330" class="Keyword">import</a> <a id="18337" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18380" class="Keyword">open</a> <a id="18385" class="Keyword">import</a> <a id="18392" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18440" class="Keyword">open</a> <a id="18445" class="Keyword">import</a> <a id="18452" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18490" class="Keyword">open</a> <a id="18495" class="Keyword">import</a> <a id="18502" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18539" class="Keyword">open</a> <a id="18544" class="Keyword">import</a> <a id="18551" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18597" class="Keyword">open</a> <a id="18602" class="Keyword">import</a> <a id="18609" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18626" class="Keyword">open</a> <a id="18631" class="Keyword">import</a> <a id="18638" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18666" class="Keyword">open</a> <a id="18671" class="Keyword">import</a> <a id="18678" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18706" class="Keyword">open</a> <a id="18711" class="Keyword">import</a> <a id="18718" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18754" class="Keyword">open</a> <a id="18759" class="Keyword">import</a> <a id="18766" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18804" class="Keyword">open</a> <a id="18809" class="Keyword">import</a> <a id="18816" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18849" class="Keyword">open</a> <a id="18854" class="Keyword">import</a> <a id="18861" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18882" class="Keyword">open</a> <a id="18887" class="Keyword">import</a> <a id="18894" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="18930" class="Keyword">open</a> <a id="18935" class="Keyword">import</a> <a id="18942" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18996" class="Keyword">open</a> <a id="19001" class="Keyword">import</a> <a id="19008" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19030" class="Keyword">open</a> <a id="19035" class="Keyword">import</a> <a id="19042" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19077" class="Keyword">open</a> <a id="19082" class="Keyword">import</a> <a id="19089" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19119" class="Keyword">open</a> <a id="19124" class="Keyword">import</a> <a id="19131" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19170" class="Keyword">open</a> <a id="19175" class="Keyword">import</a> <a id="19182" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19236" class="Keyword">open</a> <a id="19241" class="Keyword">import</a> <a id="19248" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19294" class="Keyword">open</a> <a id="19299" class="Keyword">import</a> <a id="19306" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19357" class="Keyword">open</a> <a id="19362" class="Keyword">import</a> <a id="19369" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19410" class="Keyword">open</a> <a id="19415" class="Keyword">import</a> <a id="19422" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19467" class="Keyword">open</a> <a id="19472" class="Keyword">import</a> <a id="19479" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19524" class="Keyword">open</a> <a id="19529" class="Keyword">import</a> <a id="19536" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19572" class="Keyword">open</a> <a id="19577" class="Keyword">import</a> <a id="19584" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19620" class="Keyword">open</a> <a id="19625" class="Keyword">import</a> <a id="19632" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19697" class="Keyword">open</a> <a id="19702" class="Keyword">import</a> <a id="19709" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19764" class="Keyword">open</a> <a id="19769" class="Keyword">import</a> <a id="19776" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19816" class="Keyword">open</a> <a id="19821" class="Keyword">import</a> <a id="19828" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19872" class="Keyword">open</a> <a id="19877" class="Keyword">import</a> <a id="19884" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19929" class="Keyword">open</a> <a id="19934" class="Keyword">import</a> <a id="19941" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19982" class="Keyword">open</a> <a id="19987" class="Keyword">import</a> <a id="19994" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20034" class="Keyword">open</a> <a id="20039" class="Keyword">import</a> <a id="20046" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20073" class="Keyword">open</a> <a id="20078" class="Keyword">import</a> <a id="20085" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20121" class="Keyword">open</a> <a id="20126" class="Keyword">import</a> <a id="20133" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20160" class="Keyword">open</a> <a id="20165" class="Keyword">import</a> <a id="20172" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20209" class="Keyword">open</a> <a id="20214" class="Keyword">import</a> <a id="20221" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20249" class="Keyword">open</a> <a id="20254" class="Keyword">import</a> <a id="20261" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20280" class="Keyword">open</a> <a id="20285" class="Keyword">import</a> <a id="20292" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20332" class="Keyword">open</a> <a id="20337" class="Keyword">import</a> <a id="20344" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20376" class="Keyword">open</a> <a id="20381" class="Keyword">import</a> <a id="20388" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20436" class="Keyword">open</a> <a id="20441" class="Keyword">import</a> <a id="20448" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20471" class="Keyword">open</a> <a id="20476" class="Keyword">import</a> <a id="20483" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20507" class="Keyword">open</a> <a id="20512" class="Keyword">import</a> <a id="20519" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20559" class="Keyword">open</a> <a id="20564" class="Keyword">import</a> <a id="20571" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20614" class="Keyword">open</a> <a id="20619" class="Keyword">import</a> <a id="20626" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20660" class="Keyword">open</a> <a id="20665" class="Keyword">import</a> <a id="20672" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20704" class="Keyword">open</a> <a id="20709" class="Keyword">import</a> <a id="20716" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20746" class="Keyword">open</a> <a id="20751" class="Keyword">import</a> <a id="20758" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20792" class="Keyword">open</a> <a id="20797" class="Keyword">import</a> <a id="20804" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20839" class="Keyword">open</a> <a id="20844" class="Keyword">import</a> <a id="20851" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20888" class="Keyword">open</a> <a id="20893" class="Keyword">import</a> <a id="20900" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20927" class="Keyword">open</a> <a id="20932" class="Keyword">import</a> <a id="20939" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20967" class="Keyword">open</a> <a id="20972" class="Keyword">import</a> <a id="20979" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21028" class="Keyword">open</a> <a id="21033" class="Keyword">import</a> <a id="21040" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21086" class="Keyword">open</a> <a id="21091" class="Keyword">import</a> <a id="21098" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21138" class="Keyword">open</a> <a id="21143" class="Keyword">import</a> <a id="21150" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21188" class="Keyword">open</a> <a id="21193" class="Keyword">import</a> <a id="21200" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21229" class="Keyword">open</a> <a id="21234" class="Keyword">import</a> <a id="21241" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21271" class="Keyword">open</a> <a id="21276" class="Keyword">import</a> <a id="21283" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21314" class="Keyword">open</a> <a id="21319" class="Keyword">import</a> <a id="21326" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21366" class="Keyword">open</a> <a id="21371" class="Keyword">import</a> <a id="21378" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21404" class="Keyword">open</a> <a id="21409" class="Keyword">import</a> <a id="21416" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21471" class="Keyword">open</a> <a id="21476" class="Keyword">import</a> <a id="21483" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21534" class="Keyword">open</a> <a id="21539" class="Keyword">import</a> <a id="21546" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21591" class="Keyword">open</a> <a id="21596" class="Keyword">import</a> <a id="21603" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21657" class="Keyword">open</a> <a id="21662" class="Keyword">import</a> <a id="21669" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21696" class="Keyword">open</a> <a id="21701" class="Keyword">import</a> <a id="21708" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21741" class="Keyword">open</a> <a id="21746" class="Keyword">import</a> <a id="21753" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21784" class="Keyword">open</a> <a id="21789" class="Keyword">import</a> <a id="21796" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21833" class="Keyword">open</a> <a id="21838" class="Keyword">import</a> <a id="21845" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21870" class="Keyword">open</a> <a id="21875" class="Keyword">import</a> <a id="21882" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21914" class="Keyword">open</a> <a id="21919" class="Keyword">import</a> <a id="21926" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21961" class="Keyword">open</a> <a id="21966" class="Keyword">import</a> <a id="21973" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22002" class="Keyword">open</a> <a id="22007" class="Keyword">import</a> <a id="22014" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22040" class="Keyword">open</a> <a id="22045" class="Keyword">import</a> <a id="22052" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22080" class="Keyword">open</a> <a id="22085" class="Keyword">import</a> <a id="22092" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22117" class="Keyword">open</a> <a id="22122" class="Keyword">import</a> <a id="22129" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22150" class="Keyword">open</a> <a id="22155" class="Keyword">import</a> <a id="22162" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22198" class="Keyword">open</a> <a id="22203" class="Keyword">import</a> <a id="22210" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22253" class="Keyword">open</a> <a id="22258" class="Keyword">import</a> <a id="22265" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22290" class="Keyword">open</a> <a id="22295" class="Keyword">import</a> <a id="22302" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22333" class="Keyword">open</a> <a id="22338" class="Keyword">import</a> <a id="22345" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22377" class="Keyword">open</a> <a id="22382" class="Keyword">import</a> <a id="22389" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22423" class="Keyword">open</a> <a id="22428" class="Keyword">import</a> <a id="22435" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22491" class="Keyword">open</a> <a id="22496" class="Keyword">import</a> <a id="22503" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22556" class="Keyword">open</a> <a id="22561" class="Keyword">import</a> <a id="22568" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22595" class="Keyword">open</a> <a id="22600" class="Keyword">import</a> <a id="22607" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22652" class="Keyword">open</a> <a id="22657" class="Keyword">import</a> <a id="22664" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22726" class="Keyword">open</a> <a id="22731" class="Keyword">import</a> <a id="22738" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22751" class="Keyword">open</a> <a id="22756" class="Keyword">import</a> <a id="22763" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="22803" class="Keyword">open</a> <a id="22808" class="Keyword">import</a> <a id="22815" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="22859" class="Keyword">open</a> <a id="22864" class="Keyword">import</a> <a id="22871" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="22910" class="Keyword">open</a> <a id="22915" class="Keyword">import</a> <a id="22922" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="22964" class="Keyword">open</a> <a id="22969" class="Keyword">import</a> <a id="22976" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23016" class="Keyword">open</a> <a id="23021" class="Keyword">import</a> <a id="23028" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23069" class="Keyword">open</a> <a id="23074" class="Keyword">import</a> <a id="23081" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23119" class="Keyword">open</a> <a id="23124" class="Keyword">import</a> <a id="23131" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23194" class="Keyword">open</a> <a id="23199" class="Keyword">import</a> <a id="23206" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23235" class="Keyword">open</a> <a id="23240" class="Keyword">import</a> <a id="23247" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23292" class="Keyword">open</a> <a id="23297" class="Keyword">import</a> <a id="23304" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23346" class="Keyword">open</a> <a id="23351" class="Keyword">import</a> <a id="23358" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23402" class="Keyword">open</a> <a id="23407" class="Keyword">import</a> <a id="23414" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23463" class="Keyword">open</a> <a id="23468" class="Keyword">import</a> <a id="23475" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23525" class="Keyword">open</a> <a id="23530" class="Keyword">import</a> <a id="23537" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23564" class="Keyword">open</a> <a id="23569" class="Keyword">import</a> <a id="23576" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23617" class="Keyword">open</a> <a id="23622" class="Keyword">import</a> <a id="23629" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23652" class="Keyword">open</a> <a id="23657" class="Keyword">import</a> <a id="23664" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23713" class="Keyword">open</a> <a id="23718" class="Keyword">import</a> <a id="23725" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23764" class="Keyword">open</a> <a id="23769" class="Keyword">import</a> <a id="23776" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="23817" class="Keyword">open</a> <a id="23822" class="Keyword">import</a> <a id="23829" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="23873" class="Keyword">open</a> <a id="23878" class="Keyword">import</a> <a id="23885" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="23922" class="Keyword">open</a> <a id="23927" class="Keyword">import</a> <a id="23934" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="23956" class="Keyword">open</a> <a id="23961" class="Keyword">import</a> <a id="23968" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23998" class="Keyword">open</a> <a id="24003" class="Keyword">import</a> <a id="24010" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24049" class="Keyword">open</a> <a id="24054" class="Keyword">import</a> <a id="24061" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24099" class="Keyword">open</a> <a id="24104" class="Keyword">import</a> <a id="24111" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24169" class="Keyword">open</a> <a id="24174" class="Keyword">import</a> <a id="24181" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24246" class="Keyword">open</a> <a id="24251" class="Keyword">import</a> <a id="24258" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24289" class="Keyword">open</a> <a id="24294" class="Keyword">import</a> <a id="24301" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24328" class="Keyword">open</a> <a id="24333" class="Keyword">import</a> <a id="24340" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24398" class="Keyword">open</a> <a id="24403" class="Keyword">import</a> <a id="24410" href="group-theory.html" class="Module">group-theory</a>
<a id="24423" class="Keyword">open</a> <a id="24428" class="Keyword">import</a> <a id="24435" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24463" class="Keyword">open</a> <a id="24468" class="Keyword">import</a> <a id="24475" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="24506" class="Keyword">open</a> <a id="24511" class="Keyword">import</a> <a id="24518" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="24554" class="Keyword">open</a> <a id="24559" class="Keyword">import</a> <a id="24566" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24617" class="Keyword">open</a> <a id="24622" class="Keyword">import</a> <a id="24629" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24662" class="Keyword">open</a> <a id="24667" class="Keyword">import</a> <a id="24674" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24721" class="Keyword">open</a> <a id="24726" class="Keyword">import</a> <a id="24733" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24772" class="Keyword">open</a> <a id="24777" class="Keyword">import</a> <a id="24784" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24824" class="Keyword">open</a> <a id="24829" class="Keyword">import</a> <a id="24836" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="24879" class="Keyword">open</a> <a id="24884" class="Keyword">import</a> <a id="24891" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="24923" class="Keyword">open</a> <a id="24928" class="Keyword">import</a> <a id="24935" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="24971" class="Keyword">open</a> <a id="24976" class="Keyword">import</a> <a id="24983" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25012" class="Keyword">open</a> <a id="25017" class="Keyword">import</a> <a id="25024" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25057" class="Keyword">open</a> <a id="25062" class="Keyword">import</a> <a id="25069" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25105" class="Keyword">open</a> <a id="25110" class="Keyword">import</a> <a id="25117" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25146" class="Keyword">open</a> <a id="25151" class="Keyword">import</a> <a id="25158" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="25190" class="Keyword">open</a> <a id="25195" class="Keyword">import</a> <a id="25202" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25227" class="Keyword">open</a> <a id="25232" class="Keyword">import</a> <a id="25239" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25270" class="Keyword">open</a> <a id="25275" class="Keyword">import</a> <a id="25282" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25329" class="Keyword">open</a> <a id="25334" class="Keyword">import</a> <a id="25341" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25374" class="Keyword">open</a> <a id="25379" class="Keyword">import</a> <a id="25386" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25426" class="Keyword">open</a> <a id="25431" class="Keyword">import</a> <a id="25438" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25475" class="Keyword">open</a> <a id="25480" class="Keyword">import</a> <a id="25487" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="25523" class="Keyword">open</a> <a id="25528" class="Keyword">import</a> <a id="25535" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25567" class="Keyword">open</a> <a id="25572" class="Keyword">import</a> <a id="25579" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25606" class="Keyword">open</a> <a id="25611" class="Keyword">import</a> <a id="25618" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="25638" class="Keyword">open</a> <a id="25643" class="Keyword">import</a> <a id="25650" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="25677" class="Keyword">open</a> <a id="25682" class="Keyword">import</a> <a id="25689" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="25731" class="Keyword">open</a> <a id="25736" class="Keyword">import</a> <a id="25743" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="25790" class="Keyword">open</a> <a id="25795" class="Keyword">import</a> <a id="25802" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="25843" class="Keyword">open</a> <a id="25848" class="Keyword">import</a> <a id="25855" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="25889" class="Keyword">open</a> <a id="25894" class="Keyword">import</a> <a id="25901" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="25936" class="Keyword">open</a> <a id="25941" class="Keyword">import</a> <a id="25948" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="25986" class="Keyword">open</a> <a id="25991" class="Keyword">import</a> <a id="25998" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26030" class="Keyword">open</a> <a id="26035" class="Keyword">import</a> <a id="26042" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="26083" class="Keyword">open</a> <a id="26088" class="Keyword">import</a> <a id="26095" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="26136" class="Keyword">open</a> <a id="26141" class="Keyword">import</a> <a id="26148" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26188" class="Keyword">open</a> <a id="26193" class="Keyword">import</a> <a id="26200" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26233" class="Keyword">open</a> <a id="26238" class="Keyword">import</a> <a id="26245" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="26282" class="Keyword">open</a> <a id="26287" class="Keyword">import</a> <a id="26294" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="26324" class="Keyword">open</a> <a id="26329" class="Keyword">import</a> <a id="26336" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="26381" class="Keyword">open</a> <a id="26386" class="Keyword">import</a> <a id="26393" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="26421" class="Keyword">open</a> <a id="26426" class="Keyword">import</a> <a id="26433" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="26454" class="Keyword">open</a> <a id="26459" class="Keyword">import</a> <a id="26466" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="26500" class="Keyword">open</a> <a id="26505" class="Keyword">import</a> <a id="26512" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="26546" class="Keyword">open</a> <a id="26551" class="Keyword">import</a> <a id="26558" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="26593" class="Keyword">open</a> <a id="26598" class="Keyword">import</a> <a id="26605" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="26647" class="Keyword">open</a> <a id="26652" class="Keyword">import</a> <a id="26659" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="26694" class="Keyword">open</a> <a id="26699" class="Keyword">import</a> <a id="26706" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="26745" class="Keyword">open</a> <a id="26750" class="Keyword">import</a> <a id="26757" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="26794" class="Keyword">open</a> <a id="26799" class="Keyword">import</a> <a id="26806" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="26830" class="Keyword">open</a> <a id="26835" class="Keyword">import</a> <a id="26842" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="26867" class="Keyword">open</a> <a id="26872" class="Keyword">import</a> <a id="26879" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="26910" class="Keyword">open</a> <a id="26915" class="Keyword">import</a> <a id="26922" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="26973" class="Keyword">open</a> <a id="26978" class="Keyword">import</a> <a id="26985" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="27008" class="Keyword">open</a> <a id="27013" class="Keyword">import</a> <a id="27020" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="27068" class="Keyword">open</a> <a id="27073" class="Keyword">import</a> <a id="27080" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="27110" class="Keyword">open</a> <a id="27115" class="Keyword">import</a> <a id="27122" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="27192" class="Keyword">open</a> <a id="27197" class="Keyword">import</a> <a id="27204" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="27219" class="Keyword">open</a> <a id="27224" class="Keyword">import</a> <a id="27231" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="27264" class="Keyword">open</a> <a id="27269" class="Keyword">import</a> <a id="27276" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="27308" class="Keyword">open</a> <a id="27313" class="Keyword">import</a> <a id="27320" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="27362" class="Keyword">open</a> <a id="27367" class="Keyword">import</a> <a id="27374" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="27412" class="Keyword">open</a> <a id="27417" class="Keyword">import</a> <a id="27424" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="27461" class="Keyword">open</a> <a id="27466" class="Keyword">import</a> <a id="27473" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="27506" class="Keyword">open</a> <a id="27511" class="Keyword">import</a> <a id="27518" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="27542" class="Keyword">open</a> <a id="27547" class="Keyword">import</a> <a id="27554" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="27593" class="Keyword">open</a> <a id="27598" class="Keyword">import</a> <a id="27605" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="27651" class="Keyword">open</a> <a id="27656" class="Keyword">import</a> <a id="27663" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="27708" class="Keyword">open</a> <a id="27713" class="Keyword">import</a> <a id="27720" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="27758" class="Keyword">open</a> <a id="27763" class="Keyword">import</a> <a id="27770" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="27802" class="Keyword">open</a> <a id="27807" class="Keyword">import</a> <a id="27814" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="27867" class="Keyword">open</a> <a id="27872" class="Keyword">import</a> <a id="27879" href="order-theory.html" class="Module">order-theory</a>
<a id="27892" class="Keyword">open</a> <a id="27897" class="Keyword">import</a> <a id="27904" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="27931" class="Keyword">open</a> <a id="27936" class="Keyword">import</a> <a id="27943" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="27973" class="Keyword">open</a> <a id="27978" class="Keyword">import</a> <a id="27985" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="28018" class="Keyword">open</a> <a id="28023" class="Keyword">import</a> <a id="28030" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="28066" class="Keyword">open</a> <a id="28071" class="Keyword">import</a> <a id="28078" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="28113" class="Keyword">open</a> <a id="28118" class="Keyword">import</a> <a id="28125" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="28152" class="Keyword">open</a> <a id="28157" class="Keyword">import</a> <a id="28164" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="28194" class="Keyword">open</a> <a id="28199" class="Keyword">import</a> <a id="28206" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="28242" class="Keyword">open</a> <a id="28247" class="Keyword">import</a> <a id="28254" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="28296" class="Keyword">open</a> <a id="28301" class="Keyword">import</a> <a id="28308" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="28340" class="Keyword">open</a> <a id="28345" class="Keyword">import</a> <a id="28352" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="28383" class="Keyword">open</a> <a id="28388" class="Keyword">import</a> <a id="28395" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="28421" class="Keyword">open</a> <a id="28426" class="Keyword">import</a> <a id="28433" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="28462" class="Keyword">open</a> <a id="28467" class="Keyword">import</a> <a id="28474" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="28511" class="Keyword">open</a> <a id="28516" class="Keyword">import</a> <a id="28523" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="28563" class="Keyword">open</a> <a id="28568" class="Keyword">import</a> <a id="28575" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="28597" class="Keyword">open</a> <a id="28602" class="Keyword">import</a> <a id="28609" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="28644" class="Keyword">open</a> <a id="28649" class="Keyword">import</a> <a id="28656" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="28694" class="Keyword">open</a> <a id="28699" class="Keyword">import</a> <a id="28706" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="28745" class="Keyword">open</a> <a id="28750" class="Keyword">import</a> <a id="28757" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="28792" class="Keyword">open</a> <a id="28797" class="Keyword">import</a> <a id="28804" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="28839" class="Keyword">open</a> <a id="28844" class="Keyword">import</a> <a id="28851" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="28889" class="Keyword">open</a> <a id="28894" class="Keyword">import</a> <a id="28901" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="28932" class="Keyword">open</a> <a id="28937" class="Keyword">import</a> <a id="28944" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="28986" class="Keyword">open</a> <a id="28991" class="Keyword">import</a> <a id="28998" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="29043" class="Keyword">open</a> <a id="29048" class="Keyword">import</a> <a id="29055" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="29088" class="Keyword">open</a> <a id="29093" class="Keyword">import</a> <a id="29100" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="29120" class="Keyword">open</a> <a id="29125" class="Keyword">import</a> <a id="29132" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="29155" class="Keyword">open</a> <a id="29160" class="Keyword">import</a> <a id="29167" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="29190" class="Keyword">open</a> <a id="29195" class="Keyword">import</a> <a id="29202" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="29228" class="Keyword">open</a> <a id="29233" class="Keyword">import</a> <a id="29240" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="29266" class="Keyword">open</a> <a id="29271" class="Keyword">import</a> <a id="29278" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="29342" class="Keyword">open</a> <a id="29347" class="Keyword">import</a> <a id="29354" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="29372" class="Keyword">open</a> <a id="29377" class="Keyword">import</a> <a id="29384" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="29411" class="Keyword">open</a> <a id="29416" class="Keyword">import</a> <a id="29423" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="29481" class="Keyword">open</a> <a id="29486" class="Keyword">import</a> <a id="29493" href="polytopes.html" class="Module">polytopes</a>
<a id="29503" class="Keyword">open</a> <a id="29508" class="Keyword">import</a> <a id="29515" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="29573" class="Keyword">open</a> <a id="29578" class="Keyword">import</a> <a id="29585" href="ring-theory.html" class="Module">ring-theory</a>
<a id="29597" class="Keyword">open</a> <a id="29602" class="Keyword">import</a> <a id="29609" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="29646" class="Keyword">open</a> <a id="29651" class="Keyword">import</a> <a id="29658" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="29685" class="Keyword">open</a> <a id="29690" class="Keyword">import</a> <a id="29697" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="29729" class="Keyword">open</a> <a id="29734" class="Keyword">import</a> <a id="29741" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="29787" class="Keyword">open</a> <a id="29792" class="Keyword">import</a> <a id="29799" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="29824" class="Keyword">open</a> <a id="29829" class="Keyword">import</a> <a id="29836" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="29879" class="Keyword">open</a> <a id="29884" class="Keyword">import</a> <a id="29891" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="29929" class="Keyword">open</a> <a id="29934" class="Keyword">import</a> <a id="29941" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="29972" class="Keyword">open</a> <a id="29977" class="Keyword">import</a> <a id="29984" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="30008" class="Keyword">open</a> <a id="30013" class="Keyword">import</a> <a id="30020" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="30052" class="Keyword">open</a> <a id="30057" class="Keyword">import</a> <a id="30064" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="30090" class="Keyword">open</a> <a id="30095" class="Keyword">import</a> <a id="30102" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="30131" class="Keyword">open</a> <a id="30136" class="Keyword">import</a> <a id="30143" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="30180" class="Keyword">open</a> <a id="30185" class="Keyword">import</a> <a id="30192" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="30221" class="Keyword">open</a> <a id="30226" class="Keyword">import</a> <a id="30233" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="30260" class="Keyword">open</a> <a id="30265" class="Keyword">import</a> <a id="30272" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="30309" class="Keyword">open</a> <a id="30314" class="Keyword">import</a> <a id="30321" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="30348" class="Keyword">open</a> <a id="30353" class="Keyword">import</a> <a id="30360" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="30393" class="Keyword">open</a> <a id="30398" class="Keyword">import</a> <a id="30405" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="30423" class="Keyword">open</a> <a id="30428" class="Keyword">import</a> <a id="30435" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="30489" class="Keyword">open</a> <a id="30494" class="Keyword">import</a> <a id="30501" href="set-theory.html" class="Module">set-theory</a>
<a id="30512" class="Keyword">open</a> <a id="30517" class="Keyword">import</a> <a id="30524" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="30547" class="Keyword">open</a> <a id="30552" class="Keyword">import</a> <a id="30559" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="30583" class="Keyword">open</a> <a id="30588" class="Keyword">import</a> <a id="30595" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="30621" class="Keyword">open</a> <a id="30626" class="Keyword">import</a> <a id="30633" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="30695" class="Keyword">open</a> <a id="30700" class="Keyword">import</a> <a id="30707" href="structured-types.html" class="Module">structured-types</a>
<a id="30724" class="Keyword">open</a> <a id="30729" class="Keyword">import</a> <a id="30736" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="30771" class="Keyword">open</a> <a id="30776" class="Keyword">import</a> <a id="30783" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="30827" class="Keyword">open</a> <a id="30832" class="Keyword">import</a> <a id="30839" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="30903" class="Keyword">open</a> <a id="30908" class="Keyword">import</a> <a id="30915" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="30961" class="Keyword">open</a> <a id="30966" class="Keyword">import</a> <a id="30973" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="30997" class="Keyword">open</a> <a id="31002" class="Keyword">import</a> <a id="31009" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="31078" class="Keyword">open</a> <a id="31083" class="Keyword">import</a> <a id="31090" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="31135" class="Keyword">open</a> <a id="31140" class="Keyword">import</a> <a id="31147" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="31181" class="Keyword">open</a> <a id="31186" class="Keyword">import</a> <a id="31193" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="31254" class="Keyword">open</a> <a id="31259" class="Keyword">import</a> <a id="31266" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="31311" class="Keyword">open</a> <a id="31316" class="Keyword">import</a> <a id="31323" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="31361" class="Keyword">open</a> <a id="31366" class="Keyword">import</a> <a id="31373" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="31416" class="Keyword">open</a> <a id="31421" class="Keyword">import</a> <a id="31428" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="31464" class="Keyword">open</a> <a id="31469" class="Keyword">import</a> <a id="31476" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="31506" class="Keyword">open</a> <a id="31511" class="Keyword">import</a> <a id="31518" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="31549" class="Keyword">open</a> <a id="31554" class="Keyword">import</a> <a id="31561" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="31620" class="Keyword">open</a> <a id="31625" class="Keyword">import</a> <a id="31632" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="31683" class="Keyword">open</a> <a id="31688" class="Keyword">import</a> <a id="31695" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="31746" class="Keyword">open</a> <a id="31751" class="Keyword">import</a> <a id="31758" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="31813" class="Keyword">open</a> <a id="31818" class="Keyword">import</a> <a id="31825" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="31854" class="Keyword">open</a> <a id="31859" class="Keyword">import</a> <a id="31866" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="31894" class="Keyword">open</a> <a id="31899" class="Keyword">import</a> <a id="31906" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="31936" class="Keyword">open</a> <a id="31941" class="Keyword">import</a> <a id="31948" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="31982" class="Keyword">open</a> <a id="31987" class="Keyword">import</a> <a id="31994" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="32070" class="Keyword">open</a> <a id="32075" class="Keyword">import</a> <a id="32082" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="32108" class="Keyword">open</a> <a id="32113" class="Keyword">import</a> <a id="32120" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="32159" class="Keyword">open</a> <a id="32164" class="Keyword">import</a> <a id="32171" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="32209" class="Keyword">open</a> <a id="32214" class="Keyword">import</a> <a id="32221" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="32267" class="Keyword">open</a> <a id="32272" class="Keyword">import</a> <a id="32279" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="32316" class="Keyword">open</a> <a id="32321" class="Keyword">import</a> <a id="32328" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="32368" class="Keyword">open</a> <a id="32373" class="Keyword">import</a> <a id="32380" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="32419" class="Keyword">open</a> <a id="32424" class="Keyword">import</a> <a id="32431" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="32464" class="Keyword">open</a> <a id="32469" class="Keyword">import</a> <a id="32476" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="32511" class="Keyword">open</a> <a id="32516" class="Keyword">import</a> <a id="32523" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="32568" class="Keyword">open</a> <a id="32573" class="Keyword">import</a> <a id="32580" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="32632" class="Keyword">open</a> <a id="32637" class="Keyword">import</a> <a id="32644" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="32697" class="Keyword">open</a> <a id="32702" class="Keyword">import</a> <a id="32709" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="32757" class="Keyword">open</a> <a id="32762" class="Keyword">import</a> <a id="32769" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="32809" class="Keyword">open</a> <a id="32814" class="Keyword">import</a> <a id="32821" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="32868" class="Keyword">open</a> <a id="32873" class="Keyword">import</a> <a id="32880" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="32921" class="Keyword">open</a> <a id="32926" class="Keyword">import</a> <a id="32933" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="32971" class="Keyword">open</a> <a id="32976" class="Keyword">import</a> <a id="32983" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="33031" class="Keyword">open</a> <a id="33036" class="Keyword">import</a> <a id="33043" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="33088" class="Keyword">open</a> <a id="33093" class="Keyword">import</a> <a id="33100" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="33149" class="Keyword">open</a> <a id="33154" class="Keyword">import</a> <a id="33161" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="33238" class="Keyword">open</a> <a id="33243" class="Keyword">import</a> <a id="33250" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="33302" class="Keyword">open</a> <a id="33307" class="Keyword">import</a> <a id="33314" href="type-theories.html" class="Module">type-theories</a>
<a id="33328" class="Keyword">open</a> <a id="33333" class="Keyword">import</a> <a id="33340" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="33382" class="Keyword">open</a> <a id="33387" class="Keyword">import</a> <a id="33394" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="33432" class="Keyword">open</a> <a id="33437" class="Keyword">import</a> <a id="33444" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="33490" class="Keyword">open</a> <a id="33495" class="Keyword">import</a> <a id="33502" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="33549" class="Keyword">open</a> <a id="33554" class="Keyword">import</a> <a id="33561" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="33596" class="Keyword">open</a> <a id="33601" class="Keyword">import</a> <a id="33608" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="33686" class="Keyword">open</a> <a id="33691" class="Keyword">import</a> <a id="33698" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="33722" class="Keyword">open</a> <a id="33727" class="Keyword">import</a> <a id="33734" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="33787" class="Keyword">open</a> <a id="33792" class="Keyword">import</a> <a id="33799" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="33842" class="Keyword">open</a> <a id="33847" class="Keyword">import</a> <a id="33854" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="33894" class="Keyword">open</a> <a id="33899" class="Keyword">import</a> <a id="33906" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="33945" class="Keyword">open</a> <a id="33950" class="Keyword">import</a> <a id="33957" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="33991" class="Keyword">open</a> <a id="33996" class="Keyword">import</a> <a id="34003" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="34051" class="Keyword">open</a> <a id="34056" class="Keyword">import</a> <a id="34063" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="34114" class="Keyword">open</a> <a id="34119" class="Keyword">import</a> <a id="34126" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="34173" class="Keyword">open</a> <a id="34178" class="Keyword">import</a> <a id="34185" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="34237" class="Keyword">open</a> <a id="34242" class="Keyword">import</a> <a id="34249" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="34293" class="Keyword">open</a> <a id="34298" class="Keyword">import</a> <a id="34305" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="34345" class="Keyword">open</a> <a id="34350" class="Keyword">import</a> <a id="34357" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="34400" class="Keyword">open</a> <a id="34405" class="Keyword">import</a> <a id="34412" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="34464" class="Keyword">open</a> <a id="34469" class="Keyword">import</a> <a id="34476" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="34530" class="Keyword">open</a> <a id="34535" class="Keyword">import</a> <a id="34542" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="34590" class="Keyword">open</a> <a id="34595" class="Keyword">import</a> <a id="34602" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="34641" class="Keyword">open</a> <a id="34646" class="Keyword">import</a> <a id="34653" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="34686" class="Keyword">open</a> <a id="34691" class="Keyword">import</a> <a id="34698" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="34728" class="Keyword">open</a> <a id="34733" class="Keyword">import</a> <a id="34740" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="34791" class="Keyword">open</a> <a id="34796" class="Keyword">import</a> <a id="34803" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="34844" class="Keyword">open</a> <a id="34849" class="Keyword">import</a> <a id="34856" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="34893" class="Keyword">open</a> <a id="34898" class="Keyword">import</a> <a id="34905" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="34964" class="Keyword">open</a> <a id="34969" class="Keyword">import</a> <a id="34976" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="35031" class="Keyword">open</a> <a id="35036" class="Keyword">import</a> <a id="35043" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="35099" class="Keyword">open</a> <a id="35104" class="Keyword">import</a> <a id="35111" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="35158" class="Keyword">open</a> <a id="35163" class="Keyword">import</a> <a id="35170" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="35213" class="Keyword">open</a> <a id="35218" class="Keyword">import</a> <a id="35225" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="35270" class="Keyword">open</a> <a id="35275" class="Keyword">import</a> <a id="35282" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="35331" class="Keyword">open</a> <a id="35336" class="Keyword">import</a> <a id="35343" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="35394" class="Keyword">open</a> <a id="35399" class="Keyword">import</a> <a id="35406" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="35450" class="Keyword">open</a> <a id="35455" class="Keyword">import</a> <a id="35462" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="35540" class="Keyword">open</a> <a id="35545" class="Keyword">import</a> <a id="35552" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="35592" class="Keyword">open</a> <a id="35597" class="Keyword">import</a> <a id="35604" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="35661" class="Keyword">open</a> <a id="35666" class="Keyword">import</a> <a id="35673" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="35708" class="Keyword">open</a> <a id="35713" class="Keyword">import</a> <a id="35720" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="35766" class="Keyword">open</a> <a id="35771" class="Keyword">import</a> <a id="35778" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="35833" class="Keyword">open</a> <a id="35838" class="Keyword">import</a> <a id="35845" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="35888" class="Keyword">open</a> <a id="35893" class="Keyword">import</a> <a id="35900" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="35945" class="Keyword">open</a> <a id="35950" class="Keyword">import</a> <a id="35957" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="36016" class="Keyword">open</a> <a id="36021" class="Keyword">import</a> <a id="36028" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="36065" class="Keyword">open</a> <a id="36070" class="Keyword">import</a> <a id="36077" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="36119" class="Keyword">open</a> <a id="36124" class="Keyword">import</a> <a id="36131" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="36172" class="Keyword">open</a> <a id="36177" class="Keyword">import</a> <a id="36184" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="36223" class="Keyword">open</a> <a id="36228" class="Keyword">import</a> <a id="36235" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="36273" class="Keyword">open</a> <a id="36278" class="Keyword">import</a> <a id="36285" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="36337" class="Keyword">open</a> <a id="36342" class="Keyword">import</a> <a id="36349" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="36394" class="Keyword">open</a> <a id="36399" class="Keyword">import</a> <a id="36406" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="36445" class="Keyword">open</a> <a id="36450" class="Keyword">import</a> <a id="36457" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="36494" class="Keyword">open</a> <a id="36499" class="Keyword">import</a> <a id="36506" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="36555" class="Keyword">open</a> <a id="36560" class="Keyword">import</a> <a id="36567" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="36606" class="Keyword">open</a> <a id="36611" class="Keyword">import</a> <a id="36618" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="36656" class="Keyword">open</a> <a id="36661" class="Keyword">import</a> <a id="36668" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="36723" class="Keyword">open</a> <a id="36728" class="Keyword">import</a> <a id="36735" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="36774" class="Keyword">open</a> <a id="36779" class="Keyword">import</a> <a id="36786" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="36834" class="Keyword">open</a> <a id="36839" class="Keyword">import</a> <a id="36846" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="36893" class="Keyword">open</a> <a id="36898" class="Keyword">import</a> <a id="36905" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="36943" class="Keyword">open</a> <a id="36948" class="Keyword">import</a> <a id="36955" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="36985" class="Keyword">open</a> <a id="36990" class="Keyword">import</a> <a id="36997" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="37054" class="Keyword">open</a> <a id="37059" class="Keyword">import</a> <a id="37066" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="37120" class="Keyword">open</a> <a id="37125" class="Keyword">import</a> <a id="37132" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="37162" class="Keyword">open</a> <a id="37167" class="Keyword">import</a> <a id="37174" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="37223" class="Keyword">open</a> <a id="37228" class="Keyword">import</a> <a id="37235" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="37277" class="Keyword">open</a> <a id="37282" class="Keyword">import</a> <a id="37289" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="37323" class="Keyword">open</a> <a id="37328" class="Keyword">import</a> <a id="37335" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="37398" class="Keyword">open</a> <a id="37403" class="Keyword">import</a> <a id="37410" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="37453" class="Keyword">open</a> <a id="37458" class="Keyword">import</a> <a id="37465" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="37500" class="Keyword">open</a> <a id="37505" class="Keyword">import</a> <a id="37512" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="37547" class="Keyword">open</a> <a id="37552" class="Keyword">import</a> <a id="37559" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="37599" class="Keyword">open</a> <a id="37604" class="Keyword">import</a> <a id="37611" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="37656" class="Keyword">open</a> <a id="37661" class="Keyword">import</a> <a id="37668" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="37709" class="Keyword">open</a> <a id="37714" class="Keyword">import</a> <a id="37721" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="37775" class="Keyword">open</a> <a id="37780" class="Keyword">import</a> <a id="37787" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="37837" class="Keyword">open</a> <a id="37842" class="Keyword">import</a> <a id="37849" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="37896" class="Keyword">open</a> <a id="37901" class="Keyword">import</a> <a id="37908" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="37946" class="Keyword">open</a> <a id="37951" class="Keyword">import</a> <a id="37958" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="38007" class="Keyword">open</a> <a id="38012" class="Keyword">import</a> <a id="38019" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="38066" class="Keyword">open</a> <a id="38071" class="Keyword">import</a> <a id="38078" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="38141" class="Keyword">open</a> <a id="38146" class="Keyword">import</a> <a id="38153" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="38185" class="Keyword">open</a> <a id="38190" class="Keyword">import</a> <a id="38197" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="38250" class="Keyword">open</a> <a id="38255" class="Keyword">import</a> <a id="38262" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="38308" class="Keyword">open</a> <a id="38313" class="Keyword">import</a> <a id="38320" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="38366" class="Keyword">open</a> <a id="38371" class="Keyword">import</a> <a id="38378" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="38426" class="Keyword">open</a> <a id="38431" class="Keyword">import</a> <a id="38438" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="38478" class="Keyword">open</a> <a id="38483" class="Keyword">import</a> <a id="38490" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="38535" class="Keyword">open</a> <a id="38540" class="Keyword">import</a> <a id="38547" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="38612" class="Keyword">open</a> <a id="38617" class="Keyword">import</a> <a id="38624" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="38669" class="Keyword">open</a> <a id="38674" class="Keyword">import</a> <a id="38681" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="38728" class="Keyword">open</a> <a id="38733" class="Keyword">import</a> <a id="38740" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="38793" class="Keyword">open</a> <a id="38798" class="Keyword">import</a> <a id="38805" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>