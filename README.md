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
<a id="5373" class="Keyword">open</a> <a id="5378" class="Keyword">import</a> <a id="5385" href="commutative-algebra.zarisky-topology.html" class="Module">commutative-algebra.zarisky-topology</a>
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
<a id="8971" class="Keyword">open</a> <a id="8976" class="Keyword">import</a> <a id="8983" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="9025" class="Keyword">open</a> <a id="9030" class="Keyword">import</a> <a id="9037" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="9088" class="Keyword">open</a> <a id="9093" class="Keyword">import</a> <a id="9100" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9158" class="Keyword">open</a> <a id="9163" class="Keyword">import</a> <a id="9170" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9234" class="Keyword">open</a> <a id="9239" class="Keyword">import</a> <a id="9246" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9299" class="Keyword">open</a> <a id="9304" class="Keyword">import</a> <a id="9311" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9364" class="Keyword">open</a> <a id="9369" class="Keyword">import</a> <a id="9376" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9437" class="Keyword">open</a> <a id="9442" class="Keyword">import</a> <a id="9449" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9507" class="Keyword">open</a> <a id="9512" class="Keyword">import</a> <a id="9519" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9568" class="Keyword">open</a> <a id="9573" class="Keyword">import</a> <a id="9580" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9623" class="Keyword">open</a> <a id="9628" class="Keyword">import</a> <a id="9635" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9679" class="Keyword">open</a> <a id="9684" class="Keyword">import</a> <a id="9691" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9738" class="Keyword">open</a> <a id="9743" class="Keyword">import</a> <a id="9750" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9811" class="Keyword">open</a> <a id="9816" class="Keyword">import</a> <a id="9823" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9886" class="Keyword">open</a> <a id="9891" class="Keyword">import</a> <a id="9898" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="9958" class="Keyword">open</a> <a id="9963" class="Keyword">import</a> <a id="9970" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="10024" class="Keyword">open</a> <a id="10029" class="Keyword">import</a> <a id="10036" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="10101" class="Keyword">open</a> <a id="10106" class="Keyword">import</a> <a id="10113" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10221" class="Keyword">open</a> <a id="10226" class="Keyword">import</a> <a id="10233" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10253" class="Keyword">open</a> <a id="10258" class="Keyword">import</a> <a id="10265" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10311" class="Keyword">open</a> <a id="10316" class="Keyword">import</a> <a id="10323" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10379" class="Keyword">open</a> <a id="10384" class="Keyword">import</a> <a id="10391" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10437" class="Keyword">open</a> <a id="10442" class="Keyword">import</a> <a id="10449" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10483" class="Keyword">open</a> <a id="10488" class="Keyword">import</a> <a id="10495" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10530" class="Keyword">open</a> <a id="10535" class="Keyword">import</a> <a id="10542" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10580" class="Keyword">open</a> <a id="10585" class="Keyword">import</a> <a id="10592" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10630" class="Keyword">open</a> <a id="10635" class="Keyword">import</a> <a id="10642" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10682" class="Keyword">open</a> <a id="10687" class="Keyword">import</a> <a id="10694" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10727" class="Keyword">open</a> <a id="10732" class="Keyword">import</a> <a id="10739" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10777" class="Keyword">open</a> <a id="10782" class="Keyword">import</a> <a id="10789" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10852" class="Keyword">open</a> <a id="10857" class="Keyword">import</a> <a id="10864" href="foundation.html" class="Module">foundation</a>
<a id="10875" class="Keyword">open</a> <a id="10880" class="Keyword">import</a> <a id="10887" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10905" class="Keyword">open</a> <a id="10910" class="Keyword">import</a> <a id="10917" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10936" class="Keyword">open</a> <a id="10941" class="Keyword">import</a> <a id="10948" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10967" class="Keyword">open</a> <a id="10972" class="Keyword">import</a> <a id="10979" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11023" class="Keyword">open</a> <a id="11028" class="Keyword">import</a> <a id="11035" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11060" class="Keyword">open</a> <a id="11065" class="Keyword">import</a> <a id="11072" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11099" class="Keyword">open</a> <a id="11104" class="Keyword">import</a> <a id="11111" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11128" class="Keyword">open</a> <a id="11133" class="Keyword">import</a> <a id="11140" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11169" class="Keyword">open</a> <a id="11174" class="Keyword">import</a> <a id="11181" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11237" class="Keyword">open</a> <a id="11242" class="Keyword">import</a> <a id="11249" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11280" class="Keyword">open</a> <a id="11285" class="Keyword">import</a> <a id="11292" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11346" class="Keyword">open</a> <a id="11351" class="Keyword">import</a> <a id="11358" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11386" class="Keyword">open</a> <a id="11391" class="Keyword">import</a> <a id="11398" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11428" class="Keyword">open</a> <a id="11433" class="Keyword">import</a> <a id="11440" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11460" class="Keyword">open</a> <a id="11465" class="Keyword">import</a> <a id="11472" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11517" class="Keyword">open</a> <a id="11522" class="Keyword">import</a> <a id="11529" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11566" class="Keyword">open</a> <a id="11571" class="Keyword">import</a> <a id="11578" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11613" class="Keyword">open</a> <a id="11618" class="Keyword">import</a> <a id="11625" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11683" class="Keyword">open</a> <a id="11688" class="Keyword">import</a> <a id="11695" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11733" class="Keyword">open</a> <a id="11738" class="Keyword">import</a> <a id="11745" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11779" class="Keyword">open</a> <a id="11784" class="Keyword">import</a> <a id="11791" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11820" class="Keyword">open</a> <a id="11825" class="Keyword">import</a> <a id="11832" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11855" class="Keyword">open</a> <a id="11860" class="Keyword">import</a> <a id="11867" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="11894" class="Keyword">open</a> <a id="11899" class="Keyword">import</a> <a id="11906" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11929" class="Keyword">open</a> <a id="11934" class="Keyword">import</a> <a id="11941" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="11983" class="Keyword">open</a> <a id="11988" class="Keyword">import</a> <a id="11995" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12027" class="Keyword">open</a> <a id="12032" class="Keyword">import</a> <a id="12039" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12066" class="Keyword">open</a> <a id="12071" class="Keyword">import</a> <a id="12078" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12103" class="Keyword">open</a> <a id="12108" class="Keyword">import</a> <a id="12115" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12144" class="Keyword">open</a> <a id="12149" class="Keyword">import</a> <a id="12156" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12186" class="Keyword">open</a> <a id="12191" class="Keyword">import</a> <a id="12198" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12225" class="Keyword">open</a> <a id="12230" class="Keyword">import</a> <a id="12237" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12256" class="Keyword">open</a> <a id="12261" class="Keyword">import</a> <a id="12268" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12314" class="Keyword">open</a> <a id="12319" class="Keyword">import</a> <a id="12326" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12368" class="Keyword">open</a> <a id="12373" class="Keyword">import</a> <a id="12380" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12412" class="Keyword">open</a> <a id="12417" class="Keyword">import</a> <a id="12424" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12454" class="Keyword">open</a> <a id="12459" class="Keyword">import</a> <a id="12466" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12492" class="Keyword">open</a> <a id="12497" class="Keyword">import</a> <a id="12504" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12538" class="Keyword">open</a> <a id="12543" class="Keyword">import</a> <a id="12550" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12580" class="Keyword">open</a> <a id="12585" class="Keyword">import</a> <a id="12592" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12619" class="Keyword">open</a> <a id="12624" class="Keyword">import</a> <a id="12631" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="12669" class="Keyword">open</a> <a id="12674" class="Keyword">import</a> <a id="12681" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12713" class="Keyword">open</a> <a id="12718" class="Keyword">import</a> <a id="12725" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12759" class="Keyword">open</a> <a id="12764" class="Keyword">import</a> <a id="12771" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12794" class="Keyword">open</a> <a id="12799" class="Keyword">import</a> <a id="12806" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12833" class="Keyword">open</a> <a id="12838" class="Keyword">import</a> <a id="12845" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12873" class="Keyword">open</a> <a id="12878" class="Keyword">import</a> <a id="12885" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12922" class="Keyword">open</a> <a id="12927" class="Keyword">import</a> <a id="12934" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12982" class="Keyword">open</a> <a id="12987" class="Keyword">import</a> <a id="12994" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13034" class="Keyword">open</a> <a id="13039" class="Keyword">import</a> <a id="13046" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13068" class="Keyword">open</a> <a id="13073" class="Keyword">import</a> <a id="13080" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13103" class="Keyword">open</a> <a id="13108" class="Keyword">import</a> <a id="13115" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13140" class="Keyword">open</a> <a id="13145" class="Keyword">import</a> <a id="13152" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13197" class="Keyword">open</a> <a id="13202" class="Keyword">import</a> <a id="13209" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13253" class="Keyword">open</a> <a id="13258" class="Keyword">import</a> <a id="13265" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13301" class="Keyword">open</a> <a id="13306" class="Keyword">import</a> <a id="13313" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13358" class="Keyword">open</a> <a id="13363" class="Keyword">import</a> <a id="13370" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13411" class="Keyword">open</a> <a id="13416" class="Keyword">import</a> <a id="13423" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13458" class="Keyword">open</a> <a id="13463" class="Keyword">import</a> <a id="13470" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13502" class="Keyword">open</a> <a id="13507" class="Keyword">import</a> <a id="13514" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13545" class="Keyword">open</a> <a id="13550" class="Keyword">import</a> <a id="13557" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13590" class="Keyword">open</a> <a id="13595" class="Keyword">import</a> <a id="13602" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13635" class="Keyword">open</a> <a id="13640" class="Keyword">import</a> <a id="13647" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13677" class="Keyword">open</a> <a id="13682" class="Keyword">import</a> <a id="13689" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13713" class="Keyword">open</a> <a id="13718" class="Keyword">import</a> <a id="13725" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13763" class="Keyword">open</a> <a id="13768" class="Keyword">import</a> <a id="13775" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13806" class="Keyword">open</a> <a id="13811" class="Keyword">import</a> <a id="13818" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13843" class="Keyword">open</a> <a id="13848" class="Keyword">import</a> <a id="13855" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13883" class="Keyword">open</a> <a id="13888" class="Keyword">import</a> <a id="13895" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13919" class="Keyword">open</a> <a id="13924" class="Keyword">import</a> <a id="13931" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13957" class="Keyword">open</a> <a id="13962" class="Keyword">import</a> <a id="13969" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="14004" class="Keyword">open</a> <a id="14009" class="Keyword">import</a> <a id="14016" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14037" class="Keyword">open</a> <a id="14042" class="Keyword">import</a> <a id="14049" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14098" class="Keyword">open</a> <a id="14103" class="Keyword">import</a> <a id="14110" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14151" class="Keyword">open</a> <a id="14156" class="Keyword">import</a> <a id="14163" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14213" class="Keyword">open</a> <a id="14218" class="Keyword">import</a> <a id="14225" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14271" class="Keyword">open</a> <a id="14276" class="Keyword">import</a> <a id="14283" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14323" class="Keyword">open</a> <a id="14328" class="Keyword">import</a> <a id="14335" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14385" class="Keyword">open</a> <a id="14390" class="Keyword">import</a> <a id="14397" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14436" class="Keyword">open</a> <a id="14441" class="Keyword">import</a> <a id="14448" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14488" class="Keyword">open</a> <a id="14493" class="Keyword">import</a> <a id="14500" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14533" class="Keyword">open</a> <a id="14538" class="Keyword">import</a> <a id="14545" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14594" class="Keyword">open</a> <a id="14599" class="Keyword">import</a> <a id="14606" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14631" class="Keyword">open</a> <a id="14636" class="Keyword">import</a> <a id="14643" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14681" class="Keyword">open</a> <a id="14686" class="Keyword">import</a> <a id="14693" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14715" class="Keyword">open</a> <a id="14720" class="Keyword">import</a> <a id="14727" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14755" class="Keyword">open</a> <a id="14760" class="Keyword">import</a> <a id="14767" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="14803" class="Keyword">open</a> <a id="14808" class="Keyword">import</a> <a id="14815" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14841" class="Keyword">open</a> <a id="14846" class="Keyword">import</a> <a id="14853" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14871" class="Keyword">open</a> <a id="14876" class="Keyword">import</a> <a id="14883" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14918" class="Keyword">open</a> <a id="14923" class="Keyword">import</a> <a id="14930" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="14965" class="Keyword">open</a> <a id="14970" class="Keyword">import</a> <a id="14977" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="15004" class="Keyword">open</a> <a id="15009" class="Keyword">import</a> <a id="15016" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15072" class="Keyword">open</a> <a id="15077" class="Keyword">import</a> <a id="15084" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15113" class="Keyword">open</a> <a id="15118" class="Keyword">import</a> <a id="15125" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15155" class="Keyword">open</a> <a id="15160" class="Keyword">import</a> <a id="15167" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15194" class="Keyword">open</a> <a id="15199" class="Keyword">import</a> <a id="15206" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15232" class="Keyword">open</a> <a id="15237" class="Keyword">import</a> <a id="15244" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15271" class="Keyword">open</a> <a id="15276" class="Keyword">import</a> <a id="15283" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15307" class="Keyword">open</a> <a id="15312" class="Keyword">import</a> <a id="15319" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15342" class="Keyword">open</a> <a id="15347" class="Keyword">import</a> <a id="15354" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15381" class="Keyword">open</a> <a id="15386" class="Keyword">import</a> <a id="15393" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15425" class="Keyword">open</a> <a id="15430" class="Keyword">import</a> <a id="15437" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15472" class="Keyword">open</a> <a id="15477" class="Keyword">import</a> <a id="15484" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15515" class="Keyword">open</a> <a id="15520" class="Keyword">import</a> <a id="15527" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15560" class="Keyword">open</a> <a id="15565" class="Keyword">import</a> <a id="15572" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15606" class="Keyword">open</a> <a id="15611" class="Keyword">import</a> <a id="15618" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15658" class="Keyword">open</a> <a id="15663" class="Keyword">import</a> <a id="15670" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15701" class="Keyword">open</a> <a id="15706" class="Keyword">import</a> <a id="15713" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15745" class="Keyword">open</a> <a id="15750" class="Keyword">import</a> <a id="15757" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15788" class="Keyword">open</a> <a id="15793" class="Keyword">import</a> <a id="15800" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15817" class="Keyword">open</a> <a id="15822" class="Keyword">import</a> <a id="15829" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15854" class="Keyword">open</a> <a id="15859" class="Keyword">import</a> <a id="15866" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15895" class="Keyword">open</a> <a id="15900" class="Keyword">import</a> <a id="15907" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15932" class="Keyword">open</a> <a id="15937" class="Keyword">import</a> <a id="15944" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15965" class="Keyword">open</a> <a id="15970" class="Keyword">import</a> <a id="15977" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="16001" class="Keyword">open</a> <a id="16006" class="Keyword">import</a> <a id="16013" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16033" class="Keyword">open</a> <a id="16038" class="Keyword">import</a> <a id="16045" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16079" class="Keyword">open</a> <a id="16084" class="Keyword">import</a> <a id="16091" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16129" class="Keyword">open</a> <a id="16134" class="Keyword">import</a> <a id="16141" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16169" class="Keyword">open</a> <a id="16174" class="Keyword">import</a> <a id="16181" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16205" class="Keyword">open</a> <a id="16210" class="Keyword">import</a> <a id="16217" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16244" class="Keyword">open</a> <a id="16249" class="Keyword">import</a> <a id="16256" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16291" class="Keyword">open</a> <a id="16296" class="Keyword">import</a> <a id="16303" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16324" class="Keyword">open</a> <a id="16329" class="Keyword">import</a> <a id="16336" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16372" class="Keyword">open</a> <a id="16377" class="Keyword">import</a> <a id="16384" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16429" class="Keyword">open</a> <a id="16434" class="Keyword">import</a> <a id="16441" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16487" class="Keyword">open</a> <a id="16492" class="Keyword">import</a> <a id="16499" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16539" class="Keyword">open</a> <a id="16544" class="Keyword">import</a> <a id="16551" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16581" class="Keyword">open</a> <a id="16586" class="Keyword">import</a> <a id="16593" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="16627" class="Keyword">open</a> <a id="16632" class="Keyword">import</a> <a id="16639" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16676" class="Keyword">open</a> <a id="16681" class="Keyword">import</a> <a id="16688" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16712" class="Keyword">open</a> <a id="16717" class="Keyword">import</a> <a id="16724" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16745" class="Keyword">open</a> <a id="16750" class="Keyword">import</a> <a id="16757" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16792" class="Keyword">open</a> <a id="16797" class="Keyword">import</a> <a id="16804" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16841" class="Keyword">open</a> <a id="16846" class="Keyword">import</a> <a id="16853" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16902" class="Keyword">open</a> <a id="16907" class="Keyword">import</a> <a id="16914" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16947" class="Keyword">open</a> <a id="16952" class="Keyword">import</a> <a id="16959" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16982" class="Keyword">open</a> <a id="16987" class="Keyword">import</a> <a id="16994" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="17017" class="Keyword">open</a> <a id="17022" class="Keyword">import</a> <a id="17029" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="17052" class="Keyword">open</a> <a id="17057" class="Keyword">import</a> <a id="17064" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17092" class="Keyword">open</a> <a id="17097" class="Keyword">import</a> <a id="17104" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17124" class="Keyword">open</a> <a id="17129" class="Keyword">import</a> <a id="17136" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17157" class="Keyword">open</a> <a id="17162" class="Keyword">import</a> <a id="17169" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17200" class="Keyword">open</a> <a id="17205" class="Keyword">import</a> <a id="17212" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17239" class="Keyword">open</a> <a id="17244" class="Keyword">import</a> <a id="17251" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17267" class="Keyword">open</a> <a id="17272" class="Keyword">import</a> <a id="17279" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17310" class="Keyword">open</a> <a id="17315" class="Keyword">import</a> <a id="17322" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17339" class="Keyword">open</a> <a id="17344" class="Keyword">import</a> <a id="17351" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17373" class="Keyword">open</a> <a id="17378" class="Keyword">import</a> <a id="17385" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17412" class="Keyword">open</a> <a id="17417" class="Keyword">import</a> <a id="17424" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17447" class="Keyword">open</a> <a id="17452" class="Keyword">import</a> <a id="17459" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17486" class="Keyword">open</a> <a id="17491" class="Keyword">import</a> <a id="17498" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17531" class="Keyword">open</a> <a id="17536" class="Keyword">import</a> <a id="17543" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17583" class="Keyword">open</a> <a id="17588" class="Keyword">import</a> <a id="17595" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17616" class="Keyword">open</a> <a id="17621" class="Keyword">import</a> <a id="17628" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17657" class="Keyword">open</a> <a id="17662" class="Keyword">import</a> <a id="17669" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17707" class="Keyword">open</a> <a id="17712" class="Keyword">import</a> <a id="17719" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17739" class="Keyword">open</a> <a id="17744" class="Keyword">import</a> <a id="17751" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17775" class="Keyword">open</a> <a id="17780" class="Keyword">import</a> <a id="17787" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17814" class="Keyword">open</a> <a id="17819" class="Keyword">import</a> <a id="17826" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17858" class="Keyword">open</a> <a id="17863" class="Keyword">import</a> <a id="17870" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17900" class="Keyword">open</a> <a id="17905" class="Keyword">import</a> <a id="17912" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17938" class="Keyword">open</a> <a id="17943" class="Keyword">import</a> <a id="17950" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17977" class="Keyword">open</a> <a id="17982" class="Keyword">import</a> <a id="17989" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="18018" class="Keyword">open</a> <a id="18023" class="Keyword">import</a> <a id="18030" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="18053" class="Keyword">open</a> <a id="18058" class="Keyword">import</a> <a id="18065" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18116" class="Keyword">open</a> <a id="18121" class="Keyword">import</a> <a id="18128" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18171" class="Keyword">open</a> <a id="18176" class="Keyword">import</a> <a id="18183" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18231" class="Keyword">open</a> <a id="18236" class="Keyword">import</a> <a id="18243" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18281" class="Keyword">open</a> <a id="18286" class="Keyword">import</a> <a id="18293" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18330" class="Keyword">open</a> <a id="18335" class="Keyword">import</a> <a id="18342" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18388" class="Keyword">open</a> <a id="18393" class="Keyword">import</a> <a id="18400" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18417" class="Keyword">open</a> <a id="18422" class="Keyword">import</a> <a id="18429" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18457" class="Keyword">open</a> <a id="18462" class="Keyword">import</a> <a id="18469" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18497" class="Keyword">open</a> <a id="18502" class="Keyword">import</a> <a id="18509" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18545" class="Keyword">open</a> <a id="18550" class="Keyword">import</a> <a id="18557" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18595" class="Keyword">open</a> <a id="18600" class="Keyword">import</a> <a id="18607" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18640" class="Keyword">open</a> <a id="18645" class="Keyword">import</a> <a id="18652" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18673" class="Keyword">open</a> <a id="18678" class="Keyword">import</a> <a id="18685" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="18721" class="Keyword">open</a> <a id="18726" class="Keyword">import</a> <a id="18733" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18787" class="Keyword">open</a> <a id="18792" class="Keyword">import</a> <a id="18799" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18821" class="Keyword">open</a> <a id="18826" class="Keyword">import</a> <a id="18833" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18868" class="Keyword">open</a> <a id="18873" class="Keyword">import</a> <a id="18880" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18910" class="Keyword">open</a> <a id="18915" class="Keyword">import</a> <a id="18922" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18961" class="Keyword">open</a> <a id="18966" class="Keyword">import</a> <a id="18973" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="19027" class="Keyword">open</a> <a id="19032" class="Keyword">import</a> <a id="19039" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="19085" class="Keyword">open</a> <a id="19090" class="Keyword">import</a> <a id="19097" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="19148" class="Keyword">open</a> <a id="19153" class="Keyword">import</a> <a id="19160" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19201" class="Keyword">open</a> <a id="19206" class="Keyword">import</a> <a id="19213" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19258" class="Keyword">open</a> <a id="19263" class="Keyword">import</a> <a id="19270" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19315" class="Keyword">open</a> <a id="19320" class="Keyword">import</a> <a id="19327" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19363" class="Keyword">open</a> <a id="19368" class="Keyword">import</a> <a id="19375" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19411" class="Keyword">open</a> <a id="19416" class="Keyword">import</a> <a id="19423" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19488" class="Keyword">open</a> <a id="19493" class="Keyword">import</a> <a id="19500" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19555" class="Keyword">open</a> <a id="19560" class="Keyword">import</a> <a id="19567" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19607" class="Keyword">open</a> <a id="19612" class="Keyword">import</a> <a id="19619" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19663" class="Keyword">open</a> <a id="19668" class="Keyword">import</a> <a id="19675" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19720" class="Keyword">open</a> <a id="19725" class="Keyword">import</a> <a id="19732" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19773" class="Keyword">open</a> <a id="19778" class="Keyword">import</a> <a id="19785" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19825" class="Keyword">open</a> <a id="19830" class="Keyword">import</a> <a id="19837" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19864" class="Keyword">open</a> <a id="19869" class="Keyword">import</a> <a id="19876" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19912" class="Keyword">open</a> <a id="19917" class="Keyword">import</a> <a id="19924" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19951" class="Keyword">open</a> <a id="19956" class="Keyword">import</a> <a id="19963" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="20000" class="Keyword">open</a> <a id="20005" class="Keyword">import</a> <a id="20012" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="20040" class="Keyword">open</a> <a id="20045" class="Keyword">import</a> <a id="20052" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="20071" class="Keyword">open</a> <a id="20076" class="Keyword">import</a> <a id="20083" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="20123" class="Keyword">open</a> <a id="20128" class="Keyword">import</a> <a id="20135" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="20167" class="Keyword">open</a> <a id="20172" class="Keyword">import</a> <a id="20179" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20227" class="Keyword">open</a> <a id="20232" class="Keyword">import</a> <a id="20239" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20262" class="Keyword">open</a> <a id="20267" class="Keyword">import</a> <a id="20274" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20298" class="Keyword">open</a> <a id="20303" class="Keyword">import</a> <a id="20310" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20350" class="Keyword">open</a> <a id="20355" class="Keyword">import</a> <a id="20362" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20405" class="Keyword">open</a> <a id="20410" class="Keyword">import</a> <a id="20417" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20451" class="Keyword">open</a> <a id="20456" class="Keyword">import</a> <a id="20463" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20495" class="Keyword">open</a> <a id="20500" class="Keyword">import</a> <a id="20507" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20537" class="Keyword">open</a> <a id="20542" class="Keyword">import</a> <a id="20549" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20583" class="Keyword">open</a> <a id="20588" class="Keyword">import</a> <a id="20595" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20630" class="Keyword">open</a> <a id="20635" class="Keyword">import</a> <a id="20642" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20679" class="Keyword">open</a> <a id="20684" class="Keyword">import</a> <a id="20691" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20718" class="Keyword">open</a> <a id="20723" class="Keyword">import</a> <a id="20730" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20758" class="Keyword">open</a> <a id="20763" class="Keyword">import</a> <a id="20770" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20819" class="Keyword">open</a> <a id="20824" class="Keyword">import</a> <a id="20831" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20877" class="Keyword">open</a> <a id="20882" class="Keyword">import</a> <a id="20889" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20929" class="Keyword">open</a> <a id="20934" class="Keyword">import</a> <a id="20941" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20979" class="Keyword">open</a> <a id="20984" class="Keyword">import</a> <a id="20991" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="21020" class="Keyword">open</a> <a id="21025" class="Keyword">import</a> <a id="21032" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="21062" class="Keyword">open</a> <a id="21067" class="Keyword">import</a> <a id="21074" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="21105" class="Keyword">open</a> <a id="21110" class="Keyword">import</a> <a id="21117" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="21157" class="Keyword">open</a> <a id="21162" class="Keyword">import</a> <a id="21169" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21195" class="Keyword">open</a> <a id="21200" class="Keyword">import</a> <a id="21207" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21262" class="Keyword">open</a> <a id="21267" class="Keyword">import</a> <a id="21274" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21325" class="Keyword">open</a> <a id="21330" class="Keyword">import</a> <a id="21337" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21382" class="Keyword">open</a> <a id="21387" class="Keyword">import</a> <a id="21394" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21448" class="Keyword">open</a> <a id="21453" class="Keyword">import</a> <a id="21460" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21487" class="Keyword">open</a> <a id="21492" class="Keyword">import</a> <a id="21499" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21532" class="Keyword">open</a> <a id="21537" class="Keyword">import</a> <a id="21544" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21575" class="Keyword">open</a> <a id="21580" class="Keyword">import</a> <a id="21587" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21624" class="Keyword">open</a> <a id="21629" class="Keyword">import</a> <a id="21636" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21661" class="Keyword">open</a> <a id="21666" class="Keyword">import</a> <a id="21673" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21705" class="Keyword">open</a> <a id="21710" class="Keyword">import</a> <a id="21717" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21752" class="Keyword">open</a> <a id="21757" class="Keyword">import</a> <a id="21764" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21793" class="Keyword">open</a> <a id="21798" class="Keyword">import</a> <a id="21805" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21831" class="Keyword">open</a> <a id="21836" class="Keyword">import</a> <a id="21843" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21871" class="Keyword">open</a> <a id="21876" class="Keyword">import</a> <a id="21883" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21908" class="Keyword">open</a> <a id="21913" class="Keyword">import</a> <a id="21920" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21941" class="Keyword">open</a> <a id="21946" class="Keyword">import</a> <a id="21953" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21989" class="Keyword">open</a> <a id="21994" class="Keyword">import</a> <a id="22001" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="22044" class="Keyword">open</a> <a id="22049" class="Keyword">import</a> <a id="22056" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="22081" class="Keyword">open</a> <a id="22086" class="Keyword">import</a> <a id="22093" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="22124" class="Keyword">open</a> <a id="22129" class="Keyword">import</a> <a id="22136" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="22168" class="Keyword">open</a> <a id="22173" class="Keyword">import</a> <a id="22180" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22214" class="Keyword">open</a> <a id="22219" class="Keyword">import</a> <a id="22226" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22282" class="Keyword">open</a> <a id="22287" class="Keyword">import</a> <a id="22294" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22347" class="Keyword">open</a> <a id="22352" class="Keyword">import</a> <a id="22359" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22386" class="Keyword">open</a> <a id="22391" class="Keyword">import</a> <a id="22398" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22443" class="Keyword">open</a> <a id="22448" class="Keyword">import</a> <a id="22455" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22517" class="Keyword">open</a> <a id="22522" class="Keyword">import</a> <a id="22529" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22542" class="Keyword">open</a> <a id="22547" class="Keyword">import</a> <a id="22554" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="22594" class="Keyword">open</a> <a id="22599" class="Keyword">import</a> <a id="22606" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="22650" class="Keyword">open</a> <a id="22655" class="Keyword">import</a> <a id="22662" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22703" class="Keyword">open</a> <a id="22708" class="Keyword">import</a> <a id="22715" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="22753" class="Keyword">open</a> <a id="22758" class="Keyword">import</a> <a id="22765" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22794" class="Keyword">open</a> <a id="22799" class="Keyword">import</a> <a id="22806" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22851" class="Keyword">open</a> <a id="22856" class="Keyword">import</a> <a id="22863" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="22905" class="Keyword">open</a> <a id="22910" class="Keyword">import</a> <a id="22917" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22961" class="Keyword">open</a> <a id="22966" class="Keyword">import</a> <a id="22973" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="23022" class="Keyword">open</a> <a id="23027" class="Keyword">import</a> <a id="23034" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="23084" class="Keyword">open</a> <a id="23089" class="Keyword">import</a> <a id="23096" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="23123" class="Keyword">open</a> <a id="23128" class="Keyword">import</a> <a id="23135" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="23176" class="Keyword">open</a> <a id="23181" class="Keyword">import</a> <a id="23188" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="23211" class="Keyword">open</a> <a id="23216" class="Keyword">import</a> <a id="23223" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="23272" class="Keyword">open</a> <a id="23277" class="Keyword">import</a> <a id="23284" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="23323" class="Keyword">open</a> <a id="23328" class="Keyword">import</a> <a id="23335" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="23376" class="Keyword">open</a> <a id="23381" class="Keyword">import</a> <a id="23388" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="23432" class="Keyword">open</a> <a id="23437" class="Keyword">import</a> <a id="23444" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="23481" class="Keyword">open</a> <a id="23486" class="Keyword">import</a> <a id="23493" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="23515" class="Keyword">open</a> <a id="23520" class="Keyword">import</a> <a id="23527" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23557" class="Keyword">open</a> <a id="23562" class="Keyword">import</a> <a id="23569" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="23608" class="Keyword">open</a> <a id="23613" class="Keyword">import</a> <a id="23620" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="23658" class="Keyword">open</a> <a id="23663" class="Keyword">import</a> <a id="23670" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="23728" class="Keyword">open</a> <a id="23733" class="Keyword">import</a> <a id="23740" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="23771" class="Keyword">open</a> <a id="23776" class="Keyword">import</a> <a id="23783" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="23810" class="Keyword">open</a> <a id="23815" class="Keyword">import</a> <a id="23822" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="23880" class="Keyword">open</a> <a id="23885" class="Keyword">import</a> <a id="23892" href="group-theory.html" class="Module">group-theory</a>
<a id="23905" class="Keyword">open</a> <a id="23910" class="Keyword">import</a> <a id="23917" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="23945" class="Keyword">open</a> <a id="23950" class="Keyword">import</a> <a id="23957" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="23988" class="Keyword">open</a> <a id="23993" class="Keyword">import</a> <a id="24000" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="24036" class="Keyword">open</a> <a id="24041" class="Keyword">import</a> <a id="24048" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="24099" class="Keyword">open</a> <a id="24104" class="Keyword">import</a> <a id="24111" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="24144" class="Keyword">open</a> <a id="24149" class="Keyword">import</a> <a id="24156" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="24203" class="Keyword">open</a> <a id="24208" class="Keyword">import</a> <a id="24215" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="24254" class="Keyword">open</a> <a id="24259" class="Keyword">import</a> <a id="24266" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="24306" class="Keyword">open</a> <a id="24311" class="Keyword">import</a> <a id="24318" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="24361" class="Keyword">open</a> <a id="24366" class="Keyword">import</a> <a id="24373" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="24405" class="Keyword">open</a> <a id="24410" class="Keyword">import</a> <a id="24417" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="24453" class="Keyword">open</a> <a id="24458" class="Keyword">import</a> <a id="24465" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="24494" class="Keyword">open</a> <a id="24499" class="Keyword">import</a> <a id="24506" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="24539" class="Keyword">open</a> <a id="24544" class="Keyword">import</a> <a id="24551" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="24587" class="Keyword">open</a> <a id="24592" class="Keyword">import</a> <a id="24599" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="24628" class="Keyword">open</a> <a id="24633" class="Keyword">import</a> <a id="24640" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="24672" class="Keyword">open</a> <a id="24677" class="Keyword">import</a> <a id="24684" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="24709" class="Keyword">open</a> <a id="24714" class="Keyword">import</a> <a id="24721" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="24752" class="Keyword">open</a> <a id="24757" class="Keyword">import</a> <a id="24764" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="24811" class="Keyword">open</a> <a id="24816" class="Keyword">import</a> <a id="24823" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="24856" class="Keyword">open</a> <a id="24861" class="Keyword">import</a> <a id="24868" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="24908" class="Keyword">open</a> <a id="24913" class="Keyword">import</a> <a id="24920" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="24957" class="Keyword">open</a> <a id="24962" class="Keyword">import</a> <a id="24969" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="25005" class="Keyword">open</a> <a id="25010" class="Keyword">import</a> <a id="25017" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="25049" class="Keyword">open</a> <a id="25054" class="Keyword">import</a> <a id="25061" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="25088" class="Keyword">open</a> <a id="25093" class="Keyword">import</a> <a id="25100" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="25120" class="Keyword">open</a> <a id="25125" class="Keyword">import</a> <a id="25132" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="25159" class="Keyword">open</a> <a id="25164" class="Keyword">import</a> <a id="25171" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="25213" class="Keyword">open</a> <a id="25218" class="Keyword">import</a> <a id="25225" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="25272" class="Keyword">open</a> <a id="25277" class="Keyword">import</a> <a id="25284" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="25325" class="Keyword">open</a> <a id="25330" class="Keyword">import</a> <a id="25337" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="25371" class="Keyword">open</a> <a id="25376" class="Keyword">import</a> <a id="25383" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="25418" class="Keyword">open</a> <a id="25423" class="Keyword">import</a> <a id="25430" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="25468" class="Keyword">open</a> <a id="25473" class="Keyword">import</a> <a id="25480" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="25512" class="Keyword">open</a> <a id="25517" class="Keyword">import</a> <a id="25524" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="25565" class="Keyword">open</a> <a id="25570" class="Keyword">import</a> <a id="25577" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="25618" class="Keyword">open</a> <a id="25623" class="Keyword">import</a> <a id="25630" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="25670" class="Keyword">open</a> <a id="25675" class="Keyword">import</a> <a id="25682" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="25715" class="Keyword">open</a> <a id="25720" class="Keyword">import</a> <a id="25727" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="25764" class="Keyword">open</a> <a id="25769" class="Keyword">import</a> <a id="25776" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="25806" class="Keyword">open</a> <a id="25811" class="Keyword">import</a> <a id="25818" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="25863" class="Keyword">open</a> <a id="25868" class="Keyword">import</a> <a id="25875" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="25903" class="Keyword">open</a> <a id="25908" class="Keyword">import</a> <a id="25915" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="25936" class="Keyword">open</a> <a id="25941" class="Keyword">import</a> <a id="25948" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="25982" class="Keyword">open</a> <a id="25987" class="Keyword">import</a> <a id="25994" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="26028" class="Keyword">open</a> <a id="26033" class="Keyword">import</a> <a id="26040" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="26075" class="Keyword">open</a> <a id="26080" class="Keyword">import</a> <a id="26087" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="26129" class="Keyword">open</a> <a id="26134" class="Keyword">import</a> <a id="26141" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="26176" class="Keyword">open</a> <a id="26181" class="Keyword">import</a> <a id="26188" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="26227" class="Keyword">open</a> <a id="26232" class="Keyword">import</a> <a id="26239" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="26276" class="Keyword">open</a> <a id="26281" class="Keyword">import</a> <a id="26288" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="26312" class="Keyword">open</a> <a id="26317" class="Keyword">import</a> <a id="26324" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="26349" class="Keyword">open</a> <a id="26354" class="Keyword">import</a> <a id="26361" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="26392" class="Keyword">open</a> <a id="26397" class="Keyword">import</a> <a id="26404" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="26455" class="Keyword">open</a> <a id="26460" class="Keyword">import</a> <a id="26467" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="26490" class="Keyword">open</a> <a id="26495" class="Keyword">import</a> <a id="26502" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="26550" class="Keyword">open</a> <a id="26555" class="Keyword">import</a> <a id="26562" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="26592" class="Keyword">open</a> <a id="26597" class="Keyword">import</a> <a id="26604" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="26674" class="Keyword">open</a> <a id="26679" class="Keyword">import</a> <a id="26686" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="26701" class="Keyword">open</a> <a id="26706" class="Keyword">import</a> <a id="26713" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="26746" class="Keyword">open</a> <a id="26751" class="Keyword">import</a> <a id="26758" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="26790" class="Keyword">open</a> <a id="26795" class="Keyword">import</a> <a id="26802" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="26844" class="Keyword">open</a> <a id="26849" class="Keyword">import</a> <a id="26856" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="26894" class="Keyword">open</a> <a id="26899" class="Keyword">import</a> <a id="26906" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="26943" class="Keyword">open</a> <a id="26948" class="Keyword">import</a> <a id="26955" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="26988" class="Keyword">open</a> <a id="26993" class="Keyword">import</a> <a id="27000" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="27024" class="Keyword">open</a> <a id="27029" class="Keyword">import</a> <a id="27036" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="27075" class="Keyword">open</a> <a id="27080" class="Keyword">import</a> <a id="27087" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="27133" class="Keyword">open</a> <a id="27138" class="Keyword">import</a> <a id="27145" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="27190" class="Keyword">open</a> <a id="27195" class="Keyword">import</a> <a id="27202" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="27240" class="Keyword">open</a> <a id="27245" class="Keyword">import</a> <a id="27252" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="27284" class="Keyword">open</a> <a id="27289" class="Keyword">import</a> <a id="27296" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="27349" class="Keyword">open</a> <a id="27354" class="Keyword">import</a> <a id="27361" href="order-theory.html" class="Module">order-theory</a>
<a id="27374" class="Keyword">open</a> <a id="27379" class="Keyword">import</a> <a id="27386" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="27413" class="Keyword">open</a> <a id="27418" class="Keyword">import</a> <a id="27425" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="27455" class="Keyword">open</a> <a id="27460" class="Keyword">import</a> <a id="27467" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="27500" class="Keyword">open</a> <a id="27505" class="Keyword">import</a> <a id="27512" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="27548" class="Keyword">open</a> <a id="27553" class="Keyword">import</a> <a id="27560" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="27595" class="Keyword">open</a> <a id="27600" class="Keyword">import</a> <a id="27607" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="27634" class="Keyword">open</a> <a id="27639" class="Keyword">import</a> <a id="27646" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="27676" class="Keyword">open</a> <a id="27681" class="Keyword">import</a> <a id="27688" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="27724" class="Keyword">open</a> <a id="27729" class="Keyword">import</a> <a id="27736" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="27778" class="Keyword">open</a> <a id="27783" class="Keyword">import</a> <a id="27790" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="27822" class="Keyword">open</a> <a id="27827" class="Keyword">import</a> <a id="27834" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="27865" class="Keyword">open</a> <a id="27870" class="Keyword">import</a> <a id="27877" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="27903" class="Keyword">open</a> <a id="27908" class="Keyword">import</a> <a id="27915" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="27944" class="Keyword">open</a> <a id="27949" class="Keyword">import</a> <a id="27956" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="27993" class="Keyword">open</a> <a id="27998" class="Keyword">import</a> <a id="28005" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="28045" class="Keyword">open</a> <a id="28050" class="Keyword">import</a> <a id="28057" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="28079" class="Keyword">open</a> <a id="28084" class="Keyword">import</a> <a id="28091" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="28126" class="Keyword">open</a> <a id="28131" class="Keyword">import</a> <a id="28138" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="28176" class="Keyword">open</a> <a id="28181" class="Keyword">import</a> <a id="28188" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="28227" class="Keyword">open</a> <a id="28232" class="Keyword">import</a> <a id="28239" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="28274" class="Keyword">open</a> <a id="28279" class="Keyword">import</a> <a id="28286" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="28321" class="Keyword">open</a> <a id="28326" class="Keyword">import</a> <a id="28333" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="28371" class="Keyword">open</a> <a id="28376" class="Keyword">import</a> <a id="28383" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="28414" class="Keyword">open</a> <a id="28419" class="Keyword">import</a> <a id="28426" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="28468" class="Keyword">open</a> <a id="28473" class="Keyword">import</a> <a id="28480" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="28525" class="Keyword">open</a> <a id="28530" class="Keyword">import</a> <a id="28537" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="28570" class="Keyword">open</a> <a id="28575" class="Keyword">import</a> <a id="28582" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="28602" class="Keyword">open</a> <a id="28607" class="Keyword">import</a> <a id="28614" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="28637" class="Keyword">open</a> <a id="28642" class="Keyword">import</a> <a id="28649" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="28672" class="Keyword">open</a> <a id="28677" class="Keyword">import</a> <a id="28684" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="28710" class="Keyword">open</a> <a id="28715" class="Keyword">import</a> <a id="28722" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="28748" class="Keyword">open</a> <a id="28753" class="Keyword">import</a> <a id="28760" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="28816" class="Keyword">open</a> <a id="28821" class="Keyword">import</a> <a id="28828" href="polytopes.html" class="Module">polytopes</a>
<a id="28838" class="Keyword">open</a> <a id="28843" class="Keyword">import</a> <a id="28850" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="28908" class="Keyword">open</a> <a id="28913" class="Keyword">import</a> <a id="28920" href="ring-theory.html" class="Module">ring-theory</a>
<a id="28932" class="Keyword">open</a> <a id="28937" class="Keyword">import</a> <a id="28944" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="28981" class="Keyword">open</a> <a id="28986" class="Keyword">import</a> <a id="28993" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="29020" class="Keyword">open</a> <a id="29025" class="Keyword">import</a> <a id="29032" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="29064" class="Keyword">open</a> <a id="29069" class="Keyword">import</a> <a id="29076" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="29122" class="Keyword">open</a> <a id="29127" class="Keyword">import</a> <a id="29134" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="29159" class="Keyword">open</a> <a id="29164" class="Keyword">import</a> <a id="29171" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="29214" class="Keyword">open</a> <a id="29219" class="Keyword">import</a> <a id="29226" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="29264" class="Keyword">open</a> <a id="29269" class="Keyword">import</a> <a id="29276" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="29307" class="Keyword">open</a> <a id="29312" class="Keyword">import</a> <a id="29319" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="29343" class="Keyword">open</a> <a id="29348" class="Keyword">import</a> <a id="29355" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="29387" class="Keyword">open</a> <a id="29392" class="Keyword">import</a> <a id="29399" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="29425" class="Keyword">open</a> <a id="29430" class="Keyword">import</a> <a id="29437" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="29466" class="Keyword">open</a> <a id="29471" class="Keyword">import</a> <a id="29478" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="29515" class="Keyword">open</a> <a id="29520" class="Keyword">import</a> <a id="29527" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="29556" class="Keyword">open</a> <a id="29561" class="Keyword">import</a> <a id="29568" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="29595" class="Keyword">open</a> <a id="29600" class="Keyword">import</a> <a id="29607" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="29644" class="Keyword">open</a> <a id="29649" class="Keyword">import</a> <a id="29656" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="29683" class="Keyword">open</a> <a id="29688" class="Keyword">import</a> <a id="29695" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="29728" class="Keyword">open</a> <a id="29733" class="Keyword">import</a> <a id="29740" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="29758" class="Keyword">open</a> <a id="29763" class="Keyword">import</a> <a id="29770" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="29824" class="Keyword">open</a> <a id="29829" class="Keyword">import</a> <a id="29836" href="set-theory.html" class="Module">set-theory</a>
<a id="29847" class="Keyword">open</a> <a id="29852" class="Keyword">import</a> <a id="29859" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="29885" class="Keyword">open</a> <a id="29890" class="Keyword">import</a> <a id="29897" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="29959" class="Keyword">open</a> <a id="29964" class="Keyword">import</a> <a id="29971" href="structured-types.html" class="Module">structured-types</a>
<a id="29988" class="Keyword">open</a> <a id="29993" class="Keyword">import</a> <a id="30000" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="30035" class="Keyword">open</a> <a id="30040" class="Keyword">import</a> <a id="30047" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="30091" class="Keyword">open</a> <a id="30096" class="Keyword">import</a> <a id="30103" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="30167" class="Keyword">open</a> <a id="30172" class="Keyword">import</a> <a id="30179" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="30225" class="Keyword">open</a> <a id="30230" class="Keyword">import</a> <a id="30237" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="30261" class="Keyword">open</a> <a id="30266" class="Keyword">import</a> <a id="30273" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="30342" class="Keyword">open</a> <a id="30347" class="Keyword">import</a> <a id="30354" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="30399" class="Keyword">open</a> <a id="30404" class="Keyword">import</a> <a id="30411" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="30445" class="Keyword">open</a> <a id="30450" class="Keyword">import</a> <a id="30457" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="30518" class="Keyword">open</a> <a id="30523" class="Keyword">import</a> <a id="30530" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="30575" class="Keyword">open</a> <a id="30580" class="Keyword">import</a> <a id="30587" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="30625" class="Keyword">open</a> <a id="30630" class="Keyword">import</a> <a id="30637" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="30680" class="Keyword">open</a> <a id="30685" class="Keyword">import</a> <a id="30692" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="30728" class="Keyword">open</a> <a id="30733" class="Keyword">import</a> <a id="30740" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="30770" class="Keyword">open</a> <a id="30775" class="Keyword">import</a> <a id="30782" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="30813" class="Keyword">open</a> <a id="30818" class="Keyword">import</a> <a id="30825" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="30884" class="Keyword">open</a> <a id="30889" class="Keyword">import</a> <a id="30896" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="30947" class="Keyword">open</a> <a id="30952" class="Keyword">import</a> <a id="30959" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="31010" class="Keyword">open</a> <a id="31015" class="Keyword">import</a> <a id="31022" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="31077" class="Keyword">open</a> <a id="31082" class="Keyword">import</a> <a id="31089" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="31118" class="Keyword">open</a> <a id="31123" class="Keyword">import</a> <a id="31130" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="31158" class="Keyword">open</a> <a id="31163" class="Keyword">import</a> <a id="31170" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="31200" class="Keyword">open</a> <a id="31205" class="Keyword">import</a> <a id="31212" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="31246" class="Keyword">open</a> <a id="31251" class="Keyword">import</a> <a id="31258" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="31334" class="Keyword">open</a> <a id="31339" class="Keyword">import</a> <a id="31346" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="31372" class="Keyword">open</a> <a id="31377" class="Keyword">import</a> <a id="31384" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="31423" class="Keyword">open</a> <a id="31428" class="Keyword">import</a> <a id="31435" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="31473" class="Keyword">open</a> <a id="31478" class="Keyword">import</a> <a id="31485" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="31531" class="Keyword">open</a> <a id="31536" class="Keyword">import</a> <a id="31543" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="31580" class="Keyword">open</a> <a id="31585" class="Keyword">import</a> <a id="31592" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="31632" class="Keyword">open</a> <a id="31637" class="Keyword">import</a> <a id="31644" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="31683" class="Keyword">open</a> <a id="31688" class="Keyword">import</a> <a id="31695" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="31728" class="Keyword">open</a> <a id="31733" class="Keyword">import</a> <a id="31740" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="31775" class="Keyword">open</a> <a id="31780" class="Keyword">import</a> <a id="31787" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="31832" class="Keyword">open</a> <a id="31837" class="Keyword">import</a> <a id="31844" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="31896" class="Keyword">open</a> <a id="31901" class="Keyword">import</a> <a id="31908" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="31961" class="Keyword">open</a> <a id="31966" class="Keyword">import</a> <a id="31973" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="32021" class="Keyword">open</a> <a id="32026" class="Keyword">import</a> <a id="32033" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="32073" class="Keyword">open</a> <a id="32078" class="Keyword">import</a> <a id="32085" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="32132" class="Keyword">open</a> <a id="32137" class="Keyword">import</a> <a id="32144" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="32185" class="Keyword">open</a> <a id="32190" class="Keyword">import</a> <a id="32197" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="32235" class="Keyword">open</a> <a id="32240" class="Keyword">import</a> <a id="32247" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="32295" class="Keyword">open</a> <a id="32300" class="Keyword">import</a> <a id="32307" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="32352" class="Keyword">open</a> <a id="32357" class="Keyword">import</a> <a id="32364" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="32413" class="Keyword">open</a> <a id="32418" class="Keyword">import</a> <a id="32425" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="32502" class="Keyword">open</a> <a id="32507" class="Keyword">import</a> <a id="32514" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="32566" class="Keyword">open</a> <a id="32571" class="Keyword">import</a> <a id="32578" href="type-theories.html" class="Module">type-theories</a>
<a id="32592" class="Keyword">open</a> <a id="32597" class="Keyword">import</a> <a id="32604" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="32646" class="Keyword">open</a> <a id="32651" class="Keyword">import</a> <a id="32658" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="32696" class="Keyword">open</a> <a id="32701" class="Keyword">import</a> <a id="32708" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="32754" class="Keyword">open</a> <a id="32759" class="Keyword">import</a> <a id="32766" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="32813" class="Keyword">open</a> <a id="32818" class="Keyword">import</a> <a id="32825" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="32860" class="Keyword">open</a> <a id="32865" class="Keyword">import</a> <a id="32872" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="32950" class="Keyword">open</a> <a id="32955" class="Keyword">import</a> <a id="32962" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="32986" class="Keyword">open</a> <a id="32991" class="Keyword">import</a> <a id="32998" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="33051" class="Keyword">open</a> <a id="33056" class="Keyword">import</a> <a id="33063" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="33106" class="Keyword">open</a> <a id="33111" class="Keyword">import</a> <a id="33118" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="33158" class="Keyword">open</a> <a id="33163" class="Keyword">import</a> <a id="33170" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="33209" class="Keyword">open</a> <a id="33214" class="Keyword">import</a> <a id="33221" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="33255" class="Keyword">open</a> <a id="33260" class="Keyword">import</a> <a id="33267" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="33315" class="Keyword">open</a> <a id="33320" class="Keyword">import</a> <a id="33327" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="33378" class="Keyword">open</a> <a id="33383" class="Keyword">import</a> <a id="33390" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="33437" class="Keyword">open</a> <a id="33442" class="Keyword">import</a> <a id="33449" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="33501" class="Keyword">open</a> <a id="33506" class="Keyword">import</a> <a id="33513" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="33557" class="Keyword">open</a> <a id="33562" class="Keyword">import</a> <a id="33569" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="33609" class="Keyword">open</a> <a id="33614" class="Keyword">import</a> <a id="33621" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="33664" class="Keyword">open</a> <a id="33669" class="Keyword">import</a> <a id="33676" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="33728" class="Keyword">open</a> <a id="33733" class="Keyword">import</a> <a id="33740" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="33794" class="Keyword">open</a> <a id="33799" class="Keyword">import</a> <a id="33806" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="33854" class="Keyword">open</a> <a id="33859" class="Keyword">import</a> <a id="33866" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="33905" class="Keyword">open</a> <a id="33910" class="Keyword">import</a> <a id="33917" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="33950" class="Keyword">open</a> <a id="33955" class="Keyword">import</a> <a id="33962" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="33992" class="Keyword">open</a> <a id="33997" class="Keyword">import</a> <a id="34004" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="34055" class="Keyword">open</a> <a id="34060" class="Keyword">import</a> <a id="34067" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="34108" class="Keyword">open</a> <a id="34113" class="Keyword">import</a> <a id="34120" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="34157" class="Keyword">open</a> <a id="34162" class="Keyword">import</a> <a id="34169" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="34228" class="Keyword">open</a> <a id="34233" class="Keyword">import</a> <a id="34240" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="34295" class="Keyword">open</a> <a id="34300" class="Keyword">import</a> <a id="34307" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="34354" class="Keyword">open</a> <a id="34359" class="Keyword">import</a> <a id="34366" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="34409" class="Keyword">open</a> <a id="34414" class="Keyword">import</a> <a id="34421" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="34466" class="Keyword">open</a> <a id="34471" class="Keyword">import</a> <a id="34478" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="34527" class="Keyword">open</a> <a id="34532" class="Keyword">import</a> <a id="34539" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="34590" class="Keyword">open</a> <a id="34595" class="Keyword">import</a> <a id="34602" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="34646" class="Keyword">open</a> <a id="34651" class="Keyword">import</a> <a id="34658" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="34736" class="Keyword">open</a> <a id="34741" class="Keyword">import</a> <a id="34748" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="34788" class="Keyword">open</a> <a id="34793" class="Keyword">import</a> <a id="34800" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="34857" class="Keyword">open</a> <a id="34862" class="Keyword">import</a> <a id="34869" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="34904" class="Keyword">open</a> <a id="34909" class="Keyword">import</a> <a id="34916" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="34962" class="Keyword">open</a> <a id="34967" class="Keyword">import</a> <a id="34974" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="35029" class="Keyword">open</a> <a id="35034" class="Keyword">import</a> <a id="35041" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="35084" class="Keyword">open</a> <a id="35089" class="Keyword">import</a> <a id="35096" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="35141" class="Keyword">open</a> <a id="35146" class="Keyword">import</a> <a id="35153" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="35212" class="Keyword">open</a> <a id="35217" class="Keyword">import</a> <a id="35224" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="35261" class="Keyword">open</a> <a id="35266" class="Keyword">import</a> <a id="35273" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="35315" class="Keyword">open</a> <a id="35320" class="Keyword">import</a> <a id="35327" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="35368" class="Keyword">open</a> <a id="35373" class="Keyword">import</a> <a id="35380" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="35419" class="Keyword">open</a> <a id="35424" class="Keyword">import</a> <a id="35431" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="35469" class="Keyword">open</a> <a id="35474" class="Keyword">import</a> <a id="35481" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="35533" class="Keyword">open</a> <a id="35538" class="Keyword">import</a> <a id="35545" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="35590" class="Keyword">open</a> <a id="35595" class="Keyword">import</a> <a id="35602" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="35641" class="Keyword">open</a> <a id="35646" class="Keyword">import</a> <a id="35653" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="35690" class="Keyword">open</a> <a id="35695" class="Keyword">import</a> <a id="35702" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="35751" class="Keyword">open</a> <a id="35756" class="Keyword">import</a> <a id="35763" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="35802" class="Keyword">open</a> <a id="35807" class="Keyword">import</a> <a id="35814" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="35852" class="Keyword">open</a> <a id="35857" class="Keyword">import</a> <a id="35864" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="35919" class="Keyword">open</a> <a id="35924" class="Keyword">import</a> <a id="35931" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="35970" class="Keyword">open</a> <a id="35975" class="Keyword">import</a> <a id="35982" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="36030" class="Keyword">open</a> <a id="36035" class="Keyword">import</a> <a id="36042" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="36089" class="Keyword">open</a> <a id="36094" class="Keyword">import</a> <a id="36101" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="36139" class="Keyword">open</a> <a id="36144" class="Keyword">import</a> <a id="36151" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="36181" class="Keyword">open</a> <a id="36186" class="Keyword">import</a> <a id="36193" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="36250" class="Keyword">open</a> <a id="36255" class="Keyword">import</a> <a id="36262" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="36316" class="Keyword">open</a> <a id="36321" class="Keyword">import</a> <a id="36328" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="36358" class="Keyword">open</a> <a id="36363" class="Keyword">import</a> <a id="36370" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="36419" class="Keyword">open</a> <a id="36424" class="Keyword">import</a> <a id="36431" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="36473" class="Keyword">open</a> <a id="36478" class="Keyword">import</a> <a id="36485" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="36519" class="Keyword">open</a> <a id="36524" class="Keyword">import</a> <a id="36531" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="36594" class="Keyword">open</a> <a id="36599" class="Keyword">import</a> <a id="36606" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="36649" class="Keyword">open</a> <a id="36654" class="Keyword">import</a> <a id="36661" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="36696" class="Keyword">open</a> <a id="36701" class="Keyword">import</a> <a id="36708" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="36743" class="Keyword">open</a> <a id="36748" class="Keyword">import</a> <a id="36755" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="36795" class="Keyword">open</a> <a id="36800" class="Keyword">import</a> <a id="36807" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="36852" class="Keyword">open</a> <a id="36857" class="Keyword">import</a> <a id="36864" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="36905" class="Keyword">open</a> <a id="36910" class="Keyword">import</a> <a id="36917" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="36971" class="Keyword">open</a> <a id="36976" class="Keyword">import</a> <a id="36983" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="37033" class="Keyword">open</a> <a id="37038" class="Keyword">import</a> <a id="37045" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="37083" class="Keyword">open</a> <a id="37088" class="Keyword">import</a> <a id="37095" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="37144" class="Keyword">open</a> <a id="37149" class="Keyword">import</a> <a id="37156" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="37203" class="Keyword">open</a> <a id="37208" class="Keyword">import</a> <a id="37215" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="37278" class="Keyword">open</a> <a id="37283" class="Keyword">import</a> <a id="37290" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="37322" class="Keyword">open</a> <a id="37327" class="Keyword">import</a> <a id="37334" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="37387" class="Keyword">open</a> <a id="37392" class="Keyword">import</a> <a id="37399" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="37445" class="Keyword">open</a> <a id="37450" class="Keyword">import</a> <a id="37457" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="37503" class="Keyword">open</a> <a id="37508" class="Keyword">import</a> <a id="37515" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="37563" class="Keyword">open</a> <a id="37568" class="Keyword">import</a> <a id="37575" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="37615" class="Keyword">open</a> <a id="37620" class="Keyword">import</a> <a id="37627" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="37672" class="Keyword">open</a> <a id="37677" class="Keyword">import</a> <a id="37684" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="37749" class="Keyword">open</a> <a id="37754" class="Keyword">import</a> <a id="37761" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="37806" class="Keyword">open</a> <a id="37811" class="Keyword">import</a> <a id="37818" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="37865" class="Keyword">open</a> <a id="37870" class="Keyword">import</a> <a id="37877" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="37930" class="Keyword">open</a> <a id="37935" class="Keyword">import</a> <a id="37942" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>