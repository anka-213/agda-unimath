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
<a id="22707" class="Keyword">open</a> <a id="22712" class="Keyword">import</a> <a id="22719" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22760" class="Keyword">open</a> <a id="22765" class="Keyword">import</a> <a id="22772" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="22810" class="Keyword">open</a> <a id="22815" class="Keyword">import</a> <a id="22822" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22851" class="Keyword">open</a> <a id="22856" class="Keyword">import</a> <a id="22863" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22908" class="Keyword">open</a> <a id="22913" class="Keyword">import</a> <a id="22920" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="22962" class="Keyword">open</a> <a id="22967" class="Keyword">import</a> <a id="22974" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23018" class="Keyword">open</a> <a id="23023" class="Keyword">import</a> <a id="23030" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23079" class="Keyword">open</a> <a id="23084" class="Keyword">import</a> <a id="23091" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23141" class="Keyword">open</a> <a id="23146" class="Keyword">import</a> <a id="23153" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23180" class="Keyword">open</a> <a id="23185" class="Keyword">import</a> <a id="23192" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23233" class="Keyword">open</a> <a id="23238" class="Keyword">import</a> <a id="23245" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23268" class="Keyword">open</a> <a id="23273" class="Keyword">import</a> <a id="23280" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23329" class="Keyword">open</a> <a id="23334" class="Keyword">import</a> <a id="23341" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23380" class="Keyword">open</a> <a id="23385" class="Keyword">import</a> <a id="23392" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="23433" class="Keyword">open</a> <a id="23438" class="Keyword">import</a> <a id="23445" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="23489" class="Keyword">open</a> <a id="23494" class="Keyword">import</a> <a id="23501" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="23538" class="Keyword">open</a> <a id="23543" class="Keyword">import</a> <a id="23550" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="23572" class="Keyword">open</a> <a id="23577" class="Keyword">import</a> <a id="23584" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23614" class="Keyword">open</a> <a id="23619" class="Keyword">import</a> <a id="23626" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="23665" class="Keyword">open</a> <a id="23670" class="Keyword">import</a> <a id="23677" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="23715" class="Keyword">open</a> <a id="23720" class="Keyword">import</a> <a id="23727" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="23785" class="Keyword">open</a> <a id="23790" class="Keyword">import</a> <a id="23797" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="23828" class="Keyword">open</a> <a id="23833" class="Keyword">import</a> <a id="23840" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="23867" class="Keyword">open</a> <a id="23872" class="Keyword">import</a> <a id="23879" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="23937" class="Keyword">open</a> <a id="23942" class="Keyword">import</a> <a id="23949" href="group-theory.html" class="Module">group-theory</a>
<a id="23962" class="Keyword">open</a> <a id="23967" class="Keyword">import</a> <a id="23974" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24002" class="Keyword">open</a> <a id="24007" class="Keyword">import</a> <a id="24014" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="24045" class="Keyword">open</a> <a id="24050" class="Keyword">import</a> <a id="24057" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="24093" class="Keyword">open</a> <a id="24098" class="Keyword">import</a> <a id="24105" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24156" class="Keyword">open</a> <a id="24161" class="Keyword">import</a> <a id="24168" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24201" class="Keyword">open</a> <a id="24206" class="Keyword">import</a> <a id="24213" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24260" class="Keyword">open</a> <a id="24265" class="Keyword">import</a> <a id="24272" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24311" class="Keyword">open</a> <a id="24316" class="Keyword">import</a> <a id="24323" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24363" class="Keyword">open</a> <a id="24368" class="Keyword">import</a> <a id="24375" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="24418" class="Keyword">open</a> <a id="24423" class="Keyword">import</a> <a id="24430" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="24462" class="Keyword">open</a> <a id="24467" class="Keyword">import</a> <a id="24474" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="24510" class="Keyword">open</a> <a id="24515" class="Keyword">import</a> <a id="24522" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="24551" class="Keyword">open</a> <a id="24556" class="Keyword">import</a> <a id="24563" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="24596" class="Keyword">open</a> <a id="24601" class="Keyword">import</a> <a id="24608" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="24644" class="Keyword">open</a> <a id="24649" class="Keyword">import</a> <a id="24656" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="24685" class="Keyword">open</a> <a id="24690" class="Keyword">import</a> <a id="24697" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="24729" class="Keyword">open</a> <a id="24734" class="Keyword">import</a> <a id="24741" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="24766" class="Keyword">open</a> <a id="24771" class="Keyword">import</a> <a id="24778" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="24809" class="Keyword">open</a> <a id="24814" class="Keyword">import</a> <a id="24821" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="24868" class="Keyword">open</a> <a id="24873" class="Keyword">import</a> <a id="24880" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="24913" class="Keyword">open</a> <a id="24918" class="Keyword">import</a> <a id="24925" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="24965" class="Keyword">open</a> <a id="24970" class="Keyword">import</a> <a id="24977" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25014" class="Keyword">open</a> <a id="25019" class="Keyword">import</a> <a id="25026" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="25062" class="Keyword">open</a> <a id="25067" class="Keyword">import</a> <a id="25074" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25106" class="Keyword">open</a> <a id="25111" class="Keyword">import</a> <a id="25118" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25145" class="Keyword">open</a> <a id="25150" class="Keyword">import</a> <a id="25157" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="25177" class="Keyword">open</a> <a id="25182" class="Keyword">import</a> <a id="25189" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="25216" class="Keyword">open</a> <a id="25221" class="Keyword">import</a> <a id="25228" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="25270" class="Keyword">open</a> <a id="25275" class="Keyword">import</a> <a id="25282" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="25329" class="Keyword">open</a> <a id="25334" class="Keyword">import</a> <a id="25341" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="25382" class="Keyword">open</a> <a id="25387" class="Keyword">import</a> <a id="25394" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="25428" class="Keyword">open</a> <a id="25433" class="Keyword">import</a> <a id="25440" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="25475" class="Keyword">open</a> <a id="25480" class="Keyword">import</a> <a id="25487" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="25525" class="Keyword">open</a> <a id="25530" class="Keyword">import</a> <a id="25537" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="25569" class="Keyword">open</a> <a id="25574" class="Keyword">import</a> <a id="25581" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="25622" class="Keyword">open</a> <a id="25627" class="Keyword">import</a> <a id="25634" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="25675" class="Keyword">open</a> <a id="25680" class="Keyword">import</a> <a id="25687" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="25727" class="Keyword">open</a> <a id="25732" class="Keyword">import</a> <a id="25739" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="25772" class="Keyword">open</a> <a id="25777" class="Keyword">import</a> <a id="25784" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="25821" class="Keyword">open</a> <a id="25826" class="Keyword">import</a> <a id="25833" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="25863" class="Keyword">open</a> <a id="25868" class="Keyword">import</a> <a id="25875" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="25920" class="Keyword">open</a> <a id="25925" class="Keyword">import</a> <a id="25932" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="25960" class="Keyword">open</a> <a id="25965" class="Keyword">import</a> <a id="25972" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="25993" class="Keyword">open</a> <a id="25998" class="Keyword">import</a> <a id="26005" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="26039" class="Keyword">open</a> <a id="26044" class="Keyword">import</a> <a id="26051" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="26085" class="Keyword">open</a> <a id="26090" class="Keyword">import</a> <a id="26097" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="26132" class="Keyword">open</a> <a id="26137" class="Keyword">import</a> <a id="26144" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="26186" class="Keyword">open</a> <a id="26191" class="Keyword">import</a> <a id="26198" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="26233" class="Keyword">open</a> <a id="26238" class="Keyword">import</a> <a id="26245" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="26284" class="Keyword">open</a> <a id="26289" class="Keyword">import</a> <a id="26296" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="26333" class="Keyword">open</a> <a id="26338" class="Keyword">import</a> <a id="26345" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="26369" class="Keyword">open</a> <a id="26374" class="Keyword">import</a> <a id="26381" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="26406" class="Keyword">open</a> <a id="26411" class="Keyword">import</a> <a id="26418" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="26449" class="Keyword">open</a> <a id="26454" class="Keyword">import</a> <a id="26461" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="26512" class="Keyword">open</a> <a id="26517" class="Keyword">import</a> <a id="26524" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="26547" class="Keyword">open</a> <a id="26552" class="Keyword">import</a> <a id="26559" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="26607" class="Keyword">open</a> <a id="26612" class="Keyword">import</a> <a id="26619" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="26649" class="Keyword">open</a> <a id="26654" class="Keyword">import</a> <a id="26661" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="26731" class="Keyword">open</a> <a id="26736" class="Keyword">import</a> <a id="26743" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="26758" class="Keyword">open</a> <a id="26763" class="Keyword">import</a> <a id="26770" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="26803" class="Keyword">open</a> <a id="26808" class="Keyword">import</a> <a id="26815" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="26847" class="Keyword">open</a> <a id="26852" class="Keyword">import</a> <a id="26859" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="26901" class="Keyword">open</a> <a id="26906" class="Keyword">import</a> <a id="26913" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="26951" class="Keyword">open</a> <a id="26956" class="Keyword">import</a> <a id="26963" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="27000" class="Keyword">open</a> <a id="27005" class="Keyword">import</a> <a id="27012" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="27045" class="Keyword">open</a> <a id="27050" class="Keyword">import</a> <a id="27057" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="27081" class="Keyword">open</a> <a id="27086" class="Keyword">import</a> <a id="27093" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="27132" class="Keyword">open</a> <a id="27137" class="Keyword">import</a> <a id="27144" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="27190" class="Keyword">open</a> <a id="27195" class="Keyword">import</a> <a id="27202" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="27247" class="Keyword">open</a> <a id="27252" class="Keyword">import</a> <a id="27259" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="27297" class="Keyword">open</a> <a id="27302" class="Keyword">import</a> <a id="27309" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="27341" class="Keyword">open</a> <a id="27346" class="Keyword">import</a> <a id="27353" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="27406" class="Keyword">open</a> <a id="27411" class="Keyword">import</a> <a id="27418" href="order-theory.html" class="Module">order-theory</a>
<a id="27431" class="Keyword">open</a> <a id="27436" class="Keyword">import</a> <a id="27443" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="27470" class="Keyword">open</a> <a id="27475" class="Keyword">import</a> <a id="27482" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="27512" class="Keyword">open</a> <a id="27517" class="Keyword">import</a> <a id="27524" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="27557" class="Keyword">open</a> <a id="27562" class="Keyword">import</a> <a id="27569" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="27605" class="Keyword">open</a> <a id="27610" class="Keyword">import</a> <a id="27617" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="27652" class="Keyword">open</a> <a id="27657" class="Keyword">import</a> <a id="27664" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="27691" class="Keyword">open</a> <a id="27696" class="Keyword">import</a> <a id="27703" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="27733" class="Keyword">open</a> <a id="27738" class="Keyword">import</a> <a id="27745" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="27781" class="Keyword">open</a> <a id="27786" class="Keyword">import</a> <a id="27793" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="27835" class="Keyword">open</a> <a id="27840" class="Keyword">import</a> <a id="27847" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="27879" class="Keyword">open</a> <a id="27884" class="Keyword">import</a> <a id="27891" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="27922" class="Keyword">open</a> <a id="27927" class="Keyword">import</a> <a id="27934" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="27960" class="Keyword">open</a> <a id="27965" class="Keyword">import</a> <a id="27972" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="28001" class="Keyword">open</a> <a id="28006" class="Keyword">import</a> <a id="28013" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="28050" class="Keyword">open</a> <a id="28055" class="Keyword">import</a> <a id="28062" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="28102" class="Keyword">open</a> <a id="28107" class="Keyword">import</a> <a id="28114" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="28136" class="Keyword">open</a> <a id="28141" class="Keyword">import</a> <a id="28148" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="28183" class="Keyword">open</a> <a id="28188" class="Keyword">import</a> <a id="28195" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="28233" class="Keyword">open</a> <a id="28238" class="Keyword">import</a> <a id="28245" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="28284" class="Keyword">open</a> <a id="28289" class="Keyword">import</a> <a id="28296" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="28331" class="Keyword">open</a> <a id="28336" class="Keyword">import</a> <a id="28343" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="28378" class="Keyword">open</a> <a id="28383" class="Keyword">import</a> <a id="28390" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="28428" class="Keyword">open</a> <a id="28433" class="Keyword">import</a> <a id="28440" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="28471" class="Keyword">open</a> <a id="28476" class="Keyword">import</a> <a id="28483" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="28525" class="Keyword">open</a> <a id="28530" class="Keyword">import</a> <a id="28537" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="28582" class="Keyword">open</a> <a id="28587" class="Keyword">import</a> <a id="28594" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="28627" class="Keyword">open</a> <a id="28632" class="Keyword">import</a> <a id="28639" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="28659" class="Keyword">open</a> <a id="28664" class="Keyword">import</a> <a id="28671" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="28694" class="Keyword">open</a> <a id="28699" class="Keyword">import</a> <a id="28706" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="28729" class="Keyword">open</a> <a id="28734" class="Keyword">import</a> <a id="28741" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="28767" class="Keyword">open</a> <a id="28772" class="Keyword">import</a> <a id="28779" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="28805" class="Keyword">open</a> <a id="28810" class="Keyword">import</a> <a id="28817" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="28873" class="Keyword">open</a> <a id="28878" class="Keyword">import</a> <a id="28885" href="polytopes.html" class="Module">polytopes</a>
<a id="28895" class="Keyword">open</a> <a id="28900" class="Keyword">import</a> <a id="28907" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="28965" class="Keyword">open</a> <a id="28970" class="Keyword">import</a> <a id="28977" href="ring-theory.html" class="Module">ring-theory</a>
<a id="28989" class="Keyword">open</a> <a id="28994" class="Keyword">import</a> <a id="29001" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="29038" class="Keyword">open</a> <a id="29043" class="Keyword">import</a> <a id="29050" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="29077" class="Keyword">open</a> <a id="29082" class="Keyword">import</a> <a id="29089" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="29121" class="Keyword">open</a> <a id="29126" class="Keyword">import</a> <a id="29133" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="29179" class="Keyword">open</a> <a id="29184" class="Keyword">import</a> <a id="29191" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="29216" class="Keyword">open</a> <a id="29221" class="Keyword">import</a> <a id="29228" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="29271" class="Keyword">open</a> <a id="29276" class="Keyword">import</a> <a id="29283" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="29321" class="Keyword">open</a> <a id="29326" class="Keyword">import</a> <a id="29333" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="29364" class="Keyword">open</a> <a id="29369" class="Keyword">import</a> <a id="29376" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="29400" class="Keyword">open</a> <a id="29405" class="Keyword">import</a> <a id="29412" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="29444" class="Keyword">open</a> <a id="29449" class="Keyword">import</a> <a id="29456" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="29482" class="Keyword">open</a> <a id="29487" class="Keyword">import</a> <a id="29494" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="29523" class="Keyword">open</a> <a id="29528" class="Keyword">import</a> <a id="29535" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="29572" class="Keyword">open</a> <a id="29577" class="Keyword">import</a> <a id="29584" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="29613" class="Keyword">open</a> <a id="29618" class="Keyword">import</a> <a id="29625" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="29652" class="Keyword">open</a> <a id="29657" class="Keyword">import</a> <a id="29664" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="29701" class="Keyword">open</a> <a id="29706" class="Keyword">import</a> <a id="29713" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="29740" class="Keyword">open</a> <a id="29745" class="Keyword">import</a> <a id="29752" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="29785" class="Keyword">open</a> <a id="29790" class="Keyword">import</a> <a id="29797" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="29815" class="Keyword">open</a> <a id="29820" class="Keyword">import</a> <a id="29827" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="29881" class="Keyword">open</a> <a id="29886" class="Keyword">import</a> <a id="29893" href="set-theory.html" class="Module">set-theory</a>
<a id="29904" class="Keyword">open</a> <a id="29909" class="Keyword">import</a> <a id="29916" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="29942" class="Keyword">open</a> <a id="29947" class="Keyword">import</a> <a id="29954" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="30016" class="Keyword">open</a> <a id="30021" class="Keyword">import</a> <a id="30028" href="structured-types.html" class="Module">structured-types</a>
<a id="30045" class="Keyword">open</a> <a id="30050" class="Keyword">import</a> <a id="30057" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="30092" class="Keyword">open</a> <a id="30097" class="Keyword">import</a> <a id="30104" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="30148" class="Keyword">open</a> <a id="30153" class="Keyword">import</a> <a id="30160" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="30224" class="Keyword">open</a> <a id="30229" class="Keyword">import</a> <a id="30236" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="30282" class="Keyword">open</a> <a id="30287" class="Keyword">import</a> <a id="30294" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="30318" class="Keyword">open</a> <a id="30323" class="Keyword">import</a> <a id="30330" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="30399" class="Keyword">open</a> <a id="30404" class="Keyword">import</a> <a id="30411" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="30456" class="Keyword">open</a> <a id="30461" class="Keyword">import</a> <a id="30468" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="30502" class="Keyword">open</a> <a id="30507" class="Keyword">import</a> <a id="30514" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="30575" class="Keyword">open</a> <a id="30580" class="Keyword">import</a> <a id="30587" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="30632" class="Keyword">open</a> <a id="30637" class="Keyword">import</a> <a id="30644" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="30682" class="Keyword">open</a> <a id="30687" class="Keyword">import</a> <a id="30694" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="30737" class="Keyword">open</a> <a id="30742" class="Keyword">import</a> <a id="30749" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="30785" class="Keyword">open</a> <a id="30790" class="Keyword">import</a> <a id="30797" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="30827" class="Keyword">open</a> <a id="30832" class="Keyword">import</a> <a id="30839" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="30870" class="Keyword">open</a> <a id="30875" class="Keyword">import</a> <a id="30882" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="30941" class="Keyword">open</a> <a id="30946" class="Keyword">import</a> <a id="30953" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="31004" class="Keyword">open</a> <a id="31009" class="Keyword">import</a> <a id="31016" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="31067" class="Keyword">open</a> <a id="31072" class="Keyword">import</a> <a id="31079" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="31134" class="Keyword">open</a> <a id="31139" class="Keyword">import</a> <a id="31146" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="31175" class="Keyword">open</a> <a id="31180" class="Keyword">import</a> <a id="31187" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="31215" class="Keyword">open</a> <a id="31220" class="Keyword">import</a> <a id="31227" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="31257" class="Keyword">open</a> <a id="31262" class="Keyword">import</a> <a id="31269" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="31303" class="Keyword">open</a> <a id="31308" class="Keyword">import</a> <a id="31315" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="31391" class="Keyword">open</a> <a id="31396" class="Keyword">import</a> <a id="31403" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="31429" class="Keyword">open</a> <a id="31434" class="Keyword">import</a> <a id="31441" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="31480" class="Keyword">open</a> <a id="31485" class="Keyword">import</a> <a id="31492" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="31530" class="Keyword">open</a> <a id="31535" class="Keyword">import</a> <a id="31542" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="31588" class="Keyword">open</a> <a id="31593" class="Keyword">import</a> <a id="31600" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="31637" class="Keyword">open</a> <a id="31642" class="Keyword">import</a> <a id="31649" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="31689" class="Keyword">open</a> <a id="31694" class="Keyword">import</a> <a id="31701" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="31740" class="Keyword">open</a> <a id="31745" class="Keyword">import</a> <a id="31752" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="31785" class="Keyword">open</a> <a id="31790" class="Keyword">import</a> <a id="31797" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="31832" class="Keyword">open</a> <a id="31837" class="Keyword">import</a> <a id="31844" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="31889" class="Keyword">open</a> <a id="31894" class="Keyword">import</a> <a id="31901" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="31953" class="Keyword">open</a> <a id="31958" class="Keyword">import</a> <a id="31965" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="32018" class="Keyword">open</a> <a id="32023" class="Keyword">import</a> <a id="32030" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="32078" class="Keyword">open</a> <a id="32083" class="Keyword">import</a> <a id="32090" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="32130" class="Keyword">open</a> <a id="32135" class="Keyword">import</a> <a id="32142" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="32189" class="Keyword">open</a> <a id="32194" class="Keyword">import</a> <a id="32201" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="32242" class="Keyword">open</a> <a id="32247" class="Keyword">import</a> <a id="32254" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="32292" class="Keyword">open</a> <a id="32297" class="Keyword">import</a> <a id="32304" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="32352" class="Keyword">open</a> <a id="32357" class="Keyword">import</a> <a id="32364" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="32409" class="Keyword">open</a> <a id="32414" class="Keyword">import</a> <a id="32421" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="32470" class="Keyword">open</a> <a id="32475" class="Keyword">import</a> <a id="32482" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="32559" class="Keyword">open</a> <a id="32564" class="Keyword">import</a> <a id="32571" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="32623" class="Keyword">open</a> <a id="32628" class="Keyword">import</a> <a id="32635" href="type-theories.html" class="Module">type-theories</a>
<a id="32649" class="Keyword">open</a> <a id="32654" class="Keyword">import</a> <a id="32661" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="32703" class="Keyword">open</a> <a id="32708" class="Keyword">import</a> <a id="32715" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="32753" class="Keyword">open</a> <a id="32758" class="Keyword">import</a> <a id="32765" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="32811" class="Keyword">open</a> <a id="32816" class="Keyword">import</a> <a id="32823" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="32870" class="Keyword">open</a> <a id="32875" class="Keyword">import</a> <a id="32882" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="32917" class="Keyword">open</a> <a id="32922" class="Keyword">import</a> <a id="32929" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="33007" class="Keyword">open</a> <a id="33012" class="Keyword">import</a> <a id="33019" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="33043" class="Keyword">open</a> <a id="33048" class="Keyword">import</a> <a id="33055" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="33108" class="Keyword">open</a> <a id="33113" class="Keyword">import</a> <a id="33120" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="33163" class="Keyword">open</a> <a id="33168" class="Keyword">import</a> <a id="33175" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="33215" class="Keyword">open</a> <a id="33220" class="Keyword">import</a> <a id="33227" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="33266" class="Keyword">open</a> <a id="33271" class="Keyword">import</a> <a id="33278" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="33312" class="Keyword">open</a> <a id="33317" class="Keyword">import</a> <a id="33324" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="33372" class="Keyword">open</a> <a id="33377" class="Keyword">import</a> <a id="33384" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="33435" class="Keyword">open</a> <a id="33440" class="Keyword">import</a> <a id="33447" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="33494" class="Keyword">open</a> <a id="33499" class="Keyword">import</a> <a id="33506" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="33558" class="Keyword">open</a> <a id="33563" class="Keyword">import</a> <a id="33570" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="33614" class="Keyword">open</a> <a id="33619" class="Keyword">import</a> <a id="33626" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="33666" class="Keyword">open</a> <a id="33671" class="Keyword">import</a> <a id="33678" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="33721" class="Keyword">open</a> <a id="33726" class="Keyword">import</a> <a id="33733" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="33785" class="Keyword">open</a> <a id="33790" class="Keyword">import</a> <a id="33797" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="33851" class="Keyword">open</a> <a id="33856" class="Keyword">import</a> <a id="33863" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="33911" class="Keyword">open</a> <a id="33916" class="Keyword">import</a> <a id="33923" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="33962" class="Keyword">open</a> <a id="33967" class="Keyword">import</a> <a id="33974" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="34007" class="Keyword">open</a> <a id="34012" class="Keyword">import</a> <a id="34019" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="34049" class="Keyword">open</a> <a id="34054" class="Keyword">import</a> <a id="34061" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="34112" class="Keyword">open</a> <a id="34117" class="Keyword">import</a> <a id="34124" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="34165" class="Keyword">open</a> <a id="34170" class="Keyword">import</a> <a id="34177" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="34214" class="Keyword">open</a> <a id="34219" class="Keyword">import</a> <a id="34226" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="34285" class="Keyword">open</a> <a id="34290" class="Keyword">import</a> <a id="34297" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="34352" class="Keyword">open</a> <a id="34357" class="Keyword">import</a> <a id="34364" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="34411" class="Keyword">open</a> <a id="34416" class="Keyword">import</a> <a id="34423" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="34466" class="Keyword">open</a> <a id="34471" class="Keyword">import</a> <a id="34478" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="34523" class="Keyword">open</a> <a id="34528" class="Keyword">import</a> <a id="34535" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="34584" class="Keyword">open</a> <a id="34589" class="Keyword">import</a> <a id="34596" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="34647" class="Keyword">open</a> <a id="34652" class="Keyword">import</a> <a id="34659" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="34703" class="Keyword">open</a> <a id="34708" class="Keyword">import</a> <a id="34715" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="34793" class="Keyword">open</a> <a id="34798" class="Keyword">import</a> <a id="34805" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="34845" class="Keyword">open</a> <a id="34850" class="Keyword">import</a> <a id="34857" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="34914" class="Keyword">open</a> <a id="34919" class="Keyword">import</a> <a id="34926" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="34961" class="Keyword">open</a> <a id="34966" class="Keyword">import</a> <a id="34973" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="35019" class="Keyword">open</a> <a id="35024" class="Keyword">import</a> <a id="35031" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="35086" class="Keyword">open</a> <a id="35091" class="Keyword">import</a> <a id="35098" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="35141" class="Keyword">open</a> <a id="35146" class="Keyword">import</a> <a id="35153" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="35198" class="Keyword">open</a> <a id="35203" class="Keyword">import</a> <a id="35210" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="35269" class="Keyword">open</a> <a id="35274" class="Keyword">import</a> <a id="35281" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="35318" class="Keyword">open</a> <a id="35323" class="Keyword">import</a> <a id="35330" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="35372" class="Keyword">open</a> <a id="35377" class="Keyword">import</a> <a id="35384" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="35425" class="Keyword">open</a> <a id="35430" class="Keyword">import</a> <a id="35437" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="35476" class="Keyword">open</a> <a id="35481" class="Keyword">import</a> <a id="35488" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="35526" class="Keyword">open</a> <a id="35531" class="Keyword">import</a> <a id="35538" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="35590" class="Keyword">open</a> <a id="35595" class="Keyword">import</a> <a id="35602" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="35647" class="Keyword">open</a> <a id="35652" class="Keyword">import</a> <a id="35659" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="35698" class="Keyword">open</a> <a id="35703" class="Keyword">import</a> <a id="35710" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="35747" class="Keyword">open</a> <a id="35752" class="Keyword">import</a> <a id="35759" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="35808" class="Keyword">open</a> <a id="35813" class="Keyword">import</a> <a id="35820" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="35859" class="Keyword">open</a> <a id="35864" class="Keyword">import</a> <a id="35871" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="35909" class="Keyword">open</a> <a id="35914" class="Keyword">import</a> <a id="35921" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="35976" class="Keyword">open</a> <a id="35981" class="Keyword">import</a> <a id="35988" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="36027" class="Keyword">open</a> <a id="36032" class="Keyword">import</a> <a id="36039" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="36087" class="Keyword">open</a> <a id="36092" class="Keyword">import</a> <a id="36099" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="36146" class="Keyword">open</a> <a id="36151" class="Keyword">import</a> <a id="36158" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="36196" class="Keyword">open</a> <a id="36201" class="Keyword">import</a> <a id="36208" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="36238" class="Keyword">open</a> <a id="36243" class="Keyword">import</a> <a id="36250" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="36307" class="Keyword">open</a> <a id="36312" class="Keyword">import</a> <a id="36319" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="36373" class="Keyword">open</a> <a id="36378" class="Keyword">import</a> <a id="36385" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="36415" class="Keyword">open</a> <a id="36420" class="Keyword">import</a> <a id="36427" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="36476" class="Keyword">open</a> <a id="36481" class="Keyword">import</a> <a id="36488" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="36530" class="Keyword">open</a> <a id="36535" class="Keyword">import</a> <a id="36542" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="36576" class="Keyword">open</a> <a id="36581" class="Keyword">import</a> <a id="36588" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="36651" class="Keyword">open</a> <a id="36656" class="Keyword">import</a> <a id="36663" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="36706" class="Keyword">open</a> <a id="36711" class="Keyword">import</a> <a id="36718" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="36753" class="Keyword">open</a> <a id="36758" class="Keyword">import</a> <a id="36765" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="36800" class="Keyword">open</a> <a id="36805" class="Keyword">import</a> <a id="36812" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="36852" class="Keyword">open</a> <a id="36857" class="Keyword">import</a> <a id="36864" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="36909" class="Keyword">open</a> <a id="36914" class="Keyword">import</a> <a id="36921" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="36962" class="Keyword">open</a> <a id="36967" class="Keyword">import</a> <a id="36974" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="37028" class="Keyword">open</a> <a id="37033" class="Keyword">import</a> <a id="37040" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="37090" class="Keyword">open</a> <a id="37095" class="Keyword">import</a> <a id="37102" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="37140" class="Keyword">open</a> <a id="37145" class="Keyword">import</a> <a id="37152" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="37201" class="Keyword">open</a> <a id="37206" class="Keyword">import</a> <a id="37213" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="37260" class="Keyword">open</a> <a id="37265" class="Keyword">import</a> <a id="37272" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="37335" class="Keyword">open</a> <a id="37340" class="Keyword">import</a> <a id="37347" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="37379" class="Keyword">open</a> <a id="37384" class="Keyword">import</a> <a id="37391" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="37444" class="Keyword">open</a> <a id="37449" class="Keyword">import</a> <a id="37456" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="37502" class="Keyword">open</a> <a id="37507" class="Keyword">import</a> <a id="37514" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="37560" class="Keyword">open</a> <a id="37565" class="Keyword">import</a> <a id="37572" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="37620" class="Keyword">open</a> <a id="37625" class="Keyword">import</a> <a id="37632" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="37672" class="Keyword">open</a> <a id="37677" class="Keyword">import</a> <a id="37684" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="37729" class="Keyword">open</a> <a id="37734" class="Keyword">import</a> <a id="37741" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="37806" class="Keyword">open</a> <a id="37811" class="Keyword">import</a> <a id="37818" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="37863" class="Keyword">open</a> <a id="37868" class="Keyword">import</a> <a id="37875" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="37922" class="Keyword">open</a> <a id="37927" class="Keyword">import</a> <a id="37934" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="37987" class="Keyword">open</a> <a id="37992" class="Keyword">import</a> <a id="37999" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>