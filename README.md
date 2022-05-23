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

<pre class="Agda"><a id="2980" class="Symbol">{-#</a> <a id="2984" class="Keyword">OPTIONS</a> <a id="2992" class="Pragma">--without-K</a> <a id="3004" class="Pragma">--exact-split</a> <a id="3018" class="Pragma">--guardedness</a> <a id="3032" class="Symbol">#-}</a>
</pre>
See the list of all Agda modules [here](everything.html).

## Category theory

<pre class="Agda"><a id="3128" class="Keyword">open</a> <a id="3133" class="Keyword">import</a> <a id="3140" href="category-theory.html" class="Module">category-theory</a>
<a id="3156" class="Keyword">open</a> <a id="3161" class="Keyword">import</a> <a id="3168" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="3216" class="Keyword">open</a> <a id="3221" class="Keyword">import</a> <a id="3228" href="category-theory.anafunctors.html" class="Module">category-theory.anafunctors</a>
<a id="3256" class="Keyword">open</a> <a id="3261" class="Keyword">import</a> <a id="3268" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="3295" class="Keyword">open</a> <a id="3300" class="Keyword">import</a> <a id="3307" href="category-theory.epimorphisms-large-precategories.html" class="Module">category-theory.epimorphisms-large-precategories</a>
<a id="3356" class="Keyword">open</a> <a id="3361" class="Keyword">import</a> <a id="3368" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="3408" class="Keyword">open</a> <a id="3413" class="Keyword">import</a> <a id="3420" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="3469" class="Keyword">open</a> <a id="3474" class="Keyword">import</a> <a id="3481" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="3524" class="Keyword">open</a> <a id="3529" class="Keyword">import</a> <a id="3536" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="3572" class="Keyword">open</a> <a id="3577" class="Keyword">import</a> <a id="3584" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="3629" class="Keyword">open</a> <a id="3634" class="Keyword">import</a> <a id="3641" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="3680" class="Keyword">open</a> <a id="3685" class="Keyword">import</a> <a id="3692" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="3763" class="Keyword">open</a> <a id="3768" class="Keyword">import</a> <a id="3775" href="category-theory.initial-objects-precategories.html" class="Module">category-theory.initial-objects-precategories</a>
<a id="3821" class="Keyword">open</a> <a id="3826" class="Keyword">import</a> <a id="3833" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="3873" class="Keyword">open</a> <a id="3878" class="Keyword">import</a> <a id="3885" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="3934" class="Keyword">open</a> <a id="3939" class="Keyword">import</a> <a id="3946" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="3989" class="Keyword">open</a> <a id="3994" class="Keyword">import</a> <a id="4001" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="4034" class="Keyword">open</a> <a id="4039" class="Keyword">import</a> <a id="4046" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="4082" class="Keyword">open</a> <a id="4087" class="Keyword">import</a> <a id="4094" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="4144" class="Keyword">open</a> <a id="4149" class="Keyword">import</a> <a id="4156" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="4204" class="Keyword">open</a> <a id="4209" class="Keyword">import</a> <a id="4216" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="4273" class="Keyword">open</a> <a id="4278" class="Keyword">import</a> <a id="4285" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="4336" class="Keyword">open</a> <a id="4341" class="Keyword">import</a> <a id="4348" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="4399" class="Keyword">open</a> <a id="4404" class="Keyword">import</a> <a id="4411" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="4471" class="Keyword">open</a> <a id="4476" class="Keyword">import</a> <a id="4483" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="4537" class="Keyword">open</a> <a id="4542" class="Keyword">import</a> <a id="4549" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
<a id="4579" class="Keyword">open</a> <a id="4584" class="Keyword">import</a> <a id="4591" href="category-theory.slice-precategories.html" class="Module">category-theory.slice-precategories</a>
<a id="4627" class="Keyword">open</a> <a id="4632" class="Keyword">import</a> <a id="4639" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Commutative algebra

<pre class="Agda"><a id="4723" class="Keyword">open</a> <a id="4728" class="Keyword">import</a> <a id="4735" href="commutative-algebra.html" class="Module">commutative-algebra</a>
<a id="4755" class="Keyword">open</a> <a id="4760" class="Keyword">import</a> <a id="4767" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>
<a id="4805" class="Keyword">open</a> <a id="4810" class="Keyword">import</a> <a id="4817" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a>
<a id="4853" class="Keyword">open</a> <a id="4858" class="Keyword">import</a> <a id="4865" href="commutative-algebra.eisenstein-integers.html" class="Module">commutative-algebra.eisenstein-integers</a>
<a id="4905" class="Keyword">open</a> <a id="4910" class="Keyword">import</a> <a id="4917" href="commutative-algebra.gaussian-integers.html" class="Module">commutative-algebra.gaussian-integers</a>
<a id="4955" class="Keyword">open</a> <a id="4960" class="Keyword">import</a> <a id="4967" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a>
<a id="5019" class="Keyword">open</a> <a id="5024" class="Keyword">import</a> <a id="5031" href="commutative-algebra.ideals-commutative-rings.html" class="Module">commutative-algebra.ideals-commutative-rings</a>
<a id="5076" class="Keyword">open</a> <a id="5081" class="Keyword">import</a> <a id="5088" href="commutative-algebra.integral-domains.html" class="Module">commutative-algebra.integral-domains</a>
<a id="5125" class="Keyword">open</a> <a id="5130" class="Keyword">import</a> <a id="5137" href="commutative-algebra.isomorphisms-commutative-rings.html" class="Module">commutative-algebra.isomorphisms-commutative-rings</a>
<a id="5188" class="Keyword">open</a> <a id="5193" class="Keyword">import</a> <a id="5200" href="commutative-algebra.prime-ideals-commutative-rings.html" class="Module">commutative-algebra.prime-ideals-commutative-rings</a>
<a id="5251" class="Keyword">open</a> <a id="5256" class="Keyword">import</a> <a id="5263" href="commutative-algebra.zarisky-topology.html" class="Module">commutative-algebra.zarisky-topology</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="5342" class="Keyword">open</a> <a id="5347" class="Keyword">import</a> <a id="5354" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5379" class="Keyword">open</a> <a id="5384" class="Keyword">import</a> <a id="5391" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5440" class="Keyword">open</a> <a id="5445" class="Keyword">import</a> <a id="5452" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5495" class="Keyword">open</a> <a id="5500" class="Keyword">import</a> <a id="5507" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5557" class="Keyword">open</a> <a id="5562" class="Keyword">import</a> <a id="5569" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5615" class="Keyword">open</a> <a id="5620" class="Keyword">import</a> <a id="5627" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5674" class="Keyword">open</a> <a id="5679" class="Keyword">import</a> <a id="5686" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5745" class="Keyword">open</a> <a id="5750" class="Keyword">import</a> <a id="5757" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="5798" class="Keyword">open</a> <a id="5803" class="Keyword">import</a> <a id="5810" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="5853" class="Keyword">open</a> <a id="5858" class="Keyword">import</a> <a id="5865" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="5909" class="Keyword">open</a> <a id="5914" class="Keyword">import</a> <a id="5921" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="5966" class="Keyword">open</a> <a id="5971" class="Keyword">import</a> <a id="5978" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="6030" class="Keyword">open</a> <a id="6035" class="Keyword">import</a> <a id="6042" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="6102" class="Keyword">open</a> <a id="6107" class="Keyword">import</a> <a id="6114" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="6155" class="Keyword">open</a> <a id="6160" class="Keyword">import</a> <a id="6167" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6212" class="Keyword">open</a> <a id="6217" class="Keyword">import</a> <a id="6224" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6271" class="Keyword">open</a> <a id="6276" class="Keyword">import</a> <a id="6283" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6326" class="Keyword">open</a> <a id="6331" class="Keyword">import</a> <a id="6338" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6388" class="Keyword">open</a> <a id="6393" class="Keyword">import</a> <a id="6400" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6447" class="Keyword">open</a> <a id="6452" class="Keyword">import</a> <a id="6459" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6516" class="Keyword">open</a> <a id="6521" class="Keyword">import</a> <a id="6528" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6582" class="Keyword">open</a> <a id="6587" class="Keyword">import</a> <a id="6594" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6654" class="Keyword">open</a> <a id="6659" class="Keyword">import</a> <a id="6666" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6709" class="Keyword">open</a> <a id="6714" class="Keyword">import</a> <a id="6721" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="6771" class="Keyword">open</a> <a id="6776" class="Keyword">import</a> <a id="6783" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="6843" class="Keyword">open</a> <a id="6848" class="Keyword">import</a> <a id="6855" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="6904" class="Keyword">open</a> <a id="6909" class="Keyword">import</a> <a id="6916" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="6972" class="Keyword">open</a> <a id="6977" class="Keyword">import</a> <a id="6984" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="7020" class="Keyword">open</a> <a id="7025" class="Keyword">import</a> <a id="7032" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="7076" class="Keyword">open</a> <a id="7081" class="Keyword">import</a> <a id="7088" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="7132" class="Keyword">open</a> <a id="7137" class="Keyword">import</a> <a id="7144" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7194" class="Keyword">open</a> <a id="7199" class="Keyword">import</a> <a id="7206" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7252" class="Keyword">open</a> <a id="7257" class="Keyword">import</a> <a id="7264" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7299" class="Keyword">open</a> <a id="7304" class="Keyword">import</a> <a id="7311" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7356" class="Keyword">open</a> <a id="7361" class="Keyword">import</a> <a id="7368" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7426" class="Keyword">open</a> <a id="7431" class="Keyword">import</a> <a id="7438" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7503" class="Keyword">open</a> <a id="7508" class="Keyword">import</a> <a id="7515" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7558" class="Keyword">open</a> <a id="7563" class="Keyword">import</a> <a id="7570" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7624" class="Keyword">open</a> <a id="7629" class="Keyword">import</a> <a id="7636" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7681" class="Keyword">open</a> <a id="7686" class="Keyword">import</a> <a id="7693" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7745" class="Keyword">open</a> <a id="7750" class="Keyword">import</a> <a id="7757" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7815" class="Keyword">open</a> <a id="7820" class="Keyword">import</a> <a id="7827" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="7873" class="Keyword">open</a> <a id="7878" class="Keyword">import</a> <a id="7885" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="7929" class="Keyword">open</a> <a id="7934" class="Keyword">import</a> <a id="7941" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="7975" class="Keyword">open</a> <a id="7980" class="Keyword">import</a> <a id="7987" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="8041" class="Keyword">open</a> <a id="8046" class="Keyword">import</a> <a id="8053" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="8102" class="Keyword">open</a> <a id="8107" class="Keyword">import</a> <a id="8114" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="8155" class="Keyword">open</a> <a id="8160" class="Keyword">import</a> <a id="8167" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8216" class="Keyword">open</a> <a id="8221" class="Keyword">import</a> <a id="8228" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8294" class="Keyword">open</a> <a id="8299" class="Keyword">import</a> <a id="8306" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8350" class="Keyword">open</a> <a id="8355" class="Keyword">import</a> <a id="8362" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8411" class="Keyword">open</a> <a id="8416" class="Keyword">import</a> <a id="8423" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8479" class="Keyword">open</a> <a id="8484" class="Keyword">import</a> <a id="8491" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8532" class="Keyword">open</a> <a id="8537" class="Keyword">import</a> <a id="8544" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8593" class="Keyword">open</a> <a id="8598" class="Keyword">import</a> <a id="8605" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8664" class="Keyword">open</a> <a id="8669" class="Keyword">import</a> <a id="8676" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8715" class="Keyword">open</a> <a id="8720" class="Keyword">import</a> <a id="8727" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8780" class="Keyword">open</a> <a id="8785" class="Keyword">import</a> <a id="8792" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="8849" class="Keyword">open</a> <a id="8854" class="Keyword">import</a> <a id="8861" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="8903" class="Keyword">open</a> <a id="8908" class="Keyword">import</a> <a id="8915" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="8966" class="Keyword">open</a> <a id="8971" class="Keyword">import</a> <a id="8978" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9036" class="Keyword">open</a> <a id="9041" class="Keyword">import</a> <a id="9048" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9112" class="Keyword">open</a> <a id="9117" class="Keyword">import</a> <a id="9124" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9177" class="Keyword">open</a> <a id="9182" class="Keyword">import</a> <a id="9189" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9242" class="Keyword">open</a> <a id="9247" class="Keyword">import</a> <a id="9254" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9315" class="Keyword">open</a> <a id="9320" class="Keyword">import</a> <a id="9327" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9385" class="Keyword">open</a> <a id="9390" class="Keyword">import</a> <a id="9397" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9446" class="Keyword">open</a> <a id="9451" class="Keyword">import</a> <a id="9458" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9501" class="Keyword">open</a> <a id="9506" class="Keyword">import</a> <a id="9513" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9557" class="Keyword">open</a> <a id="9562" class="Keyword">import</a> <a id="9569" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9616" class="Keyword">open</a> <a id="9621" class="Keyword">import</a> <a id="9628" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9689" class="Keyword">open</a> <a id="9694" class="Keyword">import</a> <a id="9701" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9764" class="Keyword">open</a> <a id="9769" class="Keyword">import</a> <a id="9776" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="9836" class="Keyword">open</a> <a id="9841" class="Keyword">import</a> <a id="9848" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="9902" class="Keyword">open</a> <a id="9907" class="Keyword">import</a> <a id="9914" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="9979" class="Keyword">open</a> <a id="9984" class="Keyword">import</a> <a id="9991" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10099" class="Keyword">open</a> <a id="10104" class="Keyword">import</a> <a id="10111" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10131" class="Keyword">open</a> <a id="10136" class="Keyword">import</a> <a id="10143" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10189" class="Keyword">open</a> <a id="10194" class="Keyword">import</a> <a id="10201" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10247" class="Keyword">open</a> <a id="10252" class="Keyword">import</a> <a id="10259" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10293" class="Keyword">open</a> <a id="10298" class="Keyword">import</a> <a id="10305" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10340" class="Keyword">open</a> <a id="10345" class="Keyword">import</a> <a id="10352" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10390" class="Keyword">open</a> <a id="10395" class="Keyword">import</a> <a id="10402" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10440" class="Keyword">open</a> <a id="10445" class="Keyword">import</a> <a id="10452" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10492" class="Keyword">open</a> <a id="10497" class="Keyword">import</a> <a id="10504" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10537" class="Keyword">open</a> <a id="10542" class="Keyword">import</a> <a id="10549" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10587" class="Keyword">open</a> <a id="10592" class="Keyword">import</a> <a id="10599" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10662" class="Keyword">open</a> <a id="10667" class="Keyword">import</a> <a id="10674" href="foundation.html" class="Module">foundation</a>
<a id="10685" class="Keyword">open</a> <a id="10690" class="Keyword">import</a> <a id="10697" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10715" class="Keyword">open</a> <a id="10720" class="Keyword">import</a> <a id="10727" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10746" class="Keyword">open</a> <a id="10751" class="Keyword">import</a> <a id="10758" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10777" class="Keyword">open</a> <a id="10782" class="Keyword">import</a> <a id="10789" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="10833" class="Keyword">open</a> <a id="10838" class="Keyword">import</a> <a id="10845" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="10870" class="Keyword">open</a> <a id="10875" class="Keyword">import</a> <a id="10882" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="10909" class="Keyword">open</a> <a id="10914" class="Keyword">import</a> <a id="10921" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="10938" class="Keyword">open</a> <a id="10943" class="Keyword">import</a> <a id="10950" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="10979" class="Keyword">open</a> <a id="10984" class="Keyword">import</a> <a id="10991" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11047" class="Keyword">open</a> <a id="11052" class="Keyword">import</a> <a id="11059" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="11090" class="Keyword">open</a> <a id="11095" class="Keyword">import</a> <a id="11102" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="11156" class="Keyword">open</a> <a id="11161" class="Keyword">import</a> <a id="11168" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="11196" class="Keyword">open</a> <a id="11201" class="Keyword">import</a> <a id="11208" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11238" class="Keyword">open</a> <a id="11243" class="Keyword">import</a> <a id="11250" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11270" class="Keyword">open</a> <a id="11275" class="Keyword">import</a> <a id="11282" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="11327" class="Keyword">open</a> <a id="11332" class="Keyword">import</a> <a id="11339" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11376" class="Keyword">open</a> <a id="11381" class="Keyword">import</a> <a id="11388" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11423" class="Keyword">open</a> <a id="11428" class="Keyword">import</a> <a id="11435" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11493" class="Keyword">open</a> <a id="11498" class="Keyword">import</a> <a id="11505" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11543" class="Keyword">open</a> <a id="11548" class="Keyword">import</a> <a id="11555" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11589" class="Keyword">open</a> <a id="11594" class="Keyword">import</a> <a id="11601" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11630" class="Keyword">open</a> <a id="11635" class="Keyword">import</a> <a id="11642" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11665" class="Keyword">open</a> <a id="11670" class="Keyword">import</a> <a id="11677" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="11704" class="Keyword">open</a> <a id="11709" class="Keyword">import</a> <a id="11716" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11739" class="Keyword">open</a> <a id="11744" class="Keyword">import</a> <a id="11751" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="11793" class="Keyword">open</a> <a id="11798" class="Keyword">import</a> <a id="11805" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="11837" class="Keyword">open</a> <a id="11842" class="Keyword">import</a> <a id="11849" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="11876" class="Keyword">open</a> <a id="11881" class="Keyword">import</a> <a id="11888" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="11913" class="Keyword">open</a> <a id="11918" class="Keyword">import</a> <a id="11925" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="11954" class="Keyword">open</a> <a id="11959" class="Keyword">import</a> <a id="11966" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="11996" class="Keyword">open</a> <a id="12001" class="Keyword">import</a> <a id="12008" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="12035" class="Keyword">open</a> <a id="12040" class="Keyword">import</a> <a id="12047" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="12066" class="Keyword">open</a> <a id="12071" class="Keyword">import</a> <a id="12078" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="12124" class="Keyword">open</a> <a id="12129" class="Keyword">import</a> <a id="12136" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="12178" class="Keyword">open</a> <a id="12183" class="Keyword">import</a> <a id="12190" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="12222" class="Keyword">open</a> <a id="12227" class="Keyword">import</a> <a id="12234" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="12264" class="Keyword">open</a> <a id="12269" class="Keyword">import</a> <a id="12276" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12302" class="Keyword">open</a> <a id="12307" class="Keyword">import</a> <a id="12314" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12348" class="Keyword">open</a> <a id="12353" class="Keyword">import</a> <a id="12360" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12390" class="Keyword">open</a> <a id="12395" class="Keyword">import</a> <a id="12402" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12429" class="Keyword">open</a> <a id="12434" class="Keyword">import</a> <a id="12441" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12473" class="Keyword">open</a> <a id="12478" class="Keyword">import</a> <a id="12485" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12519" class="Keyword">open</a> <a id="12524" class="Keyword">import</a> <a id="12531" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12554" class="Keyword">open</a> <a id="12559" class="Keyword">import</a> <a id="12566" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="12636" class="Keyword">open</a> <a id="12641" class="Keyword">import</a> <a id="12648" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="12718" class="Keyword">open</a> <a id="12723" class="Keyword">import</a> <a id="12730" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12757" class="Keyword">open</a> <a id="12762" class="Keyword">import</a> <a id="12769" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12797" class="Keyword">open</a> <a id="12802" class="Keyword">import</a> <a id="12809" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12846" class="Keyword">open</a> <a id="12851" class="Keyword">import</a> <a id="12858" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12906" class="Keyword">open</a> <a id="12911" class="Keyword">import</a> <a id="12918" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="12958" class="Keyword">open</a> <a id="12963" class="Keyword">import</a> <a id="12970" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="12992" class="Keyword">open</a> <a id="12997" class="Keyword">import</a> <a id="13004" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="13027" class="Keyword">open</a> <a id="13032" class="Keyword">import</a> <a id="13039" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="13064" class="Keyword">open</a> <a id="13069" class="Keyword">import</a> <a id="13076" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="13121" class="Keyword">open</a> <a id="13126" class="Keyword">import</a> <a id="13133" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="13177" class="Keyword">open</a> <a id="13182" class="Keyword">import</a> <a id="13189" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="13225" class="Keyword">open</a> <a id="13230" class="Keyword">import</a> <a id="13237" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="13282" class="Keyword">open</a> <a id="13287" class="Keyword">import</a> <a id="13294" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13335" class="Keyword">open</a> <a id="13340" class="Keyword">import</a> <a id="13347" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13382" class="Keyword">open</a> <a id="13387" class="Keyword">import</a> <a id="13394" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13425" class="Keyword">open</a> <a id="13430" class="Keyword">import</a> <a id="13437" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13470" class="Keyword">open</a> <a id="13475" class="Keyword">import</a> <a id="13482" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13515" class="Keyword">open</a> <a id="13520" class="Keyword">import</a> <a id="13527" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13557" class="Keyword">open</a> <a id="13562" class="Keyword">import</a> <a id="13569" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13593" class="Keyword">open</a> <a id="13598" class="Keyword">import</a> <a id="13605" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13643" class="Keyword">open</a> <a id="13648" class="Keyword">import</a> <a id="13655" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13686" class="Keyword">open</a> <a id="13691" class="Keyword">import</a> <a id="13698" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13723" class="Keyword">open</a> <a id="13728" class="Keyword">import</a> <a id="13735" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13763" class="Keyword">open</a> <a id="13768" class="Keyword">import</a> <a id="13775" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13799" class="Keyword">open</a> <a id="13804" class="Keyword">import</a> <a id="13811" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13837" class="Keyword">open</a> <a id="13842" class="Keyword">import</a> <a id="13849" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="13884" class="Keyword">open</a> <a id="13889" class="Keyword">import</a> <a id="13896" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="13917" class="Keyword">open</a> <a id="13922" class="Keyword">import</a> <a id="13929" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="13978" class="Keyword">open</a> <a id="13983" class="Keyword">import</a> <a id="13990" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="14031" class="Keyword">open</a> <a id="14036" class="Keyword">import</a> <a id="14043" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="14093" class="Keyword">open</a> <a id="14098" class="Keyword">import</a> <a id="14105" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="14151" class="Keyword">open</a> <a id="14156" class="Keyword">import</a> <a id="14163" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="14203" class="Keyword">open</a> <a id="14208" class="Keyword">import</a> <a id="14215" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="14265" class="Keyword">open</a> <a id="14270" class="Keyword">import</a> <a id="14277" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14316" class="Keyword">open</a> <a id="14321" class="Keyword">import</a> <a id="14328" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14368" class="Keyword">open</a> <a id="14373" class="Keyword">import</a> <a id="14380" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14413" class="Keyword">open</a> <a id="14418" class="Keyword">import</a> <a id="14425" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14474" class="Keyword">open</a> <a id="14479" class="Keyword">import</a> <a id="14486" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14511" class="Keyword">open</a> <a id="14516" class="Keyword">import</a> <a id="14523" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14561" class="Keyword">open</a> <a id="14566" class="Keyword">import</a> <a id="14573" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14595" class="Keyword">open</a> <a id="14600" class="Keyword">import</a> <a id="14607" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14635" class="Keyword">open</a> <a id="14640" class="Keyword">import</a> <a id="14647" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14673" class="Keyword">open</a> <a id="14678" class="Keyword">import</a> <a id="14685" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14703" class="Keyword">open</a> <a id="14708" class="Keyword">import</a> <a id="14715" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14750" class="Keyword">open</a> <a id="14755" class="Keyword">import</a> <a id="14762" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="14789" class="Keyword">open</a> <a id="14794" class="Keyword">import</a> <a id="14801" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="14857" class="Keyword">open</a> <a id="14862" class="Keyword">import</a> <a id="14869" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="14898" class="Keyword">open</a> <a id="14903" class="Keyword">import</a> <a id="14910" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="14940" class="Keyword">open</a> <a id="14945" class="Keyword">import</a> <a id="14952" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="14979" class="Keyword">open</a> <a id="14984" class="Keyword">import</a> <a id="14991" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="15017" class="Keyword">open</a> <a id="15022" class="Keyword">import</a> <a id="15029" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="15056" class="Keyword">open</a> <a id="15061" class="Keyword">import</a> <a id="15068" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="15092" class="Keyword">open</a> <a id="15097" class="Keyword">import</a> <a id="15104" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="15127" class="Keyword">open</a> <a id="15132" class="Keyword">import</a> <a id="15139" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="15166" class="Keyword">open</a> <a id="15171" class="Keyword">import</a> <a id="15178" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="15210" class="Keyword">open</a> <a id="15215" class="Keyword">import</a> <a id="15222" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="15257" class="Keyword">open</a> <a id="15262" class="Keyword">import</a> <a id="15269" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15300" class="Keyword">open</a> <a id="15305" class="Keyword">import</a> <a id="15312" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15345" class="Keyword">open</a> <a id="15350" class="Keyword">import</a> <a id="15357" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15391" class="Keyword">open</a> <a id="15396" class="Keyword">import</a> <a id="15403" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15443" class="Keyword">open</a> <a id="15448" class="Keyword">import</a> <a id="15455" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15486" class="Keyword">open</a> <a id="15491" class="Keyword">import</a> <a id="15498" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15530" class="Keyword">open</a> <a id="15535" class="Keyword">import</a> <a id="15542" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15573" class="Keyword">open</a> <a id="15578" class="Keyword">import</a> <a id="15585" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15602" class="Keyword">open</a> <a id="15607" class="Keyword">import</a> <a id="15614" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15639" class="Keyword">open</a> <a id="15644" class="Keyword">import</a> <a id="15651" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15680" class="Keyword">open</a> <a id="15685" class="Keyword">import</a> <a id="15692" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15717" class="Keyword">open</a> <a id="15722" class="Keyword">import</a> <a id="15729" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15750" class="Keyword">open</a> <a id="15755" class="Keyword">import</a> <a id="15762" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="15786" class="Keyword">open</a> <a id="15791" class="Keyword">import</a> <a id="15798" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="15818" class="Keyword">open</a> <a id="15823" class="Keyword">import</a> <a id="15830" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="15864" class="Keyword">open</a> <a id="15869" class="Keyword">import</a> <a id="15876" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="15914" class="Keyword">open</a> <a id="15919" class="Keyword">import</a> <a id="15926" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="15950" class="Keyword">open</a> <a id="15955" class="Keyword">import</a> <a id="15962" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="15989" class="Keyword">open</a> <a id="15994" class="Keyword">import</a> <a id="16001" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="16036" class="Keyword">open</a> <a id="16041" class="Keyword">import</a> <a id="16048" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="16069" class="Keyword">open</a> <a id="16074" class="Keyword">import</a> <a id="16081" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="16117" class="Keyword">open</a> <a id="16122" class="Keyword">import</a> <a id="16129" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="16174" class="Keyword">open</a> <a id="16179" class="Keyword">import</a> <a id="16186" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="16232" class="Keyword">open</a> <a id="16237" class="Keyword">import</a> <a id="16244" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="16284" class="Keyword">open</a> <a id="16289" class="Keyword">import</a> <a id="16296" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16326" class="Keyword">open</a> <a id="16331" class="Keyword">import</a> <a id="16338" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16375" class="Keyword">open</a> <a id="16380" class="Keyword">import</a> <a id="16387" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16411" class="Keyword">open</a> <a id="16416" class="Keyword">import</a> <a id="16423" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16444" class="Keyword">open</a> <a id="16449" class="Keyword">import</a> <a id="16456" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16491" class="Keyword">open</a> <a id="16496" class="Keyword">import</a> <a id="16503" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16540" class="Keyword">open</a> <a id="16545" class="Keyword">import</a> <a id="16552" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16601" class="Keyword">open</a> <a id="16606" class="Keyword">import</a> <a id="16613" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16646" class="Keyword">open</a> <a id="16651" class="Keyword">import</a> <a id="16658" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16681" class="Keyword">open</a> <a id="16686" class="Keyword">import</a> <a id="16693" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="16716" class="Keyword">open</a> <a id="16721" class="Keyword">import</a> <a id="16728" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="16751" class="Keyword">open</a> <a id="16756" class="Keyword">import</a> <a id="16763" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="16791" class="Keyword">open</a> <a id="16796" class="Keyword">import</a> <a id="16803" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="16823" class="Keyword">open</a> <a id="16828" class="Keyword">import</a> <a id="16835" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="16856" class="Keyword">open</a> <a id="16861" class="Keyword">import</a> <a id="16868" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="16899" class="Keyword">open</a> <a id="16904" class="Keyword">import</a> <a id="16911" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="16938" class="Keyword">open</a> <a id="16943" class="Keyword">import</a> <a id="16950" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="16966" class="Keyword">open</a> <a id="16971" class="Keyword">import</a> <a id="16978" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="17009" class="Keyword">open</a> <a id="17014" class="Keyword">import</a> <a id="17021" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="17038" class="Keyword">open</a> <a id="17043" class="Keyword">import</a> <a id="17050" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="17072" class="Keyword">open</a> <a id="17077" class="Keyword">import</a> <a id="17084" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="17111" class="Keyword">open</a> <a id="17116" class="Keyword">import</a> <a id="17123" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="17146" class="Keyword">open</a> <a id="17151" class="Keyword">import</a> <a id="17158" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="17185" class="Keyword">open</a> <a id="17190" class="Keyword">import</a> <a id="17197" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="17230" class="Keyword">open</a> <a id="17235" class="Keyword">import</a> <a id="17242" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="17282" class="Keyword">open</a> <a id="17287" class="Keyword">import</a> <a id="17294" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17315" class="Keyword">open</a> <a id="17320" class="Keyword">import</a> <a id="17327" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17356" class="Keyword">open</a> <a id="17361" class="Keyword">import</a> <a id="17368" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17406" class="Keyword">open</a> <a id="17411" class="Keyword">import</a> <a id="17418" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17438" class="Keyword">open</a> <a id="17443" class="Keyword">import</a> <a id="17450" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17474" class="Keyword">open</a> <a id="17479" class="Keyword">import</a> <a id="17486" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17513" class="Keyword">open</a> <a id="17518" class="Keyword">import</a> <a id="17525" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17557" class="Keyword">open</a> <a id="17562" class="Keyword">import</a> <a id="17569" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17599" class="Keyword">open</a> <a id="17604" class="Keyword">import</a> <a id="17611" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17637" class="Keyword">open</a> <a id="17642" class="Keyword">import</a> <a id="17649" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17676" class="Keyword">open</a> <a id="17681" class="Keyword">import</a> <a id="17688" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="17717" class="Keyword">open</a> <a id="17722" class="Keyword">import</a> <a id="17729" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="17752" class="Keyword">open</a> <a id="17757" class="Keyword">import</a> <a id="17764" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="17815" class="Keyword">open</a> <a id="17820" class="Keyword">import</a> <a id="17827" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="17870" class="Keyword">open</a> <a id="17875" class="Keyword">import</a> <a id="17882" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="17930" class="Keyword">open</a> <a id="17935" class="Keyword">import</a> <a id="17942" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="17980" class="Keyword">open</a> <a id="17985" class="Keyword">import</a> <a id="17992" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="18029" class="Keyword">open</a> <a id="18034" class="Keyword">import</a> <a id="18041" href="foundation.union.html" class="Module">foundation.union</a>
<a id="18058" class="Keyword">open</a> <a id="18063" class="Keyword">import</a> <a id="18070" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="18098" class="Keyword">open</a> <a id="18103" class="Keyword">import</a> <a id="18110" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="18146" class="Keyword">open</a> <a id="18151" class="Keyword">import</a> <a id="18158" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="18196" class="Keyword">open</a> <a id="18201" class="Keyword">import</a> <a id="18208" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="18241" class="Keyword">open</a> <a id="18246" class="Keyword">import</a> <a id="18253" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="18274" class="Keyword">open</a> <a id="18279" class="Keyword">import</a> <a id="18286" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18340" class="Keyword">open</a> <a id="18345" class="Keyword">import</a> <a id="18352" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18374" class="Keyword">open</a> <a id="18379" class="Keyword">import</a> <a id="18386" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18421" class="Keyword">open</a> <a id="18426" class="Keyword">import</a> <a id="18433" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18463" class="Keyword">open</a> <a id="18468" class="Keyword">import</a> <a id="18475" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18514" class="Keyword">open</a> <a id="18519" class="Keyword">import</a> <a id="18526" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18580" class="Keyword">open</a> <a id="18585" class="Keyword">import</a> <a id="18592" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18638" class="Keyword">open</a> <a id="18643" class="Keyword">import</a> <a id="18650" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18701" class="Keyword">open</a> <a id="18706" class="Keyword">import</a> <a id="18713" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="18754" class="Keyword">open</a> <a id="18759" class="Keyword">import</a> <a id="18766" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="18811" class="Keyword">open</a> <a id="18816" class="Keyword">import</a> <a id="18823" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="18868" class="Keyword">open</a> <a id="18873" class="Keyword">import</a> <a id="18880" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="18916" class="Keyword">open</a> <a id="18921" class="Keyword">import</a> <a id="18928" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="18964" class="Keyword">open</a> <a id="18969" class="Keyword">import</a> <a id="18976" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="19041" class="Keyword">open</a> <a id="19046" class="Keyword">import</a> <a id="19053" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="19108" class="Keyword">open</a> <a id="19113" class="Keyword">import</a> <a id="19120" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="19160" class="Keyword">open</a> <a id="19165" class="Keyword">import</a> <a id="19172" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="19216" class="Keyword">open</a> <a id="19221" class="Keyword">import</a> <a id="19228" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="19273" class="Keyword">open</a> <a id="19278" class="Keyword">import</a> <a id="19285" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19326" class="Keyword">open</a> <a id="19331" class="Keyword">import</a> <a id="19338" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19378" class="Keyword">open</a> <a id="19383" class="Keyword">import</a> <a id="19390" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19417" class="Keyword">open</a> <a id="19422" class="Keyword">import</a> <a id="19429" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19465" class="Keyword">open</a> <a id="19470" class="Keyword">import</a> <a id="19477" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19504" class="Keyword">open</a> <a id="19509" class="Keyword">import</a> <a id="19516" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19553" class="Keyword">open</a> <a id="19558" class="Keyword">import</a> <a id="19565" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19593" class="Keyword">open</a> <a id="19598" class="Keyword">import</a> <a id="19605" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19624" class="Keyword">open</a> <a id="19629" class="Keyword">import</a> <a id="19636" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19676" class="Keyword">open</a> <a id="19681" class="Keyword">import</a> <a id="19688" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19720" class="Keyword">open</a> <a id="19725" class="Keyword">import</a> <a id="19732" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="19780" class="Keyword">open</a> <a id="19785" class="Keyword">import</a> <a id="19792" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="19815" class="Keyword">open</a> <a id="19820" class="Keyword">import</a> <a id="19827" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="19851" class="Keyword">open</a> <a id="19856" class="Keyword">import</a> <a id="19863" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="19903" class="Keyword">open</a> <a id="19908" class="Keyword">import</a> <a id="19915" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="19958" class="Keyword">open</a> <a id="19963" class="Keyword">import</a> <a id="19970" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="20004" class="Keyword">open</a> <a id="20009" class="Keyword">import</a> <a id="20016" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="20048" class="Keyword">open</a> <a id="20053" class="Keyword">import</a> <a id="20060" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="20090" class="Keyword">open</a> <a id="20095" class="Keyword">import</a> <a id="20102" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="20136" class="Keyword">open</a> <a id="20141" class="Keyword">import</a> <a id="20148" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="20183" class="Keyword">open</a> <a id="20188" class="Keyword">import</a> <a id="20195" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="20232" class="Keyword">open</a> <a id="20237" class="Keyword">import</a> <a id="20244" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="20271" class="Keyword">open</a> <a id="20276" class="Keyword">import</a> <a id="20283" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="20311" class="Keyword">open</a> <a id="20316" class="Keyword">import</a> <a id="20323" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20372" class="Keyword">open</a> <a id="20377" class="Keyword">import</a> <a id="20384" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20430" class="Keyword">open</a> <a id="20435" class="Keyword">import</a> <a id="20442" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20482" class="Keyword">open</a> <a id="20487" class="Keyword">import</a> <a id="20494" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20532" class="Keyword">open</a> <a id="20537" class="Keyword">import</a> <a id="20544" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20573" class="Keyword">open</a> <a id="20578" class="Keyword">import</a> <a id="20585" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20615" class="Keyword">open</a> <a id="20620" class="Keyword">import</a> <a id="20627" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20658" class="Keyword">open</a> <a id="20663" class="Keyword">import</a> <a id="20670" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="20710" class="Keyword">open</a> <a id="20715" class="Keyword">import</a> <a id="20722" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="20748" class="Keyword">open</a> <a id="20753" class="Keyword">import</a> <a id="20760" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="20815" class="Keyword">open</a> <a id="20820" class="Keyword">import</a> <a id="20827" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="20878" class="Keyword">open</a> <a id="20883" class="Keyword">import</a> <a id="20890" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="20935" class="Keyword">open</a> <a id="20940" class="Keyword">import</a> <a id="20947" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="21001" class="Keyword">open</a> <a id="21006" class="Keyword">import</a> <a id="21013" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="21040" class="Keyword">open</a> <a id="21045" class="Keyword">import</a> <a id="21052" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="21085" class="Keyword">open</a> <a id="21090" class="Keyword">import</a> <a id="21097" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="21128" class="Keyword">open</a> <a id="21133" class="Keyword">import</a> <a id="21140" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="21177" class="Keyword">open</a> <a id="21182" class="Keyword">import</a> <a id="21189" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="21214" class="Keyword">open</a> <a id="21219" class="Keyword">import</a> <a id="21226" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="21258" class="Keyword">open</a> <a id="21263" class="Keyword">import</a> <a id="21270" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="21305" class="Keyword">open</a> <a id="21310" class="Keyword">import</a> <a id="21317" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="21346" class="Keyword">open</a> <a id="21351" class="Keyword">import</a> <a id="21358" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="21384" class="Keyword">open</a> <a id="21389" class="Keyword">import</a> <a id="21396" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="21424" class="Keyword">open</a> <a id="21429" class="Keyword">import</a> <a id="21436" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="21461" class="Keyword">open</a> <a id="21466" class="Keyword">import</a> <a id="21473" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="21494" class="Keyword">open</a> <a id="21499" class="Keyword">import</a> <a id="21506" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="21542" class="Keyword">open</a> <a id="21547" class="Keyword">import</a> <a id="21554" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21597" class="Keyword">open</a> <a id="21602" class="Keyword">import</a> <a id="21609" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21634" class="Keyword">open</a> <a id="21639" class="Keyword">import</a> <a id="21646" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21677" class="Keyword">open</a> <a id="21682" class="Keyword">import</a> <a id="21689" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21721" class="Keyword">open</a> <a id="21726" class="Keyword">import</a> <a id="21733" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="21767" class="Keyword">open</a> <a id="21772" class="Keyword">import</a> <a id="21779" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="21835" class="Keyword">open</a> <a id="21840" class="Keyword">import</a> <a id="21847" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="21900" class="Keyword">open</a> <a id="21905" class="Keyword">import</a> <a id="21912" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="21939" class="Keyword">open</a> <a id="21944" class="Keyword">import</a> <a id="21951" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="21996" class="Keyword">open</a> <a id="22001" class="Keyword">import</a> <a id="22008" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="22070" class="Keyword">open</a> <a id="22075" class="Keyword">import</a> <a id="22082" href="graph-theory.html" class="Module">graph-theory</a>
<a id="22095" class="Keyword">open</a> <a id="22100" class="Keyword">import</a> <a id="22107" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="22148" class="Keyword">open</a> <a id="22153" class="Keyword">import</a> <a id="22160" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="22189" class="Keyword">open</a> <a id="22194" class="Keyword">import</a> <a id="22201" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="22246" class="Keyword">open</a> <a id="22251" class="Keyword">import</a> <a id="22258" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="22302" class="Keyword">open</a> <a id="22307" class="Keyword">import</a> <a id="22314" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="22341" class="Keyword">open</a> <a id="22346" class="Keyword">import</a> <a id="22353" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="22394" class="Keyword">open</a> <a id="22399" class="Keyword">import</a> <a id="22406" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="22429" class="Keyword">open</a> <a id="22434" class="Keyword">import</a> <a id="22441" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="22490" class="Keyword">open</a> <a id="22495" class="Keyword">import</a> <a id="22502" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="22541" class="Keyword">open</a> <a id="22546" class="Keyword">import</a> <a id="22553" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="22594" class="Keyword">open</a> <a id="22599" class="Keyword">import</a> <a id="22606" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22650" class="Keyword">open</a> <a id="22655" class="Keyword">import</a> <a id="22662" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22699" class="Keyword">open</a> <a id="22704" class="Keyword">import</a> <a id="22711" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="22733" class="Keyword">open</a> <a id="22738" class="Keyword">import</a> <a id="22745" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="22775" class="Keyword">open</a> <a id="22780" class="Keyword">import</a> <a id="22787" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="22826" class="Keyword">open</a> <a id="22831" class="Keyword">import</a> <a id="22838" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="22876" class="Keyword">open</a> <a id="22881" class="Keyword">import</a> <a id="22888" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="22919" class="Keyword">open</a> <a id="22924" class="Keyword">import</a> <a id="22931" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="22958" class="Keyword">open</a> <a id="22963" class="Keyword">import</a> <a id="22970" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="23028" class="Keyword">open</a> <a id="23033" class="Keyword">import</a> <a id="23040" href="group-theory.html" class="Module">group-theory</a>
<a id="23053" class="Keyword">open</a> <a id="23058" class="Keyword">import</a> <a id="23065" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="23093" class="Keyword">open</a> <a id="23098" class="Keyword">import</a> <a id="23105" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="23136" class="Keyword">open</a> <a id="23141" class="Keyword">import</a> <a id="23148" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="23184" class="Keyword">open</a> <a id="23189" class="Keyword">import</a> <a id="23196" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="23247" class="Keyword">open</a> <a id="23252" class="Keyword">import</a> <a id="23259" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="23292" class="Keyword">open</a> <a id="23297" class="Keyword">import</a> <a id="23304" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="23351" class="Keyword">open</a> <a id="23356" class="Keyword">import</a> <a id="23363" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="23402" class="Keyword">open</a> <a id="23407" class="Keyword">import</a> <a id="23414" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="23454" class="Keyword">open</a> <a id="23459" class="Keyword">import</a> <a id="23466" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="23509" class="Keyword">open</a> <a id="23514" class="Keyword">import</a> <a id="23521" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="23553" class="Keyword">open</a> <a id="23558" class="Keyword">import</a> <a id="23565" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="23601" class="Keyword">open</a> <a id="23606" class="Keyword">import</a> <a id="23613" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="23642" class="Keyword">open</a> <a id="23647" class="Keyword">import</a> <a id="23654" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="23687" class="Keyword">open</a> <a id="23692" class="Keyword">import</a> <a id="23699" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="23735" class="Keyword">open</a> <a id="23740" class="Keyword">import</a> <a id="23747" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="23776" class="Keyword">open</a> <a id="23781" class="Keyword">import</a> <a id="23788" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="23820" class="Keyword">open</a> <a id="23825" class="Keyword">import</a> <a id="23832" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="23857" class="Keyword">open</a> <a id="23862" class="Keyword">import</a> <a id="23869" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="23900" class="Keyword">open</a> <a id="23905" class="Keyword">import</a> <a id="23912" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="23959" class="Keyword">open</a> <a id="23964" class="Keyword">import</a> <a id="23971" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="24004" class="Keyword">open</a> <a id="24009" class="Keyword">import</a> <a id="24016" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="24056" class="Keyword">open</a> <a id="24061" class="Keyword">import</a> <a id="24068" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="24105" class="Keyword">open</a> <a id="24110" class="Keyword">import</a> <a id="24117" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="24153" class="Keyword">open</a> <a id="24158" class="Keyword">import</a> <a id="24165" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="24197" class="Keyword">open</a> <a id="24202" class="Keyword">import</a> <a id="24209" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="24236" class="Keyword">open</a> <a id="24241" class="Keyword">import</a> <a id="24248" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="24268" class="Keyword">open</a> <a id="24273" class="Keyword">import</a> <a id="24280" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="24307" class="Keyword">open</a> <a id="24312" class="Keyword">import</a> <a id="24319" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="24361" class="Keyword">open</a> <a id="24366" class="Keyword">import</a> <a id="24373" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="24420" class="Keyword">open</a> <a id="24425" class="Keyword">import</a> <a id="24432" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="24473" class="Keyword">open</a> <a id="24478" class="Keyword">import</a> <a id="24485" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="24519" class="Keyword">open</a> <a id="24524" class="Keyword">import</a> <a id="24531" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="24566" class="Keyword">open</a> <a id="24571" class="Keyword">import</a> <a id="24578" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="24616" class="Keyword">open</a> <a id="24621" class="Keyword">import</a> <a id="24628" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="24660" class="Keyword">open</a> <a id="24665" class="Keyword">import</a> <a id="24672" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="24713" class="Keyword">open</a> <a id="24718" class="Keyword">import</a> <a id="24725" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="24766" class="Keyword">open</a> <a id="24771" class="Keyword">import</a> <a id="24778" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="24818" class="Keyword">open</a> <a id="24823" class="Keyword">import</a> <a id="24830" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="24863" class="Keyword">open</a> <a id="24868" class="Keyword">import</a> <a id="24875" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="24912" class="Keyword">open</a> <a id="24917" class="Keyword">import</a> <a id="24924" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="24969" class="Keyword">open</a> <a id="24974" class="Keyword">import</a> <a id="24981" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="25009" class="Keyword">open</a> <a id="25014" class="Keyword">import</a> <a id="25021" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="25042" class="Keyword">open</a> <a id="25047" class="Keyword">import</a> <a id="25054" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="25088" class="Keyword">open</a> <a id="25093" class="Keyword">import</a> <a id="25100" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="25134" class="Keyword">open</a> <a id="25139" class="Keyword">import</a> <a id="25146" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="25181" class="Keyword">open</a> <a id="25186" class="Keyword">import</a> <a id="25193" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="25235" class="Keyword">open</a> <a id="25240" class="Keyword">import</a> <a id="25247" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="25282" class="Keyword">open</a> <a id="25287" class="Keyword">import</a> <a id="25294" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="25333" class="Keyword">open</a> <a id="25338" class="Keyword">import</a> <a id="25345" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="25382" class="Keyword">open</a> <a id="25387" class="Keyword">import</a> <a id="25394" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="25418" class="Keyword">open</a> <a id="25423" class="Keyword">import</a> <a id="25430" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="25455" class="Keyword">open</a> <a id="25460" class="Keyword">import</a> <a id="25467" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="25498" class="Keyword">open</a> <a id="25503" class="Keyword">import</a> <a id="25510" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="25561" class="Keyword">open</a> <a id="25566" class="Keyword">import</a> <a id="25573" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="25596" class="Keyword">open</a> <a id="25601" class="Keyword">import</a> <a id="25608" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="25656" class="Keyword">open</a> <a id="25661" class="Keyword">import</a> <a id="25668" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="25698" class="Keyword">open</a> <a id="25703" class="Keyword">import</a> <a id="25710" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="25780" class="Keyword">open</a> <a id="25785" class="Keyword">import</a> <a id="25792" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="25807" class="Keyword">open</a> <a id="25812" class="Keyword">import</a> <a id="25819" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="25852" class="Keyword">open</a> <a id="25857" class="Keyword">import</a> <a id="25864" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="25896" class="Keyword">open</a> <a id="25901" class="Keyword">import</a> <a id="25908" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="25950" class="Keyword">open</a> <a id="25955" class="Keyword">import</a> <a id="25962" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="26000" class="Keyword">open</a> <a id="26005" class="Keyword">import</a> <a id="26012" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="26049" class="Keyword">open</a> <a id="26054" class="Keyword">import</a> <a id="26061" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="26094" class="Keyword">open</a> <a id="26099" class="Keyword">import</a> <a id="26106" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="26130" class="Keyword">open</a> <a id="26135" class="Keyword">import</a> <a id="26142" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="26181" class="Keyword">open</a> <a id="26186" class="Keyword">import</a> <a id="26193" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="26239" class="Keyword">open</a> <a id="26244" class="Keyword">import</a> <a id="26251" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="26296" class="Keyword">open</a> <a id="26301" class="Keyword">import</a> <a id="26308" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="26346" class="Keyword">open</a> <a id="26351" class="Keyword">import</a> <a id="26358" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="26390" class="Keyword">open</a> <a id="26395" class="Keyword">import</a> <a id="26402" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="26455" class="Keyword">open</a> <a id="26460" class="Keyword">import</a> <a id="26467" href="order-theory.html" class="Module">order-theory</a>
<a id="26480" class="Keyword">open</a> <a id="26485" class="Keyword">import</a> <a id="26492" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="26519" class="Keyword">open</a> <a id="26524" class="Keyword">import</a> <a id="26531" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="26561" class="Keyword">open</a> <a id="26566" class="Keyword">import</a> <a id="26573" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="26606" class="Keyword">open</a> <a id="26611" class="Keyword">import</a> <a id="26618" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="26654" class="Keyword">open</a> <a id="26659" class="Keyword">import</a> <a id="26666" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="26693" class="Keyword">open</a> <a id="26698" class="Keyword">import</a> <a id="26705" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="26735" class="Keyword">open</a> <a id="26740" class="Keyword">import</a> <a id="26747" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="26783" class="Keyword">open</a> <a id="26788" class="Keyword">import</a> <a id="26795" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="26837" class="Keyword">open</a> <a id="26842" class="Keyword">import</a> <a id="26849" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="26881" class="Keyword">open</a> <a id="26886" class="Keyword">import</a> <a id="26893" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="26924" class="Keyword">open</a> <a id="26929" class="Keyword">import</a> <a id="26936" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="26962" class="Keyword">open</a> <a id="26967" class="Keyword">import</a> <a id="26974" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="27003" class="Keyword">open</a> <a id="27008" class="Keyword">import</a> <a id="27015" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="27052" class="Keyword">open</a> <a id="27057" class="Keyword">import</a> <a id="27064" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="27104" class="Keyword">open</a> <a id="27109" class="Keyword">import</a> <a id="27116" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="27138" class="Keyword">open</a> <a id="27143" class="Keyword">import</a> <a id="27150" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="27185" class="Keyword">open</a> <a id="27190" class="Keyword">import</a> <a id="27197" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="27235" class="Keyword">open</a> <a id="27240" class="Keyword">import</a> <a id="27247" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="27286" class="Keyword">open</a> <a id="27291" class="Keyword">import</a> <a id="27298" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="27333" class="Keyword">open</a> <a id="27338" class="Keyword">import</a> <a id="27345" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="27380" class="Keyword">open</a> <a id="27385" class="Keyword">import</a> <a id="27392" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="27430" class="Keyword">open</a> <a id="27435" class="Keyword">import</a> <a id="27442" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="27473" class="Keyword">open</a> <a id="27478" class="Keyword">import</a> <a id="27485" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="27527" class="Keyword">open</a> <a id="27532" class="Keyword">import</a> <a id="27539" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="27584" class="Keyword">open</a> <a id="27589" class="Keyword">import</a> <a id="27596" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="27629" class="Keyword">open</a> <a id="27634" class="Keyword">import</a> <a id="27641" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="27661" class="Keyword">open</a> <a id="27666" class="Keyword">import</a> <a id="27673" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="27696" class="Keyword">open</a> <a id="27701" class="Keyword">import</a> <a id="27708" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="27731" class="Keyword">open</a> <a id="27736" class="Keyword">import</a> <a id="27743" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="27769" class="Keyword">open</a> <a id="27774" class="Keyword">import</a> <a id="27781" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="27807" class="Keyword">open</a> <a id="27812" class="Keyword">import</a> <a id="27819" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="27875" class="Keyword">open</a> <a id="27880" class="Keyword">import</a> <a id="27887" href="polytopes.html" class="Module">polytopes</a>
<a id="27897" class="Keyword">open</a> <a id="27902" class="Keyword">import</a> <a id="27909" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="27967" class="Keyword">open</a> <a id="27972" class="Keyword">import</a> <a id="27979" href="ring-theory.html" class="Module">ring-theory</a>
<a id="27991" class="Keyword">open</a> <a id="27996" class="Keyword">import</a> <a id="28003" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="28040" class="Keyword">open</a> <a id="28045" class="Keyword">import</a> <a id="28052" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="28079" class="Keyword">open</a> <a id="28084" class="Keyword">import</a> <a id="28091" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="28123" class="Keyword">open</a> <a id="28128" class="Keyword">import</a> <a id="28135" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="28181" class="Keyword">open</a> <a id="28186" class="Keyword">import</a> <a id="28193" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="28218" class="Keyword">open</a> <a id="28223" class="Keyword">import</a> <a id="28230" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="28273" class="Keyword">open</a> <a id="28278" class="Keyword">import</a> <a id="28285" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="28323" class="Keyword">open</a> <a id="28328" class="Keyword">import</a> <a id="28335" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="28366" class="Keyword">open</a> <a id="28371" class="Keyword">import</a> <a id="28378" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="28410" class="Keyword">open</a> <a id="28415" class="Keyword">import</a> <a id="28422" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="28448" class="Keyword">open</a> <a id="28453" class="Keyword">import</a> <a id="28460" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="28489" class="Keyword">open</a> <a id="28494" class="Keyword">import</a> <a id="28501" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="28538" class="Keyword">open</a> <a id="28543" class="Keyword">import</a> <a id="28550" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="28579" class="Keyword">open</a> <a id="28584" class="Keyword">import</a> <a id="28591" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="28618" class="Keyword">open</a> <a id="28623" class="Keyword">import</a> <a id="28630" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="28667" class="Keyword">open</a> <a id="28672" class="Keyword">import</a> <a id="28679" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="28706" class="Keyword">open</a> <a id="28711" class="Keyword">import</a> <a id="28718" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="28751" class="Keyword">open</a> <a id="28756" class="Keyword">import</a> <a id="28763" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="28781" class="Keyword">open</a> <a id="28786" class="Keyword">import</a> <a id="28793" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="28847" class="Keyword">open</a> <a id="28852" class="Keyword">import</a> <a id="28859" href="set-theory.html" class="Module">set-theory</a>
<a id="28870" class="Keyword">open</a> <a id="28875" class="Keyword">import</a> <a id="28882" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="28908" class="Keyword">open</a> <a id="28913" class="Keyword">import</a> <a id="28920" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="28982" class="Keyword">open</a> <a id="28987" class="Keyword">import</a> <a id="28994" href="structured-types.html" class="Module">structured-types</a>
<a id="29011" class="Keyword">open</a> <a id="29016" class="Keyword">import</a> <a id="29023" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="29067" class="Keyword">open</a> <a id="29072" class="Keyword">import</a> <a id="29079" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="29143" class="Keyword">open</a> <a id="29148" class="Keyword">import</a> <a id="29155" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="29201" class="Keyword">open</a> <a id="29206" class="Keyword">import</a> <a id="29213" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="29237" class="Keyword">open</a> <a id="29242" class="Keyword">import</a> <a id="29249" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="29318" class="Keyword">open</a> <a id="29323" class="Keyword">import</a> <a id="29330" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="29364" class="Keyword">open</a> <a id="29369" class="Keyword">import</a> <a id="29376" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="29437" class="Keyword">open</a> <a id="29442" class="Keyword">import</a> <a id="29449" href="structured-types.morphisms-wild-unital-magmas.html" class="Module">structured-types.morphisms-wild-unital-magmas</a>
<a id="29495" class="Keyword">open</a> <a id="29500" class="Keyword">import</a> <a id="29507" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="29552" class="Keyword">open</a> <a id="29557" class="Keyword">import</a> <a id="29564" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="29602" class="Keyword">open</a> <a id="29607" class="Keyword">import</a> <a id="29614" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="29657" class="Keyword">open</a> <a id="29662" class="Keyword">import</a> <a id="29669" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="29705" class="Keyword">open</a> <a id="29710" class="Keyword">import</a> <a id="29717" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="29747" class="Keyword">open</a> <a id="29752" class="Keyword">import</a> <a id="29759" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="29790" class="Keyword">open</a> <a id="29795" class="Keyword">import</a> <a id="29802" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="29853" class="Keyword">open</a> <a id="29858" class="Keyword">import</a> <a id="29865" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="29920" class="Keyword">open</a> <a id="29925" class="Keyword">import</a> <a id="29932" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="29961" class="Keyword">open</a> <a id="29966" class="Keyword">import</a> <a id="29973" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="30001" class="Keyword">open</a> <a id="30006" class="Keyword">import</a> <a id="30013" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="30043" class="Keyword">open</a> <a id="30048" class="Keyword">import</a> <a id="30055" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="30089" class="Keyword">open</a> <a id="30094" class="Keyword">import</a> <a id="30101" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
<a id="30134" class="Keyword">open</a> <a id="30139" class="Keyword">import</a> <a id="30146" href="structured-types.wild-unital-magmas.html" class="Module">structured-types.wild-unital-magmas</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="30225" class="Keyword">open</a> <a id="30230" class="Keyword">import</a> <a id="30237" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="30263" class="Keyword">open</a> <a id="30268" class="Keyword">import</a> <a id="30275" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="30314" class="Keyword">open</a> <a id="30319" class="Keyword">import</a> <a id="30326" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="30364" class="Keyword">open</a> <a id="30369" class="Keyword">import</a> <a id="30376" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="30422" class="Keyword">open</a> <a id="30427" class="Keyword">import</a> <a id="30434" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="30471" class="Keyword">open</a> <a id="30476" class="Keyword">import</a> <a id="30483" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="30523" class="Keyword">open</a> <a id="30528" class="Keyword">import</a> <a id="30535" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="30574" class="Keyword">open</a> <a id="30579" class="Keyword">import</a> <a id="30586" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="30619" class="Keyword">open</a> <a id="30624" class="Keyword">import</a> <a id="30631" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="30666" class="Keyword">open</a> <a id="30671" class="Keyword">import</a> <a id="30678" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="30717" class="Keyword">open</a> <a id="30722" class="Keyword">import</a> <a id="30729" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="30774" class="Keyword">open</a> <a id="30779" class="Keyword">import</a> <a id="30786" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="30838" class="Keyword">open</a> <a id="30843" class="Keyword">import</a> <a id="30850" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="30903" class="Keyword">open</a> <a id="30908" class="Keyword">import</a> <a id="30915" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="30963" class="Keyword">open</a> <a id="30968" class="Keyword">import</a> <a id="30975" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="31015" class="Keyword">open</a> <a id="31020" class="Keyword">import</a> <a id="31027" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="31074" class="Keyword">open</a> <a id="31079" class="Keyword">import</a> <a id="31086" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="31127" class="Keyword">open</a> <a id="31132" class="Keyword">import</a> <a id="31139" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="31177" class="Keyword">open</a> <a id="31182" class="Keyword">import</a> <a id="31189" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="31234" class="Keyword">open</a> <a id="31239" class="Keyword">import</a> <a id="31246" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="31295" class="Keyword">open</a> <a id="31300" class="Keyword">import</a> <a id="31307" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="31384" class="Keyword">open</a> <a id="31389" class="Keyword">import</a> <a id="31396" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="31448" class="Keyword">open</a> <a id="31453" class="Keyword">import</a> <a id="31460" href="type-theories.html" class="Module">type-theories</a>
<a id="31474" class="Keyword">open</a> <a id="31479" class="Keyword">import</a> <a id="31486" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="31528" class="Keyword">open</a> <a id="31533" class="Keyword">import</a> <a id="31540" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="31578" class="Keyword">open</a> <a id="31583" class="Keyword">import</a> <a id="31590" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="31636" class="Keyword">open</a> <a id="31641" class="Keyword">import</a> <a id="31648" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="31695" class="Keyword">open</a> <a id="31700" class="Keyword">import</a> <a id="31707" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="31742" class="Keyword">open</a> <a id="31747" class="Keyword">import</a> <a id="31754" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="31832" class="Keyword">open</a> <a id="31837" class="Keyword">import</a> <a id="31844" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="31868" class="Keyword">open</a> <a id="31873" class="Keyword">import</a> <a id="31880" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="31933" class="Keyword">open</a> <a id="31938" class="Keyword">import</a> <a id="31945" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="31988" class="Keyword">open</a> <a id="31993" class="Keyword">import</a> <a id="32000" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="32040" class="Keyword">open</a> <a id="32045" class="Keyword">import</a> <a id="32052" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="32091" class="Keyword">open</a> <a id="32096" class="Keyword">import</a> <a id="32103" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="32151" class="Keyword">open</a> <a id="32156" class="Keyword">import</a> <a id="32163" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="32210" class="Keyword">open</a> <a id="32215" class="Keyword">import</a> <a id="32222" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="32274" class="Keyword">open</a> <a id="32279" class="Keyword">import</a> <a id="32286" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="32330" class="Keyword">open</a> <a id="32335" class="Keyword">import</a> <a id="32342" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="32382" class="Keyword">open</a> <a id="32387" class="Keyword">import</a> <a id="32394" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="32446" class="Keyword">open</a> <a id="32451" class="Keyword">import</a> <a id="32458" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="32512" class="Keyword">open</a> <a id="32517" class="Keyword">import</a> <a id="32524" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="32572" class="Keyword">open</a> <a id="32577" class="Keyword">import</a> <a id="32584" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="32623" class="Keyword">open</a> <a id="32628" class="Keyword">import</a> <a id="32635" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="32668" class="Keyword">open</a> <a id="32673" class="Keyword">import</a> <a id="32680" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="32710" class="Keyword">open</a> <a id="32715" class="Keyword">import</a> <a id="32722" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="32781" class="Keyword">open</a> <a id="32786" class="Keyword">import</a> <a id="32793" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="32848" class="Keyword">open</a> <a id="32853" class="Keyword">import</a> <a id="32860" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="32907" class="Keyword">open</a> <a id="32912" class="Keyword">import</a> <a id="32919" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="32962" class="Keyword">open</a> <a id="32967" class="Keyword">import</a> <a id="32974" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="33019" class="Keyword">open</a> <a id="33024" class="Keyword">import</a> <a id="33031" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="33080" class="Keyword">open</a> <a id="33085" class="Keyword">import</a> <a id="33092" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="33143" class="Keyword">open</a> <a id="33148" class="Keyword">import</a> <a id="33155" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="33233" class="Keyword">open</a> <a id="33238" class="Keyword">import</a> <a id="33245" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="33285" class="Keyword">open</a> <a id="33290" class="Keyword">import</a> <a id="33297" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="33354" class="Keyword">open</a> <a id="33359" class="Keyword">import</a> <a id="33366" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="33401" class="Keyword">open</a> <a id="33406" class="Keyword">import</a> <a id="33413" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="33459" class="Keyword">open</a> <a id="33464" class="Keyword">import</a> <a id="33471" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="33526" class="Keyword">open</a> <a id="33531" class="Keyword">import</a> <a id="33538" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="33581" class="Keyword">open</a> <a id="33586" class="Keyword">import</a> <a id="33593" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="33652" class="Keyword">open</a> <a id="33657" class="Keyword">import</a> <a id="33664" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="33701" class="Keyword">open</a> <a id="33706" class="Keyword">import</a> <a id="33713" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="33754" class="Keyword">open</a> <a id="33759" class="Keyword">import</a> <a id="33766" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="33805" class="Keyword">open</a> <a id="33810" class="Keyword">import</a> <a id="33817" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="33855" class="Keyword">open</a> <a id="33860" class="Keyword">import</a> <a id="33867" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="33919" class="Keyword">open</a> <a id="33924" class="Keyword">import</a> <a id="33931" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="33976" class="Keyword">open</a> <a id="33981" class="Keyword">import</a> <a id="33988" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="34025" class="Keyword">open</a> <a id="34030" class="Keyword">import</a> <a id="34037" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="34086" class="Keyword">open</a> <a id="34091" class="Keyword">import</a> <a id="34098" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="34137" class="Keyword">open</a> <a id="34142" class="Keyword">import</a> <a id="34149" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="34187" class="Keyword">open</a> <a id="34192" class="Keyword">import</a> <a id="34199" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="34254" class="Keyword">open</a> <a id="34259" class="Keyword">import</a> <a id="34266" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="34305" class="Keyword">open</a> <a id="34310" class="Keyword">import</a> <a id="34317" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="34365" class="Keyword">open</a> <a id="34370" class="Keyword">import</a> <a id="34377" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="34424" class="Keyword">open</a> <a id="34429" class="Keyword">import</a> <a id="34436" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="34474" class="Keyword">open</a> <a id="34479" class="Keyword">import</a> <a id="34486" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="34516" class="Keyword">open</a> <a id="34521" class="Keyword">import</a> <a id="34528" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="34585" class="Keyword">open</a> <a id="34590" class="Keyword">import</a> <a id="34597" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="34651" class="Keyword">open</a> <a id="34656" class="Keyword">import</a> <a id="34663" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="34693" class="Keyword">open</a> <a id="34698" class="Keyword">import</a> <a id="34705" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="34768" class="Keyword">open</a> <a id="34773" class="Keyword">import</a> <a id="34780" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="34823" class="Keyword">open</a> <a id="34828" class="Keyword">import</a> <a id="34835" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="34870" class="Keyword">open</a> <a id="34875" class="Keyword">import</a> <a id="34882" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="34922" class="Keyword">open</a> <a id="34927" class="Keyword">import</a> <a id="34934" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="34979" class="Keyword">open</a> <a id="34984" class="Keyword">import</a> <a id="34991" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="35041" class="Keyword">open</a> <a id="35046" class="Keyword">import</a> <a id="35053" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="35091" class="Keyword">open</a> <a id="35096" class="Keyword">import</a> <a id="35103" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="35152" class="Keyword">open</a> <a id="35157" class="Keyword">import</a> <a id="35164" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="35211" class="Keyword">open</a> <a id="35216" class="Keyword">import</a> <a id="35223" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="35286" class="Keyword">open</a> <a id="35291" class="Keyword">import</a> <a id="35298" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="35330" class="Keyword">open</a> <a id="35335" class="Keyword">import</a> <a id="35342" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="35395" class="Keyword">open</a> <a id="35400" class="Keyword">import</a> <a id="35407" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="35453" class="Keyword">open</a> <a id="35458" class="Keyword">import</a> <a id="35465" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="35511" class="Keyword">open</a> <a id="35516" class="Keyword">import</a> <a id="35523" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="35571" class="Keyword">open</a> <a id="35576" class="Keyword">import</a> <a id="35583" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="35623" class="Keyword">open</a> <a id="35628" class="Keyword">import</a> <a id="35635" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="35680" class="Keyword">open</a> <a id="35685" class="Keyword">import</a> <a id="35692" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>