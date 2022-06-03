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
<a id="12493" class="Keyword">open</a> <a id="12498" class="Keyword">import</a> <a id="12505" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12537" class="Keyword">open</a> <a id="12542" class="Keyword">import</a> <a id="12549" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12583" class="Keyword">open</a> <a id="12588" class="Keyword">import</a> <a id="12595" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12618" class="Keyword">open</a> <a id="12623" class="Keyword">import</a> <a id="12630" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="12700" class="Keyword">open</a> <a id="12705" class="Keyword">import</a> <a id="12712" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="12782" class="Keyword">open</a> <a id="12787" class="Keyword">import</a> <a id="12794" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12821" class="Keyword">open</a> <a id="12826" class="Keyword">import</a> <a id="12833" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12861" class="Keyword">open</a> <a id="12866" class="Keyword">import</a> <a id="12873" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12910" class="Keyword">open</a> <a id="12915" class="Keyword">import</a> <a id="12922" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12970" class="Keyword">open</a> <a id="12975" class="Keyword">import</a> <a id="12982" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="13022" class="Keyword">open</a> <a id="13027" class="Keyword">import</a> <a id="13034" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="13056" class="Keyword">open</a> <a id="13061" class="Keyword">import</a> <a id="13068" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13091" class="Keyword">open</a> <a id="13096" class="Keyword">import</a> <a id="13103" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13128" class="Keyword">open</a> <a id="13133" class="Keyword">import</a> <a id="13140" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13185" class="Keyword">open</a> <a id="13190" class="Keyword">import</a> <a id="13197" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13241" class="Keyword">open</a> <a id="13246" class="Keyword">import</a> <a id="13253" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13289" class="Keyword">open</a> <a id="13294" class="Keyword">import</a> <a id="13301" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13346" class="Keyword">open</a> <a id="13351" class="Keyword">import</a> <a id="13358" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13399" class="Keyword">open</a> <a id="13404" class="Keyword">import</a> <a id="13411" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13446" class="Keyword">open</a> <a id="13451" class="Keyword">import</a> <a id="13458" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="13490" class="Keyword">open</a> <a id="13495" class="Keyword">import</a> <a id="13502" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13533" class="Keyword">open</a> <a id="13538" class="Keyword">import</a> <a id="13545" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13578" class="Keyword">open</a> <a id="13583" class="Keyword">import</a> <a id="13590" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13623" class="Keyword">open</a> <a id="13628" class="Keyword">import</a> <a id="13635" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13665" class="Keyword">open</a> <a id="13670" class="Keyword">import</a> <a id="13677" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13701" class="Keyword">open</a> <a id="13706" class="Keyword">import</a> <a id="13713" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13751" class="Keyword">open</a> <a id="13756" class="Keyword">import</a> <a id="13763" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13794" class="Keyword">open</a> <a id="13799" class="Keyword">import</a> <a id="13806" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13831" class="Keyword">open</a> <a id="13836" class="Keyword">import</a> <a id="13843" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13871" class="Keyword">open</a> <a id="13876" class="Keyword">import</a> <a id="13883" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13907" class="Keyword">open</a> <a id="13912" class="Keyword">import</a> <a id="13919" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13945" class="Keyword">open</a> <a id="13950" class="Keyword">import</a> <a id="13957" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="13992" class="Keyword">open</a> <a id="13997" class="Keyword">import</a> <a id="14004" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="14025" class="Keyword">open</a> <a id="14030" class="Keyword">import</a> <a id="14037" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="14086" class="Keyword">open</a> <a id="14091" class="Keyword">import</a> <a id="14098" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14139" class="Keyword">open</a> <a id="14144" class="Keyword">import</a> <a id="14151" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14201" class="Keyword">open</a> <a id="14206" class="Keyword">import</a> <a id="14213" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14259" class="Keyword">open</a> <a id="14264" class="Keyword">import</a> <a id="14271" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14311" class="Keyword">open</a> <a id="14316" class="Keyword">import</a> <a id="14323" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14373" class="Keyword">open</a> <a id="14378" class="Keyword">import</a> <a id="14385" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14424" class="Keyword">open</a> <a id="14429" class="Keyword">import</a> <a id="14436" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14476" class="Keyword">open</a> <a id="14481" class="Keyword">import</a> <a id="14488" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14521" class="Keyword">open</a> <a id="14526" class="Keyword">import</a> <a id="14533" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14582" class="Keyword">open</a> <a id="14587" class="Keyword">import</a> <a id="14594" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14619" class="Keyword">open</a> <a id="14624" class="Keyword">import</a> <a id="14631" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14669" class="Keyword">open</a> <a id="14674" class="Keyword">import</a> <a id="14681" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14703" class="Keyword">open</a> <a id="14708" class="Keyword">import</a> <a id="14715" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14743" class="Keyword">open</a> <a id="14748" class="Keyword">import</a> <a id="14755" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="14791" class="Keyword">open</a> <a id="14796" class="Keyword">import</a> <a id="14803" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14829" class="Keyword">open</a> <a id="14834" class="Keyword">import</a> <a id="14841" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14859" class="Keyword">open</a> <a id="14864" class="Keyword">import</a> <a id="14871" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14906" class="Keyword">open</a> <a id="14911" class="Keyword">import</a> <a id="14918" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="14953" class="Keyword">open</a> <a id="14958" class="Keyword">import</a> <a id="14965" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="14992" class="Keyword">open</a> <a id="14997" class="Keyword">import</a> <a id="15004" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="15060" class="Keyword">open</a> <a id="15065" class="Keyword">import</a> <a id="15072" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="15101" class="Keyword">open</a> <a id="15106" class="Keyword">import</a> <a id="15113" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="15143" class="Keyword">open</a> <a id="15148" class="Keyword">import</a> <a id="15155" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="15182" class="Keyword">open</a> <a id="15187" class="Keyword">import</a> <a id="15194" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15220" class="Keyword">open</a> <a id="15225" class="Keyword">import</a> <a id="15232" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15259" class="Keyword">open</a> <a id="15264" class="Keyword">import</a> <a id="15271" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15295" class="Keyword">open</a> <a id="15300" class="Keyword">import</a> <a id="15307" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15330" class="Keyword">open</a> <a id="15335" class="Keyword">import</a> <a id="15342" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15369" class="Keyword">open</a> <a id="15374" class="Keyword">import</a> <a id="15381" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15413" class="Keyword">open</a> <a id="15418" class="Keyword">import</a> <a id="15425" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15460" class="Keyword">open</a> <a id="15465" class="Keyword">import</a> <a id="15472" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15503" class="Keyword">open</a> <a id="15508" class="Keyword">import</a> <a id="15515" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15548" class="Keyword">open</a> <a id="15553" class="Keyword">import</a> <a id="15560" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15594" class="Keyword">open</a> <a id="15599" class="Keyword">import</a> <a id="15606" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15646" class="Keyword">open</a> <a id="15651" class="Keyword">import</a> <a id="15658" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15689" class="Keyword">open</a> <a id="15694" class="Keyword">import</a> <a id="15701" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15733" class="Keyword">open</a> <a id="15738" class="Keyword">import</a> <a id="15745" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15776" class="Keyword">open</a> <a id="15781" class="Keyword">import</a> <a id="15788" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15805" class="Keyword">open</a> <a id="15810" class="Keyword">import</a> <a id="15817" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15842" class="Keyword">open</a> <a id="15847" class="Keyword">import</a> <a id="15854" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15883" class="Keyword">open</a> <a id="15888" class="Keyword">import</a> <a id="15895" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15920" class="Keyword">open</a> <a id="15925" class="Keyword">import</a> <a id="15932" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15953" class="Keyword">open</a> <a id="15958" class="Keyword">import</a> <a id="15965" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="15989" class="Keyword">open</a> <a id="15994" class="Keyword">import</a> <a id="16001" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="16021" class="Keyword">open</a> <a id="16026" class="Keyword">import</a> <a id="16033" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="16067" class="Keyword">open</a> <a id="16072" class="Keyword">import</a> <a id="16079" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="16117" class="Keyword">open</a> <a id="16122" class="Keyword">import</a> <a id="16129" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="16157" class="Keyword">open</a> <a id="16162" class="Keyword">import</a> <a id="16169" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="16193" class="Keyword">open</a> <a id="16198" class="Keyword">import</a> <a id="16205" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="16232" class="Keyword">open</a> <a id="16237" class="Keyword">import</a> <a id="16244" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16279" class="Keyword">open</a> <a id="16284" class="Keyword">import</a> <a id="16291" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16312" class="Keyword">open</a> <a id="16317" class="Keyword">import</a> <a id="16324" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16360" class="Keyword">open</a> <a id="16365" class="Keyword">import</a> <a id="16372" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16417" class="Keyword">open</a> <a id="16422" class="Keyword">import</a> <a id="16429" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16475" class="Keyword">open</a> <a id="16480" class="Keyword">import</a> <a id="16487" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16527" class="Keyword">open</a> <a id="16532" class="Keyword">import</a> <a id="16539" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16569" class="Keyword">open</a> <a id="16574" class="Keyword">import</a> <a id="16581" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16618" class="Keyword">open</a> <a id="16623" class="Keyword">import</a> <a id="16630" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16654" class="Keyword">open</a> <a id="16659" class="Keyword">import</a> <a id="16666" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16687" class="Keyword">open</a> <a id="16692" class="Keyword">import</a> <a id="16699" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16734" class="Keyword">open</a> <a id="16739" class="Keyword">import</a> <a id="16746" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16783" class="Keyword">open</a> <a id="16788" class="Keyword">import</a> <a id="16795" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16844" class="Keyword">open</a> <a id="16849" class="Keyword">import</a> <a id="16856" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16889" class="Keyword">open</a> <a id="16894" class="Keyword">import</a> <a id="16901" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16924" class="Keyword">open</a> <a id="16929" class="Keyword">import</a> <a id="16936" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="16959" class="Keyword">open</a> <a id="16964" class="Keyword">import</a> <a id="16971" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="16994" class="Keyword">open</a> <a id="16999" class="Keyword">import</a> <a id="17006" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="17034" class="Keyword">open</a> <a id="17039" class="Keyword">import</a> <a id="17046" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="17066" class="Keyword">open</a> <a id="17071" class="Keyword">import</a> <a id="17078" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="17099" class="Keyword">open</a> <a id="17104" class="Keyword">import</a> <a id="17111" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="17142" class="Keyword">open</a> <a id="17147" class="Keyword">import</a> <a id="17154" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="17181" class="Keyword">open</a> <a id="17186" class="Keyword">import</a> <a id="17193" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="17209" class="Keyword">open</a> <a id="17214" class="Keyword">import</a> <a id="17221" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17252" class="Keyword">open</a> <a id="17257" class="Keyword">import</a> <a id="17264" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17281" class="Keyword">open</a> <a id="17286" class="Keyword">import</a> <a id="17293" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17315" class="Keyword">open</a> <a id="17320" class="Keyword">import</a> <a id="17327" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17354" class="Keyword">open</a> <a id="17359" class="Keyword">import</a> <a id="17366" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17389" class="Keyword">open</a> <a id="17394" class="Keyword">import</a> <a id="17401" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17428" class="Keyword">open</a> <a id="17433" class="Keyword">import</a> <a id="17440" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17473" class="Keyword">open</a> <a id="17478" class="Keyword">import</a> <a id="17485" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17525" class="Keyword">open</a> <a id="17530" class="Keyword">import</a> <a id="17537" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17558" class="Keyword">open</a> <a id="17563" class="Keyword">import</a> <a id="17570" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17599" class="Keyword">open</a> <a id="17604" class="Keyword">import</a> <a id="17611" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17649" class="Keyword">open</a> <a id="17654" class="Keyword">import</a> <a id="17661" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17681" class="Keyword">open</a> <a id="17686" class="Keyword">import</a> <a id="17693" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17717" class="Keyword">open</a> <a id="17722" class="Keyword">import</a> <a id="17729" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17756" class="Keyword">open</a> <a id="17761" class="Keyword">import</a> <a id="17768" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17800" class="Keyword">open</a> <a id="17805" class="Keyword">import</a> <a id="17812" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17842" class="Keyword">open</a> <a id="17847" class="Keyword">import</a> <a id="17854" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17880" class="Keyword">open</a> <a id="17885" class="Keyword">import</a> <a id="17892" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17919" class="Keyword">open</a> <a id="17924" class="Keyword">import</a> <a id="17931" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="17960" class="Keyword">open</a> <a id="17965" class="Keyword">import</a> <a id="17972" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="17995" class="Keyword">open</a> <a id="18000" class="Keyword">import</a> <a id="18007" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="18058" class="Keyword">open</a> <a id="18063" class="Keyword">import</a> <a id="18070" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="18113" class="Keyword">open</a> <a id="18118" class="Keyword">import</a> <a id="18125" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="18173" class="Keyword">open</a> <a id="18178" class="Keyword">import</a> <a id="18185" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="18223" class="Keyword">open</a> <a id="18228" class="Keyword">import</a> <a id="18235" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18272" class="Keyword">open</a> <a id="18277" class="Keyword">import</a> <a id="18284" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18301" class="Keyword">open</a> <a id="18306" class="Keyword">import</a> <a id="18313" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18341" class="Keyword">open</a> <a id="18346" class="Keyword">import</a> <a id="18353" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18389" class="Keyword">open</a> <a id="18394" class="Keyword">import</a> <a id="18401" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18439" class="Keyword">open</a> <a id="18444" class="Keyword">import</a> <a id="18451" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18484" class="Keyword">open</a> <a id="18489" class="Keyword">import</a> <a id="18496" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18517" class="Keyword">open</a> <a id="18522" class="Keyword">import</a> <a id="18529" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18583" class="Keyword">open</a> <a id="18588" class="Keyword">import</a> <a id="18595" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18617" class="Keyword">open</a> <a id="18622" class="Keyword">import</a> <a id="18629" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18664" class="Keyword">open</a> <a id="18669" class="Keyword">import</a> <a id="18676" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18706" class="Keyword">open</a> <a id="18711" class="Keyword">import</a> <a id="18718" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18757" class="Keyword">open</a> <a id="18762" class="Keyword">import</a> <a id="18769" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18823" class="Keyword">open</a> <a id="18828" class="Keyword">import</a> <a id="18835" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18881" class="Keyword">open</a> <a id="18886" class="Keyword">import</a> <a id="18893" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18944" class="Keyword">open</a> <a id="18949" class="Keyword">import</a> <a id="18956" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="18997" class="Keyword">open</a> <a id="19002" class="Keyword">import</a> <a id="19009" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="19054" class="Keyword">open</a> <a id="19059" class="Keyword">import</a> <a id="19066" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="19111" class="Keyword">open</a> <a id="19116" class="Keyword">import</a> <a id="19123" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="19159" class="Keyword">open</a> <a id="19164" class="Keyword">import</a> <a id="19171" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="19207" class="Keyword">open</a> <a id="19212" class="Keyword">import</a> <a id="19219" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19284" class="Keyword">open</a> <a id="19289" class="Keyword">import</a> <a id="19296" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19351" class="Keyword">open</a> <a id="19356" class="Keyword">import</a> <a id="19363" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19403" class="Keyword">open</a> <a id="19408" class="Keyword">import</a> <a id="19415" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19459" class="Keyword">open</a> <a id="19464" class="Keyword">import</a> <a id="19471" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19516" class="Keyword">open</a> <a id="19521" class="Keyword">import</a> <a id="19528" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19569" class="Keyword">open</a> <a id="19574" class="Keyword">import</a> <a id="19581" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19621" class="Keyword">open</a> <a id="19626" class="Keyword">import</a> <a id="19633" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19660" class="Keyword">open</a> <a id="19665" class="Keyword">import</a> <a id="19672" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19708" class="Keyword">open</a> <a id="19713" class="Keyword">import</a> <a id="19720" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19747" class="Keyword">open</a> <a id="19752" class="Keyword">import</a> <a id="19759" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19796" class="Keyword">open</a> <a id="19801" class="Keyword">import</a> <a id="19808" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19836" class="Keyword">open</a> <a id="19841" class="Keyword">import</a> <a id="19848" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19867" class="Keyword">open</a> <a id="19872" class="Keyword">import</a> <a id="19879" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19919" class="Keyword">open</a> <a id="19924" class="Keyword">import</a> <a id="19931" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19963" class="Keyword">open</a> <a id="19968" class="Keyword">import</a> <a id="19975" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="20023" class="Keyword">open</a> <a id="20028" class="Keyword">import</a> <a id="20035" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="20058" class="Keyword">open</a> <a id="20063" class="Keyword">import</a> <a id="20070" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="20094" class="Keyword">open</a> <a id="20099" class="Keyword">import</a> <a id="20106" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="20146" class="Keyword">open</a> <a id="20151" class="Keyword">import</a> <a id="20158" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="20201" class="Keyword">open</a> <a id="20206" class="Keyword">import</a> <a id="20213" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20247" class="Keyword">open</a> <a id="20252" class="Keyword">import</a> <a id="20259" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20291" class="Keyword">open</a> <a id="20296" class="Keyword">import</a> <a id="20303" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20333" class="Keyword">open</a> <a id="20338" class="Keyword">import</a> <a id="20345" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20379" class="Keyword">open</a> <a id="20384" class="Keyword">import</a> <a id="20391" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20426" class="Keyword">open</a> <a id="20431" class="Keyword">import</a> <a id="20438" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20475" class="Keyword">open</a> <a id="20480" class="Keyword">import</a> <a id="20487" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20514" class="Keyword">open</a> <a id="20519" class="Keyword">import</a> <a id="20526" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20554" class="Keyword">open</a> <a id="20559" class="Keyword">import</a> <a id="20566" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20615" class="Keyword">open</a> <a id="20620" class="Keyword">import</a> <a id="20627" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20673" class="Keyword">open</a> <a id="20678" class="Keyword">import</a> <a id="20685" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20725" class="Keyword">open</a> <a id="20730" class="Keyword">import</a> <a id="20737" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20775" class="Keyword">open</a> <a id="20780" class="Keyword">import</a> <a id="20787" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20816" class="Keyword">open</a> <a id="20821" class="Keyword">import</a> <a id="20828" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20858" class="Keyword">open</a> <a id="20863" class="Keyword">import</a> <a id="20870" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20901" class="Keyword">open</a> <a id="20906" class="Keyword">import</a> <a id="20913" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="20953" class="Keyword">open</a> <a id="20958" class="Keyword">import</a> <a id="20965" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="20991" class="Keyword">open</a> <a id="20996" class="Keyword">import</a> <a id="21003" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="21058" class="Keyword">open</a> <a id="21063" class="Keyword">import</a> <a id="21070" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="21121" class="Keyword">open</a> <a id="21126" class="Keyword">import</a> <a id="21133" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="21178" class="Keyword">open</a> <a id="21183" class="Keyword">import</a> <a id="21190" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21244" class="Keyword">open</a> <a id="21249" class="Keyword">import</a> <a id="21256" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21283" class="Keyword">open</a> <a id="21288" class="Keyword">import</a> <a id="21295" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21328" class="Keyword">open</a> <a id="21333" class="Keyword">import</a> <a id="21340" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21371" class="Keyword">open</a> <a id="21376" class="Keyword">import</a> <a id="21383" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21420" class="Keyword">open</a> <a id="21425" class="Keyword">import</a> <a id="21432" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21457" class="Keyword">open</a> <a id="21462" class="Keyword">import</a> <a id="21469" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21501" class="Keyword">open</a> <a id="21506" class="Keyword">import</a> <a id="21513" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21548" class="Keyword">open</a> <a id="21553" class="Keyword">import</a> <a id="21560" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21589" class="Keyword">open</a> <a id="21594" class="Keyword">import</a> <a id="21601" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21627" class="Keyword">open</a> <a id="21632" class="Keyword">import</a> <a id="21639" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21667" class="Keyword">open</a> <a id="21672" class="Keyword">import</a> <a id="21679" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21704" class="Keyword">open</a> <a id="21709" class="Keyword">import</a> <a id="21716" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21737" class="Keyword">open</a> <a id="21742" class="Keyword">import</a> <a id="21749" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21785" class="Keyword">open</a> <a id="21790" class="Keyword">import</a> <a id="21797" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21840" class="Keyword">open</a> <a id="21845" class="Keyword">import</a> <a id="21852" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21877" class="Keyword">open</a> <a id="21882" class="Keyword">import</a> <a id="21889" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21920" class="Keyword">open</a> <a id="21925" class="Keyword">import</a> <a id="21932" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21964" class="Keyword">open</a> <a id="21969" class="Keyword">import</a> <a id="21976" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="22010" class="Keyword">open</a> <a id="22015" class="Keyword">import</a> <a id="22022" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="22078" class="Keyword">open</a> <a id="22083" class="Keyword">import</a> <a id="22090" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="22143" class="Keyword">open</a> <a id="22148" class="Keyword">import</a> <a id="22155" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="22182" class="Keyword">open</a> <a id="22187" class="Keyword">import</a> <a id="22194" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="22239" class="Keyword">open</a> <a id="22244" class="Keyword">import</a> <a id="22251" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22313" class="Keyword">open</a> <a id="22318" class="Keyword">import</a> <a id="22325" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22338" class="Keyword">open</a> <a id="22343" class="Keyword">import</a> <a id="22350" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22391" class="Keyword">open</a> <a id="22396" class="Keyword">import</a> <a id="22403" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22432" class="Keyword">open</a> <a id="22437" class="Keyword">import</a> <a id="22444" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22489" class="Keyword">open</a> <a id="22494" class="Keyword">import</a> <a id="22501" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22545" class="Keyword">open</a> <a id="22550" class="Keyword">import</a> <a id="22557" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="22584" class="Keyword">open</a> <a id="22589" class="Keyword">import</a> <a id="22596" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="22637" class="Keyword">open</a> <a id="22642" class="Keyword">import</a> <a id="22649" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="22672" class="Keyword">open</a> <a id="22677" class="Keyword">import</a> <a id="22684" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="22733" class="Keyword">open</a> <a id="22738" class="Keyword">import</a> <a id="22745" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="22784" class="Keyword">open</a> <a id="22789" class="Keyword">import</a> <a id="22796" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="22837" class="Keyword">open</a> <a id="22842" class="Keyword">import</a> <a id="22849" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22893" class="Keyword">open</a> <a id="22898" class="Keyword">import</a> <a id="22905" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22942" class="Keyword">open</a> <a id="22947" class="Keyword">import</a> <a id="22954" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="22976" class="Keyword">open</a> <a id="22981" class="Keyword">import</a> <a id="22988" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="23018" class="Keyword">open</a> <a id="23023" class="Keyword">import</a> <a id="23030" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="23069" class="Keyword">open</a> <a id="23074" class="Keyword">import</a> <a id="23081" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="23119" class="Keyword">open</a> <a id="23124" class="Keyword">import</a> <a id="23131" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="23162" class="Keyword">open</a> <a id="23167" class="Keyword">import</a> <a id="23174" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="23201" class="Keyword">open</a> <a id="23206" class="Keyword">import</a> <a id="23213" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="23271" class="Keyword">open</a> <a id="23276" class="Keyword">import</a> <a id="23283" href="group-theory.html" class="Module">group-theory</a>
<a id="23296" class="Keyword">open</a> <a id="23301" class="Keyword">import</a> <a id="23308" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="23336" class="Keyword">open</a> <a id="23341" class="Keyword">import</a> <a id="23348" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="23379" class="Keyword">open</a> <a id="23384" class="Keyword">import</a> <a id="23391" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="23427" class="Keyword">open</a> <a id="23432" class="Keyword">import</a> <a id="23439" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="23490" class="Keyword">open</a> <a id="23495" class="Keyword">import</a> <a id="23502" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="23535" class="Keyword">open</a> <a id="23540" class="Keyword">import</a> <a id="23547" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="23594" class="Keyword">open</a> <a id="23599" class="Keyword">import</a> <a id="23606" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="23645" class="Keyword">open</a> <a id="23650" class="Keyword">import</a> <a id="23657" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="23697" class="Keyword">open</a> <a id="23702" class="Keyword">import</a> <a id="23709" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="23752" class="Keyword">open</a> <a id="23757" class="Keyword">import</a> <a id="23764" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="23796" class="Keyword">open</a> <a id="23801" class="Keyword">import</a> <a id="23808" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="23844" class="Keyword">open</a> <a id="23849" class="Keyword">import</a> <a id="23856" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="23885" class="Keyword">open</a> <a id="23890" class="Keyword">import</a> <a id="23897" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="23930" class="Keyword">open</a> <a id="23935" class="Keyword">import</a> <a id="23942" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="23978" class="Keyword">open</a> <a id="23983" class="Keyword">import</a> <a id="23990" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="24019" class="Keyword">open</a> <a id="24024" class="Keyword">import</a> <a id="24031" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="24063" class="Keyword">open</a> <a id="24068" class="Keyword">import</a> <a id="24075" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="24100" class="Keyword">open</a> <a id="24105" class="Keyword">import</a> <a id="24112" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="24143" class="Keyword">open</a> <a id="24148" class="Keyword">import</a> <a id="24155" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="24202" class="Keyword">open</a> <a id="24207" class="Keyword">import</a> <a id="24214" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="24247" class="Keyword">open</a> <a id="24252" class="Keyword">import</a> <a id="24259" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="24299" class="Keyword">open</a> <a id="24304" class="Keyword">import</a> <a id="24311" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="24348" class="Keyword">open</a> <a id="24353" class="Keyword">import</a> <a id="24360" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="24396" class="Keyword">open</a> <a id="24401" class="Keyword">import</a> <a id="24408" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="24440" class="Keyword">open</a> <a id="24445" class="Keyword">import</a> <a id="24452" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="24479" class="Keyword">open</a> <a id="24484" class="Keyword">import</a> <a id="24491" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="24511" class="Keyword">open</a> <a id="24516" class="Keyword">import</a> <a id="24523" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="24550" class="Keyword">open</a> <a id="24555" class="Keyword">import</a> <a id="24562" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="24604" class="Keyword">open</a> <a id="24609" class="Keyword">import</a> <a id="24616" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="24663" class="Keyword">open</a> <a id="24668" class="Keyword">import</a> <a id="24675" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="24716" class="Keyword">open</a> <a id="24721" class="Keyword">import</a> <a id="24728" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="24762" class="Keyword">open</a> <a id="24767" class="Keyword">import</a> <a id="24774" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="24809" class="Keyword">open</a> <a id="24814" class="Keyword">import</a> <a id="24821" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="24859" class="Keyword">open</a> <a id="24864" class="Keyword">import</a> <a id="24871" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="24903" class="Keyword">open</a> <a id="24908" class="Keyword">import</a> <a id="24915" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="24956" class="Keyword">open</a> <a id="24961" class="Keyword">import</a> <a id="24968" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="25009" class="Keyword">open</a> <a id="25014" class="Keyword">import</a> <a id="25021" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="25061" class="Keyword">open</a> <a id="25066" class="Keyword">import</a> <a id="25073" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="25106" class="Keyword">open</a> <a id="25111" class="Keyword">import</a> <a id="25118" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="25155" class="Keyword">open</a> <a id="25160" class="Keyword">import</a> <a id="25167" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="25197" class="Keyword">open</a> <a id="25202" class="Keyword">import</a> <a id="25209" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="25254" class="Keyword">open</a> <a id="25259" class="Keyword">import</a> <a id="25266" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="25294" class="Keyword">open</a> <a id="25299" class="Keyword">import</a> <a id="25306" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="25327" class="Keyword">open</a> <a id="25332" class="Keyword">import</a> <a id="25339" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="25373" class="Keyword">open</a> <a id="25378" class="Keyword">import</a> <a id="25385" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="25419" class="Keyword">open</a> <a id="25424" class="Keyword">import</a> <a id="25431" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="25466" class="Keyword">open</a> <a id="25471" class="Keyword">import</a> <a id="25478" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="25520" class="Keyword">open</a> <a id="25525" class="Keyword">import</a> <a id="25532" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="25567" class="Keyword">open</a> <a id="25572" class="Keyword">import</a> <a id="25579" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="25618" class="Keyword">open</a> <a id="25623" class="Keyword">import</a> <a id="25630" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="25667" class="Keyword">open</a> <a id="25672" class="Keyword">import</a> <a id="25679" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="25703" class="Keyword">open</a> <a id="25708" class="Keyword">import</a> <a id="25715" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="25740" class="Keyword">open</a> <a id="25745" class="Keyword">import</a> <a id="25752" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="25783" class="Keyword">open</a> <a id="25788" class="Keyword">import</a> <a id="25795" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="25846" class="Keyword">open</a> <a id="25851" class="Keyword">import</a> <a id="25858" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="25881" class="Keyword">open</a> <a id="25886" class="Keyword">import</a> <a id="25893" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="25941" class="Keyword">open</a> <a id="25946" class="Keyword">import</a> <a id="25953" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="25983" class="Keyword">open</a> <a id="25988" class="Keyword">import</a> <a id="25995" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="26065" class="Keyword">open</a> <a id="26070" class="Keyword">import</a> <a id="26077" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="26092" class="Keyword">open</a> <a id="26097" class="Keyword">import</a> <a id="26104" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="26137" class="Keyword">open</a> <a id="26142" class="Keyword">import</a> <a id="26149" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="26181" class="Keyword">open</a> <a id="26186" class="Keyword">import</a> <a id="26193" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="26235" class="Keyword">open</a> <a id="26240" class="Keyword">import</a> <a id="26247" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="26285" class="Keyword">open</a> <a id="26290" class="Keyword">import</a> <a id="26297" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="26334" class="Keyword">open</a> <a id="26339" class="Keyword">import</a> <a id="26346" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="26379" class="Keyword">open</a> <a id="26384" class="Keyword">import</a> <a id="26391" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="26415" class="Keyword">open</a> <a id="26420" class="Keyword">import</a> <a id="26427" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="26466" class="Keyword">open</a> <a id="26471" class="Keyword">import</a> <a id="26478" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="26524" class="Keyword">open</a> <a id="26529" class="Keyword">import</a> <a id="26536" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="26581" class="Keyword">open</a> <a id="26586" class="Keyword">import</a> <a id="26593" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="26631" class="Keyword">open</a> <a id="26636" class="Keyword">import</a> <a id="26643" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="26675" class="Keyword">open</a> <a id="26680" class="Keyword">import</a> <a id="26687" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="26740" class="Keyword">open</a> <a id="26745" class="Keyword">import</a> <a id="26752" href="order-theory.html" class="Module">order-theory</a>
<a id="26765" class="Keyword">open</a> <a id="26770" class="Keyword">import</a> <a id="26777" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="26804" class="Keyword">open</a> <a id="26809" class="Keyword">import</a> <a id="26816" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="26846" class="Keyword">open</a> <a id="26851" class="Keyword">import</a> <a id="26858" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="26891" class="Keyword">open</a> <a id="26896" class="Keyword">import</a> <a id="26903" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="26939" class="Keyword">open</a> <a id="26944" class="Keyword">import</a> <a id="26951" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="26978" class="Keyword">open</a> <a id="26983" class="Keyword">import</a> <a id="26990" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="27020" class="Keyword">open</a> <a id="27025" class="Keyword">import</a> <a id="27032" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="27068" class="Keyword">open</a> <a id="27073" class="Keyword">import</a> <a id="27080" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="27122" class="Keyword">open</a> <a id="27127" class="Keyword">import</a> <a id="27134" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="27166" class="Keyword">open</a> <a id="27171" class="Keyword">import</a> <a id="27178" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="27209" class="Keyword">open</a> <a id="27214" class="Keyword">import</a> <a id="27221" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="27247" class="Keyword">open</a> <a id="27252" class="Keyword">import</a> <a id="27259" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="27288" class="Keyword">open</a> <a id="27293" class="Keyword">import</a> <a id="27300" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="27337" class="Keyword">open</a> <a id="27342" class="Keyword">import</a> <a id="27349" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="27389" class="Keyword">open</a> <a id="27394" class="Keyword">import</a> <a id="27401" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="27423" class="Keyword">open</a> <a id="27428" class="Keyword">import</a> <a id="27435" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="27470" class="Keyword">open</a> <a id="27475" class="Keyword">import</a> <a id="27482" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="27520" class="Keyword">open</a> <a id="27525" class="Keyword">import</a> <a id="27532" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="27571" class="Keyword">open</a> <a id="27576" class="Keyword">import</a> <a id="27583" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="27618" class="Keyword">open</a> <a id="27623" class="Keyword">import</a> <a id="27630" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="27665" class="Keyword">open</a> <a id="27670" class="Keyword">import</a> <a id="27677" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="27715" class="Keyword">open</a> <a id="27720" class="Keyword">import</a> <a id="27727" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="27758" class="Keyword">open</a> <a id="27763" class="Keyword">import</a> <a id="27770" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="27812" class="Keyword">open</a> <a id="27817" class="Keyword">import</a> <a id="27824" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="27869" class="Keyword">open</a> <a id="27874" class="Keyword">import</a> <a id="27881" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="27914" class="Keyword">open</a> <a id="27919" class="Keyword">import</a> <a id="27926" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="27946" class="Keyword">open</a> <a id="27951" class="Keyword">import</a> <a id="27958" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="27981" class="Keyword">open</a> <a id="27986" class="Keyword">import</a> <a id="27993" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="28016" class="Keyword">open</a> <a id="28021" class="Keyword">import</a> <a id="28028" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="28054" class="Keyword">open</a> <a id="28059" class="Keyword">import</a> <a id="28066" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="28092" class="Keyword">open</a> <a id="28097" class="Keyword">import</a> <a id="28104" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="28160" class="Keyword">open</a> <a id="28165" class="Keyword">import</a> <a id="28172" href="polytopes.html" class="Module">polytopes</a>
<a id="28182" class="Keyword">open</a> <a id="28187" class="Keyword">import</a> <a id="28194" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="28252" class="Keyword">open</a> <a id="28257" class="Keyword">import</a> <a id="28264" href="ring-theory.html" class="Module">ring-theory</a>
<a id="28276" class="Keyword">open</a> <a id="28281" class="Keyword">import</a> <a id="28288" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="28325" class="Keyword">open</a> <a id="28330" class="Keyword">import</a> <a id="28337" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="28364" class="Keyword">open</a> <a id="28369" class="Keyword">import</a> <a id="28376" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="28408" class="Keyword">open</a> <a id="28413" class="Keyword">import</a> <a id="28420" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="28466" class="Keyword">open</a> <a id="28471" class="Keyword">import</a> <a id="28478" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="28503" class="Keyword">open</a> <a id="28508" class="Keyword">import</a> <a id="28515" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="28558" class="Keyword">open</a> <a id="28563" class="Keyword">import</a> <a id="28570" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="28608" class="Keyword">open</a> <a id="28613" class="Keyword">import</a> <a id="28620" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="28651" class="Keyword">open</a> <a id="28656" class="Keyword">import</a> <a id="28663" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="28695" class="Keyword">open</a> <a id="28700" class="Keyword">import</a> <a id="28707" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="28733" class="Keyword">open</a> <a id="28738" class="Keyword">import</a> <a id="28745" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="28774" class="Keyword">open</a> <a id="28779" class="Keyword">import</a> <a id="28786" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="28823" class="Keyword">open</a> <a id="28828" class="Keyword">import</a> <a id="28835" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="28864" class="Keyword">open</a> <a id="28869" class="Keyword">import</a> <a id="28876" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="28903" class="Keyword">open</a> <a id="28908" class="Keyword">import</a> <a id="28915" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="28952" class="Keyword">open</a> <a id="28957" class="Keyword">import</a> <a id="28964" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="28991" class="Keyword">open</a> <a id="28996" class="Keyword">import</a> <a id="29003" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="29036" class="Keyword">open</a> <a id="29041" class="Keyword">import</a> <a id="29048" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="29066" class="Keyword">open</a> <a id="29071" class="Keyword">import</a> <a id="29078" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="29132" class="Keyword">open</a> <a id="29137" class="Keyword">import</a> <a id="29144" href="set-theory.html" class="Module">set-theory</a>
<a id="29155" class="Keyword">open</a> <a id="29160" class="Keyword">import</a> <a id="29167" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="29193" class="Keyword">open</a> <a id="29198" class="Keyword">import</a> <a id="29205" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="29267" class="Keyword">open</a> <a id="29272" class="Keyword">import</a> <a id="29279" href="structured-types.html" class="Module">structured-types</a>
<a id="29296" class="Keyword">open</a> <a id="29301" class="Keyword">import</a> <a id="29308" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="29343" class="Keyword">open</a> <a id="29348" class="Keyword">import</a> <a id="29355" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="29399" class="Keyword">open</a> <a id="29404" class="Keyword">import</a> <a id="29411" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="29475" class="Keyword">open</a> <a id="29480" class="Keyword">import</a> <a id="29487" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="29533" class="Keyword">open</a> <a id="29538" class="Keyword">import</a> <a id="29545" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="29569" class="Keyword">open</a> <a id="29574" class="Keyword">import</a> <a id="29581" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="29650" class="Keyword">open</a> <a id="29655" class="Keyword">import</a> <a id="29662" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="29707" class="Keyword">open</a> <a id="29712" class="Keyword">import</a> <a id="29719" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="29753" class="Keyword">open</a> <a id="29758" class="Keyword">import</a> <a id="29765" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="29826" class="Keyword">open</a> <a id="29831" class="Keyword">import</a> <a id="29838" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="29883" class="Keyword">open</a> <a id="29888" class="Keyword">import</a> <a id="29895" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="29933" class="Keyword">open</a> <a id="29938" class="Keyword">import</a> <a id="29945" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="29988" class="Keyword">open</a> <a id="29993" class="Keyword">import</a> <a id="30000" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="30036" class="Keyword">open</a> <a id="30041" class="Keyword">import</a> <a id="30048" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="30078" class="Keyword">open</a> <a id="30083" class="Keyword">import</a> <a id="30090" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="30121" class="Keyword">open</a> <a id="30126" class="Keyword">import</a> <a id="30133" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="30184" class="Keyword">open</a> <a id="30189" class="Keyword">import</a> <a id="30196" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="30251" class="Keyword">open</a> <a id="30256" class="Keyword">import</a> <a id="30263" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="30292" class="Keyword">open</a> <a id="30297" class="Keyword">import</a> <a id="30304" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="30332" class="Keyword">open</a> <a id="30337" class="Keyword">import</a> <a id="30344" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="30374" class="Keyword">open</a> <a id="30379" class="Keyword">import</a> <a id="30386" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="30420" class="Keyword">open</a> <a id="30425" class="Keyword">import</a> <a id="30432" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="30508" class="Keyword">open</a> <a id="30513" class="Keyword">import</a> <a id="30520" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="30546" class="Keyword">open</a> <a id="30551" class="Keyword">import</a> <a id="30558" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="30597" class="Keyword">open</a> <a id="30602" class="Keyword">import</a> <a id="30609" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="30647" class="Keyword">open</a> <a id="30652" class="Keyword">import</a> <a id="30659" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="30705" class="Keyword">open</a> <a id="30710" class="Keyword">import</a> <a id="30717" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="30754" class="Keyword">open</a> <a id="30759" class="Keyword">import</a> <a id="30766" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="30806" class="Keyword">open</a> <a id="30811" class="Keyword">import</a> <a id="30818" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="30857" class="Keyword">open</a> <a id="30862" class="Keyword">import</a> <a id="30869" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="30902" class="Keyword">open</a> <a id="30907" class="Keyword">import</a> <a id="30914" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="30949" class="Keyword">open</a> <a id="30954" class="Keyword">import</a> <a id="30961" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="31000" class="Keyword">open</a> <a id="31005" class="Keyword">import</a> <a id="31012" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="31057" class="Keyword">open</a> <a id="31062" class="Keyword">import</a> <a id="31069" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="31121" class="Keyword">open</a> <a id="31126" class="Keyword">import</a> <a id="31133" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="31186" class="Keyword">open</a> <a id="31191" class="Keyword">import</a> <a id="31198" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="31246" class="Keyword">open</a> <a id="31251" class="Keyword">import</a> <a id="31258" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="31298" class="Keyword">open</a> <a id="31303" class="Keyword">import</a> <a id="31310" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="31357" class="Keyword">open</a> <a id="31362" class="Keyword">import</a> <a id="31369" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="31410" class="Keyword">open</a> <a id="31415" class="Keyword">import</a> <a id="31422" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="31460" class="Keyword">open</a> <a id="31465" class="Keyword">import</a> <a id="31472" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="31517" class="Keyword">open</a> <a id="31522" class="Keyword">import</a> <a id="31529" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="31578" class="Keyword">open</a> <a id="31583" class="Keyword">import</a> <a id="31590" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="31667" class="Keyword">open</a> <a id="31672" class="Keyword">import</a> <a id="31679" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="31731" class="Keyword">open</a> <a id="31736" class="Keyword">import</a> <a id="31743" href="type-theories.html" class="Module">type-theories</a>
<a id="31757" class="Keyword">open</a> <a id="31762" class="Keyword">import</a> <a id="31769" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="31811" class="Keyword">open</a> <a id="31816" class="Keyword">import</a> <a id="31823" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="31861" class="Keyword">open</a> <a id="31866" class="Keyword">import</a> <a id="31873" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="31919" class="Keyword">open</a> <a id="31924" class="Keyword">import</a> <a id="31931" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="31978" class="Keyword">open</a> <a id="31983" class="Keyword">import</a> <a id="31990" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="32025" class="Keyword">open</a> <a id="32030" class="Keyword">import</a> <a id="32037" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="32115" class="Keyword">open</a> <a id="32120" class="Keyword">import</a> <a id="32127" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="32151" class="Keyword">open</a> <a id="32156" class="Keyword">import</a> <a id="32163" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="32216" class="Keyword">open</a> <a id="32221" class="Keyword">import</a> <a id="32228" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="32271" class="Keyword">open</a> <a id="32276" class="Keyword">import</a> <a id="32283" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="32323" class="Keyword">open</a> <a id="32328" class="Keyword">import</a> <a id="32335" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="32374" class="Keyword">open</a> <a id="32379" class="Keyword">import</a> <a id="32386" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="32434" class="Keyword">open</a> <a id="32439" class="Keyword">import</a> <a id="32446" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="32493" class="Keyword">open</a> <a id="32498" class="Keyword">import</a> <a id="32505" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="32557" class="Keyword">open</a> <a id="32562" class="Keyword">import</a> <a id="32569" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="32613" class="Keyword">open</a> <a id="32618" class="Keyword">import</a> <a id="32625" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="32665" class="Keyword">open</a> <a id="32670" class="Keyword">import</a> <a id="32677" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="32729" class="Keyword">open</a> <a id="32734" class="Keyword">import</a> <a id="32741" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="32795" class="Keyword">open</a> <a id="32800" class="Keyword">import</a> <a id="32807" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="32855" class="Keyword">open</a> <a id="32860" class="Keyword">import</a> <a id="32867" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="32906" class="Keyword">open</a> <a id="32911" class="Keyword">import</a> <a id="32918" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="32951" class="Keyword">open</a> <a id="32956" class="Keyword">import</a> <a id="32963" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="32993" class="Keyword">open</a> <a id="32998" class="Keyword">import</a> <a id="33005" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="33064" class="Keyword">open</a> <a id="33069" class="Keyword">import</a> <a id="33076" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="33131" class="Keyword">open</a> <a id="33136" class="Keyword">import</a> <a id="33143" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="33190" class="Keyword">open</a> <a id="33195" class="Keyword">import</a> <a id="33202" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="33245" class="Keyword">open</a> <a id="33250" class="Keyword">import</a> <a id="33257" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="33302" class="Keyword">open</a> <a id="33307" class="Keyword">import</a> <a id="33314" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="33363" class="Keyword">open</a> <a id="33368" class="Keyword">import</a> <a id="33375" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="33426" class="Keyword">open</a> <a id="33431" class="Keyword">import</a> <a id="33438" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="33516" class="Keyword">open</a> <a id="33521" class="Keyword">import</a> <a id="33528" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="33568" class="Keyword">open</a> <a id="33573" class="Keyword">import</a> <a id="33580" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="33637" class="Keyword">open</a> <a id="33642" class="Keyword">import</a> <a id="33649" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="33684" class="Keyword">open</a> <a id="33689" class="Keyword">import</a> <a id="33696" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="33742" class="Keyword">open</a> <a id="33747" class="Keyword">import</a> <a id="33754" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="33809" class="Keyword">open</a> <a id="33814" class="Keyword">import</a> <a id="33821" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="33864" class="Keyword">open</a> <a id="33869" class="Keyword">import</a> <a id="33876" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="33935" class="Keyword">open</a> <a id="33940" class="Keyword">import</a> <a id="33947" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="33984" class="Keyword">open</a> <a id="33989" class="Keyword">import</a> <a id="33996" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="34037" class="Keyword">open</a> <a id="34042" class="Keyword">import</a> <a id="34049" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="34088" class="Keyword">open</a> <a id="34093" class="Keyword">import</a> <a id="34100" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="34138" class="Keyword">open</a> <a id="34143" class="Keyword">import</a> <a id="34150" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="34202" class="Keyword">open</a> <a id="34207" class="Keyword">import</a> <a id="34214" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="34259" class="Keyword">open</a> <a id="34264" class="Keyword">import</a> <a id="34271" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="34308" class="Keyword">open</a> <a id="34313" class="Keyword">import</a> <a id="34320" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="34369" class="Keyword">open</a> <a id="34374" class="Keyword">import</a> <a id="34381" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="34420" class="Keyword">open</a> <a id="34425" class="Keyword">import</a> <a id="34432" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="34470" class="Keyword">open</a> <a id="34475" class="Keyword">import</a> <a id="34482" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="34537" class="Keyword">open</a> <a id="34542" class="Keyword">import</a> <a id="34549" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="34588" class="Keyword">open</a> <a id="34593" class="Keyword">import</a> <a id="34600" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="34648" class="Keyword">open</a> <a id="34653" class="Keyword">import</a> <a id="34660" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="34707" class="Keyword">open</a> <a id="34712" class="Keyword">import</a> <a id="34719" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="34757" class="Keyword">open</a> <a id="34762" class="Keyword">import</a> <a id="34769" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="34799" class="Keyword">open</a> <a id="34804" class="Keyword">import</a> <a id="34811" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="34868" class="Keyword">open</a> <a id="34873" class="Keyword">import</a> <a id="34880" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="34934" class="Keyword">open</a> <a id="34939" class="Keyword">import</a> <a id="34946" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="34976" class="Keyword">open</a> <a id="34981" class="Keyword">import</a> <a id="34988" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="35051" class="Keyword">open</a> <a id="35056" class="Keyword">import</a> <a id="35063" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="35106" class="Keyword">open</a> <a id="35111" class="Keyword">import</a> <a id="35118" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="35153" class="Keyword">open</a> <a id="35158" class="Keyword">import</a> <a id="35165" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="35205" class="Keyword">open</a> <a id="35210" class="Keyword">import</a> <a id="35217" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="35262" class="Keyword">open</a> <a id="35267" class="Keyword">import</a> <a id="35274" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="35324" class="Keyword">open</a> <a id="35329" class="Keyword">import</a> <a id="35336" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="35374" class="Keyword">open</a> <a id="35379" class="Keyword">import</a> <a id="35386" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="35435" class="Keyword">open</a> <a id="35440" class="Keyword">import</a> <a id="35447" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="35494" class="Keyword">open</a> <a id="35499" class="Keyword">import</a> <a id="35506" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="35569" class="Keyword">open</a> <a id="35574" class="Keyword">import</a> <a id="35581" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="35613" class="Keyword">open</a> <a id="35618" class="Keyword">import</a> <a id="35625" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="35678" class="Keyword">open</a> <a id="35683" class="Keyword">import</a> <a id="35690" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="35736" class="Keyword">open</a> <a id="35741" class="Keyword">import</a> <a id="35748" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="35794" class="Keyword">open</a> <a id="35799" class="Keyword">import</a> <a id="35806" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="35854" class="Keyword">open</a> <a id="35859" class="Keyword">import</a> <a id="35866" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="35906" class="Keyword">open</a> <a id="35911" class="Keyword">import</a> <a id="35918" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="35963" class="Keyword">open</a> <a id="35968" class="Keyword">import</a> <a id="35975" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>