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
<a id="27175" class="Keyword">open</a> <a id="27180" class="Keyword">import</a> <a id="27187" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27212" class="Keyword">open</a> <a id="27217" class="Keyword">import</a> <a id="27224" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27286" class="Keyword">open</a> <a id="27291" class="Keyword">import</a> <a id="27298" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27339" class="Keyword">open</a> <a id="27344" class="Keyword">import</a> <a id="27351" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27380" class="Keyword">open</a> <a id="27385" class="Keyword">import</a> <a id="27392" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27416" class="Keyword">open</a> <a id="27421" class="Keyword">import</a> <a id="27428" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27459" class="Keyword">open</a> <a id="27464" class="Keyword">import</a> <a id="27471" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27518" class="Keyword">open</a> <a id="27523" class="Keyword">import</a> <a id="27530" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="27563" class="Keyword">open</a> <a id="27568" class="Keyword">import</a> <a id="27575" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="27624" class="Keyword">open</a> <a id="27629" class="Keyword">import</a> <a id="27636" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="27676" class="Keyword">open</a> <a id="27681" class="Keyword">import</a> <a id="27688" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="27728" class="Keyword">open</a> <a id="27733" class="Keyword">import</a> <a id="27740" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="27777" class="Keyword">open</a> <a id="27782" class="Keyword">import</a> <a id="27789" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="27836" class="Keyword">open</a> <a id="27841" class="Keyword">import</a> <a id="27848" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="27889" class="Keyword">open</a> <a id="27894" class="Keyword">import</a> <a id="27901" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="27945" class="Keyword">open</a> <a id="27950" class="Keyword">import</a> <a id="27957" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="27996" class="Keyword">open</a> <a id="28001" class="Keyword">import</a> <a id="28008" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28040" class="Keyword">open</a> <a id="28045" class="Keyword">import</a> <a id="28052" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28079" class="Keyword">open</a> <a id="28084" class="Keyword">import</a> <a id="28091" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28111" class="Keyword">open</a> <a id="28116" class="Keyword">import</a> <a id="28123" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28157" class="Keyword">open</a> <a id="28162" class="Keyword">import</a> <a id="28169" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28196" class="Keyword">open</a> <a id="28201" class="Keyword">import</a> <a id="28208" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28250" class="Keyword">open</a> <a id="28255" class="Keyword">import</a> <a id="28262" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28312" class="Keyword">open</a> <a id="28317" class="Keyword">import</a> <a id="28324" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28371" class="Keyword">open</a> <a id="28376" class="Keyword">import</a> <a id="28383" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28424" class="Keyword">open</a> <a id="28429" class="Keyword">import</a> <a id="28436" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28470" class="Keyword">open</a> <a id="28475" class="Keyword">import</a> <a id="28482" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="28530" class="Keyword">open</a> <a id="28535" class="Keyword">import</a> <a id="28542" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="28583" class="Keyword">open</a> <a id="28588" class="Keyword">import</a> <a id="28595" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="28630" class="Keyword">open</a> <a id="28635" class="Keyword">import</a> <a id="28642" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="28680" class="Keyword">open</a> <a id="28685" class="Keyword">import</a> <a id="28692" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="28727" class="Keyword">open</a> <a id="28732" class="Keyword">import</a> <a id="28739" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="28771" class="Keyword">open</a> <a id="28776" class="Keyword">import</a> <a id="28783" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="28824" class="Keyword">open</a> <a id="28829" class="Keyword">import</a> <a id="28836" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="28877" class="Keyword">open</a> <a id="28882" class="Keyword">import</a> <a id="28889" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="28929" class="Keyword">open</a> <a id="28934" class="Keyword">import</a> <a id="28941" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="28974" class="Keyword">open</a> <a id="28979" class="Keyword">import</a> <a id="28986" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29023" class="Keyword">open</a> <a id="29028" class="Keyword">import</a> <a id="29035" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29065" class="Keyword">open</a> <a id="29070" class="Keyword">import</a> <a id="29077" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29098" class="Keyword">open</a> <a id="29103" class="Keyword">import</a> <a id="29110" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29164" class="Keyword">open</a> <a id="29169" class="Keyword">import</a> <a id="29176" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29221" class="Keyword">open</a> <a id="29226" class="Keyword">import</a> <a id="29233" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29261" class="Keyword">open</a> <a id="29266" class="Keyword">import</a> <a id="29273" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29294" class="Keyword">open</a> <a id="29299" class="Keyword">import</a> <a id="29306" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29349" class="Keyword">open</a> <a id="29354" class="Keyword">import</a> <a id="29361" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29395" class="Keyword">open</a> <a id="29400" class="Keyword">import</a> <a id="29407" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29437" class="Keyword">open</a> <a id="29442" class="Keyword">import</a> <a id="29449" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29495" class="Keyword">open</a> <a id="29500" class="Keyword">import</a> <a id="29507" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="29561" class="Keyword">open</a> <a id="29566" class="Keyword">import</a> <a id="29573" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="29616" class="Keyword">open</a> <a id="29621" class="Keyword">import</a> <a id="29628" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="29662" class="Keyword">open</a> <a id="29667" class="Keyword">import</a> <a id="29674" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="29715" class="Keyword">open</a> <a id="29720" class="Keyword">import</a> <a id="29727" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="29762" class="Keyword">open</a> <a id="29767" class="Keyword">import</a> <a id="29774" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a>
<a id="29813" class="Keyword">open</a> <a id="29818" class="Keyword">import</a> <a id="29825" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="29867" class="Keyword">open</a> <a id="29872" class="Keyword">import</a> <a id="29879" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="29914" class="Keyword">open</a> <a id="29919" class="Keyword">import</a> <a id="29926" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="29965" class="Keyword">open</a> <a id="29970" class="Keyword">import</a> <a id="29977" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="30014" class="Keyword">open</a> <a id="30019" class="Keyword">import</a> <a id="30026" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30073" class="Keyword">open</a> <a id="30078" class="Keyword">import</a> <a id="30085" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30149" class="Keyword">open</a> <a id="30154" class="Keyword">import</a> <a id="30161" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30206" class="Keyword">open</a> <a id="30211" class="Keyword">import</a> <a id="30218" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30242" class="Keyword">open</a> <a id="30247" class="Keyword">import</a> <a id="30254" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30279" class="Keyword">open</a> <a id="30284" class="Keyword">import</a> <a id="30291" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30334" class="Keyword">open</a> <a id="30339" class="Keyword">import</a> <a id="30346" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30377" class="Keyword">open</a> <a id="30382" class="Keyword">import</a> <a id="30389" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30443" class="Keyword">open</a> <a id="30448" class="Keyword">import</a> <a id="30455" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30478" class="Keyword">open</a> <a id="30483" class="Keyword">import</a> <a id="30490" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="30528" class="Keyword">open</a> <a id="30533" class="Keyword">import</a> <a id="30540" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="30579" class="Keyword">open</a> <a id="30584" class="Keyword">import</a> <a id="30591" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="30642" class="Keyword">open</a> <a id="30647" class="Keyword">import</a> <a id="30654" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="30691" class="Keyword">open</a> <a id="30696" class="Keyword">import</a> <a id="30703" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="30727" class="Keyword">open</a> <a id="30732" class="Keyword">import</a> <a id="30739" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="30766" class="Keyword">open</a> <a id="30771" class="Keyword">import</a> <a id="30778" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="30835" class="Keyword">open</a> <a id="30840" class="Keyword">import</a> <a id="30847" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="30895" class="Keyword">open</a> <a id="30900" class="Keyword">import</a> <a id="30907" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="30937" class="Keyword">open</a> <a id="30942" class="Keyword">import</a> <a id="30949" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="30986" class="Keyword">open</a> <a id="30991" class="Keyword">import</a> <a id="30998" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="31019" class="Keyword">open</a> <a id="31024" class="Keyword">import</a> <a id="31031" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31078" class="Keyword">open</a> <a id="31083" class="Keyword">import</a> <a id="31090" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31128" class="Keyword">open</a> <a id="31133" class="Keyword">import</a> <a id="31140" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31234" class="Keyword">open</a> <a id="31239" class="Keyword">import</a> <a id="31246" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31261" class="Keyword">open</a> <a id="31266" class="Keyword">import</a> <a id="31273" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31306" class="Keyword">open</a> <a id="31311" class="Keyword">import</a> <a id="31318" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="31350" class="Keyword">open</a> <a id="31355" class="Keyword">import</a> <a id="31362" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="31404" class="Keyword">open</a> <a id="31409" class="Keyword">import</a> <a id="31416" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="31454" class="Keyword">open</a> <a id="31459" class="Keyword">import</a> <a id="31466" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="31503" class="Keyword">open</a> <a id="31508" class="Keyword">import</a> <a id="31515" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="31548" class="Keyword">open</a> <a id="31553" class="Keyword">import</a> <a id="31560" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="31584" class="Keyword">open</a> <a id="31589" class="Keyword">import</a> <a id="31596" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="31635" class="Keyword">open</a> <a id="31640" class="Keyword">import</a> <a id="31647" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="31693" class="Keyword">open</a> <a id="31698" class="Keyword">import</a> <a id="31705" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="31750" class="Keyword">open</a> <a id="31755" class="Keyword">import</a> <a id="31762" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="31800" class="Keyword">open</a> <a id="31805" class="Keyword">import</a> <a id="31812" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="31844" class="Keyword">open</a> <a id="31849" class="Keyword">import</a> <a id="31856" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="31909" class="Keyword">open</a> <a id="31914" class="Keyword">import</a> <a id="31921" href="order-theory.html" class="Module">order-theory</a>
<a id="31934" class="Keyword">open</a> <a id="31939" class="Keyword">import</a> <a id="31946" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="31973" class="Keyword">open</a> <a id="31978" class="Keyword">import</a> <a id="31985" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="32015" class="Keyword">open</a> <a id="32020" class="Keyword">import</a> <a id="32027" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32060" class="Keyword">open</a> <a id="32065" class="Keyword">import</a> <a id="32072" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32108" class="Keyword">open</a> <a id="32113" class="Keyword">import</a> <a id="32120" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32155" class="Keyword">open</a> <a id="32160" class="Keyword">import</a> <a id="32167" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32194" class="Keyword">open</a> <a id="32199" class="Keyword">import</a> <a id="32206" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32236" class="Keyword">open</a> <a id="32241" class="Keyword">import</a> <a id="32248" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32284" class="Keyword">open</a> <a id="32289" class="Keyword">import</a> <a id="32296" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="32338" class="Keyword">open</a> <a id="32343" class="Keyword">import</a> <a id="32350" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32380" class="Keyword">open</a> <a id="32385" class="Keyword">import</a> <a id="32392" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="32424" class="Keyword">open</a> <a id="32429" class="Keyword">import</a> <a id="32436" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="32467" class="Keyword">open</a> <a id="32472" class="Keyword">import</a> <a id="32479" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="32505" class="Keyword">open</a> <a id="32510" class="Keyword">import</a> <a id="32517" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="32546" class="Keyword">open</a> <a id="32551" class="Keyword">import</a> <a id="32558" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="32595" class="Keyword">open</a> <a id="32600" class="Keyword">import</a> <a id="32607" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="32647" class="Keyword">open</a> <a id="32652" class="Keyword">import</a> <a id="32659" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="32681" class="Keyword">open</a> <a id="32686" class="Keyword">import</a> <a id="32693" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="32728" class="Keyword">open</a> <a id="32733" class="Keyword">import</a> <a id="32740" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="32778" class="Keyword">open</a> <a id="32783" class="Keyword">import</a> <a id="32790" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="32829" class="Keyword">open</a> <a id="32834" class="Keyword">import</a> <a id="32841" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="32876" class="Keyword">open</a> <a id="32881" class="Keyword">import</a> <a id="32888" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="32923" class="Keyword">open</a> <a id="32928" class="Keyword">import</a> <a id="32935" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="32970" class="Keyword">open</a> <a id="32975" class="Keyword">import</a> <a id="32982" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="33020" class="Keyword">open</a> <a id="33025" class="Keyword">import</a> <a id="33032" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33063" class="Keyword">open</a> <a id="33068" class="Keyword">import</a> <a id="33075" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33117" class="Keyword">open</a> <a id="33122" class="Keyword">import</a> <a id="33129" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33174" class="Keyword">open</a> <a id="33179" class="Keyword">import</a> <a id="33186" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33219" class="Keyword">open</a> <a id="33224" class="Keyword">import</a> <a id="33231" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33251" class="Keyword">open</a> <a id="33256" class="Keyword">import</a> <a id="33263" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33286" class="Keyword">open</a> <a id="33291" class="Keyword">import</a> <a id="33298" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="33321" class="Keyword">open</a> <a id="33326" class="Keyword">import</a> <a id="33333" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33359" class="Keyword">open</a> <a id="33364" class="Keyword">import</a> <a id="33371" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33397" class="Keyword">open</a> <a id="33402" class="Keyword">import</a> <a id="33409" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="33473" class="Keyword">open</a> <a id="33478" class="Keyword">import</a> <a id="33485" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="33503" class="Keyword">open</a> <a id="33508" class="Keyword">import</a> <a id="33515" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="33542" class="Keyword">open</a> <a id="33547" class="Keyword">import</a> <a id="33554" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="33580" class="Keyword">open</a> <a id="33585" class="Keyword">import</a> <a id="33592" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="33618" class="Keyword">open</a> <a id="33623" class="Keyword">import</a> <a id="33630" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="33656" class="Keyword">open</a> <a id="33661" class="Keyword">import</a> <a id="33668" href="organic-chemistry.ethane.html" class="Module">organic-chemistry.ethane</a>
<a id="33693" class="Keyword">open</a> <a id="33698" class="Keyword">import</a> <a id="33705" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="33736" class="Keyword">open</a> <a id="33741" class="Keyword">import</a> <a id="33748" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="33774" class="Keyword">open</a> <a id="33779" class="Keyword">import</a> <a id="33786" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="33849" class="Keyword">open</a> <a id="33854" class="Keyword">import</a> <a id="33861" href="polytopes.html" class="Module">polytopes</a>
<a id="33871" class="Keyword">open</a> <a id="33876" class="Keyword">import</a> <a id="33883" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="33941" class="Keyword">open</a> <a id="33946" class="Keyword">import</a> <a id="33953" href="ring-theory.html" class="Module">ring-theory</a>
<a id="33965" class="Keyword">open</a> <a id="33970" class="Keyword">import</a> <a id="33977" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="34014" class="Keyword">open</a> <a id="34019" class="Keyword">import</a> <a id="34026" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="34053" class="Keyword">open</a> <a id="34058" class="Keyword">import</a> <a id="34065" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34097" class="Keyword">open</a> <a id="34102" class="Keyword">import</a> <a id="34109" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34155" class="Keyword">open</a> <a id="34160" class="Keyword">import</a> <a id="34167" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34192" class="Keyword">open</a> <a id="34197" class="Keyword">import</a> <a id="34204" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34242" class="Keyword">open</a> <a id="34247" class="Keyword">import</a> <a id="34254" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34297" class="Keyword">open</a> <a id="34302" class="Keyword">import</a> <a id="34309" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="34347" class="Keyword">open</a> <a id="34352" class="Keyword">import</a> <a id="34359" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="34390" class="Keyword">open</a> <a id="34395" class="Keyword">import</a> <a id="34402" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="34426" class="Keyword">open</a> <a id="34431" class="Keyword">import</a> <a id="34438" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="34470" class="Keyword">open</a> <a id="34475" class="Keyword">import</a> <a id="34482" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="34508" class="Keyword">open</a> <a id="34513" class="Keyword">import</a> <a id="34520" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="34549" class="Keyword">open</a> <a id="34554" class="Keyword">import</a> <a id="34561" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="34598" class="Keyword">open</a> <a id="34603" class="Keyword">import</a> <a id="34610" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="34639" class="Keyword">open</a> <a id="34644" class="Keyword">import</a> <a id="34651" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="34678" class="Keyword">open</a> <a id="34683" class="Keyword">import</a> <a id="34690" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="34727" class="Keyword">open</a> <a id="34732" class="Keyword">import</a> <a id="34739" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="34766" class="Keyword">open</a> <a id="34771" class="Keyword">import</a> <a id="34778" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="34811" class="Keyword">open</a> <a id="34816" class="Keyword">import</a> <a id="34823" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="34841" class="Keyword">open</a> <a id="34846" class="Keyword">import</a> <a id="34853" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="34907" class="Keyword">open</a> <a id="34912" class="Keyword">import</a> <a id="34919" href="set-theory.html" class="Module">set-theory</a>
<a id="34930" class="Keyword">open</a> <a id="34935" class="Keyword">import</a> <a id="34942" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="34965" class="Keyword">open</a> <a id="34970" class="Keyword">import</a> <a id="34977" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="35001" class="Keyword">open</a> <a id="35006" class="Keyword">import</a> <a id="35013" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="35038" class="Keyword">open</a> <a id="35043" class="Keyword">import</a> <a id="35050" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="35076" class="Keyword">open</a> <a id="35081" class="Keyword">import</a> <a id="35088" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35150" class="Keyword">open</a> <a id="35155" class="Keyword">import</a> <a id="35162" href="structured-types.html" class="Module">structured-types</a>
<a id="35179" class="Keyword">open</a> <a id="35184" class="Keyword">import</a> <a id="35191" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35226" class="Keyword">open</a> <a id="35231" class="Keyword">import</a> <a id="35238" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35282" class="Keyword">open</a> <a id="35287" class="Keyword">import</a> <a id="35294" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="35358" class="Keyword">open</a> <a id="35363" class="Keyword">import</a> <a id="35370" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="35409" class="Keyword">open</a> <a id="35414" class="Keyword">import</a> <a id="35421" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="35467" class="Keyword">open</a> <a id="35472" class="Keyword">import</a> <a id="35479" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="35544" class="Keyword">open</a> <a id="35549" class="Keyword">import</a> <a id="35556" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="35580" class="Keyword">open</a> <a id="35585" class="Keyword">import</a> <a id="35592" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="35661" class="Keyword">open</a> <a id="35666" class="Keyword">import</a> <a id="35673" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="35718" class="Keyword">open</a> <a id="35723" class="Keyword">import</a> <a id="35730" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="35764" class="Keyword">open</a> <a id="35769" class="Keyword">import</a> <a id="35776" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="35837" class="Keyword">open</a> <a id="35842" class="Keyword">import</a> <a id="35849" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="35894" class="Keyword">open</a> <a id="35899" class="Keyword">import</a> <a id="35906" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="35944" class="Keyword">open</a> <a id="35949" class="Keyword">import</a> <a id="35956" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="35999" class="Keyword">open</a> <a id="36004" class="Keyword">import</a> <a id="36011" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="36047" class="Keyword">open</a> <a id="36052" class="Keyword">import</a> <a id="36059" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36089" class="Keyword">open</a> <a id="36094" class="Keyword">import</a> <a id="36101" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36135" class="Keyword">open</a> <a id="36140" class="Keyword">import</a> <a id="36147" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36178" class="Keyword">open</a> <a id="36183" class="Keyword">import</a> <a id="36190" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36249" class="Keyword">open</a> <a id="36254" class="Keyword">import</a> <a id="36261" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="36312" class="Keyword">open</a> <a id="36317" class="Keyword">import</a> <a id="36324" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="36375" class="Keyword">open</a> <a id="36380" class="Keyword">import</a> <a id="36387" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="36442" class="Keyword">open</a> <a id="36447" class="Keyword">import</a> <a id="36454" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="36486" class="Keyword">open</a> <a id="36491" class="Keyword">import</a> <a id="36498" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="36527" class="Keyword">open</a> <a id="36532" class="Keyword">import</a> <a id="36539" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="36567" class="Keyword">open</a> <a id="36572" class="Keyword">import</a> <a id="36579" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="36609" class="Keyword">open</a> <a id="36614" class="Keyword">import</a> <a id="36621" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="36655" class="Keyword">open</a> <a id="36660" class="Keyword">import</a> <a id="36667" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="36743" class="Keyword">open</a> <a id="36748" class="Keyword">import</a> <a id="36755" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="36781" class="Keyword">open</a> <a id="36786" class="Keyword">import</a> <a id="36793" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="36831" class="Keyword">open</a> <a id="36836" class="Keyword">import</a> <a id="36843" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="36880" class="Keyword">open</a> <a id="36885" class="Keyword">import</a> <a id="36892" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="36932" class="Keyword">open</a> <a id="36937" class="Keyword">import</a> <a id="36944" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="36983" class="Keyword">open</a> <a id="36988" class="Keyword">import</a> <a id="36995" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="37028" class="Keyword">open</a> <a id="37033" class="Keyword">import</a> <a id="37040" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="37083" class="Keyword">open</a> <a id="37088" class="Keyword">import</a> <a id="37095" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37130" class="Keyword">open</a> <a id="37135" class="Keyword">import</a> <a id="37142" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37187" class="Keyword">open</a> <a id="37192" class="Keyword">import</a> <a id="37199" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37236" class="Keyword">open</a> <a id="37241" class="Keyword">import</a> <a id="37248" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37300" class="Keyword">open</a> <a id="37305" class="Keyword">import</a> <a id="37312" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="37365" class="Keyword">open</a> <a id="37370" class="Keyword">import</a> <a id="37377" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="37437" class="Keyword">open</a> <a id="37442" class="Keyword">import</a> <a id="37449" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="37497" class="Keyword">open</a> <a id="37502" class="Keyword">import</a> <a id="37509" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="37549" class="Keyword">open</a> <a id="37554" class="Keyword">import</a> <a id="37561" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="37608" class="Keyword">open</a> <a id="37613" class="Keyword">import</a> <a id="37620" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="37661" class="Keyword">open</a> <a id="37666" class="Keyword">import</a> <a id="37673" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="37711" class="Keyword">open</a> <a id="37716" class="Keyword">import</a> <a id="37723" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="37771" class="Keyword">open</a> <a id="37776" class="Keyword">import</a> <a id="37783" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="37820" class="Keyword">open</a> <a id="37825" class="Keyword">import</a> <a id="37832" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="37867" class="Keyword">open</a> <a id="37872" class="Keyword">import</a> <a id="37879" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="37913" class="Keyword">open</a> <a id="37918" class="Keyword">import</a> <a id="37925" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="37972" class="Keyword">open</a> <a id="37977" class="Keyword">import</a> <a id="37984" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="38029" class="Keyword">open</a> <a id="38034" class="Keyword">import</a> <a id="38041" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38090" class="Keyword">open</a> <a id="38095" class="Keyword">import</a> <a id="38102" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38154" class="Keyword">open</a> <a id="38159" class="Keyword">import</a> <a id="38166" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38220" class="Keyword">open</a> <a id="38225" class="Keyword">import</a> <a id="38232" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="38309" class="Keyword">open</a> <a id="38314" class="Keyword">import</a> <a id="38321" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="38373" class="Keyword">open</a> <a id="38378" class="Keyword">import</a> <a id="38385" href="type-theories.html" class="Module">type-theories</a>
<a id="38399" class="Keyword">open</a> <a id="38404" class="Keyword">import</a> <a id="38411" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="38453" class="Keyword">open</a> <a id="38458" class="Keyword">import</a> <a id="38465" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="38503" class="Keyword">open</a> <a id="38508" class="Keyword">import</a> <a id="38515" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="38561" class="Keyword">open</a> <a id="38566" class="Keyword">import</a> <a id="38573" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="38620" class="Keyword">open</a> <a id="38625" class="Keyword">import</a> <a id="38632" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="38667" class="Keyword">open</a> <a id="38672" class="Keyword">import</a> <a id="38679" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="38757" class="Keyword">open</a> <a id="38762" class="Keyword">import</a> <a id="38769" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="38793" class="Keyword">open</a> <a id="38798" class="Keyword">import</a> <a id="38805" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="38858" class="Keyword">open</a> <a id="38863" class="Keyword">import</a> <a id="38870" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="38913" class="Keyword">open</a> <a id="38918" class="Keyword">import</a> <a id="38925" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="38965" class="Keyword">open</a> <a id="38970" class="Keyword">import</a> <a id="38977" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="39016" class="Keyword">open</a> <a id="39021" class="Keyword">import</a> <a id="39028" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="39062" class="Keyword">open</a> <a id="39067" class="Keyword">import</a> <a id="39074" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39122" class="Keyword">open</a> <a id="39127" class="Keyword">import</a> <a id="39134" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39185" class="Keyword">open</a> <a id="39190" class="Keyword">import</a> <a id="39197" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39244" class="Keyword">open</a> <a id="39249" class="Keyword">import</a> <a id="39256" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39308" class="Keyword">open</a> <a id="39313" class="Keyword">import</a> <a id="39320" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39364" class="Keyword">open</a> <a id="39369" class="Keyword">import</a> <a id="39376" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="39416" class="Keyword">open</a> <a id="39421" class="Keyword">import</a> <a id="39428" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="39471" class="Keyword">open</a> <a id="39476" class="Keyword">import</a> <a id="39483" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="39535" class="Keyword">open</a> <a id="39540" class="Keyword">import</a> <a id="39547" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="39601" class="Keyword">open</a> <a id="39606" class="Keyword">import</a> <a id="39613" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="39661" class="Keyword">open</a> <a id="39666" class="Keyword">import</a> <a id="39673" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="39712" class="Keyword">open</a> <a id="39717" class="Keyword">import</a> <a id="39724" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="39757" class="Keyword">open</a> <a id="39762" class="Keyword">import</a> <a id="39769" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="39799" class="Keyword">open</a> <a id="39804" class="Keyword">import</a> <a id="39811" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="39862" class="Keyword">open</a> <a id="39867" class="Keyword">import</a> <a id="39874" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="39915" class="Keyword">open</a> <a id="39920" class="Keyword">import</a> <a id="39927" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="39964" class="Keyword">open</a> <a id="39969" class="Keyword">import</a> <a id="39976" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="40035" class="Keyword">open</a> <a id="40040" class="Keyword">import</a> <a id="40047" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40102" class="Keyword">open</a> <a id="40107" class="Keyword">import</a> <a id="40114" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40170" class="Keyword">open</a> <a id="40175" class="Keyword">import</a> <a id="40182" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40229" class="Keyword">open</a> <a id="40234" class="Keyword">import</a> <a id="40241" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40284" class="Keyword">open</a> <a id="40289" class="Keyword">import</a> <a id="40296" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40341" class="Keyword">open</a> <a id="40346" class="Keyword">import</a> <a id="40353" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="40402" class="Keyword">open</a> <a id="40407" class="Keyword">import</a> <a id="40414" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="40465" class="Keyword">open</a> <a id="40470" class="Keyword">import</a> <a id="40477" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="40521" class="Keyword">open</a> <a id="40526" class="Keyword">import</a> <a id="40533" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="40611" class="Keyword">open</a> <a id="40616" class="Keyword">import</a> <a id="40623" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="40663" class="Keyword">open</a> <a id="40668" class="Keyword">import</a> <a id="40675" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="40732" class="Keyword">open</a> <a id="40737" class="Keyword">import</a> <a id="40744" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="40779" class="Keyword">open</a> <a id="40784" class="Keyword">import</a> <a id="40791" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="40837" class="Keyword">open</a> <a id="40842" class="Keyword">import</a> <a id="40849" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="40904" class="Keyword">open</a> <a id="40909" class="Keyword">import</a> <a id="40916" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="40959" class="Keyword">open</a> <a id="40964" class="Keyword">import</a> <a id="40971" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="41016" class="Keyword">open</a> <a id="41021" class="Keyword">import</a> <a id="41028" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41087" class="Keyword">open</a> <a id="41092" class="Keyword">import</a> <a id="41099" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41136" class="Keyword">open</a> <a id="41141" class="Keyword">import</a> <a id="41148" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41190" class="Keyword">open</a> <a id="41195" class="Keyword">import</a> <a id="41202" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41243" class="Keyword">open</a> <a id="41248" class="Keyword">import</a> <a id="41255" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41294" class="Keyword">open</a> <a id="41299" class="Keyword">import</a> <a id="41306" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41344" class="Keyword">open</a> <a id="41349" class="Keyword">import</a> <a id="41356" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="41408" class="Keyword">open</a> <a id="41413" class="Keyword">import</a> <a id="41420" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="41465" class="Keyword">open</a> <a id="41470" class="Keyword">import</a> <a id="41477" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="41516" class="Keyword">open</a> <a id="41521" class="Keyword">import</a> <a id="41528" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="41565" class="Keyword">open</a> <a id="41570" class="Keyword">import</a> <a id="41577" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="41626" class="Keyword">open</a> <a id="41631" class="Keyword">import</a> <a id="41638" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="41677" class="Keyword">open</a> <a id="41682" class="Keyword">import</a> <a id="41689" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="41727" class="Keyword">open</a> <a id="41732" class="Keyword">import</a> <a id="41739" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="41794" class="Keyword">open</a> <a id="41799" class="Keyword">import</a> <a id="41806" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="41845" class="Keyword">open</a> <a id="41850" class="Keyword">import</a> <a id="41857" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="41905" class="Keyword">open</a> <a id="41910" class="Keyword">import</a> <a id="41917" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="41964" class="Keyword">open</a> <a id="41969" class="Keyword">import</a> <a id="41976" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="42014" class="Keyword">open</a> <a id="42019" class="Keyword">import</a> <a id="42026" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="42056" class="Keyword">open</a> <a id="42061" class="Keyword">import</a> <a id="42068" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42125" class="Keyword">open</a> <a id="42130" class="Keyword">import</a> <a id="42137" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42191" class="Keyword">open</a> <a id="42196" class="Keyword">import</a> <a id="42203" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42233" class="Keyword">open</a> <a id="42238" class="Keyword">import</a> <a id="42245" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42294" class="Keyword">open</a> <a id="42299" class="Keyword">import</a> <a id="42306" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42348" class="Keyword">open</a> <a id="42353" class="Keyword">import</a> <a id="42360" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="42394" class="Keyword">open</a> <a id="42399" class="Keyword">import</a> <a id="42406" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="42469" class="Keyword">open</a> <a id="42474" class="Keyword">import</a> <a id="42481" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="42524" class="Keyword">open</a> <a id="42529" class="Keyword">import</a> <a id="42536" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="42571" class="Keyword">open</a> <a id="42576" class="Keyword">import</a> <a id="42583" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="42618" class="Keyword">open</a> <a id="42623" class="Keyword">import</a> <a id="42630" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="42670" class="Keyword">open</a> <a id="42675" class="Keyword">import</a> <a id="42682" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="42727" class="Keyword">open</a> <a id="42732" class="Keyword">import</a> <a id="42739" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="42780" class="Keyword">open</a> <a id="42785" class="Keyword">import</a> <a id="42792" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="42846" class="Keyword">open</a> <a id="42851" class="Keyword">import</a> <a id="42858" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="42908" class="Keyword">open</a> <a id="42913" class="Keyword">import</a> <a id="42920" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="42967" class="Keyword">open</a> <a id="42972" class="Keyword">import</a> <a id="42979" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="43017" class="Keyword">open</a> <a id="43022" class="Keyword">import</a> <a id="43029" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="43078" class="Keyword">open</a> <a id="43083" class="Keyword">import</a> <a id="43090" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43137" class="Keyword">open</a> <a id="43142" class="Keyword">import</a> <a id="43149" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43212" class="Keyword">open</a> <a id="43217" class="Keyword">import</a> <a id="43224" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43256" class="Keyword">open</a> <a id="43261" class="Keyword">import</a> <a id="43268" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43321" class="Keyword">open</a> <a id="43326" class="Keyword">import</a> <a id="43333" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="43379" class="Keyword">open</a> <a id="43384" class="Keyword">import</a> <a id="43391" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="43437" class="Keyword">open</a> <a id="43442" class="Keyword">import</a> <a id="43449" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="43489" class="Keyword">open</a> <a id="43494" class="Keyword">import</a> <a id="43501" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="43548" class="Keyword">open</a> <a id="43553" class="Keyword">import</a> <a id="43560" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="43608" class="Keyword">open</a> <a id="43613" class="Keyword">import</a> <a id="43620" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="43660" class="Keyword">open</a> <a id="43665" class="Keyword">import</a> <a id="43672" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="43717" class="Keyword">open</a> <a id="43722" class="Keyword">import</a> <a id="43729" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="43794" class="Keyword">open</a> <a id="43799" class="Keyword">import</a> <a id="43806" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="43851" class="Keyword">open</a> <a id="43856" class="Keyword">import</a> <a id="43863" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="43910" class="Keyword">open</a> <a id="43915" class="Keyword">import</a> <a id="43922" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="43975" class="Keyword">open</a> <a id="43980" class="Keyword">import</a> <a id="43987" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>