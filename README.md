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
<a id="17445" class="Keyword">open</a> <a id="17450" class="Keyword">import</a> <a id="17457" href="foundation.noncontractible-types.html" class="Module">foundation.noncontractible-types</a>
<a id="17490" class="Keyword">open</a> <a id="17495" class="Keyword">import</a> <a id="17502" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17540" class="Keyword">open</a> <a id="17545" class="Keyword">import</a> <a id="17552" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17580" class="Keyword">open</a> <a id="17585" class="Keyword">import</a> <a id="17592" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17616" class="Keyword">open</a> <a id="17621" class="Keyword">import</a> <a id="17628" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17655" class="Keyword">open</a> <a id="17660" class="Keyword">import</a> <a id="17667" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17702" class="Keyword">open</a> <a id="17707" class="Keyword">import</a> <a id="17714" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17735" class="Keyword">open</a> <a id="17740" class="Keyword">import</a> <a id="17747" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17783" class="Keyword">open</a> <a id="17788" class="Keyword">import</a> <a id="17795" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17840" class="Keyword">open</a> <a id="17845" class="Keyword">import</a> <a id="17852" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="17898" class="Keyword">open</a> <a id="17903" class="Keyword">import</a> <a id="17910" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="17950" class="Keyword">open</a> <a id="17955" class="Keyword">import</a> <a id="17962" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="17992" class="Keyword">open</a> <a id="17997" class="Keyword">import</a> <a id="18004" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="18038" class="Keyword">open</a> <a id="18043" class="Keyword">import</a> <a id="18050" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="18087" class="Keyword">open</a> <a id="18092" class="Keyword">import</a> <a id="18099" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="18123" class="Keyword">open</a> <a id="18128" class="Keyword">import</a> <a id="18135" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="18156" class="Keyword">open</a> <a id="18161" class="Keyword">import</a> <a id="18168" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="18203" class="Keyword">open</a> <a id="18208" class="Keyword">import</a> <a id="18215" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="18252" class="Keyword">open</a> <a id="18257" class="Keyword">import</a> <a id="18264" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="18313" class="Keyword">open</a> <a id="18318" class="Keyword">import</a> <a id="18325" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="18358" class="Keyword">open</a> <a id="18363" class="Keyword">import</a> <a id="18370" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="18393" class="Keyword">open</a> <a id="18398" class="Keyword">import</a> <a id="18405" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="18428" class="Keyword">open</a> <a id="18433" class="Keyword">import</a> <a id="18440" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18463" class="Keyword">open</a> <a id="18468" class="Keyword">import</a> <a id="18475" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18503" class="Keyword">open</a> <a id="18508" class="Keyword">import</a> <a id="18515" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18535" class="Keyword">open</a> <a id="18540" class="Keyword">import</a> <a id="18547" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18568" class="Keyword">open</a> <a id="18573" class="Keyword">import</a> <a id="18580" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18611" class="Keyword">open</a> <a id="18616" class="Keyword">import</a> <a id="18623" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18650" class="Keyword">open</a> <a id="18655" class="Keyword">import</a> <a id="18662" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18678" class="Keyword">open</a> <a id="18683" class="Keyword">import</a> <a id="18690" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18721" class="Keyword">open</a> <a id="18726" class="Keyword">import</a> <a id="18733" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18750" class="Keyword">open</a> <a id="18755" class="Keyword">import</a> <a id="18762" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18784" class="Keyword">open</a> <a id="18789" class="Keyword">import</a> <a id="18796" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18823" class="Keyword">open</a> <a id="18828" class="Keyword">import</a> <a id="18835" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18858" class="Keyword">open</a> <a id="18863" class="Keyword">import</a> <a id="18870" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="18897" class="Keyword">open</a> <a id="18902" class="Keyword">import</a> <a id="18909" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="18942" class="Keyword">open</a> <a id="18947" class="Keyword">import</a> <a id="18954" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="18994" class="Keyword">open</a> <a id="18999" class="Keyword">import</a> <a id="19006" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="19027" class="Keyword">open</a> <a id="19032" class="Keyword">import</a> <a id="19039" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="19068" class="Keyword">open</a> <a id="19073" class="Keyword">import</a> <a id="19080" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="19118" class="Keyword">open</a> <a id="19123" class="Keyword">import</a> <a id="19130" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="19150" class="Keyword">open</a> <a id="19155" class="Keyword">import</a> <a id="19162" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="19186" class="Keyword">open</a> <a id="19191" class="Keyword">import</a> <a id="19198" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="19225" class="Keyword">open</a> <a id="19230" class="Keyword">import</a> <a id="19237" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="19269" class="Keyword">open</a> <a id="19274" class="Keyword">import</a> <a id="19281" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="19311" class="Keyword">open</a> <a id="19316" class="Keyword">import</a> <a id="19323" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19349" class="Keyword">open</a> <a id="19354" class="Keyword">import</a> <a id="19361" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19388" class="Keyword">open</a> <a id="19393" class="Keyword">import</a> <a id="19400" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19437" class="Keyword">open</a> <a id="19442" class="Keyword">import</a> <a id="19449" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19478" class="Keyword">open</a> <a id="19483" class="Keyword">import</a> <a id="19490" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19513" class="Keyword">open</a> <a id="19518" class="Keyword">import</a> <a id="19525" href="foundation.type-arithmetic-booleans.html" class="Module">foundation.type-arithmetic-booleans</a>
<a id="19561" class="Keyword">open</a> <a id="19566" class="Keyword">import</a> <a id="19573" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19624" class="Keyword">open</a> <a id="19629" class="Keyword">import</a> <a id="19636" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19679" class="Keyword">open</a> <a id="19684" class="Keyword">import</a> <a id="19691" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19743" class="Keyword">open</a> <a id="19748" class="Keyword">import</a> <a id="19755" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19803" class="Keyword">open</a> <a id="19808" class="Keyword">import</a> <a id="19815" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19853" class="Keyword">open</a> <a id="19858" class="Keyword">import</a> <a id="19865" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="19902" class="Keyword">open</a> <a id="19907" class="Keyword">import</a> <a id="19914" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="19960" class="Keyword">open</a> <a id="19965" class="Keyword">import</a> <a id="19972" href="foundation.union.html" class="Module">foundation.union</a>
<a id="19989" class="Keyword">open</a> <a id="19994" class="Keyword">import</a> <a id="20001" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="20029" class="Keyword">open</a> <a id="20034" class="Keyword">import</a> <a id="20041" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="20069" class="Keyword">open</a> <a id="20074" class="Keyword">import</a> <a id="20081" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="20117" class="Keyword">open</a> <a id="20122" class="Keyword">import</a> <a id="20129" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="20167" class="Keyword">open</a> <a id="20172" class="Keyword">import</a> <a id="20179" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="20212" class="Keyword">open</a> <a id="20217" class="Keyword">import</a> <a id="20224" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="20245" class="Keyword">open</a> <a id="20250" class="Keyword">import</a> <a id="20257" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="20293" class="Keyword">open</a> <a id="20298" class="Keyword">import</a> <a id="20305" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="20359" class="Keyword">open</a> <a id="20364" class="Keyword">import</a> <a id="20371" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20393" class="Keyword">open</a> <a id="20398" class="Keyword">import</a> <a id="20405" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20440" class="Keyword">open</a> <a id="20445" class="Keyword">import</a> <a id="20452" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20482" class="Keyword">open</a> <a id="20487" class="Keyword">import</a> <a id="20494" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20533" class="Keyword">open</a> <a id="20538" class="Keyword">import</a> <a id="20545" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20599" class="Keyword">open</a> <a id="20604" class="Keyword">import</a> <a id="20611" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20657" class="Keyword">open</a> <a id="20662" class="Keyword">import</a> <a id="20669" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20720" class="Keyword">open</a> <a id="20725" class="Keyword">import</a> <a id="20732" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20773" class="Keyword">open</a> <a id="20778" class="Keyword">import</a> <a id="20785" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20830" class="Keyword">open</a> <a id="20835" class="Keyword">import</a> <a id="20842" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="20887" class="Keyword">open</a> <a id="20892" class="Keyword">import</a> <a id="20899" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="20935" class="Keyword">open</a> <a id="20940" class="Keyword">import</a> <a id="20947" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="20983" class="Keyword">open</a> <a id="20988" class="Keyword">import</a> <a id="20995" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="21060" class="Keyword">open</a> <a id="21065" class="Keyword">import</a> <a id="21072" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="21127" class="Keyword">open</a> <a id="21132" class="Keyword">import</a> <a id="21139" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="21179" class="Keyword">open</a> <a id="21184" class="Keyword">import</a> <a id="21191" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="21235" class="Keyword">open</a> <a id="21240" class="Keyword">import</a> <a id="21247" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="21292" class="Keyword">open</a> <a id="21297" class="Keyword">import</a> <a id="21304" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="21345" class="Keyword">open</a> <a id="21350" class="Keyword">import</a> <a id="21357" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21397" class="Keyword">open</a> <a id="21402" class="Keyword">import</a> <a id="21409" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21436" class="Keyword">open</a> <a id="21441" class="Keyword">import</a> <a id="21448" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21484" class="Keyword">open</a> <a id="21489" class="Keyword">import</a> <a id="21496" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21523" class="Keyword">open</a> <a id="21528" class="Keyword">import</a> <a id="21535" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21572" class="Keyword">open</a> <a id="21577" class="Keyword">import</a> <a id="21584" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21612" class="Keyword">open</a> <a id="21617" class="Keyword">import</a> <a id="21624" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21643" class="Keyword">open</a> <a id="21648" class="Keyword">import</a> <a id="21655" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21695" class="Keyword">open</a> <a id="21700" class="Keyword">import</a> <a id="21707" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="21756" class="Keyword">open</a> <a id="21761" class="Keyword">import</a> <a id="21768" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21800" class="Keyword">open</a> <a id="21805" class="Keyword">import</a> <a id="21812" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21860" class="Keyword">open</a> <a id="21865" class="Keyword">import</a> <a id="21872" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="21895" class="Keyword">open</a> <a id="21900" class="Keyword">import</a> <a id="21907" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="21931" class="Keyword">open</a> <a id="21936" class="Keyword">import</a> <a id="21943" href="foundation-core.automorphisms.html" class="Module">foundation-core.automorphisms</a>
<a id="21973" class="Keyword">open</a> <a id="21978" class="Keyword">import</a> <a id="21985" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="22025" class="Keyword">open</a> <a id="22030" class="Keyword">import</a> <a id="22037" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22080" class="Keyword">open</a> <a id="22085" class="Keyword">import</a> <a id="22092" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22126" class="Keyword">open</a> <a id="22131" class="Keyword">import</a> <a id="22138" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22170" class="Keyword">open</a> <a id="22175" class="Keyword">import</a> <a id="22182" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22212" class="Keyword">open</a> <a id="22217" class="Keyword">import</a> <a id="22224" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22258" class="Keyword">open</a> <a id="22263" class="Keyword">import</a> <a id="22270" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22305" class="Keyword">open</a> <a id="22310" class="Keyword">import</a> <a id="22317" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22341" class="Keyword">open</a> <a id="22346" class="Keyword">import</a> <a id="22353" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22390" class="Keyword">open</a> <a id="22395" class="Keyword">import</a> <a id="22402" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22429" class="Keyword">open</a> <a id="22434" class="Keyword">import</a> <a id="22441" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22469" class="Keyword">open</a> <a id="22474" class="Keyword">import</a> <a id="22481" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22511" class="Keyword">open</a> <a id="22516" class="Keyword">import</a> <a id="22523" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22572" class="Keyword">open</a> <a id="22577" class="Keyword">import</a> <a id="22584" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22630" class="Keyword">open</a> <a id="22635" class="Keyword">import</a> <a id="22642" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22682" class="Keyword">open</a> <a id="22687" class="Keyword">import</a> <a id="22694" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22732" class="Keyword">open</a> <a id="22737" class="Keyword">import</a> <a id="22744" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22773" class="Keyword">open</a> <a id="22778" class="Keyword">import</a> <a id="22785" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22815" class="Keyword">open</a> <a id="22820" class="Keyword">import</a> <a id="22827" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22858" class="Keyword">open</a> <a id="22863" class="Keyword">import</a> <a id="22870" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="22910" class="Keyword">open</a> <a id="22915" class="Keyword">import</a> <a id="22922" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22948" class="Keyword">open</a> <a id="22953" class="Keyword">import</a> <a id="22960" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="23015" class="Keyword">open</a> <a id="23020" class="Keyword">import</a> <a id="23027" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23078" class="Keyword">open</a> <a id="23083" class="Keyword">import</a> <a id="23090" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23135" class="Keyword">open</a> <a id="23140" class="Keyword">import</a> <a id="23147" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23192" class="Keyword">open</a> <a id="23197" class="Keyword">import</a> <a id="23204" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23258" class="Keyword">open</a> <a id="23263" class="Keyword">import</a> <a id="23270" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23297" class="Keyword">open</a> <a id="23302" class="Keyword">import</a> <a id="23309" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23342" class="Keyword">open</a> <a id="23347" class="Keyword">import</a> <a id="23354" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23385" class="Keyword">open</a> <a id="23390" class="Keyword">import</a> <a id="23397" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23434" class="Keyword">open</a> <a id="23439" class="Keyword">import</a> <a id="23446" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23480" class="Keyword">open</a> <a id="23485" class="Keyword">import</a> <a id="23492" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23517" class="Keyword">open</a> <a id="23522" class="Keyword">import</a> <a id="23529" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23561" class="Keyword">open</a> <a id="23566" class="Keyword">import</a> <a id="23573" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23608" class="Keyword">open</a> <a id="23613" class="Keyword">import</a> <a id="23620" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23649" class="Keyword">open</a> <a id="23654" class="Keyword">import</a> <a id="23661" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23687" class="Keyword">open</a> <a id="23692" class="Keyword">import</a> <a id="23699" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23727" class="Keyword">open</a> <a id="23732" class="Keyword">import</a> <a id="23739" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23764" class="Keyword">open</a> <a id="23769" class="Keyword">import</a> <a id="23776" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23797" class="Keyword">open</a> <a id="23802" class="Keyword">import</a> <a id="23809" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23845" class="Keyword">open</a> <a id="23850" class="Keyword">import</a> <a id="23857" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="23900" class="Keyword">open</a> <a id="23905" class="Keyword">import</a> <a id="23912" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23937" class="Keyword">open</a> <a id="23942" class="Keyword">import</a> <a id="23949" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23980" class="Keyword">open</a> <a id="23985" class="Keyword">import</a> <a id="23992" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="24024" class="Keyword">open</a> <a id="24029" class="Keyword">import</a> <a id="24036" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24070" class="Keyword">open</a> <a id="24075" class="Keyword">import</a> <a id="24082" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24138" class="Keyword">open</a> <a id="24143" class="Keyword">import</a> <a id="24150" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24203" class="Keyword">open</a> <a id="24208" class="Keyword">import</a> <a id="24215" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24242" class="Keyword">open</a> <a id="24247" class="Keyword">import</a> <a id="24254" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24299" class="Keyword">open</a> <a id="24304" class="Keyword">import</a> <a id="24311" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24373" class="Keyword">open</a> <a id="24378" class="Keyword">import</a> <a id="24385" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24398" class="Keyword">open</a> <a id="24403" class="Keyword">import</a> <a id="24410" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24450" class="Keyword">open</a> <a id="24455" class="Keyword">import</a> <a id="24462" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24506" class="Keyword">open</a> <a id="24511" class="Keyword">import</a> <a id="24518" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24557" class="Keyword">open</a> <a id="24562" class="Keyword">import</a> <a id="24569" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24611" class="Keyword">open</a> <a id="24616" class="Keyword">import</a> <a id="24623" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24663" class="Keyword">open</a> <a id="24668" class="Keyword">import</a> <a id="24675" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24716" class="Keyword">open</a> <a id="24721" class="Keyword">import</a> <a id="24728" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24766" class="Keyword">open</a> <a id="24771" class="Keyword">import</a> <a id="24778" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24841" class="Keyword">open</a> <a id="24846" class="Keyword">import</a> <a id="24853" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="24882" class="Keyword">open</a> <a id="24887" class="Keyword">import</a> <a id="24894" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24939" class="Keyword">open</a> <a id="24944" class="Keyword">import</a> <a id="24951" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24993" class="Keyword">open</a> <a id="24998" class="Keyword">import</a> <a id="25005" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25045" class="Keyword">open</a> <a id="25050" class="Keyword">import</a> <a id="25057" href="graph-theory.equivalences-enriched-undirected-graphs.html" class="Module">graph-theory.equivalences-enriched-undirected-graphs</a>
<a id="25110" class="Keyword">open</a> <a id="25115" class="Keyword">import</a> <a id="25122" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25166" class="Keyword">open</a> <a id="25171" class="Keyword">import</a> <a id="25178" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25227" class="Keyword">open</a> <a id="25232" class="Keyword">import</a> <a id="25239" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25289" class="Keyword">open</a> <a id="25294" class="Keyword">import</a> <a id="25301" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25328" class="Keyword">open</a> <a id="25333" class="Keyword">import</a> <a id="25340" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25365" class="Keyword">open</a> <a id="25370" class="Keyword">import</a> <a id="25377" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25400" class="Keyword">open</a> <a id="25405" class="Keyword">import</a> <a id="25412" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25461" class="Keyword">open</a> <a id="25466" class="Keyword">import</a> <a id="25473" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25512" class="Keyword">open</a> <a id="25517" class="Keyword">import</a> <a id="25524" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25565" class="Keyword">open</a> <a id="25570" class="Keyword">import</a> <a id="25577" href="graph-theory.neighbors-undirected-graphs.html" class="Module">graph-theory.neighbors-undirected-graphs</a>
<a id="25618" class="Keyword">open</a> <a id="25623" class="Keyword">import</a> <a id="25630" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25674" class="Keyword">open</a> <a id="25679" class="Keyword">import</a> <a id="25686" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25723" class="Keyword">open</a> <a id="25728" class="Keyword">import</a> <a id="25735" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="25757" class="Keyword">open</a> <a id="25762" class="Keyword">import</a> <a id="25769" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="25799" class="Keyword">open</a> <a id="25804" class="Keyword">import</a> <a id="25811" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="25850" class="Keyword">open</a> <a id="25855" class="Keyword">import</a> <a id="25862" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="25893" class="Keyword">open</a> <a id="25898" class="Keyword">import</a> <a id="25905" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="25931" class="Keyword">open</a> <a id="25936" class="Keyword">import</a> <a id="25943" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25981" class="Keyword">open</a> <a id="25986" class="Keyword">import</a> <a id="25993" href="graph-theory.stereoisomerism-enriched-undirected-graphs.html" class="Module">graph-theory.stereoisomerism-enriched-undirected-graphs</a>
<a id="26049" class="Keyword">open</a> <a id="26054" class="Keyword">import</a> <a id="26061" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="26119" class="Keyword">open</a> <a id="26124" class="Keyword">import</a> <a id="26131" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="26169" class="Keyword">open</a> <a id="26174" class="Keyword">import</a> <a id="26181" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26200" class="Keyword">open</a> <a id="26205" class="Keyword">import</a> <a id="26212" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26277" class="Keyword">open</a> <a id="26282" class="Keyword">import</a> <a id="26289" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26320" class="Keyword">open</a> <a id="26325" class="Keyword">import</a> <a id="26332" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26359" class="Keyword">open</a> <a id="26364" class="Keyword">import</a> <a id="26371" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26399" class="Keyword">open</a> <a id="26404" class="Keyword">import</a> <a id="26411" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26478" class="Keyword">open</a> <a id="26483" class="Keyword">import</a> <a id="26490" href="group-theory.html" class="Module">group-theory</a>
<a id="26503" class="Keyword">open</a> <a id="26508" class="Keyword">import</a> <a id="26515" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26543" class="Keyword">open</a> <a id="26548" class="Keyword">import</a> <a id="26555" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26606" class="Keyword">open</a> <a id="26611" class="Keyword">import</a> <a id="26618" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="26651" class="Keyword">open</a> <a id="26656" class="Keyword">import</a> <a id="26663" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26710" class="Keyword">open</a> <a id="26715" class="Keyword">import</a> <a id="26722" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26761" class="Keyword">open</a> <a id="26766" class="Keyword">import</a> <a id="26773" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="26813" class="Keyword">open</a> <a id="26818" class="Keyword">import</a> <a id="26825" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="26868" class="Keyword">open</a> <a id="26873" class="Keyword">import</a> <a id="26880" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="26912" class="Keyword">open</a> <a id="26917" class="Keyword">import</a> <a id="26924" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="26960" class="Keyword">open</a> <a id="26965" class="Keyword">import</a> <a id="26972" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="27001" class="Keyword">open</a> <a id="27006" class="Keyword">import</a> <a id="27013" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="27041" class="Keyword">open</a> <a id="27046" class="Keyword">import</a> <a id="27053" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="27086" class="Keyword">open</a> <a id="27091" class="Keyword">import</a> <a id="27098" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="27134" class="Keyword">open</a> <a id="27139" class="Keyword">import</a> <a id="27146" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27175" class="Keyword">open</a> <a id="27180" class="Keyword">import</a> <a id="27187" href="group-theory.congruence-relations-groups.html" class="Module">group-theory.congruence-relations-groups</a>
<a id="27228" class="Keyword">open</a> <a id="27233" class="Keyword">import</a> <a id="27240" href="group-theory.congruence-relations-monoids.html" class="Module">group-theory.congruence-relations-monoids</a>
<a id="27282" class="Keyword">open</a> <a id="27287" class="Keyword">import</a> <a id="27294" href="group-theory.congruence-relations-semigroups.html" class="Module">group-theory.congruence-relations-semigroups</a>
<a id="27339" class="Keyword">open</a> <a id="27344" class="Keyword">import</a> <a id="27351" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27376" class="Keyword">open</a> <a id="27381" class="Keyword">import</a> <a id="27388" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27450" class="Keyword">open</a> <a id="27455" class="Keyword">import</a> <a id="27462" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27503" class="Keyword">open</a> <a id="27508" class="Keyword">import</a> <a id="27515" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27544" class="Keyword">open</a> <a id="27549" class="Keyword">import</a> <a id="27556" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27580" class="Keyword">open</a> <a id="27585" class="Keyword">import</a> <a id="27592" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27623" class="Keyword">open</a> <a id="27628" class="Keyword">import</a> <a id="27635" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27682" class="Keyword">open</a> <a id="27687" class="Keyword">import</a> <a id="27694" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="27727" class="Keyword">open</a> <a id="27732" class="Keyword">import</a> <a id="27739" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="27788" class="Keyword">open</a> <a id="27793" class="Keyword">import</a> <a id="27800" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="27840" class="Keyword">open</a> <a id="27845" class="Keyword">import</a> <a id="27852" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="27892" class="Keyword">open</a> <a id="27897" class="Keyword">import</a> <a id="27904" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="27941" class="Keyword">open</a> <a id="27946" class="Keyword">import</a> <a id="27953" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="28000" class="Keyword">open</a> <a id="28005" class="Keyword">import</a> <a id="28012" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="28053" class="Keyword">open</a> <a id="28058" class="Keyword">import</a> <a id="28065" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="28109" class="Keyword">open</a> <a id="28114" class="Keyword">import</a> <a id="28121" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="28160" class="Keyword">open</a> <a id="28165" class="Keyword">import</a> <a id="28172" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28204" class="Keyword">open</a> <a id="28209" class="Keyword">import</a> <a id="28216" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28243" class="Keyword">open</a> <a id="28248" class="Keyword">import</a> <a id="28255" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28275" class="Keyword">open</a> <a id="28280" class="Keyword">import</a> <a id="28287" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28321" class="Keyword">open</a> <a id="28326" class="Keyword">import</a> <a id="28333" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28360" class="Keyword">open</a> <a id="28365" class="Keyword">import</a> <a id="28372" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28414" class="Keyword">open</a> <a id="28419" class="Keyword">import</a> <a id="28426" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28476" class="Keyword">open</a> <a id="28481" class="Keyword">import</a> <a id="28488" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28535" class="Keyword">open</a> <a id="28540" class="Keyword">import</a> <a id="28547" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28588" class="Keyword">open</a> <a id="28593" class="Keyword">import</a> <a id="28600" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28634" class="Keyword">open</a> <a id="28639" class="Keyword">import</a> <a id="28646" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="28694" class="Keyword">open</a> <a id="28699" class="Keyword">import</a> <a id="28706" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="28747" class="Keyword">open</a> <a id="28752" class="Keyword">import</a> <a id="28759" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="28794" class="Keyword">open</a> <a id="28799" class="Keyword">import</a> <a id="28806" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="28844" class="Keyword">open</a> <a id="28849" class="Keyword">import</a> <a id="28856" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="28891" class="Keyword">open</a> <a id="28896" class="Keyword">import</a> <a id="28903" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="28935" class="Keyword">open</a> <a id="28940" class="Keyword">import</a> <a id="28947" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="28988" class="Keyword">open</a> <a id="28993" class="Keyword">import</a> <a id="29000" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="29041" class="Keyword">open</a> <a id="29046" class="Keyword">import</a> <a id="29053" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="29093" class="Keyword">open</a> <a id="29098" class="Keyword">import</a> <a id="29105" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="29138" class="Keyword">open</a> <a id="29143" class="Keyword">import</a> <a id="29150" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29187" class="Keyword">open</a> <a id="29192" class="Keyword">import</a> <a id="29199" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29229" class="Keyword">open</a> <a id="29234" class="Keyword">import</a> <a id="29241" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29262" class="Keyword">open</a> <a id="29267" class="Keyword">import</a> <a id="29274" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29328" class="Keyword">open</a> <a id="29333" class="Keyword">import</a> <a id="29340" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29385" class="Keyword">open</a> <a id="29390" class="Keyword">import</a> <a id="29397" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29425" class="Keyword">open</a> <a id="29430" class="Keyword">import</a> <a id="29437" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29458" class="Keyword">open</a> <a id="29463" class="Keyword">import</a> <a id="29470" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29513" class="Keyword">open</a> <a id="29518" class="Keyword">import</a> <a id="29525" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29559" class="Keyword">open</a> <a id="29564" class="Keyword">import</a> <a id="29571" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29601" class="Keyword">open</a> <a id="29606" class="Keyword">import</a> <a id="29613" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29659" class="Keyword">open</a> <a id="29664" class="Keyword">import</a> <a id="29671" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="29725" class="Keyword">open</a> <a id="29730" class="Keyword">import</a> <a id="29737" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="29780" class="Keyword">open</a> <a id="29785" class="Keyword">import</a> <a id="29792" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="29826" class="Keyword">open</a> <a id="29831" class="Keyword">import</a> <a id="29838" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="29879" class="Keyword">open</a> <a id="29884" class="Keyword">import</a> <a id="29891" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="29926" class="Keyword">open</a> <a id="29931" class="Keyword">import</a> <a id="29938" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a>
<a id="29977" class="Keyword">open</a> <a id="29982" class="Keyword">import</a> <a id="29989" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="30031" class="Keyword">open</a> <a id="30036" class="Keyword">import</a> <a id="30043" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="30078" class="Keyword">open</a> <a id="30083" class="Keyword">import</a> <a id="30090" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="30129" class="Keyword">open</a> <a id="30134" class="Keyword">import</a> <a id="30141" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="30178" class="Keyword">open</a> <a id="30183" class="Keyword">import</a> <a id="30190" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30237" class="Keyword">open</a> <a id="30242" class="Keyword">import</a> <a id="30249" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30313" class="Keyword">open</a> <a id="30318" class="Keyword">import</a> <a id="30325" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30370" class="Keyword">open</a> <a id="30375" class="Keyword">import</a> <a id="30382" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30406" class="Keyword">open</a> <a id="30411" class="Keyword">import</a> <a id="30418" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30443" class="Keyword">open</a> <a id="30448" class="Keyword">import</a> <a id="30455" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30498" class="Keyword">open</a> <a id="30503" class="Keyword">import</a> <a id="30510" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30541" class="Keyword">open</a> <a id="30546" class="Keyword">import</a> <a id="30553" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30607" class="Keyword">open</a> <a id="30612" class="Keyword">import</a> <a id="30619" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30642" class="Keyword">open</a> <a id="30647" class="Keyword">import</a> <a id="30654" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="30692" class="Keyword">open</a> <a id="30697" class="Keyword">import</a> <a id="30704" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="30743" class="Keyword">open</a> <a id="30748" class="Keyword">import</a> <a id="30755" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="30806" class="Keyword">open</a> <a id="30811" class="Keyword">import</a> <a id="30818" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="30855" class="Keyword">open</a> <a id="30860" class="Keyword">import</a> <a id="30867" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="30891" class="Keyword">open</a> <a id="30896" class="Keyword">import</a> <a id="30903" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="30930" class="Keyword">open</a> <a id="30935" class="Keyword">import</a> <a id="30942" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="30999" class="Keyword">open</a> <a id="31004" class="Keyword">import</a> <a id="31011" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="31059" class="Keyword">open</a> <a id="31064" class="Keyword">import</a> <a id="31071" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="31101" class="Keyword">open</a> <a id="31106" class="Keyword">import</a> <a id="31113" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="31150" class="Keyword">open</a> <a id="31155" class="Keyword">import</a> <a id="31162" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="31183" class="Keyword">open</a> <a id="31188" class="Keyword">import</a> <a id="31195" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31242" class="Keyword">open</a> <a id="31247" class="Keyword">import</a> <a id="31254" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31292" class="Keyword">open</a> <a id="31297" class="Keyword">import</a> <a id="31304" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31398" class="Keyword">open</a> <a id="31403" class="Keyword">import</a> <a id="31410" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31425" class="Keyword">open</a> <a id="31430" class="Keyword">import</a> <a id="31437" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31470" class="Keyword">open</a> <a id="31475" class="Keyword">import</a> <a id="31482" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="31514" class="Keyword">open</a> <a id="31519" class="Keyword">import</a> <a id="31526" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="31568" class="Keyword">open</a> <a id="31573" class="Keyword">import</a> <a id="31580" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="31618" class="Keyword">open</a> <a id="31623" class="Keyword">import</a> <a id="31630" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="31667" class="Keyword">open</a> <a id="31672" class="Keyword">import</a> <a id="31679" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="31712" class="Keyword">open</a> <a id="31717" class="Keyword">import</a> <a id="31724" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="31748" class="Keyword">open</a> <a id="31753" class="Keyword">import</a> <a id="31760" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="31799" class="Keyword">open</a> <a id="31804" class="Keyword">import</a> <a id="31811" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="31857" class="Keyword">open</a> <a id="31862" class="Keyword">import</a> <a id="31869" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="31914" class="Keyword">open</a> <a id="31919" class="Keyword">import</a> <a id="31926" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="31964" class="Keyword">open</a> <a id="31969" class="Keyword">import</a> <a id="31976" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="32008" class="Keyword">open</a> <a id="32013" class="Keyword">import</a> <a id="32020" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="32073" class="Keyword">open</a> <a id="32078" class="Keyword">import</a> <a id="32085" href="order-theory.html" class="Module">order-theory</a>
<a id="32098" class="Keyword">open</a> <a id="32103" class="Keyword">import</a> <a id="32110" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="32137" class="Keyword">open</a> <a id="32142" class="Keyword">import</a> <a id="32149" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="32179" class="Keyword">open</a> <a id="32184" class="Keyword">import</a> <a id="32191" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32224" class="Keyword">open</a> <a id="32229" class="Keyword">import</a> <a id="32236" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32272" class="Keyword">open</a> <a id="32277" class="Keyword">import</a> <a id="32284" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32319" class="Keyword">open</a> <a id="32324" class="Keyword">import</a> <a id="32331" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32358" class="Keyword">open</a> <a id="32363" class="Keyword">import</a> <a id="32370" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32400" class="Keyword">open</a> <a id="32405" class="Keyword">import</a> <a id="32412" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32448" class="Keyword">open</a> <a id="32453" class="Keyword">import</a> <a id="32460" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="32502" class="Keyword">open</a> <a id="32507" class="Keyword">import</a> <a id="32514" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32544" class="Keyword">open</a> <a id="32549" class="Keyword">import</a> <a id="32556" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="32588" class="Keyword">open</a> <a id="32593" class="Keyword">import</a> <a id="32600" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="32631" class="Keyword">open</a> <a id="32636" class="Keyword">import</a> <a id="32643" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="32669" class="Keyword">open</a> <a id="32674" class="Keyword">import</a> <a id="32681" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="32710" class="Keyword">open</a> <a id="32715" class="Keyword">import</a> <a id="32722" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="32759" class="Keyword">open</a> <a id="32764" class="Keyword">import</a> <a id="32771" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="32811" class="Keyword">open</a> <a id="32816" class="Keyword">import</a> <a id="32823" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="32845" class="Keyword">open</a> <a id="32850" class="Keyword">import</a> <a id="32857" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="32892" class="Keyword">open</a> <a id="32897" class="Keyword">import</a> <a id="32904" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="32942" class="Keyword">open</a> <a id="32947" class="Keyword">import</a> <a id="32954" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="32993" class="Keyword">open</a> <a id="32998" class="Keyword">import</a> <a id="33005" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="33040" class="Keyword">open</a> <a id="33045" class="Keyword">import</a> <a id="33052" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="33087" class="Keyword">open</a> <a id="33092" class="Keyword">import</a> <a id="33099" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="33134" class="Keyword">open</a> <a id="33139" class="Keyword">import</a> <a id="33146" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="33184" class="Keyword">open</a> <a id="33189" class="Keyword">import</a> <a id="33196" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33227" class="Keyword">open</a> <a id="33232" class="Keyword">import</a> <a id="33239" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33281" class="Keyword">open</a> <a id="33286" class="Keyword">import</a> <a id="33293" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33338" class="Keyword">open</a> <a id="33343" class="Keyword">import</a> <a id="33350" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33383" class="Keyword">open</a> <a id="33388" class="Keyword">import</a> <a id="33395" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33415" class="Keyword">open</a> <a id="33420" class="Keyword">import</a> <a id="33427" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33450" class="Keyword">open</a> <a id="33455" class="Keyword">import</a> <a id="33462" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="33485" class="Keyword">open</a> <a id="33490" class="Keyword">import</a> <a id="33497" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33523" class="Keyword">open</a> <a id="33528" class="Keyword">import</a> <a id="33535" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33561" class="Keyword">open</a> <a id="33566" class="Keyword">import</a> <a id="33573" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="33637" class="Keyword">open</a> <a id="33642" class="Keyword">import</a> <a id="33649" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="33667" class="Keyword">open</a> <a id="33672" class="Keyword">import</a> <a id="33679" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="33706" class="Keyword">open</a> <a id="33711" class="Keyword">import</a> <a id="33718" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="33744" class="Keyword">open</a> <a id="33749" class="Keyword">import</a> <a id="33756" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="33782" class="Keyword">open</a> <a id="33787" class="Keyword">import</a> <a id="33794" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="33820" class="Keyword">open</a> <a id="33825" class="Keyword">import</a> <a id="33832" href="organic-chemistry.ethane.html" class="Module">organic-chemistry.ethane</a>
<a id="33857" class="Keyword">open</a> <a id="33862" class="Keyword">import</a> <a id="33869" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="33900" class="Keyword">open</a> <a id="33905" class="Keyword">import</a> <a id="33912" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="33938" class="Keyword">open</a> <a id="33943" class="Keyword">import</a> <a id="33950" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="34013" class="Keyword">open</a> <a id="34018" class="Keyword">import</a> <a id="34025" href="polytopes.html" class="Module">polytopes</a>
<a id="34035" class="Keyword">open</a> <a id="34040" class="Keyword">import</a> <a id="34047" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="34105" class="Keyword">open</a> <a id="34110" class="Keyword">import</a> <a id="34117" href="ring-theory.html" class="Module">ring-theory</a>
<a id="34129" class="Keyword">open</a> <a id="34134" class="Keyword">import</a> <a id="34141" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="34178" class="Keyword">open</a> <a id="34183" class="Keyword">import</a> <a id="34190" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="34217" class="Keyword">open</a> <a id="34222" class="Keyword">import</a> <a id="34229" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34261" class="Keyword">open</a> <a id="34266" class="Keyword">import</a> <a id="34273" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34319" class="Keyword">open</a> <a id="34324" class="Keyword">import</a> <a id="34331" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34356" class="Keyword">open</a> <a id="34361" class="Keyword">import</a> <a id="34368" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34406" class="Keyword">open</a> <a id="34411" class="Keyword">import</a> <a id="34418" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34461" class="Keyword">open</a> <a id="34466" class="Keyword">import</a> <a id="34473" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="34511" class="Keyword">open</a> <a id="34516" class="Keyword">import</a> <a id="34523" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="34554" class="Keyword">open</a> <a id="34559" class="Keyword">import</a> <a id="34566" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="34590" class="Keyword">open</a> <a id="34595" class="Keyword">import</a> <a id="34602" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="34634" class="Keyword">open</a> <a id="34639" class="Keyword">import</a> <a id="34646" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="34672" class="Keyword">open</a> <a id="34677" class="Keyword">import</a> <a id="34684" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="34713" class="Keyword">open</a> <a id="34718" class="Keyword">import</a> <a id="34725" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="34762" class="Keyword">open</a> <a id="34767" class="Keyword">import</a> <a id="34774" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="34803" class="Keyword">open</a> <a id="34808" class="Keyword">import</a> <a id="34815" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="34842" class="Keyword">open</a> <a id="34847" class="Keyword">import</a> <a id="34854" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="34891" class="Keyword">open</a> <a id="34896" class="Keyword">import</a> <a id="34903" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="34930" class="Keyword">open</a> <a id="34935" class="Keyword">import</a> <a id="34942" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="34975" class="Keyword">open</a> <a id="34980" class="Keyword">import</a> <a id="34987" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="35005" class="Keyword">open</a> <a id="35010" class="Keyword">import</a> <a id="35017" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="35071" class="Keyword">open</a> <a id="35076" class="Keyword">import</a> <a id="35083" href="set-theory.html" class="Module">set-theory</a>
<a id="35094" class="Keyword">open</a> <a id="35099" class="Keyword">import</a> <a id="35106" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="35129" class="Keyword">open</a> <a id="35134" class="Keyword">import</a> <a id="35141" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="35165" class="Keyword">open</a> <a id="35170" class="Keyword">import</a> <a id="35177" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="35202" class="Keyword">open</a> <a id="35207" class="Keyword">import</a> <a id="35214" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="35240" class="Keyword">open</a> <a id="35245" class="Keyword">import</a> <a id="35252" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35314" class="Keyword">open</a> <a id="35319" class="Keyword">import</a> <a id="35326" href="structured-types.html" class="Module">structured-types</a>
<a id="35343" class="Keyword">open</a> <a id="35348" class="Keyword">import</a> <a id="35355" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35390" class="Keyword">open</a> <a id="35395" class="Keyword">import</a> <a id="35402" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35446" class="Keyword">open</a> <a id="35451" class="Keyword">import</a> <a id="35458" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="35522" class="Keyword">open</a> <a id="35527" class="Keyword">import</a> <a id="35534" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="35573" class="Keyword">open</a> <a id="35578" class="Keyword">import</a> <a id="35585" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="35631" class="Keyword">open</a> <a id="35636" class="Keyword">import</a> <a id="35643" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="35708" class="Keyword">open</a> <a id="35713" class="Keyword">import</a> <a id="35720" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="35744" class="Keyword">open</a> <a id="35749" class="Keyword">import</a> <a id="35756" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="35825" class="Keyword">open</a> <a id="35830" class="Keyword">import</a> <a id="35837" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="35882" class="Keyword">open</a> <a id="35887" class="Keyword">import</a> <a id="35894" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="35928" class="Keyword">open</a> <a id="35933" class="Keyword">import</a> <a id="35940" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="36001" class="Keyword">open</a> <a id="36006" class="Keyword">import</a> <a id="36013" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="36058" class="Keyword">open</a> <a id="36063" class="Keyword">import</a> <a id="36070" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="36108" class="Keyword">open</a> <a id="36113" class="Keyword">import</a> <a id="36120" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="36163" class="Keyword">open</a> <a id="36168" class="Keyword">import</a> <a id="36175" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="36211" class="Keyword">open</a> <a id="36216" class="Keyword">import</a> <a id="36223" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36253" class="Keyword">open</a> <a id="36258" class="Keyword">import</a> <a id="36265" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36299" class="Keyword">open</a> <a id="36304" class="Keyword">import</a> <a id="36311" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36342" class="Keyword">open</a> <a id="36347" class="Keyword">import</a> <a id="36354" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36413" class="Keyword">open</a> <a id="36418" class="Keyword">import</a> <a id="36425" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="36476" class="Keyword">open</a> <a id="36481" class="Keyword">import</a> <a id="36488" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="36539" class="Keyword">open</a> <a id="36544" class="Keyword">import</a> <a id="36551" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="36606" class="Keyword">open</a> <a id="36611" class="Keyword">import</a> <a id="36618" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="36650" class="Keyword">open</a> <a id="36655" class="Keyword">import</a> <a id="36662" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="36691" class="Keyword">open</a> <a id="36696" class="Keyword">import</a> <a id="36703" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="36731" class="Keyword">open</a> <a id="36736" class="Keyword">import</a> <a id="36743" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="36773" class="Keyword">open</a> <a id="36778" class="Keyword">import</a> <a id="36785" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="36819" class="Keyword">open</a> <a id="36824" class="Keyword">import</a> <a id="36831" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="36907" class="Keyword">open</a> <a id="36912" class="Keyword">import</a> <a id="36919" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="36945" class="Keyword">open</a> <a id="36950" class="Keyword">import</a> <a id="36957" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="36995" class="Keyword">open</a> <a id="37000" class="Keyword">import</a> <a id="37007" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="37044" class="Keyword">open</a> <a id="37049" class="Keyword">import</a> <a id="37056" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="37096" class="Keyword">open</a> <a id="37101" class="Keyword">import</a> <a id="37108" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="37147" class="Keyword">open</a> <a id="37152" class="Keyword">import</a> <a id="37159" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="37192" class="Keyword">open</a> <a id="37197" class="Keyword">import</a> <a id="37204" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="37247" class="Keyword">open</a> <a id="37252" class="Keyword">import</a> <a id="37259" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37294" class="Keyword">open</a> <a id="37299" class="Keyword">import</a> <a id="37306" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37351" class="Keyword">open</a> <a id="37356" class="Keyword">import</a> <a id="37363" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37400" class="Keyword">open</a> <a id="37405" class="Keyword">import</a> <a id="37412" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37464" class="Keyword">open</a> <a id="37469" class="Keyword">import</a> <a id="37476" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="37529" class="Keyword">open</a> <a id="37534" class="Keyword">import</a> <a id="37541" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="37601" class="Keyword">open</a> <a id="37606" class="Keyword">import</a> <a id="37613" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="37661" class="Keyword">open</a> <a id="37666" class="Keyword">import</a> <a id="37673" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="37713" class="Keyword">open</a> <a id="37718" class="Keyword">import</a> <a id="37725" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="37772" class="Keyword">open</a> <a id="37777" class="Keyword">import</a> <a id="37784" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="37825" class="Keyword">open</a> <a id="37830" class="Keyword">import</a> <a id="37837" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="37875" class="Keyword">open</a> <a id="37880" class="Keyword">import</a> <a id="37887" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="37935" class="Keyword">open</a> <a id="37940" class="Keyword">import</a> <a id="37947" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="37984" class="Keyword">open</a> <a id="37989" class="Keyword">import</a> <a id="37996" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="38031" class="Keyword">open</a> <a id="38036" class="Keyword">import</a> <a id="38043" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="38077" class="Keyword">open</a> <a id="38082" class="Keyword">import</a> <a id="38089" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="38136" class="Keyword">open</a> <a id="38141" class="Keyword">import</a> <a id="38148" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="38193" class="Keyword">open</a> <a id="38198" class="Keyword">import</a> <a id="38205" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38254" class="Keyword">open</a> <a id="38259" class="Keyword">import</a> <a id="38266" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38318" class="Keyword">open</a> <a id="38323" class="Keyword">import</a> <a id="38330" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38384" class="Keyword">open</a> <a id="38389" class="Keyword">import</a> <a id="38396" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="38473" class="Keyword">open</a> <a id="38478" class="Keyword">import</a> <a id="38485" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="38537" class="Keyword">open</a> <a id="38542" class="Keyword">import</a> <a id="38549" href="type-theories.html" class="Module">type-theories</a>
<a id="38563" class="Keyword">open</a> <a id="38568" class="Keyword">import</a> <a id="38575" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="38617" class="Keyword">open</a> <a id="38622" class="Keyword">import</a> <a id="38629" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="38667" class="Keyword">open</a> <a id="38672" class="Keyword">import</a> <a id="38679" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="38725" class="Keyword">open</a> <a id="38730" class="Keyword">import</a> <a id="38737" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="38784" class="Keyword">open</a> <a id="38789" class="Keyword">import</a> <a id="38796" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="38831" class="Keyword">open</a> <a id="38836" class="Keyword">import</a> <a id="38843" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="38921" class="Keyword">open</a> <a id="38926" class="Keyword">import</a> <a id="38933" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="38957" class="Keyword">open</a> <a id="38962" class="Keyword">import</a> <a id="38969" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="39022" class="Keyword">open</a> <a id="39027" class="Keyword">import</a> <a id="39034" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="39077" class="Keyword">open</a> <a id="39082" class="Keyword">import</a> <a id="39089" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="39129" class="Keyword">open</a> <a id="39134" class="Keyword">import</a> <a id="39141" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="39180" class="Keyword">open</a> <a id="39185" class="Keyword">import</a> <a id="39192" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="39226" class="Keyword">open</a> <a id="39231" class="Keyword">import</a> <a id="39238" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39286" class="Keyword">open</a> <a id="39291" class="Keyword">import</a> <a id="39298" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39349" class="Keyword">open</a> <a id="39354" class="Keyword">import</a> <a id="39361" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39408" class="Keyword">open</a> <a id="39413" class="Keyword">import</a> <a id="39420" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39472" class="Keyword">open</a> <a id="39477" class="Keyword">import</a> <a id="39484" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39528" class="Keyword">open</a> <a id="39533" class="Keyword">import</a> <a id="39540" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="39580" class="Keyword">open</a> <a id="39585" class="Keyword">import</a> <a id="39592" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="39635" class="Keyword">open</a> <a id="39640" class="Keyword">import</a> <a id="39647" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="39699" class="Keyword">open</a> <a id="39704" class="Keyword">import</a> <a id="39711" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="39765" class="Keyword">open</a> <a id="39770" class="Keyword">import</a> <a id="39777" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="39825" class="Keyword">open</a> <a id="39830" class="Keyword">import</a> <a id="39837" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="39876" class="Keyword">open</a> <a id="39881" class="Keyword">import</a> <a id="39888" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="39921" class="Keyword">open</a> <a id="39926" class="Keyword">import</a> <a id="39933" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="39963" class="Keyword">open</a> <a id="39968" class="Keyword">import</a> <a id="39975" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="40026" class="Keyword">open</a> <a id="40031" class="Keyword">import</a> <a id="40038" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="40079" class="Keyword">open</a> <a id="40084" class="Keyword">import</a> <a id="40091" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="40128" class="Keyword">open</a> <a id="40133" class="Keyword">import</a> <a id="40140" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="40199" class="Keyword">open</a> <a id="40204" class="Keyword">import</a> <a id="40211" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40266" class="Keyword">open</a> <a id="40271" class="Keyword">import</a> <a id="40278" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40334" class="Keyword">open</a> <a id="40339" class="Keyword">import</a> <a id="40346" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40393" class="Keyword">open</a> <a id="40398" class="Keyword">import</a> <a id="40405" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40448" class="Keyword">open</a> <a id="40453" class="Keyword">import</a> <a id="40460" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40505" class="Keyword">open</a> <a id="40510" class="Keyword">import</a> <a id="40517" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="40566" class="Keyword">open</a> <a id="40571" class="Keyword">import</a> <a id="40578" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="40629" class="Keyword">open</a> <a id="40634" class="Keyword">import</a> <a id="40641" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="40685" class="Keyword">open</a> <a id="40690" class="Keyword">import</a> <a id="40697" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="40775" class="Keyword">open</a> <a id="40780" class="Keyword">import</a> <a id="40787" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="40827" class="Keyword">open</a> <a id="40832" class="Keyword">import</a> <a id="40839" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="40896" class="Keyword">open</a> <a id="40901" class="Keyword">import</a> <a id="40908" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="40943" class="Keyword">open</a> <a id="40948" class="Keyword">import</a> <a id="40955" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="41001" class="Keyword">open</a> <a id="41006" class="Keyword">import</a> <a id="41013" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="41068" class="Keyword">open</a> <a id="41073" class="Keyword">import</a> <a id="41080" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="41123" class="Keyword">open</a> <a id="41128" class="Keyword">import</a> <a id="41135" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="41180" class="Keyword">open</a> <a id="41185" class="Keyword">import</a> <a id="41192" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41251" class="Keyword">open</a> <a id="41256" class="Keyword">import</a> <a id="41263" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41300" class="Keyword">open</a> <a id="41305" class="Keyword">import</a> <a id="41312" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41354" class="Keyword">open</a> <a id="41359" class="Keyword">import</a> <a id="41366" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41407" class="Keyword">open</a> <a id="41412" class="Keyword">import</a> <a id="41419" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41458" class="Keyword">open</a> <a id="41463" class="Keyword">import</a> <a id="41470" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41508" class="Keyword">open</a> <a id="41513" class="Keyword">import</a> <a id="41520" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="41572" class="Keyword">open</a> <a id="41577" class="Keyword">import</a> <a id="41584" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="41629" class="Keyword">open</a> <a id="41634" class="Keyword">import</a> <a id="41641" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="41680" class="Keyword">open</a> <a id="41685" class="Keyword">import</a> <a id="41692" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="41729" class="Keyword">open</a> <a id="41734" class="Keyword">import</a> <a id="41741" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="41790" class="Keyword">open</a> <a id="41795" class="Keyword">import</a> <a id="41802" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="41841" class="Keyword">open</a> <a id="41846" class="Keyword">import</a> <a id="41853" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="41891" class="Keyword">open</a> <a id="41896" class="Keyword">import</a> <a id="41903" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="41958" class="Keyword">open</a> <a id="41963" class="Keyword">import</a> <a id="41970" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="42009" class="Keyword">open</a> <a id="42014" class="Keyword">import</a> <a id="42021" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="42069" class="Keyword">open</a> <a id="42074" class="Keyword">import</a> <a id="42081" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="42128" class="Keyword">open</a> <a id="42133" class="Keyword">import</a> <a id="42140" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="42178" class="Keyword">open</a> <a id="42183" class="Keyword">import</a> <a id="42190" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="42220" class="Keyword">open</a> <a id="42225" class="Keyword">import</a> <a id="42232" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42289" class="Keyword">open</a> <a id="42294" class="Keyword">import</a> <a id="42301" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42355" class="Keyword">open</a> <a id="42360" class="Keyword">import</a> <a id="42367" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42397" class="Keyword">open</a> <a id="42402" class="Keyword">import</a> <a id="42409" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42458" class="Keyword">open</a> <a id="42463" class="Keyword">import</a> <a id="42470" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42512" class="Keyword">open</a> <a id="42517" class="Keyword">import</a> <a id="42524" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="42558" class="Keyword">open</a> <a id="42563" class="Keyword">import</a> <a id="42570" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="42633" class="Keyword">open</a> <a id="42638" class="Keyword">import</a> <a id="42645" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="42688" class="Keyword">open</a> <a id="42693" class="Keyword">import</a> <a id="42700" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="42735" class="Keyword">open</a> <a id="42740" class="Keyword">import</a> <a id="42747" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="42782" class="Keyword">open</a> <a id="42787" class="Keyword">import</a> <a id="42794" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="42834" class="Keyword">open</a> <a id="42839" class="Keyword">import</a> <a id="42846" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="42891" class="Keyword">open</a> <a id="42896" class="Keyword">import</a> <a id="42903" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="42944" class="Keyword">open</a> <a id="42949" class="Keyword">import</a> <a id="42956" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="43010" class="Keyword">open</a> <a id="43015" class="Keyword">import</a> <a id="43022" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="43072" class="Keyword">open</a> <a id="43077" class="Keyword">import</a> <a id="43084" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="43131" class="Keyword">open</a> <a id="43136" class="Keyword">import</a> <a id="43143" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="43181" class="Keyword">open</a> <a id="43186" class="Keyword">import</a> <a id="43193" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="43242" class="Keyword">open</a> <a id="43247" class="Keyword">import</a> <a id="43254" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43301" class="Keyword">open</a> <a id="43306" class="Keyword">import</a> <a id="43313" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43376" class="Keyword">open</a> <a id="43381" class="Keyword">import</a> <a id="43388" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43420" class="Keyword">open</a> <a id="43425" class="Keyword">import</a> <a id="43432" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43485" class="Keyword">open</a> <a id="43490" class="Keyword">import</a> <a id="43497" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="43543" class="Keyword">open</a> <a id="43548" class="Keyword">import</a> <a id="43555" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="43601" class="Keyword">open</a> <a id="43606" class="Keyword">import</a> <a id="43613" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="43653" class="Keyword">open</a> <a id="43658" class="Keyword">import</a> <a id="43665" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="43712" class="Keyword">open</a> <a id="43717" class="Keyword">import</a> <a id="43724" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="43772" class="Keyword">open</a> <a id="43777" class="Keyword">import</a> <a id="43784" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="43824" class="Keyword">open</a> <a id="43829" class="Keyword">import</a> <a id="43836" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="43881" class="Keyword">open</a> <a id="43886" class="Keyword">import</a> <a id="43893" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="43958" class="Keyword">open</a> <a id="43963" class="Keyword">import</a> <a id="43970" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="44015" class="Keyword">open</a> <a id="44020" class="Keyword">import</a> <a id="44027" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="44074" class="Keyword">open</a> <a id="44079" class="Keyword">import</a> <a id="44086" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="44139" class="Keyword">open</a> <a id="44144" class="Keyword">import</a> <a id="44151" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>