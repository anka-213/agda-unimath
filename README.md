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
<a id="18501" class="Keyword">open</a> <a id="18506" class="Keyword">import</a> <a id="18513" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18567" class="Keyword">open</a> <a id="18572" class="Keyword">import</a> <a id="18579" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18601" class="Keyword">open</a> <a id="18606" class="Keyword">import</a> <a id="18613" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18648" class="Keyword">open</a> <a id="18653" class="Keyword">import</a> <a id="18660" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18690" class="Keyword">open</a> <a id="18695" class="Keyword">import</a> <a id="18702" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18741" class="Keyword">open</a> <a id="18746" class="Keyword">import</a> <a id="18753" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18807" class="Keyword">open</a> <a id="18812" class="Keyword">import</a> <a id="18819" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18865" class="Keyword">open</a> <a id="18870" class="Keyword">import</a> <a id="18877" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18928" class="Keyword">open</a> <a id="18933" class="Keyword">import</a> <a id="18940" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="18981" class="Keyword">open</a> <a id="18986" class="Keyword">import</a> <a id="18993" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19038" class="Keyword">open</a> <a id="19043" class="Keyword">import</a> <a id="19050" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19095" class="Keyword">open</a> <a id="19100" class="Keyword">import</a> <a id="19107" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19143" class="Keyword">open</a> <a id="19148" class="Keyword">import</a> <a id="19155" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19191" class="Keyword">open</a> <a id="19196" class="Keyword">import</a> <a id="19203" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19268" class="Keyword">open</a> <a id="19273" class="Keyword">import</a> <a id="19280" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19335" class="Keyword">open</a> <a id="19340" class="Keyword">import</a> <a id="19347" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19387" class="Keyword">open</a> <a id="19392" class="Keyword">import</a> <a id="19399" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19443" class="Keyword">open</a> <a id="19448" class="Keyword">import</a> <a id="19455" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19500" class="Keyword">open</a> <a id="19505" class="Keyword">import</a> <a id="19512" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19553" class="Keyword">open</a> <a id="19558" class="Keyword">import</a> <a id="19565" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19605" class="Keyword">open</a> <a id="19610" class="Keyword">import</a> <a id="19617" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19644" class="Keyword">open</a> <a id="19649" class="Keyword">import</a> <a id="19656" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19692" class="Keyword">open</a> <a id="19697" class="Keyword">import</a> <a id="19704" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19731" class="Keyword">open</a> <a id="19736" class="Keyword">import</a> <a id="19743" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19780" class="Keyword">open</a> <a id="19785" class="Keyword">import</a> <a id="19792" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19820" class="Keyword">open</a> <a id="19825" class="Keyword">import</a> <a id="19832" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19851" class="Keyword">open</a> <a id="19856" class="Keyword">import</a> <a id="19863" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19903" class="Keyword">open</a> <a id="19908" class="Keyword">import</a> <a id="19915" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19947" class="Keyword">open</a> <a id="19952" class="Keyword">import</a> <a id="19959" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20007" class="Keyword">open</a> <a id="20012" class="Keyword">import</a> <a id="20019" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20042" class="Keyword">open</a> <a id="20047" class="Keyword">import</a> <a id="20054" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20078" class="Keyword">open</a> <a id="20083" class="Keyword">import</a> <a id="20090" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20130" class="Keyword">open</a> <a id="20135" class="Keyword">import</a> <a id="20142" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20185" class="Keyword">open</a> <a id="20190" class="Keyword">import</a> <a id="20197" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20231" class="Keyword">open</a> <a id="20236" class="Keyword">import</a> <a id="20243" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20275" class="Keyword">open</a> <a id="20280" class="Keyword">import</a> <a id="20287" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20317" class="Keyword">open</a> <a id="20322" class="Keyword">import</a> <a id="20329" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20363" class="Keyword">open</a> <a id="20368" class="Keyword">import</a> <a id="20375" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20410" class="Keyword">open</a> <a id="20415" class="Keyword">import</a> <a id="20422" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20459" class="Keyword">open</a> <a id="20464" class="Keyword">import</a> <a id="20471" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20498" class="Keyword">open</a> <a id="20503" class="Keyword">import</a> <a id="20510" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20538" class="Keyword">open</a> <a id="20543" class="Keyword">import</a> <a id="20550" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20599" class="Keyword">open</a> <a id="20604" class="Keyword">import</a> <a id="20611" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20657" class="Keyword">open</a> <a id="20662" class="Keyword">import</a> <a id="20669" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20709" class="Keyword">open</a> <a id="20714" class="Keyword">import</a> <a id="20721" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20759" class="Keyword">open</a> <a id="20764" class="Keyword">import</a> <a id="20771" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20800" class="Keyword">open</a> <a id="20805" class="Keyword">import</a> <a id="20812" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20842" class="Keyword">open</a> <a id="20847" class="Keyword">import</a> <a id="20854" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20885" class="Keyword">open</a> <a id="20890" class="Keyword">import</a> <a id="20897" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="20937" class="Keyword">open</a> <a id="20942" class="Keyword">import</a> <a id="20949" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="20975" class="Keyword">open</a> <a id="20980" class="Keyword">import</a> <a id="20987" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21042" class="Keyword">open</a> <a id="21047" class="Keyword">import</a> <a id="21054" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21105" class="Keyword">open</a> <a id="21110" class="Keyword">import</a> <a id="21117" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21162" class="Keyword">open</a> <a id="21167" class="Keyword">import</a> <a id="21174" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21228" class="Keyword">open</a> <a id="21233" class="Keyword">import</a> <a id="21240" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21267" class="Keyword">open</a> <a id="21272" class="Keyword">import</a> <a id="21279" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21312" class="Keyword">open</a> <a id="21317" class="Keyword">import</a> <a id="21324" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21355" class="Keyword">open</a> <a id="21360" class="Keyword">import</a> <a id="21367" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21404" class="Keyword">open</a> <a id="21409" class="Keyword">import</a> <a id="21416" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21441" class="Keyword">open</a> <a id="21446" class="Keyword">import</a> <a id="21453" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21485" class="Keyword">open</a> <a id="21490" class="Keyword">import</a> <a id="21497" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21532" class="Keyword">open</a> <a id="21537" class="Keyword">import</a> <a id="21544" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21573" class="Keyword">open</a> <a id="21578" class="Keyword">import</a> <a id="21585" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21611" class="Keyword">open</a> <a id="21616" class="Keyword">import</a> <a id="21623" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21651" class="Keyword">open</a> <a id="21656" class="Keyword">import</a> <a id="21663" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21688" class="Keyword">open</a> <a id="21693" class="Keyword">import</a> <a id="21700" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21721" class="Keyword">open</a> <a id="21726" class="Keyword">import</a> <a id="21733" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21769" class="Keyword">open</a> <a id="21774" class="Keyword">import</a> <a id="21781" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21824" class="Keyword">open</a> <a id="21829" class="Keyword">import</a> <a id="21836" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21861" class="Keyword">open</a> <a id="21866" class="Keyword">import</a> <a id="21873" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21904" class="Keyword">open</a> <a id="21909" class="Keyword">import</a> <a id="21916" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21948" class="Keyword">open</a> <a id="21953" class="Keyword">import</a> <a id="21960" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="21994" class="Keyword">open</a> <a id="21999" class="Keyword">import</a> <a id="22006" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22062" class="Keyword">open</a> <a id="22067" class="Keyword">import</a> <a id="22074" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22127" class="Keyword">open</a> <a id="22132" class="Keyword">import</a> <a id="22139" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22166" class="Keyword">open</a> <a id="22171" class="Keyword">import</a> <a id="22178" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22223" class="Keyword">open</a> <a id="22228" class="Keyword">import</a> <a id="22235" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22297" class="Keyword">open</a> <a id="22302" class="Keyword">import</a> <a id="22309" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22322" class="Keyword">open</a> <a id="22327" class="Keyword">import</a> <a id="22334" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22375" class="Keyword">open</a> <a id="22380" class="Keyword">import</a> <a id="22387" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22416" class="Keyword">open</a> <a id="22421" class="Keyword">import</a> <a id="22428" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22473" class="Keyword">open</a> <a id="22478" class="Keyword">import</a> <a id="22485" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22529" class="Keyword">open</a> <a id="22534" class="Keyword">import</a> <a id="22541" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="22568" class="Keyword">open</a> <a id="22573" class="Keyword">import</a> <a id="22580" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="22621" class="Keyword">open</a> <a id="22626" class="Keyword">import</a> <a id="22633" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="22656" class="Keyword">open</a> <a id="22661" class="Keyword">import</a> <a id="22668" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="22717" class="Keyword">open</a> <a id="22722" class="Keyword">import</a> <a id="22729" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="22768" class="Keyword">open</a> <a id="22773" class="Keyword">import</a> <a id="22780" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="22821" class="Keyword">open</a> <a id="22826" class="Keyword">import</a> <a id="22833" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22877" class="Keyword">open</a> <a id="22882" class="Keyword">import</a> <a id="22889" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22926" class="Keyword">open</a> <a id="22931" class="Keyword">import</a> <a id="22938" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="22960" class="Keyword">open</a> <a id="22965" class="Keyword">import</a> <a id="22972" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23002" class="Keyword">open</a> <a id="23007" class="Keyword">import</a> <a id="23014" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="23053" class="Keyword">open</a> <a id="23058" class="Keyword">import</a> <a id="23065" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="23103" class="Keyword">open</a> <a id="23108" class="Keyword">import</a> <a id="23115" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="23146" class="Keyword">open</a> <a id="23151" class="Keyword">import</a> <a id="23158" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="23185" class="Keyword">open</a> <a id="23190" class="Keyword">import</a> <a id="23197" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="23255" class="Keyword">open</a> <a id="23260" class="Keyword">import</a> <a id="23267" href="group-theory.html" class="Module">group-theory</a>
<a id="23280" class="Keyword">open</a> <a id="23285" class="Keyword">import</a> <a id="23292" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="23320" class="Keyword">open</a> <a id="23325" class="Keyword">import</a> <a id="23332" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="23363" class="Keyword">open</a> <a id="23368" class="Keyword">import</a> <a id="23375" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="23411" class="Keyword">open</a> <a id="23416" class="Keyword">import</a> <a id="23423" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="23474" class="Keyword">open</a> <a id="23479" class="Keyword">import</a> <a id="23486" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="23519" class="Keyword">open</a> <a id="23524" class="Keyword">import</a> <a id="23531" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="23578" class="Keyword">open</a> <a id="23583" class="Keyword">import</a> <a id="23590" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="23629" class="Keyword">open</a> <a id="23634" class="Keyword">import</a> <a id="23641" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="23681" class="Keyword">open</a> <a id="23686" class="Keyword">import</a> <a id="23693" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="23736" class="Keyword">open</a> <a id="23741" class="Keyword">import</a> <a id="23748" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="23780" class="Keyword">open</a> <a id="23785" class="Keyword">import</a> <a id="23792" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="23828" class="Keyword">open</a> <a id="23833" class="Keyword">import</a> <a id="23840" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="23869" class="Keyword">open</a> <a id="23874" class="Keyword">import</a> <a id="23881" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="23914" class="Keyword">open</a> <a id="23919" class="Keyword">import</a> <a id="23926" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="23962" class="Keyword">open</a> <a id="23967" class="Keyword">import</a> <a id="23974" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="24003" class="Keyword">open</a> <a id="24008" class="Keyword">import</a> <a id="24015" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="24047" class="Keyword">open</a> <a id="24052" class="Keyword">import</a> <a id="24059" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="24084" class="Keyword">open</a> <a id="24089" class="Keyword">import</a> <a id="24096" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="24127" class="Keyword">open</a> <a id="24132" class="Keyword">import</a> <a id="24139" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="24186" class="Keyword">open</a> <a id="24191" class="Keyword">import</a> <a id="24198" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="24231" class="Keyword">open</a> <a id="24236" class="Keyword">import</a> <a id="24243" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="24283" class="Keyword">open</a> <a id="24288" class="Keyword">import</a> <a id="24295" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="24332" class="Keyword">open</a> <a id="24337" class="Keyword">import</a> <a id="24344" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="24380" class="Keyword">open</a> <a id="24385" class="Keyword">import</a> <a id="24392" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="24424" class="Keyword">open</a> <a id="24429" class="Keyword">import</a> <a id="24436" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="24463" class="Keyword">open</a> <a id="24468" class="Keyword">import</a> <a id="24475" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="24495" class="Keyword">open</a> <a id="24500" class="Keyword">import</a> <a id="24507" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="24534" class="Keyword">open</a> <a id="24539" class="Keyword">import</a> <a id="24546" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="24588" class="Keyword">open</a> <a id="24593" class="Keyword">import</a> <a id="24600" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="24647" class="Keyword">open</a> <a id="24652" class="Keyword">import</a> <a id="24659" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="24700" class="Keyword">open</a> <a id="24705" class="Keyword">import</a> <a id="24712" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="24746" class="Keyword">open</a> <a id="24751" class="Keyword">import</a> <a id="24758" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="24793" class="Keyword">open</a> <a id="24798" class="Keyword">import</a> <a id="24805" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="24843" class="Keyword">open</a> <a id="24848" class="Keyword">import</a> <a id="24855" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="24887" class="Keyword">open</a> <a id="24892" class="Keyword">import</a> <a id="24899" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="24940" class="Keyword">open</a> <a id="24945" class="Keyword">import</a> <a id="24952" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="24993" class="Keyword">open</a> <a id="24998" class="Keyword">import</a> <a id="25005" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="25045" class="Keyword">open</a> <a id="25050" class="Keyword">import</a> <a id="25057" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="25090" class="Keyword">open</a> <a id="25095" class="Keyword">import</a> <a id="25102" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="25139" class="Keyword">open</a> <a id="25144" class="Keyword">import</a> <a id="25151" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="25181" class="Keyword">open</a> <a id="25186" class="Keyword">import</a> <a id="25193" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="25238" class="Keyword">open</a> <a id="25243" class="Keyword">import</a> <a id="25250" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="25278" class="Keyword">open</a> <a id="25283" class="Keyword">import</a> <a id="25290" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="25311" class="Keyword">open</a> <a id="25316" class="Keyword">import</a> <a id="25323" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="25357" class="Keyword">open</a> <a id="25362" class="Keyword">import</a> <a id="25369" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="25403" class="Keyword">open</a> <a id="25408" class="Keyword">import</a> <a id="25415" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="25450" class="Keyword">open</a> <a id="25455" class="Keyword">import</a> <a id="25462" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="25504" class="Keyword">open</a> <a id="25509" class="Keyword">import</a> <a id="25516" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="25551" class="Keyword">open</a> <a id="25556" class="Keyword">import</a> <a id="25563" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="25602" class="Keyword">open</a> <a id="25607" class="Keyword">import</a> <a id="25614" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="25651" class="Keyword">open</a> <a id="25656" class="Keyword">import</a> <a id="25663" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="25687" class="Keyword">open</a> <a id="25692" class="Keyword">import</a> <a id="25699" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="25724" class="Keyword">open</a> <a id="25729" class="Keyword">import</a> <a id="25736" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="25767" class="Keyword">open</a> <a id="25772" class="Keyword">import</a> <a id="25779" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="25830" class="Keyword">open</a> <a id="25835" class="Keyword">import</a> <a id="25842" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="25865" class="Keyword">open</a> <a id="25870" class="Keyword">import</a> <a id="25877" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="25925" class="Keyword">open</a> <a id="25930" class="Keyword">import</a> <a id="25937" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="25967" class="Keyword">open</a> <a id="25972" class="Keyword">import</a> <a id="25979" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="26049" class="Keyword">open</a> <a id="26054" class="Keyword">import</a> <a id="26061" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="26076" class="Keyword">open</a> <a id="26081" class="Keyword">import</a> <a id="26088" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="26121" class="Keyword">open</a> <a id="26126" class="Keyword">import</a> <a id="26133" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="26165" class="Keyword">open</a> <a id="26170" class="Keyword">import</a> <a id="26177" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="26219" class="Keyword">open</a> <a id="26224" class="Keyword">import</a> <a id="26231" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="26269" class="Keyword">open</a> <a id="26274" class="Keyword">import</a> <a id="26281" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="26318" class="Keyword">open</a> <a id="26323" class="Keyword">import</a> <a id="26330" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="26363" class="Keyword">open</a> <a id="26368" class="Keyword">import</a> <a id="26375" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="26399" class="Keyword">open</a> <a id="26404" class="Keyword">import</a> <a id="26411" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="26450" class="Keyword">open</a> <a id="26455" class="Keyword">import</a> <a id="26462" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="26508" class="Keyword">open</a> <a id="26513" class="Keyword">import</a> <a id="26520" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="26565" class="Keyword">open</a> <a id="26570" class="Keyword">import</a> <a id="26577" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="26615" class="Keyword">open</a> <a id="26620" class="Keyword">import</a> <a id="26627" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="26659" class="Keyword">open</a> <a id="26664" class="Keyword">import</a> <a id="26671" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="26724" class="Keyword">open</a> <a id="26729" class="Keyword">import</a> <a id="26736" href="order-theory.html" class="Module">order-theory</a>
<a id="26749" class="Keyword">open</a> <a id="26754" class="Keyword">import</a> <a id="26761" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="26788" class="Keyword">open</a> <a id="26793" class="Keyword">import</a> <a id="26800" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="26830" class="Keyword">open</a> <a id="26835" class="Keyword">import</a> <a id="26842" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="26875" class="Keyword">open</a> <a id="26880" class="Keyword">import</a> <a id="26887" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="26923" class="Keyword">open</a> <a id="26928" class="Keyword">import</a> <a id="26935" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="26962" class="Keyword">open</a> <a id="26967" class="Keyword">import</a> <a id="26974" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="27004" class="Keyword">open</a> <a id="27009" class="Keyword">import</a> <a id="27016" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="27052" class="Keyword">open</a> <a id="27057" class="Keyword">import</a> <a id="27064" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="27106" class="Keyword">open</a> <a id="27111" class="Keyword">import</a> <a id="27118" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="27150" class="Keyword">open</a> <a id="27155" class="Keyword">import</a> <a id="27162" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="27193" class="Keyword">open</a> <a id="27198" class="Keyword">import</a> <a id="27205" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="27231" class="Keyword">open</a> <a id="27236" class="Keyword">import</a> <a id="27243" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="27272" class="Keyword">open</a> <a id="27277" class="Keyword">import</a> <a id="27284" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="27321" class="Keyword">open</a> <a id="27326" class="Keyword">import</a> <a id="27333" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="27373" class="Keyword">open</a> <a id="27378" class="Keyword">import</a> <a id="27385" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="27407" class="Keyword">open</a> <a id="27412" class="Keyword">import</a> <a id="27419" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="27454" class="Keyword">open</a> <a id="27459" class="Keyword">import</a> <a id="27466" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="27504" class="Keyword">open</a> <a id="27509" class="Keyword">import</a> <a id="27516" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="27555" class="Keyword">open</a> <a id="27560" class="Keyword">import</a> <a id="27567" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="27602" class="Keyword">open</a> <a id="27607" class="Keyword">import</a> <a id="27614" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="27649" class="Keyword">open</a> <a id="27654" class="Keyword">import</a> <a id="27661" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="27699" class="Keyword">open</a> <a id="27704" class="Keyword">import</a> <a id="27711" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="27742" class="Keyword">open</a> <a id="27747" class="Keyword">import</a> <a id="27754" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="27796" class="Keyword">open</a> <a id="27801" class="Keyword">import</a> <a id="27808" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="27853" class="Keyword">open</a> <a id="27858" class="Keyword">import</a> <a id="27865" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="27898" class="Keyword">open</a> <a id="27903" class="Keyword">import</a> <a id="27910" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="27930" class="Keyword">open</a> <a id="27935" class="Keyword">import</a> <a id="27942" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="27965" class="Keyword">open</a> <a id="27970" class="Keyword">import</a> <a id="27977" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="28000" class="Keyword">open</a> <a id="28005" class="Keyword">import</a> <a id="28012" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="28038" class="Keyword">open</a> <a id="28043" class="Keyword">import</a> <a id="28050" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="28076" class="Keyword">open</a> <a id="28081" class="Keyword">import</a> <a id="28088" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="28144" class="Keyword">open</a> <a id="28149" class="Keyword">import</a> <a id="28156" href="polytopes.html" class="Module">polytopes</a>
<a id="28166" class="Keyword">open</a> <a id="28171" class="Keyword">import</a> <a id="28178" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="28236" class="Keyword">open</a> <a id="28241" class="Keyword">import</a> <a id="28248" href="ring-theory.html" class="Module">ring-theory</a>
<a id="28260" class="Keyword">open</a> <a id="28265" class="Keyword">import</a> <a id="28272" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="28309" class="Keyword">open</a> <a id="28314" class="Keyword">import</a> <a id="28321" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="28348" class="Keyword">open</a> <a id="28353" class="Keyword">import</a> <a id="28360" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="28392" class="Keyword">open</a> <a id="28397" class="Keyword">import</a> <a id="28404" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="28450" class="Keyword">open</a> <a id="28455" class="Keyword">import</a> <a id="28462" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="28487" class="Keyword">open</a> <a id="28492" class="Keyword">import</a> <a id="28499" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="28542" class="Keyword">open</a> <a id="28547" class="Keyword">import</a> <a id="28554" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="28592" class="Keyword">open</a> <a id="28597" class="Keyword">import</a> <a id="28604" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="28635" class="Keyword">open</a> <a id="28640" class="Keyword">import</a> <a id="28647" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="28679" class="Keyword">open</a> <a id="28684" class="Keyword">import</a> <a id="28691" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="28717" class="Keyword">open</a> <a id="28722" class="Keyword">import</a> <a id="28729" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="28758" class="Keyword">open</a> <a id="28763" class="Keyword">import</a> <a id="28770" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="28807" class="Keyword">open</a> <a id="28812" class="Keyword">import</a> <a id="28819" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="28848" class="Keyword">open</a> <a id="28853" class="Keyword">import</a> <a id="28860" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="28887" class="Keyword">open</a> <a id="28892" class="Keyword">import</a> <a id="28899" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="28936" class="Keyword">open</a> <a id="28941" class="Keyword">import</a> <a id="28948" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="28975" class="Keyword">open</a> <a id="28980" class="Keyword">import</a> <a id="28987" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="29020" class="Keyword">open</a> <a id="29025" class="Keyword">import</a> <a id="29032" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="29050" class="Keyword">open</a> <a id="29055" class="Keyword">import</a> <a id="29062" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="29116" class="Keyword">open</a> <a id="29121" class="Keyword">import</a> <a id="29128" href="set-theory.html" class="Module">set-theory</a>
<a id="29139" class="Keyword">open</a> <a id="29144" class="Keyword">import</a> <a id="29151" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="29177" class="Keyword">open</a> <a id="29182" class="Keyword">import</a> <a id="29189" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="29251" class="Keyword">open</a> <a id="29256" class="Keyword">import</a> <a id="29263" href="structured-types.html" class="Module">structured-types</a>
<a id="29280" class="Keyword">open</a> <a id="29285" class="Keyword">import</a> <a id="29292" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="29327" class="Keyword">open</a> <a id="29332" class="Keyword">import</a> <a id="29339" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="29383" class="Keyword">open</a> <a id="29388" class="Keyword">import</a> <a id="29395" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="29459" class="Keyword">open</a> <a id="29464" class="Keyword">import</a> <a id="29471" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="29517" class="Keyword">open</a> <a id="29522" class="Keyword">import</a> <a id="29529" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="29553" class="Keyword">open</a> <a id="29558" class="Keyword">import</a> <a id="29565" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="29634" class="Keyword">open</a> <a id="29639" class="Keyword">import</a> <a id="29646" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="29691" class="Keyword">open</a> <a id="29696" class="Keyword">import</a> <a id="29703" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="29737" class="Keyword">open</a> <a id="29742" class="Keyword">import</a> <a id="29749" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="29810" class="Keyword">open</a> <a id="29815" class="Keyword">import</a> <a id="29822" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="29867" class="Keyword">open</a> <a id="29872" class="Keyword">import</a> <a id="29879" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="29917" class="Keyword">open</a> <a id="29922" class="Keyword">import</a> <a id="29929" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="29972" class="Keyword">open</a> <a id="29977" class="Keyword">import</a> <a id="29984" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="30020" class="Keyword">open</a> <a id="30025" class="Keyword">import</a> <a id="30032" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="30062" class="Keyword">open</a> <a id="30067" class="Keyword">import</a> <a id="30074" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="30105" class="Keyword">open</a> <a id="30110" class="Keyword">import</a> <a id="30117" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="30168" class="Keyword">open</a> <a id="30173" class="Keyword">import</a> <a id="30180" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="30235" class="Keyword">open</a> <a id="30240" class="Keyword">import</a> <a id="30247" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="30276" class="Keyword">open</a> <a id="30281" class="Keyword">import</a> <a id="30288" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="30316" class="Keyword">open</a> <a id="30321" class="Keyword">import</a> <a id="30328" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="30358" class="Keyword">open</a> <a id="30363" class="Keyword">import</a> <a id="30370" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="30404" class="Keyword">open</a> <a id="30409" class="Keyword">import</a> <a id="30416" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="30492" class="Keyword">open</a> <a id="30497" class="Keyword">import</a> <a id="30504" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="30530" class="Keyword">open</a> <a id="30535" class="Keyword">import</a> <a id="30542" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="30581" class="Keyword">open</a> <a id="30586" class="Keyword">import</a> <a id="30593" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="30631" class="Keyword">open</a> <a id="30636" class="Keyword">import</a> <a id="30643" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="30689" class="Keyword">open</a> <a id="30694" class="Keyword">import</a> <a id="30701" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="30738" class="Keyword">open</a> <a id="30743" class="Keyword">import</a> <a id="30750" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="30790" class="Keyword">open</a> <a id="30795" class="Keyword">import</a> <a id="30802" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="30841" class="Keyword">open</a> <a id="30846" class="Keyword">import</a> <a id="30853" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="30886" class="Keyword">open</a> <a id="30891" class="Keyword">import</a> <a id="30898" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="30933" class="Keyword">open</a> <a id="30938" class="Keyword">import</a> <a id="30945" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="30984" class="Keyword">open</a> <a id="30989" class="Keyword">import</a> <a id="30996" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="31041" class="Keyword">open</a> <a id="31046" class="Keyword">import</a> <a id="31053" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="31105" class="Keyword">open</a> <a id="31110" class="Keyword">import</a> <a id="31117" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="31170" class="Keyword">open</a> <a id="31175" class="Keyword">import</a> <a id="31182" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="31230" class="Keyword">open</a> <a id="31235" class="Keyword">import</a> <a id="31242" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="31282" class="Keyword">open</a> <a id="31287" class="Keyword">import</a> <a id="31294" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="31341" class="Keyword">open</a> <a id="31346" class="Keyword">import</a> <a id="31353" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="31394" class="Keyword">open</a> <a id="31399" class="Keyword">import</a> <a id="31406" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="31444" class="Keyword">open</a> <a id="31449" class="Keyword">import</a> <a id="31456" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="31501" class="Keyword">open</a> <a id="31506" class="Keyword">import</a> <a id="31513" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="31562" class="Keyword">open</a> <a id="31567" class="Keyword">import</a> <a id="31574" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="31651" class="Keyword">open</a> <a id="31656" class="Keyword">import</a> <a id="31663" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="31715" class="Keyword">open</a> <a id="31720" class="Keyword">import</a> <a id="31727" href="type-theories.html" class="Module">type-theories</a>
<a id="31741" class="Keyword">open</a> <a id="31746" class="Keyword">import</a> <a id="31753" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="31795" class="Keyword">open</a> <a id="31800" class="Keyword">import</a> <a id="31807" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="31845" class="Keyword">open</a> <a id="31850" class="Keyword">import</a> <a id="31857" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="31903" class="Keyword">open</a> <a id="31908" class="Keyword">import</a> <a id="31915" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="31962" class="Keyword">open</a> <a id="31967" class="Keyword">import</a> <a id="31974" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="32009" class="Keyword">open</a> <a id="32014" class="Keyword">import</a> <a id="32021" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="32099" class="Keyword">open</a> <a id="32104" class="Keyword">import</a> <a id="32111" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="32135" class="Keyword">open</a> <a id="32140" class="Keyword">import</a> <a id="32147" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="32200" class="Keyword">open</a> <a id="32205" class="Keyword">import</a> <a id="32212" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="32255" class="Keyword">open</a> <a id="32260" class="Keyword">import</a> <a id="32267" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="32307" class="Keyword">open</a> <a id="32312" class="Keyword">import</a> <a id="32319" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="32358" class="Keyword">open</a> <a id="32363" class="Keyword">import</a> <a id="32370" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="32418" class="Keyword">open</a> <a id="32423" class="Keyword">import</a> <a id="32430" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="32477" class="Keyword">open</a> <a id="32482" class="Keyword">import</a> <a id="32489" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="32541" class="Keyword">open</a> <a id="32546" class="Keyword">import</a> <a id="32553" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="32597" class="Keyword">open</a> <a id="32602" class="Keyword">import</a> <a id="32609" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="32649" class="Keyword">open</a> <a id="32654" class="Keyword">import</a> <a id="32661" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="32713" class="Keyword">open</a> <a id="32718" class="Keyword">import</a> <a id="32725" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="32779" class="Keyword">open</a> <a id="32784" class="Keyword">import</a> <a id="32791" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="32839" class="Keyword">open</a> <a id="32844" class="Keyword">import</a> <a id="32851" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="32890" class="Keyword">open</a> <a id="32895" class="Keyword">import</a> <a id="32902" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="32935" class="Keyword">open</a> <a id="32940" class="Keyword">import</a> <a id="32947" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="32977" class="Keyword">open</a> <a id="32982" class="Keyword">import</a> <a id="32989" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="33048" class="Keyword">open</a> <a id="33053" class="Keyword">import</a> <a id="33060" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="33115" class="Keyword">open</a> <a id="33120" class="Keyword">import</a> <a id="33127" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="33174" class="Keyword">open</a> <a id="33179" class="Keyword">import</a> <a id="33186" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="33229" class="Keyword">open</a> <a id="33234" class="Keyword">import</a> <a id="33241" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="33286" class="Keyword">open</a> <a id="33291" class="Keyword">import</a> <a id="33298" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="33347" class="Keyword">open</a> <a id="33352" class="Keyword">import</a> <a id="33359" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="33410" class="Keyword">open</a> <a id="33415" class="Keyword">import</a> <a id="33422" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="33500" class="Keyword">open</a> <a id="33505" class="Keyword">import</a> <a id="33512" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="33552" class="Keyword">open</a> <a id="33557" class="Keyword">import</a> <a id="33564" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="33621" class="Keyword">open</a> <a id="33626" class="Keyword">import</a> <a id="33633" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="33668" class="Keyword">open</a> <a id="33673" class="Keyword">import</a> <a id="33680" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="33726" class="Keyword">open</a> <a id="33731" class="Keyword">import</a> <a id="33738" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="33793" class="Keyword">open</a> <a id="33798" class="Keyword">import</a> <a id="33805" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="33848" class="Keyword">open</a> <a id="33853" class="Keyword">import</a> <a id="33860" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="33919" class="Keyword">open</a> <a id="33924" class="Keyword">import</a> <a id="33931" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="33968" class="Keyword">open</a> <a id="33973" class="Keyword">import</a> <a id="33980" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="34021" class="Keyword">open</a> <a id="34026" class="Keyword">import</a> <a id="34033" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="34072" class="Keyword">open</a> <a id="34077" class="Keyword">import</a> <a id="34084" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="34122" class="Keyword">open</a> <a id="34127" class="Keyword">import</a> <a id="34134" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="34186" class="Keyword">open</a> <a id="34191" class="Keyword">import</a> <a id="34198" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="34243" class="Keyword">open</a> <a id="34248" class="Keyword">import</a> <a id="34255" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="34292" class="Keyword">open</a> <a id="34297" class="Keyword">import</a> <a id="34304" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="34353" class="Keyword">open</a> <a id="34358" class="Keyword">import</a> <a id="34365" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="34404" class="Keyword">open</a> <a id="34409" class="Keyword">import</a> <a id="34416" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="34454" class="Keyword">open</a> <a id="34459" class="Keyword">import</a> <a id="34466" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="34521" class="Keyword">open</a> <a id="34526" class="Keyword">import</a> <a id="34533" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="34572" class="Keyword">open</a> <a id="34577" class="Keyword">import</a> <a id="34584" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="34632" class="Keyword">open</a> <a id="34637" class="Keyword">import</a> <a id="34644" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="34691" class="Keyword">open</a> <a id="34696" class="Keyword">import</a> <a id="34703" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="34741" class="Keyword">open</a> <a id="34746" class="Keyword">import</a> <a id="34753" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="34783" class="Keyword">open</a> <a id="34788" class="Keyword">import</a> <a id="34795" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="34852" class="Keyword">open</a> <a id="34857" class="Keyword">import</a> <a id="34864" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="34918" class="Keyword">open</a> <a id="34923" class="Keyword">import</a> <a id="34930" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="34960" class="Keyword">open</a> <a id="34965" class="Keyword">import</a> <a id="34972" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="35035" class="Keyword">open</a> <a id="35040" class="Keyword">import</a> <a id="35047" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="35090" class="Keyword">open</a> <a id="35095" class="Keyword">import</a> <a id="35102" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="35137" class="Keyword">open</a> <a id="35142" class="Keyword">import</a> <a id="35149" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="35189" class="Keyword">open</a> <a id="35194" class="Keyword">import</a> <a id="35201" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="35246" class="Keyword">open</a> <a id="35251" class="Keyword">import</a> <a id="35258" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="35308" class="Keyword">open</a> <a id="35313" class="Keyword">import</a> <a id="35320" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="35358" class="Keyword">open</a> <a id="35363" class="Keyword">import</a> <a id="35370" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="35419" class="Keyword">open</a> <a id="35424" class="Keyword">import</a> <a id="35431" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="35478" class="Keyword">open</a> <a id="35483" class="Keyword">import</a> <a id="35490" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="35553" class="Keyword">open</a> <a id="35558" class="Keyword">import</a> <a id="35565" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="35597" class="Keyword">open</a> <a id="35602" class="Keyword">import</a> <a id="35609" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="35662" class="Keyword">open</a> <a id="35667" class="Keyword">import</a> <a id="35674" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="35720" class="Keyword">open</a> <a id="35725" class="Keyword">import</a> <a id="35732" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="35778" class="Keyword">open</a> <a id="35783" class="Keyword">import</a> <a id="35790" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="35838" class="Keyword">open</a> <a id="35843" class="Keyword">import</a> <a id="35850" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="35890" class="Keyword">open</a> <a id="35895" class="Keyword">import</a> <a id="35902" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="35947" class="Keyword">open</a> <a id="35952" class="Keyword">import</a> <a id="35959" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>