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
<a id="10834" class="Keyword">open</a> <a id="10839" class="Keyword">import</a> <a id="10846" href="finite-group-theory.simpson-delooping-sign-homomorphism.html" class="Module">finite-group-theory.simpson-delooping-sign-homomorphism</a>
<a id="10902" class="Keyword">open</a> <a id="10907" class="Keyword">import</a> <a id="10914" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="10956" class="Keyword">open</a> <a id="10961" class="Keyword">import</a> <a id="10968" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="11031" class="Keyword">open</a> <a id="11036" class="Keyword">import</a> <a id="11043" href="foundation.html" class="Module">foundation</a>
<a id="11054" class="Keyword">open</a> <a id="11059" class="Keyword">import</a> <a id="11066" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11084" class="Keyword">open</a> <a id="11089" class="Keyword">import</a> <a id="11096" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11115" class="Keyword">open</a> <a id="11120" class="Keyword">import</a> <a id="11127" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11146" class="Keyword">open</a> <a id="11151" class="Keyword">import</a> <a id="11158" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11202" class="Keyword">open</a> <a id="11207" class="Keyword">import</a> <a id="11214" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11239" class="Keyword">open</a> <a id="11244" class="Keyword">import</a> <a id="11251" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11278" class="Keyword">open</a> <a id="11283" class="Keyword">import</a> <a id="11290" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11307" class="Keyword">open</a> <a id="11312" class="Keyword">import</a> <a id="11319" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11348" class="Keyword">open</a> <a id="11353" class="Keyword">import</a> <a id="11360" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11416" class="Keyword">open</a> <a id="11421" class="Keyword">import</a> <a id="11428" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11459" class="Keyword">open</a> <a id="11464" class="Keyword">import</a> <a id="11471" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11525" class="Keyword">open</a> <a id="11530" class="Keyword">import</a> <a id="11537" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11565" class="Keyword">open</a> <a id="11570" class="Keyword">import</a> <a id="11577" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11607" class="Keyword">open</a> <a id="11612" class="Keyword">import</a> <a id="11619" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11639" class="Keyword">open</a> <a id="11644" class="Keyword">import</a> <a id="11651" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11696" class="Keyword">open</a> <a id="11701" class="Keyword">import</a> <a id="11708" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11745" class="Keyword">open</a> <a id="11750" class="Keyword">import</a> <a id="11757" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11792" class="Keyword">open</a> <a id="11797" class="Keyword">import</a> <a id="11804" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11862" class="Keyword">open</a> <a id="11867" class="Keyword">import</a> <a id="11874" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11912" class="Keyword">open</a> <a id="11917" class="Keyword">import</a> <a id="11924" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11958" class="Keyword">open</a> <a id="11963" class="Keyword">import</a> <a id="11970" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11999" class="Keyword">open</a> <a id="12004" class="Keyword">import</a> <a id="12011" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12034" class="Keyword">open</a> <a id="12039" class="Keyword">import</a> <a id="12046" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12073" class="Keyword">open</a> <a id="12078" class="Keyword">import</a> <a id="12085" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12108" class="Keyword">open</a> <a id="12113" class="Keyword">import</a> <a id="12120" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12162" class="Keyword">open</a> <a id="12167" class="Keyword">import</a> <a id="12174" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12206" class="Keyword">open</a> <a id="12211" class="Keyword">import</a> <a id="12218" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12245" class="Keyword">open</a> <a id="12250" class="Keyword">import</a> <a id="12257" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12282" class="Keyword">open</a> <a id="12287" class="Keyword">import</a> <a id="12294" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12323" class="Keyword">open</a> <a id="12328" class="Keyword">import</a> <a id="12335" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12365" class="Keyword">open</a> <a id="12370" class="Keyword">import</a> <a id="12377" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12404" class="Keyword">open</a> <a id="12409" class="Keyword">import</a> <a id="12416" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12435" class="Keyword">open</a> <a id="12440" class="Keyword">import</a> <a id="12447" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12493" class="Keyword">open</a> <a id="12498" class="Keyword">import</a> <a id="12505" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12547" class="Keyword">open</a> <a id="12552" class="Keyword">import</a> <a id="12559" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12591" class="Keyword">open</a> <a id="12596" class="Keyword">import</a> <a id="12603" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12633" class="Keyword">open</a> <a id="12638" class="Keyword">import</a> <a id="12645" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="12688" class="Keyword">open</a> <a id="12693" class="Keyword">import</a> <a id="12700" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12726" class="Keyword">open</a> <a id="12731" class="Keyword">import</a> <a id="12738" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12772" class="Keyword">open</a> <a id="12777" class="Keyword">import</a> <a id="12784" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="12815" class="Keyword">open</a> <a id="12820" class="Keyword">import</a> <a id="12827" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12857" class="Keyword">open</a> <a id="12862" class="Keyword">import</a> <a id="12869" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12896" class="Keyword">open</a> <a id="12901" class="Keyword">import</a> <a id="12908" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="12946" class="Keyword">open</a> <a id="12951" class="Keyword">import</a> <a id="12958" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12990" class="Keyword">open</a> <a id="12995" class="Keyword">import</a> <a id="13002" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13036" class="Keyword">open</a> <a id="13041" class="Keyword">import</a> <a id="13048" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13071" class="Keyword">open</a> <a id="13076" class="Keyword">import</a> <a id="13083" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13110" class="Keyword">open</a> <a id="13115" class="Keyword">import</a> <a id="13122" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13150" class="Keyword">open</a> <a id="13155" class="Keyword">import</a> <a id="13162" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13199" class="Keyword">open</a> <a id="13204" class="Keyword">import</a> <a id="13211" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13259" class="Keyword">open</a> <a id="13264" class="Keyword">import</a> <a id="13271" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13311" class="Keyword">open</a> <a id="13316" class="Keyword">import</a> <a id="13323" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13345" class="Keyword">open</a> <a id="13350" class="Keyword">import</a> <a id="13357" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13380" class="Keyword">open</a> <a id="13385" class="Keyword">import</a> <a id="13392" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13417" class="Keyword">open</a> <a id="13422" class="Keyword">import</a> <a id="13429" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13474" class="Keyword">open</a> <a id="13479" class="Keyword">import</a> <a id="13486" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13530" class="Keyword">open</a> <a id="13535" class="Keyword">import</a> <a id="13542" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13578" class="Keyword">open</a> <a id="13583" class="Keyword">import</a> <a id="13590" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13635" class="Keyword">open</a> <a id="13640" class="Keyword">import</a> <a id="13647" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13688" class="Keyword">open</a> <a id="13693" class="Keyword">import</a> <a id="13700" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13735" class="Keyword">open</a> <a id="13740" class="Keyword">import</a> <a id="13747" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13779" class="Keyword">open</a> <a id="13784" class="Keyword">import</a> <a id="13791" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13822" class="Keyword">open</a> <a id="13827" class="Keyword">import</a> <a id="13834" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13867" class="Keyword">open</a> <a id="13872" class="Keyword">import</a> <a id="13879" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13912" class="Keyword">open</a> <a id="13917" class="Keyword">import</a> <a id="13924" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13954" class="Keyword">open</a> <a id="13959" class="Keyword">import</a> <a id="13966" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13990" class="Keyword">open</a> <a id="13995" class="Keyword">import</a> <a id="14002" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14040" class="Keyword">open</a> <a id="14045" class="Keyword">import</a> <a id="14052" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14083" class="Keyword">open</a> <a id="14088" class="Keyword">import</a> <a id="14095" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14120" class="Keyword">open</a> <a id="14125" class="Keyword">import</a> <a id="14132" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14160" class="Keyword">open</a> <a id="14165" class="Keyword">import</a> <a id="14172" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14196" class="Keyword">open</a> <a id="14201" class="Keyword">import</a> <a id="14208" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14234" class="Keyword">open</a> <a id="14239" class="Keyword">import</a> <a id="14246" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14281" class="Keyword">open</a> <a id="14286" class="Keyword">import</a> <a id="14293" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14314" class="Keyword">open</a> <a id="14319" class="Keyword">import</a> <a id="14326" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14375" class="Keyword">open</a> <a id="14380" class="Keyword">import</a> <a id="14387" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14428" class="Keyword">open</a> <a id="14433" class="Keyword">import</a> <a id="14440" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14490" class="Keyword">open</a> <a id="14495" class="Keyword">import</a> <a id="14502" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14548" class="Keyword">open</a> <a id="14553" class="Keyword">import</a> <a id="14560" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14600" class="Keyword">open</a> <a id="14605" class="Keyword">import</a> <a id="14612" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14662" class="Keyword">open</a> <a id="14667" class="Keyword">import</a> <a id="14674" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14713" class="Keyword">open</a> <a id="14718" class="Keyword">import</a> <a id="14725" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14765" class="Keyword">open</a> <a id="14770" class="Keyword">import</a> <a id="14777" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14810" class="Keyword">open</a> <a id="14815" class="Keyword">import</a> <a id="14822" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14871" class="Keyword">open</a> <a id="14876" class="Keyword">import</a> <a id="14883" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14908" class="Keyword">open</a> <a id="14913" class="Keyword">import</a> <a id="14920" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14958" class="Keyword">open</a> <a id="14963" class="Keyword">import</a> <a id="14970" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14992" class="Keyword">open</a> <a id="14997" class="Keyword">import</a> <a id="15004" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15032" class="Keyword">open</a> <a id="15037" class="Keyword">import</a> <a id="15044" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15080" class="Keyword">open</a> <a id="15085" class="Keyword">import</a> <a id="15092" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15118" class="Keyword">open</a> <a id="15123" class="Keyword">import</a> <a id="15130" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15148" class="Keyword">open</a> <a id="15153" class="Keyword">import</a> <a id="15160" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15195" class="Keyword">open</a> <a id="15200" class="Keyword">import</a> <a id="15207" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15242" class="Keyword">open</a> <a id="15247" class="Keyword">import</a> <a id="15254" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15281" class="Keyword">open</a> <a id="15286" class="Keyword">import</a> <a id="15293" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15349" class="Keyword">open</a> <a id="15354" class="Keyword">import</a> <a id="15361" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15390" class="Keyword">open</a> <a id="15395" class="Keyword">import</a> <a id="15402" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15432" class="Keyword">open</a> <a id="15437" class="Keyword">import</a> <a id="15444" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15471" class="Keyword">open</a> <a id="15476" class="Keyword">import</a> <a id="15483" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15509" class="Keyword">open</a> <a id="15514" class="Keyword">import</a> <a id="15521" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15548" class="Keyword">open</a> <a id="15553" class="Keyword">import</a> <a id="15560" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15584" class="Keyword">open</a> <a id="15589" class="Keyword">import</a> <a id="15596" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15619" class="Keyword">open</a> <a id="15624" class="Keyword">import</a> <a id="15631" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15658" class="Keyword">open</a> <a id="15663" class="Keyword">import</a> <a id="15670" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15702" class="Keyword">open</a> <a id="15707" class="Keyword">import</a> <a id="15714" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15749" class="Keyword">open</a> <a id="15754" class="Keyword">import</a> <a id="15761" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15792" class="Keyword">open</a> <a id="15797" class="Keyword">import</a> <a id="15804" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15837" class="Keyword">open</a> <a id="15842" class="Keyword">import</a> <a id="15849" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15883" class="Keyword">open</a> <a id="15888" class="Keyword">import</a> <a id="15895" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15935" class="Keyword">open</a> <a id="15940" class="Keyword">import</a> <a id="15947" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15978" class="Keyword">open</a> <a id="15983" class="Keyword">import</a> <a id="15990" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16022" class="Keyword">open</a> <a id="16027" class="Keyword">import</a> <a id="16034" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16065" class="Keyword">open</a> <a id="16070" class="Keyword">import</a> <a id="16077" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16094" class="Keyword">open</a> <a id="16099" class="Keyword">import</a> <a id="16106" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16131" class="Keyword">open</a> <a id="16136" class="Keyword">import</a> <a id="16143" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16172" class="Keyword">open</a> <a id="16177" class="Keyword">import</a> <a id="16184" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16209" class="Keyword">open</a> <a id="16214" class="Keyword">import</a> <a id="16221" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16242" class="Keyword">open</a> <a id="16247" class="Keyword">import</a> <a id="16254" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16278" class="Keyword">open</a> <a id="16283" class="Keyword">import</a> <a id="16290" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16310" class="Keyword">open</a> <a id="16315" class="Keyword">import</a> <a id="16322" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16356" class="Keyword">open</a> <a id="16361" class="Keyword">import</a> <a id="16368" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16406" class="Keyword">open</a> <a id="16411" class="Keyword">import</a> <a id="16418" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16446" class="Keyword">open</a> <a id="16451" class="Keyword">import</a> <a id="16458" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16482" class="Keyword">open</a> <a id="16487" class="Keyword">import</a> <a id="16494" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16521" class="Keyword">open</a> <a id="16526" class="Keyword">import</a> <a id="16533" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16568" class="Keyword">open</a> <a id="16573" class="Keyword">import</a> <a id="16580" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16601" class="Keyword">open</a> <a id="16606" class="Keyword">import</a> <a id="16613" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16649" class="Keyword">open</a> <a id="16654" class="Keyword">import</a> <a id="16661" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16706" class="Keyword">open</a> <a id="16711" class="Keyword">import</a> <a id="16718" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16764" class="Keyword">open</a> <a id="16769" class="Keyword">import</a> <a id="16776" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16816" class="Keyword">open</a> <a id="16821" class="Keyword">import</a> <a id="16828" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16858" class="Keyword">open</a> <a id="16863" class="Keyword">import</a> <a id="16870" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="16904" class="Keyword">open</a> <a id="16909" class="Keyword">import</a> <a id="16916" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16953" class="Keyword">open</a> <a id="16958" class="Keyword">import</a> <a id="16965" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16989" class="Keyword">open</a> <a id="16994" class="Keyword">import</a> <a id="17001" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17022" class="Keyword">open</a> <a id="17027" class="Keyword">import</a> <a id="17034" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17069" class="Keyword">open</a> <a id="17074" class="Keyword">import</a> <a id="17081" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17118" class="Keyword">open</a> <a id="17123" class="Keyword">import</a> <a id="17130" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17179" class="Keyword">open</a> <a id="17184" class="Keyword">import</a> <a id="17191" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17224" class="Keyword">open</a> <a id="17229" class="Keyword">import</a> <a id="17236" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17259" class="Keyword">open</a> <a id="17264" class="Keyword">import</a> <a id="17271" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17294" class="Keyword">open</a> <a id="17299" class="Keyword">import</a> <a id="17306" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17329" class="Keyword">open</a> <a id="17334" class="Keyword">import</a> <a id="17341" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17369" class="Keyword">open</a> <a id="17374" class="Keyword">import</a> <a id="17381" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17401" class="Keyword">open</a> <a id="17406" class="Keyword">import</a> <a id="17413" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17434" class="Keyword">open</a> <a id="17439" class="Keyword">import</a> <a id="17446" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17477" class="Keyword">open</a> <a id="17482" class="Keyword">import</a> <a id="17489" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17516" class="Keyword">open</a> <a id="17521" class="Keyword">import</a> <a id="17528" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17544" class="Keyword">open</a> <a id="17549" class="Keyword">import</a> <a id="17556" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17587" class="Keyword">open</a> <a id="17592" class="Keyword">import</a> <a id="17599" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17616" class="Keyword">open</a> <a id="17621" class="Keyword">import</a> <a id="17628" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17650" class="Keyword">open</a> <a id="17655" class="Keyword">import</a> <a id="17662" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17689" class="Keyword">open</a> <a id="17694" class="Keyword">import</a> <a id="17701" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17724" class="Keyword">open</a> <a id="17729" class="Keyword">import</a> <a id="17736" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17763" class="Keyword">open</a> <a id="17768" class="Keyword">import</a> <a id="17775" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17808" class="Keyword">open</a> <a id="17813" class="Keyword">import</a> <a id="17820" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17860" class="Keyword">open</a> <a id="17865" class="Keyword">import</a> <a id="17872" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17893" class="Keyword">open</a> <a id="17898" class="Keyword">import</a> <a id="17905" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17934" class="Keyword">open</a> <a id="17939" class="Keyword">import</a> <a id="17946" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17984" class="Keyword">open</a> <a id="17989" class="Keyword">import</a> <a id="17996" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18016" class="Keyword">open</a> <a id="18021" class="Keyword">import</a> <a id="18028" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18052" class="Keyword">open</a> <a id="18057" class="Keyword">import</a> <a id="18064" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18091" class="Keyword">open</a> <a id="18096" class="Keyword">import</a> <a id="18103" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18135" class="Keyword">open</a> <a id="18140" class="Keyword">import</a> <a id="18147" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18177" class="Keyword">open</a> <a id="18182" class="Keyword">import</a> <a id="18189" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18215" class="Keyword">open</a> <a id="18220" class="Keyword">import</a> <a id="18227" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18254" class="Keyword">open</a> <a id="18259" class="Keyword">import</a> <a id="18266" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18295" class="Keyword">open</a> <a id="18300" class="Keyword">import</a> <a id="18307" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18330" class="Keyword">open</a> <a id="18335" class="Keyword">import</a> <a id="18342" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18393" class="Keyword">open</a> <a id="18398" class="Keyword">import</a> <a id="18405" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18448" class="Keyword">open</a> <a id="18453" class="Keyword">import</a> <a id="18460" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18508" class="Keyword">open</a> <a id="18513" class="Keyword">import</a> <a id="18520" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18558" class="Keyword">open</a> <a id="18563" class="Keyword">import</a> <a id="18570" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18607" class="Keyword">open</a> <a id="18612" class="Keyword">import</a> <a id="18619" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18665" class="Keyword">open</a> <a id="18670" class="Keyword">import</a> <a id="18677" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18694" class="Keyword">open</a> <a id="18699" class="Keyword">import</a> <a id="18706" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18734" class="Keyword">open</a> <a id="18739" class="Keyword">import</a> <a id="18746" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18774" class="Keyword">open</a> <a id="18779" class="Keyword">import</a> <a id="18786" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18822" class="Keyword">open</a> <a id="18827" class="Keyword">import</a> <a id="18834" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18872" class="Keyword">open</a> <a id="18877" class="Keyword">import</a> <a id="18884" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18917" class="Keyword">open</a> <a id="18922" class="Keyword">import</a> <a id="18929" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18950" class="Keyword">open</a> <a id="18955" class="Keyword">import</a> <a id="18962" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="18998" class="Keyword">open</a> <a id="19003" class="Keyword">import</a> <a id="19010" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19064" class="Keyword">open</a> <a id="19069" class="Keyword">import</a> <a id="19076" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19098" class="Keyword">open</a> <a id="19103" class="Keyword">import</a> <a id="19110" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19145" class="Keyword">open</a> <a id="19150" class="Keyword">import</a> <a id="19157" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19187" class="Keyword">open</a> <a id="19192" class="Keyword">import</a> <a id="19199" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19238" class="Keyword">open</a> <a id="19243" class="Keyword">import</a> <a id="19250" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19304" class="Keyword">open</a> <a id="19309" class="Keyword">import</a> <a id="19316" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19362" class="Keyword">open</a> <a id="19367" class="Keyword">import</a> <a id="19374" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19425" class="Keyword">open</a> <a id="19430" class="Keyword">import</a> <a id="19437" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19478" class="Keyword">open</a> <a id="19483" class="Keyword">import</a> <a id="19490" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19535" class="Keyword">open</a> <a id="19540" class="Keyword">import</a> <a id="19547" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19592" class="Keyword">open</a> <a id="19597" class="Keyword">import</a> <a id="19604" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19640" class="Keyword">open</a> <a id="19645" class="Keyword">import</a> <a id="19652" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19688" class="Keyword">open</a> <a id="19693" class="Keyword">import</a> <a id="19700" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19765" class="Keyword">open</a> <a id="19770" class="Keyword">import</a> <a id="19777" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19832" class="Keyword">open</a> <a id="19837" class="Keyword">import</a> <a id="19844" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19884" class="Keyword">open</a> <a id="19889" class="Keyword">import</a> <a id="19896" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19940" class="Keyword">open</a> <a id="19945" class="Keyword">import</a> <a id="19952" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19997" class="Keyword">open</a> <a id="20002" class="Keyword">import</a> <a id="20009" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20050" class="Keyword">open</a> <a id="20055" class="Keyword">import</a> <a id="20062" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20102" class="Keyword">open</a> <a id="20107" class="Keyword">import</a> <a id="20114" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20141" class="Keyword">open</a> <a id="20146" class="Keyword">import</a> <a id="20153" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20189" class="Keyword">open</a> <a id="20194" class="Keyword">import</a> <a id="20201" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20228" class="Keyword">open</a> <a id="20233" class="Keyword">import</a> <a id="20240" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20277" class="Keyword">open</a> <a id="20282" class="Keyword">import</a> <a id="20289" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20317" class="Keyword">open</a> <a id="20322" class="Keyword">import</a> <a id="20329" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20348" class="Keyword">open</a> <a id="20353" class="Keyword">import</a> <a id="20360" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20400" class="Keyword">open</a> <a id="20405" class="Keyword">import</a> <a id="20412" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20444" class="Keyword">open</a> <a id="20449" class="Keyword">import</a> <a id="20456" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20504" class="Keyword">open</a> <a id="20509" class="Keyword">import</a> <a id="20516" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20539" class="Keyword">open</a> <a id="20544" class="Keyword">import</a> <a id="20551" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20575" class="Keyword">open</a> <a id="20580" class="Keyword">import</a> <a id="20587" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20627" class="Keyword">open</a> <a id="20632" class="Keyword">import</a> <a id="20639" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20682" class="Keyword">open</a> <a id="20687" class="Keyword">import</a> <a id="20694" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20728" class="Keyword">open</a> <a id="20733" class="Keyword">import</a> <a id="20740" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20772" class="Keyword">open</a> <a id="20777" class="Keyword">import</a> <a id="20784" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20814" class="Keyword">open</a> <a id="20819" class="Keyword">import</a> <a id="20826" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20860" class="Keyword">open</a> <a id="20865" class="Keyword">import</a> <a id="20872" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20907" class="Keyword">open</a> <a id="20912" class="Keyword">import</a> <a id="20919" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20956" class="Keyword">open</a> <a id="20961" class="Keyword">import</a> <a id="20968" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20995" class="Keyword">open</a> <a id="21000" class="Keyword">import</a> <a id="21007" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21035" class="Keyword">open</a> <a id="21040" class="Keyword">import</a> <a id="21047" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21096" class="Keyword">open</a> <a id="21101" class="Keyword">import</a> <a id="21108" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21154" class="Keyword">open</a> <a id="21159" class="Keyword">import</a> <a id="21166" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21206" class="Keyword">open</a> <a id="21211" class="Keyword">import</a> <a id="21218" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21256" class="Keyword">open</a> <a id="21261" class="Keyword">import</a> <a id="21268" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21297" class="Keyword">open</a> <a id="21302" class="Keyword">import</a> <a id="21309" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21339" class="Keyword">open</a> <a id="21344" class="Keyword">import</a> <a id="21351" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21382" class="Keyword">open</a> <a id="21387" class="Keyword">import</a> <a id="21394" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21434" class="Keyword">open</a> <a id="21439" class="Keyword">import</a> <a id="21446" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21472" class="Keyword">open</a> <a id="21477" class="Keyword">import</a> <a id="21484" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21539" class="Keyword">open</a> <a id="21544" class="Keyword">import</a> <a id="21551" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21602" class="Keyword">open</a> <a id="21607" class="Keyword">import</a> <a id="21614" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21659" class="Keyword">open</a> <a id="21664" class="Keyword">import</a> <a id="21671" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21725" class="Keyword">open</a> <a id="21730" class="Keyword">import</a> <a id="21737" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21764" class="Keyword">open</a> <a id="21769" class="Keyword">import</a> <a id="21776" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21809" class="Keyword">open</a> <a id="21814" class="Keyword">import</a> <a id="21821" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21852" class="Keyword">open</a> <a id="21857" class="Keyword">import</a> <a id="21864" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21901" class="Keyword">open</a> <a id="21906" class="Keyword">import</a> <a id="21913" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21938" class="Keyword">open</a> <a id="21943" class="Keyword">import</a> <a id="21950" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21982" class="Keyword">open</a> <a id="21987" class="Keyword">import</a> <a id="21994" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22029" class="Keyword">open</a> <a id="22034" class="Keyword">import</a> <a id="22041" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22070" class="Keyword">open</a> <a id="22075" class="Keyword">import</a> <a id="22082" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22108" class="Keyword">open</a> <a id="22113" class="Keyword">import</a> <a id="22120" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22148" class="Keyword">open</a> <a id="22153" class="Keyword">import</a> <a id="22160" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22185" class="Keyword">open</a> <a id="22190" class="Keyword">import</a> <a id="22197" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22218" class="Keyword">open</a> <a id="22223" class="Keyword">import</a> <a id="22230" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22266" class="Keyword">open</a> <a id="22271" class="Keyword">import</a> <a id="22278" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22321" class="Keyword">open</a> <a id="22326" class="Keyword">import</a> <a id="22333" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22358" class="Keyword">open</a> <a id="22363" class="Keyword">import</a> <a id="22370" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22401" class="Keyword">open</a> <a id="22406" class="Keyword">import</a> <a id="22413" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22445" class="Keyword">open</a> <a id="22450" class="Keyword">import</a> <a id="22457" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22491" class="Keyword">open</a> <a id="22496" class="Keyword">import</a> <a id="22503" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22559" class="Keyword">open</a> <a id="22564" class="Keyword">import</a> <a id="22571" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22624" class="Keyword">open</a> <a id="22629" class="Keyword">import</a> <a id="22636" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22663" class="Keyword">open</a> <a id="22668" class="Keyword">import</a> <a id="22675" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22720" class="Keyword">open</a> <a id="22725" class="Keyword">import</a> <a id="22732" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22794" class="Keyword">open</a> <a id="22799" class="Keyword">import</a> <a id="22806" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22819" class="Keyword">open</a> <a id="22824" class="Keyword">import</a> <a id="22831" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="22871" class="Keyword">open</a> <a id="22876" class="Keyword">import</a> <a id="22883" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="22927" class="Keyword">open</a> <a id="22932" class="Keyword">import</a> <a id="22939" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="22978" class="Keyword">open</a> <a id="22983" class="Keyword">import</a> <a id="22990" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23032" class="Keyword">open</a> <a id="23037" class="Keyword">import</a> <a id="23044" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23084" class="Keyword">open</a> <a id="23089" class="Keyword">import</a> <a id="23096" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23137" class="Keyword">open</a> <a id="23142" class="Keyword">import</a> <a id="23149" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23187" class="Keyword">open</a> <a id="23192" class="Keyword">import</a> <a id="23199" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23262" class="Keyword">open</a> <a id="23267" class="Keyword">import</a> <a id="23274" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23303" class="Keyword">open</a> <a id="23308" class="Keyword">import</a> <a id="23315" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23360" class="Keyword">open</a> <a id="23365" class="Keyword">import</a> <a id="23372" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23414" class="Keyword">open</a> <a id="23419" class="Keyword">import</a> <a id="23426" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23470" class="Keyword">open</a> <a id="23475" class="Keyword">import</a> <a id="23482" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23531" class="Keyword">open</a> <a id="23536" class="Keyword">import</a> <a id="23543" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23593" class="Keyword">open</a> <a id="23598" class="Keyword">import</a> <a id="23605" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23632" class="Keyword">open</a> <a id="23637" class="Keyword">import</a> <a id="23644" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23685" class="Keyword">open</a> <a id="23690" class="Keyword">import</a> <a id="23697" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23720" class="Keyword">open</a> <a id="23725" class="Keyword">import</a> <a id="23732" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23781" class="Keyword">open</a> <a id="23786" class="Keyword">import</a> <a id="23793" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23832" class="Keyword">open</a> <a id="23837" class="Keyword">import</a> <a id="23844" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="23885" class="Keyword">open</a> <a id="23890" class="Keyword">import</a> <a id="23897" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="23941" class="Keyword">open</a> <a id="23946" class="Keyword">import</a> <a id="23953" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="23990" class="Keyword">open</a> <a id="23995" class="Keyword">import</a> <a id="24002" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24024" class="Keyword">open</a> <a id="24029" class="Keyword">import</a> <a id="24036" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24066" class="Keyword">open</a> <a id="24071" class="Keyword">import</a> <a id="24078" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24117" class="Keyword">open</a> <a id="24122" class="Keyword">import</a> <a id="24129" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24167" class="Keyword">open</a> <a id="24172" class="Keyword">import</a> <a id="24179" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24237" class="Keyword">open</a> <a id="24242" class="Keyword">import</a> <a id="24249" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24314" class="Keyword">open</a> <a id="24319" class="Keyword">import</a> <a id="24326" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24357" class="Keyword">open</a> <a id="24362" class="Keyword">import</a> <a id="24369" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24396" class="Keyword">open</a> <a id="24401" class="Keyword">import</a> <a id="24408" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24466" class="Keyword">open</a> <a id="24471" class="Keyword">import</a> <a id="24478" href="group-theory.html" class="Module">group-theory</a>
<a id="24491" class="Keyword">open</a> <a id="24496" class="Keyword">import</a> <a id="24503" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24531" class="Keyword">open</a> <a id="24536" class="Keyword">import</a> <a id="24543" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24594" class="Keyword">open</a> <a id="24599" class="Keyword">import</a> <a id="24606" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24639" class="Keyword">open</a> <a id="24644" class="Keyword">import</a> <a id="24651" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24698" class="Keyword">open</a> <a id="24703" class="Keyword">import</a> <a id="24710" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24749" class="Keyword">open</a> <a id="24754" class="Keyword">import</a> <a id="24761" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24801" class="Keyword">open</a> <a id="24806" class="Keyword">import</a> <a id="24813" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="24856" class="Keyword">open</a> <a id="24861" class="Keyword">import</a> <a id="24868" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="24900" class="Keyword">open</a> <a id="24905" class="Keyword">import</a> <a id="24912" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="24948" class="Keyword">open</a> <a id="24953" class="Keyword">import</a> <a id="24960" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="24989" class="Keyword">open</a> <a id="24994" class="Keyword">import</a> <a id="25001" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25034" class="Keyword">open</a> <a id="25039" class="Keyword">import</a> <a id="25046" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25082" class="Keyword">open</a> <a id="25087" class="Keyword">import</a> <a id="25094" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25123" class="Keyword">open</a> <a id="25128" class="Keyword">import</a> <a id="25135" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25160" class="Keyword">open</a> <a id="25165" class="Keyword">import</a> <a id="25172" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25234" class="Keyword">open</a> <a id="25239" class="Keyword">import</a> <a id="25246" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25277" class="Keyword">open</a> <a id="25282" class="Keyword">import</a> <a id="25289" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25336" class="Keyword">open</a> <a id="25341" class="Keyword">import</a> <a id="25348" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25381" class="Keyword">open</a> <a id="25386" class="Keyword">import</a> <a id="25393" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25433" class="Keyword">open</a> <a id="25438" class="Keyword">import</a> <a id="25445" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25482" class="Keyword">open</a> <a id="25487" class="Keyword">import</a> <a id="25494" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="25530" class="Keyword">open</a> <a id="25535" class="Keyword">import</a> <a id="25542" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="25583" class="Keyword">open</a> <a id="25588" class="Keyword">import</a> <a id="25595" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25627" class="Keyword">open</a> <a id="25632" class="Keyword">import</a> <a id="25639" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25666" class="Keyword">open</a> <a id="25671" class="Keyword">import</a> <a id="25678" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="25698" class="Keyword">open</a> <a id="25703" class="Keyword">import</a> <a id="25710" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="25737" class="Keyword">open</a> <a id="25742" class="Keyword">import</a> <a id="25749" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="25791" class="Keyword">open</a> <a id="25796" class="Keyword">import</a> <a id="25803" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="25853" class="Keyword">open</a> <a id="25858" class="Keyword">import</a> <a id="25865" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="25912" class="Keyword">open</a> <a id="25917" class="Keyword">import</a> <a id="25924" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="25965" class="Keyword">open</a> <a id="25970" class="Keyword">import</a> <a id="25977" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26011" class="Keyword">open</a> <a id="26016" class="Keyword">import</a> <a id="26023" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="26058" class="Keyword">open</a> <a id="26063" class="Keyword">import</a> <a id="26070" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="26108" class="Keyword">open</a> <a id="26113" class="Keyword">import</a> <a id="26120" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26152" class="Keyword">open</a> <a id="26157" class="Keyword">import</a> <a id="26164" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="26205" class="Keyword">open</a> <a id="26210" class="Keyword">import</a> <a id="26217" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="26258" class="Keyword">open</a> <a id="26263" class="Keyword">import</a> <a id="26270" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26310" class="Keyword">open</a> <a id="26315" class="Keyword">import</a> <a id="26322" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26355" class="Keyword">open</a> <a id="26360" class="Keyword">import</a> <a id="26367" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="26404" class="Keyword">open</a> <a id="26409" class="Keyword">import</a> <a id="26416" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="26446" class="Keyword">open</a> <a id="26451" class="Keyword">import</a> <a id="26458" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="26503" class="Keyword">open</a> <a id="26508" class="Keyword">import</a> <a id="26515" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="26543" class="Keyword">open</a> <a id="26548" class="Keyword">import</a> <a id="26555" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="26576" class="Keyword">open</a> <a id="26581" class="Keyword">import</a> <a id="26588" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="26622" class="Keyword">open</a> <a id="26627" class="Keyword">import</a> <a id="26634" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="26677" class="Keyword">open</a> <a id="26682" class="Keyword">import</a> <a id="26689" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="26723" class="Keyword">open</a> <a id="26728" class="Keyword">import</a> <a id="26735" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="26770" class="Keyword">open</a> <a id="26775" class="Keyword">import</a> <a id="26782" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="26824" class="Keyword">open</a> <a id="26829" class="Keyword">import</a> <a id="26836" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="26871" class="Keyword">open</a> <a id="26876" class="Keyword">import</a> <a id="26883" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="26922" class="Keyword">open</a> <a id="26927" class="Keyword">import</a> <a id="26934" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="26971" class="Keyword">open</a> <a id="26976" class="Keyword">import</a> <a id="26983" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="27030" class="Keyword">open</a> <a id="27035" class="Keyword">import</a> <a id="27042" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="27106" class="Keyword">open</a> <a id="27111" class="Keyword">import</a> <a id="27118" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="27142" class="Keyword">open</a> <a id="27147" class="Keyword">import</a> <a id="27154" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="27179" class="Keyword">open</a> <a id="27184" class="Keyword">import</a> <a id="27191" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="27234" class="Keyword">open</a> <a id="27239" class="Keyword">import</a> <a id="27246" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="27277" class="Keyword">open</a> <a id="27282" class="Keyword">import</a> <a id="27289" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="27343" class="Keyword">open</a> <a id="27348" class="Keyword">import</a> <a id="27355" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="27378" class="Keyword">open</a> <a id="27383" class="Keyword">import</a> <a id="27390" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="27428" class="Keyword">open</a> <a id="27433" class="Keyword">import</a> <a id="27440" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="27479" class="Keyword">open</a> <a id="27484" class="Keyword">import</a> <a id="27491" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="27542" class="Keyword">open</a> <a id="27547" class="Keyword">import</a> <a id="27554" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="27611" class="Keyword">open</a> <a id="27616" class="Keyword">import</a> <a id="27623" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="27671" class="Keyword">open</a> <a id="27676" class="Keyword">import</a> <a id="27683" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="27713" class="Keyword">open</a> <a id="27718" class="Keyword">import</a> <a id="27725" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="27746" class="Keyword">open</a> <a id="27751" class="Keyword">import</a> <a id="27758" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="27805" class="Keyword">open</a> <a id="27810" class="Keyword">import</a> <a id="27817" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="27855" class="Keyword">open</a> <a id="27860" class="Keyword">import</a> <a id="27867" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="27961" class="Keyword">open</a> <a id="27966" class="Keyword">import</a> <a id="27973" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="27988" class="Keyword">open</a> <a id="27993" class="Keyword">import</a> <a id="28000" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="28033" class="Keyword">open</a> <a id="28038" class="Keyword">import</a> <a id="28045" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="28077" class="Keyword">open</a> <a id="28082" class="Keyword">import</a> <a id="28089" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="28131" class="Keyword">open</a> <a id="28136" class="Keyword">import</a> <a id="28143" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="28181" class="Keyword">open</a> <a id="28186" class="Keyword">import</a> <a id="28193" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="28230" class="Keyword">open</a> <a id="28235" class="Keyword">import</a> <a id="28242" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="28275" class="Keyword">open</a> <a id="28280" class="Keyword">import</a> <a id="28287" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="28311" class="Keyword">open</a> <a id="28316" class="Keyword">import</a> <a id="28323" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="28362" class="Keyword">open</a> <a id="28367" class="Keyword">import</a> <a id="28374" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="28420" class="Keyword">open</a> <a id="28425" class="Keyword">import</a> <a id="28432" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="28477" class="Keyword">open</a> <a id="28482" class="Keyword">import</a> <a id="28489" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="28527" class="Keyword">open</a> <a id="28532" class="Keyword">import</a> <a id="28539" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="28571" class="Keyword">open</a> <a id="28576" class="Keyword">import</a> <a id="28583" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="28636" class="Keyword">open</a> <a id="28641" class="Keyword">import</a> <a id="28648" href="order-theory.html" class="Module">order-theory</a>
<a id="28661" class="Keyword">open</a> <a id="28666" class="Keyword">import</a> <a id="28673" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="28700" class="Keyword">open</a> <a id="28705" class="Keyword">import</a> <a id="28712" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="28742" class="Keyword">open</a> <a id="28747" class="Keyword">import</a> <a id="28754" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="28787" class="Keyword">open</a> <a id="28792" class="Keyword">import</a> <a id="28799" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="28835" class="Keyword">open</a> <a id="28840" class="Keyword">import</a> <a id="28847" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="28882" class="Keyword">open</a> <a id="28887" class="Keyword">import</a> <a id="28894" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="28921" class="Keyword">open</a> <a id="28926" class="Keyword">import</a> <a id="28933" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="28963" class="Keyword">open</a> <a id="28968" class="Keyword">import</a> <a id="28975" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="29011" class="Keyword">open</a> <a id="29016" class="Keyword">import</a> <a id="29023" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="29065" class="Keyword">open</a> <a id="29070" class="Keyword">import</a> <a id="29077" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="29109" class="Keyword">open</a> <a id="29114" class="Keyword">import</a> <a id="29121" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="29152" class="Keyword">open</a> <a id="29157" class="Keyword">import</a> <a id="29164" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="29190" class="Keyword">open</a> <a id="29195" class="Keyword">import</a> <a id="29202" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="29231" class="Keyword">open</a> <a id="29236" class="Keyword">import</a> <a id="29243" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="29280" class="Keyword">open</a> <a id="29285" class="Keyword">import</a> <a id="29292" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="29332" class="Keyword">open</a> <a id="29337" class="Keyword">import</a> <a id="29344" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="29366" class="Keyword">open</a> <a id="29371" class="Keyword">import</a> <a id="29378" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="29413" class="Keyword">open</a> <a id="29418" class="Keyword">import</a> <a id="29425" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="29463" class="Keyword">open</a> <a id="29468" class="Keyword">import</a> <a id="29475" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="29514" class="Keyword">open</a> <a id="29519" class="Keyword">import</a> <a id="29526" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="29561" class="Keyword">open</a> <a id="29566" class="Keyword">import</a> <a id="29573" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="29608" class="Keyword">open</a> <a id="29613" class="Keyword">import</a> <a id="29620" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="29658" class="Keyword">open</a> <a id="29663" class="Keyword">import</a> <a id="29670" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="29701" class="Keyword">open</a> <a id="29706" class="Keyword">import</a> <a id="29713" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="29755" class="Keyword">open</a> <a id="29760" class="Keyword">import</a> <a id="29767" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="29812" class="Keyword">open</a> <a id="29817" class="Keyword">import</a> <a id="29824" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="29857" class="Keyword">open</a> <a id="29862" class="Keyword">import</a> <a id="29869" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="29889" class="Keyword">open</a> <a id="29894" class="Keyword">import</a> <a id="29901" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="29924" class="Keyword">open</a> <a id="29929" class="Keyword">import</a> <a id="29936" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="29959" class="Keyword">open</a> <a id="29964" class="Keyword">import</a> <a id="29971" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="29997" class="Keyword">open</a> <a id="30002" class="Keyword">import</a> <a id="30009" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="30035" class="Keyword">open</a> <a id="30040" class="Keyword">import</a> <a id="30047" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="30111" class="Keyword">open</a> <a id="30116" class="Keyword">import</a> <a id="30123" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="30141" class="Keyword">open</a> <a id="30146" class="Keyword">import</a> <a id="30153" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="30180" class="Keyword">open</a> <a id="30185" class="Keyword">import</a> <a id="30192" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="30218" class="Keyword">open</a> <a id="30223" class="Keyword">import</a> <a id="30230" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="30256" class="Keyword">open</a> <a id="30261" class="Keyword">import</a> <a id="30268" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="30294" class="Keyword">open</a> <a id="30299" class="Keyword">import</a> <a id="30306" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="30337" class="Keyword">open</a> <a id="30342" class="Keyword">import</a> <a id="30349" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="30412" class="Keyword">open</a> <a id="30417" class="Keyword">import</a> <a id="30424" href="polytopes.html" class="Module">polytopes</a>
<a id="30434" class="Keyword">open</a> <a id="30439" class="Keyword">import</a> <a id="30446" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="30504" class="Keyword">open</a> <a id="30509" class="Keyword">import</a> <a id="30516" href="ring-theory.html" class="Module">ring-theory</a>
<a id="30528" class="Keyword">open</a> <a id="30533" class="Keyword">import</a> <a id="30540" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="30577" class="Keyword">open</a> <a id="30582" class="Keyword">import</a> <a id="30589" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="30616" class="Keyword">open</a> <a id="30621" class="Keyword">import</a> <a id="30628" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="30660" class="Keyword">open</a> <a id="30665" class="Keyword">import</a> <a id="30672" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="30718" class="Keyword">open</a> <a id="30723" class="Keyword">import</a> <a id="30730" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="30755" class="Keyword">open</a> <a id="30760" class="Keyword">import</a> <a id="30767" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="30810" class="Keyword">open</a> <a id="30815" class="Keyword">import</a> <a id="30822" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="30860" class="Keyword">open</a> <a id="30865" class="Keyword">import</a> <a id="30872" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="30903" class="Keyword">open</a> <a id="30908" class="Keyword">import</a> <a id="30915" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="30939" class="Keyword">open</a> <a id="30944" class="Keyword">import</a> <a id="30951" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="30983" class="Keyword">open</a> <a id="30988" class="Keyword">import</a> <a id="30995" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="31021" class="Keyword">open</a> <a id="31026" class="Keyword">import</a> <a id="31033" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="31062" class="Keyword">open</a> <a id="31067" class="Keyword">import</a> <a id="31074" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="31111" class="Keyword">open</a> <a id="31116" class="Keyword">import</a> <a id="31123" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="31152" class="Keyword">open</a> <a id="31157" class="Keyword">import</a> <a id="31164" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="31191" class="Keyword">open</a> <a id="31196" class="Keyword">import</a> <a id="31203" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="31240" class="Keyword">open</a> <a id="31245" class="Keyword">import</a> <a id="31252" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="31279" class="Keyword">open</a> <a id="31284" class="Keyword">import</a> <a id="31291" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="31324" class="Keyword">open</a> <a id="31329" class="Keyword">import</a> <a id="31336" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="31354" class="Keyword">open</a> <a id="31359" class="Keyword">import</a> <a id="31366" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="31420" class="Keyword">open</a> <a id="31425" class="Keyword">import</a> <a id="31432" href="set-theory.html" class="Module">set-theory</a>
<a id="31443" class="Keyword">open</a> <a id="31448" class="Keyword">import</a> <a id="31455" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="31478" class="Keyword">open</a> <a id="31483" class="Keyword">import</a> <a id="31490" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="31514" class="Keyword">open</a> <a id="31519" class="Keyword">import</a> <a id="31526" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="31552" class="Keyword">open</a> <a id="31557" class="Keyword">import</a> <a id="31564" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="31626" class="Keyword">open</a> <a id="31631" class="Keyword">import</a> <a id="31638" href="structured-types.html" class="Module">structured-types</a>
<a id="31655" class="Keyword">open</a> <a id="31660" class="Keyword">import</a> <a id="31667" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="31702" class="Keyword">open</a> <a id="31707" class="Keyword">import</a> <a id="31714" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="31758" class="Keyword">open</a> <a id="31763" class="Keyword">import</a> <a id="31770" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="31834" class="Keyword">open</a> <a id="31839" class="Keyword">import</a> <a id="31846" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="31892" class="Keyword">open</a> <a id="31897" class="Keyword">import</a> <a id="31904" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="31928" class="Keyword">open</a> <a id="31933" class="Keyword">import</a> <a id="31940" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="32009" class="Keyword">open</a> <a id="32014" class="Keyword">import</a> <a id="32021" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="32066" class="Keyword">open</a> <a id="32071" class="Keyword">import</a> <a id="32078" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="32112" class="Keyword">open</a> <a id="32117" class="Keyword">import</a> <a id="32124" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="32185" class="Keyword">open</a> <a id="32190" class="Keyword">import</a> <a id="32197" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="32242" class="Keyword">open</a> <a id="32247" class="Keyword">import</a> <a id="32254" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="32292" class="Keyword">open</a> <a id="32297" class="Keyword">import</a> <a id="32304" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="32347" class="Keyword">open</a> <a id="32352" class="Keyword">import</a> <a id="32359" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="32395" class="Keyword">open</a> <a id="32400" class="Keyword">import</a> <a id="32407" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="32437" class="Keyword">open</a> <a id="32442" class="Keyword">import</a> <a id="32449" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="32480" class="Keyword">open</a> <a id="32485" class="Keyword">import</a> <a id="32492" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="32551" class="Keyword">open</a> <a id="32556" class="Keyword">import</a> <a id="32563" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="32614" class="Keyword">open</a> <a id="32619" class="Keyword">import</a> <a id="32626" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="32677" class="Keyword">open</a> <a id="32682" class="Keyword">import</a> <a id="32689" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="32744" class="Keyword">open</a> <a id="32749" class="Keyword">import</a> <a id="32756" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="32785" class="Keyword">open</a> <a id="32790" class="Keyword">import</a> <a id="32797" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="32825" class="Keyword">open</a> <a id="32830" class="Keyword">import</a> <a id="32837" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="32867" class="Keyword">open</a> <a id="32872" class="Keyword">import</a> <a id="32879" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="32913" class="Keyword">open</a> <a id="32918" class="Keyword">import</a> <a id="32925" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="33001" class="Keyword">open</a> <a id="33006" class="Keyword">import</a> <a id="33013" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="33039" class="Keyword">open</a> <a id="33044" class="Keyword">import</a> <a id="33051" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="33090" class="Keyword">open</a> <a id="33095" class="Keyword">import</a> <a id="33102" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="33140" class="Keyword">open</a> <a id="33145" class="Keyword">import</a> <a id="33152" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="33198" class="Keyword">open</a> <a id="33203" class="Keyword">import</a> <a id="33210" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="33247" class="Keyword">open</a> <a id="33252" class="Keyword">import</a> <a id="33259" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="33299" class="Keyword">open</a> <a id="33304" class="Keyword">import</a> <a id="33311" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="33350" class="Keyword">open</a> <a id="33355" class="Keyword">import</a> <a id="33362" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="33395" class="Keyword">open</a> <a id="33400" class="Keyword">import</a> <a id="33407" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="33442" class="Keyword">open</a> <a id="33447" class="Keyword">import</a> <a id="33454" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="33499" class="Keyword">open</a> <a id="33504" class="Keyword">import</a> <a id="33511" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="33563" class="Keyword">open</a> <a id="33568" class="Keyword">import</a> <a id="33575" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="33628" class="Keyword">open</a> <a id="33633" class="Keyword">import</a> <a id="33640" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="33700" class="Keyword">open</a> <a id="33705" class="Keyword">import</a> <a id="33712" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="33760" class="Keyword">open</a> <a id="33765" class="Keyword">import</a> <a id="33772" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="33812" class="Keyword">open</a> <a id="33817" class="Keyword">import</a> <a id="33824" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="33871" class="Keyword">open</a> <a id="33876" class="Keyword">import</a> <a id="33883" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="33924" class="Keyword">open</a> <a id="33929" class="Keyword">import</a> <a id="33936" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="33974" class="Keyword">open</a> <a id="33979" class="Keyword">import</a> <a id="33986" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="34034" class="Keyword">open</a> <a id="34039" class="Keyword">import</a> <a id="34046" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="34083" class="Keyword">open</a> <a id="34088" class="Keyword">import</a> <a id="34095" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="34129" class="Keyword">open</a> <a id="34134" class="Keyword">import</a> <a id="34141" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="34188" class="Keyword">open</a> <a id="34193" class="Keyword">import</a> <a id="34200" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="34245" class="Keyword">open</a> <a id="34250" class="Keyword">import</a> <a id="34257" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="34306" class="Keyword">open</a> <a id="34311" class="Keyword">import</a> <a id="34318" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="34395" class="Keyword">open</a> <a id="34400" class="Keyword">import</a> <a id="34407" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="34459" class="Keyword">open</a> <a id="34464" class="Keyword">import</a> <a id="34471" href="type-theories.html" class="Module">type-theories</a>
<a id="34485" class="Keyword">open</a> <a id="34490" class="Keyword">import</a> <a id="34497" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="34539" class="Keyword">open</a> <a id="34544" class="Keyword">import</a> <a id="34551" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="34589" class="Keyword">open</a> <a id="34594" class="Keyword">import</a> <a id="34601" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="34647" class="Keyword">open</a> <a id="34652" class="Keyword">import</a> <a id="34659" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="34706" class="Keyword">open</a> <a id="34711" class="Keyword">import</a> <a id="34718" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="34753" class="Keyword">open</a> <a id="34758" class="Keyword">import</a> <a id="34765" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="34843" class="Keyword">open</a> <a id="34848" class="Keyword">import</a> <a id="34855" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="34879" class="Keyword">open</a> <a id="34884" class="Keyword">import</a> <a id="34891" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="34944" class="Keyword">open</a> <a id="34949" class="Keyword">import</a> <a id="34956" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="34999" class="Keyword">open</a> <a id="35004" class="Keyword">import</a> <a id="35011" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="35051" class="Keyword">open</a> <a id="35056" class="Keyword">import</a> <a id="35063" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="35102" class="Keyword">open</a> <a id="35107" class="Keyword">import</a> <a id="35114" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="35148" class="Keyword">open</a> <a id="35153" class="Keyword">import</a> <a id="35160" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="35208" class="Keyword">open</a> <a id="35213" class="Keyword">import</a> <a id="35220" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="35271" class="Keyword">open</a> <a id="35276" class="Keyword">import</a> <a id="35283" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="35330" class="Keyword">open</a> <a id="35335" class="Keyword">import</a> <a id="35342" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="35394" class="Keyword">open</a> <a id="35399" class="Keyword">import</a> <a id="35406" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="35450" class="Keyword">open</a> <a id="35455" class="Keyword">import</a> <a id="35462" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="35502" class="Keyword">open</a> <a id="35507" class="Keyword">import</a> <a id="35514" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="35557" class="Keyword">open</a> <a id="35562" class="Keyword">import</a> <a id="35569" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="35621" class="Keyword">open</a> <a id="35626" class="Keyword">import</a> <a id="35633" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="35687" class="Keyword">open</a> <a id="35692" class="Keyword">import</a> <a id="35699" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="35747" class="Keyword">open</a> <a id="35752" class="Keyword">import</a> <a id="35759" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="35798" class="Keyword">open</a> <a id="35803" class="Keyword">import</a> <a id="35810" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="35843" class="Keyword">open</a> <a id="35848" class="Keyword">import</a> <a id="35855" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="35885" class="Keyword">open</a> <a id="35890" class="Keyword">import</a> <a id="35897" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="35948" class="Keyword">open</a> <a id="35953" class="Keyword">import</a> <a id="35960" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="36001" class="Keyword">open</a> <a id="36006" class="Keyword">import</a> <a id="36013" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="36050" class="Keyword">open</a> <a id="36055" class="Keyword">import</a> <a id="36062" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="36121" class="Keyword">open</a> <a id="36126" class="Keyword">import</a> <a id="36133" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="36188" class="Keyword">open</a> <a id="36193" class="Keyword">import</a> <a id="36200" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="36256" class="Keyword">open</a> <a id="36261" class="Keyword">import</a> <a id="36268" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="36315" class="Keyword">open</a> <a id="36320" class="Keyword">import</a> <a id="36327" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="36370" class="Keyword">open</a> <a id="36375" class="Keyword">import</a> <a id="36382" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="36427" class="Keyword">open</a> <a id="36432" class="Keyword">import</a> <a id="36439" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="36488" class="Keyword">open</a> <a id="36493" class="Keyword">import</a> <a id="36500" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="36551" class="Keyword">open</a> <a id="36556" class="Keyword">import</a> <a id="36563" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="36607" class="Keyword">open</a> <a id="36612" class="Keyword">import</a> <a id="36619" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="36697" class="Keyword">open</a> <a id="36702" class="Keyword">import</a> <a id="36709" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="36749" class="Keyword">open</a> <a id="36754" class="Keyword">import</a> <a id="36761" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="36818" class="Keyword">open</a> <a id="36823" class="Keyword">import</a> <a id="36830" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="36865" class="Keyword">open</a> <a id="36870" class="Keyword">import</a> <a id="36877" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="36923" class="Keyword">open</a> <a id="36928" class="Keyword">import</a> <a id="36935" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="36990" class="Keyword">open</a> <a id="36995" class="Keyword">import</a> <a id="37002" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="37045" class="Keyword">open</a> <a id="37050" class="Keyword">import</a> <a id="37057" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="37102" class="Keyword">open</a> <a id="37107" class="Keyword">import</a> <a id="37114" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="37173" class="Keyword">open</a> <a id="37178" class="Keyword">import</a> <a id="37185" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="37222" class="Keyword">open</a> <a id="37227" class="Keyword">import</a> <a id="37234" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="37276" class="Keyword">open</a> <a id="37281" class="Keyword">import</a> <a id="37288" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="37329" class="Keyword">open</a> <a id="37334" class="Keyword">import</a> <a id="37341" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="37380" class="Keyword">open</a> <a id="37385" class="Keyword">import</a> <a id="37392" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="37430" class="Keyword">open</a> <a id="37435" class="Keyword">import</a> <a id="37442" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="37494" class="Keyword">open</a> <a id="37499" class="Keyword">import</a> <a id="37506" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="37551" class="Keyword">open</a> <a id="37556" class="Keyword">import</a> <a id="37563" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="37602" class="Keyword">open</a> <a id="37607" class="Keyword">import</a> <a id="37614" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="37651" class="Keyword">open</a> <a id="37656" class="Keyword">import</a> <a id="37663" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="37712" class="Keyword">open</a> <a id="37717" class="Keyword">import</a> <a id="37724" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="37763" class="Keyword">open</a> <a id="37768" class="Keyword">import</a> <a id="37775" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="37813" class="Keyword">open</a> <a id="37818" class="Keyword">import</a> <a id="37825" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="37880" class="Keyword">open</a> <a id="37885" class="Keyword">import</a> <a id="37892" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="37931" class="Keyword">open</a> <a id="37936" class="Keyword">import</a> <a id="37943" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="37991" class="Keyword">open</a> <a id="37996" class="Keyword">import</a> <a id="38003" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="38050" class="Keyword">open</a> <a id="38055" class="Keyword">import</a> <a id="38062" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="38100" class="Keyword">open</a> <a id="38105" class="Keyword">import</a> <a id="38112" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="38142" class="Keyword">open</a> <a id="38147" class="Keyword">import</a> <a id="38154" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="38211" class="Keyword">open</a> <a id="38216" class="Keyword">import</a> <a id="38223" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="38277" class="Keyword">open</a> <a id="38282" class="Keyword">import</a> <a id="38289" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="38319" class="Keyword">open</a> <a id="38324" class="Keyword">import</a> <a id="38331" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="38380" class="Keyword">open</a> <a id="38385" class="Keyword">import</a> <a id="38392" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="38434" class="Keyword">open</a> <a id="38439" class="Keyword">import</a> <a id="38446" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="38480" class="Keyword">open</a> <a id="38485" class="Keyword">import</a> <a id="38492" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="38555" class="Keyword">open</a> <a id="38560" class="Keyword">import</a> <a id="38567" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="38610" class="Keyword">open</a> <a id="38615" class="Keyword">import</a> <a id="38622" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="38657" class="Keyword">open</a> <a id="38662" class="Keyword">import</a> <a id="38669" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="38704" class="Keyword">open</a> <a id="38709" class="Keyword">import</a> <a id="38716" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="38756" class="Keyword">open</a> <a id="38761" class="Keyword">import</a> <a id="38768" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="38813" class="Keyword">open</a> <a id="38818" class="Keyword">import</a> <a id="38825" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="38866" class="Keyword">open</a> <a id="38871" class="Keyword">import</a> <a id="38878" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="38932" class="Keyword">open</a> <a id="38937" class="Keyword">import</a> <a id="38944" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="38994" class="Keyword">open</a> <a id="38999" class="Keyword">import</a> <a id="39006" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="39053" class="Keyword">open</a> <a id="39058" class="Keyword">import</a> <a id="39065" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="39103" class="Keyword">open</a> <a id="39108" class="Keyword">import</a> <a id="39115" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="39164" class="Keyword">open</a> <a id="39169" class="Keyword">import</a> <a id="39176" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="39223" class="Keyword">open</a> <a id="39228" class="Keyword">import</a> <a id="39235" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="39298" class="Keyword">open</a> <a id="39303" class="Keyword">import</a> <a id="39310" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="39342" class="Keyword">open</a> <a id="39347" class="Keyword">import</a> <a id="39354" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="39407" class="Keyword">open</a> <a id="39412" class="Keyword">import</a> <a id="39419" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="39465" class="Keyword">open</a> <a id="39470" class="Keyword">import</a> <a id="39477" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="39523" class="Keyword">open</a> <a id="39528" class="Keyword">import</a> <a id="39535" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="39583" class="Keyword">open</a> <a id="39588" class="Keyword">import</a> <a id="39595" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="39635" class="Keyword">open</a> <a id="39640" class="Keyword">import</a> <a id="39647" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="39692" class="Keyword">open</a> <a id="39697" class="Keyword">import</a> <a id="39704" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="39769" class="Keyword">open</a> <a id="39774" class="Keyword">import</a> <a id="39781" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="39826" class="Keyword">open</a> <a id="39831" class="Keyword">import</a> <a id="39838" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="39885" class="Keyword">open</a> <a id="39890" class="Keyword">import</a> <a id="39897" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="39950" class="Keyword">open</a> <a id="39955" class="Keyword">import</a> <a id="39962" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>