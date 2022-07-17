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
<a id="18578" class="Keyword">open</a> <a id="18583" class="Keyword">import</a> <a id="18590" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18638" class="Keyword">open</a> <a id="18643" class="Keyword">import</a> <a id="18650" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18688" class="Keyword">open</a> <a id="18693" class="Keyword">import</a> <a id="18700" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18737" class="Keyword">open</a> <a id="18742" class="Keyword">import</a> <a id="18749" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18795" class="Keyword">open</a> <a id="18800" class="Keyword">import</a> <a id="18807" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18824" class="Keyword">open</a> <a id="18829" class="Keyword">import</a> <a id="18836" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18864" class="Keyword">open</a> <a id="18869" class="Keyword">import</a> <a id="18876" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18904" class="Keyword">open</a> <a id="18909" class="Keyword">import</a> <a id="18916" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18952" class="Keyword">open</a> <a id="18957" class="Keyword">import</a> <a id="18964" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="19002" class="Keyword">open</a> <a id="19007" class="Keyword">import</a> <a id="19014" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="19047" class="Keyword">open</a> <a id="19052" class="Keyword">import</a> <a id="19059" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="19080" class="Keyword">open</a> <a id="19085" class="Keyword">import</a> <a id="19092" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="19128" class="Keyword">open</a> <a id="19133" class="Keyword">import</a> <a id="19140" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="19194" class="Keyword">open</a> <a id="19199" class="Keyword">import</a> <a id="19206" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="19228" class="Keyword">open</a> <a id="19233" class="Keyword">import</a> <a id="19240" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="19275" class="Keyword">open</a> <a id="19280" class="Keyword">import</a> <a id="19287" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="19317" class="Keyword">open</a> <a id="19322" class="Keyword">import</a> <a id="19329" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="19368" class="Keyword">open</a> <a id="19373" class="Keyword">import</a> <a id="19380" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19434" class="Keyword">open</a> <a id="19439" class="Keyword">import</a> <a id="19446" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19492" class="Keyword">open</a> <a id="19497" class="Keyword">import</a> <a id="19504" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19555" class="Keyword">open</a> <a id="19560" class="Keyword">import</a> <a id="19567" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19608" class="Keyword">open</a> <a id="19613" class="Keyword">import</a> <a id="19620" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19665" class="Keyword">open</a> <a id="19670" class="Keyword">import</a> <a id="19677" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19722" class="Keyword">open</a> <a id="19727" class="Keyword">import</a> <a id="19734" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19770" class="Keyword">open</a> <a id="19775" class="Keyword">import</a> <a id="19782" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19818" class="Keyword">open</a> <a id="19823" class="Keyword">import</a> <a id="19830" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19895" class="Keyword">open</a> <a id="19900" class="Keyword">import</a> <a id="19907" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19962" class="Keyword">open</a> <a id="19967" class="Keyword">import</a> <a id="19974" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="20014" class="Keyword">open</a> <a id="20019" class="Keyword">import</a> <a id="20026" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="20070" class="Keyword">open</a> <a id="20075" class="Keyword">import</a> <a id="20082" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="20127" class="Keyword">open</a> <a id="20132" class="Keyword">import</a> <a id="20139" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="20180" class="Keyword">open</a> <a id="20185" class="Keyword">import</a> <a id="20192" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="20232" class="Keyword">open</a> <a id="20237" class="Keyword">import</a> <a id="20244" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="20271" class="Keyword">open</a> <a id="20276" class="Keyword">import</a> <a id="20283" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="20319" class="Keyword">open</a> <a id="20324" class="Keyword">import</a> <a id="20331" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="20358" class="Keyword">open</a> <a id="20363" class="Keyword">import</a> <a id="20370" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20407" class="Keyword">open</a> <a id="20412" class="Keyword">import</a> <a id="20419" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20447" class="Keyword">open</a> <a id="20452" class="Keyword">import</a> <a id="20459" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20478" class="Keyword">open</a> <a id="20483" class="Keyword">import</a> <a id="20490" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20530" class="Keyword">open</a> <a id="20535" class="Keyword">import</a> <a id="20542" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20574" class="Keyword">open</a> <a id="20579" class="Keyword">import</a> <a id="20586" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20634" class="Keyword">open</a> <a id="20639" class="Keyword">import</a> <a id="20646" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20669" class="Keyword">open</a> <a id="20674" class="Keyword">import</a> <a id="20681" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20705" class="Keyword">open</a> <a id="20710" class="Keyword">import</a> <a id="20717" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20757" class="Keyword">open</a> <a id="20762" class="Keyword">import</a> <a id="20769" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20812" class="Keyword">open</a> <a id="20817" class="Keyword">import</a> <a id="20824" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20858" class="Keyword">open</a> <a id="20863" class="Keyword">import</a> <a id="20870" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20902" class="Keyword">open</a> <a id="20907" class="Keyword">import</a> <a id="20914" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20944" class="Keyword">open</a> <a id="20949" class="Keyword">import</a> <a id="20956" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20990" class="Keyword">open</a> <a id="20995" class="Keyword">import</a> <a id="21002" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="21037" class="Keyword">open</a> <a id="21042" class="Keyword">import</a> <a id="21049" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="21086" class="Keyword">open</a> <a id="21091" class="Keyword">import</a> <a id="21098" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="21125" class="Keyword">open</a> <a id="21130" class="Keyword">import</a> <a id="21137" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="21165" class="Keyword">open</a> <a id="21170" class="Keyword">import</a> <a id="21177" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="21226" class="Keyword">open</a> <a id="21231" class="Keyword">import</a> <a id="21238" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="21284" class="Keyword">open</a> <a id="21289" class="Keyword">import</a> <a id="21296" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="21336" class="Keyword">open</a> <a id="21341" class="Keyword">import</a> <a id="21348" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="21386" class="Keyword">open</a> <a id="21391" class="Keyword">import</a> <a id="21398" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21427" class="Keyword">open</a> <a id="21432" class="Keyword">import</a> <a id="21439" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21469" class="Keyword">open</a> <a id="21474" class="Keyword">import</a> <a id="21481" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21512" class="Keyword">open</a> <a id="21517" class="Keyword">import</a> <a id="21524" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21564" class="Keyword">open</a> <a id="21569" class="Keyword">import</a> <a id="21576" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21602" class="Keyword">open</a> <a id="21607" class="Keyword">import</a> <a id="21614" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21669" class="Keyword">open</a> <a id="21674" class="Keyword">import</a> <a id="21681" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21732" class="Keyword">open</a> <a id="21737" class="Keyword">import</a> <a id="21744" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21789" class="Keyword">open</a> <a id="21794" class="Keyword">import</a> <a id="21801" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21855" class="Keyword">open</a> <a id="21860" class="Keyword">import</a> <a id="21867" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21894" class="Keyword">open</a> <a id="21899" class="Keyword">import</a> <a id="21906" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21939" class="Keyword">open</a> <a id="21944" class="Keyword">import</a> <a id="21951" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21982" class="Keyword">open</a> <a id="21987" class="Keyword">import</a> <a id="21994" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="22031" class="Keyword">open</a> <a id="22036" class="Keyword">import</a> <a id="22043" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="22068" class="Keyword">open</a> <a id="22073" class="Keyword">import</a> <a id="22080" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="22112" class="Keyword">open</a> <a id="22117" class="Keyword">import</a> <a id="22124" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="22159" class="Keyword">open</a> <a id="22164" class="Keyword">import</a> <a id="22171" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="22200" class="Keyword">open</a> <a id="22205" class="Keyword">import</a> <a id="22212" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="22238" class="Keyword">open</a> <a id="22243" class="Keyword">import</a> <a id="22250" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="22278" class="Keyword">open</a> <a id="22283" class="Keyword">import</a> <a id="22290" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="22315" class="Keyword">open</a> <a id="22320" class="Keyword">import</a> <a id="22327" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="22348" class="Keyword">open</a> <a id="22353" class="Keyword">import</a> <a id="22360" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="22396" class="Keyword">open</a> <a id="22401" class="Keyword">import</a> <a id="22408" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22451" class="Keyword">open</a> <a id="22456" class="Keyword">import</a> <a id="22463" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22488" class="Keyword">open</a> <a id="22493" class="Keyword">import</a> <a id="22500" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22531" class="Keyword">open</a> <a id="22536" class="Keyword">import</a> <a id="22543" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22575" class="Keyword">open</a> <a id="22580" class="Keyword">import</a> <a id="22587" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22621" class="Keyword">open</a> <a id="22626" class="Keyword">import</a> <a id="22633" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22689" class="Keyword">open</a> <a id="22694" class="Keyword">import</a> <a id="22701" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22754" class="Keyword">open</a> <a id="22759" class="Keyword">import</a> <a id="22766" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22793" class="Keyword">open</a> <a id="22798" class="Keyword">import</a> <a id="22805" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22850" class="Keyword">open</a> <a id="22855" class="Keyword">import</a> <a id="22862" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22924" class="Keyword">open</a> <a id="22929" class="Keyword">import</a> <a id="22936" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22949" class="Keyword">open</a> <a id="22954" class="Keyword">import</a> <a id="22961" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="23001" class="Keyword">open</a> <a id="23006" class="Keyword">import</a> <a id="23013" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="23057" class="Keyword">open</a> <a id="23062" class="Keyword">import</a> <a id="23069" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="23108" class="Keyword">open</a> <a id="23113" class="Keyword">import</a> <a id="23120" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="23162" class="Keyword">open</a> <a id="23167" class="Keyword">import</a> <a id="23174" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="23214" class="Keyword">open</a> <a id="23219" class="Keyword">import</a> <a id="23226" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="23267" class="Keyword">open</a> <a id="23272" class="Keyword">import</a> <a id="23279" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="23317" class="Keyword">open</a> <a id="23322" class="Keyword">import</a> <a id="23329" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="23392" class="Keyword">open</a> <a id="23397" class="Keyword">import</a> <a id="23404" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="23433" class="Keyword">open</a> <a id="23438" class="Keyword">import</a> <a id="23445" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="23490" class="Keyword">open</a> <a id="23495" class="Keyword">import</a> <a id="23502" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="23544" class="Keyword">open</a> <a id="23549" class="Keyword">import</a> <a id="23556" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="23600" class="Keyword">open</a> <a id="23605" class="Keyword">import</a> <a id="23612" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23661" class="Keyword">open</a> <a id="23666" class="Keyword">import</a> <a id="23673" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23723" class="Keyword">open</a> <a id="23728" class="Keyword">import</a> <a id="23735" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23762" class="Keyword">open</a> <a id="23767" class="Keyword">import</a> <a id="23774" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="23799" class="Keyword">open</a> <a id="23804" class="Keyword">import</a> <a id="23811" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23852" class="Keyword">open</a> <a id="23857" class="Keyword">import</a> <a id="23864" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23887" class="Keyword">open</a> <a id="23892" class="Keyword">import</a> <a id="23899" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23948" class="Keyword">open</a> <a id="23953" class="Keyword">import</a> <a id="23960" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23999" class="Keyword">open</a> <a id="24004" class="Keyword">import</a> <a id="24011" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="24052" class="Keyword">open</a> <a id="24057" class="Keyword">import</a> <a id="24064" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="24108" class="Keyword">open</a> <a id="24113" class="Keyword">import</a> <a id="24120" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="24157" class="Keyword">open</a> <a id="24162" class="Keyword">import</a> <a id="24169" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="24191" class="Keyword">open</a> <a id="24196" class="Keyword">import</a> <a id="24203" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="24233" class="Keyword">open</a> <a id="24238" class="Keyword">import</a> <a id="24245" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="24284" class="Keyword">open</a> <a id="24289" class="Keyword">import</a> <a id="24296" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="24334" class="Keyword">open</a> <a id="24339" class="Keyword">import</a> <a id="24346" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="24404" class="Keyword">open</a> <a id="24409" class="Keyword">import</a> <a id="24416" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="24481" class="Keyword">open</a> <a id="24486" class="Keyword">import</a> <a id="24493" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="24524" class="Keyword">open</a> <a id="24529" class="Keyword">import</a> <a id="24536" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="24563" class="Keyword">open</a> <a id="24568" class="Keyword">import</a> <a id="24575" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="24633" class="Keyword">open</a> <a id="24638" class="Keyword">import</a> <a id="24645" href="group-theory.html" class="Module">group-theory</a>
<a id="24658" class="Keyword">open</a> <a id="24663" class="Keyword">import</a> <a id="24670" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="24698" class="Keyword">open</a> <a id="24703" class="Keyword">import</a> <a id="24710" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24761" class="Keyword">open</a> <a id="24766" class="Keyword">import</a> <a id="24773" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24806" class="Keyword">open</a> <a id="24811" class="Keyword">import</a> <a id="24818" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24865" class="Keyword">open</a> <a id="24870" class="Keyword">import</a> <a id="24877" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24916" class="Keyword">open</a> <a id="24921" class="Keyword">import</a> <a id="24928" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24968" class="Keyword">open</a> <a id="24973" class="Keyword">import</a> <a id="24980" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="25023" class="Keyword">open</a> <a id="25028" class="Keyword">import</a> <a id="25035" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="25067" class="Keyword">open</a> <a id="25072" class="Keyword">import</a> <a id="25079" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="25115" class="Keyword">open</a> <a id="25120" class="Keyword">import</a> <a id="25127" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="25156" class="Keyword">open</a> <a id="25161" class="Keyword">import</a> <a id="25168" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="25196" class="Keyword">open</a> <a id="25201" class="Keyword">import</a> <a id="25208" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="25241" class="Keyword">open</a> <a id="25246" class="Keyword">import</a> <a id="25253" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="25289" class="Keyword">open</a> <a id="25294" class="Keyword">import</a> <a id="25301" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="25330" class="Keyword">open</a> <a id="25335" class="Keyword">import</a> <a id="25342" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="25367" class="Keyword">open</a> <a id="25372" class="Keyword">import</a> <a id="25379" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="25441" class="Keyword">open</a> <a id="25446" class="Keyword">import</a> <a id="25453" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="25484" class="Keyword">open</a> <a id="25489" class="Keyword">import</a> <a id="25496" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="25543" class="Keyword">open</a> <a id="25548" class="Keyword">import</a> <a id="25555" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="25588" class="Keyword">open</a> <a id="25593" class="Keyword">import</a> <a id="25600" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="25649" class="Keyword">open</a> <a id="25654" class="Keyword">import</a> <a id="25661" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="25701" class="Keyword">open</a> <a id="25706" class="Keyword">import</a> <a id="25713" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="25750" class="Keyword">open</a> <a id="25755" class="Keyword">import</a> <a id="25762" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="25809" class="Keyword">open</a> <a id="25814" class="Keyword">import</a> <a id="25821" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="25862" class="Keyword">open</a> <a id="25867" class="Keyword">import</a> <a id="25874" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="25913" class="Keyword">open</a> <a id="25918" class="Keyword">import</a> <a id="25925" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25957" class="Keyword">open</a> <a id="25962" class="Keyword">import</a> <a id="25969" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25996" class="Keyword">open</a> <a id="26001" class="Keyword">import</a> <a id="26008" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="26028" class="Keyword">open</a> <a id="26033" class="Keyword">import</a> <a id="26040" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="26074" class="Keyword">open</a> <a id="26079" class="Keyword">import</a> <a id="26086" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="26113" class="Keyword">open</a> <a id="26118" class="Keyword">import</a> <a id="26125" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="26167" class="Keyword">open</a> <a id="26172" class="Keyword">import</a> <a id="26179" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="26229" class="Keyword">open</a> <a id="26234" class="Keyword">import</a> <a id="26241" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="26288" class="Keyword">open</a> <a id="26293" class="Keyword">import</a> <a id="26300" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="26341" class="Keyword">open</a> <a id="26346" class="Keyword">import</a> <a id="26353" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="26387" class="Keyword">open</a> <a id="26392" class="Keyword">import</a> <a id="26399" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="26440" class="Keyword">open</a> <a id="26445" class="Keyword">import</a> <a id="26452" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="26487" class="Keyword">open</a> <a id="26492" class="Keyword">import</a> <a id="26499" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="26537" class="Keyword">open</a> <a id="26542" class="Keyword">import</a> <a id="26549" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="26584" class="Keyword">open</a> <a id="26589" class="Keyword">import</a> <a id="26596" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="26628" class="Keyword">open</a> <a id="26633" class="Keyword">import</a> <a id="26640" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="26681" class="Keyword">open</a> <a id="26686" class="Keyword">import</a> <a id="26693" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="26734" class="Keyword">open</a> <a id="26739" class="Keyword">import</a> <a id="26746" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="26786" class="Keyword">open</a> <a id="26791" class="Keyword">import</a> <a id="26798" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="26831" class="Keyword">open</a> <a id="26836" class="Keyword">import</a> <a id="26843" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="26880" class="Keyword">open</a> <a id="26885" class="Keyword">import</a> <a id="26892" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="26922" class="Keyword">open</a> <a id="26927" class="Keyword">import</a> <a id="26934" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="26955" class="Keyword">open</a> <a id="26960" class="Keyword">import</a> <a id="26967" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="27012" class="Keyword">open</a> <a id="27017" class="Keyword">import</a> <a id="27024" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="27052" class="Keyword">open</a> <a id="27057" class="Keyword">import</a> <a id="27064" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="27085" class="Keyword">open</a> <a id="27090" class="Keyword">import</a> <a id="27097" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="27140" class="Keyword">open</a> <a id="27145" class="Keyword">import</a> <a id="27152" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="27186" class="Keyword">open</a> <a id="27191" class="Keyword">import</a> <a id="27198" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="27228" class="Keyword">open</a> <a id="27233" class="Keyword">import</a> <a id="27240" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="27286" class="Keyword">open</a> <a id="27291" class="Keyword">import</a> <a id="27298" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="27352" class="Keyword">open</a> <a id="27357" class="Keyword">import</a> <a id="27364" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="27407" class="Keyword">open</a> <a id="27412" class="Keyword">import</a> <a id="27419" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="27453" class="Keyword">open</a> <a id="27458" class="Keyword">import</a> <a id="27465" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="27506" class="Keyword">open</a> <a id="27511" class="Keyword">import</a> <a id="27518" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="27553" class="Keyword">open</a> <a id="27558" class="Keyword">import</a> <a id="27565" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="27607" class="Keyword">open</a> <a id="27612" class="Keyword">import</a> <a id="27619" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="27654" class="Keyword">open</a> <a id="27659" class="Keyword">import</a> <a id="27666" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="27705" class="Keyword">open</a> <a id="27710" class="Keyword">import</a> <a id="27717" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="27754" class="Keyword">open</a> <a id="27759" class="Keyword">import</a> <a id="27766" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="27813" class="Keyword">open</a> <a id="27818" class="Keyword">import</a> <a id="27825" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="27889" class="Keyword">open</a> <a id="27894" class="Keyword">import</a> <a id="27901" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="27925" class="Keyword">open</a> <a id="27930" class="Keyword">import</a> <a id="27937" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="27962" class="Keyword">open</a> <a id="27967" class="Keyword">import</a> <a id="27974" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="28017" class="Keyword">open</a> <a id="28022" class="Keyword">import</a> <a id="28029" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="28060" class="Keyword">open</a> <a id="28065" class="Keyword">import</a> <a id="28072" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="28126" class="Keyword">open</a> <a id="28131" class="Keyword">import</a> <a id="28138" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="28161" class="Keyword">open</a> <a id="28166" class="Keyword">import</a> <a id="28173" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="28211" class="Keyword">open</a> <a id="28216" class="Keyword">import</a> <a id="28223" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="28262" class="Keyword">open</a> <a id="28267" class="Keyword">import</a> <a id="28274" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="28325" class="Keyword">open</a> <a id="28330" class="Keyword">import</a> <a id="28337" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="28374" class="Keyword">open</a> <a id="28379" class="Keyword">import</a> <a id="28386" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="28443" class="Keyword">open</a> <a id="28448" class="Keyword">import</a> <a id="28455" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="28503" class="Keyword">open</a> <a id="28508" class="Keyword">import</a> <a id="28515" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="28545" class="Keyword">open</a> <a id="28550" class="Keyword">import</a> <a id="28557" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="28594" class="Keyword">open</a> <a id="28599" class="Keyword">import</a> <a id="28606" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="28627" class="Keyword">open</a> <a id="28632" class="Keyword">import</a> <a id="28639" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="28686" class="Keyword">open</a> <a id="28691" class="Keyword">import</a> <a id="28698" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="28736" class="Keyword">open</a> <a id="28741" class="Keyword">import</a> <a id="28748" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="28842" class="Keyword">open</a> <a id="28847" class="Keyword">import</a> <a id="28854" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="28869" class="Keyword">open</a> <a id="28874" class="Keyword">import</a> <a id="28881" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="28914" class="Keyword">open</a> <a id="28919" class="Keyword">import</a> <a id="28926" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="28958" class="Keyword">open</a> <a id="28963" class="Keyword">import</a> <a id="28970" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="29012" class="Keyword">open</a> <a id="29017" class="Keyword">import</a> <a id="29024" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="29062" class="Keyword">open</a> <a id="29067" class="Keyword">import</a> <a id="29074" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="29111" class="Keyword">open</a> <a id="29116" class="Keyword">import</a> <a id="29123" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="29156" class="Keyword">open</a> <a id="29161" class="Keyword">import</a> <a id="29168" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="29192" class="Keyword">open</a> <a id="29197" class="Keyword">import</a> <a id="29204" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="29243" class="Keyword">open</a> <a id="29248" class="Keyword">import</a> <a id="29255" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="29301" class="Keyword">open</a> <a id="29306" class="Keyword">import</a> <a id="29313" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="29358" class="Keyword">open</a> <a id="29363" class="Keyword">import</a> <a id="29370" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="29408" class="Keyword">open</a> <a id="29413" class="Keyword">import</a> <a id="29420" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="29452" class="Keyword">open</a> <a id="29457" class="Keyword">import</a> <a id="29464" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="29517" class="Keyword">open</a> <a id="29522" class="Keyword">import</a> <a id="29529" href="order-theory.html" class="Module">order-theory</a>
<a id="29542" class="Keyword">open</a> <a id="29547" class="Keyword">import</a> <a id="29554" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="29581" class="Keyword">open</a> <a id="29586" class="Keyword">import</a> <a id="29593" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="29623" class="Keyword">open</a> <a id="29628" class="Keyword">import</a> <a id="29635" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="29668" class="Keyword">open</a> <a id="29673" class="Keyword">import</a> <a id="29680" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="29716" class="Keyword">open</a> <a id="29721" class="Keyword">import</a> <a id="29728" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="29763" class="Keyword">open</a> <a id="29768" class="Keyword">import</a> <a id="29775" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="29802" class="Keyword">open</a> <a id="29807" class="Keyword">import</a> <a id="29814" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="29844" class="Keyword">open</a> <a id="29849" class="Keyword">import</a> <a id="29856" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="29892" class="Keyword">open</a> <a id="29897" class="Keyword">import</a> <a id="29904" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="29946" class="Keyword">open</a> <a id="29951" class="Keyword">import</a> <a id="29958" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="29990" class="Keyword">open</a> <a id="29995" class="Keyword">import</a> <a id="30002" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="30033" class="Keyword">open</a> <a id="30038" class="Keyword">import</a> <a id="30045" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="30071" class="Keyword">open</a> <a id="30076" class="Keyword">import</a> <a id="30083" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="30112" class="Keyword">open</a> <a id="30117" class="Keyword">import</a> <a id="30124" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="30161" class="Keyword">open</a> <a id="30166" class="Keyword">import</a> <a id="30173" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="30213" class="Keyword">open</a> <a id="30218" class="Keyword">import</a> <a id="30225" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="30247" class="Keyword">open</a> <a id="30252" class="Keyword">import</a> <a id="30259" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="30294" class="Keyword">open</a> <a id="30299" class="Keyword">import</a> <a id="30306" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="30344" class="Keyword">open</a> <a id="30349" class="Keyword">import</a> <a id="30356" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="30395" class="Keyword">open</a> <a id="30400" class="Keyword">import</a> <a id="30407" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="30442" class="Keyword">open</a> <a id="30447" class="Keyword">import</a> <a id="30454" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="30489" class="Keyword">open</a> <a id="30494" class="Keyword">import</a> <a id="30501" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="30539" class="Keyword">open</a> <a id="30544" class="Keyword">import</a> <a id="30551" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="30582" class="Keyword">open</a> <a id="30587" class="Keyword">import</a> <a id="30594" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="30636" class="Keyword">open</a> <a id="30641" class="Keyword">import</a> <a id="30648" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="30693" class="Keyword">open</a> <a id="30698" class="Keyword">import</a> <a id="30705" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="30738" class="Keyword">open</a> <a id="30743" class="Keyword">import</a> <a id="30750" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="30770" class="Keyword">open</a> <a id="30775" class="Keyword">import</a> <a id="30782" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="30805" class="Keyword">open</a> <a id="30810" class="Keyword">import</a> <a id="30817" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="30840" class="Keyword">open</a> <a id="30845" class="Keyword">import</a> <a id="30852" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="30878" class="Keyword">open</a> <a id="30883" class="Keyword">import</a> <a id="30890" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="30916" class="Keyword">open</a> <a id="30921" class="Keyword">import</a> <a id="30928" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="30992" class="Keyword">open</a> <a id="30997" class="Keyword">import</a> <a id="31004" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="31022" class="Keyword">open</a> <a id="31027" class="Keyword">import</a> <a id="31034" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="31061" class="Keyword">open</a> <a id="31066" class="Keyword">import</a> <a id="31073" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="31099" class="Keyword">open</a> <a id="31104" class="Keyword">import</a> <a id="31111" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="31137" class="Keyword">open</a> <a id="31142" class="Keyword">import</a> <a id="31149" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="31175" class="Keyword">open</a> <a id="31180" class="Keyword">import</a> <a id="31187" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="31218" class="Keyword">open</a> <a id="31223" class="Keyword">import</a> <a id="31230" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="31293" class="Keyword">open</a> <a id="31298" class="Keyword">import</a> <a id="31305" href="polytopes.html" class="Module">polytopes</a>
<a id="31315" class="Keyword">open</a> <a id="31320" class="Keyword">import</a> <a id="31327" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="31385" class="Keyword">open</a> <a id="31390" class="Keyword">import</a> <a id="31397" href="ring-theory.html" class="Module">ring-theory</a>
<a id="31409" class="Keyword">open</a> <a id="31414" class="Keyword">import</a> <a id="31421" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="31458" class="Keyword">open</a> <a id="31463" class="Keyword">import</a> <a id="31470" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="31497" class="Keyword">open</a> <a id="31502" class="Keyword">import</a> <a id="31509" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="31541" class="Keyword">open</a> <a id="31546" class="Keyword">import</a> <a id="31553" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="31599" class="Keyword">open</a> <a id="31604" class="Keyword">import</a> <a id="31611" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="31636" class="Keyword">open</a> <a id="31641" class="Keyword">import</a> <a id="31648" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="31691" class="Keyword">open</a> <a id="31696" class="Keyword">import</a> <a id="31703" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="31741" class="Keyword">open</a> <a id="31746" class="Keyword">import</a> <a id="31753" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="31784" class="Keyword">open</a> <a id="31789" class="Keyword">import</a> <a id="31796" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="31820" class="Keyword">open</a> <a id="31825" class="Keyword">import</a> <a id="31832" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="31864" class="Keyword">open</a> <a id="31869" class="Keyword">import</a> <a id="31876" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="31902" class="Keyword">open</a> <a id="31907" class="Keyword">import</a> <a id="31914" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="31943" class="Keyword">open</a> <a id="31948" class="Keyword">import</a> <a id="31955" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="31992" class="Keyword">open</a> <a id="31997" class="Keyword">import</a> <a id="32004" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="32033" class="Keyword">open</a> <a id="32038" class="Keyword">import</a> <a id="32045" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="32072" class="Keyword">open</a> <a id="32077" class="Keyword">import</a> <a id="32084" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="32121" class="Keyword">open</a> <a id="32126" class="Keyword">import</a> <a id="32133" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="32160" class="Keyword">open</a> <a id="32165" class="Keyword">import</a> <a id="32172" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="32205" class="Keyword">open</a> <a id="32210" class="Keyword">import</a> <a id="32217" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="32235" class="Keyword">open</a> <a id="32240" class="Keyword">import</a> <a id="32247" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="32301" class="Keyword">open</a> <a id="32306" class="Keyword">import</a> <a id="32313" href="set-theory.html" class="Module">set-theory</a>
<a id="32324" class="Keyword">open</a> <a id="32329" class="Keyword">import</a> <a id="32336" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="32359" class="Keyword">open</a> <a id="32364" class="Keyword">import</a> <a id="32371" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="32395" class="Keyword">open</a> <a id="32400" class="Keyword">import</a> <a id="32407" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="32433" class="Keyword">open</a> <a id="32438" class="Keyword">import</a> <a id="32445" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="32507" class="Keyword">open</a> <a id="32512" class="Keyword">import</a> <a id="32519" href="structured-types.html" class="Module">structured-types</a>
<a id="32536" class="Keyword">open</a> <a id="32541" class="Keyword">import</a> <a id="32548" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="32583" class="Keyword">open</a> <a id="32588" class="Keyword">import</a> <a id="32595" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="32639" class="Keyword">open</a> <a id="32644" class="Keyword">import</a> <a id="32651" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="32715" class="Keyword">open</a> <a id="32720" class="Keyword">import</a> <a id="32727" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="32766" class="Keyword">open</a> <a id="32771" class="Keyword">import</a> <a id="32778" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="32824" class="Keyword">open</a> <a id="32829" class="Keyword">import</a> <a id="32836" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="32860" class="Keyword">open</a> <a id="32865" class="Keyword">import</a> <a id="32872" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="32941" class="Keyword">open</a> <a id="32946" class="Keyword">import</a> <a id="32953" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="32998" class="Keyword">open</a> <a id="33003" class="Keyword">import</a> <a id="33010" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="33044" class="Keyword">open</a> <a id="33049" class="Keyword">import</a> <a id="33056" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="33117" class="Keyword">open</a> <a id="33122" class="Keyword">import</a> <a id="33129" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="33174" class="Keyword">open</a> <a id="33179" class="Keyword">import</a> <a id="33186" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="33224" class="Keyword">open</a> <a id="33229" class="Keyword">import</a> <a id="33236" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="33279" class="Keyword">open</a> <a id="33284" class="Keyword">import</a> <a id="33291" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="33327" class="Keyword">open</a> <a id="33332" class="Keyword">import</a> <a id="33339" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="33369" class="Keyword">open</a> <a id="33374" class="Keyword">import</a> <a id="33381" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="33412" class="Keyword">open</a> <a id="33417" class="Keyword">import</a> <a id="33424" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="33483" class="Keyword">open</a> <a id="33488" class="Keyword">import</a> <a id="33495" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="33546" class="Keyword">open</a> <a id="33551" class="Keyword">import</a> <a id="33558" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="33609" class="Keyword">open</a> <a id="33614" class="Keyword">import</a> <a id="33621" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="33676" class="Keyword">open</a> <a id="33681" class="Keyword">import</a> <a id="33688" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="33717" class="Keyword">open</a> <a id="33722" class="Keyword">import</a> <a id="33729" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="33757" class="Keyword">open</a> <a id="33762" class="Keyword">import</a> <a id="33769" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="33799" class="Keyword">open</a> <a id="33804" class="Keyword">import</a> <a id="33811" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="33845" class="Keyword">open</a> <a id="33850" class="Keyword">import</a> <a id="33857" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="33933" class="Keyword">open</a> <a id="33938" class="Keyword">import</a> <a id="33945" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="33971" class="Keyword">open</a> <a id="33976" class="Keyword">import</a> <a id="33983" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="34022" class="Keyword">open</a> <a id="34027" class="Keyword">import</a> <a id="34034" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="34072" class="Keyword">open</a> <a id="34077" class="Keyword">import</a> <a id="34084" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="34130" class="Keyword">open</a> <a id="34135" class="Keyword">import</a> <a id="34142" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="34179" class="Keyword">open</a> <a id="34184" class="Keyword">import</a> <a id="34191" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="34231" class="Keyword">open</a> <a id="34236" class="Keyword">import</a> <a id="34243" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="34282" class="Keyword">open</a> <a id="34287" class="Keyword">import</a> <a id="34294" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="34327" class="Keyword">open</a> <a id="34332" class="Keyword">import</a> <a id="34339" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="34374" class="Keyword">open</a> <a id="34379" class="Keyword">import</a> <a id="34386" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="34431" class="Keyword">open</a> <a id="34436" class="Keyword">import</a> <a id="34443" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="34495" class="Keyword">open</a> <a id="34500" class="Keyword">import</a> <a id="34507" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="34560" class="Keyword">open</a> <a id="34565" class="Keyword">import</a> <a id="34572" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="34632" class="Keyword">open</a> <a id="34637" class="Keyword">import</a> <a id="34644" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="34692" class="Keyword">open</a> <a id="34697" class="Keyword">import</a> <a id="34704" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="34744" class="Keyword">open</a> <a id="34749" class="Keyword">import</a> <a id="34756" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="34803" class="Keyword">open</a> <a id="34808" class="Keyword">import</a> <a id="34815" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="34856" class="Keyword">open</a> <a id="34861" class="Keyword">import</a> <a id="34868" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="34906" class="Keyword">open</a> <a id="34911" class="Keyword">import</a> <a id="34918" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="34966" class="Keyword">open</a> <a id="34971" class="Keyword">import</a> <a id="34978" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="35015" class="Keyword">open</a> <a id="35020" class="Keyword">import</a> <a id="35027" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="35061" class="Keyword">open</a> <a id="35066" class="Keyword">import</a> <a id="35073" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="35120" class="Keyword">open</a> <a id="35125" class="Keyword">import</a> <a id="35132" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="35177" class="Keyword">open</a> <a id="35182" class="Keyword">import</a> <a id="35189" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="35238" class="Keyword">open</a> <a id="35243" class="Keyword">import</a> <a id="35250" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="35327" class="Keyword">open</a> <a id="35332" class="Keyword">import</a> <a id="35339" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="35391" class="Keyword">open</a> <a id="35396" class="Keyword">import</a> <a id="35403" href="type-theories.html" class="Module">type-theories</a>
<a id="35417" class="Keyword">open</a> <a id="35422" class="Keyword">import</a> <a id="35429" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="35471" class="Keyword">open</a> <a id="35476" class="Keyword">import</a> <a id="35483" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="35521" class="Keyword">open</a> <a id="35526" class="Keyword">import</a> <a id="35533" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="35579" class="Keyword">open</a> <a id="35584" class="Keyword">import</a> <a id="35591" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="35638" class="Keyword">open</a> <a id="35643" class="Keyword">import</a> <a id="35650" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="35685" class="Keyword">open</a> <a id="35690" class="Keyword">import</a> <a id="35697" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="35775" class="Keyword">open</a> <a id="35780" class="Keyword">import</a> <a id="35787" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="35811" class="Keyword">open</a> <a id="35816" class="Keyword">import</a> <a id="35823" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="35876" class="Keyword">open</a> <a id="35881" class="Keyword">import</a> <a id="35888" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="35931" class="Keyword">open</a> <a id="35936" class="Keyword">import</a> <a id="35943" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="35983" class="Keyword">open</a> <a id="35988" class="Keyword">import</a> <a id="35995" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="36034" class="Keyword">open</a> <a id="36039" class="Keyword">import</a> <a id="36046" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="36080" class="Keyword">open</a> <a id="36085" class="Keyword">import</a> <a id="36092" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="36140" class="Keyword">open</a> <a id="36145" class="Keyword">import</a> <a id="36152" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="36203" class="Keyword">open</a> <a id="36208" class="Keyword">import</a> <a id="36215" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="36262" class="Keyword">open</a> <a id="36267" class="Keyword">import</a> <a id="36274" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="36326" class="Keyword">open</a> <a id="36331" class="Keyword">import</a> <a id="36338" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="36382" class="Keyword">open</a> <a id="36387" class="Keyword">import</a> <a id="36394" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="36434" class="Keyword">open</a> <a id="36439" class="Keyword">import</a> <a id="36446" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="36489" class="Keyword">open</a> <a id="36494" class="Keyword">import</a> <a id="36501" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="36553" class="Keyword">open</a> <a id="36558" class="Keyword">import</a> <a id="36565" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="36619" class="Keyword">open</a> <a id="36624" class="Keyword">import</a> <a id="36631" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="36679" class="Keyword">open</a> <a id="36684" class="Keyword">import</a> <a id="36691" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="36730" class="Keyword">open</a> <a id="36735" class="Keyword">import</a> <a id="36742" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="36775" class="Keyword">open</a> <a id="36780" class="Keyword">import</a> <a id="36787" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="36817" class="Keyword">open</a> <a id="36822" class="Keyword">import</a> <a id="36829" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="36880" class="Keyword">open</a> <a id="36885" class="Keyword">import</a> <a id="36892" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="36933" class="Keyword">open</a> <a id="36938" class="Keyword">import</a> <a id="36945" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="36982" class="Keyword">open</a> <a id="36987" class="Keyword">import</a> <a id="36994" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="37053" class="Keyword">open</a> <a id="37058" class="Keyword">import</a> <a id="37065" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="37120" class="Keyword">open</a> <a id="37125" class="Keyword">import</a> <a id="37132" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="37188" class="Keyword">open</a> <a id="37193" class="Keyword">import</a> <a id="37200" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="37247" class="Keyword">open</a> <a id="37252" class="Keyword">import</a> <a id="37259" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="37302" class="Keyword">open</a> <a id="37307" class="Keyword">import</a> <a id="37314" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="37359" class="Keyword">open</a> <a id="37364" class="Keyword">import</a> <a id="37371" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="37420" class="Keyword">open</a> <a id="37425" class="Keyword">import</a> <a id="37432" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="37483" class="Keyword">open</a> <a id="37488" class="Keyword">import</a> <a id="37495" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="37539" class="Keyword">open</a> <a id="37544" class="Keyword">import</a> <a id="37551" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="37629" class="Keyword">open</a> <a id="37634" class="Keyword">import</a> <a id="37641" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="37681" class="Keyword">open</a> <a id="37686" class="Keyword">import</a> <a id="37693" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="37750" class="Keyword">open</a> <a id="37755" class="Keyword">import</a> <a id="37762" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="37797" class="Keyword">open</a> <a id="37802" class="Keyword">import</a> <a id="37809" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="37855" class="Keyword">open</a> <a id="37860" class="Keyword">import</a> <a id="37867" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="37922" class="Keyword">open</a> <a id="37927" class="Keyword">import</a> <a id="37934" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="37977" class="Keyword">open</a> <a id="37982" class="Keyword">import</a> <a id="37989" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="38034" class="Keyword">open</a> <a id="38039" class="Keyword">import</a> <a id="38046" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="38105" class="Keyword">open</a> <a id="38110" class="Keyword">import</a> <a id="38117" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="38154" class="Keyword">open</a> <a id="38159" class="Keyword">import</a> <a id="38166" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="38208" class="Keyword">open</a> <a id="38213" class="Keyword">import</a> <a id="38220" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="38261" class="Keyword">open</a> <a id="38266" class="Keyword">import</a> <a id="38273" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="38312" class="Keyword">open</a> <a id="38317" class="Keyword">import</a> <a id="38324" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="38362" class="Keyword">open</a> <a id="38367" class="Keyword">import</a> <a id="38374" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="38426" class="Keyword">open</a> <a id="38431" class="Keyword">import</a> <a id="38438" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="38483" class="Keyword">open</a> <a id="38488" class="Keyword">import</a> <a id="38495" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="38534" class="Keyword">open</a> <a id="38539" class="Keyword">import</a> <a id="38546" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="38583" class="Keyword">open</a> <a id="38588" class="Keyword">import</a> <a id="38595" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="38644" class="Keyword">open</a> <a id="38649" class="Keyword">import</a> <a id="38656" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="38695" class="Keyword">open</a> <a id="38700" class="Keyword">import</a> <a id="38707" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="38745" class="Keyword">open</a> <a id="38750" class="Keyword">import</a> <a id="38757" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="38812" class="Keyword">open</a> <a id="38817" class="Keyword">import</a> <a id="38824" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="38863" class="Keyword">open</a> <a id="38868" class="Keyword">import</a> <a id="38875" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="38923" class="Keyword">open</a> <a id="38928" class="Keyword">import</a> <a id="38935" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="38982" class="Keyword">open</a> <a id="38987" class="Keyword">import</a> <a id="38994" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="39032" class="Keyword">open</a> <a id="39037" class="Keyword">import</a> <a id="39044" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="39074" class="Keyword">open</a> <a id="39079" class="Keyword">import</a> <a id="39086" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="39143" class="Keyword">open</a> <a id="39148" class="Keyword">import</a> <a id="39155" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="39209" class="Keyword">open</a> <a id="39214" class="Keyword">import</a> <a id="39221" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="39251" class="Keyword">open</a> <a id="39256" class="Keyword">import</a> <a id="39263" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="39312" class="Keyword">open</a> <a id="39317" class="Keyword">import</a> <a id="39324" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="39366" class="Keyword">open</a> <a id="39371" class="Keyword">import</a> <a id="39378" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="39412" class="Keyword">open</a> <a id="39417" class="Keyword">import</a> <a id="39424" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="39487" class="Keyword">open</a> <a id="39492" class="Keyword">import</a> <a id="39499" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="39542" class="Keyword">open</a> <a id="39547" class="Keyword">import</a> <a id="39554" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="39589" class="Keyword">open</a> <a id="39594" class="Keyword">import</a> <a id="39601" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="39636" class="Keyword">open</a> <a id="39641" class="Keyword">import</a> <a id="39648" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="39688" class="Keyword">open</a> <a id="39693" class="Keyword">import</a> <a id="39700" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="39745" class="Keyword">open</a> <a id="39750" class="Keyword">import</a> <a id="39757" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="39798" class="Keyword">open</a> <a id="39803" class="Keyword">import</a> <a id="39810" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="39864" class="Keyword">open</a> <a id="39869" class="Keyword">import</a> <a id="39876" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="39926" class="Keyword">open</a> <a id="39931" class="Keyword">import</a> <a id="39938" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="39985" class="Keyword">open</a> <a id="39990" class="Keyword">import</a> <a id="39997" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="40035" class="Keyword">open</a> <a id="40040" class="Keyword">import</a> <a id="40047" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="40096" class="Keyword">open</a> <a id="40101" class="Keyword">import</a> <a id="40108" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="40155" class="Keyword">open</a> <a id="40160" class="Keyword">import</a> <a id="40167" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="40230" class="Keyword">open</a> <a id="40235" class="Keyword">import</a> <a id="40242" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="40274" class="Keyword">open</a> <a id="40279" class="Keyword">import</a> <a id="40286" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="40339" class="Keyword">open</a> <a id="40344" class="Keyword">import</a> <a id="40351" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="40397" class="Keyword">open</a> <a id="40402" class="Keyword">import</a> <a id="40409" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="40455" class="Keyword">open</a> <a id="40460" class="Keyword">import</a> <a id="40467" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="40507" class="Keyword">open</a> <a id="40512" class="Keyword">import</a> <a id="40519" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="40566" class="Keyword">open</a> <a id="40571" class="Keyword">import</a> <a id="40578" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="40626" class="Keyword">open</a> <a id="40631" class="Keyword">import</a> <a id="40638" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="40678" class="Keyword">open</a> <a id="40683" class="Keyword">import</a> <a id="40690" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="40735" class="Keyword">open</a> <a id="40740" class="Keyword">import</a> <a id="40747" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="40812" class="Keyword">open</a> <a id="40817" class="Keyword">import</a> <a id="40824" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="40869" class="Keyword">open</a> <a id="40874" class="Keyword">import</a> <a id="40881" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="40928" class="Keyword">open</a> <a id="40933" class="Keyword">import</a> <a id="40940" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="40993" class="Keyword">open</a> <a id="40998" class="Keyword">import</a> <a id="41005" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>