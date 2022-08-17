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
<a id="21932" class="Keyword">open</a> <a id="21937" class="Keyword">import</a> <a id="21944" href="foundation-core.automorphisms.html" class="Module">foundation-core.automorphisms</a>
<a id="21974" class="Keyword">open</a> <a id="21979" class="Keyword">import</a> <a id="21986" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="22026" class="Keyword">open</a> <a id="22031" class="Keyword">import</a> <a id="22038" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22081" class="Keyword">open</a> <a id="22086" class="Keyword">import</a> <a id="22093" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22127" class="Keyword">open</a> <a id="22132" class="Keyword">import</a> <a id="22139" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22171" class="Keyword">open</a> <a id="22176" class="Keyword">import</a> <a id="22183" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22213" class="Keyword">open</a> <a id="22218" class="Keyword">import</a> <a id="22225" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22259" class="Keyword">open</a> <a id="22264" class="Keyword">import</a> <a id="22271" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22306" class="Keyword">open</a> <a id="22311" class="Keyword">import</a> <a id="22318" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22342" class="Keyword">open</a> <a id="22347" class="Keyword">import</a> <a id="22354" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22391" class="Keyword">open</a> <a id="22396" class="Keyword">import</a> <a id="22403" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22430" class="Keyword">open</a> <a id="22435" class="Keyword">import</a> <a id="22442" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22470" class="Keyword">open</a> <a id="22475" class="Keyword">import</a> <a id="22482" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22512" class="Keyword">open</a> <a id="22517" class="Keyword">import</a> <a id="22524" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22573" class="Keyword">open</a> <a id="22578" class="Keyword">import</a> <a id="22585" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22631" class="Keyword">open</a> <a id="22636" class="Keyword">import</a> <a id="22643" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22683" class="Keyword">open</a> <a id="22688" class="Keyword">import</a> <a id="22695" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22733" class="Keyword">open</a> <a id="22738" class="Keyword">import</a> <a id="22745" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22774" class="Keyword">open</a> <a id="22779" class="Keyword">import</a> <a id="22786" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22816" class="Keyword">open</a> <a id="22821" class="Keyword">import</a> <a id="22828" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22859" class="Keyword">open</a> <a id="22864" class="Keyword">import</a> <a id="22871" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="22911" class="Keyword">open</a> <a id="22916" class="Keyword">import</a> <a id="22923" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="22949" class="Keyword">open</a> <a id="22954" class="Keyword">import</a> <a id="22961" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="23016" class="Keyword">open</a> <a id="23021" class="Keyword">import</a> <a id="23028" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23079" class="Keyword">open</a> <a id="23084" class="Keyword">import</a> <a id="23091" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23136" class="Keyword">open</a> <a id="23141" class="Keyword">import</a> <a id="23148" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23193" class="Keyword">open</a> <a id="23198" class="Keyword">import</a> <a id="23205" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23259" class="Keyword">open</a> <a id="23264" class="Keyword">import</a> <a id="23271" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23298" class="Keyword">open</a> <a id="23303" class="Keyword">import</a> <a id="23310" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23343" class="Keyword">open</a> <a id="23348" class="Keyword">import</a> <a id="23355" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23386" class="Keyword">open</a> <a id="23391" class="Keyword">import</a> <a id="23398" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23435" class="Keyword">open</a> <a id="23440" class="Keyword">import</a> <a id="23447" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23481" class="Keyword">open</a> <a id="23486" class="Keyword">import</a> <a id="23493" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23518" class="Keyword">open</a> <a id="23523" class="Keyword">import</a> <a id="23530" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23562" class="Keyword">open</a> <a id="23567" class="Keyword">import</a> <a id="23574" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23609" class="Keyword">open</a> <a id="23614" class="Keyword">import</a> <a id="23621" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23650" class="Keyword">open</a> <a id="23655" class="Keyword">import</a> <a id="23662" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23688" class="Keyword">open</a> <a id="23693" class="Keyword">import</a> <a id="23700" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23728" class="Keyword">open</a> <a id="23733" class="Keyword">import</a> <a id="23740" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23765" class="Keyword">open</a> <a id="23770" class="Keyword">import</a> <a id="23777" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23798" class="Keyword">open</a> <a id="23803" class="Keyword">import</a> <a id="23810" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23846" class="Keyword">open</a> <a id="23851" class="Keyword">import</a> <a id="23858" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="23901" class="Keyword">open</a> <a id="23906" class="Keyword">import</a> <a id="23913" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="23938" class="Keyword">open</a> <a id="23943" class="Keyword">import</a> <a id="23950" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="23981" class="Keyword">open</a> <a id="23986" class="Keyword">import</a> <a id="23993" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="24025" class="Keyword">open</a> <a id="24030" class="Keyword">import</a> <a id="24037" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24071" class="Keyword">open</a> <a id="24076" class="Keyword">import</a> <a id="24083" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24139" class="Keyword">open</a> <a id="24144" class="Keyword">import</a> <a id="24151" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24204" class="Keyword">open</a> <a id="24209" class="Keyword">import</a> <a id="24216" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24243" class="Keyword">open</a> <a id="24248" class="Keyword">import</a> <a id="24255" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24300" class="Keyword">open</a> <a id="24305" class="Keyword">import</a> <a id="24312" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24374" class="Keyword">open</a> <a id="24379" class="Keyword">import</a> <a id="24386" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24399" class="Keyword">open</a> <a id="24404" class="Keyword">import</a> <a id="24411" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24451" class="Keyword">open</a> <a id="24456" class="Keyword">import</a> <a id="24463" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24507" class="Keyword">open</a> <a id="24512" class="Keyword">import</a> <a id="24519" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24558" class="Keyword">open</a> <a id="24563" class="Keyword">import</a> <a id="24570" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24612" class="Keyword">open</a> <a id="24617" class="Keyword">import</a> <a id="24624" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24664" class="Keyword">open</a> <a id="24669" class="Keyword">import</a> <a id="24676" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24717" class="Keyword">open</a> <a id="24722" class="Keyword">import</a> <a id="24729" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24767" class="Keyword">open</a> <a id="24772" class="Keyword">import</a> <a id="24779" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24842" class="Keyword">open</a> <a id="24847" class="Keyword">import</a> <a id="24854" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="24883" class="Keyword">open</a> <a id="24888" class="Keyword">import</a> <a id="24895" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="24940" class="Keyword">open</a> <a id="24945" class="Keyword">import</a> <a id="24952" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="24994" class="Keyword">open</a> <a id="24999" class="Keyword">import</a> <a id="25006" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25046" class="Keyword">open</a> <a id="25051" class="Keyword">import</a> <a id="25058" href="graph-theory.equivalences-enriched-undirected-graphs.html" class="Module">graph-theory.equivalences-enriched-undirected-graphs</a>
<a id="25111" class="Keyword">open</a> <a id="25116" class="Keyword">import</a> <a id="25123" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25167" class="Keyword">open</a> <a id="25172" class="Keyword">import</a> <a id="25179" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25228" class="Keyword">open</a> <a id="25233" class="Keyword">import</a> <a id="25240" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25290" class="Keyword">open</a> <a id="25295" class="Keyword">import</a> <a id="25302" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25329" class="Keyword">open</a> <a id="25334" class="Keyword">import</a> <a id="25341" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25366" class="Keyword">open</a> <a id="25371" class="Keyword">import</a> <a id="25378" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25401" class="Keyword">open</a> <a id="25406" class="Keyword">import</a> <a id="25413" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25462" class="Keyword">open</a> <a id="25467" class="Keyword">import</a> <a id="25474" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25513" class="Keyword">open</a> <a id="25518" class="Keyword">import</a> <a id="25525" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25566" class="Keyword">open</a> <a id="25571" class="Keyword">import</a> <a id="25578" href="graph-theory.neighbors-undirected-graphs.html" class="Module">graph-theory.neighbors-undirected-graphs</a>
<a id="25619" class="Keyword">open</a> <a id="25624" class="Keyword">import</a> <a id="25631" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25675" class="Keyword">open</a> <a id="25680" class="Keyword">import</a> <a id="25687" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25724" class="Keyword">open</a> <a id="25729" class="Keyword">import</a> <a id="25736" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="25758" class="Keyword">open</a> <a id="25763" class="Keyword">import</a> <a id="25770" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="25800" class="Keyword">open</a> <a id="25805" class="Keyword">import</a> <a id="25812" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="25851" class="Keyword">open</a> <a id="25856" class="Keyword">import</a> <a id="25863" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="25894" class="Keyword">open</a> <a id="25899" class="Keyword">import</a> <a id="25906" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="25932" class="Keyword">open</a> <a id="25937" class="Keyword">import</a> <a id="25944" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="25982" class="Keyword">open</a> <a id="25987" class="Keyword">import</a> <a id="25994" href="graph-theory.stereoisomerism-enriched-undirected-graphs.html" class="Module">graph-theory.stereoisomerism-enriched-undirected-graphs</a>
<a id="26050" class="Keyword">open</a> <a id="26055" class="Keyword">import</a> <a id="26062" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="26120" class="Keyword">open</a> <a id="26125" class="Keyword">import</a> <a id="26132" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="26170" class="Keyword">open</a> <a id="26175" class="Keyword">import</a> <a id="26182" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26201" class="Keyword">open</a> <a id="26206" class="Keyword">import</a> <a id="26213" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26278" class="Keyword">open</a> <a id="26283" class="Keyword">import</a> <a id="26290" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26321" class="Keyword">open</a> <a id="26326" class="Keyword">import</a> <a id="26333" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26360" class="Keyword">open</a> <a id="26365" class="Keyword">import</a> <a id="26372" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26400" class="Keyword">open</a> <a id="26405" class="Keyword">import</a> <a id="26412" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26479" class="Keyword">open</a> <a id="26484" class="Keyword">import</a> <a id="26491" href="group-theory.html" class="Module">group-theory</a>
<a id="26504" class="Keyword">open</a> <a id="26509" class="Keyword">import</a> <a id="26516" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26544" class="Keyword">open</a> <a id="26549" class="Keyword">import</a> <a id="26556" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26607" class="Keyword">open</a> <a id="26612" class="Keyword">import</a> <a id="26619" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="26652" class="Keyword">open</a> <a id="26657" class="Keyword">import</a> <a id="26664" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26711" class="Keyword">open</a> <a id="26716" class="Keyword">import</a> <a id="26723" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26762" class="Keyword">open</a> <a id="26767" class="Keyword">import</a> <a id="26774" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="26814" class="Keyword">open</a> <a id="26819" class="Keyword">import</a> <a id="26826" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="26869" class="Keyword">open</a> <a id="26874" class="Keyword">import</a> <a id="26881" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="26913" class="Keyword">open</a> <a id="26918" class="Keyword">import</a> <a id="26925" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="26961" class="Keyword">open</a> <a id="26966" class="Keyword">import</a> <a id="26973" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="27002" class="Keyword">open</a> <a id="27007" class="Keyword">import</a> <a id="27014" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="27042" class="Keyword">open</a> <a id="27047" class="Keyword">import</a> <a id="27054" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="27087" class="Keyword">open</a> <a id="27092" class="Keyword">import</a> <a id="27099" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="27135" class="Keyword">open</a> <a id="27140" class="Keyword">import</a> <a id="27147" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27176" class="Keyword">open</a> <a id="27181" class="Keyword">import</a> <a id="27188" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27213" class="Keyword">open</a> <a id="27218" class="Keyword">import</a> <a id="27225" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27287" class="Keyword">open</a> <a id="27292" class="Keyword">import</a> <a id="27299" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27340" class="Keyword">open</a> <a id="27345" class="Keyword">import</a> <a id="27352" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27381" class="Keyword">open</a> <a id="27386" class="Keyword">import</a> <a id="27393" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27417" class="Keyword">open</a> <a id="27422" class="Keyword">import</a> <a id="27429" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27460" class="Keyword">open</a> <a id="27465" class="Keyword">import</a> <a id="27472" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27519" class="Keyword">open</a> <a id="27524" class="Keyword">import</a> <a id="27531" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="27564" class="Keyword">open</a> <a id="27569" class="Keyword">import</a> <a id="27576" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="27625" class="Keyword">open</a> <a id="27630" class="Keyword">import</a> <a id="27637" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="27677" class="Keyword">open</a> <a id="27682" class="Keyword">import</a> <a id="27689" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="27729" class="Keyword">open</a> <a id="27734" class="Keyword">import</a> <a id="27741" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="27778" class="Keyword">open</a> <a id="27783" class="Keyword">import</a> <a id="27790" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="27837" class="Keyword">open</a> <a id="27842" class="Keyword">import</a> <a id="27849" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="27890" class="Keyword">open</a> <a id="27895" class="Keyword">import</a> <a id="27902" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="27946" class="Keyword">open</a> <a id="27951" class="Keyword">import</a> <a id="27958" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="27997" class="Keyword">open</a> <a id="28002" class="Keyword">import</a> <a id="28009" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28041" class="Keyword">open</a> <a id="28046" class="Keyword">import</a> <a id="28053" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28080" class="Keyword">open</a> <a id="28085" class="Keyword">import</a> <a id="28092" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28112" class="Keyword">open</a> <a id="28117" class="Keyword">import</a> <a id="28124" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28158" class="Keyword">open</a> <a id="28163" class="Keyword">import</a> <a id="28170" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28197" class="Keyword">open</a> <a id="28202" class="Keyword">import</a> <a id="28209" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28251" class="Keyword">open</a> <a id="28256" class="Keyword">import</a> <a id="28263" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28313" class="Keyword">open</a> <a id="28318" class="Keyword">import</a> <a id="28325" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28372" class="Keyword">open</a> <a id="28377" class="Keyword">import</a> <a id="28384" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28425" class="Keyword">open</a> <a id="28430" class="Keyword">import</a> <a id="28437" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28471" class="Keyword">open</a> <a id="28476" class="Keyword">import</a> <a id="28483" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="28531" class="Keyword">open</a> <a id="28536" class="Keyword">import</a> <a id="28543" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="28584" class="Keyword">open</a> <a id="28589" class="Keyword">import</a> <a id="28596" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="28631" class="Keyword">open</a> <a id="28636" class="Keyword">import</a> <a id="28643" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="28681" class="Keyword">open</a> <a id="28686" class="Keyword">import</a> <a id="28693" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="28728" class="Keyword">open</a> <a id="28733" class="Keyword">import</a> <a id="28740" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="28772" class="Keyword">open</a> <a id="28777" class="Keyword">import</a> <a id="28784" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="28825" class="Keyword">open</a> <a id="28830" class="Keyword">import</a> <a id="28837" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="28878" class="Keyword">open</a> <a id="28883" class="Keyword">import</a> <a id="28890" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="28930" class="Keyword">open</a> <a id="28935" class="Keyword">import</a> <a id="28942" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="28975" class="Keyword">open</a> <a id="28980" class="Keyword">import</a> <a id="28987" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29024" class="Keyword">open</a> <a id="29029" class="Keyword">import</a> <a id="29036" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29066" class="Keyword">open</a> <a id="29071" class="Keyword">import</a> <a id="29078" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29099" class="Keyword">open</a> <a id="29104" class="Keyword">import</a> <a id="29111" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29165" class="Keyword">open</a> <a id="29170" class="Keyword">import</a> <a id="29177" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29222" class="Keyword">open</a> <a id="29227" class="Keyword">import</a> <a id="29234" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29262" class="Keyword">open</a> <a id="29267" class="Keyword">import</a> <a id="29274" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29295" class="Keyword">open</a> <a id="29300" class="Keyword">import</a> <a id="29307" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29350" class="Keyword">open</a> <a id="29355" class="Keyword">import</a> <a id="29362" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29396" class="Keyword">open</a> <a id="29401" class="Keyword">import</a> <a id="29408" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29438" class="Keyword">open</a> <a id="29443" class="Keyword">import</a> <a id="29450" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29496" class="Keyword">open</a> <a id="29501" class="Keyword">import</a> <a id="29508" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="29562" class="Keyword">open</a> <a id="29567" class="Keyword">import</a> <a id="29574" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="29617" class="Keyword">open</a> <a id="29622" class="Keyword">import</a> <a id="29629" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="29663" class="Keyword">open</a> <a id="29668" class="Keyword">import</a> <a id="29675" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="29716" class="Keyword">open</a> <a id="29721" class="Keyword">import</a> <a id="29728" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="29763" class="Keyword">open</a> <a id="29768" class="Keyword">import</a> <a id="29775" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="29817" class="Keyword">open</a> <a id="29822" class="Keyword">import</a> <a id="29829" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="29864" class="Keyword">open</a> <a id="29869" class="Keyword">import</a> <a id="29876" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="29915" class="Keyword">open</a> <a id="29920" class="Keyword">import</a> <a id="29927" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="29964" class="Keyword">open</a> <a id="29969" class="Keyword">import</a> <a id="29976" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30023" class="Keyword">open</a> <a id="30028" class="Keyword">import</a> <a id="30035" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30099" class="Keyword">open</a> <a id="30104" class="Keyword">import</a> <a id="30111" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30156" class="Keyword">open</a> <a id="30161" class="Keyword">import</a> <a id="30168" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30192" class="Keyword">open</a> <a id="30197" class="Keyword">import</a> <a id="30204" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30229" class="Keyword">open</a> <a id="30234" class="Keyword">import</a> <a id="30241" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30284" class="Keyword">open</a> <a id="30289" class="Keyword">import</a> <a id="30296" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30327" class="Keyword">open</a> <a id="30332" class="Keyword">import</a> <a id="30339" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30393" class="Keyword">open</a> <a id="30398" class="Keyword">import</a> <a id="30405" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30428" class="Keyword">open</a> <a id="30433" class="Keyword">import</a> <a id="30440" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="30478" class="Keyword">open</a> <a id="30483" class="Keyword">import</a> <a id="30490" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="30529" class="Keyword">open</a> <a id="30534" class="Keyword">import</a> <a id="30541" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="30592" class="Keyword">open</a> <a id="30597" class="Keyword">import</a> <a id="30604" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="30641" class="Keyword">open</a> <a id="30646" class="Keyword">import</a> <a id="30653" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="30677" class="Keyword">open</a> <a id="30682" class="Keyword">import</a> <a id="30689" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="30716" class="Keyword">open</a> <a id="30721" class="Keyword">import</a> <a id="30728" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="30785" class="Keyword">open</a> <a id="30790" class="Keyword">import</a> <a id="30797" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="30845" class="Keyword">open</a> <a id="30850" class="Keyword">import</a> <a id="30857" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="30887" class="Keyword">open</a> <a id="30892" class="Keyword">import</a> <a id="30899" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="30936" class="Keyword">open</a> <a id="30941" class="Keyword">import</a> <a id="30948" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="30969" class="Keyword">open</a> <a id="30974" class="Keyword">import</a> <a id="30981" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31028" class="Keyword">open</a> <a id="31033" class="Keyword">import</a> <a id="31040" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31078" class="Keyword">open</a> <a id="31083" class="Keyword">import</a> <a id="31090" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31184" class="Keyword">open</a> <a id="31189" class="Keyword">import</a> <a id="31196" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31211" class="Keyword">open</a> <a id="31216" class="Keyword">import</a> <a id="31223" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31256" class="Keyword">open</a> <a id="31261" class="Keyword">import</a> <a id="31268" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="31300" class="Keyword">open</a> <a id="31305" class="Keyword">import</a> <a id="31312" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="31354" class="Keyword">open</a> <a id="31359" class="Keyword">import</a> <a id="31366" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="31404" class="Keyword">open</a> <a id="31409" class="Keyword">import</a> <a id="31416" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="31453" class="Keyword">open</a> <a id="31458" class="Keyword">import</a> <a id="31465" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="31498" class="Keyword">open</a> <a id="31503" class="Keyword">import</a> <a id="31510" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="31534" class="Keyword">open</a> <a id="31539" class="Keyword">import</a> <a id="31546" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="31585" class="Keyword">open</a> <a id="31590" class="Keyword">import</a> <a id="31597" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="31643" class="Keyword">open</a> <a id="31648" class="Keyword">import</a> <a id="31655" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="31700" class="Keyword">open</a> <a id="31705" class="Keyword">import</a> <a id="31712" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="31750" class="Keyword">open</a> <a id="31755" class="Keyword">import</a> <a id="31762" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="31794" class="Keyword">open</a> <a id="31799" class="Keyword">import</a> <a id="31806" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="31859" class="Keyword">open</a> <a id="31864" class="Keyword">import</a> <a id="31871" href="order-theory.html" class="Module">order-theory</a>
<a id="31884" class="Keyword">open</a> <a id="31889" class="Keyword">import</a> <a id="31896" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="31923" class="Keyword">open</a> <a id="31928" class="Keyword">import</a> <a id="31935" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="31965" class="Keyword">open</a> <a id="31970" class="Keyword">import</a> <a id="31977" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32010" class="Keyword">open</a> <a id="32015" class="Keyword">import</a> <a id="32022" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32058" class="Keyword">open</a> <a id="32063" class="Keyword">import</a> <a id="32070" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32105" class="Keyword">open</a> <a id="32110" class="Keyword">import</a> <a id="32117" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32144" class="Keyword">open</a> <a id="32149" class="Keyword">import</a> <a id="32156" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32186" class="Keyword">open</a> <a id="32191" class="Keyword">import</a> <a id="32198" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32234" class="Keyword">open</a> <a id="32239" class="Keyword">import</a> <a id="32246" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="32288" class="Keyword">open</a> <a id="32293" class="Keyword">import</a> <a id="32300" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32330" class="Keyword">open</a> <a id="32335" class="Keyword">import</a> <a id="32342" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="32374" class="Keyword">open</a> <a id="32379" class="Keyword">import</a> <a id="32386" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="32417" class="Keyword">open</a> <a id="32422" class="Keyword">import</a> <a id="32429" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="32455" class="Keyword">open</a> <a id="32460" class="Keyword">import</a> <a id="32467" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="32496" class="Keyword">open</a> <a id="32501" class="Keyword">import</a> <a id="32508" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="32545" class="Keyword">open</a> <a id="32550" class="Keyword">import</a> <a id="32557" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="32597" class="Keyword">open</a> <a id="32602" class="Keyword">import</a> <a id="32609" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="32631" class="Keyword">open</a> <a id="32636" class="Keyword">import</a> <a id="32643" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="32678" class="Keyword">open</a> <a id="32683" class="Keyword">import</a> <a id="32690" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="32728" class="Keyword">open</a> <a id="32733" class="Keyword">import</a> <a id="32740" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="32779" class="Keyword">open</a> <a id="32784" class="Keyword">import</a> <a id="32791" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="32826" class="Keyword">open</a> <a id="32831" class="Keyword">import</a> <a id="32838" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="32873" class="Keyword">open</a> <a id="32878" class="Keyword">import</a> <a id="32885" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="32920" class="Keyword">open</a> <a id="32925" class="Keyword">import</a> <a id="32932" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="32970" class="Keyword">open</a> <a id="32975" class="Keyword">import</a> <a id="32982" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33013" class="Keyword">open</a> <a id="33018" class="Keyword">import</a> <a id="33025" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33067" class="Keyword">open</a> <a id="33072" class="Keyword">import</a> <a id="33079" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33124" class="Keyword">open</a> <a id="33129" class="Keyword">import</a> <a id="33136" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33169" class="Keyword">open</a> <a id="33174" class="Keyword">import</a> <a id="33181" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33201" class="Keyword">open</a> <a id="33206" class="Keyword">import</a> <a id="33213" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33236" class="Keyword">open</a> <a id="33241" class="Keyword">import</a> <a id="33248" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="33271" class="Keyword">open</a> <a id="33276" class="Keyword">import</a> <a id="33283" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33309" class="Keyword">open</a> <a id="33314" class="Keyword">import</a> <a id="33321" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33347" class="Keyword">open</a> <a id="33352" class="Keyword">import</a> <a id="33359" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="33423" class="Keyword">open</a> <a id="33428" class="Keyword">import</a> <a id="33435" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="33453" class="Keyword">open</a> <a id="33458" class="Keyword">import</a> <a id="33465" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="33492" class="Keyword">open</a> <a id="33497" class="Keyword">import</a> <a id="33504" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="33530" class="Keyword">open</a> <a id="33535" class="Keyword">import</a> <a id="33542" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="33568" class="Keyword">open</a> <a id="33573" class="Keyword">import</a> <a id="33580" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="33606" class="Keyword">open</a> <a id="33611" class="Keyword">import</a> <a id="33618" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="33649" class="Keyword">open</a> <a id="33654" class="Keyword">import</a> <a id="33661" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="33687" class="Keyword">open</a> <a id="33692" class="Keyword">import</a> <a id="33699" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="33762" class="Keyword">open</a> <a id="33767" class="Keyword">import</a> <a id="33774" href="polytopes.html" class="Module">polytopes</a>
<a id="33784" class="Keyword">open</a> <a id="33789" class="Keyword">import</a> <a id="33796" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="33854" class="Keyword">open</a> <a id="33859" class="Keyword">import</a> <a id="33866" href="ring-theory.html" class="Module">ring-theory</a>
<a id="33878" class="Keyword">open</a> <a id="33883" class="Keyword">import</a> <a id="33890" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="33927" class="Keyword">open</a> <a id="33932" class="Keyword">import</a> <a id="33939" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="33966" class="Keyword">open</a> <a id="33971" class="Keyword">import</a> <a id="33978" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34010" class="Keyword">open</a> <a id="34015" class="Keyword">import</a> <a id="34022" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34068" class="Keyword">open</a> <a id="34073" class="Keyword">import</a> <a id="34080" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34105" class="Keyword">open</a> <a id="34110" class="Keyword">import</a> <a id="34117" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34155" class="Keyword">open</a> <a id="34160" class="Keyword">import</a> <a id="34167" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34210" class="Keyword">open</a> <a id="34215" class="Keyword">import</a> <a id="34222" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="34260" class="Keyword">open</a> <a id="34265" class="Keyword">import</a> <a id="34272" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="34303" class="Keyword">open</a> <a id="34308" class="Keyword">import</a> <a id="34315" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="34339" class="Keyword">open</a> <a id="34344" class="Keyword">import</a> <a id="34351" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="34383" class="Keyword">open</a> <a id="34388" class="Keyword">import</a> <a id="34395" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="34421" class="Keyword">open</a> <a id="34426" class="Keyword">import</a> <a id="34433" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="34462" class="Keyword">open</a> <a id="34467" class="Keyword">import</a> <a id="34474" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="34511" class="Keyword">open</a> <a id="34516" class="Keyword">import</a> <a id="34523" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="34552" class="Keyword">open</a> <a id="34557" class="Keyword">import</a> <a id="34564" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="34591" class="Keyword">open</a> <a id="34596" class="Keyword">import</a> <a id="34603" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="34640" class="Keyword">open</a> <a id="34645" class="Keyword">import</a> <a id="34652" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="34679" class="Keyword">open</a> <a id="34684" class="Keyword">import</a> <a id="34691" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="34724" class="Keyword">open</a> <a id="34729" class="Keyword">import</a> <a id="34736" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="34754" class="Keyword">open</a> <a id="34759" class="Keyword">import</a> <a id="34766" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="34820" class="Keyword">open</a> <a id="34825" class="Keyword">import</a> <a id="34832" href="set-theory.html" class="Module">set-theory</a>
<a id="34843" class="Keyword">open</a> <a id="34848" class="Keyword">import</a> <a id="34855" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="34878" class="Keyword">open</a> <a id="34883" class="Keyword">import</a> <a id="34890" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="34914" class="Keyword">open</a> <a id="34919" class="Keyword">import</a> <a id="34926" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="34951" class="Keyword">open</a> <a id="34956" class="Keyword">import</a> <a id="34963" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="34989" class="Keyword">open</a> <a id="34994" class="Keyword">import</a> <a id="35001" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35063" class="Keyword">open</a> <a id="35068" class="Keyword">import</a> <a id="35075" href="structured-types.html" class="Module">structured-types</a>
<a id="35092" class="Keyword">open</a> <a id="35097" class="Keyword">import</a> <a id="35104" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35139" class="Keyword">open</a> <a id="35144" class="Keyword">import</a> <a id="35151" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35195" class="Keyword">open</a> <a id="35200" class="Keyword">import</a> <a id="35207" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="35271" class="Keyword">open</a> <a id="35276" class="Keyword">import</a> <a id="35283" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="35322" class="Keyword">open</a> <a id="35327" class="Keyword">import</a> <a id="35334" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="35380" class="Keyword">open</a> <a id="35385" class="Keyword">import</a> <a id="35392" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="35457" class="Keyword">open</a> <a id="35462" class="Keyword">import</a> <a id="35469" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="35493" class="Keyword">open</a> <a id="35498" class="Keyword">import</a> <a id="35505" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="35574" class="Keyword">open</a> <a id="35579" class="Keyword">import</a> <a id="35586" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="35631" class="Keyword">open</a> <a id="35636" class="Keyword">import</a> <a id="35643" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="35677" class="Keyword">open</a> <a id="35682" class="Keyword">import</a> <a id="35689" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="35750" class="Keyword">open</a> <a id="35755" class="Keyword">import</a> <a id="35762" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="35807" class="Keyword">open</a> <a id="35812" class="Keyword">import</a> <a id="35819" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="35857" class="Keyword">open</a> <a id="35862" class="Keyword">import</a> <a id="35869" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="35912" class="Keyword">open</a> <a id="35917" class="Keyword">import</a> <a id="35924" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="35960" class="Keyword">open</a> <a id="35965" class="Keyword">import</a> <a id="35972" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36002" class="Keyword">open</a> <a id="36007" class="Keyword">import</a> <a id="36014" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36048" class="Keyword">open</a> <a id="36053" class="Keyword">import</a> <a id="36060" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36091" class="Keyword">open</a> <a id="36096" class="Keyword">import</a> <a id="36103" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36162" class="Keyword">open</a> <a id="36167" class="Keyword">import</a> <a id="36174" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="36225" class="Keyword">open</a> <a id="36230" class="Keyword">import</a> <a id="36237" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="36288" class="Keyword">open</a> <a id="36293" class="Keyword">import</a> <a id="36300" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="36355" class="Keyword">open</a> <a id="36360" class="Keyword">import</a> <a id="36367" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="36399" class="Keyword">open</a> <a id="36404" class="Keyword">import</a> <a id="36411" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="36440" class="Keyword">open</a> <a id="36445" class="Keyword">import</a> <a id="36452" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="36480" class="Keyword">open</a> <a id="36485" class="Keyword">import</a> <a id="36492" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="36522" class="Keyword">open</a> <a id="36527" class="Keyword">import</a> <a id="36534" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="36568" class="Keyword">open</a> <a id="36573" class="Keyword">import</a> <a id="36580" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="36656" class="Keyword">open</a> <a id="36661" class="Keyword">import</a> <a id="36668" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="36694" class="Keyword">open</a> <a id="36699" class="Keyword">import</a> <a id="36706" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="36744" class="Keyword">open</a> <a id="36749" class="Keyword">import</a> <a id="36756" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="36793" class="Keyword">open</a> <a id="36798" class="Keyword">import</a> <a id="36805" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="36845" class="Keyword">open</a> <a id="36850" class="Keyword">import</a> <a id="36857" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="36896" class="Keyword">open</a> <a id="36901" class="Keyword">import</a> <a id="36908" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="36941" class="Keyword">open</a> <a id="36946" class="Keyword">import</a> <a id="36953" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="36996" class="Keyword">open</a> <a id="37001" class="Keyword">import</a> <a id="37008" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37043" class="Keyword">open</a> <a id="37048" class="Keyword">import</a> <a id="37055" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37100" class="Keyword">open</a> <a id="37105" class="Keyword">import</a> <a id="37112" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37149" class="Keyword">open</a> <a id="37154" class="Keyword">import</a> <a id="37161" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37213" class="Keyword">open</a> <a id="37218" class="Keyword">import</a> <a id="37225" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="37278" class="Keyword">open</a> <a id="37283" class="Keyword">import</a> <a id="37290" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="37350" class="Keyword">open</a> <a id="37355" class="Keyword">import</a> <a id="37362" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="37410" class="Keyword">open</a> <a id="37415" class="Keyword">import</a> <a id="37422" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="37462" class="Keyword">open</a> <a id="37467" class="Keyword">import</a> <a id="37474" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="37521" class="Keyword">open</a> <a id="37526" class="Keyword">import</a> <a id="37533" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="37574" class="Keyword">open</a> <a id="37579" class="Keyword">import</a> <a id="37586" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="37624" class="Keyword">open</a> <a id="37629" class="Keyword">import</a> <a id="37636" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="37684" class="Keyword">open</a> <a id="37689" class="Keyword">import</a> <a id="37696" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="37733" class="Keyword">open</a> <a id="37738" class="Keyword">import</a> <a id="37745" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="37780" class="Keyword">open</a> <a id="37785" class="Keyword">import</a> <a id="37792" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="37826" class="Keyword">open</a> <a id="37831" class="Keyword">import</a> <a id="37838" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="37885" class="Keyword">open</a> <a id="37890" class="Keyword">import</a> <a id="37897" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="37942" class="Keyword">open</a> <a id="37947" class="Keyword">import</a> <a id="37954" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38003" class="Keyword">open</a> <a id="38008" class="Keyword">import</a> <a id="38015" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38067" class="Keyword">open</a> <a id="38072" class="Keyword">import</a> <a id="38079" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38133" class="Keyword">open</a> <a id="38138" class="Keyword">import</a> <a id="38145" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="38222" class="Keyword">open</a> <a id="38227" class="Keyword">import</a> <a id="38234" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="38286" class="Keyword">open</a> <a id="38291" class="Keyword">import</a> <a id="38298" href="type-theories.html" class="Module">type-theories</a>
<a id="38312" class="Keyword">open</a> <a id="38317" class="Keyword">import</a> <a id="38324" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="38366" class="Keyword">open</a> <a id="38371" class="Keyword">import</a> <a id="38378" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="38416" class="Keyword">open</a> <a id="38421" class="Keyword">import</a> <a id="38428" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="38474" class="Keyword">open</a> <a id="38479" class="Keyword">import</a> <a id="38486" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="38533" class="Keyword">open</a> <a id="38538" class="Keyword">import</a> <a id="38545" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="38580" class="Keyword">open</a> <a id="38585" class="Keyword">import</a> <a id="38592" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="38670" class="Keyword">open</a> <a id="38675" class="Keyword">import</a> <a id="38682" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="38706" class="Keyword">open</a> <a id="38711" class="Keyword">import</a> <a id="38718" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="38771" class="Keyword">open</a> <a id="38776" class="Keyword">import</a> <a id="38783" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="38826" class="Keyword">open</a> <a id="38831" class="Keyword">import</a> <a id="38838" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="38878" class="Keyword">open</a> <a id="38883" class="Keyword">import</a> <a id="38890" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="38929" class="Keyword">open</a> <a id="38934" class="Keyword">import</a> <a id="38941" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="38975" class="Keyword">open</a> <a id="38980" class="Keyword">import</a> <a id="38987" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39035" class="Keyword">open</a> <a id="39040" class="Keyword">import</a> <a id="39047" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39098" class="Keyword">open</a> <a id="39103" class="Keyword">import</a> <a id="39110" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39157" class="Keyword">open</a> <a id="39162" class="Keyword">import</a> <a id="39169" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39221" class="Keyword">open</a> <a id="39226" class="Keyword">import</a> <a id="39233" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39277" class="Keyword">open</a> <a id="39282" class="Keyword">import</a> <a id="39289" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="39329" class="Keyword">open</a> <a id="39334" class="Keyword">import</a> <a id="39341" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="39384" class="Keyword">open</a> <a id="39389" class="Keyword">import</a> <a id="39396" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="39448" class="Keyword">open</a> <a id="39453" class="Keyword">import</a> <a id="39460" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="39514" class="Keyword">open</a> <a id="39519" class="Keyword">import</a> <a id="39526" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="39574" class="Keyword">open</a> <a id="39579" class="Keyword">import</a> <a id="39586" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="39625" class="Keyword">open</a> <a id="39630" class="Keyword">import</a> <a id="39637" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="39670" class="Keyword">open</a> <a id="39675" class="Keyword">import</a> <a id="39682" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="39712" class="Keyword">open</a> <a id="39717" class="Keyword">import</a> <a id="39724" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="39775" class="Keyword">open</a> <a id="39780" class="Keyword">import</a> <a id="39787" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="39828" class="Keyword">open</a> <a id="39833" class="Keyword">import</a> <a id="39840" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="39877" class="Keyword">open</a> <a id="39882" class="Keyword">import</a> <a id="39889" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="39948" class="Keyword">open</a> <a id="39953" class="Keyword">import</a> <a id="39960" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40015" class="Keyword">open</a> <a id="40020" class="Keyword">import</a> <a id="40027" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40083" class="Keyword">open</a> <a id="40088" class="Keyword">import</a> <a id="40095" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40142" class="Keyword">open</a> <a id="40147" class="Keyword">import</a> <a id="40154" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40197" class="Keyword">open</a> <a id="40202" class="Keyword">import</a> <a id="40209" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40254" class="Keyword">open</a> <a id="40259" class="Keyword">import</a> <a id="40266" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="40315" class="Keyword">open</a> <a id="40320" class="Keyword">import</a> <a id="40327" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="40378" class="Keyword">open</a> <a id="40383" class="Keyword">import</a> <a id="40390" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="40434" class="Keyword">open</a> <a id="40439" class="Keyword">import</a> <a id="40446" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="40524" class="Keyword">open</a> <a id="40529" class="Keyword">import</a> <a id="40536" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="40576" class="Keyword">open</a> <a id="40581" class="Keyword">import</a> <a id="40588" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="40645" class="Keyword">open</a> <a id="40650" class="Keyword">import</a> <a id="40657" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="40692" class="Keyword">open</a> <a id="40697" class="Keyword">import</a> <a id="40704" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="40750" class="Keyword">open</a> <a id="40755" class="Keyword">import</a> <a id="40762" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="40817" class="Keyword">open</a> <a id="40822" class="Keyword">import</a> <a id="40829" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="40872" class="Keyword">open</a> <a id="40877" class="Keyword">import</a> <a id="40884" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="40929" class="Keyword">open</a> <a id="40934" class="Keyword">import</a> <a id="40941" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41000" class="Keyword">open</a> <a id="41005" class="Keyword">import</a> <a id="41012" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41049" class="Keyword">open</a> <a id="41054" class="Keyword">import</a> <a id="41061" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41103" class="Keyword">open</a> <a id="41108" class="Keyword">import</a> <a id="41115" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41156" class="Keyword">open</a> <a id="41161" class="Keyword">import</a> <a id="41168" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41207" class="Keyword">open</a> <a id="41212" class="Keyword">import</a> <a id="41219" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41257" class="Keyword">open</a> <a id="41262" class="Keyword">import</a> <a id="41269" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="41321" class="Keyword">open</a> <a id="41326" class="Keyword">import</a> <a id="41333" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="41378" class="Keyword">open</a> <a id="41383" class="Keyword">import</a> <a id="41390" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="41429" class="Keyword">open</a> <a id="41434" class="Keyword">import</a> <a id="41441" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="41478" class="Keyword">open</a> <a id="41483" class="Keyword">import</a> <a id="41490" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="41539" class="Keyword">open</a> <a id="41544" class="Keyword">import</a> <a id="41551" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="41590" class="Keyword">open</a> <a id="41595" class="Keyword">import</a> <a id="41602" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="41640" class="Keyword">open</a> <a id="41645" class="Keyword">import</a> <a id="41652" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="41707" class="Keyword">open</a> <a id="41712" class="Keyword">import</a> <a id="41719" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="41758" class="Keyword">open</a> <a id="41763" class="Keyword">import</a> <a id="41770" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="41818" class="Keyword">open</a> <a id="41823" class="Keyword">import</a> <a id="41830" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="41877" class="Keyword">open</a> <a id="41882" class="Keyword">import</a> <a id="41889" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="41927" class="Keyword">open</a> <a id="41932" class="Keyword">import</a> <a id="41939" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="41969" class="Keyword">open</a> <a id="41974" class="Keyword">import</a> <a id="41981" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42038" class="Keyword">open</a> <a id="42043" class="Keyword">import</a> <a id="42050" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42104" class="Keyword">open</a> <a id="42109" class="Keyword">import</a> <a id="42116" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42146" class="Keyword">open</a> <a id="42151" class="Keyword">import</a> <a id="42158" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42207" class="Keyword">open</a> <a id="42212" class="Keyword">import</a> <a id="42219" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42261" class="Keyword">open</a> <a id="42266" class="Keyword">import</a> <a id="42273" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="42307" class="Keyword">open</a> <a id="42312" class="Keyword">import</a> <a id="42319" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="42382" class="Keyword">open</a> <a id="42387" class="Keyword">import</a> <a id="42394" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="42437" class="Keyword">open</a> <a id="42442" class="Keyword">import</a> <a id="42449" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="42484" class="Keyword">open</a> <a id="42489" class="Keyword">import</a> <a id="42496" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="42531" class="Keyword">open</a> <a id="42536" class="Keyword">import</a> <a id="42543" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="42583" class="Keyword">open</a> <a id="42588" class="Keyword">import</a> <a id="42595" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="42640" class="Keyword">open</a> <a id="42645" class="Keyword">import</a> <a id="42652" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="42693" class="Keyword">open</a> <a id="42698" class="Keyword">import</a> <a id="42705" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="42759" class="Keyword">open</a> <a id="42764" class="Keyword">import</a> <a id="42771" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="42821" class="Keyword">open</a> <a id="42826" class="Keyword">import</a> <a id="42833" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="42880" class="Keyword">open</a> <a id="42885" class="Keyword">import</a> <a id="42892" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="42930" class="Keyword">open</a> <a id="42935" class="Keyword">import</a> <a id="42942" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="42991" class="Keyword">open</a> <a id="42996" class="Keyword">import</a> <a id="43003" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43050" class="Keyword">open</a> <a id="43055" class="Keyword">import</a> <a id="43062" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43125" class="Keyword">open</a> <a id="43130" class="Keyword">import</a> <a id="43137" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43169" class="Keyword">open</a> <a id="43174" class="Keyword">import</a> <a id="43181" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43234" class="Keyword">open</a> <a id="43239" class="Keyword">import</a> <a id="43246" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="43292" class="Keyword">open</a> <a id="43297" class="Keyword">import</a> <a id="43304" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="43350" class="Keyword">open</a> <a id="43355" class="Keyword">import</a> <a id="43362" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="43402" class="Keyword">open</a> <a id="43407" class="Keyword">import</a> <a id="43414" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="43461" class="Keyword">open</a> <a id="43466" class="Keyword">import</a> <a id="43473" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="43521" class="Keyword">open</a> <a id="43526" class="Keyword">import</a> <a id="43533" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="43573" class="Keyword">open</a> <a id="43578" class="Keyword">import</a> <a id="43585" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="43630" class="Keyword">open</a> <a id="43635" class="Keyword">import</a> <a id="43642" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="43707" class="Keyword">open</a> <a id="43712" class="Keyword">import</a> <a id="43719" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="43764" class="Keyword">open</a> <a id="43769" class="Keyword">import</a> <a id="43776" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="43823" class="Keyword">open</a> <a id="43828" class="Keyword">import</a> <a id="43835" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="43888" class="Keyword">open</a> <a id="43893" class="Keyword">import</a> <a id="43900" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>