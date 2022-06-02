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
<a id="10185" class="Keyword">open</a> <a id="10190" class="Keyword">import</a> <a id="10197" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10243" class="Keyword">open</a> <a id="10248" class="Keyword">import</a> <a id="10255" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10289" class="Keyword">open</a> <a id="10294" class="Keyword">import</a> <a id="10301" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10336" class="Keyword">open</a> <a id="10341" class="Keyword">import</a> <a id="10348" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10386" class="Keyword">open</a> <a id="10391" class="Keyword">import</a> <a id="10398" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10436" class="Keyword">open</a> <a id="10441" class="Keyword">import</a> <a id="10448" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10488" class="Keyword">open</a> <a id="10493" class="Keyword">import</a> <a id="10500" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10533" class="Keyword">open</a> <a id="10538" class="Keyword">import</a> <a id="10545" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10583" class="Keyword">open</a> <a id="10588" class="Keyword">import</a> <a id="10595" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10658" class="Keyword">open</a> <a id="10663" class="Keyword">import</a> <a id="10670" href="foundation.html" class="Module">foundation</a>
<a id="10681" class="Keyword">open</a> <a id="10686" class="Keyword">import</a> <a id="10693" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10711" class="Keyword">open</a> <a id="10716" class="Keyword">import</a> <a id="10723" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10742" class="Keyword">open</a> <a id="10747" class="Keyword">import</a> <a id="10754" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10773" class="Keyword">open</a> <a id="10778" class="Keyword">import</a> <a id="10785" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="10829" class="Keyword">open</a> <a id="10834" class="Keyword">import</a> <a id="10841" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="10866" class="Keyword">open</a> <a id="10871" class="Keyword">import</a> <a id="10878" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="10905" class="Keyword">open</a> <a id="10910" class="Keyword">import</a> <a id="10917" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="10934" class="Keyword">open</a> <a id="10939" class="Keyword">import</a> <a id="10946" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="10975" class="Keyword">open</a> <a id="10980" class="Keyword">import</a> <a id="10987" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11043" class="Keyword">open</a> <a id="11048" class="Keyword">import</a> <a id="11055" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11086" class="Keyword">open</a> <a id="11091" class="Keyword">import</a> <a id="11098" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11152" class="Keyword">open</a> <a id="11157" class="Keyword">import</a> <a id="11164" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11192" class="Keyword">open</a> <a id="11197" class="Keyword">import</a> <a id="11204" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11234" class="Keyword">open</a> <a id="11239" class="Keyword">import</a> <a id="11246" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11266" class="Keyword">open</a> <a id="11271" class="Keyword">import</a> <a id="11278" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11323" class="Keyword">open</a> <a id="11328" class="Keyword">import</a> <a id="11335" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11372" class="Keyword">open</a> <a id="11377" class="Keyword">import</a> <a id="11384" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11419" class="Keyword">open</a> <a id="11424" class="Keyword">import</a> <a id="11431" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11489" class="Keyword">open</a> <a id="11494" class="Keyword">import</a> <a id="11501" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11539" class="Keyword">open</a> <a id="11544" class="Keyword">import</a> <a id="11551" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11585" class="Keyword">open</a> <a id="11590" class="Keyword">import</a> <a id="11597" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11626" class="Keyword">open</a> <a id="11631" class="Keyword">import</a> <a id="11638" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11661" class="Keyword">open</a> <a id="11666" class="Keyword">import</a> <a id="11673" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="11700" class="Keyword">open</a> <a id="11705" class="Keyword">import</a> <a id="11712" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11735" class="Keyword">open</a> <a id="11740" class="Keyword">import</a> <a id="11747" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="11789" class="Keyword">open</a> <a id="11794" class="Keyword">import</a> <a id="11801" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="11833" class="Keyword">open</a> <a id="11838" class="Keyword">import</a> <a id="11845" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="11872" class="Keyword">open</a> <a id="11877" class="Keyword">import</a> <a id="11884" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="11909" class="Keyword">open</a> <a id="11914" class="Keyword">import</a> <a id="11921" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="11950" class="Keyword">open</a> <a id="11955" class="Keyword">import</a> <a id="11962" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="11992" class="Keyword">open</a> <a id="11997" class="Keyword">import</a> <a id="12004" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12031" class="Keyword">open</a> <a id="12036" class="Keyword">import</a> <a id="12043" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12062" class="Keyword">open</a> <a id="12067" class="Keyword">import</a> <a id="12074" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12120" class="Keyword">open</a> <a id="12125" class="Keyword">import</a> <a id="12132" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12174" class="Keyword">open</a> <a id="12179" class="Keyword">import</a> <a id="12186" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12218" class="Keyword">open</a> <a id="12223" class="Keyword">import</a> <a id="12230" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12260" class="Keyword">open</a> <a id="12265" class="Keyword">import</a> <a id="12272" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12298" class="Keyword">open</a> <a id="12303" class="Keyword">import</a> <a id="12310" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12344" class="Keyword">open</a> <a id="12349" class="Keyword">import</a> <a id="12356" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12386" class="Keyword">open</a> <a id="12391" class="Keyword">import</a> <a id="12398" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12425" class="Keyword">open</a> <a id="12430" class="Keyword">import</a> <a id="12437" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12469" class="Keyword">open</a> <a id="12474" class="Keyword">import</a> <a id="12481" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12515" class="Keyword">open</a> <a id="12520" class="Keyword">import</a> <a id="12527" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12550" class="Keyword">open</a> <a id="12555" class="Keyword">import</a> <a id="12562" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="12632" class="Keyword">open</a> <a id="12637" class="Keyword">import</a> <a id="12644" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="12714" class="Keyword">open</a> <a id="12719" class="Keyword">import</a> <a id="12726" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12753" class="Keyword">open</a> <a id="12758" class="Keyword">import</a> <a id="12765" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12793" class="Keyword">open</a> <a id="12798" class="Keyword">import</a> <a id="12805" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12842" class="Keyword">open</a> <a id="12847" class="Keyword">import</a> <a id="12854" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12902" class="Keyword">open</a> <a id="12907" class="Keyword">import</a> <a id="12914" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="12954" class="Keyword">open</a> <a id="12959" class="Keyword">import</a> <a id="12966" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="12988" class="Keyword">open</a> <a id="12993" class="Keyword">import</a> <a id="13000" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13023" class="Keyword">open</a> <a id="13028" class="Keyword">import</a> <a id="13035" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13060" class="Keyword">open</a> <a id="13065" class="Keyword">import</a> <a id="13072" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13117" class="Keyword">open</a> <a id="13122" class="Keyword">import</a> <a id="13129" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13173" class="Keyword">open</a> <a id="13178" class="Keyword">import</a> <a id="13185" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13221" class="Keyword">open</a> <a id="13226" class="Keyword">import</a> <a id="13233" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13278" class="Keyword">open</a> <a id="13283" class="Keyword">import</a> <a id="13290" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13331" class="Keyword">open</a> <a id="13336" class="Keyword">import</a> <a id="13343" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13378" class="Keyword">open</a> <a id="13383" class="Keyword">import</a> <a id="13390" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13422" class="Keyword">open</a> <a id="13427" class="Keyword">import</a> <a id="13434" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13465" class="Keyword">open</a> <a id="13470" class="Keyword">import</a> <a id="13477" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13510" class="Keyword">open</a> <a id="13515" class="Keyword">import</a> <a id="13522" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13555" class="Keyword">open</a> <a id="13560" class="Keyword">import</a> <a id="13567" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13597" class="Keyword">open</a> <a id="13602" class="Keyword">import</a> <a id="13609" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13633" class="Keyword">open</a> <a id="13638" class="Keyword">import</a> <a id="13645" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13683" class="Keyword">open</a> <a id="13688" class="Keyword">import</a> <a id="13695" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13726" class="Keyword">open</a> <a id="13731" class="Keyword">import</a> <a id="13738" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13763" class="Keyword">open</a> <a id="13768" class="Keyword">import</a> <a id="13775" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13803" class="Keyword">open</a> <a id="13808" class="Keyword">import</a> <a id="13815" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13839" class="Keyword">open</a> <a id="13844" class="Keyword">import</a> <a id="13851" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13877" class="Keyword">open</a> <a id="13882" class="Keyword">import</a> <a id="13889" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="13924" class="Keyword">open</a> <a id="13929" class="Keyword">import</a> <a id="13936" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="13957" class="Keyword">open</a> <a id="13962" class="Keyword">import</a> <a id="13969" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14018" class="Keyword">open</a> <a id="14023" class="Keyword">import</a> <a id="14030" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14071" class="Keyword">open</a> <a id="14076" class="Keyword">import</a> <a id="14083" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14133" class="Keyword">open</a> <a id="14138" class="Keyword">import</a> <a id="14145" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14191" class="Keyword">open</a> <a id="14196" class="Keyword">import</a> <a id="14203" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14243" class="Keyword">open</a> <a id="14248" class="Keyword">import</a> <a id="14255" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14305" class="Keyword">open</a> <a id="14310" class="Keyword">import</a> <a id="14317" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14356" class="Keyword">open</a> <a id="14361" class="Keyword">import</a> <a id="14368" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14408" class="Keyword">open</a> <a id="14413" class="Keyword">import</a> <a id="14420" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14453" class="Keyword">open</a> <a id="14458" class="Keyword">import</a> <a id="14465" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14514" class="Keyword">open</a> <a id="14519" class="Keyword">import</a> <a id="14526" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14551" class="Keyword">open</a> <a id="14556" class="Keyword">import</a> <a id="14563" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14601" class="Keyword">open</a> <a id="14606" class="Keyword">import</a> <a id="14613" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14635" class="Keyword">open</a> <a id="14640" class="Keyword">import</a> <a id="14647" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14675" class="Keyword">open</a> <a id="14680" class="Keyword">import</a> <a id="14687" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14713" class="Keyword">open</a> <a id="14718" class="Keyword">import</a> <a id="14725" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14743" class="Keyword">open</a> <a id="14748" class="Keyword">import</a> <a id="14755" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14790" class="Keyword">open</a> <a id="14795" class="Keyword">import</a> <a id="14802" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="14837" class="Keyword">open</a> <a id="14842" class="Keyword">import</a> <a id="14849" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="14876" class="Keyword">open</a> <a id="14881" class="Keyword">import</a> <a id="14888" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="14944" class="Keyword">open</a> <a id="14949" class="Keyword">import</a> <a id="14956" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="14985" class="Keyword">open</a> <a id="14990" class="Keyword">import</a> <a id="14997" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15027" class="Keyword">open</a> <a id="15032" class="Keyword">import</a> <a id="15039" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15066" class="Keyword">open</a> <a id="15071" class="Keyword">import</a> <a id="15078" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15104" class="Keyword">open</a> <a id="15109" class="Keyword">import</a> <a id="15116" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15143" class="Keyword">open</a> <a id="15148" class="Keyword">import</a> <a id="15155" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15179" class="Keyword">open</a> <a id="15184" class="Keyword">import</a> <a id="15191" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15214" class="Keyword">open</a> <a id="15219" class="Keyword">import</a> <a id="15226" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15253" class="Keyword">open</a> <a id="15258" class="Keyword">import</a> <a id="15265" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15297" class="Keyword">open</a> <a id="15302" class="Keyword">import</a> <a id="15309" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15344" class="Keyword">open</a> <a id="15349" class="Keyword">import</a> <a id="15356" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15387" class="Keyword">open</a> <a id="15392" class="Keyword">import</a> <a id="15399" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15432" class="Keyword">open</a> <a id="15437" class="Keyword">import</a> <a id="15444" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15478" class="Keyword">open</a> <a id="15483" class="Keyword">import</a> <a id="15490" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15530" class="Keyword">open</a> <a id="15535" class="Keyword">import</a> <a id="15542" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15573" class="Keyword">open</a> <a id="15578" class="Keyword">import</a> <a id="15585" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15617" class="Keyword">open</a> <a id="15622" class="Keyword">import</a> <a id="15629" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15660" class="Keyword">open</a> <a id="15665" class="Keyword">import</a> <a id="15672" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15689" class="Keyword">open</a> <a id="15694" class="Keyword">import</a> <a id="15701" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15726" class="Keyword">open</a> <a id="15731" class="Keyword">import</a> <a id="15738" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15767" class="Keyword">open</a> <a id="15772" class="Keyword">import</a> <a id="15779" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15804" class="Keyword">open</a> <a id="15809" class="Keyword">import</a> <a id="15816" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15837" class="Keyword">open</a> <a id="15842" class="Keyword">import</a> <a id="15849" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="15873" class="Keyword">open</a> <a id="15878" class="Keyword">import</a> <a id="15885" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="15905" class="Keyword">open</a> <a id="15910" class="Keyword">import</a> <a id="15917" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="15951" class="Keyword">open</a> <a id="15956" class="Keyword">import</a> <a id="15963" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16001" class="Keyword">open</a> <a id="16006" class="Keyword">import</a> <a id="16013" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16041" class="Keyword">open</a> <a id="16046" class="Keyword">import</a> <a id="16053" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16077" class="Keyword">open</a> <a id="16082" class="Keyword">import</a> <a id="16089" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16116" class="Keyword">open</a> <a id="16121" class="Keyword">import</a> <a id="16128" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16163" class="Keyword">open</a> <a id="16168" class="Keyword">import</a> <a id="16175" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16196" class="Keyword">open</a> <a id="16201" class="Keyword">import</a> <a id="16208" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16244" class="Keyword">open</a> <a id="16249" class="Keyword">import</a> <a id="16256" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16301" class="Keyword">open</a> <a id="16306" class="Keyword">import</a> <a id="16313" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16359" class="Keyword">open</a> <a id="16364" class="Keyword">import</a> <a id="16371" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16411" class="Keyword">open</a> <a id="16416" class="Keyword">import</a> <a id="16423" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16453" class="Keyword">open</a> <a id="16458" class="Keyword">import</a> <a id="16465" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16502" class="Keyword">open</a> <a id="16507" class="Keyword">import</a> <a id="16514" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16538" class="Keyword">open</a> <a id="16543" class="Keyword">import</a> <a id="16550" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16571" class="Keyword">open</a> <a id="16576" class="Keyword">import</a> <a id="16583" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16618" class="Keyword">open</a> <a id="16623" class="Keyword">import</a> <a id="16630" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16667" class="Keyword">open</a> <a id="16672" class="Keyword">import</a> <a id="16679" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16728" class="Keyword">open</a> <a id="16733" class="Keyword">import</a> <a id="16740" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16773" class="Keyword">open</a> <a id="16778" class="Keyword">import</a> <a id="16785" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16808" class="Keyword">open</a> <a id="16813" class="Keyword">import</a> <a id="16820" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="16843" class="Keyword">open</a> <a id="16848" class="Keyword">import</a> <a id="16855" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="16878" class="Keyword">open</a> <a id="16883" class="Keyword">import</a> <a id="16890" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="16918" class="Keyword">open</a> <a id="16923" class="Keyword">import</a> <a id="16930" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="16950" class="Keyword">open</a> <a id="16955" class="Keyword">import</a> <a id="16962" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="16983" class="Keyword">open</a> <a id="16988" class="Keyword">import</a> <a id="16995" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17026" class="Keyword">open</a> <a id="17031" class="Keyword">import</a> <a id="17038" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17065" class="Keyword">open</a> <a id="17070" class="Keyword">import</a> <a id="17077" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17093" class="Keyword">open</a> <a id="17098" class="Keyword">import</a> <a id="17105" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17136" class="Keyword">open</a> <a id="17141" class="Keyword">import</a> <a id="17148" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17165" class="Keyword">open</a> <a id="17170" class="Keyword">import</a> <a id="17177" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17199" class="Keyword">open</a> <a id="17204" class="Keyword">import</a> <a id="17211" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17238" class="Keyword">open</a> <a id="17243" class="Keyword">import</a> <a id="17250" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17273" class="Keyword">open</a> <a id="17278" class="Keyword">import</a> <a id="17285" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17312" class="Keyword">open</a> <a id="17317" class="Keyword">import</a> <a id="17324" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17357" class="Keyword">open</a> <a id="17362" class="Keyword">import</a> <a id="17369" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17409" class="Keyword">open</a> <a id="17414" class="Keyword">import</a> <a id="17421" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17442" class="Keyword">open</a> <a id="17447" class="Keyword">import</a> <a id="17454" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17483" class="Keyword">open</a> <a id="17488" class="Keyword">import</a> <a id="17495" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17533" class="Keyword">open</a> <a id="17538" class="Keyword">import</a> <a id="17545" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17565" class="Keyword">open</a> <a id="17570" class="Keyword">import</a> <a id="17577" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17601" class="Keyword">open</a> <a id="17606" class="Keyword">import</a> <a id="17613" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17640" class="Keyword">open</a> <a id="17645" class="Keyword">import</a> <a id="17652" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17684" class="Keyword">open</a> <a id="17689" class="Keyword">import</a> <a id="17696" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17726" class="Keyword">open</a> <a id="17731" class="Keyword">import</a> <a id="17738" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17764" class="Keyword">open</a> <a id="17769" class="Keyword">import</a> <a id="17776" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17803" class="Keyword">open</a> <a id="17808" class="Keyword">import</a> <a id="17815" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="17844" class="Keyword">open</a> <a id="17849" class="Keyword">import</a> <a id="17856" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="17879" class="Keyword">open</a> <a id="17884" class="Keyword">import</a> <a id="17891" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="17942" class="Keyword">open</a> <a id="17947" class="Keyword">import</a> <a id="17954" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="17997" class="Keyword">open</a> <a id="18002" class="Keyword">import</a> <a id="18009" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18057" class="Keyword">open</a> <a id="18062" class="Keyword">import</a> <a id="18069" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18107" class="Keyword">open</a> <a id="18112" class="Keyword">import</a> <a id="18119" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18156" class="Keyword">open</a> <a id="18161" class="Keyword">import</a> <a id="18168" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18185" class="Keyword">open</a> <a id="18190" class="Keyword">import</a> <a id="18197" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18225" class="Keyword">open</a> <a id="18230" class="Keyword">import</a> <a id="18237" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18273" class="Keyword">open</a> <a id="18278" class="Keyword">import</a> <a id="18285" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18323" class="Keyword">open</a> <a id="18328" class="Keyword">import</a> <a id="18335" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18368" class="Keyword">open</a> <a id="18373" class="Keyword">import</a> <a id="18380" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18401" class="Keyword">open</a> <a id="18406" class="Keyword">import</a> <a id="18413" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18467" class="Keyword">open</a> <a id="18472" class="Keyword">import</a> <a id="18479" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18501" class="Keyword">open</a> <a id="18506" class="Keyword">import</a> <a id="18513" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18548" class="Keyword">open</a> <a id="18553" class="Keyword">import</a> <a id="18560" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18590" class="Keyword">open</a> <a id="18595" class="Keyword">import</a> <a id="18602" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18641" class="Keyword">open</a> <a id="18646" class="Keyword">import</a> <a id="18653" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18707" class="Keyword">open</a> <a id="18712" class="Keyword">import</a> <a id="18719" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18765" class="Keyword">open</a> <a id="18770" class="Keyword">import</a> <a id="18777" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18828" class="Keyword">open</a> <a id="18833" class="Keyword">import</a> <a id="18840" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="18881" class="Keyword">open</a> <a id="18886" class="Keyword">import</a> <a id="18893" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="18938" class="Keyword">open</a> <a id="18943" class="Keyword">import</a> <a id="18950" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="18995" class="Keyword">open</a> <a id="19000" class="Keyword">import</a> <a id="19007" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19043" class="Keyword">open</a> <a id="19048" class="Keyword">import</a> <a id="19055" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19091" class="Keyword">open</a> <a id="19096" class="Keyword">import</a> <a id="19103" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19168" class="Keyword">open</a> <a id="19173" class="Keyword">import</a> <a id="19180" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19235" class="Keyword">open</a> <a id="19240" class="Keyword">import</a> <a id="19247" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19287" class="Keyword">open</a> <a id="19292" class="Keyword">import</a> <a id="19299" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19343" class="Keyword">open</a> <a id="19348" class="Keyword">import</a> <a id="19355" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19400" class="Keyword">open</a> <a id="19405" class="Keyword">import</a> <a id="19412" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19453" class="Keyword">open</a> <a id="19458" class="Keyword">import</a> <a id="19465" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19505" class="Keyword">open</a> <a id="19510" class="Keyword">import</a> <a id="19517" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19544" class="Keyword">open</a> <a id="19549" class="Keyword">import</a> <a id="19556" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19592" class="Keyword">open</a> <a id="19597" class="Keyword">import</a> <a id="19604" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19631" class="Keyword">open</a> <a id="19636" class="Keyword">import</a> <a id="19643" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19680" class="Keyword">open</a> <a id="19685" class="Keyword">import</a> <a id="19692" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19720" class="Keyword">open</a> <a id="19725" class="Keyword">import</a> <a id="19732" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19751" class="Keyword">open</a> <a id="19756" class="Keyword">import</a> <a id="19763" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19803" class="Keyword">open</a> <a id="19808" class="Keyword">import</a> <a id="19815" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19847" class="Keyword">open</a> <a id="19852" class="Keyword">import</a> <a id="19859" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="19907" class="Keyword">open</a> <a id="19912" class="Keyword">import</a> <a id="19919" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="19942" class="Keyword">open</a> <a id="19947" class="Keyword">import</a> <a id="19954" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="19978" class="Keyword">open</a> <a id="19983" class="Keyword">import</a> <a id="19990" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20030" class="Keyword">open</a> <a id="20035" class="Keyword">import</a> <a id="20042" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20085" class="Keyword">open</a> <a id="20090" class="Keyword">import</a> <a id="20097" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20131" class="Keyword">open</a> <a id="20136" class="Keyword">import</a> <a id="20143" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20175" class="Keyword">open</a> <a id="20180" class="Keyword">import</a> <a id="20187" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20217" class="Keyword">open</a> <a id="20222" class="Keyword">import</a> <a id="20229" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20263" class="Keyword">open</a> <a id="20268" class="Keyword">import</a> <a id="20275" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20310" class="Keyword">open</a> <a id="20315" class="Keyword">import</a> <a id="20322" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20359" class="Keyword">open</a> <a id="20364" class="Keyword">import</a> <a id="20371" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20398" class="Keyword">open</a> <a id="20403" class="Keyword">import</a> <a id="20410" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20438" class="Keyword">open</a> <a id="20443" class="Keyword">import</a> <a id="20450" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20499" class="Keyword">open</a> <a id="20504" class="Keyword">import</a> <a id="20511" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20557" class="Keyword">open</a> <a id="20562" class="Keyword">import</a> <a id="20569" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20609" class="Keyword">open</a> <a id="20614" class="Keyword">import</a> <a id="20621" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20659" class="Keyword">open</a> <a id="20664" class="Keyword">import</a> <a id="20671" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20700" class="Keyword">open</a> <a id="20705" class="Keyword">import</a> <a id="20712" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20742" class="Keyword">open</a> <a id="20747" class="Keyword">import</a> <a id="20754" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20785" class="Keyword">open</a> <a id="20790" class="Keyword">import</a> <a id="20797" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="20837" class="Keyword">open</a> <a id="20842" class="Keyword">import</a> <a id="20849" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="20875" class="Keyword">open</a> <a id="20880" class="Keyword">import</a> <a id="20887" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="20942" class="Keyword">open</a> <a id="20947" class="Keyword">import</a> <a id="20954" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21005" class="Keyword">open</a> <a id="21010" class="Keyword">import</a> <a id="21017" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21062" class="Keyword">open</a> <a id="21067" class="Keyword">import</a> <a id="21074" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21128" class="Keyword">open</a> <a id="21133" class="Keyword">import</a> <a id="21140" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21167" class="Keyword">open</a> <a id="21172" class="Keyword">import</a> <a id="21179" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21212" class="Keyword">open</a> <a id="21217" class="Keyword">import</a> <a id="21224" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21255" class="Keyword">open</a> <a id="21260" class="Keyword">import</a> <a id="21267" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21304" class="Keyword">open</a> <a id="21309" class="Keyword">import</a> <a id="21316" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21341" class="Keyword">open</a> <a id="21346" class="Keyword">import</a> <a id="21353" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21385" class="Keyword">open</a> <a id="21390" class="Keyword">import</a> <a id="21397" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21432" class="Keyword">open</a> <a id="21437" class="Keyword">import</a> <a id="21444" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21473" class="Keyword">open</a> <a id="21478" class="Keyword">import</a> <a id="21485" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21511" class="Keyword">open</a> <a id="21516" class="Keyword">import</a> <a id="21523" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21551" class="Keyword">open</a> <a id="21556" class="Keyword">import</a> <a id="21563" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21588" class="Keyword">open</a> <a id="21593" class="Keyword">import</a> <a id="21600" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21621" class="Keyword">open</a> <a id="21626" class="Keyword">import</a> <a id="21633" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21669" class="Keyword">open</a> <a id="21674" class="Keyword">import</a> <a id="21681" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21724" class="Keyword">open</a> <a id="21729" class="Keyword">import</a> <a id="21736" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21761" class="Keyword">open</a> <a id="21766" class="Keyword">import</a> <a id="21773" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21804" class="Keyword">open</a> <a id="21809" class="Keyword">import</a> <a id="21816" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21848" class="Keyword">open</a> <a id="21853" class="Keyword">import</a> <a id="21860" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="21894" class="Keyword">open</a> <a id="21899" class="Keyword">import</a> <a id="21906" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="21962" class="Keyword">open</a> <a id="21967" class="Keyword">import</a> <a id="21974" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22027" class="Keyword">open</a> <a id="22032" class="Keyword">import</a> <a id="22039" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22066" class="Keyword">open</a> <a id="22071" class="Keyword">import</a> <a id="22078" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22123" class="Keyword">open</a> <a id="22128" class="Keyword">import</a> <a id="22135" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22197" class="Keyword">open</a> <a id="22202" class="Keyword">import</a> <a id="22209" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22222" class="Keyword">open</a> <a id="22227" class="Keyword">import</a> <a id="22234" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22275" class="Keyword">open</a> <a id="22280" class="Keyword">import</a> <a id="22287" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22316" class="Keyword">open</a> <a id="22321" class="Keyword">import</a> <a id="22328" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22373" class="Keyword">open</a> <a id="22378" class="Keyword">import</a> <a id="22385" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22429" class="Keyword">open</a> <a id="22434" class="Keyword">import</a> <a id="22441" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="22468" class="Keyword">open</a> <a id="22473" class="Keyword">import</a> <a id="22480" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="22521" class="Keyword">open</a> <a id="22526" class="Keyword">import</a> <a id="22533" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="22556" class="Keyword">open</a> <a id="22561" class="Keyword">import</a> <a id="22568" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="22617" class="Keyword">open</a> <a id="22622" class="Keyword">import</a> <a id="22629" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="22668" class="Keyword">open</a> <a id="22673" class="Keyword">import</a> <a id="22680" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="22721" class="Keyword">open</a> <a id="22726" class="Keyword">import</a> <a id="22733" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22777" class="Keyword">open</a> <a id="22782" class="Keyword">import</a> <a id="22789" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22826" class="Keyword">open</a> <a id="22831" class="Keyword">import</a> <a id="22838" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="22860" class="Keyword">open</a> <a id="22865" class="Keyword">import</a> <a id="22872" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="22902" class="Keyword">open</a> <a id="22907" class="Keyword">import</a> <a id="22914" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="22953" class="Keyword">open</a> <a id="22958" class="Keyword">import</a> <a id="22965" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="23003" class="Keyword">open</a> <a id="23008" class="Keyword">import</a> <a id="23015" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="23046" class="Keyword">open</a> <a id="23051" class="Keyword">import</a> <a id="23058" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="23085" class="Keyword">open</a> <a id="23090" class="Keyword">import</a> <a id="23097" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="23155" class="Keyword">open</a> <a id="23160" class="Keyword">import</a> <a id="23167" href="group-theory.html" class="Module">group-theory</a>
<a id="23180" class="Keyword">open</a> <a id="23185" class="Keyword">import</a> <a id="23192" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="23220" class="Keyword">open</a> <a id="23225" class="Keyword">import</a> <a id="23232" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="23263" class="Keyword">open</a> <a id="23268" class="Keyword">import</a> <a id="23275" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="23311" class="Keyword">open</a> <a id="23316" class="Keyword">import</a> <a id="23323" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="23374" class="Keyword">open</a> <a id="23379" class="Keyword">import</a> <a id="23386" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="23419" class="Keyword">open</a> <a id="23424" class="Keyword">import</a> <a id="23431" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="23478" class="Keyword">open</a> <a id="23483" class="Keyword">import</a> <a id="23490" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="23529" class="Keyword">open</a> <a id="23534" class="Keyword">import</a> <a id="23541" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="23581" class="Keyword">open</a> <a id="23586" class="Keyword">import</a> <a id="23593" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="23636" class="Keyword">open</a> <a id="23641" class="Keyword">import</a> <a id="23648" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="23680" class="Keyword">open</a> <a id="23685" class="Keyword">import</a> <a id="23692" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="23728" class="Keyword">open</a> <a id="23733" class="Keyword">import</a> <a id="23740" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="23769" class="Keyword">open</a> <a id="23774" class="Keyword">import</a> <a id="23781" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="23814" class="Keyword">open</a> <a id="23819" class="Keyword">import</a> <a id="23826" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="23862" class="Keyword">open</a> <a id="23867" class="Keyword">import</a> <a id="23874" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="23903" class="Keyword">open</a> <a id="23908" class="Keyword">import</a> <a id="23915" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="23947" class="Keyword">open</a> <a id="23952" class="Keyword">import</a> <a id="23959" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="23984" class="Keyword">open</a> <a id="23989" class="Keyword">import</a> <a id="23996" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="24027" class="Keyword">open</a> <a id="24032" class="Keyword">import</a> <a id="24039" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="24086" class="Keyword">open</a> <a id="24091" class="Keyword">import</a> <a id="24098" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="24131" class="Keyword">open</a> <a id="24136" class="Keyword">import</a> <a id="24143" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="24183" class="Keyword">open</a> <a id="24188" class="Keyword">import</a> <a id="24195" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="24232" class="Keyword">open</a> <a id="24237" class="Keyword">import</a> <a id="24244" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="24280" class="Keyword">open</a> <a id="24285" class="Keyword">import</a> <a id="24292" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="24324" class="Keyword">open</a> <a id="24329" class="Keyword">import</a> <a id="24336" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="24363" class="Keyword">open</a> <a id="24368" class="Keyword">import</a> <a id="24375" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="24395" class="Keyword">open</a> <a id="24400" class="Keyword">import</a> <a id="24407" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="24434" class="Keyword">open</a> <a id="24439" class="Keyword">import</a> <a id="24446" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="24488" class="Keyword">open</a> <a id="24493" class="Keyword">import</a> <a id="24500" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="24547" class="Keyword">open</a> <a id="24552" class="Keyword">import</a> <a id="24559" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="24600" class="Keyword">open</a> <a id="24605" class="Keyword">import</a> <a id="24612" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="24646" class="Keyword">open</a> <a id="24651" class="Keyword">import</a> <a id="24658" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="24693" class="Keyword">open</a> <a id="24698" class="Keyword">import</a> <a id="24705" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="24743" class="Keyword">open</a> <a id="24748" class="Keyword">import</a> <a id="24755" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="24787" class="Keyword">open</a> <a id="24792" class="Keyword">import</a> <a id="24799" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="24840" class="Keyword">open</a> <a id="24845" class="Keyword">import</a> <a id="24852" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="24893" class="Keyword">open</a> <a id="24898" class="Keyword">import</a> <a id="24905" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="24945" class="Keyword">open</a> <a id="24950" class="Keyword">import</a> <a id="24957" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="24990" class="Keyword">open</a> <a id="24995" class="Keyword">import</a> <a id="25002" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="25039" class="Keyword">open</a> <a id="25044" class="Keyword">import</a> <a id="25051" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="25096" class="Keyword">open</a> <a id="25101" class="Keyword">import</a> <a id="25108" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="25136" class="Keyword">open</a> <a id="25141" class="Keyword">import</a> <a id="25148" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="25169" class="Keyword">open</a> <a id="25174" class="Keyword">import</a> <a id="25181" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="25215" class="Keyword">open</a> <a id="25220" class="Keyword">import</a> <a id="25227" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="25261" class="Keyword">open</a> <a id="25266" class="Keyword">import</a> <a id="25273" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="25308" class="Keyword">open</a> <a id="25313" class="Keyword">import</a> <a id="25320" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="25362" class="Keyword">open</a> <a id="25367" class="Keyword">import</a> <a id="25374" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="25409" class="Keyword">open</a> <a id="25414" class="Keyword">import</a> <a id="25421" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="25460" class="Keyword">open</a> <a id="25465" class="Keyword">import</a> <a id="25472" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="25509" class="Keyword">open</a> <a id="25514" class="Keyword">import</a> <a id="25521" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="25545" class="Keyword">open</a> <a id="25550" class="Keyword">import</a> <a id="25557" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="25582" class="Keyword">open</a> <a id="25587" class="Keyword">import</a> <a id="25594" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="25625" class="Keyword">open</a> <a id="25630" class="Keyword">import</a> <a id="25637" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="25688" class="Keyword">open</a> <a id="25693" class="Keyword">import</a> <a id="25700" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="25723" class="Keyword">open</a> <a id="25728" class="Keyword">import</a> <a id="25735" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="25783" class="Keyword">open</a> <a id="25788" class="Keyword">import</a> <a id="25795" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="25825" class="Keyword">open</a> <a id="25830" class="Keyword">import</a> <a id="25837" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="25907" class="Keyword">open</a> <a id="25912" class="Keyword">import</a> <a id="25919" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="25934" class="Keyword">open</a> <a id="25939" class="Keyword">import</a> <a id="25946" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="25979" class="Keyword">open</a> <a id="25984" class="Keyword">import</a> <a id="25991" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="26023" class="Keyword">open</a> <a id="26028" class="Keyword">import</a> <a id="26035" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="26077" class="Keyword">open</a> <a id="26082" class="Keyword">import</a> <a id="26089" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="26127" class="Keyword">open</a> <a id="26132" class="Keyword">import</a> <a id="26139" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="26176" class="Keyword">open</a> <a id="26181" class="Keyword">import</a> <a id="26188" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="26221" class="Keyword">open</a> <a id="26226" class="Keyword">import</a> <a id="26233" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="26257" class="Keyword">open</a> <a id="26262" class="Keyword">import</a> <a id="26269" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="26308" class="Keyword">open</a> <a id="26313" class="Keyword">import</a> <a id="26320" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="26366" class="Keyword">open</a> <a id="26371" class="Keyword">import</a> <a id="26378" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="26423" class="Keyword">open</a> <a id="26428" class="Keyword">import</a> <a id="26435" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="26473" class="Keyword">open</a> <a id="26478" class="Keyword">import</a> <a id="26485" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="26517" class="Keyword">open</a> <a id="26522" class="Keyword">import</a> <a id="26529" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="26582" class="Keyword">open</a> <a id="26587" class="Keyword">import</a> <a id="26594" href="order-theory.html" class="Module">order-theory</a>
<a id="26607" class="Keyword">open</a> <a id="26612" class="Keyword">import</a> <a id="26619" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="26646" class="Keyword">open</a> <a id="26651" class="Keyword">import</a> <a id="26658" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="26688" class="Keyword">open</a> <a id="26693" class="Keyword">import</a> <a id="26700" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="26733" class="Keyword">open</a> <a id="26738" class="Keyword">import</a> <a id="26745" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="26781" class="Keyword">open</a> <a id="26786" class="Keyword">import</a> <a id="26793" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="26820" class="Keyword">open</a> <a id="26825" class="Keyword">import</a> <a id="26832" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="26862" class="Keyword">open</a> <a id="26867" class="Keyword">import</a> <a id="26874" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="26910" class="Keyword">open</a> <a id="26915" class="Keyword">import</a> <a id="26922" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="26964" class="Keyword">open</a> <a id="26969" class="Keyword">import</a> <a id="26976" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="27008" class="Keyword">open</a> <a id="27013" class="Keyword">import</a> <a id="27020" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="27051" class="Keyword">open</a> <a id="27056" class="Keyword">import</a> <a id="27063" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="27089" class="Keyword">open</a> <a id="27094" class="Keyword">import</a> <a id="27101" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="27130" class="Keyword">open</a> <a id="27135" class="Keyword">import</a> <a id="27142" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="27179" class="Keyword">open</a> <a id="27184" class="Keyword">import</a> <a id="27191" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="27231" class="Keyword">open</a> <a id="27236" class="Keyword">import</a> <a id="27243" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="27265" class="Keyword">open</a> <a id="27270" class="Keyword">import</a> <a id="27277" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="27312" class="Keyword">open</a> <a id="27317" class="Keyword">import</a> <a id="27324" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="27362" class="Keyword">open</a> <a id="27367" class="Keyword">import</a> <a id="27374" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="27413" class="Keyword">open</a> <a id="27418" class="Keyword">import</a> <a id="27425" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="27460" class="Keyword">open</a> <a id="27465" class="Keyword">import</a> <a id="27472" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="27507" class="Keyword">open</a> <a id="27512" class="Keyword">import</a> <a id="27519" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="27557" class="Keyword">open</a> <a id="27562" class="Keyword">import</a> <a id="27569" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="27600" class="Keyword">open</a> <a id="27605" class="Keyword">import</a> <a id="27612" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="27654" class="Keyword">open</a> <a id="27659" class="Keyword">import</a> <a id="27666" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="27711" class="Keyword">open</a> <a id="27716" class="Keyword">import</a> <a id="27723" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="27756" class="Keyword">open</a> <a id="27761" class="Keyword">import</a> <a id="27768" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="27788" class="Keyword">open</a> <a id="27793" class="Keyword">import</a> <a id="27800" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="27823" class="Keyword">open</a> <a id="27828" class="Keyword">import</a> <a id="27835" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="27858" class="Keyword">open</a> <a id="27863" class="Keyword">import</a> <a id="27870" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="27896" class="Keyword">open</a> <a id="27901" class="Keyword">import</a> <a id="27908" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="27934" class="Keyword">open</a> <a id="27939" class="Keyword">import</a> <a id="27946" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="28002" class="Keyword">open</a> <a id="28007" class="Keyword">import</a> <a id="28014" href="polytopes.html" class="Module">polytopes</a>
<a id="28024" class="Keyword">open</a> <a id="28029" class="Keyword">import</a> <a id="28036" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="28094" class="Keyword">open</a> <a id="28099" class="Keyword">import</a> <a id="28106" href="ring-theory.html" class="Module">ring-theory</a>
<a id="28118" class="Keyword">open</a> <a id="28123" class="Keyword">import</a> <a id="28130" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="28167" class="Keyword">open</a> <a id="28172" class="Keyword">import</a> <a id="28179" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="28206" class="Keyword">open</a> <a id="28211" class="Keyword">import</a> <a id="28218" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="28250" class="Keyword">open</a> <a id="28255" class="Keyword">import</a> <a id="28262" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="28308" class="Keyword">open</a> <a id="28313" class="Keyword">import</a> <a id="28320" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="28345" class="Keyword">open</a> <a id="28350" class="Keyword">import</a> <a id="28357" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="28400" class="Keyword">open</a> <a id="28405" class="Keyword">import</a> <a id="28412" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="28450" class="Keyword">open</a> <a id="28455" class="Keyword">import</a> <a id="28462" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="28493" class="Keyword">open</a> <a id="28498" class="Keyword">import</a> <a id="28505" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="28537" class="Keyword">open</a> <a id="28542" class="Keyword">import</a> <a id="28549" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="28575" class="Keyword">open</a> <a id="28580" class="Keyword">import</a> <a id="28587" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="28616" class="Keyword">open</a> <a id="28621" class="Keyword">import</a> <a id="28628" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="28665" class="Keyword">open</a> <a id="28670" class="Keyword">import</a> <a id="28677" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="28706" class="Keyword">open</a> <a id="28711" class="Keyword">import</a> <a id="28718" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="28745" class="Keyword">open</a> <a id="28750" class="Keyword">import</a> <a id="28757" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="28794" class="Keyword">open</a> <a id="28799" class="Keyword">import</a> <a id="28806" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="28833" class="Keyword">open</a> <a id="28838" class="Keyword">import</a> <a id="28845" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="28878" class="Keyword">open</a> <a id="28883" class="Keyword">import</a> <a id="28890" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="28908" class="Keyword">open</a> <a id="28913" class="Keyword">import</a> <a id="28920" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="28974" class="Keyword">open</a> <a id="28979" class="Keyword">import</a> <a id="28986" href="set-theory.html" class="Module">set-theory</a>
<a id="28997" class="Keyword">open</a> <a id="29002" class="Keyword">import</a> <a id="29009" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="29035" class="Keyword">open</a> <a id="29040" class="Keyword">import</a> <a id="29047" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="29109" class="Keyword">open</a> <a id="29114" class="Keyword">import</a> <a id="29121" href="structured-types.html" class="Module">structured-types</a>
<a id="29138" class="Keyword">open</a> <a id="29143" class="Keyword">import</a> <a id="29150" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="29194" class="Keyword">open</a> <a id="29199" class="Keyword">import</a> <a id="29206" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="29270" class="Keyword">open</a> <a id="29275" class="Keyword">import</a> <a id="29282" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="29328" class="Keyword">open</a> <a id="29333" class="Keyword">import</a> <a id="29340" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="29364" class="Keyword">open</a> <a id="29369" class="Keyword">import</a> <a id="29376" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="29445" class="Keyword">open</a> <a id="29450" class="Keyword">import</a> <a id="29457" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="29491" class="Keyword">open</a> <a id="29496" class="Keyword">import</a> <a id="29503" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="29564" class="Keyword">open</a> <a id="29569" class="Keyword">import</a> <a id="29576" href="structured-types.morphisms-wild-unital-magmas.html" class="Module">structured-types.morphisms-wild-unital-magmas</a>
<a id="29622" class="Keyword">open</a> <a id="29627" class="Keyword">import</a> <a id="29634" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="29679" class="Keyword">open</a> <a id="29684" class="Keyword">import</a> <a id="29691" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="29729" class="Keyword">open</a> <a id="29734" class="Keyword">import</a> <a id="29741" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="29784" class="Keyword">open</a> <a id="29789" class="Keyword">import</a> <a id="29796" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="29832" class="Keyword">open</a> <a id="29837" class="Keyword">import</a> <a id="29844" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="29874" class="Keyword">open</a> <a id="29879" class="Keyword">import</a> <a id="29886" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="29917" class="Keyword">open</a> <a id="29922" class="Keyword">import</a> <a id="29929" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="29980" class="Keyword">open</a> <a id="29985" class="Keyword">import</a> <a id="29992" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="30047" class="Keyword">open</a> <a id="30052" class="Keyword">import</a> <a id="30059" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="30088" class="Keyword">open</a> <a id="30093" class="Keyword">import</a> <a id="30100" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="30128" class="Keyword">open</a> <a id="30133" class="Keyword">import</a> <a id="30140" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="30170" class="Keyword">open</a> <a id="30175" class="Keyword">import</a> <a id="30182" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="30216" class="Keyword">open</a> <a id="30221" class="Keyword">import</a> <a id="30228" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
<a id="30261" class="Keyword">open</a> <a id="30266" class="Keyword">import</a> <a id="30273" href="structured-types.wild-unital-magmas.html" class="Module">structured-types.wild-unital-magmas</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="30352" class="Keyword">open</a> <a id="30357" class="Keyword">import</a> <a id="30364" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="30390" class="Keyword">open</a> <a id="30395" class="Keyword">import</a> <a id="30402" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="30441" class="Keyword">open</a> <a id="30446" class="Keyword">import</a> <a id="30453" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="30491" class="Keyword">open</a> <a id="30496" class="Keyword">import</a> <a id="30503" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="30549" class="Keyword">open</a> <a id="30554" class="Keyword">import</a> <a id="30561" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="30598" class="Keyword">open</a> <a id="30603" class="Keyword">import</a> <a id="30610" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="30650" class="Keyword">open</a> <a id="30655" class="Keyword">import</a> <a id="30662" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="30701" class="Keyword">open</a> <a id="30706" class="Keyword">import</a> <a id="30713" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="30746" class="Keyword">open</a> <a id="30751" class="Keyword">import</a> <a id="30758" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="30793" class="Keyword">open</a> <a id="30798" class="Keyword">import</a> <a id="30805" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="30844" class="Keyword">open</a> <a id="30849" class="Keyword">import</a> <a id="30856" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="30901" class="Keyword">open</a> <a id="30906" class="Keyword">import</a> <a id="30913" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="30965" class="Keyword">open</a> <a id="30970" class="Keyword">import</a> <a id="30977" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="31030" class="Keyword">open</a> <a id="31035" class="Keyword">import</a> <a id="31042" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="31090" class="Keyword">open</a> <a id="31095" class="Keyword">import</a> <a id="31102" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="31142" class="Keyword">open</a> <a id="31147" class="Keyword">import</a> <a id="31154" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="31201" class="Keyword">open</a> <a id="31206" class="Keyword">import</a> <a id="31213" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="31254" class="Keyword">open</a> <a id="31259" class="Keyword">import</a> <a id="31266" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="31304" class="Keyword">open</a> <a id="31309" class="Keyword">import</a> <a id="31316" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="31361" class="Keyword">open</a> <a id="31366" class="Keyword">import</a> <a id="31373" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="31422" class="Keyword">open</a> <a id="31427" class="Keyword">import</a> <a id="31434" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="31511" class="Keyword">open</a> <a id="31516" class="Keyword">import</a> <a id="31523" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="31575" class="Keyword">open</a> <a id="31580" class="Keyword">import</a> <a id="31587" href="type-theories.html" class="Module">type-theories</a>
<a id="31601" class="Keyword">open</a> <a id="31606" class="Keyword">import</a> <a id="31613" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="31655" class="Keyword">open</a> <a id="31660" class="Keyword">import</a> <a id="31667" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="31705" class="Keyword">open</a> <a id="31710" class="Keyword">import</a> <a id="31717" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="31763" class="Keyword">open</a> <a id="31768" class="Keyword">import</a> <a id="31775" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="31822" class="Keyword">open</a> <a id="31827" class="Keyword">import</a> <a id="31834" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="31869" class="Keyword">open</a> <a id="31874" class="Keyword">import</a> <a id="31881" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="31959" class="Keyword">open</a> <a id="31964" class="Keyword">import</a> <a id="31971" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="31995" class="Keyword">open</a> <a id="32000" class="Keyword">import</a> <a id="32007" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="32060" class="Keyword">open</a> <a id="32065" class="Keyword">import</a> <a id="32072" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="32115" class="Keyword">open</a> <a id="32120" class="Keyword">import</a> <a id="32127" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="32167" class="Keyword">open</a> <a id="32172" class="Keyword">import</a> <a id="32179" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="32218" class="Keyword">open</a> <a id="32223" class="Keyword">import</a> <a id="32230" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="32278" class="Keyword">open</a> <a id="32283" class="Keyword">import</a> <a id="32290" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="32337" class="Keyword">open</a> <a id="32342" class="Keyword">import</a> <a id="32349" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="32401" class="Keyword">open</a> <a id="32406" class="Keyword">import</a> <a id="32413" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="32457" class="Keyword">open</a> <a id="32462" class="Keyword">import</a> <a id="32469" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="32509" class="Keyword">open</a> <a id="32514" class="Keyword">import</a> <a id="32521" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="32573" class="Keyword">open</a> <a id="32578" class="Keyword">import</a> <a id="32585" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="32639" class="Keyword">open</a> <a id="32644" class="Keyword">import</a> <a id="32651" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="32699" class="Keyword">open</a> <a id="32704" class="Keyword">import</a> <a id="32711" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="32750" class="Keyword">open</a> <a id="32755" class="Keyword">import</a> <a id="32762" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="32795" class="Keyword">open</a> <a id="32800" class="Keyword">import</a> <a id="32807" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="32837" class="Keyword">open</a> <a id="32842" class="Keyword">import</a> <a id="32849" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="32908" class="Keyword">open</a> <a id="32913" class="Keyword">import</a> <a id="32920" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="32975" class="Keyword">open</a> <a id="32980" class="Keyword">import</a> <a id="32987" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="33034" class="Keyword">open</a> <a id="33039" class="Keyword">import</a> <a id="33046" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="33089" class="Keyword">open</a> <a id="33094" class="Keyword">import</a> <a id="33101" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="33146" class="Keyword">open</a> <a id="33151" class="Keyword">import</a> <a id="33158" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="33207" class="Keyword">open</a> <a id="33212" class="Keyword">import</a> <a id="33219" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="33270" class="Keyword">open</a> <a id="33275" class="Keyword">import</a> <a id="33282" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="33360" class="Keyword">open</a> <a id="33365" class="Keyword">import</a> <a id="33372" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="33412" class="Keyword">open</a> <a id="33417" class="Keyword">import</a> <a id="33424" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="33481" class="Keyword">open</a> <a id="33486" class="Keyword">import</a> <a id="33493" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="33528" class="Keyword">open</a> <a id="33533" class="Keyword">import</a> <a id="33540" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="33586" class="Keyword">open</a> <a id="33591" class="Keyword">import</a> <a id="33598" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="33653" class="Keyword">open</a> <a id="33658" class="Keyword">import</a> <a id="33665" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="33708" class="Keyword">open</a> <a id="33713" class="Keyword">import</a> <a id="33720" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="33779" class="Keyword">open</a> <a id="33784" class="Keyword">import</a> <a id="33791" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="33828" class="Keyword">open</a> <a id="33833" class="Keyword">import</a> <a id="33840" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="33881" class="Keyword">open</a> <a id="33886" class="Keyword">import</a> <a id="33893" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="33932" class="Keyword">open</a> <a id="33937" class="Keyword">import</a> <a id="33944" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="33982" class="Keyword">open</a> <a id="33987" class="Keyword">import</a> <a id="33994" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="34046" class="Keyword">open</a> <a id="34051" class="Keyword">import</a> <a id="34058" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="34103" class="Keyword">open</a> <a id="34108" class="Keyword">import</a> <a id="34115" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="34152" class="Keyword">open</a> <a id="34157" class="Keyword">import</a> <a id="34164" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="34213" class="Keyword">open</a> <a id="34218" class="Keyword">import</a> <a id="34225" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="34264" class="Keyword">open</a> <a id="34269" class="Keyword">import</a> <a id="34276" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="34314" class="Keyword">open</a> <a id="34319" class="Keyword">import</a> <a id="34326" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="34381" class="Keyword">open</a> <a id="34386" class="Keyword">import</a> <a id="34393" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="34432" class="Keyword">open</a> <a id="34437" class="Keyword">import</a> <a id="34444" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="34492" class="Keyword">open</a> <a id="34497" class="Keyword">import</a> <a id="34504" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="34551" class="Keyword">open</a> <a id="34556" class="Keyword">import</a> <a id="34563" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="34601" class="Keyword">open</a> <a id="34606" class="Keyword">import</a> <a id="34613" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="34643" class="Keyword">open</a> <a id="34648" class="Keyword">import</a> <a id="34655" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="34712" class="Keyword">open</a> <a id="34717" class="Keyword">import</a> <a id="34724" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="34778" class="Keyword">open</a> <a id="34783" class="Keyword">import</a> <a id="34790" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="34820" class="Keyword">open</a> <a id="34825" class="Keyword">import</a> <a id="34832" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="34895" class="Keyword">open</a> <a id="34900" class="Keyword">import</a> <a id="34907" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="34950" class="Keyword">open</a> <a id="34955" class="Keyword">import</a> <a id="34962" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="34997" class="Keyword">open</a> <a id="35002" class="Keyword">import</a> <a id="35009" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="35049" class="Keyword">open</a> <a id="35054" class="Keyword">import</a> <a id="35061" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="35106" class="Keyword">open</a> <a id="35111" class="Keyword">import</a> <a id="35118" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="35168" class="Keyword">open</a> <a id="35173" class="Keyword">import</a> <a id="35180" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="35218" class="Keyword">open</a> <a id="35223" class="Keyword">import</a> <a id="35230" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="35279" class="Keyword">open</a> <a id="35284" class="Keyword">import</a> <a id="35291" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="35338" class="Keyword">open</a> <a id="35343" class="Keyword">import</a> <a id="35350" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="35413" class="Keyword">open</a> <a id="35418" class="Keyword">import</a> <a id="35425" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="35457" class="Keyword">open</a> <a id="35462" class="Keyword">import</a> <a id="35469" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="35522" class="Keyword">open</a> <a id="35527" class="Keyword">import</a> <a id="35534" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="35580" class="Keyword">open</a> <a id="35585" class="Keyword">import</a> <a id="35592" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="35638" class="Keyword">open</a> <a id="35643" class="Keyword">import</a> <a id="35650" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="35698" class="Keyword">open</a> <a id="35703" class="Keyword">import</a> <a id="35710" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="35750" class="Keyword">open</a> <a id="35755" class="Keyword">import</a> <a id="35762" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="35807" class="Keyword">open</a> <a id="35812" class="Keyword">import</a> <a id="35819" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>