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
<a id="4751" class="Keyword">open</a> <a id="4756" class="Keyword">import</a> <a id="4763" href="commutative-algebra.boolean-rings.html" class="Module">commutative-algebra.boolean-rings</a>
<a id="4797" class="Keyword">open</a> <a id="4802" class="Keyword">import</a> <a id="4809" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>
<a id="4847" class="Keyword">open</a> <a id="4852" class="Keyword">import</a> <a id="4859" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a>
<a id="4895" class="Keyword">open</a> <a id="4900" class="Keyword">import</a> <a id="4907" href="commutative-algebra.eisenstein-integers.html" class="Module">commutative-algebra.eisenstein-integers</a>
<a id="4947" class="Keyword">open</a> <a id="4952" class="Keyword">import</a> <a id="4959" href="commutative-algebra.gaussian-integers.html" class="Module">commutative-algebra.gaussian-integers</a>
<a id="4997" class="Keyword">open</a> <a id="5002" class="Keyword">import</a> <a id="5009" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a>
<a id="5061" class="Keyword">open</a> <a id="5066" class="Keyword">import</a> <a id="5073" href="commutative-algebra.ideals-commutative-rings.html" class="Module">commutative-algebra.ideals-commutative-rings</a>
<a id="5118" class="Keyword">open</a> <a id="5123" class="Keyword">import</a> <a id="5130" href="commutative-algebra.integral-domains.html" class="Module">commutative-algebra.integral-domains</a>
<a id="5167" class="Keyword">open</a> <a id="5172" class="Keyword">import</a> <a id="5179" href="commutative-algebra.invertible-elements-commutative-rings.html" class="Module">commutative-algebra.invertible-elements-commutative-rings</a>
<a id="5237" class="Keyword">open</a> <a id="5242" class="Keyword">import</a> <a id="5249" href="commutative-algebra.isomorphisms-commutative-rings.html" class="Module">commutative-algebra.isomorphisms-commutative-rings</a>
<a id="5300" class="Keyword">open</a> <a id="5305" class="Keyword">import</a> <a id="5312" href="commutative-algebra.local-commutative-rings.html" class="Module">commutative-algebra.local-commutative-rings</a>
<a id="5356" class="Keyword">open</a> <a id="5361" class="Keyword">import</a> <a id="5368" href="commutative-algebra.maximal-ideals-commutative-rings.html" class="Module">commutative-algebra.maximal-ideals-commutative-rings</a>
<a id="5421" class="Keyword">open</a> <a id="5426" class="Keyword">import</a> <a id="5433" href="commutative-algebra.prime-ideals-commutative-rings.html" class="Module">commutative-algebra.prime-ideals-commutative-rings</a>
<a id="5484" class="Keyword">open</a> <a id="5489" class="Keyword">import</a> <a id="5496" href="commutative-algebra.zariski-topology.html" class="Module">commutative-algebra.zariski-topology</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="5575" class="Keyword">open</a> <a id="5580" class="Keyword">import</a> <a id="5587" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5612" class="Keyword">open</a> <a id="5617" class="Keyword">import</a> <a id="5624" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5673" class="Keyword">open</a> <a id="5678" class="Keyword">import</a> <a id="5685" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5728" class="Keyword">open</a> <a id="5733" class="Keyword">import</a> <a id="5740" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5790" class="Keyword">open</a> <a id="5795" class="Keyword">import</a> <a id="5802" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5848" class="Keyword">open</a> <a id="5853" class="Keyword">import</a> <a id="5860" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5907" class="Keyword">open</a> <a id="5912" class="Keyword">import</a> <a id="5919" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5978" class="Keyword">open</a> <a id="5983" class="Keyword">import</a> <a id="5990" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="6031" class="Keyword">open</a> <a id="6036" class="Keyword">import</a> <a id="6043" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="6086" class="Keyword">open</a> <a id="6091" class="Keyword">import</a> <a id="6098" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="6142" class="Keyword">open</a> <a id="6147" class="Keyword">import</a> <a id="6154" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="6199" class="Keyword">open</a> <a id="6204" class="Keyword">import</a> <a id="6211" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="6263" class="Keyword">open</a> <a id="6268" class="Keyword">import</a> <a id="6275" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="6335" class="Keyword">open</a> <a id="6340" class="Keyword">import</a> <a id="6347" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="6388" class="Keyword">open</a> <a id="6393" class="Keyword">import</a> <a id="6400" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6445" class="Keyword">open</a> <a id="6450" class="Keyword">import</a> <a id="6457" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6504" class="Keyword">open</a> <a id="6509" class="Keyword">import</a> <a id="6516" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6559" class="Keyword">open</a> <a id="6564" class="Keyword">import</a> <a id="6571" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6621" class="Keyword">open</a> <a id="6626" class="Keyword">import</a> <a id="6633" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6680" class="Keyword">open</a> <a id="6685" class="Keyword">import</a> <a id="6692" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6749" class="Keyword">open</a> <a id="6754" class="Keyword">import</a> <a id="6761" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6815" class="Keyword">open</a> <a id="6820" class="Keyword">import</a> <a id="6827" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6887" class="Keyword">open</a> <a id="6892" class="Keyword">import</a> <a id="6899" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6942" class="Keyword">open</a> <a id="6947" class="Keyword">import</a> <a id="6954" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="7004" class="Keyword">open</a> <a id="7009" class="Keyword">import</a> <a id="7016" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="7076" class="Keyword">open</a> <a id="7081" class="Keyword">import</a> <a id="7088" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="7137" class="Keyword">open</a> <a id="7142" class="Keyword">import</a> <a id="7149" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="7205" class="Keyword">open</a> <a id="7210" class="Keyword">import</a> <a id="7217" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="7253" class="Keyword">open</a> <a id="7258" class="Keyword">import</a> <a id="7265" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="7309" class="Keyword">open</a> <a id="7314" class="Keyword">import</a> <a id="7321" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="7365" class="Keyword">open</a> <a id="7370" class="Keyword">import</a> <a id="7377" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7427" class="Keyword">open</a> <a id="7432" class="Keyword">import</a> <a id="7439" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7485" class="Keyword">open</a> <a id="7490" class="Keyword">import</a> <a id="7497" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7532" class="Keyword">open</a> <a id="7537" class="Keyword">import</a> <a id="7544" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7589" class="Keyword">open</a> <a id="7594" class="Keyword">import</a> <a id="7601" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7659" class="Keyword">open</a> <a id="7664" class="Keyword">import</a> <a id="7671" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7736" class="Keyword">open</a> <a id="7741" class="Keyword">import</a> <a id="7748" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7791" class="Keyword">open</a> <a id="7796" class="Keyword">import</a> <a id="7803" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7857" class="Keyword">open</a> <a id="7862" class="Keyword">import</a> <a id="7869" href="elementary-number-theory.half-integers.html" class="Module">elementary-number-theory.half-integers</a>
<a id="7908" class="Keyword">open</a> <a id="7913" class="Keyword">import</a> <a id="7920" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7965" class="Keyword">open</a> <a id="7970" class="Keyword">import</a> <a id="7977" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="8029" class="Keyword">open</a> <a id="8034" class="Keyword">import</a> <a id="8041" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="8099" class="Keyword">open</a> <a id="8104" class="Keyword">import</a> <a id="8111" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="8157" class="Keyword">open</a> <a id="8162" class="Keyword">import</a> <a id="8169" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="8213" class="Keyword">open</a> <a id="8218" class="Keyword">import</a> <a id="8225" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="8259" class="Keyword">open</a> <a id="8264" class="Keyword">import</a> <a id="8271" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="8325" class="Keyword">open</a> <a id="8330" class="Keyword">import</a> <a id="8337" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="8386" class="Keyword">open</a> <a id="8391" class="Keyword">import</a> <a id="8398" href="elementary-number-theory.maximum-standard-finite-types.html" class="Module">elementary-number-theory.maximum-standard-finite-types</a>
<a id="8453" class="Keyword">open</a> <a id="8458" class="Keyword">import</a> <a id="8465" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="8506" class="Keyword">open</a> <a id="8511" class="Keyword">import</a> <a id="8518" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8567" class="Keyword">open</a> <a id="8572" class="Keyword">import</a> <a id="8579" href="elementary-number-theory.minimum-standard-finite-types.html" class="Module">elementary-number-theory.minimum-standard-finite-types</a>
<a id="8634" class="Keyword">open</a> <a id="8639" class="Keyword">import</a> <a id="8646" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8712" class="Keyword">open</a> <a id="8717" class="Keyword">import</a> <a id="8724" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8768" class="Keyword">open</a> <a id="8773" class="Keyword">import</a> <a id="8780" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8829" class="Keyword">open</a> <a id="8834" class="Keyword">import</a> <a id="8841" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8897" class="Keyword">open</a> <a id="8902" class="Keyword">import</a> <a id="8909" href="elementary-number-theory.multiset-coefficients.html" class="Module">elementary-number-theory.multiset-coefficients</a>
<a id="8956" class="Keyword">open</a> <a id="8961" class="Keyword">import</a> <a id="8968" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="9009" class="Keyword">open</a> <a id="9014" class="Keyword">import</a> <a id="9021" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="9070" class="Keyword">open</a> <a id="9075" class="Keyword">import</a> <a id="9082" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="9141" class="Keyword">open</a> <a id="9146" class="Keyword">import</a> <a id="9153" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="9192" class="Keyword">open</a> <a id="9197" class="Keyword">import</a> <a id="9204" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="9257" class="Keyword">open</a> <a id="9262" class="Keyword">import</a> <a id="9269" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="9326" class="Keyword">open</a> <a id="9331" class="Keyword">import</a> <a id="9338" href="elementary-number-theory.pythagorean-triples.html" class="Module">elementary-number-theory.pythagorean-triples</a>
<a id="9383" class="Keyword">open</a> <a id="9388" class="Keyword">import</a> <a id="9395" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="9437" class="Keyword">open</a> <a id="9442" class="Keyword">import</a> <a id="9449" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="9500" class="Keyword">open</a> <a id="9505" class="Keyword">import</a> <a id="9512" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9570" class="Keyword">open</a> <a id="9575" class="Keyword">import</a> <a id="9582" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9646" class="Keyword">open</a> <a id="9651" class="Keyword">import</a> <a id="9658" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9711" class="Keyword">open</a> <a id="9716" class="Keyword">import</a> <a id="9723" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9776" class="Keyword">open</a> <a id="9781" class="Keyword">import</a> <a id="9788" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9849" class="Keyword">open</a> <a id="9854" class="Keyword">import</a> <a id="9861" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9919" class="Keyword">open</a> <a id="9924" class="Keyword">import</a> <a id="9931" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9980" class="Keyword">open</a> <a id="9985" class="Keyword">import</a> <a id="9992" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="10035" class="Keyword">open</a> <a id="10040" class="Keyword">import</a> <a id="10047" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="10091" class="Keyword">open</a> <a id="10096" class="Keyword">import</a> <a id="10103" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="10150" class="Keyword">open</a> <a id="10155" class="Keyword">import</a> <a id="10162" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="10223" class="Keyword">open</a> <a id="10228" class="Keyword">import</a> <a id="10235" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="10298" class="Keyword">open</a> <a id="10303" class="Keyword">import</a> <a id="10310" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="10370" class="Keyword">open</a> <a id="10375" class="Keyword">import</a> <a id="10382" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="10436" class="Keyword">open</a> <a id="10441" class="Keyword">import</a> <a id="10448" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="10513" class="Keyword">open</a> <a id="10518" class="Keyword">import</a> <a id="10525" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10633" class="Keyword">open</a> <a id="10638" class="Keyword">import</a> <a id="10645" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10665" class="Keyword">open</a> <a id="10670" class="Keyword">import</a> <a id="10677" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10723" class="Keyword">open</a> <a id="10728" class="Keyword">import</a> <a id="10735" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a>
<a id="10774" class="Keyword">open</a> <a id="10779" class="Keyword">import</a> <a id="10786" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10842" class="Keyword">open</a> <a id="10847" class="Keyword">import</a> <a id="10854" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10900" class="Keyword">open</a> <a id="10905" class="Keyword">import</a> <a id="10912" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10946" class="Keyword">open</a> <a id="10951" class="Keyword">import</a> <a id="10958" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10993" class="Keyword">open</a> <a id="10998" class="Keyword">import</a> <a id="11005" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="11043" class="Keyword">open</a> <a id="11048" class="Keyword">import</a> <a id="11055" href="finite-group-theory.finite-type-groups.html" class="Module">finite-group-theory.finite-type-groups</a>
<a id="11094" class="Keyword">open</a> <a id="11099" class="Keyword">import</a> <a id="11106" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="11144" class="Keyword">open</a> <a id="11149" class="Keyword">import</a> <a id="11156" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="11196" class="Keyword">open</a> <a id="11201" class="Keyword">import</a> <a id="11208" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="11241" class="Keyword">open</a> <a id="11246" class="Keyword">import</a> <a id="11253" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="11291" class="Keyword">open</a> <a id="11296" class="Keyword">import</a> <a id="11303" href="finite-group-theory.simpson-delooping-sign-homomorphism.html" class="Module">finite-group-theory.simpson-delooping-sign-homomorphism</a>
<a id="11359" class="Keyword">open</a> <a id="11364" class="Keyword">import</a> <a id="11371" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="11413" class="Keyword">open</a> <a id="11418" class="Keyword">import</a> <a id="11425" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="11488" class="Keyword">open</a> <a id="11493" class="Keyword">import</a> <a id="11500" href="foundation.html" class="Module">foundation</a>
<a id="11511" class="Keyword">open</a> <a id="11516" class="Keyword">import</a> <a id="11523" href="foundation.0-connected-types.html" class="Module">foundation.0-connected-types</a>
<a id="11552" class="Keyword">open</a> <a id="11557" class="Keyword">import</a> <a id="11564" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a>
<a id="11592" class="Keyword">open</a> <a id="11597" class="Keyword">import</a> <a id="11604" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11622" class="Keyword">open</a> <a id="11627" class="Keyword">import</a> <a id="11634" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11653" class="Keyword">open</a> <a id="11658" class="Keyword">import</a> <a id="11665" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11684" class="Keyword">open</a> <a id="11689" class="Keyword">import</a> <a id="11696" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11740" class="Keyword">open</a> <a id="11745" class="Keyword">import</a> <a id="11752" href="foundation.apartness-relations.html" class="Module">foundation.apartness-relations</a>
<a id="11783" class="Keyword">open</a> <a id="11788" class="Keyword">import</a> <a id="11795" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11820" class="Keyword">open</a> <a id="11825" class="Keyword">import</a> <a id="11832" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11859" class="Keyword">open</a> <a id="11864" class="Keyword">import</a> <a id="11871" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11888" class="Keyword">open</a> <a id="11893" class="Keyword">import</a> <a id="11900" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="11929" class="Keyword">open</a> <a id="11934" class="Keyword">import</a> <a id="11941" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="11997" class="Keyword">open</a> <a id="12002" class="Keyword">import</a> <a id="12009" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="12040" class="Keyword">open</a> <a id="12045" class="Keyword">import</a> <a id="12052" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="12106" class="Keyword">open</a> <a id="12111" class="Keyword">import</a> <a id="12118" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="12146" class="Keyword">open</a> <a id="12151" class="Keyword">import</a> <a id="12158" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="12188" class="Keyword">open</a> <a id="12193" class="Keyword">import</a> <a id="12200" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="12220" class="Keyword">open</a> <a id="12225" class="Keyword">import</a> <a id="12232" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="12277" class="Keyword">open</a> <a id="12282" class="Keyword">import</a> <a id="12289" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="12326" class="Keyword">open</a> <a id="12331" class="Keyword">import</a> <a id="12338" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="12373" class="Keyword">open</a> <a id="12378" class="Keyword">import</a> <a id="12385" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="12443" class="Keyword">open</a> <a id="12448" class="Keyword">import</a> <a id="12455" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12493" class="Keyword">open</a> <a id="12498" class="Keyword">import</a> <a id="12505" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12539" class="Keyword">open</a> <a id="12544" class="Keyword">import</a> <a id="12551" href="foundation.commuting-cubes.html" class="Module">foundation.commuting-cubes</a>
<a id="12578" class="Keyword">open</a> <a id="12583" class="Keyword">import</a> <a id="12590" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12619" class="Keyword">open</a> <a id="12624" class="Keyword">import</a> <a id="12631" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12654" class="Keyword">open</a> <a id="12659" class="Keyword">import</a> <a id="12666" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12693" class="Keyword">open</a> <a id="12698" class="Keyword">import</a> <a id="12705" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12728" class="Keyword">open</a> <a id="12733" class="Keyword">import</a> <a id="12740" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12782" class="Keyword">open</a> <a id="12787" class="Keyword">import</a> <a id="12794" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12826" class="Keyword">open</a> <a id="12831" class="Keyword">import</a> <a id="12838" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="12864" class="Keyword">open</a> <a id="12869" class="Keyword">import</a> <a id="12876" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12903" class="Keyword">open</a> <a id="12908" class="Keyword">import</a> <a id="12915" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="12940" class="Keyword">open</a> <a id="12945" class="Keyword">import</a> <a id="12952" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="12981" class="Keyword">open</a> <a id="12986" class="Keyword">import</a> <a id="12993" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="13023" class="Keyword">open</a> <a id="13028" class="Keyword">import</a> <a id="13035" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="13062" class="Keyword">open</a> <a id="13067" class="Keyword">import</a> <a id="13074" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="13093" class="Keyword">open</a> <a id="13098" class="Keyword">import</a> <a id="13105" href="foundation.cospans.html" class="Module">foundation.cospans</a>
<a id="13124" class="Keyword">open</a> <a id="13129" class="Keyword">import</a> <a id="13136" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="13182" class="Keyword">open</a> <a id="13187" class="Keyword">import</a> <a id="13194" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="13236" class="Keyword">open</a> <a id="13241" class="Keyword">import</a> <a id="13248" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="13280" class="Keyword">open</a> <a id="13285" class="Keyword">import</a> <a id="13292" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="13322" class="Keyword">open</a> <a id="13327" class="Keyword">import</a> <a id="13334" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="13377" class="Keyword">open</a> <a id="13382" class="Keyword">import</a> <a id="13389" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="13415" class="Keyword">open</a> <a id="13420" class="Keyword">import</a> <a id="13427" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="13461" class="Keyword">open</a> <a id="13466" class="Keyword">import</a> <a id="13473" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="13504" class="Keyword">open</a> <a id="13509" class="Keyword">import</a> <a id="13516" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13546" class="Keyword">open</a> <a id="13551" class="Keyword">import</a> <a id="13558" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13585" class="Keyword">open</a> <a id="13590" class="Keyword">import</a> <a id="13597" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13635" class="Keyword">open</a> <a id="13640" class="Keyword">import</a> <a id="13647" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13679" class="Keyword">open</a> <a id="13684" class="Keyword">import</a> <a id="13691" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13726" class="Keyword">open</a> <a id="13731" class="Keyword">import</a> <a id="13738" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13778" class="Keyword">open</a> <a id="13783" class="Keyword">import</a> <a id="13790" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13821" class="Keyword">open</a> <a id="13826" class="Keyword">import</a> <a id="13833" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13867" class="Keyword">open</a> <a id="13872" class="Keyword">import</a> <a id="13879" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="13908" class="Keyword">open</a> <a id="13913" class="Keyword">import</a> <a id="13920" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="13943" class="Keyword">open</a> <a id="13948" class="Keyword">import</a> <a id="13955" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="13982" class="Keyword">open</a> <a id="13987" class="Keyword">import</a> <a id="13994" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="14022" class="Keyword">open</a> <a id="14027" class="Keyword">import</a> <a id="14034" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="14071" class="Keyword">open</a> <a id="14076" class="Keyword">import</a> <a id="14083" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="14131" class="Keyword">open</a> <a id="14136" class="Keyword">import</a> <a id="14143" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="14183" class="Keyword">open</a> <a id="14188" class="Keyword">import</a> <a id="14195" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="14217" class="Keyword">open</a> <a id="14222" class="Keyword">import</a> <a id="14229" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="14252" class="Keyword">open</a> <a id="14257" class="Keyword">import</a> <a id="14264" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="14289" class="Keyword">open</a> <a id="14294" class="Keyword">import</a> <a id="14301" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="14346" class="Keyword">open</a> <a id="14351" class="Keyword">import</a> <a id="14358" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="14402" class="Keyword">open</a> <a id="14407" class="Keyword">import</a> <a id="14414" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14450" class="Keyword">open</a> <a id="14455" class="Keyword">import</a> <a id="14462" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14507" class="Keyword">open</a> <a id="14512" class="Keyword">import</a> <a id="14519" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14560" class="Keyword">open</a> <a id="14565" class="Keyword">import</a> <a id="14572" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14607" class="Keyword">open</a> <a id="14612" class="Keyword">import</a> <a id="14619" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14651" class="Keyword">open</a> <a id="14656" class="Keyword">import</a> <a id="14663" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14694" class="Keyword">open</a> <a id="14699" class="Keyword">import</a> <a id="14706" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14739" class="Keyword">open</a> <a id="14744" class="Keyword">import</a> <a id="14751" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14784" class="Keyword">open</a> <a id="14789" class="Keyword">import</a> <a id="14796" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14826" class="Keyword">open</a> <a id="14831" class="Keyword">import</a> <a id="14838" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14862" class="Keyword">open</a> <a id="14867" class="Keyword">import</a> <a id="14874" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14912" class="Keyword">open</a> <a id="14917" class="Keyword">import</a> <a id="14924" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="14955" class="Keyword">open</a> <a id="14960" class="Keyword">import</a> <a id="14967" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="14992" class="Keyword">open</a> <a id="14997" class="Keyword">import</a> <a id="15004" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="15032" class="Keyword">open</a> <a id="15037" class="Keyword">import</a> <a id="15044" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="15068" class="Keyword">open</a> <a id="15073" class="Keyword">import</a> <a id="15080" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="15106" class="Keyword">open</a> <a id="15111" class="Keyword">import</a> <a id="15118" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="15153" class="Keyword">open</a> <a id="15158" class="Keyword">import</a> <a id="15165" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="15186" class="Keyword">open</a> <a id="15191" class="Keyword">import</a> <a id="15198" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="15247" class="Keyword">open</a> <a id="15252" class="Keyword">import</a> <a id="15259" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="15300" class="Keyword">open</a> <a id="15305" class="Keyword">import</a> <a id="15312" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="15362" class="Keyword">open</a> <a id="15367" class="Keyword">import</a> <a id="15374" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="15420" class="Keyword">open</a> <a id="15425" class="Keyword">import</a> <a id="15432" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15472" class="Keyword">open</a> <a id="15477" class="Keyword">import</a> <a id="15484" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15524" class="Keyword">open</a> <a id="15529" class="Keyword">import</a> <a id="15536" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15586" class="Keyword">open</a> <a id="15591" class="Keyword">import</a> <a id="15598" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15637" class="Keyword">open</a> <a id="15642" class="Keyword">import</a> <a id="15649" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15689" class="Keyword">open</a> <a id="15694" class="Keyword">import</a> <a id="15701" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15734" class="Keyword">open</a> <a id="15739" class="Keyword">import</a> <a id="15746" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15795" class="Keyword">open</a> <a id="15800" class="Keyword">import</a> <a id="15807" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15832" class="Keyword">open</a> <a id="15837" class="Keyword">import</a> <a id="15844" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="15883" class="Keyword">open</a> <a id="15888" class="Keyword">import</a> <a id="15895" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="15933" class="Keyword">open</a> <a id="15938" class="Keyword">import</a> <a id="15945" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="15967" class="Keyword">open</a> <a id="15972" class="Keyword">import</a> <a id="15979" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="16007" class="Keyword">open</a> <a id="16012" class="Keyword">import</a> <a id="16019" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="16055" class="Keyword">open</a> <a id="16060" class="Keyword">import</a> <a id="16067" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="16093" class="Keyword">open</a> <a id="16098" class="Keyword">import</a> <a id="16105" href="foundation.images.html" class="Module">foundation.images</a>
<a id="16123" class="Keyword">open</a> <a id="16128" class="Keyword">import</a> <a id="16135" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="16170" class="Keyword">open</a> <a id="16175" class="Keyword">import</a> <a id="16182" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="16217" class="Keyword">open</a> <a id="16222" class="Keyword">import</a> <a id="16229" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="16256" class="Keyword">open</a> <a id="16261" class="Keyword">import</a> <a id="16268" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="16324" class="Keyword">open</a> <a id="16329" class="Keyword">import</a> <a id="16336" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="16365" class="Keyword">open</a> <a id="16370" class="Keyword">import</a> <a id="16377" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="16407" class="Keyword">open</a> <a id="16412" class="Keyword">import</a> <a id="16419" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="16446" class="Keyword">open</a> <a id="16451" class="Keyword">import</a> <a id="16458" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16484" class="Keyword">open</a> <a id="16489" class="Keyword">import</a> <a id="16496" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16523" class="Keyword">open</a> <a id="16528" class="Keyword">import</a> <a id="16535" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16559" class="Keyword">open</a> <a id="16564" class="Keyword">import</a> <a id="16571" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16594" class="Keyword">open</a> <a id="16599" class="Keyword">import</a> <a id="16606" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16633" class="Keyword">open</a> <a id="16638" class="Keyword">import</a> <a id="16645" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16677" class="Keyword">open</a> <a id="16682" class="Keyword">import</a> <a id="16689" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16724" class="Keyword">open</a> <a id="16729" class="Keyword">import</a> <a id="16736" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16767" class="Keyword">open</a> <a id="16772" class="Keyword">import</a> <a id="16779" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16812" class="Keyword">open</a> <a id="16817" class="Keyword">import</a> <a id="16824" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16858" class="Keyword">open</a> <a id="16863" class="Keyword">import</a> <a id="16870" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="16910" class="Keyword">open</a> <a id="16915" class="Keyword">import</a> <a id="16922" href="foundation.lesser-limited-principle-of-omniscience.html" class="Module">foundation.lesser-limited-principle-of-omniscience</a>
<a id="16973" class="Keyword">open</a> <a id="16978" class="Keyword">import</a> <a id="16985" href="foundation.limited-principle-of-omniscience.html" class="Module">foundation.limited-principle-of-omniscience</a>
<a id="17029" class="Keyword">open</a> <a id="17034" class="Keyword">import</a> <a id="17041" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="17072" class="Keyword">open</a> <a id="17077" class="Keyword">import</a> <a id="17084" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="17116" class="Keyword">open</a> <a id="17121" class="Keyword">import</a> <a id="17128" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="17159" class="Keyword">open</a> <a id="17164" class="Keyword">import</a> <a id="17171" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="17188" class="Keyword">open</a> <a id="17193" class="Keyword">import</a> <a id="17200" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="17225" class="Keyword">open</a> <a id="17230" class="Keyword">import</a> <a id="17237" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="17266" class="Keyword">open</a> <a id="17271" class="Keyword">import</a> <a id="17278" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="17303" class="Keyword">open</a> <a id="17308" class="Keyword">import</a> <a id="17315" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="17344" class="Keyword">open</a> <a id="17349" class="Keyword">import</a> <a id="17356" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="17377" class="Keyword">open</a> <a id="17382" class="Keyword">import</a> <a id="17389" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="17413" class="Keyword">open</a> <a id="17418" class="Keyword">import</a> <a id="17425" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="17445" class="Keyword">open</a> <a id="17450" class="Keyword">import</a> <a id="17457" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="17491" class="Keyword">open</a> <a id="17496" class="Keyword">import</a> <a id="17503" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17541" class="Keyword">open</a> <a id="17546" class="Keyword">import</a> <a id="17553" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17581" class="Keyword">open</a> <a id="17586" class="Keyword">import</a> <a id="17593" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17617" class="Keyword">open</a> <a id="17622" class="Keyword">import</a> <a id="17629" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17656" class="Keyword">open</a> <a id="17661" class="Keyword">import</a> <a id="17668" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17703" class="Keyword">open</a> <a id="17708" class="Keyword">import</a> <a id="17715" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17736" class="Keyword">open</a> <a id="17741" class="Keyword">import</a> <a id="17748" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17784" class="Keyword">open</a> <a id="17789" class="Keyword">import</a> <a id="17796" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17841" class="Keyword">open</a> <a id="17846" class="Keyword">import</a> <a id="17853" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17899" class="Keyword">open</a> <a id="17904" class="Keyword">import</a> <a id="17911" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17951" class="Keyword">open</a> <a id="17956" class="Keyword">import</a> <a id="17963" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17993" class="Keyword">open</a> <a id="17998" class="Keyword">import</a> <a id="18005" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="18039" class="Keyword">open</a> <a id="18044" class="Keyword">import</a> <a id="18051" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="18088" class="Keyword">open</a> <a id="18093" class="Keyword">import</a> <a id="18100" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="18124" class="Keyword">open</a> <a id="18129" class="Keyword">import</a> <a id="18136" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="18157" class="Keyword">open</a> <a id="18162" class="Keyword">import</a> <a id="18169" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="18204" class="Keyword">open</a> <a id="18209" class="Keyword">import</a> <a id="18216" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="18253" class="Keyword">open</a> <a id="18258" class="Keyword">import</a> <a id="18265" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="18314" class="Keyword">open</a> <a id="18319" class="Keyword">import</a> <a id="18326" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="18359" class="Keyword">open</a> <a id="18364" class="Keyword">import</a> <a id="18371" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="18394" class="Keyword">open</a> <a id="18399" class="Keyword">import</a> <a id="18406" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="18429" class="Keyword">open</a> <a id="18434" class="Keyword">import</a> <a id="18441" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18464" class="Keyword">open</a> <a id="18469" class="Keyword">import</a> <a id="18476" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18504" class="Keyword">open</a> <a id="18509" class="Keyword">import</a> <a id="18516" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18536" class="Keyword">open</a> <a id="18541" class="Keyword">import</a> <a id="18548" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18569" class="Keyword">open</a> <a id="18574" class="Keyword">import</a> <a id="18581" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18612" class="Keyword">open</a> <a id="18617" class="Keyword">import</a> <a id="18624" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18651" class="Keyword">open</a> <a id="18656" class="Keyword">import</a> <a id="18663" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18679" class="Keyword">open</a> <a id="18684" class="Keyword">import</a> <a id="18691" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18722" class="Keyword">open</a> <a id="18727" class="Keyword">import</a> <a id="18734" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18751" class="Keyword">open</a> <a id="18756" class="Keyword">import</a> <a id="18763" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18785" class="Keyword">open</a> <a id="18790" class="Keyword">import</a> <a id="18797" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18824" class="Keyword">open</a> <a id="18829" class="Keyword">import</a> <a id="18836" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18859" class="Keyword">open</a> <a id="18864" class="Keyword">import</a> <a id="18871" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18898" class="Keyword">open</a> <a id="18903" class="Keyword">import</a> <a id="18910" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18943" class="Keyword">open</a> <a id="18948" class="Keyword">import</a> <a id="18955" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18995" class="Keyword">open</a> <a id="19000" class="Keyword">import</a> <a id="19007" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="19028" class="Keyword">open</a> <a id="19033" class="Keyword">import</a> <a id="19040" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="19069" class="Keyword">open</a> <a id="19074" class="Keyword">import</a> <a id="19081" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="19119" class="Keyword">open</a> <a id="19124" class="Keyword">import</a> <a id="19131" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="19151" class="Keyword">open</a> <a id="19156" class="Keyword">import</a> <a id="19163" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="19187" class="Keyword">open</a> <a id="19192" class="Keyword">import</a> <a id="19199" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="19226" class="Keyword">open</a> <a id="19231" class="Keyword">import</a> <a id="19238" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="19270" class="Keyword">open</a> <a id="19275" class="Keyword">import</a> <a id="19282" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="19312" class="Keyword">open</a> <a id="19317" class="Keyword">import</a> <a id="19324" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19350" class="Keyword">open</a> <a id="19355" class="Keyword">import</a> <a id="19362" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19389" class="Keyword">open</a> <a id="19394" class="Keyword">import</a> <a id="19401" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19438" class="Keyword">open</a> <a id="19443" class="Keyword">import</a> <a id="19450" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19479" class="Keyword">open</a> <a id="19484" class="Keyword">import</a> <a id="19491" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19514" class="Keyword">open</a> <a id="19519" class="Keyword">import</a> <a id="19526" href="foundation.type-arithmetic-booleans.html" class="Module">foundation.type-arithmetic-booleans</a>
<a id="19562" class="Keyword">open</a> <a id="19567" class="Keyword">import</a> <a id="19574" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19625" class="Keyword">open</a> <a id="19630" class="Keyword">import</a> <a id="19637" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19680" class="Keyword">open</a> <a id="19685" class="Keyword">import</a> <a id="19692" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19744" class="Keyword">open</a> <a id="19749" class="Keyword">import</a> <a id="19756" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19804" class="Keyword">open</a> <a id="19809" class="Keyword">import</a> <a id="19816" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19854" class="Keyword">open</a> <a id="19859" class="Keyword">import</a> <a id="19866" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19903" class="Keyword">open</a> <a id="19908" class="Keyword">import</a> <a id="19915" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19961" class="Keyword">open</a> <a id="19966" class="Keyword">import</a> <a id="19973" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19990" class="Keyword">open</a> <a id="19995" class="Keyword">import</a> <a id="20002" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="20030" class="Keyword">open</a> <a id="20035" class="Keyword">import</a> <a id="20042" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="20070" class="Keyword">open</a> <a id="20075" class="Keyword">import</a> <a id="20082" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="20118" class="Keyword">open</a> <a id="20123" class="Keyword">import</a> <a id="20130" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="20168" class="Keyword">open</a> <a id="20173" class="Keyword">import</a> <a id="20180" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="20213" class="Keyword">open</a> <a id="20218" class="Keyword">import</a> <a id="20225" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="20246" class="Keyword">open</a> <a id="20251" class="Keyword">import</a> <a id="20258" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="20294" class="Keyword">open</a> <a id="20299" class="Keyword">import</a> <a id="20306" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="20360" class="Keyword">open</a> <a id="20365" class="Keyword">import</a> <a id="20372" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20394" class="Keyword">open</a> <a id="20399" class="Keyword">import</a> <a id="20406" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20441" class="Keyword">open</a> <a id="20446" class="Keyword">import</a> <a id="20453" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20483" class="Keyword">open</a> <a id="20488" class="Keyword">import</a> <a id="20495" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20534" class="Keyword">open</a> <a id="20539" class="Keyword">import</a> <a id="20546" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20600" class="Keyword">open</a> <a id="20605" class="Keyword">import</a> <a id="20612" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20658" class="Keyword">open</a> <a id="20663" class="Keyword">import</a> <a id="20670" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20721" class="Keyword">open</a> <a id="20726" class="Keyword">import</a> <a id="20733" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20774" class="Keyword">open</a> <a id="20779" class="Keyword">import</a> <a id="20786" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20831" class="Keyword">open</a> <a id="20836" class="Keyword">import</a> <a id="20843" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20888" class="Keyword">open</a> <a id="20893" class="Keyword">import</a> <a id="20900" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20936" class="Keyword">open</a> <a id="20941" class="Keyword">import</a> <a id="20948" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20984" class="Keyword">open</a> <a id="20989" class="Keyword">import</a> <a id="20996" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="21061" class="Keyword">open</a> <a id="21066" class="Keyword">import</a> <a id="21073" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="21128" class="Keyword">open</a> <a id="21133" class="Keyword">import</a> <a id="21140" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="21180" class="Keyword">open</a> <a id="21185" class="Keyword">import</a> <a id="21192" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="21236" class="Keyword">open</a> <a id="21241" class="Keyword">import</a> <a id="21248" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="21293" class="Keyword">open</a> <a id="21298" class="Keyword">import</a> <a id="21305" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="21346" class="Keyword">open</a> <a id="21351" class="Keyword">import</a> <a id="21358" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21398" class="Keyword">open</a> <a id="21403" class="Keyword">import</a> <a id="21410" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21437" class="Keyword">open</a> <a id="21442" class="Keyword">import</a> <a id="21449" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21485" class="Keyword">open</a> <a id="21490" class="Keyword">import</a> <a id="21497" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21524" class="Keyword">open</a> <a id="21529" class="Keyword">import</a> <a id="21536" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21573" class="Keyword">open</a> <a id="21578" class="Keyword">import</a> <a id="21585" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21613" class="Keyword">open</a> <a id="21618" class="Keyword">import</a> <a id="21625" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21644" class="Keyword">open</a> <a id="21649" class="Keyword">import</a> <a id="21656" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21696" class="Keyword">open</a> <a id="21701" class="Keyword">import</a> <a id="21708" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="21757" class="Keyword">open</a> <a id="21762" class="Keyword">import</a> <a id="21769" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21801" class="Keyword">open</a> <a id="21806" class="Keyword">import</a> <a id="21813" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21861" class="Keyword">open</a> <a id="21866" class="Keyword">import</a> <a id="21873" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21896" class="Keyword">open</a> <a id="21901" class="Keyword">import</a> <a id="21908" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21932" class="Keyword">open</a> <a id="21937" class="Keyword">import</a> <a id="21944" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="21984" class="Keyword">open</a> <a id="21989" class="Keyword">import</a> <a id="21996" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22039" class="Keyword">open</a> <a id="22044" class="Keyword">import</a> <a id="22051" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22085" class="Keyword">open</a> <a id="22090" class="Keyword">import</a> <a id="22097" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22129" class="Keyword">open</a> <a id="22134" class="Keyword">import</a> <a id="22141" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22171" class="Keyword">open</a> <a id="22176" class="Keyword">import</a> <a id="22183" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22217" class="Keyword">open</a> <a id="22222" class="Keyword">import</a> <a id="22229" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22264" class="Keyword">open</a> <a id="22269" class="Keyword">import</a> <a id="22276" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22300" class="Keyword">open</a> <a id="22305" class="Keyword">import</a> <a id="22312" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22349" class="Keyword">open</a> <a id="22354" class="Keyword">import</a> <a id="22361" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22388" class="Keyword">open</a> <a id="22393" class="Keyword">import</a> <a id="22400" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22428" class="Keyword">open</a> <a id="22433" class="Keyword">import</a> <a id="22440" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22470" class="Keyword">open</a> <a id="22475" class="Keyword">import</a> <a id="22482" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22531" class="Keyword">open</a> <a id="22536" class="Keyword">import</a> <a id="22543" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22589" class="Keyword">open</a> <a id="22594" class="Keyword">import</a> <a id="22601" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22641" class="Keyword">open</a> <a id="22646" class="Keyword">import</a> <a id="22653" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22691" class="Keyword">open</a> <a id="22696" class="Keyword">import</a> <a id="22703" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22732" class="Keyword">open</a> <a id="22737" class="Keyword">import</a> <a id="22744" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22774" class="Keyword">open</a> <a id="22779" class="Keyword">import</a> <a id="22786" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22817" class="Keyword">open</a> <a id="22822" class="Keyword">import</a> <a id="22829" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="22869" class="Keyword">open</a> <a id="22874" class="Keyword">import</a> <a id="22881" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22907" class="Keyword">open</a> <a id="22912" class="Keyword">import</a> <a id="22919" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="22974" class="Keyword">open</a> <a id="22979" class="Keyword">import</a> <a id="22986" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23037" class="Keyword">open</a> <a id="23042" class="Keyword">import</a> <a id="23049" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23094" class="Keyword">open</a> <a id="23099" class="Keyword">import</a> <a id="23106" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23151" class="Keyword">open</a> <a id="23156" class="Keyword">import</a> <a id="23163" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23217" class="Keyword">open</a> <a id="23222" class="Keyword">import</a> <a id="23229" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23256" class="Keyword">open</a> <a id="23261" class="Keyword">import</a> <a id="23268" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23301" class="Keyword">open</a> <a id="23306" class="Keyword">import</a> <a id="23313" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23344" class="Keyword">open</a> <a id="23349" class="Keyword">import</a> <a id="23356" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23393" class="Keyword">open</a> <a id="23398" class="Keyword">import</a> <a id="23405" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23439" class="Keyword">open</a> <a id="23444" class="Keyword">import</a> <a id="23451" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23476" class="Keyword">open</a> <a id="23481" class="Keyword">import</a> <a id="23488" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23520" class="Keyword">open</a> <a id="23525" class="Keyword">import</a> <a id="23532" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23567" class="Keyword">open</a> <a id="23572" class="Keyword">import</a> <a id="23579" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23608" class="Keyword">open</a> <a id="23613" class="Keyword">import</a> <a id="23620" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23646" class="Keyword">open</a> <a id="23651" class="Keyword">import</a> <a id="23658" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23686" class="Keyword">open</a> <a id="23691" class="Keyword">import</a> <a id="23698" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23723" class="Keyword">open</a> <a id="23728" class="Keyword">import</a> <a id="23735" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23756" class="Keyword">open</a> <a id="23761" class="Keyword">import</a> <a id="23768" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23804" class="Keyword">open</a> <a id="23809" class="Keyword">import</a> <a id="23816" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="23859" class="Keyword">open</a> <a id="23864" class="Keyword">import</a> <a id="23871" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23896" class="Keyword">open</a> <a id="23901" class="Keyword">import</a> <a id="23908" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23939" class="Keyword">open</a> <a id="23944" class="Keyword">import</a> <a id="23951" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="23983" class="Keyword">open</a> <a id="23988" class="Keyword">import</a> <a id="23995" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24029" class="Keyword">open</a> <a id="24034" class="Keyword">import</a> <a id="24041" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24097" class="Keyword">open</a> <a id="24102" class="Keyword">import</a> <a id="24109" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24162" class="Keyword">open</a> <a id="24167" class="Keyword">import</a> <a id="24174" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24201" class="Keyword">open</a> <a id="24206" class="Keyword">import</a> <a id="24213" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24258" class="Keyword">open</a> <a id="24263" class="Keyword">import</a> <a id="24270" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24332" class="Keyword">open</a> <a id="24337" class="Keyword">import</a> <a id="24344" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24357" class="Keyword">open</a> <a id="24362" class="Keyword">import</a> <a id="24369" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24409" class="Keyword">open</a> <a id="24414" class="Keyword">import</a> <a id="24421" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24465" class="Keyword">open</a> <a id="24470" class="Keyword">import</a> <a id="24477" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24516" class="Keyword">open</a> <a id="24521" class="Keyword">import</a> <a id="24528" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24570" class="Keyword">open</a> <a id="24575" class="Keyword">import</a> <a id="24582" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24622" class="Keyword">open</a> <a id="24627" class="Keyword">import</a> <a id="24634" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24675" class="Keyword">open</a> <a id="24680" class="Keyword">import</a> <a id="24687" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24725" class="Keyword">open</a> <a id="24730" class="Keyword">import</a> <a id="24737" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24800" class="Keyword">open</a> <a id="24805" class="Keyword">import</a> <a id="24812" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="24841" class="Keyword">open</a> <a id="24846" class="Keyword">import</a> <a id="24853" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24898" class="Keyword">open</a> <a id="24903" class="Keyword">import</a> <a id="24910" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24952" class="Keyword">open</a> <a id="24957" class="Keyword">import</a> <a id="24964" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25004" class="Keyword">open</a> <a id="25009" class="Keyword">import</a> <a id="25016" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25060" class="Keyword">open</a> <a id="25065" class="Keyword">import</a> <a id="25072" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25121" class="Keyword">open</a> <a id="25126" class="Keyword">import</a> <a id="25133" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25183" class="Keyword">open</a> <a id="25188" class="Keyword">import</a> <a id="25195" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25222" class="Keyword">open</a> <a id="25227" class="Keyword">import</a> <a id="25234" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25259" class="Keyword">open</a> <a id="25264" class="Keyword">import</a> <a id="25271" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="25312" class="Keyword">open</a> <a id="25317" class="Keyword">import</a> <a id="25324" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25347" class="Keyword">open</a> <a id="25352" class="Keyword">import</a> <a id="25359" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25408" class="Keyword">open</a> <a id="25413" class="Keyword">import</a> <a id="25420" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25459" class="Keyword">open</a> <a id="25464" class="Keyword">import</a> <a id="25471" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25512" class="Keyword">open</a> <a id="25517" class="Keyword">import</a> <a id="25524" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25568" class="Keyword">open</a> <a id="25573" class="Keyword">import</a> <a id="25580" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25617" class="Keyword">open</a> <a id="25622" class="Keyword">import</a> <a id="25629" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="25651" class="Keyword">open</a> <a id="25656" class="Keyword">import</a> <a id="25663" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="25693" class="Keyword">open</a> <a id="25698" class="Keyword">import</a> <a id="25705" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="25744" class="Keyword">open</a> <a id="25749" class="Keyword">import</a> <a id="25756" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="25787" class="Keyword">open</a> <a id="25792" class="Keyword">import</a> <a id="25799" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="25825" class="Keyword">open</a> <a id="25830" class="Keyword">import</a> <a id="25837" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25875" class="Keyword">open</a> <a id="25880" class="Keyword">import</a> <a id="25887" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="25945" class="Keyword">open</a> <a id="25950" class="Keyword">import</a> <a id="25957" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="25995" class="Keyword">open</a> <a id="26000" class="Keyword">import</a> <a id="26007" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26026" class="Keyword">open</a> <a id="26031" class="Keyword">import</a> <a id="26038" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26103" class="Keyword">open</a> <a id="26108" class="Keyword">import</a> <a id="26115" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26146" class="Keyword">open</a> <a id="26151" class="Keyword">import</a> <a id="26158" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26185" class="Keyword">open</a> <a id="26190" class="Keyword">import</a> <a id="26197" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26225" class="Keyword">open</a> <a id="26230" class="Keyword">import</a> <a id="26237" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26304" class="Keyword">open</a> <a id="26309" class="Keyword">import</a> <a id="26316" href="group-theory.html" class="Module">group-theory</a>
<a id="26329" class="Keyword">open</a> <a id="26334" class="Keyword">import</a> <a id="26341" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26369" class="Keyword">open</a> <a id="26374" class="Keyword">import</a> <a id="26381" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26432" class="Keyword">open</a> <a id="26437" class="Keyword">import</a> <a id="26444" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="26477" class="Keyword">open</a> <a id="26482" class="Keyword">import</a> <a id="26489" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26536" class="Keyword">open</a> <a id="26541" class="Keyword">import</a> <a id="26548" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26587" class="Keyword">open</a> <a id="26592" class="Keyword">import</a> <a id="26599" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="26639" class="Keyword">open</a> <a id="26644" class="Keyword">import</a> <a id="26651" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="26694" class="Keyword">open</a> <a id="26699" class="Keyword">import</a> <a id="26706" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="26738" class="Keyword">open</a> <a id="26743" class="Keyword">import</a> <a id="26750" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="26786" class="Keyword">open</a> <a id="26791" class="Keyword">import</a> <a id="26798" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="26827" class="Keyword">open</a> <a id="26832" class="Keyword">import</a> <a id="26839" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="26867" class="Keyword">open</a> <a id="26872" class="Keyword">import</a> <a id="26879" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="26912" class="Keyword">open</a> <a id="26917" class="Keyword">import</a> <a id="26924" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="26960" class="Keyword">open</a> <a id="26965" class="Keyword">import</a> <a id="26972" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27001" class="Keyword">open</a> <a id="27006" class="Keyword">import</a> <a id="27013" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27038" class="Keyword">open</a> <a id="27043" class="Keyword">import</a> <a id="27050" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27112" class="Keyword">open</a> <a id="27117" class="Keyword">import</a> <a id="27124" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27165" class="Keyword">open</a> <a id="27170" class="Keyword">import</a> <a id="27177" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27206" class="Keyword">open</a> <a id="27211" class="Keyword">import</a> <a id="27218" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27242" class="Keyword">open</a> <a id="27247" class="Keyword">import</a> <a id="27254" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27285" class="Keyword">open</a> <a id="27290" class="Keyword">import</a> <a id="27297" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27344" class="Keyword">open</a> <a id="27349" class="Keyword">import</a> <a id="27356" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="27389" class="Keyword">open</a> <a id="27394" class="Keyword">import</a> <a id="27401" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="27450" class="Keyword">open</a> <a id="27455" class="Keyword">import</a> <a id="27462" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="27502" class="Keyword">open</a> <a id="27507" class="Keyword">import</a> <a id="27514" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="27554" class="Keyword">open</a> <a id="27559" class="Keyword">import</a> <a id="27566" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="27603" class="Keyword">open</a> <a id="27608" class="Keyword">import</a> <a id="27615" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="27662" class="Keyword">open</a> <a id="27667" class="Keyword">import</a> <a id="27674" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="27715" class="Keyword">open</a> <a id="27720" class="Keyword">import</a> <a id="27727" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="27766" class="Keyword">open</a> <a id="27771" class="Keyword">import</a> <a id="27778" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="27810" class="Keyword">open</a> <a id="27815" class="Keyword">import</a> <a id="27822" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="27849" class="Keyword">open</a> <a id="27854" class="Keyword">import</a> <a id="27861" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="27881" class="Keyword">open</a> <a id="27886" class="Keyword">import</a> <a id="27893" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="27927" class="Keyword">open</a> <a id="27932" class="Keyword">import</a> <a id="27939" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="27966" class="Keyword">open</a> <a id="27971" class="Keyword">import</a> <a id="27978" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28020" class="Keyword">open</a> <a id="28025" class="Keyword">import</a> <a id="28032" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28082" class="Keyword">open</a> <a id="28087" class="Keyword">import</a> <a id="28094" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28141" class="Keyword">open</a> <a id="28146" class="Keyword">import</a> <a id="28153" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28194" class="Keyword">open</a> <a id="28199" class="Keyword">import</a> <a id="28206" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28240" class="Keyword">open</a> <a id="28245" class="Keyword">import</a> <a id="28252" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="28300" class="Keyword">open</a> <a id="28305" class="Keyword">import</a> <a id="28312" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="28353" class="Keyword">open</a> <a id="28358" class="Keyword">import</a> <a id="28365" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="28400" class="Keyword">open</a> <a id="28405" class="Keyword">import</a> <a id="28412" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="28450" class="Keyword">open</a> <a id="28455" class="Keyword">import</a> <a id="28462" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="28497" class="Keyword">open</a> <a id="28502" class="Keyword">import</a> <a id="28509" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="28541" class="Keyword">open</a> <a id="28546" class="Keyword">import</a> <a id="28553" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="28594" class="Keyword">open</a> <a id="28599" class="Keyword">import</a> <a id="28606" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="28647" class="Keyword">open</a> <a id="28652" class="Keyword">import</a> <a id="28659" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="28699" class="Keyword">open</a> <a id="28704" class="Keyword">import</a> <a id="28711" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="28744" class="Keyword">open</a> <a id="28749" class="Keyword">import</a> <a id="28756" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="28793" class="Keyword">open</a> <a id="28798" class="Keyword">import</a> <a id="28805" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="28835" class="Keyword">open</a> <a id="28840" class="Keyword">import</a> <a id="28847" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="28868" class="Keyword">open</a> <a id="28873" class="Keyword">import</a> <a id="28880" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="28934" class="Keyword">open</a> <a id="28939" class="Keyword">import</a> <a id="28946" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="28991" class="Keyword">open</a> <a id="28996" class="Keyword">import</a> <a id="29003" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29031" class="Keyword">open</a> <a id="29036" class="Keyword">import</a> <a id="29043" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29064" class="Keyword">open</a> <a id="29069" class="Keyword">import</a> <a id="29076" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29119" class="Keyword">open</a> <a id="29124" class="Keyword">import</a> <a id="29131" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29165" class="Keyword">open</a> <a id="29170" class="Keyword">import</a> <a id="29177" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29207" class="Keyword">open</a> <a id="29212" class="Keyword">import</a> <a id="29219" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29265" class="Keyword">open</a> <a id="29270" class="Keyword">import</a> <a id="29277" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="29331" class="Keyword">open</a> <a id="29336" class="Keyword">import</a> <a id="29343" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="29386" class="Keyword">open</a> <a id="29391" class="Keyword">import</a> <a id="29398" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="29432" class="Keyword">open</a> <a id="29437" class="Keyword">import</a> <a id="29444" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="29485" class="Keyword">open</a> <a id="29490" class="Keyword">import</a> <a id="29497" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="29532" class="Keyword">open</a> <a id="29537" class="Keyword">import</a> <a id="29544" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="29586" class="Keyword">open</a> <a id="29591" class="Keyword">import</a> <a id="29598" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="29633" class="Keyword">open</a> <a id="29638" class="Keyword">import</a> <a id="29645" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="29684" class="Keyword">open</a> <a id="29689" class="Keyword">import</a> <a id="29696" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="29733" class="Keyword">open</a> <a id="29738" class="Keyword">import</a> <a id="29745" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="29792" class="Keyword">open</a> <a id="29797" class="Keyword">import</a> <a id="29804" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="29868" class="Keyword">open</a> <a id="29873" class="Keyword">import</a> <a id="29880" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="29925" class="Keyword">open</a> <a id="29930" class="Keyword">import</a> <a id="29937" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="29961" class="Keyword">open</a> <a id="29966" class="Keyword">import</a> <a id="29973" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="29998" class="Keyword">open</a> <a id="30003" class="Keyword">import</a> <a id="30010" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30053" class="Keyword">open</a> <a id="30058" class="Keyword">import</a> <a id="30065" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30096" class="Keyword">open</a> <a id="30101" class="Keyword">import</a> <a id="30108" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30162" class="Keyword">open</a> <a id="30167" class="Keyword">import</a> <a id="30174" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30197" class="Keyword">open</a> <a id="30202" class="Keyword">import</a> <a id="30209" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="30247" class="Keyword">open</a> <a id="30252" class="Keyword">import</a> <a id="30259" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="30298" class="Keyword">open</a> <a id="30303" class="Keyword">import</a> <a id="30310" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="30361" class="Keyword">open</a> <a id="30366" class="Keyword">import</a> <a id="30373" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="30410" class="Keyword">open</a> <a id="30415" class="Keyword">import</a> <a id="30422" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="30479" class="Keyword">open</a> <a id="30484" class="Keyword">import</a> <a id="30491" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="30539" class="Keyword">open</a> <a id="30544" class="Keyword">import</a> <a id="30551" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="30581" class="Keyword">open</a> <a id="30586" class="Keyword">import</a> <a id="30593" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="30630" class="Keyword">open</a> <a id="30635" class="Keyword">import</a> <a id="30642" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="30663" class="Keyword">open</a> <a id="30668" class="Keyword">import</a> <a id="30675" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="30722" class="Keyword">open</a> <a id="30727" class="Keyword">import</a> <a id="30734" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="30772" class="Keyword">open</a> <a id="30777" class="Keyword">import</a> <a id="30784" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="30878" class="Keyword">open</a> <a id="30883" class="Keyword">import</a> <a id="30890" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="30905" class="Keyword">open</a> <a id="30910" class="Keyword">import</a> <a id="30917" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="30950" class="Keyword">open</a> <a id="30955" class="Keyword">import</a> <a id="30962" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="30994" class="Keyword">open</a> <a id="30999" class="Keyword">import</a> <a id="31006" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="31048" class="Keyword">open</a> <a id="31053" class="Keyword">import</a> <a id="31060" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="31098" class="Keyword">open</a> <a id="31103" class="Keyword">import</a> <a id="31110" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="31147" class="Keyword">open</a> <a id="31152" class="Keyword">import</a> <a id="31159" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="31192" class="Keyword">open</a> <a id="31197" class="Keyword">import</a> <a id="31204" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="31228" class="Keyword">open</a> <a id="31233" class="Keyword">import</a> <a id="31240" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="31279" class="Keyword">open</a> <a id="31284" class="Keyword">import</a> <a id="31291" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="31337" class="Keyword">open</a> <a id="31342" class="Keyword">import</a> <a id="31349" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="31394" class="Keyword">open</a> <a id="31399" class="Keyword">import</a> <a id="31406" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="31444" class="Keyword">open</a> <a id="31449" class="Keyword">import</a> <a id="31456" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="31488" class="Keyword">open</a> <a id="31493" class="Keyword">import</a> <a id="31500" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="31553" class="Keyword">open</a> <a id="31558" class="Keyword">import</a> <a id="31565" href="order-theory.html" class="Module">order-theory</a>
<a id="31578" class="Keyword">open</a> <a id="31583" class="Keyword">import</a> <a id="31590" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="31617" class="Keyword">open</a> <a id="31622" class="Keyword">import</a> <a id="31629" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="31659" class="Keyword">open</a> <a id="31664" class="Keyword">import</a> <a id="31671" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="31704" class="Keyword">open</a> <a id="31709" class="Keyword">import</a> <a id="31716" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="31752" class="Keyword">open</a> <a id="31757" class="Keyword">import</a> <a id="31764" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="31799" class="Keyword">open</a> <a id="31804" class="Keyword">import</a> <a id="31811" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="31838" class="Keyword">open</a> <a id="31843" class="Keyword">import</a> <a id="31850" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="31880" class="Keyword">open</a> <a id="31885" class="Keyword">import</a> <a id="31892" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="31928" class="Keyword">open</a> <a id="31933" class="Keyword">import</a> <a id="31940" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="31982" class="Keyword">open</a> <a id="31987" class="Keyword">import</a> <a id="31994" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32024" class="Keyword">open</a> <a id="32029" class="Keyword">import</a> <a id="32036" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="32068" class="Keyword">open</a> <a id="32073" class="Keyword">import</a> <a id="32080" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="32111" class="Keyword">open</a> <a id="32116" class="Keyword">import</a> <a id="32123" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="32149" class="Keyword">open</a> <a id="32154" class="Keyword">import</a> <a id="32161" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="32190" class="Keyword">open</a> <a id="32195" class="Keyword">import</a> <a id="32202" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="32239" class="Keyword">open</a> <a id="32244" class="Keyword">import</a> <a id="32251" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="32291" class="Keyword">open</a> <a id="32296" class="Keyword">import</a> <a id="32303" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="32325" class="Keyword">open</a> <a id="32330" class="Keyword">import</a> <a id="32337" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="32372" class="Keyword">open</a> <a id="32377" class="Keyword">import</a> <a id="32384" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="32422" class="Keyword">open</a> <a id="32427" class="Keyword">import</a> <a id="32434" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="32473" class="Keyword">open</a> <a id="32478" class="Keyword">import</a> <a id="32485" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="32520" class="Keyword">open</a> <a id="32525" class="Keyword">import</a> <a id="32532" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="32567" class="Keyword">open</a> <a id="32572" class="Keyword">import</a> <a id="32579" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="32614" class="Keyword">open</a> <a id="32619" class="Keyword">import</a> <a id="32626" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="32664" class="Keyword">open</a> <a id="32669" class="Keyword">import</a> <a id="32676" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="32707" class="Keyword">open</a> <a id="32712" class="Keyword">import</a> <a id="32719" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="32761" class="Keyword">open</a> <a id="32766" class="Keyword">import</a> <a id="32773" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="32818" class="Keyword">open</a> <a id="32823" class="Keyword">import</a> <a id="32830" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="32863" class="Keyword">open</a> <a id="32868" class="Keyword">import</a> <a id="32875" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="32895" class="Keyword">open</a> <a id="32900" class="Keyword">import</a> <a id="32907" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="32930" class="Keyword">open</a> <a id="32935" class="Keyword">import</a> <a id="32942" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="32965" class="Keyword">open</a> <a id="32970" class="Keyword">import</a> <a id="32977" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33003" class="Keyword">open</a> <a id="33008" class="Keyword">import</a> <a id="33015" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33041" class="Keyword">open</a> <a id="33046" class="Keyword">import</a> <a id="33053" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="33117" class="Keyword">open</a> <a id="33122" class="Keyword">import</a> <a id="33129" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="33147" class="Keyword">open</a> <a id="33152" class="Keyword">import</a> <a id="33159" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="33186" class="Keyword">open</a> <a id="33191" class="Keyword">import</a> <a id="33198" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="33224" class="Keyword">open</a> <a id="33229" class="Keyword">import</a> <a id="33236" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="33262" class="Keyword">open</a> <a id="33267" class="Keyword">import</a> <a id="33274" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="33300" class="Keyword">open</a> <a id="33305" class="Keyword">import</a> <a id="33312" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="33343" class="Keyword">open</a> <a id="33348" class="Keyword">import</a> <a id="33355" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="33418" class="Keyword">open</a> <a id="33423" class="Keyword">import</a> <a id="33430" href="polytopes.html" class="Module">polytopes</a>
<a id="33440" class="Keyword">open</a> <a id="33445" class="Keyword">import</a> <a id="33452" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="33510" class="Keyword">open</a> <a id="33515" class="Keyword">import</a> <a id="33522" href="ring-theory.html" class="Module">ring-theory</a>
<a id="33534" class="Keyword">open</a> <a id="33539" class="Keyword">import</a> <a id="33546" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="33583" class="Keyword">open</a> <a id="33588" class="Keyword">import</a> <a id="33595" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="33622" class="Keyword">open</a> <a id="33627" class="Keyword">import</a> <a id="33634" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="33666" class="Keyword">open</a> <a id="33671" class="Keyword">import</a> <a id="33678" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="33724" class="Keyword">open</a> <a id="33729" class="Keyword">import</a> <a id="33736" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="33761" class="Keyword">open</a> <a id="33766" class="Keyword">import</a> <a id="33773" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="33811" class="Keyword">open</a> <a id="33816" class="Keyword">import</a> <a id="33823" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="33866" class="Keyword">open</a> <a id="33871" class="Keyword">import</a> <a id="33878" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="33916" class="Keyword">open</a> <a id="33921" class="Keyword">import</a> <a id="33928" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="33959" class="Keyword">open</a> <a id="33964" class="Keyword">import</a> <a id="33971" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="33995" class="Keyword">open</a> <a id="34000" class="Keyword">import</a> <a id="34007" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="34039" class="Keyword">open</a> <a id="34044" class="Keyword">import</a> <a id="34051" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="34077" class="Keyword">open</a> <a id="34082" class="Keyword">import</a> <a id="34089" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="34118" class="Keyword">open</a> <a id="34123" class="Keyword">import</a> <a id="34130" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="34167" class="Keyword">open</a> <a id="34172" class="Keyword">import</a> <a id="34179" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="34208" class="Keyword">open</a> <a id="34213" class="Keyword">import</a> <a id="34220" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="34247" class="Keyword">open</a> <a id="34252" class="Keyword">import</a> <a id="34259" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="34296" class="Keyword">open</a> <a id="34301" class="Keyword">import</a> <a id="34308" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="34335" class="Keyword">open</a> <a id="34340" class="Keyword">import</a> <a id="34347" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="34380" class="Keyword">open</a> <a id="34385" class="Keyword">import</a> <a id="34392" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="34410" class="Keyword">open</a> <a id="34415" class="Keyword">import</a> <a id="34422" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="34476" class="Keyword">open</a> <a id="34481" class="Keyword">import</a> <a id="34488" href="set-theory.html" class="Module">set-theory</a>
<a id="34499" class="Keyword">open</a> <a id="34504" class="Keyword">import</a> <a id="34511" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="34534" class="Keyword">open</a> <a id="34539" class="Keyword">import</a> <a id="34546" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="34570" class="Keyword">open</a> <a id="34575" class="Keyword">import</a> <a id="34582" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="34607" class="Keyword">open</a> <a id="34612" class="Keyword">import</a> <a id="34619" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="34645" class="Keyword">open</a> <a id="34650" class="Keyword">import</a> <a id="34657" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="34719" class="Keyword">open</a> <a id="34724" class="Keyword">import</a> <a id="34731" href="structured-types.html" class="Module">structured-types</a>
<a id="34748" class="Keyword">open</a> <a id="34753" class="Keyword">import</a> <a id="34760" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="34795" class="Keyword">open</a> <a id="34800" class="Keyword">import</a> <a id="34807" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="34851" class="Keyword">open</a> <a id="34856" class="Keyword">import</a> <a id="34863" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="34927" class="Keyword">open</a> <a id="34932" class="Keyword">import</a> <a id="34939" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="34978" class="Keyword">open</a> <a id="34983" class="Keyword">import</a> <a id="34990" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="35036" class="Keyword">open</a> <a id="35041" class="Keyword">import</a> <a id="35048" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="35072" class="Keyword">open</a> <a id="35077" class="Keyword">import</a> <a id="35084" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="35153" class="Keyword">open</a> <a id="35158" class="Keyword">import</a> <a id="35165" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="35210" class="Keyword">open</a> <a id="35215" class="Keyword">import</a> <a id="35222" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="35256" class="Keyword">open</a> <a id="35261" class="Keyword">import</a> <a id="35268" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="35329" class="Keyword">open</a> <a id="35334" class="Keyword">import</a> <a id="35341" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="35386" class="Keyword">open</a> <a id="35391" class="Keyword">import</a> <a id="35398" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="35436" class="Keyword">open</a> <a id="35441" class="Keyword">import</a> <a id="35448" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="35491" class="Keyword">open</a> <a id="35496" class="Keyword">import</a> <a id="35503" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="35539" class="Keyword">open</a> <a id="35544" class="Keyword">import</a> <a id="35551" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="35581" class="Keyword">open</a> <a id="35586" class="Keyword">import</a> <a id="35593" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="35627" class="Keyword">open</a> <a id="35632" class="Keyword">import</a> <a id="35639" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="35670" class="Keyword">open</a> <a id="35675" class="Keyword">import</a> <a id="35682" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="35741" class="Keyword">open</a> <a id="35746" class="Keyword">import</a> <a id="35753" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="35804" class="Keyword">open</a> <a id="35809" class="Keyword">import</a> <a id="35816" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="35867" class="Keyword">open</a> <a id="35872" class="Keyword">import</a> <a id="35879" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="35934" class="Keyword">open</a> <a id="35939" class="Keyword">import</a> <a id="35946" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="35978" class="Keyword">open</a> <a id="35983" class="Keyword">import</a> <a id="35990" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="36019" class="Keyword">open</a> <a id="36024" class="Keyword">import</a> <a id="36031" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="36059" class="Keyword">open</a> <a id="36064" class="Keyword">import</a> <a id="36071" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="36101" class="Keyword">open</a> <a id="36106" class="Keyword">import</a> <a id="36113" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="36147" class="Keyword">open</a> <a id="36152" class="Keyword">import</a> <a id="36159" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="36235" class="Keyword">open</a> <a id="36240" class="Keyword">import</a> <a id="36247" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="36273" class="Keyword">open</a> <a id="36278" class="Keyword">import</a> <a id="36285" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="36323" class="Keyword">open</a> <a id="36328" class="Keyword">import</a> <a id="36335" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="36372" class="Keyword">open</a> <a id="36377" class="Keyword">import</a> <a id="36384" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="36424" class="Keyword">open</a> <a id="36429" class="Keyword">import</a> <a id="36436" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="36475" class="Keyword">open</a> <a id="36480" class="Keyword">import</a> <a id="36487" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="36520" class="Keyword">open</a> <a id="36525" class="Keyword">import</a> <a id="36532" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="36575" class="Keyword">open</a> <a id="36580" class="Keyword">import</a> <a id="36587" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="36622" class="Keyword">open</a> <a id="36627" class="Keyword">import</a> <a id="36634" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="36679" class="Keyword">open</a> <a id="36684" class="Keyword">import</a> <a id="36691" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="36728" class="Keyword">open</a> <a id="36733" class="Keyword">import</a> <a id="36740" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="36792" class="Keyword">open</a> <a id="36797" class="Keyword">import</a> <a id="36804" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="36857" class="Keyword">open</a> <a id="36862" class="Keyword">import</a> <a id="36869" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="36929" class="Keyword">open</a> <a id="36934" class="Keyword">import</a> <a id="36941" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="36989" class="Keyword">open</a> <a id="36994" class="Keyword">import</a> <a id="37001" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="37041" class="Keyword">open</a> <a id="37046" class="Keyword">import</a> <a id="37053" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="37100" class="Keyword">open</a> <a id="37105" class="Keyword">import</a> <a id="37112" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="37153" class="Keyword">open</a> <a id="37158" class="Keyword">import</a> <a id="37165" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="37203" class="Keyword">open</a> <a id="37208" class="Keyword">import</a> <a id="37215" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="37263" class="Keyword">open</a> <a id="37268" class="Keyword">import</a> <a id="37275" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="37312" class="Keyword">open</a> <a id="37317" class="Keyword">import</a> <a id="37324" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="37359" class="Keyword">open</a> <a id="37364" class="Keyword">import</a> <a id="37371" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="37405" class="Keyword">open</a> <a id="37410" class="Keyword">import</a> <a id="37417" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="37464" class="Keyword">open</a> <a id="37469" class="Keyword">import</a> <a id="37476" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="37521" class="Keyword">open</a> <a id="37526" class="Keyword">import</a> <a id="37533" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="37582" class="Keyword">open</a> <a id="37587" class="Keyword">import</a> <a id="37594" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="37646" class="Keyword">open</a> <a id="37651" class="Keyword">import</a> <a id="37658" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="37712" class="Keyword">open</a> <a id="37717" class="Keyword">import</a> <a id="37724" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="37801" class="Keyword">open</a> <a id="37806" class="Keyword">import</a> <a id="37813" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="37865" class="Keyword">open</a> <a id="37870" class="Keyword">import</a> <a id="37877" href="type-theories.html" class="Module">type-theories</a>
<a id="37891" class="Keyword">open</a> <a id="37896" class="Keyword">import</a> <a id="37903" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="37945" class="Keyword">open</a> <a id="37950" class="Keyword">import</a> <a id="37957" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="37995" class="Keyword">open</a> <a id="38000" class="Keyword">import</a> <a id="38007" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="38053" class="Keyword">open</a> <a id="38058" class="Keyword">import</a> <a id="38065" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="38112" class="Keyword">open</a> <a id="38117" class="Keyword">import</a> <a id="38124" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="38159" class="Keyword">open</a> <a id="38164" class="Keyword">import</a> <a id="38171" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="38249" class="Keyword">open</a> <a id="38254" class="Keyword">import</a> <a id="38261" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="38285" class="Keyword">open</a> <a id="38290" class="Keyword">import</a> <a id="38297" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="38350" class="Keyword">open</a> <a id="38355" class="Keyword">import</a> <a id="38362" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="38405" class="Keyword">open</a> <a id="38410" class="Keyword">import</a> <a id="38417" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="38457" class="Keyword">open</a> <a id="38462" class="Keyword">import</a> <a id="38469" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="38508" class="Keyword">open</a> <a id="38513" class="Keyword">import</a> <a id="38520" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="38554" class="Keyword">open</a> <a id="38559" class="Keyword">import</a> <a id="38566" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="38614" class="Keyword">open</a> <a id="38619" class="Keyword">import</a> <a id="38626" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="38677" class="Keyword">open</a> <a id="38682" class="Keyword">import</a> <a id="38689" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="38736" class="Keyword">open</a> <a id="38741" class="Keyword">import</a> <a id="38748" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="38800" class="Keyword">open</a> <a id="38805" class="Keyword">import</a> <a id="38812" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="38856" class="Keyword">open</a> <a id="38861" class="Keyword">import</a> <a id="38868" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="38908" class="Keyword">open</a> <a id="38913" class="Keyword">import</a> <a id="38920" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="38963" class="Keyword">open</a> <a id="38968" class="Keyword">import</a> <a id="38975" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="39027" class="Keyword">open</a> <a id="39032" class="Keyword">import</a> <a id="39039" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="39093" class="Keyword">open</a> <a id="39098" class="Keyword">import</a> <a id="39105" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="39153" class="Keyword">open</a> <a id="39158" class="Keyword">import</a> <a id="39165" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="39204" class="Keyword">open</a> <a id="39209" class="Keyword">import</a> <a id="39216" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="39249" class="Keyword">open</a> <a id="39254" class="Keyword">import</a> <a id="39261" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="39291" class="Keyword">open</a> <a id="39296" class="Keyword">import</a> <a id="39303" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="39354" class="Keyword">open</a> <a id="39359" class="Keyword">import</a> <a id="39366" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="39407" class="Keyword">open</a> <a id="39412" class="Keyword">import</a> <a id="39419" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="39456" class="Keyword">open</a> <a id="39461" class="Keyword">import</a> <a id="39468" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="39527" class="Keyword">open</a> <a id="39532" class="Keyword">import</a> <a id="39539" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="39594" class="Keyword">open</a> <a id="39599" class="Keyword">import</a> <a id="39606" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="39662" class="Keyword">open</a> <a id="39667" class="Keyword">import</a> <a id="39674" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="39721" class="Keyword">open</a> <a id="39726" class="Keyword">import</a> <a id="39733" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="39776" class="Keyword">open</a> <a id="39781" class="Keyword">import</a> <a id="39788" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="39833" class="Keyword">open</a> <a id="39838" class="Keyword">import</a> <a id="39845" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="39894" class="Keyword">open</a> <a id="39899" class="Keyword">import</a> <a id="39906" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="39957" class="Keyword">open</a> <a id="39962" class="Keyword">import</a> <a id="39969" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="40013" class="Keyword">open</a> <a id="40018" class="Keyword">import</a> <a id="40025" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="40103" class="Keyword">open</a> <a id="40108" class="Keyword">import</a> <a id="40115" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="40155" class="Keyword">open</a> <a id="40160" class="Keyword">import</a> <a id="40167" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="40224" class="Keyword">open</a> <a id="40229" class="Keyword">import</a> <a id="40236" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="40271" class="Keyword">open</a> <a id="40276" class="Keyword">import</a> <a id="40283" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="40329" class="Keyword">open</a> <a id="40334" class="Keyword">import</a> <a id="40341" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="40396" class="Keyword">open</a> <a id="40401" class="Keyword">import</a> <a id="40408" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="40451" class="Keyword">open</a> <a id="40456" class="Keyword">import</a> <a id="40463" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="40508" class="Keyword">open</a> <a id="40513" class="Keyword">import</a> <a id="40520" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="40579" class="Keyword">open</a> <a id="40584" class="Keyword">import</a> <a id="40591" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="40628" class="Keyword">open</a> <a id="40633" class="Keyword">import</a> <a id="40640" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="40682" class="Keyword">open</a> <a id="40687" class="Keyword">import</a> <a id="40694" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="40735" class="Keyword">open</a> <a id="40740" class="Keyword">import</a> <a id="40747" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="40786" class="Keyword">open</a> <a id="40791" class="Keyword">import</a> <a id="40798" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="40836" class="Keyword">open</a> <a id="40841" class="Keyword">import</a> <a id="40848" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="40900" class="Keyword">open</a> <a id="40905" class="Keyword">import</a> <a id="40912" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="40957" class="Keyword">open</a> <a id="40962" class="Keyword">import</a> <a id="40969" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="41008" class="Keyword">open</a> <a id="41013" class="Keyword">import</a> <a id="41020" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="41057" class="Keyword">open</a> <a id="41062" class="Keyword">import</a> <a id="41069" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="41118" class="Keyword">open</a> <a id="41123" class="Keyword">import</a> <a id="41130" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="41169" class="Keyword">open</a> <a id="41174" class="Keyword">import</a> <a id="41181" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="41219" class="Keyword">open</a> <a id="41224" class="Keyword">import</a> <a id="41231" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="41286" class="Keyword">open</a> <a id="41291" class="Keyword">import</a> <a id="41298" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="41337" class="Keyword">open</a> <a id="41342" class="Keyword">import</a> <a id="41349" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="41397" class="Keyword">open</a> <a id="41402" class="Keyword">import</a> <a id="41409" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="41456" class="Keyword">open</a> <a id="41461" class="Keyword">import</a> <a id="41468" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="41506" class="Keyword">open</a> <a id="41511" class="Keyword">import</a> <a id="41518" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="41548" class="Keyword">open</a> <a id="41553" class="Keyword">import</a> <a id="41560" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="41617" class="Keyword">open</a> <a id="41622" class="Keyword">import</a> <a id="41629" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="41683" class="Keyword">open</a> <a id="41688" class="Keyword">import</a> <a id="41695" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="41725" class="Keyword">open</a> <a id="41730" class="Keyword">import</a> <a id="41737" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="41786" class="Keyword">open</a> <a id="41791" class="Keyword">import</a> <a id="41798" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="41840" class="Keyword">open</a> <a id="41845" class="Keyword">import</a> <a id="41852" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="41886" class="Keyword">open</a> <a id="41891" class="Keyword">import</a> <a id="41898" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="41961" class="Keyword">open</a> <a id="41966" class="Keyword">import</a> <a id="41973" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="42016" class="Keyword">open</a> <a id="42021" class="Keyword">import</a> <a id="42028" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="42063" class="Keyword">open</a> <a id="42068" class="Keyword">import</a> <a id="42075" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="42110" class="Keyword">open</a> <a id="42115" class="Keyword">import</a> <a id="42122" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="42162" class="Keyword">open</a> <a id="42167" class="Keyword">import</a> <a id="42174" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="42219" class="Keyword">open</a> <a id="42224" class="Keyword">import</a> <a id="42231" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="42272" class="Keyword">open</a> <a id="42277" class="Keyword">import</a> <a id="42284" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="42338" class="Keyword">open</a> <a id="42343" class="Keyword">import</a> <a id="42350" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="42400" class="Keyword">open</a> <a id="42405" class="Keyword">import</a> <a id="42412" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="42459" class="Keyword">open</a> <a id="42464" class="Keyword">import</a> <a id="42471" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="42509" class="Keyword">open</a> <a id="42514" class="Keyword">import</a> <a id="42521" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="42570" class="Keyword">open</a> <a id="42575" class="Keyword">import</a> <a id="42582" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="42629" class="Keyword">open</a> <a id="42634" class="Keyword">import</a> <a id="42641" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="42704" class="Keyword">open</a> <a id="42709" class="Keyword">import</a> <a id="42716" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="42748" class="Keyword">open</a> <a id="42753" class="Keyword">import</a> <a id="42760" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="42813" class="Keyword">open</a> <a id="42818" class="Keyword">import</a> <a id="42825" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="42871" class="Keyword">open</a> <a id="42876" class="Keyword">import</a> <a id="42883" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="42929" class="Keyword">open</a> <a id="42934" class="Keyword">import</a> <a id="42941" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="42981" class="Keyword">open</a> <a id="42986" class="Keyword">import</a> <a id="42993" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="43040" class="Keyword">open</a> <a id="43045" class="Keyword">import</a> <a id="43052" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="43100" class="Keyword">open</a> <a id="43105" class="Keyword">import</a> <a id="43112" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="43152" class="Keyword">open</a> <a id="43157" class="Keyword">import</a> <a id="43164" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="43209" class="Keyword">open</a> <a id="43214" class="Keyword">import</a> <a id="43221" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="43286" class="Keyword">open</a> <a id="43291" class="Keyword">import</a> <a id="43298" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="43343" class="Keyword">open</a> <a id="43348" class="Keyword">import</a> <a id="43355" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="43402" class="Keyword">open</a> <a id="43407" class="Keyword">import</a> <a id="43414" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="43467" class="Keyword">open</a> <a id="43472" class="Keyword">import</a> <a id="43479" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>