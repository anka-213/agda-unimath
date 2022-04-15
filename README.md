# Univalent mathematics in Agda

Welcome to the website of the `agda-unimath` formalization project.

[![CI](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml/badge.svg)](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml) [![pages-build-deployment](https://github.com/UniMath/agda-unimath/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/UniMath/agda-unimath/actions/workflows/pages/pages-build-deployment)[![build](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml)

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

<pre class="Agda"><a id="3135" class="Symbol">{-#</a> <a id="3139" class="Keyword">OPTIONS</a> <a id="3147" class="Pragma">--without-K</a> <a id="3159" class="Pragma">--exact-split</a> <a id="3173" class="Pragma">--guardedness</a> <a id="3187" class="Symbol">#-}</a>
</pre>
## Category theory

<pre class="Agda"><a id="3224" class="Keyword">open</a> <a id="3229" class="Keyword">import</a> <a id="3236" href="category-theory.html" class="Module">category-theory</a>
<a id="3252" class="Keyword">open</a> <a id="3257" class="Keyword">import</a> <a id="3264" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="3312" class="Keyword">open</a> <a id="3317" class="Keyword">import</a> <a id="3324" href="category-theory.anafunctors.html" class="Module">category-theory.anafunctors</a>
<a id="3352" class="Keyword">open</a> <a id="3357" class="Keyword">import</a> <a id="3364" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="3391" class="Keyword">open</a> <a id="3396" class="Keyword">import</a> <a id="3403" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="3443" class="Keyword">open</a> <a id="3448" class="Keyword">import</a> <a id="3455" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="3504" class="Keyword">open</a> <a id="3509" class="Keyword">import</a> <a id="3516" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="3559" class="Keyword">open</a> <a id="3564" class="Keyword">import</a> <a id="3571" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="3607" class="Keyword">open</a> <a id="3612" class="Keyword">import</a> <a id="3619" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="3664" class="Keyword">open</a> <a id="3669" class="Keyword">import</a> <a id="3676" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="3715" class="Keyword">open</a> <a id="3720" class="Keyword">import</a> <a id="3727" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="3798" class="Keyword">open</a> <a id="3803" class="Keyword">import</a> <a id="3810" href="category-theory.initial-objects-precategories.html" class="Module">category-theory.initial-objects-precategories</a>
<a id="3856" class="Keyword">open</a> <a id="3861" class="Keyword">import</a> <a id="3868" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="3908" class="Keyword">open</a> <a id="3913" class="Keyword">import</a> <a id="3920" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="3969" class="Keyword">open</a> <a id="3974" class="Keyword">import</a> <a id="3981" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="4024" class="Keyword">open</a> <a id="4029" class="Keyword">import</a> <a id="4036" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="4069" class="Keyword">open</a> <a id="4074" class="Keyword">import</a> <a id="4081" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="4117" class="Keyword">open</a> <a id="4122" class="Keyword">import</a> <a id="4129" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="4179" class="Keyword">open</a> <a id="4184" class="Keyword">import</a> <a id="4191" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="4239" class="Keyword">open</a> <a id="4244" class="Keyword">import</a> <a id="4251" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="4308" class="Keyword">open</a> <a id="4313" class="Keyword">import</a> <a id="4320" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="4371" class="Keyword">open</a> <a id="4376" class="Keyword">import</a> <a id="4383" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="4434" class="Keyword">open</a> <a id="4439" class="Keyword">import</a> <a id="4446" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="4506" class="Keyword">open</a> <a id="4511" class="Keyword">import</a> <a id="4518" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="4572" class="Keyword">open</a> <a id="4577" class="Keyword">import</a> <a id="4584" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
<a id="4614" class="Keyword">open</a> <a id="4619" class="Keyword">import</a> <a id="4626" href="category-theory.slice-precategories.html" class="Module">category-theory.slice-precategories</a>
<a id="4662" class="Keyword">open</a> <a id="4667" class="Keyword">import</a> <a id="4674" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="4763" class="Keyword">open</a> <a id="4768" class="Keyword">import</a> <a id="4775" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="4800" class="Keyword">open</a> <a id="4805" class="Keyword">import</a> <a id="4812" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="4861" class="Keyword">open</a> <a id="4866" class="Keyword">import</a> <a id="4873" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="4916" class="Keyword">open</a> <a id="4921" class="Keyword">import</a> <a id="4928" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="4978" class="Keyword">open</a> <a id="4983" class="Keyword">import</a> <a id="4990" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5036" class="Keyword">open</a> <a id="5041" class="Keyword">import</a> <a id="5048" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5095" class="Keyword">open</a> <a id="5100" class="Keyword">import</a> <a id="5107" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5166" class="Keyword">open</a> <a id="5171" class="Keyword">import</a> <a id="5178" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="5219" class="Keyword">open</a> <a id="5224" class="Keyword">import</a> <a id="5231" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="5274" class="Keyword">open</a> <a id="5279" class="Keyword">import</a> <a id="5286" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="5330" class="Keyword">open</a> <a id="5335" class="Keyword">import</a> <a id="5342" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="5387" class="Keyword">open</a> <a id="5392" class="Keyword">import</a> <a id="5399" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="5451" class="Keyword">open</a> <a id="5456" class="Keyword">import</a> <a id="5463" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="5523" class="Keyword">open</a> <a id="5528" class="Keyword">import</a> <a id="5535" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="5576" class="Keyword">open</a> <a id="5581" class="Keyword">import</a> <a id="5588" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="5633" class="Keyword">open</a> <a id="5638" class="Keyword">import</a> <a id="5645" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="5692" class="Keyword">open</a> <a id="5697" class="Keyword">import</a> <a id="5704" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="5747" class="Keyword">open</a> <a id="5752" class="Keyword">import</a> <a id="5759" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="5809" class="Keyword">open</a> <a id="5814" class="Keyword">import</a> <a id="5821" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="5868" class="Keyword">open</a> <a id="5873" class="Keyword">import</a> <a id="5880" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="5937" class="Keyword">open</a> <a id="5942" class="Keyword">import</a> <a id="5949" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6003" class="Keyword">open</a> <a id="6008" class="Keyword">import</a> <a id="6015" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6075" class="Keyword">open</a> <a id="6080" class="Keyword">import</a> <a id="6087" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6130" class="Keyword">open</a> <a id="6135" class="Keyword">import</a> <a id="6142" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="6192" class="Keyword">open</a> <a id="6197" class="Keyword">import</a> <a id="6204" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="6264" class="Keyword">open</a> <a id="6269" class="Keyword">import</a> <a id="6276" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="6325" class="Keyword">open</a> <a id="6330" class="Keyword">import</a> <a id="6337" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="6393" class="Keyword">open</a> <a id="6398" class="Keyword">import</a> <a id="6405" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="6441" class="Keyword">open</a> <a id="6446" class="Keyword">import</a> <a id="6453" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="6497" class="Keyword">open</a> <a id="6502" class="Keyword">import</a> <a id="6509" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="6553" class="Keyword">open</a> <a id="6558" class="Keyword">import</a> <a id="6565" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="6615" class="Keyword">open</a> <a id="6620" class="Keyword">import</a> <a id="6627" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="6673" class="Keyword">open</a> <a id="6678" class="Keyword">import</a> <a id="6685" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="6720" class="Keyword">open</a> <a id="6725" class="Keyword">import</a> <a id="6732" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="6777" class="Keyword">open</a> <a id="6782" class="Keyword">import</a> <a id="6789" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="6847" class="Keyword">open</a> <a id="6852" class="Keyword">import</a> <a id="6859" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="6924" class="Keyword">open</a> <a id="6929" class="Keyword">import</a> <a id="6936" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="6979" class="Keyword">open</a> <a id="6984" class="Keyword">import</a> <a id="6991" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7045" class="Keyword">open</a> <a id="7050" class="Keyword">import</a> <a id="7057" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7102" class="Keyword">open</a> <a id="7107" class="Keyword">import</a> <a id="7114" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7166" class="Keyword">open</a> <a id="7171" class="Keyword">import</a> <a id="7178" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7236" class="Keyword">open</a> <a id="7241" class="Keyword">import</a> <a id="7248" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="7294" class="Keyword">open</a> <a id="7299" class="Keyword">import</a> <a id="7306" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="7340" class="Keyword">open</a> <a id="7345" class="Keyword">import</a> <a id="7352" href="elementary-number-theory.iterating-functions.html" class="Module">elementary-number-theory.iterating-functions</a>
<a id="7397" class="Keyword">open</a> <a id="7402" class="Keyword">import</a> <a id="7409" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="7463" class="Keyword">open</a> <a id="7468" class="Keyword">import</a> <a id="7475" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="7524" class="Keyword">open</a> <a id="7529" class="Keyword">import</a> <a id="7536" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="7577" class="Keyword">open</a> <a id="7582" class="Keyword">import</a> <a id="7589" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="7638" class="Keyword">open</a> <a id="7643" class="Keyword">import</a> <a id="7650" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="7716" class="Keyword">open</a> <a id="7721" class="Keyword">import</a> <a id="7728" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="7772" class="Keyword">open</a> <a id="7777" class="Keyword">import</a> <a id="7784" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="7833" class="Keyword">open</a> <a id="7838" class="Keyword">import</a> <a id="7845" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="7901" class="Keyword">open</a> <a id="7906" class="Keyword">import</a> <a id="7913" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="7954" class="Keyword">open</a> <a id="7959" class="Keyword">import</a> <a id="7966" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8015" class="Keyword">open</a> <a id="8020" class="Keyword">import</a> <a id="8027" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8086" class="Keyword">open</a> <a id="8091" class="Keyword">import</a> <a id="8098" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8137" class="Keyword">open</a> <a id="8142" class="Keyword">import</a> <a id="8149" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8202" class="Keyword">open</a> <a id="8207" class="Keyword">import</a> <a id="8214" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="8271" class="Keyword">open</a> <a id="8276" class="Keyword">import</a> <a id="8283" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="8325" class="Keyword">open</a> <a id="8330" class="Keyword">import</a> <a id="8337" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="8388" class="Keyword">open</a> <a id="8393" class="Keyword">import</a> <a id="8400" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="8458" class="Keyword">open</a> <a id="8463" class="Keyword">import</a> <a id="8470" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="8534" class="Keyword">open</a> <a id="8539" class="Keyword">import</a> <a id="8546" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="8599" class="Keyword">open</a> <a id="8604" class="Keyword">import</a> <a id="8611" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="8664" class="Keyword">open</a> <a id="8669" class="Keyword">import</a> <a id="8676" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="8737" class="Keyword">open</a> <a id="8742" class="Keyword">import</a> <a id="8749" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="8807" class="Keyword">open</a> <a id="8812" class="Keyword">import</a> <a id="8819" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="8868" class="Keyword">open</a> <a id="8873" class="Keyword">import</a> <a id="8880" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="8924" class="Keyword">open</a> <a id="8929" class="Keyword">import</a> <a id="8936" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="8979" class="Keyword">open</a> <a id="8984" class="Keyword">import</a> <a id="8991" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9038" class="Keyword">open</a> <a id="9043" class="Keyword">import</a> <a id="9050" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9111" class="Keyword">open</a> <a id="9116" class="Keyword">import</a> <a id="9123" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9186" class="Keyword">open</a> <a id="9191" class="Keyword">import</a> <a id="9198" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="9258" class="Keyword">open</a> <a id="9263" class="Keyword">import</a> <a id="9270" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="9324" class="Keyword">open</a> <a id="9329" class="Keyword">import</a> <a id="9336" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="9401" class="Keyword">open</a> <a id="9406" class="Keyword">import</a> <a id="9413" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="9521" class="Keyword">open</a> <a id="9526" class="Keyword">import</a> <a id="9533" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="9553" class="Keyword">open</a> <a id="9558" class="Keyword">import</a> <a id="9565" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="9611" class="Keyword">open</a> <a id="9616" class="Keyword">import</a> <a id="9623" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="9669" class="Keyword">open</a> <a id="9674" class="Keyword">import</a> <a id="9681" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="9715" class="Keyword">open</a> <a id="9720" class="Keyword">import</a> <a id="9727" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="9762" class="Keyword">open</a> <a id="9767" class="Keyword">import</a> <a id="9774" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="9812" class="Keyword">open</a> <a id="9817" class="Keyword">import</a> <a id="9824" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="9862" class="Keyword">open</a> <a id="9867" class="Keyword">import</a> <a id="9874" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="9914" class="Keyword">open</a> <a id="9919" class="Keyword">import</a> <a id="9926" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="9959" class="Keyword">open</a> <a id="9964" class="Keyword">import</a> <a id="9971" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10009" class="Keyword">open</a> <a id="10014" class="Keyword">import</a> <a id="10021" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10084" class="Keyword">open</a> <a id="10089" class="Keyword">import</a> <a id="10096" href="foundation.html" class="Module">foundation</a>
<a id="10107" class="Keyword">open</a> <a id="10112" class="Keyword">import</a> <a id="10119" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10137" class="Keyword">open</a> <a id="10142" class="Keyword">import</a> <a id="10149" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10168" class="Keyword">open</a> <a id="10173" class="Keyword">import</a> <a id="10180" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10199" class="Keyword">open</a> <a id="10204" class="Keyword">import</a> <a id="10211" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="10255" class="Keyword">open</a> <a id="10260" class="Keyword">import</a> <a id="10267" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="10292" class="Keyword">open</a> <a id="10297" class="Keyword">import</a> <a id="10304" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="10331" class="Keyword">open</a> <a id="10336" class="Keyword">import</a> <a id="10343" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="10372" class="Keyword">open</a> <a id="10377" class="Keyword">import</a> <a id="10384" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="10415" class="Keyword">open</a> <a id="10420" class="Keyword">import</a> <a id="10427" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="10455" class="Keyword">open</a> <a id="10460" class="Keyword">import</a> <a id="10467" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="10497" class="Keyword">open</a> <a id="10502" class="Keyword">import</a> <a id="10509" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="10529" class="Keyword">open</a> <a id="10534" class="Keyword">import</a> <a id="10541" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="10578" class="Keyword">open</a> <a id="10583" class="Keyword">import</a> <a id="10590" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="10625" class="Keyword">open</a> <a id="10630" class="Keyword">import</a> <a id="10637" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="10695" class="Keyword">open</a> <a id="10700" class="Keyword">import</a> <a id="10707" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="10745" class="Keyword">open</a> <a id="10750" class="Keyword">import</a> <a id="10757" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="10786" class="Keyword">open</a> <a id="10791" class="Keyword">import</a> <a id="10798" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="10821" class="Keyword">open</a> <a id="10826" class="Keyword">import</a> <a id="10833" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="10856" class="Keyword">open</a> <a id="10861" class="Keyword">import</a> <a id="10868" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="10910" class="Keyword">open</a> <a id="10915" class="Keyword">import</a> <a id="10922" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="10954" class="Keyword">open</a> <a id="10959" class="Keyword">import</a> <a id="10966" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="10993" class="Keyword">open</a> <a id="10998" class="Keyword">import</a> <a id="11005" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="11030" class="Keyword">open</a> <a id="11035" class="Keyword">import</a> <a id="11042" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="11071" class="Keyword">open</a> <a id="11076" class="Keyword">import</a> <a id="11083" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="11113" class="Keyword">open</a> <a id="11118" class="Keyword">import</a> <a id="11125" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="11152" class="Keyword">open</a> <a id="11157" class="Keyword">import</a> <a id="11164" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="11183" class="Keyword">open</a> <a id="11188" class="Keyword">import</a> <a id="11195" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="11241" class="Keyword">open</a> <a id="11246" class="Keyword">import</a> <a id="11253" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="11295" class="Keyword">open</a> <a id="11300" class="Keyword">import</a> <a id="11307" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="11339" class="Keyword">open</a> <a id="11344" class="Keyword">import</a> <a id="11351" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="11381" class="Keyword">open</a> <a id="11386" class="Keyword">import</a> <a id="11393" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="11419" class="Keyword">open</a> <a id="11424" class="Keyword">import</a> <a id="11431" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="11465" class="Keyword">open</a> <a id="11470" class="Keyword">import</a> <a id="11477" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="11507" class="Keyword">open</a> <a id="11512" class="Keyword">import</a> <a id="11519" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="11546" class="Keyword">open</a> <a id="11551" class="Keyword">import</a> <a id="11558" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="11590" class="Keyword">open</a> <a id="11595" class="Keyword">import</a> <a id="11602" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="11636" class="Keyword">open</a> <a id="11641" class="Keyword">import</a> <a id="11648" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="11671" class="Keyword">open</a> <a id="11676" class="Keyword">import</a> <a id="11683" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="11753" class="Keyword">open</a> <a id="11758" class="Keyword">import</a> <a id="11765" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="11835" class="Keyword">open</a> <a id="11840" class="Keyword">import</a> <a id="11847" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="11874" class="Keyword">open</a> <a id="11879" class="Keyword">import</a> <a id="11886" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="11923" class="Keyword">open</a> <a id="11928" class="Keyword">import</a> <a id="11935" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="11983" class="Keyword">open</a> <a id="11988" class="Keyword">import</a> <a id="11995" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="12035" class="Keyword">open</a> <a id="12040" class="Keyword">import</a> <a id="12047" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="12069" class="Keyword">open</a> <a id="12074" class="Keyword">import</a> <a id="12081" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="12104" class="Keyword">open</a> <a id="12109" class="Keyword">import</a> <a id="12116" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="12161" class="Keyword">open</a> <a id="12166" class="Keyword">import</a> <a id="12173" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="12217" class="Keyword">open</a> <a id="12222" class="Keyword">import</a> <a id="12229" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="12265" class="Keyword">open</a> <a id="12270" class="Keyword">import</a> <a id="12277" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="12322" class="Keyword">open</a> <a id="12327" class="Keyword">import</a> <a id="12334" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="12375" class="Keyword">open</a> <a id="12380" class="Keyword">import</a> <a id="12387" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="12422" class="Keyword">open</a> <a id="12427" class="Keyword">import</a> <a id="12434" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="12465" class="Keyword">open</a> <a id="12470" class="Keyword">import</a> <a id="12477" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="12510" class="Keyword">open</a> <a id="12515" class="Keyword">import</a> <a id="12522" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="12555" class="Keyword">open</a> <a id="12560" class="Keyword">import</a> <a id="12567" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="12597" class="Keyword">open</a> <a id="12602" class="Keyword">import</a> <a id="12609" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="12633" class="Keyword">open</a> <a id="12638" class="Keyword">import</a> <a id="12645" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="12683" class="Keyword">open</a> <a id="12688" class="Keyword">import</a> <a id="12695" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="12726" class="Keyword">open</a> <a id="12731" class="Keyword">import</a> <a id="12738" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="12763" class="Keyword">open</a> <a id="12768" class="Keyword">import</a> <a id="12775" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="12803" class="Keyword">open</a> <a id="12808" class="Keyword">import</a> <a id="12815" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="12839" class="Keyword">open</a> <a id="12844" class="Keyword">import</a> <a id="12851" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="12877" class="Keyword">open</a> <a id="12882" class="Keyword">import</a> <a id="12889" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="12924" class="Keyword">open</a> <a id="12929" class="Keyword">import</a> <a id="12936" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="12957" class="Keyword">open</a> <a id="12962" class="Keyword">import</a> <a id="12969" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="13018" class="Keyword">open</a> <a id="13023" class="Keyword">import</a> <a id="13030" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="13071" class="Keyword">open</a> <a id="13076" class="Keyword">import</a> <a id="13083" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="13133" class="Keyword">open</a> <a id="13138" class="Keyword">import</a> <a id="13145" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="13191" class="Keyword">open</a> <a id="13196" class="Keyword">import</a> <a id="13203" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="13243" class="Keyword">open</a> <a id="13248" class="Keyword">import</a> <a id="13255" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="13305" class="Keyword">open</a> <a id="13310" class="Keyword">import</a> <a id="13317" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="13356" class="Keyword">open</a> <a id="13361" class="Keyword">import</a> <a id="13368" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="13408" class="Keyword">open</a> <a id="13413" class="Keyword">import</a> <a id="13420" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="13453" class="Keyword">open</a> <a id="13458" class="Keyword">import</a> <a id="13465" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="13514" class="Keyword">open</a> <a id="13519" class="Keyword">import</a> <a id="13526" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="13551" class="Keyword">open</a> <a id="13556" class="Keyword">import</a> <a id="13563" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="13601" class="Keyword">open</a> <a id="13606" class="Keyword">import</a> <a id="13613" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="13635" class="Keyword">open</a> <a id="13640" class="Keyword">import</a> <a id="13647" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="13675" class="Keyword">open</a> <a id="13680" class="Keyword">import</a> <a id="13687" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="13713" class="Keyword">open</a> <a id="13718" class="Keyword">import</a> <a id="13725" href="foundation.images.html" class="Module">foundation.images</a>
<a id="13743" class="Keyword">open</a> <a id="13748" class="Keyword">import</a> <a id="13755" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="13790" class="Keyword">open</a> <a id="13795" class="Keyword">import</a> <a id="13802" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="13829" class="Keyword">open</a> <a id="13834" class="Keyword">import</a> <a id="13841" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="13897" class="Keyword">open</a> <a id="13902" class="Keyword">import</a> <a id="13909" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="13938" class="Keyword">open</a> <a id="13943" class="Keyword">import</a> <a id="13950" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="13980" class="Keyword">open</a> <a id="13985" class="Keyword">import</a> <a id="13992" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="14018" class="Keyword">open</a> <a id="14023" class="Keyword">import</a> <a id="14030" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="14057" class="Keyword">open</a> <a id="14062" class="Keyword">import</a> <a id="14069" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="14092" class="Keyword">open</a> <a id="14097" class="Keyword">import</a> <a id="14104" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="14131" class="Keyword">open</a> <a id="14136" class="Keyword">import</a> <a id="14143" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="14175" class="Keyword">open</a> <a id="14180" class="Keyword">import</a> <a id="14187" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="14221" class="Keyword">open</a> <a id="14226" class="Keyword">import</a> <a id="14233" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="14273" class="Keyword">open</a> <a id="14278" class="Keyword">import</a> <a id="14285" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="14316" class="Keyword">open</a> <a id="14321" class="Keyword">import</a> <a id="14328" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="14360" class="Keyword">open</a> <a id="14365" class="Keyword">import</a> <a id="14372" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="14403" class="Keyword">open</a> <a id="14408" class="Keyword">import</a> <a id="14415" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="14432" class="Keyword">open</a> <a id="14437" class="Keyword">import</a> <a id="14444" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="14469" class="Keyword">open</a> <a id="14474" class="Keyword">import</a> <a id="14481" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="14510" class="Keyword">open</a> <a id="14515" class="Keyword">import</a> <a id="14522" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="14547" class="Keyword">open</a> <a id="14552" class="Keyword">import</a> <a id="14559" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="14580" class="Keyword">open</a> <a id="14585" class="Keyword">import</a> <a id="14592" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="14612" class="Keyword">open</a> <a id="14617" class="Keyword">import</a> <a id="14624" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="14658" class="Keyword">open</a> <a id="14663" class="Keyword">import</a> <a id="14670" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="14708" class="Keyword">open</a> <a id="14713" class="Keyword">import</a> <a id="14720" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="14744" class="Keyword">open</a> <a id="14749" class="Keyword">import</a> <a id="14756" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="14783" class="Keyword">open</a> <a id="14788" class="Keyword">import</a> <a id="14795" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="14830" class="Keyword">open</a> <a id="14835" class="Keyword">import</a> <a id="14842" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="14878" class="Keyword">open</a> <a id="14883" class="Keyword">import</a> <a id="14890" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="14930" class="Keyword">open</a> <a id="14935" class="Keyword">import</a> <a id="14942" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="14972" class="Keyword">open</a> <a id="14977" class="Keyword">import</a> <a id="14984" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="15021" class="Keyword">open</a> <a id="15026" class="Keyword">import</a> <a id="15033" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="15057" class="Keyword">open</a> <a id="15062" class="Keyword">import</a> <a id="15069" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="15090" class="Keyword">open</a> <a id="15095" class="Keyword">import</a> <a id="15102" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="15137" class="Keyword">open</a> <a id="15142" class="Keyword">import</a> <a id="15149" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="15186" class="Keyword">open</a> <a id="15191" class="Keyword">import</a> <a id="15198" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="15247" class="Keyword">open</a> <a id="15252" class="Keyword">import</a> <a id="15259" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="15282" class="Keyword">open</a> <a id="15287" class="Keyword">import</a> <a id="15294" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="15317" class="Keyword">open</a> <a id="15322" class="Keyword">import</a> <a id="15329" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="15357" class="Keyword">open</a> <a id="15362" class="Keyword">import</a> <a id="15369" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="15389" class="Keyword">open</a> <a id="15394" class="Keyword">import</a> <a id="15401" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="15432" class="Keyword">open</a> <a id="15437" class="Keyword">import</a> <a id="15444" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="15471" class="Keyword">open</a> <a id="15476" class="Keyword">import</a> <a id="15483" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="15499" class="Keyword">open</a> <a id="15504" class="Keyword">import</a> <a id="15511" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="15542" class="Keyword">open</a> <a id="15547" class="Keyword">import</a> <a id="15554" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="15571" class="Keyword">open</a> <a id="15576" class="Keyword">import</a> <a id="15583" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="15605" class="Keyword">open</a> <a id="15610" class="Keyword">import</a> <a id="15617" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="15644" class="Keyword">open</a> <a id="15649" class="Keyword">import</a> <a id="15656" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="15679" class="Keyword">open</a> <a id="15684" class="Keyword">import</a> <a id="15691" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="15718" class="Keyword">open</a> <a id="15723" class="Keyword">import</a> <a id="15730" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="15763" class="Keyword">open</a> <a id="15768" class="Keyword">import</a> <a id="15775" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="15815" class="Keyword">open</a> <a id="15820" class="Keyword">import</a> <a id="15827" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="15848" class="Keyword">open</a> <a id="15853" class="Keyword">import</a> <a id="15860" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="15889" class="Keyword">open</a> <a id="15894" class="Keyword">import</a> <a id="15901" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="15939" class="Keyword">open</a> <a id="15944" class="Keyword">import</a> <a id="15951" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="15971" class="Keyword">open</a> <a id="15976" class="Keyword">import</a> <a id="15983" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="16007" class="Keyword">open</a> <a id="16012" class="Keyword">import</a> <a id="16019" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="16046" class="Keyword">open</a> <a id="16051" class="Keyword">import</a> <a id="16058" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="16088" class="Keyword">open</a> <a id="16093" class="Keyword">import</a> <a id="16100" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="16126" class="Keyword">open</a> <a id="16131" class="Keyword">import</a> <a id="16138" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="16165" class="Keyword">open</a> <a id="16170" class="Keyword">import</a> <a id="16177" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="16206" class="Keyword">open</a> <a id="16211" class="Keyword">import</a> <a id="16218" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="16241" class="Keyword">open</a> <a id="16246" class="Keyword">import</a> <a id="16253" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="16304" class="Keyword">open</a> <a id="16309" class="Keyword">import</a> <a id="16316" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="16359" class="Keyword">open</a> <a id="16364" class="Keyword">import</a> <a id="16371" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="16419" class="Keyword">open</a> <a id="16424" class="Keyword">import</a> <a id="16431" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="16469" class="Keyword">open</a> <a id="16474" class="Keyword">import</a> <a id="16481" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="16518" class="Keyword">open</a> <a id="16523" class="Keyword">import</a> <a id="16530" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="16558" class="Keyword">open</a> <a id="16563" class="Keyword">import</a> <a id="16570" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="16606" class="Keyword">open</a> <a id="16611" class="Keyword">import</a> <a id="16618" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="16656" class="Keyword">open</a> <a id="16661" class="Keyword">import</a> <a id="16668" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="16701" class="Keyword">open</a> <a id="16706" class="Keyword">import</a> <a id="16713" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="16734" class="Keyword">open</a> <a id="16739" class="Keyword">import</a> <a id="16746" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="16800" class="Keyword">open</a> <a id="16805" class="Keyword">import</a> <a id="16812" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="16834" class="Keyword">open</a> <a id="16839" class="Keyword">import</a> <a id="16846" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="16881" class="Keyword">open</a> <a id="16886" class="Keyword">import</a> <a id="16893" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="16923" class="Keyword">open</a> <a id="16928" class="Keyword">import</a> <a id="16935" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="16974" class="Keyword">open</a> <a id="16979" class="Keyword">import</a> <a id="16986" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="17040" class="Keyword">open</a> <a id="17045" class="Keyword">import</a> <a id="17052" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="17098" class="Keyword">open</a> <a id="17103" class="Keyword">import</a> <a id="17110" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="17161" class="Keyword">open</a> <a id="17166" class="Keyword">import</a> <a id="17173" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="17214" class="Keyword">open</a> <a id="17219" class="Keyword">import</a> <a id="17226" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="17271" class="Keyword">open</a> <a id="17276" class="Keyword">import</a> <a id="17283" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="17328" class="Keyword">open</a> <a id="17333" class="Keyword">import</a> <a id="17340" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="17376" class="Keyword">open</a> <a id="17381" class="Keyword">import</a> <a id="17388" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="17424" class="Keyword">open</a> <a id="17429" class="Keyword">import</a> <a id="17436" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="17501" class="Keyword">open</a> <a id="17506" class="Keyword">import</a> <a id="17513" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="17568" class="Keyword">open</a> <a id="17573" class="Keyword">import</a> <a id="17580" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="17620" class="Keyword">open</a> <a id="17625" class="Keyword">import</a> <a id="17632" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="17676" class="Keyword">open</a> <a id="17681" class="Keyword">import</a> <a id="17688" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="17733" class="Keyword">open</a> <a id="17738" class="Keyword">import</a> <a id="17745" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="17786" class="Keyword">open</a> <a id="17791" class="Keyword">import</a> <a id="17798" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="17838" class="Keyword">open</a> <a id="17843" class="Keyword">import</a> <a id="17850" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="17877" class="Keyword">open</a> <a id="17882" class="Keyword">import</a> <a id="17889" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="17916" class="Keyword">open</a> <a id="17921" class="Keyword">import</a> <a id="17928" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="17947" class="Keyword">open</a> <a id="17952" class="Keyword">import</a> <a id="17959" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="17999" class="Keyword">open</a> <a id="18004" class="Keyword">import</a> <a id="18011" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="18076" class="Keyword">open</a> <a id="18081" class="Keyword">import</a> <a id="18088" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="18111" class="Keyword">open</a> <a id="18116" class="Keyword">import</a> <a id="18123" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="18147" class="Keyword">open</a> <a id="18152" class="Keyword">import</a> <a id="18159" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="18199" class="Keyword">open</a> <a id="18204" class="Keyword">import</a> <a id="18211" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="18254" class="Keyword">open</a> <a id="18259" class="Keyword">import</a> <a id="18266" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="18300" class="Keyword">open</a> <a id="18305" class="Keyword">import</a> <a id="18312" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="18342" class="Keyword">open</a> <a id="18347" class="Keyword">import</a> <a id="18354" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="18388" class="Keyword">open</a> <a id="18393" class="Keyword">import</a> <a id="18400" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="18435" class="Keyword">open</a> <a id="18440" class="Keyword">import</a> <a id="18447" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="18484" class="Keyword">open</a> <a id="18489" class="Keyword">import</a> <a id="18496" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="18523" class="Keyword">open</a> <a id="18528" class="Keyword">import</a> <a id="18535" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="18563" class="Keyword">open</a> <a id="18568" class="Keyword">import</a> <a id="18575" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="18624" class="Keyword">open</a> <a id="18629" class="Keyword">import</a> <a id="18636" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="18682" class="Keyword">open</a> <a id="18687" class="Keyword">import</a> <a id="18694" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="18734" class="Keyword">open</a> <a id="18739" class="Keyword">import</a> <a id="18746" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="18784" class="Keyword">open</a> <a id="18789" class="Keyword">import</a> <a id="18796" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="18825" class="Keyword">open</a> <a id="18830" class="Keyword">import</a> <a id="18837" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="18867" class="Keyword">open</a> <a id="18872" class="Keyword">import</a> <a id="18879" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="18910" class="Keyword">open</a> <a id="18915" class="Keyword">import</a> <a id="18922" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="18948" class="Keyword">open</a> <a id="18953" class="Keyword">import</a> <a id="18960" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="19011" class="Keyword">open</a> <a id="19016" class="Keyword">import</a> <a id="19023" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="19077" class="Keyword">open</a> <a id="19082" class="Keyword">import</a> <a id="19089" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="19116" class="Keyword">open</a> <a id="19121" class="Keyword">import</a> <a id="19128" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="19161" class="Keyword">open</a> <a id="19166" class="Keyword">import</a> <a id="19173" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="19204" class="Keyword">open</a> <a id="19209" class="Keyword">import</a> <a id="19216" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="19253" class="Keyword">open</a> <a id="19258" class="Keyword">import</a> <a id="19265" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="19290" class="Keyword">open</a> <a id="19295" class="Keyword">import</a> <a id="19302" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="19334" class="Keyword">open</a> <a id="19339" class="Keyword">import</a> <a id="19346" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="19381" class="Keyword">open</a> <a id="19386" class="Keyword">import</a> <a id="19393" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="19422" class="Keyword">open</a> <a id="19427" class="Keyword">import</a> <a id="19434" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="19462" class="Keyword">open</a> <a id="19467" class="Keyword">import</a> <a id="19474" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="19499" class="Keyword">open</a> <a id="19504" class="Keyword">import</a> <a id="19511" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="19532" class="Keyword">open</a> <a id="19537" class="Keyword">import</a> <a id="19544" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="19580" class="Keyword">open</a> <a id="19585" class="Keyword">import</a> <a id="19592" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="19635" class="Keyword">open</a> <a id="19640" class="Keyword">import</a> <a id="19647" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="19672" class="Keyword">open</a> <a id="19677" class="Keyword">import</a> <a id="19684" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="19715" class="Keyword">open</a> <a id="19720" class="Keyword">import</a> <a id="19727" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="19759" class="Keyword">open</a> <a id="19764" class="Keyword">import</a> <a id="19771" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="19805" class="Keyword">open</a> <a id="19810" class="Keyword">import</a> <a id="19817" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="19873" class="Keyword">open</a> <a id="19878" class="Keyword">import</a> <a id="19885" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="19938" class="Keyword">open</a> <a id="19943" class="Keyword">import</a> <a id="19950" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="19977" class="Keyword">open</a> <a id="19982" class="Keyword">import</a> <a id="19989" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="20051" class="Keyword">open</a> <a id="20056" class="Keyword">import</a> <a id="20063" href="graph-theory.html" class="Module">graph-theory</a>
<a id="20076" class="Keyword">open</a> <a id="20081" class="Keyword">import</a> <a id="20088" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="20129" class="Keyword">open</a> <a id="20134" class="Keyword">import</a> <a id="20141" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="20170" class="Keyword">open</a> <a id="20175" class="Keyword">import</a> <a id="20182" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="20227" class="Keyword">open</a> <a id="20232" class="Keyword">import</a> <a id="20239" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="20283" class="Keyword">open</a> <a id="20288" class="Keyword">import</a> <a id="20295" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="20322" class="Keyword">open</a> <a id="20327" class="Keyword">import</a> <a id="20334" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="20375" class="Keyword">open</a> <a id="20380" class="Keyword">import</a> <a id="20387" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="20410" class="Keyword">open</a> <a id="20415" class="Keyword">import</a> <a id="20422" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="20471" class="Keyword">open</a> <a id="20476" class="Keyword">import</a> <a id="20483" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="20522" class="Keyword">open</a> <a id="20527" class="Keyword">import</a> <a id="20534" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="20575" class="Keyword">open</a> <a id="20580" class="Keyword">import</a> <a id="20587" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="20631" class="Keyword">open</a> <a id="20636" class="Keyword">import</a> <a id="20643" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="20680" class="Keyword">open</a> <a id="20685" class="Keyword">import</a> <a id="20692" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="20714" class="Keyword">open</a> <a id="20719" class="Keyword">import</a> <a id="20726" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="20756" class="Keyword">open</a> <a id="20761" class="Keyword">import</a> <a id="20768" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="20807" class="Keyword">open</a> <a id="20812" class="Keyword">import</a> <a id="20819" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="20857" class="Keyword">open</a> <a id="20862" class="Keyword">import</a> <a id="20869" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="20900" class="Keyword">open</a> <a id="20905" class="Keyword">import</a> <a id="20912" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="20970" class="Keyword">open</a> <a id="20975" class="Keyword">import</a> <a id="20982" href="group-theory.html" class="Module">group-theory</a>
<a id="20995" class="Keyword">open</a> <a id="21000" class="Keyword">import</a> <a id="21007" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="21035" class="Keyword">open</a> <a id="21040" class="Keyword">import</a> <a id="21047" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="21078" class="Keyword">open</a> <a id="21083" class="Keyword">import</a> <a id="21090" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="21126" class="Keyword">open</a> <a id="21131" class="Keyword">import</a> <a id="21138" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="21189" class="Keyword">open</a> <a id="21194" class="Keyword">import</a> <a id="21201" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="21233" class="Keyword">open</a> <a id="21238" class="Keyword">import</a> <a id="21245" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="21281" class="Keyword">open</a> <a id="21286" class="Keyword">import</a> <a id="21293" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="21322" class="Keyword">open</a> <a id="21327" class="Keyword">import</a> <a id="21334" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="21370" class="Keyword">open</a> <a id="21375" class="Keyword">import</a> <a id="21382" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="21411" class="Keyword">open</a> <a id="21416" class="Keyword">import</a> <a id="21423" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="21455" class="Keyword">open</a> <a id="21460" class="Keyword">import</a> <a id="21467" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="21492" class="Keyword">open</a> <a id="21497" class="Keyword">import</a> <a id="21504" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="21535" class="Keyword">open</a> <a id="21540" class="Keyword">import</a> <a id="21547" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="21594" class="Keyword">open</a> <a id="21599" class="Keyword">import</a> <a id="21606" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="21646" class="Keyword">open</a> <a id="21651" class="Keyword">import</a> <a id="21658" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="21695" class="Keyword">open</a> <a id="21700" class="Keyword">import</a> <a id="21707" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="21743" class="Keyword">open</a> <a id="21748" class="Keyword">import</a> <a id="21755" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="21787" class="Keyword">open</a> <a id="21792" class="Keyword">import</a> <a id="21799" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="21826" class="Keyword">open</a> <a id="21831" class="Keyword">import</a> <a id="21838" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="21858" class="Keyword">open</a> <a id="21863" class="Keyword">import</a> <a id="21870" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="21897" class="Keyword">open</a> <a id="21902" class="Keyword">import</a> <a id="21909" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="21951" class="Keyword">open</a> <a id="21956" class="Keyword">import</a> <a id="21963" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="22004" class="Keyword">open</a> <a id="22009" class="Keyword">import</a> <a id="22016" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="22050" class="Keyword">open</a> <a id="22055" class="Keyword">import</a> <a id="22062" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="22097" class="Keyword">open</a> <a id="22102" class="Keyword">import</a> <a id="22109" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="22147" class="Keyword">open</a> <a id="22152" class="Keyword">import</a> <a id="22159" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="22191" class="Keyword">open</a> <a id="22196" class="Keyword">import</a> <a id="22203" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="22244" class="Keyword">open</a> <a id="22249" class="Keyword">import</a> <a id="22256" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="22297" class="Keyword">open</a> <a id="22302" class="Keyword">import</a> <a id="22309" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="22349" class="Keyword">open</a> <a id="22354" class="Keyword">import</a> <a id="22361" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="22394" class="Keyword">open</a> <a id="22399" class="Keyword">import</a> <a id="22406" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="22443" class="Keyword">open</a> <a id="22448" class="Keyword">import</a> <a id="22455" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="22500" class="Keyword">open</a> <a id="22505" class="Keyword">import</a> <a id="22512" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="22533" class="Keyword">open</a> <a id="22538" class="Keyword">import</a> <a id="22545" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="22579" class="Keyword">open</a> <a id="22584" class="Keyword">import</a> <a id="22591" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="22633" class="Keyword">open</a> <a id="22638" class="Keyword">import</a> <a id="22645" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="22680" class="Keyword">open</a> <a id="22685" class="Keyword">import</a> <a id="22692" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="22731" class="Keyword">open</a> <a id="22736" class="Keyword">import</a> <a id="22743" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="22780" class="Keyword">open</a> <a id="22785" class="Keyword">import</a> <a id="22792" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="22816" class="Keyword">open</a> <a id="22821" class="Keyword">import</a> <a id="22828" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="22853" class="Keyword">open</a> <a id="22858" class="Keyword">import</a> <a id="22865" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="22896" class="Keyword">open</a> <a id="22901" class="Keyword">import</a> <a id="22908" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="22931" class="Keyword">open</a> <a id="22936" class="Keyword">import</a> <a id="22943" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="22991" class="Keyword">open</a> <a id="22996" class="Keyword">import</a> <a id="23003" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="23033" class="Keyword">open</a> <a id="23038" class="Keyword">import</a> <a id="23045" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="23115" class="Keyword">open</a> <a id="23120" class="Keyword">import</a> <a id="23127" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="23142" class="Keyword">open</a> <a id="23147" class="Keyword">import</a> <a id="23154" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="23187" class="Keyword">open</a> <a id="23192" class="Keyword">import</a> <a id="23199" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="23231" class="Keyword">open</a> <a id="23236" class="Keyword">import</a> <a id="23243" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="23285" class="Keyword">open</a> <a id="23290" class="Keyword">import</a> <a id="23297" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="23335" class="Keyword">open</a> <a id="23340" class="Keyword">import</a> <a id="23347" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="23384" class="Keyword">open</a> <a id="23389" class="Keyword">import</a> <a id="23396" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="23429" class="Keyword">open</a> <a id="23434" class="Keyword">import</a> <a id="23441" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="23465" class="Keyword">open</a> <a id="23470" class="Keyword">import</a> <a id="23477" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="23516" class="Keyword">open</a> <a id="23521" class="Keyword">import</a> <a id="23528" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="23574" class="Keyword">open</a> <a id="23579" class="Keyword">import</a> <a id="23586" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="23631" class="Keyword">open</a> <a id="23636" class="Keyword">import</a> <a id="23643" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="23681" class="Keyword">open</a> <a id="23686" class="Keyword">import</a> <a id="23693" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="23725" class="Keyword">open</a> <a id="23730" class="Keyword">import</a> <a id="23737" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="23790" class="Keyword">open</a> <a id="23795" class="Keyword">import</a> <a id="23802" href="order-theory.html" class="Module">order-theory</a>
<a id="23815" class="Keyword">open</a> <a id="23820" class="Keyword">import</a> <a id="23827" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="23854" class="Keyword">open</a> <a id="23859" class="Keyword">import</a> <a id="23866" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="23896" class="Keyword">open</a> <a id="23901" class="Keyword">import</a> <a id="23908" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="23941" class="Keyword">open</a> <a id="23946" class="Keyword">import</a> <a id="23953" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="23989" class="Keyword">open</a> <a id="23994" class="Keyword">import</a> <a id="24001" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="24028" class="Keyword">open</a> <a id="24033" class="Keyword">import</a> <a id="24040" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="24070" class="Keyword">open</a> <a id="24075" class="Keyword">import</a> <a id="24082" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="24118" class="Keyword">open</a> <a id="24123" class="Keyword">import</a> <a id="24130" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="24172" class="Keyword">open</a> <a id="24177" class="Keyword">import</a> <a id="24184" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="24216" class="Keyword">open</a> <a id="24221" class="Keyword">import</a> <a id="24228" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="24265" class="Keyword">open</a> <a id="24270" class="Keyword">import</a> <a id="24277" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="24317" class="Keyword">open</a> <a id="24322" class="Keyword">import</a> <a id="24329" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="24364" class="Keyword">open</a> <a id="24369" class="Keyword">import</a> <a id="24376" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="24414" class="Keyword">open</a> <a id="24419" class="Keyword">import</a> <a id="24426" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="24461" class="Keyword">open</a> <a id="24466" class="Keyword">import</a> <a id="24473" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="24508" class="Keyword">open</a> <a id="24513" class="Keyword">import</a> <a id="24520" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="24558" class="Keyword">open</a> <a id="24563" class="Keyword">import</a> <a id="24570" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="24601" class="Keyword">open</a> <a id="24606" class="Keyword">import</a> <a id="24613" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="24646" class="Keyword">open</a> <a id="24651" class="Keyword">import</a> <a id="24658" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="24678" class="Keyword">open</a> <a id="24683" class="Keyword">import</a> <a id="24690" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="24713" class="Keyword">open</a> <a id="24718" class="Keyword">import</a> <a id="24725" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="24748" class="Keyword">open</a> <a id="24753" class="Keyword">import</a> <a id="24760" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="24786" class="Keyword">open</a> <a id="24791" class="Keyword">import</a> <a id="24798" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="24824" class="Keyword">open</a> <a id="24829" class="Keyword">import</a> <a id="24836" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="24892" class="Keyword">open</a> <a id="24897" class="Keyword">import</a> <a id="24904" href="polytopes.html" class="Module">polytopes</a>
<a id="24914" class="Keyword">open</a> <a id="24919" class="Keyword">import</a> <a id="24926" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="24984" class="Keyword">open</a> <a id="24989" class="Keyword">import</a> <a id="24996" href="ring-theory.html" class="Module">ring-theory</a>
<a id="25008" class="Keyword">open</a> <a id="25013" class="Keyword">import</a> <a id="25020" href="ring-theory.commutative-rings.html" class="Module">ring-theory.commutative-rings</a>
<a id="25050" class="Keyword">open</a> <a id="25055" class="Keyword">import</a> <a id="25062" href="ring-theory.discrete-fields.html" class="Module">ring-theory.discrete-fields</a>
<a id="25090" class="Keyword">open</a> <a id="25095" class="Keyword">import</a> <a id="25102" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="25129" class="Keyword">open</a> <a id="25134" class="Keyword">import</a> <a id="25141" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a>
<a id="25173" class="Keyword">open</a> <a id="25178" class="Keyword">import</a> <a id="25185" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a>
<a id="25215" class="Keyword">open</a> <a id="25220" class="Keyword">import</a> <a id="25227" href="ring-theory.homomorphisms-commutative-rings.html" class="Module">ring-theory.homomorphisms-commutative-rings</a>
<a id="25271" class="Keyword">open</a> <a id="25276" class="Keyword">import</a> <a id="25283" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="25315" class="Keyword">open</a> <a id="25320" class="Keyword">import</a> <a id="25327" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="25373" class="Keyword">open</a> <a id="25378" class="Keyword">import</a> <a id="25385" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="25410" class="Keyword">open</a> <a id="25415" class="Keyword">import</a> <a id="25422" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="25460" class="Keyword">open</a> <a id="25465" class="Keyword">import</a> <a id="25472" href="ring-theory.isomorphisms-commutative-rings.html" class="Module">ring-theory.isomorphisms-commutative-rings</a>
<a id="25515" class="Keyword">open</a> <a id="25520" class="Keyword">import</a> <a id="25527" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="25558" class="Keyword">open</a> <a id="25563" class="Keyword">import</a> <a id="25570" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="25602" class="Keyword">open</a> <a id="25607" class="Keyword">import</a> <a id="25614" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="25643" class="Keyword">open</a> <a id="25648" class="Keyword">import</a> <a id="25655" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="25716" class="Keyword">open</a> <a id="25721" class="Keyword">import</a> <a id="25728" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="25754" class="Keyword">open</a> <a id="25759" class="Keyword">import</a> <a id="25766" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="25805" class="Keyword">open</a> <a id="25810" class="Keyword">import</a> <a id="25817" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="25855" class="Keyword">open</a> <a id="25860" class="Keyword">import</a> <a id="25867" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="25913" class="Keyword">open</a> <a id="25918" class="Keyword">import</a> <a id="25925" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="25962" class="Keyword">open</a> <a id="25967" class="Keyword">import</a> <a id="25974" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="26014" class="Keyword">open</a> <a id="26019" class="Keyword">import</a> <a id="26026" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="26065" class="Keyword">open</a> <a id="26070" class="Keyword">import</a> <a id="26077" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="26110" class="Keyword">open</a> <a id="26115" class="Keyword">import</a> <a id="26122" href="synthetic-homotopy-theory.commutative-operations.html" class="Module">synthetic-homotopy-theory.commutative-operations</a>
<a id="26171" class="Keyword">open</a> <a id="26176" class="Keyword">import</a> <a id="26183" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="26222" class="Keyword">open</a> <a id="26227" class="Keyword">import</a> <a id="26234" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="26279" class="Keyword">open</a> <a id="26284" class="Keyword">import</a> <a id="26291" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="26343" class="Keyword">open</a> <a id="26348" class="Keyword">import</a> <a id="26355" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="26408" class="Keyword">open</a> <a id="26413" class="Keyword">import</a> <a id="26420" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="26468" class="Keyword">open</a> <a id="26473" class="Keyword">import</a> <a id="26480" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="26520" class="Keyword">open</a> <a id="26525" class="Keyword">import</a> <a id="26532" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="26579" class="Keyword">open</a> <a id="26584" class="Keyword">import</a> <a id="26591" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="26629" class="Keyword">open</a> <a id="26634" class="Keyword">import</a> <a id="26641" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a>
<a id="26695" class="Keyword">open</a> <a id="26700" class="Keyword">import</a> <a id="26707" href="synthetic-homotopy-theory.pointed-equivalences.html" class="Module">synthetic-homotopy-theory.pointed-equivalences</a>
<a id="26754" class="Keyword">open</a> <a id="26759" class="Keyword">import</a> <a id="26766" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a>
<a id="26818" class="Keyword">open</a> <a id="26823" class="Keyword">import</a> <a id="26830" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a>
<a id="26875" class="Keyword">open</a> <a id="26880" class="Keyword">import</a> <a id="26887" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a>
<a id="26926" class="Keyword">open</a> <a id="26931" class="Keyword">import</a> <a id="26938" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>
<a id="26978" class="Keyword">open</a> <a id="26983" class="Keyword">import</a> <a id="26990" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="27023" class="Keyword">open</a> <a id="27028" class="Keyword">import</a> <a id="27035" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="27080" class="Keyword">open</a> <a id="27085" class="Keyword">import</a> <a id="27092" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="27168" class="Keyword">open</a> <a id="27173" class="Keyword">import</a> <a id="27180" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="27232" class="Keyword">open</a> <a id="27237" class="Keyword">import</a> <a id="27244" href="type-theories.html" class="Module">type-theories</a>
<a id="27258" class="Keyword">open</a> <a id="27263" class="Keyword">import</a> <a id="27270" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="27312" class="Keyword">open</a> <a id="27317" class="Keyword">import</a> <a id="27324" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="27362" class="Keyword">open</a> <a id="27367" class="Keyword">import</a> <a id="27374" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="27420" class="Keyword">open</a> <a id="27425" class="Keyword">import</a> <a id="27432" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="27479" class="Keyword">open</a> <a id="27484" class="Keyword">import</a> <a id="27491" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="27526" class="Keyword">open</a> <a id="27531" class="Keyword">import</a> <a id="27538" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="27616" class="Keyword">open</a> <a id="27621" class="Keyword">import</a> <a id="27628" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="27652" class="Keyword">open</a> <a id="27657" class="Keyword">import</a> <a id="27664" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="27717" class="Keyword">open</a> <a id="27722" class="Keyword">import</a> <a id="27729" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="27772" class="Keyword">open</a> <a id="27777" class="Keyword">import</a> <a id="27784" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="27824" class="Keyword">open</a> <a id="27829" class="Keyword">import</a> <a id="27836" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="27875" class="Keyword">open</a> <a id="27880" class="Keyword">import</a> <a id="27887" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="27935" class="Keyword">open</a> <a id="27940" class="Keyword">import</a> <a id="27947" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="27994" class="Keyword">open</a> <a id="27999" class="Keyword">import</a> <a id="28006" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="28058" class="Keyword">open</a> <a id="28063" class="Keyword">import</a> <a id="28070" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="28110" class="Keyword">open</a> <a id="28115" class="Keyword">import</a> <a id="28122" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="28174" class="Keyword">open</a> <a id="28179" class="Keyword">import</a> <a id="28186" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="28240" class="Keyword">open</a> <a id="28245" class="Keyword">import</a> <a id="28252" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="28291" class="Keyword">open</a> <a id="28296" class="Keyword">import</a> <a id="28303" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="28336" class="Keyword">open</a> <a id="28341" class="Keyword">import</a> <a id="28348" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="28378" class="Keyword">open</a> <a id="28383" class="Keyword">import</a> <a id="28390" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="28449" class="Keyword">open</a> <a id="28454" class="Keyword">import</a> <a id="28461" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="28516" class="Keyword">open</a> <a id="28521" class="Keyword">import</a> <a id="28528" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="28571" class="Keyword">open</a> <a id="28576" class="Keyword">import</a> <a id="28583" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="28632" class="Keyword">open</a> <a id="28637" class="Keyword">import</a> <a id="28644" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="28689" class="Keyword">open</a> <a id="28694" class="Keyword">import</a> <a id="28701" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="28752" class="Keyword">open</a> <a id="28757" class="Keyword">import</a> <a id="28764" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="28842" class="Keyword">open</a> <a id="28847" class="Keyword">import</a> <a id="28854" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="28894" class="Keyword">open</a> <a id="28899" class="Keyword">import</a> <a id="28906" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="28963" class="Keyword">open</a> <a id="28968" class="Keyword">import</a> <a id="28975" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="29010" class="Keyword">open</a> <a id="29015" class="Keyword">import</a> <a id="29022" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="29068" class="Keyword">open</a> <a id="29073" class="Keyword">import</a> <a id="29080" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="29135" class="Keyword">open</a> <a id="29140" class="Keyword">import</a> <a id="29147" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="29190" class="Keyword">open</a> <a id="29195" class="Keyword">import</a> <a id="29202" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="29261" class="Keyword">open</a> <a id="29266" class="Keyword">import</a> <a id="29273" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="29310" class="Keyword">open</a> <a id="29315" class="Keyword">import</a> <a id="29322" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="29361" class="Keyword">open</a> <a id="29366" class="Keyword">import</a> <a id="29373" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="29411" class="Keyword">open</a> <a id="29416" class="Keyword">import</a> <a id="29423" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="29475" class="Keyword">open</a> <a id="29480" class="Keyword">import</a> <a id="29487" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="29532" class="Keyword">open</a> <a id="29537" class="Keyword">import</a> <a id="29544" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="29581" class="Keyword">open</a> <a id="29586" class="Keyword">import</a> <a id="29593" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="29642" class="Keyword">open</a> <a id="29647" class="Keyword">import</a> <a id="29654" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="29693" class="Keyword">open</a> <a id="29698" class="Keyword">import</a> <a id="29705" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="29743" class="Keyword">open</a> <a id="29748" class="Keyword">import</a> <a id="29755" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="29810" class="Keyword">open</a> <a id="29815" class="Keyword">import</a> <a id="29822" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="29861" class="Keyword">open</a> <a id="29866" class="Keyword">import</a> <a id="29873" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="29920" class="Keyword">open</a> <a id="29925" class="Keyword">import</a> <a id="29932" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="29962" class="Keyword">open</a> <a id="29967" class="Keyword">import</a> <a id="29974" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="30004" class="Keyword">open</a> <a id="30009" class="Keyword">import</a> <a id="30016" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="30059" class="Keyword">open</a> <a id="30064" class="Keyword">import</a> <a id="30071" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="30106" class="Keyword">open</a> <a id="30111" class="Keyword">import</a> <a id="30118" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="30158" class="Keyword">open</a> <a id="30163" class="Keyword">import</a> <a id="30170" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="30215" class="Keyword">open</a> <a id="30220" class="Keyword">import</a> <a id="30227" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="30277" class="Keyword">open</a> <a id="30282" class="Keyword">import</a> <a id="30289" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="30327" class="Keyword">open</a> <a id="30332" class="Keyword">import</a> <a id="30339" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="30388" class="Keyword">open</a> <a id="30393" class="Keyword">import</a> <a id="30400" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="30463" class="Keyword">open</a> <a id="30468" class="Keyword">import</a> <a id="30475" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="30507" class="Keyword">open</a> <a id="30512" class="Keyword">import</a> <a id="30519" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="30572" class="Keyword">open</a> <a id="30577" class="Keyword">import</a> <a id="30584" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="30630" class="Keyword">open</a> <a id="30635" class="Keyword">import</a> <a id="30642" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="30688" class="Keyword">open</a> <a id="30693" class="Keyword">import</a> <a id="30700" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="30748" class="Keyword">open</a> <a id="30753" class="Keyword">import</a> <a id="30760" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
</pre>
## Wild algebra

<pre class="Agda"><a id="30830" class="Keyword">open</a> <a id="30835" class="Keyword">import</a> <a id="30842" href="wild-algebra.html" class="Module">wild-algebra</a>
<a id="30855" class="Keyword">open</a> <a id="30860" class="Keyword">import</a> <a id="30867" href="wild-algebra.magmas.html" class="Module">wild-algebra.magmas</a>
<a id="30887" class="Keyword">open</a> <a id="30892" class="Keyword">import</a> <a id="30899" href="wild-algebra.morphisms-magmas.html" class="Module">wild-algebra.morphisms-magmas</a>
<a id="30929" class="Keyword">open</a> <a id="30934" class="Keyword">import</a> <a id="30941" href="wild-algebra.morphisms-wild-unital-magmas.html" class="Module">wild-algebra.morphisms-wild-unital-magmas</a>
<a id="30983" class="Keyword">open</a> <a id="30988" class="Keyword">import</a> <a id="30995" href="wild-algebra.universal-property-lists-wild-monoids.html" class="Module">wild-algebra.universal-property-lists-wild-monoids</a>
<a id="31046" class="Keyword">open</a> <a id="31051" class="Keyword">import</a> <a id="31058" href="wild-algebra.wild-groups.html" class="Module">wild-algebra.wild-groups</a>
<a id="31083" class="Keyword">open</a> <a id="31088" class="Keyword">import</a> <a id="31095" href="wild-algebra.wild-loops.html" class="Module">wild-algebra.wild-loops</a>
<a id="31119" class="Keyword">open</a> <a id="31124" class="Keyword">import</a> <a id="31131" href="wild-algebra.wild-monoids.html" class="Module">wild-algebra.wild-monoids</a>
<a id="31157" class="Keyword">open</a> <a id="31162" class="Keyword">import</a> <a id="31169" href="wild-algebra.wild-quasigroups.html" class="Module">wild-algebra.wild-quasigroups</a>
<a id="31199" class="Keyword">open</a> <a id="31204" class="Keyword">import</a> <a id="31211" href="wild-algebra.wild-semigroups.html" class="Module">wild-algebra.wild-semigroups</a>
<a id="31240" class="Keyword">open</a> <a id="31245" class="Keyword">import</a> <a id="31252" href="wild-algebra.wild-unital-magmas.html" class="Module">wild-algebra.wild-unital-magmas</a>
</pre>
## Everything

See the list of all Agda modules [here](everything.html).

