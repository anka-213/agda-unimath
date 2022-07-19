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
<a id="13160" class="Keyword">open</a> <a id="13165" class="Keyword">import</a> <a id="13172" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13206" class="Keyword">open</a> <a id="13211" class="Keyword">import</a> <a id="13218" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13241" class="Keyword">open</a> <a id="13246" class="Keyword">import</a> <a id="13253" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13280" class="Keyword">open</a> <a id="13285" class="Keyword">import</a> <a id="13292" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="13320" class="Keyword">open</a> <a id="13325" class="Keyword">import</a> <a id="13332" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="13369" class="Keyword">open</a> <a id="13374" class="Keyword">import</a> <a id="13381" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="13429" class="Keyword">open</a> <a id="13434" class="Keyword">import</a> <a id="13441" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13481" class="Keyword">open</a> <a id="13486" class="Keyword">import</a> <a id="13493" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13515" class="Keyword">open</a> <a id="13520" class="Keyword">import</a> <a id="13527" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13550" class="Keyword">open</a> <a id="13555" class="Keyword">import</a> <a id="13562" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13587" class="Keyword">open</a> <a id="13592" class="Keyword">import</a> <a id="13599" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13644" class="Keyword">open</a> <a id="13649" class="Keyword">import</a> <a id="13656" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13700" class="Keyword">open</a> <a id="13705" class="Keyword">import</a> <a id="13712" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13748" class="Keyword">open</a> <a id="13753" class="Keyword">import</a> <a id="13760" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13805" class="Keyword">open</a> <a id="13810" class="Keyword">import</a> <a id="13817" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13858" class="Keyword">open</a> <a id="13863" class="Keyword">import</a> <a id="13870" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13905" class="Keyword">open</a> <a id="13910" class="Keyword">import</a> <a id="13917" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13949" class="Keyword">open</a> <a id="13954" class="Keyword">import</a> <a id="13961" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13992" class="Keyword">open</a> <a id="13997" class="Keyword">import</a> <a id="14004" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14037" class="Keyword">open</a> <a id="14042" class="Keyword">import</a> <a id="14049" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14082" class="Keyword">open</a> <a id="14087" class="Keyword">import</a> <a id="14094" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14124" class="Keyword">open</a> <a id="14129" class="Keyword">import</a> <a id="14136" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14160" class="Keyword">open</a> <a id="14165" class="Keyword">import</a> <a id="14172" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14210" class="Keyword">open</a> <a id="14215" class="Keyword">import</a> <a id="14222" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14253" class="Keyword">open</a> <a id="14258" class="Keyword">import</a> <a id="14265" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14290" class="Keyword">open</a> <a id="14295" class="Keyword">import</a> <a id="14302" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="14330" class="Keyword">open</a> <a id="14335" class="Keyword">import</a> <a id="14342" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="14366" class="Keyword">open</a> <a id="14371" class="Keyword">import</a> <a id="14378" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="14404" class="Keyword">open</a> <a id="14409" class="Keyword">import</a> <a id="14416" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14451" class="Keyword">open</a> <a id="14456" class="Keyword">import</a> <a id="14463" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14484" class="Keyword">open</a> <a id="14489" class="Keyword">import</a> <a id="14496" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14545" class="Keyword">open</a> <a id="14550" class="Keyword">import</a> <a id="14557" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14598" class="Keyword">open</a> <a id="14603" class="Keyword">import</a> <a id="14610" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14660" class="Keyword">open</a> <a id="14665" class="Keyword">import</a> <a id="14672" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14718" class="Keyword">open</a> <a id="14723" class="Keyword">import</a> <a id="14730" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14770" class="Keyword">open</a> <a id="14775" class="Keyword">import</a> <a id="14782" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14832" class="Keyword">open</a> <a id="14837" class="Keyword">import</a> <a id="14844" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14883" class="Keyword">open</a> <a id="14888" class="Keyword">import</a> <a id="14895" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14935" class="Keyword">open</a> <a id="14940" class="Keyword">import</a> <a id="14947" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14980" class="Keyword">open</a> <a id="14985" class="Keyword">import</a> <a id="14992" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15041" class="Keyword">open</a> <a id="15046" class="Keyword">import</a> <a id="15053" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15078" class="Keyword">open</a> <a id="15083" class="Keyword">import</a> <a id="15090" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15128" class="Keyword">open</a> <a id="15133" class="Keyword">import</a> <a id="15140" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15162" class="Keyword">open</a> <a id="15167" class="Keyword">import</a> <a id="15174" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="15202" class="Keyword">open</a> <a id="15207" class="Keyword">import</a> <a id="15214" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="15250" class="Keyword">open</a> <a id="15255" class="Keyword">import</a> <a id="15262" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="15288" class="Keyword">open</a> <a id="15293" class="Keyword">import</a> <a id="15300" href="foundation.images.html" class="Module">foundation.images</a>
<a id="15318" class="Keyword">open</a> <a id="15323" class="Keyword">import</a> <a id="15330" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="15365" class="Keyword">open</a> <a id="15370" class="Keyword">import</a> <a id="15377" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="15412" class="Keyword">open</a> <a id="15417" class="Keyword">import</a> <a id="15424" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15451" class="Keyword">open</a> <a id="15456" class="Keyword">import</a> <a id="15463" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15519" class="Keyword">open</a> <a id="15524" class="Keyword">import</a> <a id="15531" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15560" class="Keyword">open</a> <a id="15565" class="Keyword">import</a> <a id="15572" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15602" class="Keyword">open</a> <a id="15607" class="Keyword">import</a> <a id="15614" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15641" class="Keyword">open</a> <a id="15646" class="Keyword">import</a> <a id="15653" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15679" class="Keyword">open</a> <a id="15684" class="Keyword">import</a> <a id="15691" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15718" class="Keyword">open</a> <a id="15723" class="Keyword">import</a> <a id="15730" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15754" class="Keyword">open</a> <a id="15759" class="Keyword">import</a> <a id="15766" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15789" class="Keyword">open</a> <a id="15794" class="Keyword">import</a> <a id="15801" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15828" class="Keyword">open</a> <a id="15833" class="Keyword">import</a> <a id="15840" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15872" class="Keyword">open</a> <a id="15877" class="Keyword">import</a> <a id="15884" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15919" class="Keyword">open</a> <a id="15924" class="Keyword">import</a> <a id="15931" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15962" class="Keyword">open</a> <a id="15967" class="Keyword">import</a> <a id="15974" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16007" class="Keyword">open</a> <a id="16012" class="Keyword">import</a> <a id="16019" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16053" class="Keyword">open</a> <a id="16058" class="Keyword">import</a> <a id="16065" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16105" class="Keyword">open</a> <a id="16110" class="Keyword">import</a> <a id="16117" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="16148" class="Keyword">open</a> <a id="16153" class="Keyword">import</a> <a id="16160" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="16192" class="Keyword">open</a> <a id="16197" class="Keyword">import</a> <a id="16204" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="16235" class="Keyword">open</a> <a id="16240" class="Keyword">import</a> <a id="16247" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="16264" class="Keyword">open</a> <a id="16269" class="Keyword">import</a> <a id="16276" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="16301" class="Keyword">open</a> <a id="16306" class="Keyword">import</a> <a id="16313" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="16342" class="Keyword">open</a> <a id="16347" class="Keyword">import</a> <a id="16354" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="16379" class="Keyword">open</a> <a id="16384" class="Keyword">import</a> <a id="16391" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="16412" class="Keyword">open</a> <a id="16417" class="Keyword">import</a> <a id="16424" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16448" class="Keyword">open</a> <a id="16453" class="Keyword">import</a> <a id="16460" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16480" class="Keyword">open</a> <a id="16485" class="Keyword">import</a> <a id="16492" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16526" class="Keyword">open</a> <a id="16531" class="Keyword">import</a> <a id="16538" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16576" class="Keyword">open</a> <a id="16581" class="Keyword">import</a> <a id="16588" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16616" class="Keyword">open</a> <a id="16621" class="Keyword">import</a> <a id="16628" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16652" class="Keyword">open</a> <a id="16657" class="Keyword">import</a> <a id="16664" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16691" class="Keyword">open</a> <a id="16696" class="Keyword">import</a> <a id="16703" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16738" class="Keyword">open</a> <a id="16743" class="Keyword">import</a> <a id="16750" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16771" class="Keyword">open</a> <a id="16776" class="Keyword">import</a> <a id="16783" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16819" class="Keyword">open</a> <a id="16824" class="Keyword">import</a> <a id="16831" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16876" class="Keyword">open</a> <a id="16881" class="Keyword">import</a> <a id="16888" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16934" class="Keyword">open</a> <a id="16939" class="Keyword">import</a> <a id="16946" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16986" class="Keyword">open</a> <a id="16991" class="Keyword">import</a> <a id="16998" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17028" class="Keyword">open</a> <a id="17033" class="Keyword">import</a> <a id="17040" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="17074" class="Keyword">open</a> <a id="17079" class="Keyword">import</a> <a id="17086" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="17123" class="Keyword">open</a> <a id="17128" class="Keyword">import</a> <a id="17135" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="17159" class="Keyword">open</a> <a id="17164" class="Keyword">import</a> <a id="17171" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="17192" class="Keyword">open</a> <a id="17197" class="Keyword">import</a> <a id="17204" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="17239" class="Keyword">open</a> <a id="17244" class="Keyword">import</a> <a id="17251" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="17288" class="Keyword">open</a> <a id="17293" class="Keyword">import</a> <a id="17300" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="17349" class="Keyword">open</a> <a id="17354" class="Keyword">import</a> <a id="17361" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="17394" class="Keyword">open</a> <a id="17399" class="Keyword">import</a> <a id="17406" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="17429" class="Keyword">open</a> <a id="17434" class="Keyword">import</a> <a id="17441" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17464" class="Keyword">open</a> <a id="17469" class="Keyword">import</a> <a id="17476" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17499" class="Keyword">open</a> <a id="17504" class="Keyword">import</a> <a id="17511" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17539" class="Keyword">open</a> <a id="17544" class="Keyword">import</a> <a id="17551" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17571" class="Keyword">open</a> <a id="17576" class="Keyword">import</a> <a id="17583" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17604" class="Keyword">open</a> <a id="17609" class="Keyword">import</a> <a id="17616" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17647" class="Keyword">open</a> <a id="17652" class="Keyword">import</a> <a id="17659" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17686" class="Keyword">open</a> <a id="17691" class="Keyword">import</a> <a id="17698" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17714" class="Keyword">open</a> <a id="17719" class="Keyword">import</a> <a id="17726" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17757" class="Keyword">open</a> <a id="17762" class="Keyword">import</a> <a id="17769" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17786" class="Keyword">open</a> <a id="17791" class="Keyword">import</a> <a id="17798" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17820" class="Keyword">open</a> <a id="17825" class="Keyword">import</a> <a id="17832" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17859" class="Keyword">open</a> <a id="17864" class="Keyword">import</a> <a id="17871" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17894" class="Keyword">open</a> <a id="17899" class="Keyword">import</a> <a id="17906" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17933" class="Keyword">open</a> <a id="17938" class="Keyword">import</a> <a id="17945" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17978" class="Keyword">open</a> <a id="17983" class="Keyword">import</a> <a id="17990" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18030" class="Keyword">open</a> <a id="18035" class="Keyword">import</a> <a id="18042" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="18063" class="Keyword">open</a> <a id="18068" class="Keyword">import</a> <a id="18075" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="18104" class="Keyword">open</a> <a id="18109" class="Keyword">import</a> <a id="18116" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="18154" class="Keyword">open</a> <a id="18159" class="Keyword">import</a> <a id="18166" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="18186" class="Keyword">open</a> <a id="18191" class="Keyword">import</a> <a id="18198" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="18222" class="Keyword">open</a> <a id="18227" class="Keyword">import</a> <a id="18234" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="18261" class="Keyword">open</a> <a id="18266" class="Keyword">import</a> <a id="18273" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="18305" class="Keyword">open</a> <a id="18310" class="Keyword">import</a> <a id="18317" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="18347" class="Keyword">open</a> <a id="18352" class="Keyword">import</a> <a id="18359" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="18385" class="Keyword">open</a> <a id="18390" class="Keyword">import</a> <a id="18397" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="18424" class="Keyword">open</a> <a id="18429" class="Keyword">import</a> <a id="18436" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="18473" class="Keyword">open</a> <a id="18478" class="Keyword">import</a> <a id="18485" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18514" class="Keyword">open</a> <a id="18519" class="Keyword">import</a> <a id="18526" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18549" class="Keyword">open</a> <a id="18554" class="Keyword">import</a> <a id="18561" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18612" class="Keyword">open</a> <a id="18617" class="Keyword">import</a> <a id="18624" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18667" class="Keyword">open</a> <a id="18672" class="Keyword">import</a> <a id="18679" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="18731" class="Keyword">open</a> <a id="18736" class="Keyword">import</a> <a id="18743" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18791" class="Keyword">open</a> <a id="18796" class="Keyword">import</a> <a id="18803" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18841" class="Keyword">open</a> <a id="18846" class="Keyword">import</a> <a id="18853" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18890" class="Keyword">open</a> <a id="18895" class="Keyword">import</a> <a id="18902" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18948" class="Keyword">open</a> <a id="18953" class="Keyword">import</a> <a id="18960" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18977" class="Keyword">open</a> <a id="18982" class="Keyword">import</a> <a id="18989" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="19017" class="Keyword">open</a> <a id="19022" class="Keyword">import</a> <a id="19029" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="19057" class="Keyword">open</a> <a id="19062" class="Keyword">import</a> <a id="19069" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="19105" class="Keyword">open</a> <a id="19110" class="Keyword">import</a> <a id="19117" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19155" class="Keyword">open</a> <a id="19160" class="Keyword">import</a> <a id="19167" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19200" class="Keyword">open</a> <a id="19205" class="Keyword">import</a> <a id="19212" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19233" class="Keyword">open</a> <a id="19238" class="Keyword">import</a> <a id="19245" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19281" class="Keyword">open</a> <a id="19286" class="Keyword">import</a> <a id="19293" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19347" class="Keyword">open</a> <a id="19352" class="Keyword">import</a> <a id="19359" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19381" class="Keyword">open</a> <a id="19386" class="Keyword">import</a> <a id="19393" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19428" class="Keyword">open</a> <a id="19433" class="Keyword">import</a> <a id="19440" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19470" class="Keyword">open</a> <a id="19475" class="Keyword">import</a> <a id="19482" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19521" class="Keyword">open</a> <a id="19526" class="Keyword">import</a> <a id="19533" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19587" class="Keyword">open</a> <a id="19592" class="Keyword">import</a> <a id="19599" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19645" class="Keyword">open</a> <a id="19650" class="Keyword">import</a> <a id="19657" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19708" class="Keyword">open</a> <a id="19713" class="Keyword">import</a> <a id="19720" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19761" class="Keyword">open</a> <a id="19766" class="Keyword">import</a> <a id="19773" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19818" class="Keyword">open</a> <a id="19823" class="Keyword">import</a> <a id="19830" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19875" class="Keyword">open</a> <a id="19880" class="Keyword">import</a> <a id="19887" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19923" class="Keyword">open</a> <a id="19928" class="Keyword">import</a> <a id="19935" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19971" class="Keyword">open</a> <a id="19976" class="Keyword">import</a> <a id="19983" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="20048" class="Keyword">open</a> <a id="20053" class="Keyword">import</a> <a id="20060" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="20115" class="Keyword">open</a> <a id="20120" class="Keyword">import</a> <a id="20127" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20167" class="Keyword">open</a> <a id="20172" class="Keyword">import</a> <a id="20179" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20223" class="Keyword">open</a> <a id="20228" class="Keyword">import</a> <a id="20235" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20280" class="Keyword">open</a> <a id="20285" class="Keyword">import</a> <a id="20292" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20333" class="Keyword">open</a> <a id="20338" class="Keyword">import</a> <a id="20345" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20385" class="Keyword">open</a> <a id="20390" class="Keyword">import</a> <a id="20397" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20424" class="Keyword">open</a> <a id="20429" class="Keyword">import</a> <a id="20436" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20472" class="Keyword">open</a> <a id="20477" class="Keyword">import</a> <a id="20484" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20511" class="Keyword">open</a> <a id="20516" class="Keyword">import</a> <a id="20523" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20560" class="Keyword">open</a> <a id="20565" class="Keyword">import</a> <a id="20572" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20600" class="Keyword">open</a> <a id="20605" class="Keyword">import</a> <a id="20612" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20631" class="Keyword">open</a> <a id="20636" class="Keyword">import</a> <a id="20643" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20683" class="Keyword">open</a> <a id="20688" class="Keyword">import</a> <a id="20695" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20727" class="Keyword">open</a> <a id="20732" class="Keyword">import</a> <a id="20739" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20787" class="Keyword">open</a> <a id="20792" class="Keyword">import</a> <a id="20799" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20822" class="Keyword">open</a> <a id="20827" class="Keyword">import</a> <a id="20834" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20858" class="Keyword">open</a> <a id="20863" class="Keyword">import</a> <a id="20870" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20910" class="Keyword">open</a> <a id="20915" class="Keyword">import</a> <a id="20922" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20965" class="Keyword">open</a> <a id="20970" class="Keyword">import</a> <a id="20977" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="21011" class="Keyword">open</a> <a id="21016" class="Keyword">import</a> <a id="21023" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="21055" class="Keyword">open</a> <a id="21060" class="Keyword">import</a> <a id="21067" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="21097" class="Keyword">open</a> <a id="21102" class="Keyword">import</a> <a id="21109" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="21143" class="Keyword">open</a> <a id="21148" class="Keyword">import</a> <a id="21155" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21190" class="Keyword">open</a> <a id="21195" class="Keyword">import</a> <a id="21202" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21239" class="Keyword">open</a> <a id="21244" class="Keyword">import</a> <a id="21251" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21278" class="Keyword">open</a> <a id="21283" class="Keyword">import</a> <a id="21290" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21318" class="Keyword">open</a> <a id="21323" class="Keyword">import</a> <a id="21330" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21379" class="Keyword">open</a> <a id="21384" class="Keyword">import</a> <a id="21391" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21437" class="Keyword">open</a> <a id="21442" class="Keyword">import</a> <a id="21449" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21489" class="Keyword">open</a> <a id="21494" class="Keyword">import</a> <a id="21501" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21539" class="Keyword">open</a> <a id="21544" class="Keyword">import</a> <a id="21551" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21580" class="Keyword">open</a> <a id="21585" class="Keyword">import</a> <a id="21592" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21622" class="Keyword">open</a> <a id="21627" class="Keyword">import</a> <a id="21634" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21665" class="Keyword">open</a> <a id="21670" class="Keyword">import</a> <a id="21677" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21717" class="Keyword">open</a> <a id="21722" class="Keyword">import</a> <a id="21729" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21755" class="Keyword">open</a> <a id="21760" class="Keyword">import</a> <a id="21767" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21822" class="Keyword">open</a> <a id="21827" class="Keyword">import</a> <a id="21834" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21885" class="Keyword">open</a> <a id="21890" class="Keyword">import</a> <a id="21897" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21942" class="Keyword">open</a> <a id="21947" class="Keyword">import</a> <a id="21954" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="22008" class="Keyword">open</a> <a id="22013" class="Keyword">import</a> <a id="22020" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="22047" class="Keyword">open</a> <a id="22052" class="Keyword">import</a> <a id="22059" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="22092" class="Keyword">open</a> <a id="22097" class="Keyword">import</a> <a id="22104" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="22135" class="Keyword">open</a> <a id="22140" class="Keyword">import</a> <a id="22147" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22184" class="Keyword">open</a> <a id="22189" class="Keyword">import</a> <a id="22196" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22221" class="Keyword">open</a> <a id="22226" class="Keyword">import</a> <a id="22233" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22265" class="Keyword">open</a> <a id="22270" class="Keyword">import</a> <a id="22277" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22312" class="Keyword">open</a> <a id="22317" class="Keyword">import</a> <a id="22324" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22353" class="Keyword">open</a> <a id="22358" class="Keyword">import</a> <a id="22365" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22391" class="Keyword">open</a> <a id="22396" class="Keyword">import</a> <a id="22403" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22431" class="Keyword">open</a> <a id="22436" class="Keyword">import</a> <a id="22443" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22468" class="Keyword">open</a> <a id="22473" class="Keyword">import</a> <a id="22480" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22501" class="Keyword">open</a> <a id="22506" class="Keyword">import</a> <a id="22513" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22549" class="Keyword">open</a> <a id="22554" class="Keyword">import</a> <a id="22561" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22604" class="Keyword">open</a> <a id="22609" class="Keyword">import</a> <a id="22616" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22641" class="Keyword">open</a> <a id="22646" class="Keyword">import</a> <a id="22653" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22684" class="Keyword">open</a> <a id="22689" class="Keyword">import</a> <a id="22696" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22728" class="Keyword">open</a> <a id="22733" class="Keyword">import</a> <a id="22740" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22774" class="Keyword">open</a> <a id="22779" class="Keyword">import</a> <a id="22786" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22842" class="Keyword">open</a> <a id="22847" class="Keyword">import</a> <a id="22854" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22907" class="Keyword">open</a> <a id="22912" class="Keyword">import</a> <a id="22919" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22946" class="Keyword">open</a> <a id="22951" class="Keyword">import</a> <a id="22958" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="23003" class="Keyword">open</a> <a id="23008" class="Keyword">import</a> <a id="23015" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="23077" class="Keyword">open</a> <a id="23082" class="Keyword">import</a> <a id="23089" href="graph-theory.html" class="Module">graph-theory</a>
<a id="23102" class="Keyword">open</a> <a id="23107" class="Keyword">import</a> <a id="23114" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23154" class="Keyword">open</a> <a id="23159" class="Keyword">import</a> <a id="23166" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23210" class="Keyword">open</a> <a id="23215" class="Keyword">import</a> <a id="23222" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23261" class="Keyword">open</a> <a id="23266" class="Keyword">import</a> <a id="23273" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23315" class="Keyword">open</a> <a id="23320" class="Keyword">import</a> <a id="23327" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23367" class="Keyword">open</a> <a id="23372" class="Keyword">import</a> <a id="23379" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23420" class="Keyword">open</a> <a id="23425" class="Keyword">import</a> <a id="23432" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23470" class="Keyword">open</a> <a id="23475" class="Keyword">import</a> <a id="23482" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23545" class="Keyword">open</a> <a id="23550" class="Keyword">import</a> <a id="23557" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23586" class="Keyword">open</a> <a id="23591" class="Keyword">import</a> <a id="23598" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23643" class="Keyword">open</a> <a id="23648" class="Keyword">import</a> <a id="23655" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23697" class="Keyword">open</a> <a id="23702" class="Keyword">import</a> <a id="23709" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23753" class="Keyword">open</a> <a id="23758" class="Keyword">import</a> <a id="23765" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23814" class="Keyword">open</a> <a id="23819" class="Keyword">import</a> <a id="23826" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23876" class="Keyword">open</a> <a id="23881" class="Keyword">import</a> <a id="23888" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23915" class="Keyword">open</a> <a id="23920" class="Keyword">import</a> <a id="23927" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="23952" class="Keyword">open</a> <a id="23957" class="Keyword">import</a> <a id="23964" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="24005" class="Keyword">open</a> <a id="24010" class="Keyword">import</a> <a id="24017" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="24040" class="Keyword">open</a> <a id="24045" class="Keyword">import</a> <a id="24052" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="24101" class="Keyword">open</a> <a id="24106" class="Keyword">import</a> <a id="24113" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="24152" class="Keyword">open</a> <a id="24157" class="Keyword">import</a> <a id="24164" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24205" class="Keyword">open</a> <a id="24210" class="Keyword">import</a> <a id="24217" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24261" class="Keyword">open</a> <a id="24266" class="Keyword">import</a> <a id="24273" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24310" class="Keyword">open</a> <a id="24315" class="Keyword">import</a> <a id="24322" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24344" class="Keyword">open</a> <a id="24349" class="Keyword">import</a> <a id="24356" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24386" class="Keyword">open</a> <a id="24391" class="Keyword">import</a> <a id="24398" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24437" class="Keyword">open</a> <a id="24442" class="Keyword">import</a> <a id="24449" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24487" class="Keyword">open</a> <a id="24492" class="Keyword">import</a> <a id="24499" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24557" class="Keyword">open</a> <a id="24562" class="Keyword">import</a> <a id="24569" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24634" class="Keyword">open</a> <a id="24639" class="Keyword">import</a> <a id="24646" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24677" class="Keyword">open</a> <a id="24682" class="Keyword">import</a> <a id="24689" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24716" class="Keyword">open</a> <a id="24721" class="Keyword">import</a> <a id="24728" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24786" class="Keyword">open</a> <a id="24791" class="Keyword">import</a> <a id="24798" href="group-theory.html" class="Module">group-theory</a>
<a id="24811" class="Keyword">open</a> <a id="24816" class="Keyword">import</a> <a id="24823" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24851" class="Keyword">open</a> <a id="24856" class="Keyword">import</a> <a id="24863" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24914" class="Keyword">open</a> <a id="24919" class="Keyword">import</a> <a id="24926" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24959" class="Keyword">open</a> <a id="24964" class="Keyword">import</a> <a id="24971" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="25018" class="Keyword">open</a> <a id="25023" class="Keyword">import</a> <a id="25030" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="25069" class="Keyword">open</a> <a id="25074" class="Keyword">import</a> <a id="25081" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="25121" class="Keyword">open</a> <a id="25126" class="Keyword">import</a> <a id="25133" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25176" class="Keyword">open</a> <a id="25181" class="Keyword">import</a> <a id="25188" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25220" class="Keyword">open</a> <a id="25225" class="Keyword">import</a> <a id="25232" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25268" class="Keyword">open</a> <a id="25273" class="Keyword">import</a> <a id="25280" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25309" class="Keyword">open</a> <a id="25314" class="Keyword">import</a> <a id="25321" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25349" class="Keyword">open</a> <a id="25354" class="Keyword">import</a> <a id="25361" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25394" class="Keyword">open</a> <a id="25399" class="Keyword">import</a> <a id="25406" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25442" class="Keyword">open</a> <a id="25447" class="Keyword">import</a> <a id="25454" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25483" class="Keyword">open</a> <a id="25488" class="Keyword">import</a> <a id="25495" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25520" class="Keyword">open</a> <a id="25525" class="Keyword">import</a> <a id="25532" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25594" class="Keyword">open</a> <a id="25599" class="Keyword">import</a> <a id="25606" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25637" class="Keyword">open</a> <a id="25642" class="Keyword">import</a> <a id="25649" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25696" class="Keyword">open</a> <a id="25701" class="Keyword">import</a> <a id="25708" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25741" class="Keyword">open</a> <a id="25746" class="Keyword">import</a> <a id="25753" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="25802" class="Keyword">open</a> <a id="25807" class="Keyword">import</a> <a id="25814" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25854" class="Keyword">open</a> <a id="25859" class="Keyword">import</a> <a id="25866" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25903" class="Keyword">open</a> <a id="25908" class="Keyword">import</a> <a id="25915" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="25962" class="Keyword">open</a> <a id="25967" class="Keyword">import</a> <a id="25974" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="26015" class="Keyword">open</a> <a id="26020" class="Keyword">import</a> <a id="26027" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="26066" class="Keyword">open</a> <a id="26071" class="Keyword">import</a> <a id="26078" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="26110" class="Keyword">open</a> <a id="26115" class="Keyword">import</a> <a id="26122" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="26149" class="Keyword">open</a> <a id="26154" class="Keyword">import</a> <a id="26161" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26181" class="Keyword">open</a> <a id="26186" class="Keyword">import</a> <a id="26193" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26227" class="Keyword">open</a> <a id="26232" class="Keyword">import</a> <a id="26239" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26266" class="Keyword">open</a> <a id="26271" class="Keyword">import</a> <a id="26278" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26320" class="Keyword">open</a> <a id="26325" class="Keyword">import</a> <a id="26332" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26382" class="Keyword">open</a> <a id="26387" class="Keyword">import</a> <a id="26394" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26441" class="Keyword">open</a> <a id="26446" class="Keyword">import</a> <a id="26453" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="26494" class="Keyword">open</a> <a id="26499" class="Keyword">import</a> <a id="26506" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26540" class="Keyword">open</a> <a id="26545" class="Keyword">import</a> <a id="26552" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="26593" class="Keyword">open</a> <a id="26598" class="Keyword">import</a> <a id="26605" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="26640" class="Keyword">open</a> <a id="26645" class="Keyword">import</a> <a id="26652" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="26690" class="Keyword">open</a> <a id="26695" class="Keyword">import</a> <a id="26702" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="26737" class="Keyword">open</a> <a id="26742" class="Keyword">import</a> <a id="26749" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26781" class="Keyword">open</a> <a id="26786" class="Keyword">import</a> <a id="26793" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="26834" class="Keyword">open</a> <a id="26839" class="Keyword">import</a> <a id="26846" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="26887" class="Keyword">open</a> <a id="26892" class="Keyword">import</a> <a id="26899" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26939" class="Keyword">open</a> <a id="26944" class="Keyword">import</a> <a id="26951" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26984" class="Keyword">open</a> <a id="26989" class="Keyword">import</a> <a id="26996" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="27033" class="Keyword">open</a> <a id="27038" class="Keyword">import</a> <a id="27045" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="27075" class="Keyword">open</a> <a id="27080" class="Keyword">import</a> <a id="27087" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="27108" class="Keyword">open</a> <a id="27113" class="Keyword">import</a> <a id="27120" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="27174" class="Keyword">open</a> <a id="27179" class="Keyword">import</a> <a id="27186" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27231" class="Keyword">open</a> <a id="27236" class="Keyword">import</a> <a id="27243" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27271" class="Keyword">open</a> <a id="27276" class="Keyword">import</a> <a id="27283" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27304" class="Keyword">open</a> <a id="27309" class="Keyword">import</a> <a id="27316" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27359" class="Keyword">open</a> <a id="27364" class="Keyword">import</a> <a id="27371" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27405" class="Keyword">open</a> <a id="27410" class="Keyword">import</a> <a id="27417" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27447" class="Keyword">open</a> <a id="27452" class="Keyword">import</a> <a id="27459" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="27505" class="Keyword">open</a> <a id="27510" class="Keyword">import</a> <a id="27517" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="27571" class="Keyword">open</a> <a id="27576" class="Keyword">import</a> <a id="27583" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="27626" class="Keyword">open</a> <a id="27631" class="Keyword">import</a> <a id="27638" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="27672" class="Keyword">open</a> <a id="27677" class="Keyword">import</a> <a id="27684" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="27725" class="Keyword">open</a> <a id="27730" class="Keyword">import</a> <a id="27737" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="27772" class="Keyword">open</a> <a id="27777" class="Keyword">import</a> <a id="27784" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="27826" class="Keyword">open</a> <a id="27831" class="Keyword">import</a> <a id="27838" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="27873" class="Keyword">open</a> <a id="27878" class="Keyword">import</a> <a id="27885" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="27924" class="Keyword">open</a> <a id="27929" class="Keyword">import</a> <a id="27936" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="27973" class="Keyword">open</a> <a id="27978" class="Keyword">import</a> <a id="27985" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="28032" class="Keyword">open</a> <a id="28037" class="Keyword">import</a> <a id="28044" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="28108" class="Keyword">open</a> <a id="28113" class="Keyword">import</a> <a id="28120" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="28165" class="Keyword">open</a> <a id="28170" class="Keyword">import</a> <a id="28177" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="28201" class="Keyword">open</a> <a id="28206" class="Keyword">import</a> <a id="28213" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="28238" class="Keyword">open</a> <a id="28243" class="Keyword">import</a> <a id="28250" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28293" class="Keyword">open</a> <a id="28298" class="Keyword">import</a> <a id="28305" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28336" class="Keyword">open</a> <a id="28341" class="Keyword">import</a> <a id="28348" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28402" class="Keyword">open</a> <a id="28407" class="Keyword">import</a> <a id="28414" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28437" class="Keyword">open</a> <a id="28442" class="Keyword">import</a> <a id="28449" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="28487" class="Keyword">open</a> <a id="28492" class="Keyword">import</a> <a id="28499" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="28538" class="Keyword">open</a> <a id="28543" class="Keyword">import</a> <a id="28550" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="28601" class="Keyword">open</a> <a id="28606" class="Keyword">import</a> <a id="28613" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="28650" class="Keyword">open</a> <a id="28655" class="Keyword">import</a> <a id="28662" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="28719" class="Keyword">open</a> <a id="28724" class="Keyword">import</a> <a id="28731" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="28779" class="Keyword">open</a> <a id="28784" class="Keyword">import</a> <a id="28791" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="28821" class="Keyword">open</a> <a id="28826" class="Keyword">import</a> <a id="28833" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="28870" class="Keyword">open</a> <a id="28875" class="Keyword">import</a> <a id="28882" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="28903" class="Keyword">open</a> <a id="28908" class="Keyword">import</a> <a id="28915" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="28962" class="Keyword">open</a> <a id="28967" class="Keyword">import</a> <a id="28974" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="29012" class="Keyword">open</a> <a id="29017" class="Keyword">import</a> <a id="29024" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="29118" class="Keyword">open</a> <a id="29123" class="Keyword">import</a> <a id="29130" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="29145" class="Keyword">open</a> <a id="29150" class="Keyword">import</a> <a id="29157" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="29190" class="Keyword">open</a> <a id="29195" class="Keyword">import</a> <a id="29202" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="29234" class="Keyword">open</a> <a id="29239" class="Keyword">import</a> <a id="29246" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29288" class="Keyword">open</a> <a id="29293" class="Keyword">import</a> <a id="29300" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29338" class="Keyword">open</a> <a id="29343" class="Keyword">import</a> <a id="29350" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29387" class="Keyword">open</a> <a id="29392" class="Keyword">import</a> <a id="29399" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29432" class="Keyword">open</a> <a id="29437" class="Keyword">import</a> <a id="29444" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="29468" class="Keyword">open</a> <a id="29473" class="Keyword">import</a> <a id="29480" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="29519" class="Keyword">open</a> <a id="29524" class="Keyword">import</a> <a id="29531" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="29577" class="Keyword">open</a> <a id="29582" class="Keyword">import</a> <a id="29589" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="29634" class="Keyword">open</a> <a id="29639" class="Keyword">import</a> <a id="29646" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="29684" class="Keyword">open</a> <a id="29689" class="Keyword">import</a> <a id="29696" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="29728" class="Keyword">open</a> <a id="29733" class="Keyword">import</a> <a id="29740" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="29793" class="Keyword">open</a> <a id="29798" class="Keyword">import</a> <a id="29805" href="order-theory.html" class="Module">order-theory</a>
<a id="29818" class="Keyword">open</a> <a id="29823" class="Keyword">import</a> <a id="29830" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="29857" class="Keyword">open</a> <a id="29862" class="Keyword">import</a> <a id="29869" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="29899" class="Keyword">open</a> <a id="29904" class="Keyword">import</a> <a id="29911" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="29944" class="Keyword">open</a> <a id="29949" class="Keyword">import</a> <a id="29956" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="29992" class="Keyword">open</a> <a id="29997" class="Keyword">import</a> <a id="30004" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="30039" class="Keyword">open</a> <a id="30044" class="Keyword">import</a> <a id="30051" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="30078" class="Keyword">open</a> <a id="30083" class="Keyword">import</a> <a id="30090" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="30120" class="Keyword">open</a> <a id="30125" class="Keyword">import</a> <a id="30132" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="30168" class="Keyword">open</a> <a id="30173" class="Keyword">import</a> <a id="30180" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="30222" class="Keyword">open</a> <a id="30227" class="Keyword">import</a> <a id="30234" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="30266" class="Keyword">open</a> <a id="30271" class="Keyword">import</a> <a id="30278" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30309" class="Keyword">open</a> <a id="30314" class="Keyword">import</a> <a id="30321" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30347" class="Keyword">open</a> <a id="30352" class="Keyword">import</a> <a id="30359" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30388" class="Keyword">open</a> <a id="30393" class="Keyword">import</a> <a id="30400" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30437" class="Keyword">open</a> <a id="30442" class="Keyword">import</a> <a id="30449" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="30489" class="Keyword">open</a> <a id="30494" class="Keyword">import</a> <a id="30501" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="30523" class="Keyword">open</a> <a id="30528" class="Keyword">import</a> <a id="30535" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="30570" class="Keyword">open</a> <a id="30575" class="Keyword">import</a> <a id="30582" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="30620" class="Keyword">open</a> <a id="30625" class="Keyword">import</a> <a id="30632" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="30671" class="Keyword">open</a> <a id="30676" class="Keyword">import</a> <a id="30683" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="30718" class="Keyword">open</a> <a id="30723" class="Keyword">import</a> <a id="30730" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="30765" class="Keyword">open</a> <a id="30770" class="Keyword">import</a> <a id="30777" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="30815" class="Keyword">open</a> <a id="30820" class="Keyword">import</a> <a id="30827" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="30858" class="Keyword">open</a> <a id="30863" class="Keyword">import</a> <a id="30870" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="30912" class="Keyword">open</a> <a id="30917" class="Keyword">import</a> <a id="30924" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="30969" class="Keyword">open</a> <a id="30974" class="Keyword">import</a> <a id="30981" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="31014" class="Keyword">open</a> <a id="31019" class="Keyword">import</a> <a id="31026" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="31046" class="Keyword">open</a> <a id="31051" class="Keyword">import</a> <a id="31058" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="31081" class="Keyword">open</a> <a id="31086" class="Keyword">import</a> <a id="31093" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="31116" class="Keyword">open</a> <a id="31121" class="Keyword">import</a> <a id="31128" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="31154" class="Keyword">open</a> <a id="31159" class="Keyword">import</a> <a id="31166" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="31192" class="Keyword">open</a> <a id="31197" class="Keyword">import</a> <a id="31204" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="31268" class="Keyword">open</a> <a id="31273" class="Keyword">import</a> <a id="31280" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31298" class="Keyword">open</a> <a id="31303" class="Keyword">import</a> <a id="31310" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31337" class="Keyword">open</a> <a id="31342" class="Keyword">import</a> <a id="31349" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31375" class="Keyword">open</a> <a id="31380" class="Keyword">import</a> <a id="31387" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31413" class="Keyword">open</a> <a id="31418" class="Keyword">import</a> <a id="31425" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31451" class="Keyword">open</a> <a id="31456" class="Keyword">import</a> <a id="31463" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="31494" class="Keyword">open</a> <a id="31499" class="Keyword">import</a> <a id="31506" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="31569" class="Keyword">open</a> <a id="31574" class="Keyword">import</a> <a id="31581" href="polytopes.html" class="Module">polytopes</a>
<a id="31591" class="Keyword">open</a> <a id="31596" class="Keyword">import</a> <a id="31603" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="31661" class="Keyword">open</a> <a id="31666" class="Keyword">import</a> <a id="31673" href="ring-theory.html" class="Module">ring-theory</a>
<a id="31685" class="Keyword">open</a> <a id="31690" class="Keyword">import</a> <a id="31697" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="31734" class="Keyword">open</a> <a id="31739" class="Keyword">import</a> <a id="31746" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="31773" class="Keyword">open</a> <a id="31778" class="Keyword">import</a> <a id="31785" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="31817" class="Keyword">open</a> <a id="31822" class="Keyword">import</a> <a id="31829" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="31875" class="Keyword">open</a> <a id="31880" class="Keyword">import</a> <a id="31887" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="31912" class="Keyword">open</a> <a id="31917" class="Keyword">import</a> <a id="31924" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="31967" class="Keyword">open</a> <a id="31972" class="Keyword">import</a> <a id="31979" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="32017" class="Keyword">open</a> <a id="32022" class="Keyword">import</a> <a id="32029" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="32060" class="Keyword">open</a> <a id="32065" class="Keyword">import</a> <a id="32072" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="32096" class="Keyword">open</a> <a id="32101" class="Keyword">import</a> <a id="32108" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="32140" class="Keyword">open</a> <a id="32145" class="Keyword">import</a> <a id="32152" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="32178" class="Keyword">open</a> <a id="32183" class="Keyword">import</a> <a id="32190" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="32219" class="Keyword">open</a> <a id="32224" class="Keyword">import</a> <a id="32231" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="32268" class="Keyword">open</a> <a id="32273" class="Keyword">import</a> <a id="32280" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32309" class="Keyword">open</a> <a id="32314" class="Keyword">import</a> <a id="32321" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32348" class="Keyword">open</a> <a id="32353" class="Keyword">import</a> <a id="32360" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32397" class="Keyword">open</a> <a id="32402" class="Keyword">import</a> <a id="32409" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32436" class="Keyword">open</a> <a id="32441" class="Keyword">import</a> <a id="32448" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="32481" class="Keyword">open</a> <a id="32486" class="Keyword">import</a> <a id="32493" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="32511" class="Keyword">open</a> <a id="32516" class="Keyword">import</a> <a id="32523" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="32577" class="Keyword">open</a> <a id="32582" class="Keyword">import</a> <a id="32589" href="set-theory.html" class="Module">set-theory</a>
<a id="32600" class="Keyword">open</a> <a id="32605" class="Keyword">import</a> <a id="32612" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="32635" class="Keyword">open</a> <a id="32640" class="Keyword">import</a> <a id="32647" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="32671" class="Keyword">open</a> <a id="32676" class="Keyword">import</a> <a id="32683" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="32709" class="Keyword">open</a> <a id="32714" class="Keyword">import</a> <a id="32721" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="32783" class="Keyword">open</a> <a id="32788" class="Keyword">import</a> <a id="32795" href="structured-types.html" class="Module">structured-types</a>
<a id="32812" class="Keyword">open</a> <a id="32817" class="Keyword">import</a> <a id="32824" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="32859" class="Keyword">open</a> <a id="32864" class="Keyword">import</a> <a id="32871" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="32915" class="Keyword">open</a> <a id="32920" class="Keyword">import</a> <a id="32927" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="32991" class="Keyword">open</a> <a id="32996" class="Keyword">import</a> <a id="33003" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="33042" class="Keyword">open</a> <a id="33047" class="Keyword">import</a> <a id="33054" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="33100" class="Keyword">open</a> <a id="33105" class="Keyword">import</a> <a id="33112" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="33136" class="Keyword">open</a> <a id="33141" class="Keyword">import</a> <a id="33148" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="33217" class="Keyword">open</a> <a id="33222" class="Keyword">import</a> <a id="33229" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="33274" class="Keyword">open</a> <a id="33279" class="Keyword">import</a> <a id="33286" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33320" class="Keyword">open</a> <a id="33325" class="Keyword">import</a> <a id="33332" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33393" class="Keyword">open</a> <a id="33398" class="Keyword">import</a> <a id="33405" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33450" class="Keyword">open</a> <a id="33455" class="Keyword">import</a> <a id="33462" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="33500" class="Keyword">open</a> <a id="33505" class="Keyword">import</a> <a id="33512" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="33555" class="Keyword">open</a> <a id="33560" class="Keyword">import</a> <a id="33567" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="33603" class="Keyword">open</a> <a id="33608" class="Keyword">import</a> <a id="33615" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="33645" class="Keyword">open</a> <a id="33650" class="Keyword">import</a> <a id="33657" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="33688" class="Keyword">open</a> <a id="33693" class="Keyword">import</a> <a id="33700" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="33759" class="Keyword">open</a> <a id="33764" class="Keyword">import</a> <a id="33771" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="33822" class="Keyword">open</a> <a id="33827" class="Keyword">import</a> <a id="33834" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="33885" class="Keyword">open</a> <a id="33890" class="Keyword">import</a> <a id="33897" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="33952" class="Keyword">open</a> <a id="33957" class="Keyword">import</a> <a id="33964" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="33993" class="Keyword">open</a> <a id="33998" class="Keyword">import</a> <a id="34005" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="34033" class="Keyword">open</a> <a id="34038" class="Keyword">import</a> <a id="34045" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="34075" class="Keyword">open</a> <a id="34080" class="Keyword">import</a> <a id="34087" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="34121" class="Keyword">open</a> <a id="34126" class="Keyword">import</a> <a id="34133" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="34209" class="Keyword">open</a> <a id="34214" class="Keyword">import</a> <a id="34221" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="34247" class="Keyword">open</a> <a id="34252" class="Keyword">import</a> <a id="34259" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="34298" class="Keyword">open</a> <a id="34303" class="Keyword">import</a> <a id="34310" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34348" class="Keyword">open</a> <a id="34353" class="Keyword">import</a> <a id="34360" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34406" class="Keyword">open</a> <a id="34411" class="Keyword">import</a> <a id="34418" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34455" class="Keyword">open</a> <a id="34460" class="Keyword">import</a> <a id="34467" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34507" class="Keyword">open</a> <a id="34512" class="Keyword">import</a> <a id="34519" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="34558" class="Keyword">open</a> <a id="34563" class="Keyword">import</a> <a id="34570" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="34603" class="Keyword">open</a> <a id="34608" class="Keyword">import</a> <a id="34615" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="34650" class="Keyword">open</a> <a id="34655" class="Keyword">import</a> <a id="34662" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="34707" class="Keyword">open</a> <a id="34712" class="Keyword">import</a> <a id="34719" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="34771" class="Keyword">open</a> <a id="34776" class="Keyword">import</a> <a id="34783" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="34836" class="Keyword">open</a> <a id="34841" class="Keyword">import</a> <a id="34848" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="34908" class="Keyword">open</a> <a id="34913" class="Keyword">import</a> <a id="34920" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="34968" class="Keyword">open</a> <a id="34973" class="Keyword">import</a> <a id="34980" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="35020" class="Keyword">open</a> <a id="35025" class="Keyword">import</a> <a id="35032" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="35079" class="Keyword">open</a> <a id="35084" class="Keyword">import</a> <a id="35091" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="35132" class="Keyword">open</a> <a id="35137" class="Keyword">import</a> <a id="35144" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="35182" class="Keyword">open</a> <a id="35187" class="Keyword">import</a> <a id="35194" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="35242" class="Keyword">open</a> <a id="35247" class="Keyword">import</a> <a id="35254" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35291" class="Keyword">open</a> <a id="35296" class="Keyword">import</a> <a id="35303" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35337" class="Keyword">open</a> <a id="35342" class="Keyword">import</a> <a id="35349" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35396" class="Keyword">open</a> <a id="35401" class="Keyword">import</a> <a id="35408" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35453" class="Keyword">open</a> <a id="35458" class="Keyword">import</a> <a id="35465" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35514" class="Keyword">open</a> <a id="35519" class="Keyword">import</a> <a id="35526" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="35603" class="Keyword">open</a> <a id="35608" class="Keyword">import</a> <a id="35615" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="35667" class="Keyword">open</a> <a id="35672" class="Keyword">import</a> <a id="35679" href="type-theories.html" class="Module">type-theories</a>
<a id="35693" class="Keyword">open</a> <a id="35698" class="Keyword">import</a> <a id="35705" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="35747" class="Keyword">open</a> <a id="35752" class="Keyword">import</a> <a id="35759" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="35797" class="Keyword">open</a> <a id="35802" class="Keyword">import</a> <a id="35809" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="35855" class="Keyword">open</a> <a id="35860" class="Keyword">import</a> <a id="35867" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="35914" class="Keyword">open</a> <a id="35919" class="Keyword">import</a> <a id="35926" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="35961" class="Keyword">open</a> <a id="35966" class="Keyword">import</a> <a id="35973" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="36051" class="Keyword">open</a> <a id="36056" class="Keyword">import</a> <a id="36063" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="36087" class="Keyword">open</a> <a id="36092" class="Keyword">import</a> <a id="36099" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="36152" class="Keyword">open</a> <a id="36157" class="Keyword">import</a> <a id="36164" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="36207" class="Keyword">open</a> <a id="36212" class="Keyword">import</a> <a id="36219" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="36259" class="Keyword">open</a> <a id="36264" class="Keyword">import</a> <a id="36271" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36310" class="Keyword">open</a> <a id="36315" class="Keyword">import</a> <a id="36322" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36356" class="Keyword">open</a> <a id="36361" class="Keyword">import</a> <a id="36368" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36416" class="Keyword">open</a> <a id="36421" class="Keyword">import</a> <a id="36428" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36479" class="Keyword">open</a> <a id="36484" class="Keyword">import</a> <a id="36491" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="36538" class="Keyword">open</a> <a id="36543" class="Keyword">import</a> <a id="36550" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="36602" class="Keyword">open</a> <a id="36607" class="Keyword">import</a> <a id="36614" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="36658" class="Keyword">open</a> <a id="36663" class="Keyword">import</a> <a id="36670" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="36710" class="Keyword">open</a> <a id="36715" class="Keyword">import</a> <a id="36722" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="36765" class="Keyword">open</a> <a id="36770" class="Keyword">import</a> <a id="36777" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="36829" class="Keyword">open</a> <a id="36834" class="Keyword">import</a> <a id="36841" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="36895" class="Keyword">open</a> <a id="36900" class="Keyword">import</a> <a id="36907" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="36955" class="Keyword">open</a> <a id="36960" class="Keyword">import</a> <a id="36967" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="37006" class="Keyword">open</a> <a id="37011" class="Keyword">import</a> <a id="37018" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="37051" class="Keyword">open</a> <a id="37056" class="Keyword">import</a> <a id="37063" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="37093" class="Keyword">open</a> <a id="37098" class="Keyword">import</a> <a id="37105" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="37156" class="Keyword">open</a> <a id="37161" class="Keyword">import</a> <a id="37168" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="37209" class="Keyword">open</a> <a id="37214" class="Keyword">import</a> <a id="37221" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="37258" class="Keyword">open</a> <a id="37263" class="Keyword">import</a> <a id="37270" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="37329" class="Keyword">open</a> <a id="37334" class="Keyword">import</a> <a id="37341" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37396" class="Keyword">open</a> <a id="37401" class="Keyword">import</a> <a id="37408" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37464" class="Keyword">open</a> <a id="37469" class="Keyword">import</a> <a id="37476" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="37523" class="Keyword">open</a> <a id="37528" class="Keyword">import</a> <a id="37535" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="37578" class="Keyword">open</a> <a id="37583" class="Keyword">import</a> <a id="37590" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="37635" class="Keyword">open</a> <a id="37640" class="Keyword">import</a> <a id="37647" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="37696" class="Keyword">open</a> <a id="37701" class="Keyword">import</a> <a id="37708" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="37759" class="Keyword">open</a> <a id="37764" class="Keyword">import</a> <a id="37771" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="37815" class="Keyword">open</a> <a id="37820" class="Keyword">import</a> <a id="37827" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="37905" class="Keyword">open</a> <a id="37910" class="Keyword">import</a> <a id="37917" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="37957" class="Keyword">open</a> <a id="37962" class="Keyword">import</a> <a id="37969" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="38026" class="Keyword">open</a> <a id="38031" class="Keyword">import</a> <a id="38038" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="38073" class="Keyword">open</a> <a id="38078" class="Keyword">import</a> <a id="38085" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="38131" class="Keyword">open</a> <a id="38136" class="Keyword">import</a> <a id="38143" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="38198" class="Keyword">open</a> <a id="38203" class="Keyword">import</a> <a id="38210" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="38253" class="Keyword">open</a> <a id="38258" class="Keyword">import</a> <a id="38265" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38310" class="Keyword">open</a> <a id="38315" class="Keyword">import</a> <a id="38322" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38381" class="Keyword">open</a> <a id="38386" class="Keyword">import</a> <a id="38393" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38430" class="Keyword">open</a> <a id="38435" class="Keyword">import</a> <a id="38442" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38484" class="Keyword">open</a> <a id="38489" class="Keyword">import</a> <a id="38496" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="38537" class="Keyword">open</a> <a id="38542" class="Keyword">import</a> <a id="38549" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="38588" class="Keyword">open</a> <a id="38593" class="Keyword">import</a> <a id="38600" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="38638" class="Keyword">open</a> <a id="38643" class="Keyword">import</a> <a id="38650" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="38702" class="Keyword">open</a> <a id="38707" class="Keyword">import</a> <a id="38714" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="38759" class="Keyword">open</a> <a id="38764" class="Keyword">import</a> <a id="38771" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="38810" class="Keyword">open</a> <a id="38815" class="Keyword">import</a> <a id="38822" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="38859" class="Keyword">open</a> <a id="38864" class="Keyword">import</a> <a id="38871" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="38920" class="Keyword">open</a> <a id="38925" class="Keyword">import</a> <a id="38932" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="38971" class="Keyword">open</a> <a id="38976" class="Keyword">import</a> <a id="38983" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="39021" class="Keyword">open</a> <a id="39026" class="Keyword">import</a> <a id="39033" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="39088" class="Keyword">open</a> <a id="39093" class="Keyword">import</a> <a id="39100" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="39139" class="Keyword">open</a> <a id="39144" class="Keyword">import</a> <a id="39151" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="39199" class="Keyword">open</a> <a id="39204" class="Keyword">import</a> <a id="39211" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="39258" class="Keyword">open</a> <a id="39263" class="Keyword">import</a> <a id="39270" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39308" class="Keyword">open</a> <a id="39313" class="Keyword">import</a> <a id="39320" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="39350" class="Keyword">open</a> <a id="39355" class="Keyword">import</a> <a id="39362" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39419" class="Keyword">open</a> <a id="39424" class="Keyword">import</a> <a id="39431" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39485" class="Keyword">open</a> <a id="39490" class="Keyword">import</a> <a id="39497" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="39527" class="Keyword">open</a> <a id="39532" class="Keyword">import</a> <a id="39539" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="39588" class="Keyword">open</a> <a id="39593" class="Keyword">import</a> <a id="39600" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="39642" class="Keyword">open</a> <a id="39647" class="Keyword">import</a> <a id="39654" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="39688" class="Keyword">open</a> <a id="39693" class="Keyword">import</a> <a id="39700" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="39763" class="Keyword">open</a> <a id="39768" class="Keyword">import</a> <a id="39775" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="39818" class="Keyword">open</a> <a id="39823" class="Keyword">import</a> <a id="39830" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="39865" class="Keyword">open</a> <a id="39870" class="Keyword">import</a> <a id="39877" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="39912" class="Keyword">open</a> <a id="39917" class="Keyword">import</a> <a id="39924" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="39964" class="Keyword">open</a> <a id="39969" class="Keyword">import</a> <a id="39976" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="40021" class="Keyword">open</a> <a id="40026" class="Keyword">import</a> <a id="40033" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="40074" class="Keyword">open</a> <a id="40079" class="Keyword">import</a> <a id="40086" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="40140" class="Keyword">open</a> <a id="40145" class="Keyword">import</a> <a id="40152" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="40202" class="Keyword">open</a> <a id="40207" class="Keyword">import</a> <a id="40214" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="40261" class="Keyword">open</a> <a id="40266" class="Keyword">import</a> <a id="40273" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40311" class="Keyword">open</a> <a id="40316" class="Keyword">import</a> <a id="40323" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40372" class="Keyword">open</a> <a id="40377" class="Keyword">import</a> <a id="40384" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40431" class="Keyword">open</a> <a id="40436" class="Keyword">import</a> <a id="40443" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40506" class="Keyword">open</a> <a id="40511" class="Keyword">import</a> <a id="40518" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="40550" class="Keyword">open</a> <a id="40555" class="Keyword">import</a> <a id="40562" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="40615" class="Keyword">open</a> <a id="40620" class="Keyword">import</a> <a id="40627" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="40673" class="Keyword">open</a> <a id="40678" class="Keyword">import</a> <a id="40685" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="40731" class="Keyword">open</a> <a id="40736" class="Keyword">import</a> <a id="40743" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="40783" class="Keyword">open</a> <a id="40788" class="Keyword">import</a> <a id="40795" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="40842" class="Keyword">open</a> <a id="40847" class="Keyword">import</a> <a id="40854" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="40902" class="Keyword">open</a> <a id="40907" class="Keyword">import</a> <a id="40914" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="40954" class="Keyword">open</a> <a id="40959" class="Keyword">import</a> <a id="40966" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="41011" class="Keyword">open</a> <a id="41016" class="Keyword">import</a> <a id="41023" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="41088" class="Keyword">open</a> <a id="41093" class="Keyword">import</a> <a id="41100" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="41145" class="Keyword">open</a> <a id="41150" class="Keyword">import</a> <a id="41157" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="41204" class="Keyword">open</a> <a id="41209" class="Keyword">import</a> <a id="41216" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="41269" class="Keyword">open</a> <a id="41274" class="Keyword">import</a> <a id="41281" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>