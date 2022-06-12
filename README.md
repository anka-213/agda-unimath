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
<a id="5121" class="Keyword">open</a> <a id="5126" class="Keyword">import</a> <a id="5133" href="commutative-algebra.isomorphisms-commutative-rings.html" class="Module">commutative-algebra.isomorphisms-commutative-rings</a>
<a id="5184" class="Keyword">open</a> <a id="5189" class="Keyword">import</a> <a id="5196" href="commutative-algebra.prime-ideals-commutative-rings.html" class="Module">commutative-algebra.prime-ideals-commutative-rings</a>
<a id="5247" class="Keyword">open</a> <a id="5252" class="Keyword">import</a> <a id="5259" href="commutative-algebra.zarisky-topology.html" class="Module">commutative-algebra.zarisky-topology</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="5338" class="Keyword">open</a> <a id="5343" class="Keyword">import</a> <a id="5350" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5375" class="Keyword">open</a> <a id="5380" class="Keyword">import</a> <a id="5387" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5436" class="Keyword">open</a> <a id="5441" class="Keyword">import</a> <a id="5448" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5491" class="Keyword">open</a> <a id="5496" class="Keyword">import</a> <a id="5503" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5553" class="Keyword">open</a> <a id="5558" class="Keyword">import</a> <a id="5565" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5611" class="Keyword">open</a> <a id="5616" class="Keyword">import</a> <a id="5623" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5670" class="Keyword">open</a> <a id="5675" class="Keyword">import</a> <a id="5682" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5741" class="Keyword">open</a> <a id="5746" class="Keyword">import</a> <a id="5753" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="5794" class="Keyword">open</a> <a id="5799" class="Keyword">import</a> <a id="5806" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="5849" class="Keyword">open</a> <a id="5854" class="Keyword">import</a> <a id="5861" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="5905" class="Keyword">open</a> <a id="5910" class="Keyword">import</a> <a id="5917" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="5962" class="Keyword">open</a> <a id="5967" class="Keyword">import</a> <a id="5974" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="6026" class="Keyword">open</a> <a id="6031" class="Keyword">import</a> <a id="6038" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="6098" class="Keyword">open</a> <a id="6103" class="Keyword">import</a> <a id="6110" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="6151" class="Keyword">open</a> <a id="6156" class="Keyword">import</a> <a id="6163" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6208" class="Keyword">open</a> <a id="6213" class="Keyword">import</a> <a id="6220" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6267" class="Keyword">open</a> <a id="6272" class="Keyword">import</a> <a id="6279" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6322" class="Keyword">open</a> <a id="6327" class="Keyword">import</a> <a id="6334" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6384" class="Keyword">open</a> <a id="6389" class="Keyword">import</a> <a id="6396" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6443" class="Keyword">open</a> <a id="6448" class="Keyword">import</a> <a id="6455" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6512" class="Keyword">open</a> <a id="6517" class="Keyword">import</a> <a id="6524" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6578" class="Keyword">open</a> <a id="6583" class="Keyword">import</a> <a id="6590" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6650" class="Keyword">open</a> <a id="6655" class="Keyword">import</a> <a id="6662" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6705" class="Keyword">open</a> <a id="6710" class="Keyword">import</a> <a id="6717" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="6767" class="Keyword">open</a> <a id="6772" class="Keyword">import</a> <a id="6779" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="6839" class="Keyword">open</a> <a id="6844" class="Keyword">import</a> <a id="6851" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="6900" class="Keyword">open</a> <a id="6905" class="Keyword">import</a> <a id="6912" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="6968" class="Keyword">open</a> <a id="6973" class="Keyword">import</a> <a id="6980" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="7016" class="Keyword">open</a> <a id="7021" class="Keyword">import</a> <a id="7028" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="7072" class="Keyword">open</a> <a id="7077" class="Keyword">import</a> <a id="7084" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="7128" class="Keyword">open</a> <a id="7133" class="Keyword">import</a> <a id="7140" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7190" class="Keyword">open</a> <a id="7195" class="Keyword">import</a> <a id="7202" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7248" class="Keyword">open</a> <a id="7253" class="Keyword">import</a> <a id="7260" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7295" class="Keyword">open</a> <a id="7300" class="Keyword">import</a> <a id="7307" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7352" class="Keyword">open</a> <a id="7357" class="Keyword">import</a> <a id="7364" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7422" class="Keyword">open</a> <a id="7427" class="Keyword">import</a> <a id="7434" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7499" class="Keyword">open</a> <a id="7504" class="Keyword">import</a> <a id="7511" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7554" class="Keyword">open</a> <a id="7559" class="Keyword">import</a> <a id="7566" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7620" class="Keyword">open</a> <a id="7625" class="Keyword">import</a> <a id="7632" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7677" class="Keyword">open</a> <a id="7682" class="Keyword">import</a> <a id="7689" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7741" class="Keyword">open</a> <a id="7746" class="Keyword">import</a> <a id="7753" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7811" class="Keyword">open</a> <a id="7816" class="Keyword">import</a> <a id="7823" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="7869" class="Keyword">open</a> <a id="7874" class="Keyword">import</a> <a id="7881" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="7925" class="Keyword">open</a> <a id="7930" class="Keyword">import</a> <a id="7937" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="7971" class="Keyword">open</a> <a id="7976" class="Keyword">import</a> <a id="7983" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="8037" class="Keyword">open</a> <a id="8042" class="Keyword">import</a> <a id="8049" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="8098" class="Keyword">open</a> <a id="8103" class="Keyword">import</a> <a id="8110" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="8151" class="Keyword">open</a> <a id="8156" class="Keyword">import</a> <a id="8163" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8212" class="Keyword">open</a> <a id="8217" class="Keyword">import</a> <a id="8224" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8290" class="Keyword">open</a> <a id="8295" class="Keyword">import</a> <a id="8302" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8346" class="Keyword">open</a> <a id="8351" class="Keyword">import</a> <a id="8358" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8407" class="Keyword">open</a> <a id="8412" class="Keyword">import</a> <a id="8419" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8475" class="Keyword">open</a> <a id="8480" class="Keyword">import</a> <a id="8487" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8528" class="Keyword">open</a> <a id="8533" class="Keyword">import</a> <a id="8540" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8589" class="Keyword">open</a> <a id="8594" class="Keyword">import</a> <a id="8601" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8660" class="Keyword">open</a> <a id="8665" class="Keyword">import</a> <a id="8672" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8711" class="Keyword">open</a> <a id="8716" class="Keyword">import</a> <a id="8723" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8776" class="Keyword">open</a> <a id="8781" class="Keyword">import</a> <a id="8788" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="8845" class="Keyword">open</a> <a id="8850" class="Keyword">import</a> <a id="8857" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="8899" class="Keyword">open</a> <a id="8904" class="Keyword">import</a> <a id="8911" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="8962" class="Keyword">open</a> <a id="8967" class="Keyword">import</a> <a id="8974" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9032" class="Keyword">open</a> <a id="9037" class="Keyword">import</a> <a id="9044" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9108" class="Keyword">open</a> <a id="9113" class="Keyword">import</a> <a id="9120" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9173" class="Keyword">open</a> <a id="9178" class="Keyword">import</a> <a id="9185" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9238" class="Keyword">open</a> <a id="9243" class="Keyword">import</a> <a id="9250" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9311" class="Keyword">open</a> <a id="9316" class="Keyword">import</a> <a id="9323" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9381" class="Keyword">open</a> <a id="9386" class="Keyword">import</a> <a id="9393" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9442" class="Keyword">open</a> <a id="9447" class="Keyword">import</a> <a id="9454" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9497" class="Keyword">open</a> <a id="9502" class="Keyword">import</a> <a id="9509" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9553" class="Keyword">open</a> <a id="9558" class="Keyword">import</a> <a id="9565" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9612" class="Keyword">open</a> <a id="9617" class="Keyword">import</a> <a id="9624" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9685" class="Keyword">open</a> <a id="9690" class="Keyword">import</a> <a id="9697" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9760" class="Keyword">open</a> <a id="9765" class="Keyword">import</a> <a id="9772" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="9832" class="Keyword">open</a> <a id="9837" class="Keyword">import</a> <a id="9844" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="9898" class="Keyword">open</a> <a id="9903" class="Keyword">import</a> <a id="9910" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="9975" class="Keyword">open</a> <a id="9980" class="Keyword">import</a> <a id="9987" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10095" class="Keyword">open</a> <a id="10100" class="Keyword">import</a> <a id="10107" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10127" class="Keyword">open</a> <a id="10132" class="Keyword">import</a> <a id="10139" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10185" class="Keyword">open</a> <a id="10190" class="Keyword">import</a> <a id="10197" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10253" class="Keyword">open</a> <a id="10258" class="Keyword">import</a> <a id="10265" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10311" class="Keyword">open</a> <a id="10316" class="Keyword">import</a> <a id="10323" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10357" class="Keyword">open</a> <a id="10362" class="Keyword">import</a> <a id="10369" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10404" class="Keyword">open</a> <a id="10409" class="Keyword">import</a> <a id="10416" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10454" class="Keyword">open</a> <a id="10459" class="Keyword">import</a> <a id="10466" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10504" class="Keyword">open</a> <a id="10509" class="Keyword">import</a> <a id="10516" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10556" class="Keyword">open</a> <a id="10561" class="Keyword">import</a> <a id="10568" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10601" class="Keyword">open</a> <a id="10606" class="Keyword">import</a> <a id="10613" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10651" class="Keyword">open</a> <a id="10656" class="Keyword">import</a> <a id="10663" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10726" class="Keyword">open</a> <a id="10731" class="Keyword">import</a> <a id="10738" href="foundation.html" class="Module">foundation</a>
<a id="10749" class="Keyword">open</a> <a id="10754" class="Keyword">import</a> <a id="10761" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10779" class="Keyword">open</a> <a id="10784" class="Keyword">import</a> <a id="10791" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10810" class="Keyword">open</a> <a id="10815" class="Keyword">import</a> <a id="10822" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10841" class="Keyword">open</a> <a id="10846" class="Keyword">import</a> <a id="10853" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="10897" class="Keyword">open</a> <a id="10902" class="Keyword">import</a> <a id="10909" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="10934" class="Keyword">open</a> <a id="10939" class="Keyword">import</a> <a id="10946" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="10973" class="Keyword">open</a> <a id="10978" class="Keyword">import</a> <a id="10985" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11002" class="Keyword">open</a> <a id="11007" class="Keyword">import</a> <a id="11014" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11043" class="Keyword">open</a> <a id="11048" class="Keyword">import</a> <a id="11055" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11111" class="Keyword">open</a> <a id="11116" class="Keyword">import</a> <a id="11123" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11154" class="Keyword">open</a> <a id="11159" class="Keyword">import</a> <a id="11166" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11220" class="Keyword">open</a> <a id="11225" class="Keyword">import</a> <a id="11232" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11260" class="Keyword">open</a> <a id="11265" class="Keyword">import</a> <a id="11272" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11302" class="Keyword">open</a> <a id="11307" class="Keyword">import</a> <a id="11314" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11334" class="Keyword">open</a> <a id="11339" class="Keyword">import</a> <a id="11346" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11391" class="Keyword">open</a> <a id="11396" class="Keyword">import</a> <a id="11403" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11440" class="Keyword">open</a> <a id="11445" class="Keyword">import</a> <a id="11452" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11487" class="Keyword">open</a> <a id="11492" class="Keyword">import</a> <a id="11499" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11557" class="Keyword">open</a> <a id="11562" class="Keyword">import</a> <a id="11569" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11607" class="Keyword">open</a> <a id="11612" class="Keyword">import</a> <a id="11619" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11653" class="Keyword">open</a> <a id="11658" class="Keyword">import</a> <a id="11665" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11694" class="Keyword">open</a> <a id="11699" class="Keyword">import</a> <a id="11706" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11729" class="Keyword">open</a> <a id="11734" class="Keyword">import</a> <a id="11741" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="11768" class="Keyword">open</a> <a id="11773" class="Keyword">import</a> <a id="11780" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11803" class="Keyword">open</a> <a id="11808" class="Keyword">import</a> <a id="11815" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="11857" class="Keyword">open</a> <a id="11862" class="Keyword">import</a> <a id="11869" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="11901" class="Keyword">open</a> <a id="11906" class="Keyword">import</a> <a id="11913" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="11940" class="Keyword">open</a> <a id="11945" class="Keyword">import</a> <a id="11952" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="11977" class="Keyword">open</a> <a id="11982" class="Keyword">import</a> <a id="11989" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12018" class="Keyword">open</a> <a id="12023" class="Keyword">import</a> <a id="12030" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="12060" class="Keyword">open</a> <a id="12065" class="Keyword">import</a> <a id="12072" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12099" class="Keyword">open</a> <a id="12104" class="Keyword">import</a> <a id="12111" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12130" class="Keyword">open</a> <a id="12135" class="Keyword">import</a> <a id="12142" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12188" class="Keyword">open</a> <a id="12193" class="Keyword">import</a> <a id="12200" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12242" class="Keyword">open</a> <a id="12247" class="Keyword">import</a> <a id="12254" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12286" class="Keyword">open</a> <a id="12291" class="Keyword">import</a> <a id="12298" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12328" class="Keyword">open</a> <a id="12333" class="Keyword">import</a> <a id="12340" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12366" class="Keyword">open</a> <a id="12371" class="Keyword">import</a> <a id="12378" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12412" class="Keyword">open</a> <a id="12417" class="Keyword">import</a> <a id="12424" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12454" class="Keyword">open</a> <a id="12459" class="Keyword">import</a> <a id="12466" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12493" class="Keyword">open</a> <a id="12498" class="Keyword">import</a> <a id="12505" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="12543" class="Keyword">open</a> <a id="12548" class="Keyword">import</a> <a id="12555" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12587" class="Keyword">open</a> <a id="12592" class="Keyword">import</a> <a id="12599" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12633" class="Keyword">open</a> <a id="12638" class="Keyword">import</a> <a id="12645" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12668" class="Keyword">open</a> <a id="12673" class="Keyword">import</a> <a id="12680" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12707" class="Keyword">open</a> <a id="12712" class="Keyword">import</a> <a id="12719" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12747" class="Keyword">open</a> <a id="12752" class="Keyword">import</a> <a id="12759" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12796" class="Keyword">open</a> <a id="12801" class="Keyword">import</a> <a id="12808" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12856" class="Keyword">open</a> <a id="12861" class="Keyword">import</a> <a id="12868" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="12908" class="Keyword">open</a> <a id="12913" class="Keyword">import</a> <a id="12920" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="12942" class="Keyword">open</a> <a id="12947" class="Keyword">import</a> <a id="12954" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="12977" class="Keyword">open</a> <a id="12982" class="Keyword">import</a> <a id="12989" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13014" class="Keyword">open</a> <a id="13019" class="Keyword">import</a> <a id="13026" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13071" class="Keyword">open</a> <a id="13076" class="Keyword">import</a> <a id="13083" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13127" class="Keyword">open</a> <a id="13132" class="Keyword">import</a> <a id="13139" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13175" class="Keyword">open</a> <a id="13180" class="Keyword">import</a> <a id="13187" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13232" class="Keyword">open</a> <a id="13237" class="Keyword">import</a> <a id="13244" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13285" class="Keyword">open</a> <a id="13290" class="Keyword">import</a> <a id="13297" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13332" class="Keyword">open</a> <a id="13337" class="Keyword">import</a> <a id="13344" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13376" class="Keyword">open</a> <a id="13381" class="Keyword">import</a> <a id="13388" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13419" class="Keyword">open</a> <a id="13424" class="Keyword">import</a> <a id="13431" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13464" class="Keyword">open</a> <a id="13469" class="Keyword">import</a> <a id="13476" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13509" class="Keyword">open</a> <a id="13514" class="Keyword">import</a> <a id="13521" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13551" class="Keyword">open</a> <a id="13556" class="Keyword">import</a> <a id="13563" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13587" class="Keyword">open</a> <a id="13592" class="Keyword">import</a> <a id="13599" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13637" class="Keyword">open</a> <a id="13642" class="Keyword">import</a> <a id="13649" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13680" class="Keyword">open</a> <a id="13685" class="Keyword">import</a> <a id="13692" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13717" class="Keyword">open</a> <a id="13722" class="Keyword">import</a> <a id="13729" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13757" class="Keyword">open</a> <a id="13762" class="Keyword">import</a> <a id="13769" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13793" class="Keyword">open</a> <a id="13798" class="Keyword">import</a> <a id="13805" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13831" class="Keyword">open</a> <a id="13836" class="Keyword">import</a> <a id="13843" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="13878" class="Keyword">open</a> <a id="13883" class="Keyword">import</a> <a id="13890" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="13911" class="Keyword">open</a> <a id="13916" class="Keyword">import</a> <a id="13923" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="13972" class="Keyword">open</a> <a id="13977" class="Keyword">import</a> <a id="13984" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14025" class="Keyword">open</a> <a id="14030" class="Keyword">import</a> <a id="14037" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14087" class="Keyword">open</a> <a id="14092" class="Keyword">import</a> <a id="14099" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14145" class="Keyword">open</a> <a id="14150" class="Keyword">import</a> <a id="14157" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14197" class="Keyword">open</a> <a id="14202" class="Keyword">import</a> <a id="14209" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14259" class="Keyword">open</a> <a id="14264" class="Keyword">import</a> <a id="14271" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14310" class="Keyword">open</a> <a id="14315" class="Keyword">import</a> <a id="14322" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14362" class="Keyword">open</a> <a id="14367" class="Keyword">import</a> <a id="14374" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14407" class="Keyword">open</a> <a id="14412" class="Keyword">import</a> <a id="14419" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14468" class="Keyword">open</a> <a id="14473" class="Keyword">import</a> <a id="14480" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14505" class="Keyword">open</a> <a id="14510" class="Keyword">import</a> <a id="14517" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14555" class="Keyword">open</a> <a id="14560" class="Keyword">import</a> <a id="14567" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14589" class="Keyword">open</a> <a id="14594" class="Keyword">import</a> <a id="14601" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14629" class="Keyword">open</a> <a id="14634" class="Keyword">import</a> <a id="14641" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="14677" class="Keyword">open</a> <a id="14682" class="Keyword">import</a> <a id="14689" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14715" class="Keyword">open</a> <a id="14720" class="Keyword">import</a> <a id="14727" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14745" class="Keyword">open</a> <a id="14750" class="Keyword">import</a> <a id="14757" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14792" class="Keyword">open</a> <a id="14797" class="Keyword">import</a> <a id="14804" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="14839" class="Keyword">open</a> <a id="14844" class="Keyword">import</a> <a id="14851" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="14878" class="Keyword">open</a> <a id="14883" class="Keyword">import</a> <a id="14890" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="14946" class="Keyword">open</a> <a id="14951" class="Keyword">import</a> <a id="14958" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="14987" class="Keyword">open</a> <a id="14992" class="Keyword">import</a> <a id="14999" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15029" class="Keyword">open</a> <a id="15034" class="Keyword">import</a> <a id="15041" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15068" class="Keyword">open</a> <a id="15073" class="Keyword">import</a> <a id="15080" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15106" class="Keyword">open</a> <a id="15111" class="Keyword">import</a> <a id="15118" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15145" class="Keyword">open</a> <a id="15150" class="Keyword">import</a> <a id="15157" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15181" class="Keyword">open</a> <a id="15186" class="Keyword">import</a> <a id="15193" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15216" class="Keyword">open</a> <a id="15221" class="Keyword">import</a> <a id="15228" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15255" class="Keyword">open</a> <a id="15260" class="Keyword">import</a> <a id="15267" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15299" class="Keyword">open</a> <a id="15304" class="Keyword">import</a> <a id="15311" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15346" class="Keyword">open</a> <a id="15351" class="Keyword">import</a> <a id="15358" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15389" class="Keyword">open</a> <a id="15394" class="Keyword">import</a> <a id="15401" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15434" class="Keyword">open</a> <a id="15439" class="Keyword">import</a> <a id="15446" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15480" class="Keyword">open</a> <a id="15485" class="Keyword">import</a> <a id="15492" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15532" class="Keyword">open</a> <a id="15537" class="Keyword">import</a> <a id="15544" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15575" class="Keyword">open</a> <a id="15580" class="Keyword">import</a> <a id="15587" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15619" class="Keyword">open</a> <a id="15624" class="Keyword">import</a> <a id="15631" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15662" class="Keyword">open</a> <a id="15667" class="Keyword">import</a> <a id="15674" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15691" class="Keyword">open</a> <a id="15696" class="Keyword">import</a> <a id="15703" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15728" class="Keyword">open</a> <a id="15733" class="Keyword">import</a> <a id="15740" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15769" class="Keyword">open</a> <a id="15774" class="Keyword">import</a> <a id="15781" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15806" class="Keyword">open</a> <a id="15811" class="Keyword">import</a> <a id="15818" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15839" class="Keyword">open</a> <a id="15844" class="Keyword">import</a> <a id="15851" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="15875" class="Keyword">open</a> <a id="15880" class="Keyword">import</a> <a id="15887" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="15907" class="Keyword">open</a> <a id="15912" class="Keyword">import</a> <a id="15919" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="15953" class="Keyword">open</a> <a id="15958" class="Keyword">import</a> <a id="15965" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16003" class="Keyword">open</a> <a id="16008" class="Keyword">import</a> <a id="16015" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16043" class="Keyword">open</a> <a id="16048" class="Keyword">import</a> <a id="16055" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16079" class="Keyword">open</a> <a id="16084" class="Keyword">import</a> <a id="16091" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16118" class="Keyword">open</a> <a id="16123" class="Keyword">import</a> <a id="16130" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16165" class="Keyword">open</a> <a id="16170" class="Keyword">import</a> <a id="16177" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16198" class="Keyword">open</a> <a id="16203" class="Keyword">import</a> <a id="16210" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16246" class="Keyword">open</a> <a id="16251" class="Keyword">import</a> <a id="16258" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16303" class="Keyword">open</a> <a id="16308" class="Keyword">import</a> <a id="16315" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16361" class="Keyword">open</a> <a id="16366" class="Keyword">import</a> <a id="16373" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16413" class="Keyword">open</a> <a id="16418" class="Keyword">import</a> <a id="16425" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16455" class="Keyword">open</a> <a id="16460" class="Keyword">import</a> <a id="16467" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16504" class="Keyword">open</a> <a id="16509" class="Keyword">import</a> <a id="16516" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16540" class="Keyword">open</a> <a id="16545" class="Keyword">import</a> <a id="16552" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16573" class="Keyword">open</a> <a id="16578" class="Keyword">import</a> <a id="16585" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16620" class="Keyword">open</a> <a id="16625" class="Keyword">import</a> <a id="16632" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16669" class="Keyword">open</a> <a id="16674" class="Keyword">import</a> <a id="16681" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16730" class="Keyword">open</a> <a id="16735" class="Keyword">import</a> <a id="16742" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16775" class="Keyword">open</a> <a id="16780" class="Keyword">import</a> <a id="16787" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16810" class="Keyword">open</a> <a id="16815" class="Keyword">import</a> <a id="16822" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="16845" class="Keyword">open</a> <a id="16850" class="Keyword">import</a> <a id="16857" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="16880" class="Keyword">open</a> <a id="16885" class="Keyword">import</a> <a id="16892" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="16920" class="Keyword">open</a> <a id="16925" class="Keyword">import</a> <a id="16932" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="16952" class="Keyword">open</a> <a id="16957" class="Keyword">import</a> <a id="16964" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="16985" class="Keyword">open</a> <a id="16990" class="Keyword">import</a> <a id="16997" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17028" class="Keyword">open</a> <a id="17033" class="Keyword">import</a> <a id="17040" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17067" class="Keyword">open</a> <a id="17072" class="Keyword">import</a> <a id="17079" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17095" class="Keyword">open</a> <a id="17100" class="Keyword">import</a> <a id="17107" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17138" class="Keyword">open</a> <a id="17143" class="Keyword">import</a> <a id="17150" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17167" class="Keyword">open</a> <a id="17172" class="Keyword">import</a> <a id="17179" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17201" class="Keyword">open</a> <a id="17206" class="Keyword">import</a> <a id="17213" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17240" class="Keyword">open</a> <a id="17245" class="Keyword">import</a> <a id="17252" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17275" class="Keyword">open</a> <a id="17280" class="Keyword">import</a> <a id="17287" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17314" class="Keyword">open</a> <a id="17319" class="Keyword">import</a> <a id="17326" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17359" class="Keyword">open</a> <a id="17364" class="Keyword">import</a> <a id="17371" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17411" class="Keyword">open</a> <a id="17416" class="Keyword">import</a> <a id="17423" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17444" class="Keyword">open</a> <a id="17449" class="Keyword">import</a> <a id="17456" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17485" class="Keyword">open</a> <a id="17490" class="Keyword">import</a> <a id="17497" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17535" class="Keyword">open</a> <a id="17540" class="Keyword">import</a> <a id="17547" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17567" class="Keyword">open</a> <a id="17572" class="Keyword">import</a> <a id="17579" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17603" class="Keyword">open</a> <a id="17608" class="Keyword">import</a> <a id="17615" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17642" class="Keyword">open</a> <a id="17647" class="Keyword">import</a> <a id="17654" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17686" class="Keyword">open</a> <a id="17691" class="Keyword">import</a> <a id="17698" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17728" class="Keyword">open</a> <a id="17733" class="Keyword">import</a> <a id="17740" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17766" class="Keyword">open</a> <a id="17771" class="Keyword">import</a> <a id="17778" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17805" class="Keyword">open</a> <a id="17810" class="Keyword">import</a> <a id="17817" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="17846" class="Keyword">open</a> <a id="17851" class="Keyword">import</a> <a id="17858" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="17881" class="Keyword">open</a> <a id="17886" class="Keyword">import</a> <a id="17893" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="17944" class="Keyword">open</a> <a id="17949" class="Keyword">import</a> <a id="17956" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="17999" class="Keyword">open</a> <a id="18004" class="Keyword">import</a> <a id="18011" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18059" class="Keyword">open</a> <a id="18064" class="Keyword">import</a> <a id="18071" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18109" class="Keyword">open</a> <a id="18114" class="Keyword">import</a> <a id="18121" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18158" class="Keyword">open</a> <a id="18163" class="Keyword">import</a> <a id="18170" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="18216" class="Keyword">open</a> <a id="18221" class="Keyword">import</a> <a id="18228" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18245" class="Keyword">open</a> <a id="18250" class="Keyword">import</a> <a id="18257" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="18285" class="Keyword">open</a> <a id="18290" class="Keyword">import</a> <a id="18297" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18325" class="Keyword">open</a> <a id="18330" class="Keyword">import</a> <a id="18337" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18373" class="Keyword">open</a> <a id="18378" class="Keyword">import</a> <a id="18385" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18423" class="Keyword">open</a> <a id="18428" class="Keyword">import</a> <a id="18435" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18468" class="Keyword">open</a> <a id="18473" class="Keyword">import</a> <a id="18480" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18501" class="Keyword">open</a> <a id="18506" class="Keyword">import</a> <a id="18513" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="18549" class="Keyword">open</a> <a id="18554" class="Keyword">import</a> <a id="18561" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18615" class="Keyword">open</a> <a id="18620" class="Keyword">import</a> <a id="18627" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18649" class="Keyword">open</a> <a id="18654" class="Keyword">import</a> <a id="18661" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18696" class="Keyword">open</a> <a id="18701" class="Keyword">import</a> <a id="18708" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18738" class="Keyword">open</a> <a id="18743" class="Keyword">import</a> <a id="18750" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18789" class="Keyword">open</a> <a id="18794" class="Keyword">import</a> <a id="18801" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18855" class="Keyword">open</a> <a id="18860" class="Keyword">import</a> <a id="18867" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18913" class="Keyword">open</a> <a id="18918" class="Keyword">import</a> <a id="18925" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18976" class="Keyword">open</a> <a id="18981" class="Keyword">import</a> <a id="18988" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="19029" class="Keyword">open</a> <a id="19034" class="Keyword">import</a> <a id="19041" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19086" class="Keyword">open</a> <a id="19091" class="Keyword">import</a> <a id="19098" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19143" class="Keyword">open</a> <a id="19148" class="Keyword">import</a> <a id="19155" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19191" class="Keyword">open</a> <a id="19196" class="Keyword">import</a> <a id="19203" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19239" class="Keyword">open</a> <a id="19244" class="Keyword">import</a> <a id="19251" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19316" class="Keyword">open</a> <a id="19321" class="Keyword">import</a> <a id="19328" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19383" class="Keyword">open</a> <a id="19388" class="Keyword">import</a> <a id="19395" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19435" class="Keyword">open</a> <a id="19440" class="Keyword">import</a> <a id="19447" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19491" class="Keyword">open</a> <a id="19496" class="Keyword">import</a> <a id="19503" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19548" class="Keyword">open</a> <a id="19553" class="Keyword">import</a> <a id="19560" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19601" class="Keyword">open</a> <a id="19606" class="Keyword">import</a> <a id="19613" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19653" class="Keyword">open</a> <a id="19658" class="Keyword">import</a> <a id="19665" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19692" class="Keyword">open</a> <a id="19697" class="Keyword">import</a> <a id="19704" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19740" class="Keyword">open</a> <a id="19745" class="Keyword">import</a> <a id="19752" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19779" class="Keyword">open</a> <a id="19784" class="Keyword">import</a> <a id="19791" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19828" class="Keyword">open</a> <a id="19833" class="Keyword">import</a> <a id="19840" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19868" class="Keyword">open</a> <a id="19873" class="Keyword">import</a> <a id="19880" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19899" class="Keyword">open</a> <a id="19904" class="Keyword">import</a> <a id="19911" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19951" class="Keyword">open</a> <a id="19956" class="Keyword">import</a> <a id="19963" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19995" class="Keyword">open</a> <a id="20000" class="Keyword">import</a> <a id="20007" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20055" class="Keyword">open</a> <a id="20060" class="Keyword">import</a> <a id="20067" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20090" class="Keyword">open</a> <a id="20095" class="Keyword">import</a> <a id="20102" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20126" class="Keyword">open</a> <a id="20131" class="Keyword">import</a> <a id="20138" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20178" class="Keyword">open</a> <a id="20183" class="Keyword">import</a> <a id="20190" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20233" class="Keyword">open</a> <a id="20238" class="Keyword">import</a> <a id="20245" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20279" class="Keyword">open</a> <a id="20284" class="Keyword">import</a> <a id="20291" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20323" class="Keyword">open</a> <a id="20328" class="Keyword">import</a> <a id="20335" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20365" class="Keyword">open</a> <a id="20370" class="Keyword">import</a> <a id="20377" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20411" class="Keyword">open</a> <a id="20416" class="Keyword">import</a> <a id="20423" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20458" class="Keyword">open</a> <a id="20463" class="Keyword">import</a> <a id="20470" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20507" class="Keyword">open</a> <a id="20512" class="Keyword">import</a> <a id="20519" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20546" class="Keyword">open</a> <a id="20551" class="Keyword">import</a> <a id="20558" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20586" class="Keyword">open</a> <a id="20591" class="Keyword">import</a> <a id="20598" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20647" class="Keyword">open</a> <a id="20652" class="Keyword">import</a> <a id="20659" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20705" class="Keyword">open</a> <a id="20710" class="Keyword">import</a> <a id="20717" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20757" class="Keyword">open</a> <a id="20762" class="Keyword">import</a> <a id="20769" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20807" class="Keyword">open</a> <a id="20812" class="Keyword">import</a> <a id="20819" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20848" class="Keyword">open</a> <a id="20853" class="Keyword">import</a> <a id="20860" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20890" class="Keyword">open</a> <a id="20895" class="Keyword">import</a> <a id="20902" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20933" class="Keyword">open</a> <a id="20938" class="Keyword">import</a> <a id="20945" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="20985" class="Keyword">open</a> <a id="20990" class="Keyword">import</a> <a id="20997" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="21023" class="Keyword">open</a> <a id="21028" class="Keyword">import</a> <a id="21035" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21090" class="Keyword">open</a> <a id="21095" class="Keyword">import</a> <a id="21102" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21153" class="Keyword">open</a> <a id="21158" class="Keyword">import</a> <a id="21165" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21210" class="Keyword">open</a> <a id="21215" class="Keyword">import</a> <a id="21222" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21276" class="Keyword">open</a> <a id="21281" class="Keyword">import</a> <a id="21288" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21315" class="Keyword">open</a> <a id="21320" class="Keyword">import</a> <a id="21327" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21360" class="Keyword">open</a> <a id="21365" class="Keyword">import</a> <a id="21372" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21403" class="Keyword">open</a> <a id="21408" class="Keyword">import</a> <a id="21415" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21452" class="Keyword">open</a> <a id="21457" class="Keyword">import</a> <a id="21464" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21489" class="Keyword">open</a> <a id="21494" class="Keyword">import</a> <a id="21501" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21533" class="Keyword">open</a> <a id="21538" class="Keyword">import</a> <a id="21545" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21580" class="Keyword">open</a> <a id="21585" class="Keyword">import</a> <a id="21592" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21621" class="Keyword">open</a> <a id="21626" class="Keyword">import</a> <a id="21633" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21659" class="Keyword">open</a> <a id="21664" class="Keyword">import</a> <a id="21671" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21699" class="Keyword">open</a> <a id="21704" class="Keyword">import</a> <a id="21711" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21736" class="Keyword">open</a> <a id="21741" class="Keyword">import</a> <a id="21748" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21769" class="Keyword">open</a> <a id="21774" class="Keyword">import</a> <a id="21781" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21817" class="Keyword">open</a> <a id="21822" class="Keyword">import</a> <a id="21829" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21872" class="Keyword">open</a> <a id="21877" class="Keyword">import</a> <a id="21884" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21909" class="Keyword">open</a> <a id="21914" class="Keyword">import</a> <a id="21921" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21952" class="Keyword">open</a> <a id="21957" class="Keyword">import</a> <a id="21964" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21996" class="Keyword">open</a> <a id="22001" class="Keyword">import</a> <a id="22008" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22042" class="Keyword">open</a> <a id="22047" class="Keyword">import</a> <a id="22054" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22110" class="Keyword">open</a> <a id="22115" class="Keyword">import</a> <a id="22122" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22175" class="Keyword">open</a> <a id="22180" class="Keyword">import</a> <a id="22187" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22214" class="Keyword">open</a> <a id="22219" class="Keyword">import</a> <a id="22226" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22271" class="Keyword">open</a> <a id="22276" class="Keyword">import</a> <a id="22283" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22345" class="Keyword">open</a> <a id="22350" class="Keyword">import</a> <a id="22357" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22370" class="Keyword">open</a> <a id="22375" class="Keyword">import</a> <a id="22382" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22423" class="Keyword">open</a> <a id="22428" class="Keyword">import</a> <a id="22435" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22464" class="Keyword">open</a> <a id="22469" class="Keyword">import</a> <a id="22476" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22521" class="Keyword">open</a> <a id="22526" class="Keyword">import</a> <a id="22533" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22577" class="Keyword">open</a> <a id="22582" class="Keyword">import</a> <a id="22589" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="22616" class="Keyword">open</a> <a id="22621" class="Keyword">import</a> <a id="22628" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="22669" class="Keyword">open</a> <a id="22674" class="Keyword">import</a> <a id="22681" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="22704" class="Keyword">open</a> <a id="22709" class="Keyword">import</a> <a id="22716" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="22765" class="Keyword">open</a> <a id="22770" class="Keyword">import</a> <a id="22777" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="22816" class="Keyword">open</a> <a id="22821" class="Keyword">import</a> <a id="22828" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="22869" class="Keyword">open</a> <a id="22874" class="Keyword">import</a> <a id="22881" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22925" class="Keyword">open</a> <a id="22930" class="Keyword">import</a> <a id="22937" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22974" class="Keyword">open</a> <a id="22979" class="Keyword">import</a> <a id="22986" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="23008" class="Keyword">open</a> <a id="23013" class="Keyword">import</a> <a id="23020" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23050" class="Keyword">open</a> <a id="23055" class="Keyword">import</a> <a id="23062" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="23101" class="Keyword">open</a> <a id="23106" class="Keyword">import</a> <a id="23113" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="23151" class="Keyword">open</a> <a id="23156" class="Keyword">import</a> <a id="23163" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="23194" class="Keyword">open</a> <a id="23199" class="Keyword">import</a> <a id="23206" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="23233" class="Keyword">open</a> <a id="23238" class="Keyword">import</a> <a id="23245" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="23303" class="Keyword">open</a> <a id="23308" class="Keyword">import</a> <a id="23315" href="group-theory.html" class="Module">group-theory</a>
<a id="23328" class="Keyword">open</a> <a id="23333" class="Keyword">import</a> <a id="23340" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="23368" class="Keyword">open</a> <a id="23373" class="Keyword">import</a> <a id="23380" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="23411" class="Keyword">open</a> <a id="23416" class="Keyword">import</a> <a id="23423" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="23459" class="Keyword">open</a> <a id="23464" class="Keyword">import</a> <a id="23471" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="23522" class="Keyword">open</a> <a id="23527" class="Keyword">import</a> <a id="23534" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="23567" class="Keyword">open</a> <a id="23572" class="Keyword">import</a> <a id="23579" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="23626" class="Keyword">open</a> <a id="23631" class="Keyword">import</a> <a id="23638" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="23677" class="Keyword">open</a> <a id="23682" class="Keyword">import</a> <a id="23689" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="23729" class="Keyword">open</a> <a id="23734" class="Keyword">import</a> <a id="23741" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="23784" class="Keyword">open</a> <a id="23789" class="Keyword">import</a> <a id="23796" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="23828" class="Keyword">open</a> <a id="23833" class="Keyword">import</a> <a id="23840" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="23876" class="Keyword">open</a> <a id="23881" class="Keyword">import</a> <a id="23888" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="23917" class="Keyword">open</a> <a id="23922" class="Keyword">import</a> <a id="23929" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="23962" class="Keyword">open</a> <a id="23967" class="Keyword">import</a> <a id="23974" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="24010" class="Keyword">open</a> <a id="24015" class="Keyword">import</a> <a id="24022" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="24051" class="Keyword">open</a> <a id="24056" class="Keyword">import</a> <a id="24063" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="24095" class="Keyword">open</a> <a id="24100" class="Keyword">import</a> <a id="24107" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="24132" class="Keyword">open</a> <a id="24137" class="Keyword">import</a> <a id="24144" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="24175" class="Keyword">open</a> <a id="24180" class="Keyword">import</a> <a id="24187" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="24234" class="Keyword">open</a> <a id="24239" class="Keyword">import</a> <a id="24246" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="24279" class="Keyword">open</a> <a id="24284" class="Keyword">import</a> <a id="24291" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="24331" class="Keyword">open</a> <a id="24336" class="Keyword">import</a> <a id="24343" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="24380" class="Keyword">open</a> <a id="24385" class="Keyword">import</a> <a id="24392" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="24428" class="Keyword">open</a> <a id="24433" class="Keyword">import</a> <a id="24440" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="24472" class="Keyword">open</a> <a id="24477" class="Keyword">import</a> <a id="24484" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="24511" class="Keyword">open</a> <a id="24516" class="Keyword">import</a> <a id="24523" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="24543" class="Keyword">open</a> <a id="24548" class="Keyword">import</a> <a id="24555" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="24582" class="Keyword">open</a> <a id="24587" class="Keyword">import</a> <a id="24594" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="24636" class="Keyword">open</a> <a id="24641" class="Keyword">import</a> <a id="24648" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="24695" class="Keyword">open</a> <a id="24700" class="Keyword">import</a> <a id="24707" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="24748" class="Keyword">open</a> <a id="24753" class="Keyword">import</a> <a id="24760" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="24794" class="Keyword">open</a> <a id="24799" class="Keyword">import</a> <a id="24806" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="24841" class="Keyword">open</a> <a id="24846" class="Keyword">import</a> <a id="24853" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="24891" class="Keyword">open</a> <a id="24896" class="Keyword">import</a> <a id="24903" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="24935" class="Keyword">open</a> <a id="24940" class="Keyword">import</a> <a id="24947" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="24988" class="Keyword">open</a> <a id="24993" class="Keyword">import</a> <a id="25000" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="25041" class="Keyword">open</a> <a id="25046" class="Keyword">import</a> <a id="25053" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="25093" class="Keyword">open</a> <a id="25098" class="Keyword">import</a> <a id="25105" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="25138" class="Keyword">open</a> <a id="25143" class="Keyword">import</a> <a id="25150" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="25187" class="Keyword">open</a> <a id="25192" class="Keyword">import</a> <a id="25199" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="25229" class="Keyword">open</a> <a id="25234" class="Keyword">import</a> <a id="25241" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="25286" class="Keyword">open</a> <a id="25291" class="Keyword">import</a> <a id="25298" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="25326" class="Keyword">open</a> <a id="25331" class="Keyword">import</a> <a id="25338" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="25359" class="Keyword">open</a> <a id="25364" class="Keyword">import</a> <a id="25371" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="25405" class="Keyword">open</a> <a id="25410" class="Keyword">import</a> <a id="25417" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="25451" class="Keyword">open</a> <a id="25456" class="Keyword">import</a> <a id="25463" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="25498" class="Keyword">open</a> <a id="25503" class="Keyword">import</a> <a id="25510" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="25552" class="Keyword">open</a> <a id="25557" class="Keyword">import</a> <a id="25564" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="25599" class="Keyword">open</a> <a id="25604" class="Keyword">import</a> <a id="25611" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="25650" class="Keyword">open</a> <a id="25655" class="Keyword">import</a> <a id="25662" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="25699" class="Keyword">open</a> <a id="25704" class="Keyword">import</a> <a id="25711" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="25735" class="Keyword">open</a> <a id="25740" class="Keyword">import</a> <a id="25747" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="25772" class="Keyword">open</a> <a id="25777" class="Keyword">import</a> <a id="25784" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="25815" class="Keyword">open</a> <a id="25820" class="Keyword">import</a> <a id="25827" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="25878" class="Keyword">open</a> <a id="25883" class="Keyword">import</a> <a id="25890" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="25913" class="Keyword">open</a> <a id="25918" class="Keyword">import</a> <a id="25925" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="25973" class="Keyword">open</a> <a id="25978" class="Keyword">import</a> <a id="25985" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="26015" class="Keyword">open</a> <a id="26020" class="Keyword">import</a> <a id="26027" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="26097" class="Keyword">open</a> <a id="26102" class="Keyword">import</a> <a id="26109" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="26124" class="Keyword">open</a> <a id="26129" class="Keyword">import</a> <a id="26136" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="26169" class="Keyword">open</a> <a id="26174" class="Keyword">import</a> <a id="26181" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="26213" class="Keyword">open</a> <a id="26218" class="Keyword">import</a> <a id="26225" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="26267" class="Keyword">open</a> <a id="26272" class="Keyword">import</a> <a id="26279" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="26317" class="Keyword">open</a> <a id="26322" class="Keyword">import</a> <a id="26329" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="26366" class="Keyword">open</a> <a id="26371" class="Keyword">import</a> <a id="26378" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="26411" class="Keyword">open</a> <a id="26416" class="Keyword">import</a> <a id="26423" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="26447" class="Keyword">open</a> <a id="26452" class="Keyword">import</a> <a id="26459" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="26498" class="Keyword">open</a> <a id="26503" class="Keyword">import</a> <a id="26510" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="26556" class="Keyword">open</a> <a id="26561" class="Keyword">import</a> <a id="26568" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="26613" class="Keyword">open</a> <a id="26618" class="Keyword">import</a> <a id="26625" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="26663" class="Keyword">open</a> <a id="26668" class="Keyword">import</a> <a id="26675" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="26707" class="Keyword">open</a> <a id="26712" class="Keyword">import</a> <a id="26719" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="26772" class="Keyword">open</a> <a id="26777" class="Keyword">import</a> <a id="26784" href="order-theory.html" class="Module">order-theory</a>
<a id="26797" class="Keyword">open</a> <a id="26802" class="Keyword">import</a> <a id="26809" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="26836" class="Keyword">open</a> <a id="26841" class="Keyword">import</a> <a id="26848" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="26878" class="Keyword">open</a> <a id="26883" class="Keyword">import</a> <a id="26890" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="26923" class="Keyword">open</a> <a id="26928" class="Keyword">import</a> <a id="26935" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="26971" class="Keyword">open</a> <a id="26976" class="Keyword">import</a> <a id="26983" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="27010" class="Keyword">open</a> <a id="27015" class="Keyword">import</a> <a id="27022" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="27052" class="Keyword">open</a> <a id="27057" class="Keyword">import</a> <a id="27064" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="27100" class="Keyword">open</a> <a id="27105" class="Keyword">import</a> <a id="27112" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="27154" class="Keyword">open</a> <a id="27159" class="Keyword">import</a> <a id="27166" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="27198" class="Keyword">open</a> <a id="27203" class="Keyword">import</a> <a id="27210" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="27241" class="Keyword">open</a> <a id="27246" class="Keyword">import</a> <a id="27253" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="27279" class="Keyword">open</a> <a id="27284" class="Keyword">import</a> <a id="27291" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="27320" class="Keyword">open</a> <a id="27325" class="Keyword">import</a> <a id="27332" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="27369" class="Keyword">open</a> <a id="27374" class="Keyword">import</a> <a id="27381" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="27421" class="Keyword">open</a> <a id="27426" class="Keyword">import</a> <a id="27433" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="27455" class="Keyword">open</a> <a id="27460" class="Keyword">import</a> <a id="27467" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="27502" class="Keyword">open</a> <a id="27507" class="Keyword">import</a> <a id="27514" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="27552" class="Keyword">open</a> <a id="27557" class="Keyword">import</a> <a id="27564" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="27603" class="Keyword">open</a> <a id="27608" class="Keyword">import</a> <a id="27615" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="27650" class="Keyword">open</a> <a id="27655" class="Keyword">import</a> <a id="27662" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="27697" class="Keyword">open</a> <a id="27702" class="Keyword">import</a> <a id="27709" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="27747" class="Keyword">open</a> <a id="27752" class="Keyword">import</a> <a id="27759" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="27790" class="Keyword">open</a> <a id="27795" class="Keyword">import</a> <a id="27802" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="27844" class="Keyword">open</a> <a id="27849" class="Keyword">import</a> <a id="27856" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="27901" class="Keyword">open</a> <a id="27906" class="Keyword">import</a> <a id="27913" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="27946" class="Keyword">open</a> <a id="27951" class="Keyword">import</a> <a id="27958" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="27978" class="Keyword">open</a> <a id="27983" class="Keyword">import</a> <a id="27990" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="28013" class="Keyword">open</a> <a id="28018" class="Keyword">import</a> <a id="28025" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="28048" class="Keyword">open</a> <a id="28053" class="Keyword">import</a> <a id="28060" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="28086" class="Keyword">open</a> <a id="28091" class="Keyword">import</a> <a id="28098" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="28124" class="Keyword">open</a> <a id="28129" class="Keyword">import</a> <a id="28136" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="28192" class="Keyword">open</a> <a id="28197" class="Keyword">import</a> <a id="28204" href="polytopes.html" class="Module">polytopes</a>
<a id="28214" class="Keyword">open</a> <a id="28219" class="Keyword">import</a> <a id="28226" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="28284" class="Keyword">open</a> <a id="28289" class="Keyword">import</a> <a id="28296" href="ring-theory.html" class="Module">ring-theory</a>
<a id="28308" class="Keyword">open</a> <a id="28313" class="Keyword">import</a> <a id="28320" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="28357" class="Keyword">open</a> <a id="28362" class="Keyword">import</a> <a id="28369" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="28396" class="Keyword">open</a> <a id="28401" class="Keyword">import</a> <a id="28408" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="28440" class="Keyword">open</a> <a id="28445" class="Keyword">import</a> <a id="28452" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="28498" class="Keyword">open</a> <a id="28503" class="Keyword">import</a> <a id="28510" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="28535" class="Keyword">open</a> <a id="28540" class="Keyword">import</a> <a id="28547" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="28590" class="Keyword">open</a> <a id="28595" class="Keyword">import</a> <a id="28602" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="28640" class="Keyword">open</a> <a id="28645" class="Keyword">import</a> <a id="28652" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="28683" class="Keyword">open</a> <a id="28688" class="Keyword">import</a> <a id="28695" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="28727" class="Keyword">open</a> <a id="28732" class="Keyword">import</a> <a id="28739" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="28765" class="Keyword">open</a> <a id="28770" class="Keyword">import</a> <a id="28777" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="28806" class="Keyword">open</a> <a id="28811" class="Keyword">import</a> <a id="28818" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="28855" class="Keyword">open</a> <a id="28860" class="Keyword">import</a> <a id="28867" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="28896" class="Keyword">open</a> <a id="28901" class="Keyword">import</a> <a id="28908" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="28935" class="Keyword">open</a> <a id="28940" class="Keyword">import</a> <a id="28947" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="28984" class="Keyword">open</a> <a id="28989" class="Keyword">import</a> <a id="28996" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="29023" class="Keyword">open</a> <a id="29028" class="Keyword">import</a> <a id="29035" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="29068" class="Keyword">open</a> <a id="29073" class="Keyword">import</a> <a id="29080" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="29098" class="Keyword">open</a> <a id="29103" class="Keyword">import</a> <a id="29110" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="29164" class="Keyword">open</a> <a id="29169" class="Keyword">import</a> <a id="29176" href="set-theory.html" class="Module">set-theory</a>
<a id="29187" class="Keyword">open</a> <a id="29192" class="Keyword">import</a> <a id="29199" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="29225" class="Keyword">open</a> <a id="29230" class="Keyword">import</a> <a id="29237" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="29299" class="Keyword">open</a> <a id="29304" class="Keyword">import</a> <a id="29311" href="structured-types.html" class="Module">structured-types</a>
<a id="29328" class="Keyword">open</a> <a id="29333" class="Keyword">import</a> <a id="29340" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="29375" class="Keyword">open</a> <a id="29380" class="Keyword">import</a> <a id="29387" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="29431" class="Keyword">open</a> <a id="29436" class="Keyword">import</a> <a id="29443" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="29507" class="Keyword">open</a> <a id="29512" class="Keyword">import</a> <a id="29519" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="29565" class="Keyword">open</a> <a id="29570" class="Keyword">import</a> <a id="29577" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="29601" class="Keyword">open</a> <a id="29606" class="Keyword">import</a> <a id="29613" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="29682" class="Keyword">open</a> <a id="29687" class="Keyword">import</a> <a id="29694" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="29739" class="Keyword">open</a> <a id="29744" class="Keyword">import</a> <a id="29751" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="29785" class="Keyword">open</a> <a id="29790" class="Keyword">import</a> <a id="29797" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="29858" class="Keyword">open</a> <a id="29863" class="Keyword">import</a> <a id="29870" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="29915" class="Keyword">open</a> <a id="29920" class="Keyword">import</a> <a id="29927" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="29965" class="Keyword">open</a> <a id="29970" class="Keyword">import</a> <a id="29977" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="30020" class="Keyword">open</a> <a id="30025" class="Keyword">import</a> <a id="30032" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="30068" class="Keyword">open</a> <a id="30073" class="Keyword">import</a> <a id="30080" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="30110" class="Keyword">open</a> <a id="30115" class="Keyword">import</a> <a id="30122" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="30153" class="Keyword">open</a> <a id="30158" class="Keyword">import</a> <a id="30165" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="30216" class="Keyword">open</a> <a id="30221" class="Keyword">import</a> <a id="30228" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="30283" class="Keyword">open</a> <a id="30288" class="Keyword">import</a> <a id="30295" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="30324" class="Keyword">open</a> <a id="30329" class="Keyword">import</a> <a id="30336" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="30364" class="Keyword">open</a> <a id="30369" class="Keyword">import</a> <a id="30376" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="30406" class="Keyword">open</a> <a id="30411" class="Keyword">import</a> <a id="30418" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="30452" class="Keyword">open</a> <a id="30457" class="Keyword">import</a> <a id="30464" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="30540" class="Keyword">open</a> <a id="30545" class="Keyword">import</a> <a id="30552" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="30578" class="Keyword">open</a> <a id="30583" class="Keyword">import</a> <a id="30590" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="30629" class="Keyword">open</a> <a id="30634" class="Keyword">import</a> <a id="30641" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="30679" class="Keyword">open</a> <a id="30684" class="Keyword">import</a> <a id="30691" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="30737" class="Keyword">open</a> <a id="30742" class="Keyword">import</a> <a id="30749" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="30786" class="Keyword">open</a> <a id="30791" class="Keyword">import</a> <a id="30798" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="30838" class="Keyword">open</a> <a id="30843" class="Keyword">import</a> <a id="30850" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="30889" class="Keyword">open</a> <a id="30894" class="Keyword">import</a> <a id="30901" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="30934" class="Keyword">open</a> <a id="30939" class="Keyword">import</a> <a id="30946" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="30981" class="Keyword">open</a> <a id="30986" class="Keyword">import</a> <a id="30993" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="31032" class="Keyword">open</a> <a id="31037" class="Keyword">import</a> <a id="31044" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="31089" class="Keyword">open</a> <a id="31094" class="Keyword">import</a> <a id="31101" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="31153" class="Keyword">open</a> <a id="31158" class="Keyword">import</a> <a id="31165" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="31218" class="Keyword">open</a> <a id="31223" class="Keyword">import</a> <a id="31230" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="31278" class="Keyword">open</a> <a id="31283" class="Keyword">import</a> <a id="31290" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="31330" class="Keyword">open</a> <a id="31335" class="Keyword">import</a> <a id="31342" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="31389" class="Keyword">open</a> <a id="31394" class="Keyword">import</a> <a id="31401" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="31442" class="Keyword">open</a> <a id="31447" class="Keyword">import</a> <a id="31454" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="31492" class="Keyword">open</a> <a id="31497" class="Keyword">import</a> <a id="31504" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="31549" class="Keyword">open</a> <a id="31554" class="Keyword">import</a> <a id="31561" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="31610" class="Keyword">open</a> <a id="31615" class="Keyword">import</a> <a id="31622" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="31699" class="Keyword">open</a> <a id="31704" class="Keyword">import</a> <a id="31711" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="31763" class="Keyword">open</a> <a id="31768" class="Keyword">import</a> <a id="31775" href="type-theories.html" class="Module">type-theories</a>
<a id="31789" class="Keyword">open</a> <a id="31794" class="Keyword">import</a> <a id="31801" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="31843" class="Keyword">open</a> <a id="31848" class="Keyword">import</a> <a id="31855" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="31893" class="Keyword">open</a> <a id="31898" class="Keyword">import</a> <a id="31905" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="31951" class="Keyword">open</a> <a id="31956" class="Keyword">import</a> <a id="31963" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="32010" class="Keyword">open</a> <a id="32015" class="Keyword">import</a> <a id="32022" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="32057" class="Keyword">open</a> <a id="32062" class="Keyword">import</a> <a id="32069" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="32147" class="Keyword">open</a> <a id="32152" class="Keyword">import</a> <a id="32159" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="32183" class="Keyword">open</a> <a id="32188" class="Keyword">import</a> <a id="32195" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="32248" class="Keyword">open</a> <a id="32253" class="Keyword">import</a> <a id="32260" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="32303" class="Keyword">open</a> <a id="32308" class="Keyword">import</a> <a id="32315" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="32355" class="Keyword">open</a> <a id="32360" class="Keyword">import</a> <a id="32367" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="32406" class="Keyword">open</a> <a id="32411" class="Keyword">import</a> <a id="32418" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="32466" class="Keyword">open</a> <a id="32471" class="Keyword">import</a> <a id="32478" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="32525" class="Keyword">open</a> <a id="32530" class="Keyword">import</a> <a id="32537" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="32589" class="Keyword">open</a> <a id="32594" class="Keyword">import</a> <a id="32601" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="32645" class="Keyword">open</a> <a id="32650" class="Keyword">import</a> <a id="32657" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="32697" class="Keyword">open</a> <a id="32702" class="Keyword">import</a> <a id="32709" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="32761" class="Keyword">open</a> <a id="32766" class="Keyword">import</a> <a id="32773" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="32827" class="Keyword">open</a> <a id="32832" class="Keyword">import</a> <a id="32839" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="32887" class="Keyword">open</a> <a id="32892" class="Keyword">import</a> <a id="32899" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="32938" class="Keyword">open</a> <a id="32943" class="Keyword">import</a> <a id="32950" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="32983" class="Keyword">open</a> <a id="32988" class="Keyword">import</a> <a id="32995" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="33025" class="Keyword">open</a> <a id="33030" class="Keyword">import</a> <a id="33037" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="33096" class="Keyword">open</a> <a id="33101" class="Keyword">import</a> <a id="33108" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="33163" class="Keyword">open</a> <a id="33168" class="Keyword">import</a> <a id="33175" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="33222" class="Keyword">open</a> <a id="33227" class="Keyword">import</a> <a id="33234" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="33277" class="Keyword">open</a> <a id="33282" class="Keyword">import</a> <a id="33289" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="33334" class="Keyword">open</a> <a id="33339" class="Keyword">import</a> <a id="33346" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="33395" class="Keyword">open</a> <a id="33400" class="Keyword">import</a> <a id="33407" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="33458" class="Keyword">open</a> <a id="33463" class="Keyword">import</a> <a id="33470" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="33548" class="Keyword">open</a> <a id="33553" class="Keyword">import</a> <a id="33560" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="33600" class="Keyword">open</a> <a id="33605" class="Keyword">import</a> <a id="33612" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="33669" class="Keyword">open</a> <a id="33674" class="Keyword">import</a> <a id="33681" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="33716" class="Keyword">open</a> <a id="33721" class="Keyword">import</a> <a id="33728" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="33774" class="Keyword">open</a> <a id="33779" class="Keyword">import</a> <a id="33786" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="33841" class="Keyword">open</a> <a id="33846" class="Keyword">import</a> <a id="33853" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="33896" class="Keyword">open</a> <a id="33901" class="Keyword">import</a> <a id="33908" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="33967" class="Keyword">open</a> <a id="33972" class="Keyword">import</a> <a id="33979" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="34016" class="Keyword">open</a> <a id="34021" class="Keyword">import</a> <a id="34028" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="34069" class="Keyword">open</a> <a id="34074" class="Keyword">import</a> <a id="34081" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="34120" class="Keyword">open</a> <a id="34125" class="Keyword">import</a> <a id="34132" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="34170" class="Keyword">open</a> <a id="34175" class="Keyword">import</a> <a id="34182" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="34234" class="Keyword">open</a> <a id="34239" class="Keyword">import</a> <a id="34246" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="34291" class="Keyword">open</a> <a id="34296" class="Keyword">import</a> <a id="34303" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="34340" class="Keyword">open</a> <a id="34345" class="Keyword">import</a> <a id="34352" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="34401" class="Keyword">open</a> <a id="34406" class="Keyword">import</a> <a id="34413" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="34452" class="Keyword">open</a> <a id="34457" class="Keyword">import</a> <a id="34464" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="34502" class="Keyword">open</a> <a id="34507" class="Keyword">import</a> <a id="34514" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="34569" class="Keyword">open</a> <a id="34574" class="Keyword">import</a> <a id="34581" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="34620" class="Keyword">open</a> <a id="34625" class="Keyword">import</a> <a id="34632" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="34680" class="Keyword">open</a> <a id="34685" class="Keyword">import</a> <a id="34692" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="34739" class="Keyword">open</a> <a id="34744" class="Keyword">import</a> <a id="34751" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="34789" class="Keyword">open</a> <a id="34794" class="Keyword">import</a> <a id="34801" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="34831" class="Keyword">open</a> <a id="34836" class="Keyword">import</a> <a id="34843" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="34900" class="Keyword">open</a> <a id="34905" class="Keyword">import</a> <a id="34912" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="34966" class="Keyword">open</a> <a id="34971" class="Keyword">import</a> <a id="34978" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="35008" class="Keyword">open</a> <a id="35013" class="Keyword">import</a> <a id="35020" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="35083" class="Keyword">open</a> <a id="35088" class="Keyword">import</a> <a id="35095" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="35138" class="Keyword">open</a> <a id="35143" class="Keyword">import</a> <a id="35150" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="35185" class="Keyword">open</a> <a id="35190" class="Keyword">import</a> <a id="35197" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="35237" class="Keyword">open</a> <a id="35242" class="Keyword">import</a> <a id="35249" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="35294" class="Keyword">open</a> <a id="35299" class="Keyword">import</a> <a id="35306" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="35356" class="Keyword">open</a> <a id="35361" class="Keyword">import</a> <a id="35368" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="35406" class="Keyword">open</a> <a id="35411" class="Keyword">import</a> <a id="35418" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="35467" class="Keyword">open</a> <a id="35472" class="Keyword">import</a> <a id="35479" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="35526" class="Keyword">open</a> <a id="35531" class="Keyword">import</a> <a id="35538" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="35601" class="Keyword">open</a> <a id="35606" class="Keyword">import</a> <a id="35613" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="35645" class="Keyword">open</a> <a id="35650" class="Keyword">import</a> <a id="35657" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="35710" class="Keyword">open</a> <a id="35715" class="Keyword">import</a> <a id="35722" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="35768" class="Keyword">open</a> <a id="35773" class="Keyword">import</a> <a id="35780" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="35826" class="Keyword">open</a> <a id="35831" class="Keyword">import</a> <a id="35838" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="35886" class="Keyword">open</a> <a id="35891" class="Keyword">import</a> <a id="35898" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="35938" class="Keyword">open</a> <a id="35943" class="Keyword">import</a> <a id="35950" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="35995" class="Keyword">open</a> <a id="36000" class="Keyword">import</a> <a id="36007" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>