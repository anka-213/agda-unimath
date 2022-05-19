# Univalent mathematics in Agda

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

<pre class="Agda"><a id="2967" class="Symbol">{-#</a> <a id="2971" class="Keyword">OPTIONS</a> <a id="2979" class="Pragma">--without-K</a> <a id="2991" class="Pragma">--exact-split</a> <a id="3005" class="Pragma">--guardedness</a> <a id="3019" class="Symbol">#-}</a>
</pre>
See the list of all Agda modules [here](everything.html).

## Category theory

<pre class="Agda"><a id="3115" class="Keyword">open</a> <a id="3120" class="Keyword">import</a> <a id="3127" href="category-theory.html" class="Module">category-theory</a>
<a id="3143" class="Keyword">open</a> <a id="3148" class="Keyword">import</a> <a id="3155" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="3203" class="Keyword">open</a> <a id="3208" class="Keyword">import</a> <a id="3215" href="category-theory.anafunctors.html" class="Module">category-theory.anafunctors</a>
<a id="3243" class="Keyword">open</a> <a id="3248" class="Keyword">import</a> <a id="3255" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="3282" class="Keyword">open</a> <a id="3287" class="Keyword">import</a> <a id="3294" href="category-theory.epimorphisms-large-precategories.html" class="Module">category-theory.epimorphisms-large-precategories</a>
<a id="3343" class="Keyword">open</a> <a id="3348" class="Keyword">import</a> <a id="3355" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="3395" class="Keyword">open</a> <a id="3400" class="Keyword">import</a> <a id="3407" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="3456" class="Keyword">open</a> <a id="3461" class="Keyword">import</a> <a id="3468" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="3511" class="Keyword">open</a> <a id="3516" class="Keyword">import</a> <a id="3523" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="3559" class="Keyword">open</a> <a id="3564" class="Keyword">import</a> <a id="3571" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="3616" class="Keyword">open</a> <a id="3621" class="Keyword">import</a> <a id="3628" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="3667" class="Keyword">open</a> <a id="3672" class="Keyword">import</a> <a id="3679" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="3750" class="Keyword">open</a> <a id="3755" class="Keyword">import</a> <a id="3762" href="category-theory.initial-objects-precategories.html" class="Module">category-theory.initial-objects-precategories</a>
<a id="3808" class="Keyword">open</a> <a id="3813" class="Keyword">import</a> <a id="3820" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="3860" class="Keyword">open</a> <a id="3865" class="Keyword">import</a> <a id="3872" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="3921" class="Keyword">open</a> <a id="3926" class="Keyword">import</a> <a id="3933" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="3976" class="Keyword">open</a> <a id="3981" class="Keyword">import</a> <a id="3988" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="4021" class="Keyword">open</a> <a id="4026" class="Keyword">import</a> <a id="4033" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="4069" class="Keyword">open</a> <a id="4074" class="Keyword">import</a> <a id="4081" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="4131" class="Keyword">open</a> <a id="4136" class="Keyword">import</a> <a id="4143" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="4191" class="Keyword">open</a> <a id="4196" class="Keyword">import</a> <a id="4203" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="4260" class="Keyword">open</a> <a id="4265" class="Keyword">import</a> <a id="4272" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="4323" class="Keyword">open</a> <a id="4328" class="Keyword">import</a> <a id="4335" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="4386" class="Keyword">open</a> <a id="4391" class="Keyword">import</a> <a id="4398" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="4458" class="Keyword">open</a> <a id="4463" class="Keyword">import</a> <a id="4470" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="4524" class="Keyword">open</a> <a id="4529" class="Keyword">import</a> <a id="4536" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
<a id="4566" class="Keyword">open</a> <a id="4571" class="Keyword">import</a> <a id="4578" href="category-theory.slice-precategories.html" class="Module">category-theory.slice-precategories</a>
<a id="4614" class="Keyword">open</a> <a id="4619" class="Keyword">import</a> <a id="4626" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Commutative algebra

<pre class="Agda"><a id="4710" class="Keyword">open</a> <a id="4715" class="Keyword">import</a> <a id="4722" href="commutative-algebra.html" class="Module">commutative-algebra</a>
<a id="4742" class="Keyword">open</a> <a id="4747" class="Keyword">import</a> <a id="4754" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>
<a id="4792" class="Keyword">open</a> <a id="4797" class="Keyword">import</a> <a id="4804" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a>
<a id="4840" class="Keyword">open</a> <a id="4845" class="Keyword">import</a> <a id="4852" href="commutative-algebra.eisenstein-integers.html" class="Module">commutative-algebra.eisenstein-integers</a>
<a id="4892" class="Keyword">open</a> <a id="4897" class="Keyword">import</a> <a id="4904" href="commutative-algebra.gaussian-integers.html" class="Module">commutative-algebra.gaussian-integers</a>
<a id="4942" class="Keyword">open</a> <a id="4947" class="Keyword">import</a> <a id="4954" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a>
<a id="5006" class="Keyword">open</a> <a id="5011" class="Keyword">import</a> <a id="5018" href="commutative-algebra.ideals-commutative-rings.html" class="Module">commutative-algebra.ideals-commutative-rings</a>
<a id="5063" class="Keyword">open</a> <a id="5068" class="Keyword">import</a> <a id="5075" href="commutative-algebra.isomorphisms-commutative-rings.html" class="Module">commutative-algebra.isomorphisms-commutative-rings</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="5168" class="Keyword">open</a> <a id="5173" class="Keyword">import</a> <a id="5180" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5205" class="Keyword">open</a> <a id="5210" class="Keyword">import</a> <a id="5217" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5266" class="Keyword">open</a> <a id="5271" class="Keyword">import</a> <a id="5278" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5321" class="Keyword">open</a> <a id="5326" class="Keyword">import</a> <a id="5333" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5383" class="Keyword">open</a> <a id="5388" class="Keyword">import</a> <a id="5395" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5441" class="Keyword">open</a> <a id="5446" class="Keyword">import</a> <a id="5453" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5500" class="Keyword">open</a> <a id="5505" class="Keyword">import</a> <a id="5512" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="5571" class="Keyword">open</a> <a id="5576" class="Keyword">import</a> <a id="5583" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="5624" class="Keyword">open</a> <a id="5629" class="Keyword">import</a> <a id="5636" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="5679" class="Keyword">open</a> <a id="5684" class="Keyword">import</a> <a id="5691" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="5735" class="Keyword">open</a> <a id="5740" class="Keyword">import</a> <a id="5747" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="5792" class="Keyword">open</a> <a id="5797" class="Keyword">import</a> <a id="5804" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="5856" class="Keyword">open</a> <a id="5861" class="Keyword">import</a> <a id="5868" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="5928" class="Keyword">open</a> <a id="5933" class="Keyword">import</a> <a id="5940" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="5981" class="Keyword">open</a> <a id="5986" class="Keyword">import</a> <a id="5993" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6038" class="Keyword">open</a> <a id="6043" class="Keyword">import</a> <a id="6050" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6097" class="Keyword">open</a> <a id="6102" class="Keyword">import</a> <a id="6109" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6152" class="Keyword">open</a> <a id="6157" class="Keyword">import</a> <a id="6164" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6214" class="Keyword">open</a> <a id="6219" class="Keyword">import</a> <a id="6226" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6273" class="Keyword">open</a> <a id="6278" class="Keyword">import</a> <a id="6285" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6342" class="Keyword">open</a> <a id="6347" class="Keyword">import</a> <a id="6354" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6408" class="Keyword">open</a> <a id="6413" class="Keyword">import</a> <a id="6420" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6480" class="Keyword">open</a> <a id="6485" class="Keyword">import</a> <a id="6492" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="6535" class="Keyword">open</a> <a id="6540" class="Keyword">import</a> <a id="6547" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="6597" class="Keyword">open</a> <a id="6602" class="Keyword">import</a> <a id="6609" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="6669" class="Keyword">open</a> <a id="6674" class="Keyword">import</a> <a id="6681" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="6730" class="Keyword">open</a> <a id="6735" class="Keyword">import</a> <a id="6742" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="6798" class="Keyword">open</a> <a id="6803" class="Keyword">import</a> <a id="6810" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="6846" class="Keyword">open</a> <a id="6851" class="Keyword">import</a> <a id="6858" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="6902" class="Keyword">open</a> <a id="6907" class="Keyword">import</a> <a id="6914" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="6958" class="Keyword">open</a> <a id="6963" class="Keyword">import</a> <a id="6970" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7020" class="Keyword">open</a> <a id="7025" class="Keyword">import</a> <a id="7032" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7078" class="Keyword">open</a> <a id="7083" class="Keyword">import</a> <a id="7090" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7125" class="Keyword">open</a> <a id="7130" class="Keyword">import</a> <a id="7137" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7182" class="Keyword">open</a> <a id="7187" class="Keyword">import</a> <a id="7194" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7252" class="Keyword">open</a> <a id="7257" class="Keyword">import</a> <a id="7264" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7329" class="Keyword">open</a> <a id="7334" class="Keyword">import</a> <a id="7341" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7384" class="Keyword">open</a> <a id="7389" class="Keyword">import</a> <a id="7396" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7450" class="Keyword">open</a> <a id="7455" class="Keyword">import</a> <a id="7462" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="7507" class="Keyword">open</a> <a id="7512" class="Keyword">import</a> <a id="7519" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="7571" class="Keyword">open</a> <a id="7576" class="Keyword">import</a> <a id="7583" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="7641" class="Keyword">open</a> <a id="7646" class="Keyword">import</a> <a id="7653" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="7699" class="Keyword">open</a> <a id="7704" class="Keyword">import</a> <a id="7711" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="7755" class="Keyword">open</a> <a id="7760" class="Keyword">import</a> <a id="7767" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="7801" class="Keyword">open</a> <a id="7806" class="Keyword">import</a> <a id="7813" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="7867" class="Keyword">open</a> <a id="7872" class="Keyword">import</a> <a id="7879" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="7928" class="Keyword">open</a> <a id="7933" class="Keyword">import</a> <a id="7940" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="7981" class="Keyword">open</a> <a id="7986" class="Keyword">import</a> <a id="7993" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8042" class="Keyword">open</a> <a id="8047" class="Keyword">import</a> <a id="8054" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8120" class="Keyword">open</a> <a id="8125" class="Keyword">import</a> <a id="8132" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8176" class="Keyword">open</a> <a id="8181" class="Keyword">import</a> <a id="8188" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8237" class="Keyword">open</a> <a id="8242" class="Keyword">import</a> <a id="8249" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8305" class="Keyword">open</a> <a id="8310" class="Keyword">import</a> <a id="8317" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="8358" class="Keyword">open</a> <a id="8363" class="Keyword">import</a> <a id="8370" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="8419" class="Keyword">open</a> <a id="8424" class="Keyword">import</a> <a id="8431" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="8490" class="Keyword">open</a> <a id="8495" class="Keyword">import</a> <a id="8502" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="8541" class="Keyword">open</a> <a id="8546" class="Keyword">import</a> <a id="8553" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="8606" class="Keyword">open</a> <a id="8611" class="Keyword">import</a> <a id="8618" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="8675" class="Keyword">open</a> <a id="8680" class="Keyword">import</a> <a id="8687" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="8729" class="Keyword">open</a> <a id="8734" class="Keyword">import</a> <a id="8741" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="8792" class="Keyword">open</a> <a id="8797" class="Keyword">import</a> <a id="8804" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="8862" class="Keyword">open</a> <a id="8867" class="Keyword">import</a> <a id="8874" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="8938" class="Keyword">open</a> <a id="8943" class="Keyword">import</a> <a id="8950" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9003" class="Keyword">open</a> <a id="9008" class="Keyword">import</a> <a id="9015" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9068" class="Keyword">open</a> <a id="9073" class="Keyword">import</a> <a id="9080" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9141" class="Keyword">open</a> <a id="9146" class="Keyword">import</a> <a id="9153" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="9211" class="Keyword">open</a> <a id="9216" class="Keyword">import</a> <a id="9223" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="9272" class="Keyword">open</a> <a id="9277" class="Keyword">import</a> <a id="9284" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="9327" class="Keyword">open</a> <a id="9332" class="Keyword">import</a> <a id="9339" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="9383" class="Keyword">open</a> <a id="9388" class="Keyword">import</a> <a id="9395" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="9442" class="Keyword">open</a> <a id="9447" class="Keyword">import</a> <a id="9454" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="9515" class="Keyword">open</a> <a id="9520" class="Keyword">import</a> <a id="9527" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="9590" class="Keyword">open</a> <a id="9595" class="Keyword">import</a> <a id="9602" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="9662" class="Keyword">open</a> <a id="9667" class="Keyword">import</a> <a id="9674" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="9728" class="Keyword">open</a> <a id="9733" class="Keyword">import</a> <a id="9740" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="9805" class="Keyword">open</a> <a id="9810" class="Keyword">import</a> <a id="9817" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="9925" class="Keyword">open</a> <a id="9930" class="Keyword">import</a> <a id="9937" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="9957" class="Keyword">open</a> <a id="9962" class="Keyword">import</a> <a id="9969" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10015" class="Keyword">open</a> <a id="10020" class="Keyword">import</a> <a id="10027" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10073" class="Keyword">open</a> <a id="10078" class="Keyword">import</a> <a id="10085" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="10119" class="Keyword">open</a> <a id="10124" class="Keyword">import</a> <a id="10131" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="10166" class="Keyword">open</a> <a id="10171" class="Keyword">import</a> <a id="10178" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="10216" class="Keyword">open</a> <a id="10221" class="Keyword">import</a> <a id="10228" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="10266" class="Keyword">open</a> <a id="10271" class="Keyword">import</a> <a id="10278" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="10318" class="Keyword">open</a> <a id="10323" class="Keyword">import</a> <a id="10330" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="10363" class="Keyword">open</a> <a id="10368" class="Keyword">import</a> <a id="10375" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="10413" class="Keyword">open</a> <a id="10418" class="Keyword">import</a> <a id="10425" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="10488" class="Keyword">open</a> <a id="10493" class="Keyword">import</a> <a id="10500" href="foundation.html" class="Module">foundation</a>
<a id="10511" class="Keyword">open</a> <a id="10516" class="Keyword">import</a> <a id="10523" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="10541" class="Keyword">open</a> <a id="10546" class="Keyword">import</a> <a id="10553" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="10572" class="Keyword">open</a> <a id="10577" class="Keyword">import</a> <a id="10584" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="10603" class="Keyword">open</a> <a id="10608" class="Keyword">import</a> <a id="10615" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="10659" class="Keyword">open</a> <a id="10664" class="Keyword">import</a> <a id="10671" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="10696" class="Keyword">open</a> <a id="10701" class="Keyword">import</a> <a id="10708" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="10735" class="Keyword">open</a> <a id="10740" class="Keyword">import</a> <a id="10747" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="10776" class="Keyword">open</a> <a id="10781" class="Keyword">import</a> <a id="10788" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="10844" class="Keyword">open</a> <a id="10849" class="Keyword">import</a> <a id="10856" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="10887" class="Keyword">open</a> <a id="10892" class="Keyword">import</a> <a id="10899" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="10953" class="Keyword">open</a> <a id="10958" class="Keyword">import</a> <a id="10965" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="10993" class="Keyword">open</a> <a id="10998" class="Keyword">import</a> <a id="11005" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="11035" class="Keyword">open</a> <a id="11040" class="Keyword">import</a> <a id="11047" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="11067" class="Keyword">open</a> <a id="11072" class="Keyword">import</a> <a id="11079" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="11116" class="Keyword">open</a> <a id="11121" class="Keyword">import</a> <a id="11128" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="11163" class="Keyword">open</a> <a id="11168" class="Keyword">import</a> <a id="11175" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="11233" class="Keyword">open</a> <a id="11238" class="Keyword">import</a> <a id="11245" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="11283" class="Keyword">open</a> <a id="11288" class="Keyword">import</a> <a id="11295" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="11329" class="Keyword">open</a> <a id="11334" class="Keyword">import</a> <a id="11341" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="11370" class="Keyword">open</a> <a id="11375" class="Keyword">import</a> <a id="11382" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="11405" class="Keyword">open</a> <a id="11410" class="Keyword">import</a> <a id="11417" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="11440" class="Keyword">open</a> <a id="11445" class="Keyword">import</a> <a id="11452" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="11494" class="Keyword">open</a> <a id="11499" class="Keyword">import</a> <a id="11506" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="11538" class="Keyword">open</a> <a id="11543" class="Keyword">import</a> <a id="11550" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="11577" class="Keyword">open</a> <a id="11582" class="Keyword">import</a> <a id="11589" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="11614" class="Keyword">open</a> <a id="11619" class="Keyword">import</a> <a id="11626" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="11655" class="Keyword">open</a> <a id="11660" class="Keyword">import</a> <a id="11667" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="11697" class="Keyword">open</a> <a id="11702" class="Keyword">import</a> <a id="11709" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="11736" class="Keyword">open</a> <a id="11741" class="Keyword">import</a> <a id="11748" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="11767" class="Keyword">open</a> <a id="11772" class="Keyword">import</a> <a id="11779" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="11825" class="Keyword">open</a> <a id="11830" class="Keyword">import</a> <a id="11837" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="11879" class="Keyword">open</a> <a id="11884" class="Keyword">import</a> <a id="11891" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="11923" class="Keyword">open</a> <a id="11928" class="Keyword">import</a> <a id="11935" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="11965" class="Keyword">open</a> <a id="11970" class="Keyword">import</a> <a id="11977" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="12003" class="Keyword">open</a> <a id="12008" class="Keyword">import</a> <a id="12015" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="12049" class="Keyword">open</a> <a id="12054" class="Keyword">import</a> <a id="12061" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="12091" class="Keyword">open</a> <a id="12096" class="Keyword">import</a> <a id="12103" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="12130" class="Keyword">open</a> <a id="12135" class="Keyword">import</a> <a id="12142" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="12174" class="Keyword">open</a> <a id="12179" class="Keyword">import</a> <a id="12186" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="12220" class="Keyword">open</a> <a id="12225" class="Keyword">import</a> <a id="12232" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="12255" class="Keyword">open</a> <a id="12260" class="Keyword">import</a> <a id="12267" href="foundation.distributivity-of-dependent-functions-over-coproduct-types.html" class="Module">foundation.distributivity-of-dependent-functions-over-coproduct-types</a>
<a id="12337" class="Keyword">open</a> <a id="12342" class="Keyword">import</a> <a id="12349" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a>
<a id="12419" class="Keyword">open</a> <a id="12424" class="Keyword">import</a> <a id="12431" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="12458" class="Keyword">open</a> <a id="12463" class="Keyword">import</a> <a id="12470" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="12498" class="Keyword">open</a> <a id="12503" class="Keyword">import</a> <a id="12510" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="12547" class="Keyword">open</a> <a id="12552" class="Keyword">import</a> <a id="12559" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="12607" class="Keyword">open</a> <a id="12612" class="Keyword">import</a> <a id="12619" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="12659" class="Keyword">open</a> <a id="12664" class="Keyword">import</a> <a id="12671" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="12693" class="Keyword">open</a> <a id="12698" class="Keyword">import</a> <a id="12705" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="12728" class="Keyword">open</a> <a id="12733" class="Keyword">import</a> <a id="12740" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="12765" class="Keyword">open</a> <a id="12770" class="Keyword">import</a> <a id="12777" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="12822" class="Keyword">open</a> <a id="12827" class="Keyword">import</a> <a id="12834" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="12878" class="Keyword">open</a> <a id="12883" class="Keyword">import</a> <a id="12890" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="12926" class="Keyword">open</a> <a id="12931" class="Keyword">import</a> <a id="12938" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="12983" class="Keyword">open</a> <a id="12988" class="Keyword">import</a> <a id="12995" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="13036" class="Keyword">open</a> <a id="13041" class="Keyword">import</a> <a id="13048" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="13083" class="Keyword">open</a> <a id="13088" class="Keyword">import</a> <a id="13095" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="13126" class="Keyword">open</a> <a id="13131" class="Keyword">import</a> <a id="13138" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="13171" class="Keyword">open</a> <a id="13176" class="Keyword">import</a> <a id="13183" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="13216" class="Keyword">open</a> <a id="13221" class="Keyword">import</a> <a id="13228" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="13258" class="Keyword">open</a> <a id="13263" class="Keyword">import</a> <a id="13270" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="13294" class="Keyword">open</a> <a id="13299" class="Keyword">import</a> <a id="13306" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="13344" class="Keyword">open</a> <a id="13349" class="Keyword">import</a> <a id="13356" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="13387" class="Keyword">open</a> <a id="13392" class="Keyword">import</a> <a id="13399" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="13424" class="Keyword">open</a> <a id="13429" class="Keyword">import</a> <a id="13436" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="13464" class="Keyword">open</a> <a id="13469" class="Keyword">import</a> <a id="13476" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="13500" class="Keyword">open</a> <a id="13505" class="Keyword">import</a> <a id="13512" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="13538" class="Keyword">open</a> <a id="13543" class="Keyword">import</a> <a id="13550" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="13585" class="Keyword">open</a> <a id="13590" class="Keyword">import</a> <a id="13597" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="13618" class="Keyword">open</a> <a id="13623" class="Keyword">import</a> <a id="13630" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="13679" class="Keyword">open</a> <a id="13684" class="Keyword">import</a> <a id="13691" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="13732" class="Keyword">open</a> <a id="13737" class="Keyword">import</a> <a id="13744" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="13794" class="Keyword">open</a> <a id="13799" class="Keyword">import</a> <a id="13806" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="13852" class="Keyword">open</a> <a id="13857" class="Keyword">import</a> <a id="13864" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="13904" class="Keyword">open</a> <a id="13909" class="Keyword">import</a> <a id="13916" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="13966" class="Keyword">open</a> <a id="13971" class="Keyword">import</a> <a id="13978" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="14017" class="Keyword">open</a> <a id="14022" class="Keyword">import</a> <a id="14029" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="14069" class="Keyword">open</a> <a id="14074" class="Keyword">import</a> <a id="14081" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="14114" class="Keyword">open</a> <a id="14119" class="Keyword">import</a> <a id="14126" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="14175" class="Keyword">open</a> <a id="14180" class="Keyword">import</a> <a id="14187" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="14212" class="Keyword">open</a> <a id="14217" class="Keyword">import</a> <a id="14224" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="14262" class="Keyword">open</a> <a id="14267" class="Keyword">import</a> <a id="14274" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="14296" class="Keyword">open</a> <a id="14301" class="Keyword">import</a> <a id="14308" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="14336" class="Keyword">open</a> <a id="14341" class="Keyword">import</a> <a id="14348" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="14374" class="Keyword">open</a> <a id="14379" class="Keyword">import</a> <a id="14386" href="foundation.images.html" class="Module">foundation.images</a>
<a id="14404" class="Keyword">open</a> <a id="14409" class="Keyword">import</a> <a id="14416" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="14451" class="Keyword">open</a> <a id="14456" class="Keyword">import</a> <a id="14463" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="14490" class="Keyword">open</a> <a id="14495" class="Keyword">import</a> <a id="14502" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="14558" class="Keyword">open</a> <a id="14563" class="Keyword">import</a> <a id="14570" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="14599" class="Keyword">open</a> <a id="14604" class="Keyword">import</a> <a id="14611" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="14641" class="Keyword">open</a> <a id="14646" class="Keyword">import</a> <a id="14653" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="14680" class="Keyword">open</a> <a id="14685" class="Keyword">import</a> <a id="14692" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="14718" class="Keyword">open</a> <a id="14723" class="Keyword">import</a> <a id="14730" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="14757" class="Keyword">open</a> <a id="14762" class="Keyword">import</a> <a id="14769" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="14793" class="Keyword">open</a> <a id="14798" class="Keyword">import</a> <a id="14805" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="14828" class="Keyword">open</a> <a id="14833" class="Keyword">import</a> <a id="14840" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="14867" class="Keyword">open</a> <a id="14872" class="Keyword">import</a> <a id="14879" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="14911" class="Keyword">open</a> <a id="14916" class="Keyword">import</a> <a id="14923" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="14958" class="Keyword">open</a> <a id="14963" class="Keyword">import</a> <a id="14970" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="15001" class="Keyword">open</a> <a id="15006" class="Keyword">import</a> <a id="15013" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="15046" class="Keyword">open</a> <a id="15051" class="Keyword">import</a> <a id="15058" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="15092" class="Keyword">open</a> <a id="15097" class="Keyword">import</a> <a id="15104" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="15144" class="Keyword">open</a> <a id="15149" class="Keyword">import</a> <a id="15156" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="15187" class="Keyword">open</a> <a id="15192" class="Keyword">import</a> <a id="15199" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="15231" class="Keyword">open</a> <a id="15236" class="Keyword">import</a> <a id="15243" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="15274" class="Keyword">open</a> <a id="15279" class="Keyword">import</a> <a id="15286" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="15303" class="Keyword">open</a> <a id="15308" class="Keyword">import</a> <a id="15315" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="15340" class="Keyword">open</a> <a id="15345" class="Keyword">import</a> <a id="15352" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="15381" class="Keyword">open</a> <a id="15386" class="Keyword">import</a> <a id="15393" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="15418" class="Keyword">open</a> <a id="15423" class="Keyword">import</a> <a id="15430" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="15451" class="Keyword">open</a> <a id="15456" class="Keyword">import</a> <a id="15463" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="15487" class="Keyword">open</a> <a id="15492" class="Keyword">import</a> <a id="15499" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="15519" class="Keyword">open</a> <a id="15524" class="Keyword">import</a> <a id="15531" href="foundation.non-contractible-types.html" class="Module">foundation.non-contractible-types</a>
<a id="15565" class="Keyword">open</a> <a id="15570" class="Keyword">import</a> <a id="15577" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="15615" class="Keyword">open</a> <a id="15620" class="Keyword">import</a> <a id="15627" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="15651" class="Keyword">open</a> <a id="15656" class="Keyword">import</a> <a id="15663" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="15690" class="Keyword">open</a> <a id="15695" class="Keyword">import</a> <a id="15702" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="15737" class="Keyword">open</a> <a id="15742" class="Keyword">import</a> <a id="15749" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="15770" class="Keyword">open</a> <a id="15775" class="Keyword">import</a> <a id="15782" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="15818" class="Keyword">open</a> <a id="15823" class="Keyword">import</a> <a id="15830" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="15875" class="Keyword">open</a> <a id="15880" class="Keyword">import</a> <a id="15887" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="15933" class="Keyword">open</a> <a id="15938" class="Keyword">import</a> <a id="15945" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="15985" class="Keyword">open</a> <a id="15990" class="Keyword">import</a> <a id="15997" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="16027" class="Keyword">open</a> <a id="16032" class="Keyword">import</a> <a id="16039" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="16076" class="Keyword">open</a> <a id="16081" class="Keyword">import</a> <a id="16088" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="16112" class="Keyword">open</a> <a id="16117" class="Keyword">import</a> <a id="16124" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="16145" class="Keyword">open</a> <a id="16150" class="Keyword">import</a> <a id="16157" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="16192" class="Keyword">open</a> <a id="16197" class="Keyword">import</a> <a id="16204" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="16241" class="Keyword">open</a> <a id="16246" class="Keyword">import</a> <a id="16253" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="16302" class="Keyword">open</a> <a id="16307" class="Keyword">import</a> <a id="16314" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="16347" class="Keyword">open</a> <a id="16352" class="Keyword">import</a> <a id="16359" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="16382" class="Keyword">open</a> <a id="16387" class="Keyword">import</a> <a id="16394" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="16417" class="Keyword">open</a> <a id="16422" class="Keyword">import</a> <a id="16429" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="16452" class="Keyword">open</a> <a id="16457" class="Keyword">import</a> <a id="16464" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="16492" class="Keyword">open</a> <a id="16497" class="Keyword">import</a> <a id="16504" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="16524" class="Keyword">open</a> <a id="16529" class="Keyword">import</a> <a id="16536" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="16557" class="Keyword">open</a> <a id="16562" class="Keyword">import</a> <a id="16569" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="16600" class="Keyword">open</a> <a id="16605" class="Keyword">import</a> <a id="16612" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="16639" class="Keyword">open</a> <a id="16644" class="Keyword">import</a> <a id="16651" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="16667" class="Keyword">open</a> <a id="16672" class="Keyword">import</a> <a id="16679" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="16710" class="Keyword">open</a> <a id="16715" class="Keyword">import</a> <a id="16722" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="16739" class="Keyword">open</a> <a id="16744" class="Keyword">import</a> <a id="16751" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="16773" class="Keyword">open</a> <a id="16778" class="Keyword">import</a> <a id="16785" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="16812" class="Keyword">open</a> <a id="16817" class="Keyword">import</a> <a id="16824" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="16847" class="Keyword">open</a> <a id="16852" class="Keyword">import</a> <a id="16859" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="16886" class="Keyword">open</a> <a id="16891" class="Keyword">import</a> <a id="16898" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="16931" class="Keyword">open</a> <a id="16936" class="Keyword">import</a> <a id="16943" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="16983" class="Keyword">open</a> <a id="16988" class="Keyword">import</a> <a id="16995" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="17016" class="Keyword">open</a> <a id="17021" class="Keyword">import</a> <a id="17028" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="17057" class="Keyword">open</a> <a id="17062" class="Keyword">import</a> <a id="17069" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="17107" class="Keyword">open</a> <a id="17112" class="Keyword">import</a> <a id="17119" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="17139" class="Keyword">open</a> <a id="17144" class="Keyword">import</a> <a id="17151" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="17175" class="Keyword">open</a> <a id="17180" class="Keyword">import</a> <a id="17187" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="17214" class="Keyword">open</a> <a id="17219" class="Keyword">import</a> <a id="17226" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="17258" class="Keyword">open</a> <a id="17263" class="Keyword">import</a> <a id="17270" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="17300" class="Keyword">open</a> <a id="17305" class="Keyword">import</a> <a id="17312" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="17338" class="Keyword">open</a> <a id="17343" class="Keyword">import</a> <a id="17350" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="17377" class="Keyword">open</a> <a id="17382" class="Keyword">import</a> <a id="17389" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="17418" class="Keyword">open</a> <a id="17423" class="Keyword">import</a> <a id="17430" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="17453" class="Keyword">open</a> <a id="17458" class="Keyword">import</a> <a id="17465" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="17516" class="Keyword">open</a> <a id="17521" class="Keyword">import</a> <a id="17528" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="17571" class="Keyword">open</a> <a id="17576" class="Keyword">import</a> <a id="17583" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="17631" class="Keyword">open</a> <a id="17636" class="Keyword">import</a> <a id="17643" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="17681" class="Keyword">open</a> <a id="17686" class="Keyword">import</a> <a id="17693" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="17730" class="Keyword">open</a> <a id="17735" class="Keyword">import</a> <a id="17742" href="foundation.union.html" class="Module">foundation.union</a>
<a id="17759" class="Keyword">open</a> <a id="17764" class="Keyword">import</a> <a id="17771" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="17799" class="Keyword">open</a> <a id="17804" class="Keyword">import</a> <a id="17811" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="17847" class="Keyword">open</a> <a id="17852" class="Keyword">import</a> <a id="17859" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="17897" class="Keyword">open</a> <a id="17902" class="Keyword">import</a> <a id="17909" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="17942" class="Keyword">open</a> <a id="17947" class="Keyword">import</a> <a id="17954" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="17975" class="Keyword">open</a> <a id="17980" class="Keyword">import</a> <a id="17987" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="18041" class="Keyword">open</a> <a id="18046" class="Keyword">import</a> <a id="18053" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="18075" class="Keyword">open</a> <a id="18080" class="Keyword">import</a> <a id="18087" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="18122" class="Keyword">open</a> <a id="18127" class="Keyword">import</a> <a id="18134" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="18164" class="Keyword">open</a> <a id="18169" class="Keyword">import</a> <a id="18176" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="18215" class="Keyword">open</a> <a id="18220" class="Keyword">import</a> <a id="18227" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="18281" class="Keyword">open</a> <a id="18286" class="Keyword">import</a> <a id="18293" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="18339" class="Keyword">open</a> <a id="18344" class="Keyword">import</a> <a id="18351" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="18402" class="Keyword">open</a> <a id="18407" class="Keyword">import</a> <a id="18414" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="18455" class="Keyword">open</a> <a id="18460" class="Keyword">import</a> <a id="18467" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="18512" class="Keyword">open</a> <a id="18517" class="Keyword">import</a> <a id="18524" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="18569" class="Keyword">open</a> <a id="18574" class="Keyword">import</a> <a id="18581" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="18617" class="Keyword">open</a> <a id="18622" class="Keyword">import</a> <a id="18629" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="18665" class="Keyword">open</a> <a id="18670" class="Keyword">import</a> <a id="18677" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="18742" class="Keyword">open</a> <a id="18747" class="Keyword">import</a> <a id="18754" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="18809" class="Keyword">open</a> <a id="18814" class="Keyword">import</a> <a id="18821" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="18861" class="Keyword">open</a> <a id="18866" class="Keyword">import</a> <a id="18873" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="18917" class="Keyword">open</a> <a id="18922" class="Keyword">import</a> <a id="18929" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="18974" class="Keyword">open</a> <a id="18979" class="Keyword">import</a> <a id="18986" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="19027" class="Keyword">open</a> <a id="19032" class="Keyword">import</a> <a id="19039" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="19079" class="Keyword">open</a> <a id="19084" class="Keyword">import</a> <a id="19091" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="19118" class="Keyword">open</a> <a id="19123" class="Keyword">import</a> <a id="19130" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="19166" class="Keyword">open</a> <a id="19171" class="Keyword">import</a> <a id="19178" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="19205" class="Keyword">open</a> <a id="19210" class="Keyword">import</a> <a id="19217" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="19254" class="Keyword">open</a> <a id="19259" class="Keyword">import</a> <a id="19266" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="19294" class="Keyword">open</a> <a id="19299" class="Keyword">import</a> <a id="19306" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="19325" class="Keyword">open</a> <a id="19330" class="Keyword">import</a> <a id="19337" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="19377" class="Keyword">open</a> <a id="19382" class="Keyword">import</a> <a id="19389" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="19421" class="Keyword">open</a> <a id="19426" class="Keyword">import</a> <a id="19433" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="19481" class="Keyword">open</a> <a id="19486" class="Keyword">import</a> <a id="19493" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="19516" class="Keyword">open</a> <a id="19521" class="Keyword">import</a> <a id="19528" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="19552" class="Keyword">open</a> <a id="19557" class="Keyword">import</a> <a id="19564" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="19604" class="Keyword">open</a> <a id="19609" class="Keyword">import</a> <a id="19616" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="19659" class="Keyword">open</a> <a id="19664" class="Keyword">import</a> <a id="19671" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="19705" class="Keyword">open</a> <a id="19710" class="Keyword">import</a> <a id="19717" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="19747" class="Keyword">open</a> <a id="19752" class="Keyword">import</a> <a id="19759" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="19793" class="Keyword">open</a> <a id="19798" class="Keyword">import</a> <a id="19805" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="19840" class="Keyword">open</a> <a id="19845" class="Keyword">import</a> <a id="19852" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="19889" class="Keyword">open</a> <a id="19894" class="Keyword">import</a> <a id="19901" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="19928" class="Keyword">open</a> <a id="19933" class="Keyword">import</a> <a id="19940" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="19968" class="Keyword">open</a> <a id="19973" class="Keyword">import</a> <a id="19980" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="20029" class="Keyword">open</a> <a id="20034" class="Keyword">import</a> <a id="20041" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="20087" class="Keyword">open</a> <a id="20092" class="Keyword">import</a> <a id="20099" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="20139" class="Keyword">open</a> <a id="20144" class="Keyword">import</a> <a id="20151" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="20189" class="Keyword">open</a> <a id="20194" class="Keyword">import</a> <a id="20201" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="20230" class="Keyword">open</a> <a id="20235" class="Keyword">import</a> <a id="20242" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="20272" class="Keyword">open</a> <a id="20277" class="Keyword">import</a> <a id="20284" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="20315" class="Keyword">open</a> <a id="20320" class="Keyword">import</a> <a id="20327" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="20353" class="Keyword">open</a> <a id="20358" class="Keyword">import</a> <a id="20365" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="20416" class="Keyword">open</a> <a id="20421" class="Keyword">import</a> <a id="20428" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="20482" class="Keyword">open</a> <a id="20487" class="Keyword">import</a> <a id="20494" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="20521" class="Keyword">open</a> <a id="20526" class="Keyword">import</a> <a id="20533" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="20566" class="Keyword">open</a> <a id="20571" class="Keyword">import</a> <a id="20578" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="20609" class="Keyword">open</a> <a id="20614" class="Keyword">import</a> <a id="20621" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="20658" class="Keyword">open</a> <a id="20663" class="Keyword">import</a> <a id="20670" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="20695" class="Keyword">open</a> <a id="20700" class="Keyword">import</a> <a id="20707" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="20739" class="Keyword">open</a> <a id="20744" class="Keyword">import</a> <a id="20751" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="20786" class="Keyword">open</a> <a id="20791" class="Keyword">import</a> <a id="20798" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="20827" class="Keyword">open</a> <a id="20832" class="Keyword">import</a> <a id="20839" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="20867" class="Keyword">open</a> <a id="20872" class="Keyword">import</a> <a id="20879" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="20904" class="Keyword">open</a> <a id="20909" class="Keyword">import</a> <a id="20916" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="20937" class="Keyword">open</a> <a id="20942" class="Keyword">import</a> <a id="20949" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="20985" class="Keyword">open</a> <a id="20990" class="Keyword">import</a> <a id="20997" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="21040" class="Keyword">open</a> <a id="21045" class="Keyword">import</a> <a id="21052" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="21077" class="Keyword">open</a> <a id="21082" class="Keyword">import</a> <a id="21089" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="21120" class="Keyword">open</a> <a id="21125" class="Keyword">import</a> <a id="21132" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="21164" class="Keyword">open</a> <a id="21169" class="Keyword">import</a> <a id="21176" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="21210" class="Keyword">open</a> <a id="21215" class="Keyword">import</a> <a id="21222" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="21278" class="Keyword">open</a> <a id="21283" class="Keyword">import</a> <a id="21290" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="21343" class="Keyword">open</a> <a id="21348" class="Keyword">import</a> <a id="21355" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="21382" class="Keyword">open</a> <a id="21387" class="Keyword">import</a> <a id="21394" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="21456" class="Keyword">open</a> <a id="21461" class="Keyword">import</a> <a id="21468" href="graph-theory.html" class="Module">graph-theory</a>
<a id="21481" class="Keyword">open</a> <a id="21486" class="Keyword">import</a> <a id="21493" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="21534" class="Keyword">open</a> <a id="21539" class="Keyword">import</a> <a id="21546" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="21575" class="Keyword">open</a> <a id="21580" class="Keyword">import</a> <a id="21587" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="21632" class="Keyword">open</a> <a id="21637" class="Keyword">import</a> <a id="21644" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="21688" class="Keyword">open</a> <a id="21693" class="Keyword">import</a> <a id="21700" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="21727" class="Keyword">open</a> <a id="21732" class="Keyword">import</a> <a id="21739" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a>
<a id="21780" class="Keyword">open</a> <a id="21785" class="Keyword">import</a> <a id="21792" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="21815" class="Keyword">open</a> <a id="21820" class="Keyword">import</a> <a id="21827" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="21876" class="Keyword">open</a> <a id="21881" class="Keyword">import</a> <a id="21888" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="21927" class="Keyword">open</a> <a id="21932" class="Keyword">import</a> <a id="21939" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="21980" class="Keyword">open</a> <a id="21985" class="Keyword">import</a> <a id="21992" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="22036" class="Keyword">open</a> <a id="22041" class="Keyword">import</a> <a id="22048" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="22085" class="Keyword">open</a> <a id="22090" class="Keyword">import</a> <a id="22097" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="22119" class="Keyword">open</a> <a id="22124" class="Keyword">import</a> <a id="22131" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="22161" class="Keyword">open</a> <a id="22166" class="Keyword">import</a> <a id="22173" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="22212" class="Keyword">open</a> <a id="22217" class="Keyword">import</a> <a id="22224" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="22262" class="Keyword">open</a> <a id="22267" class="Keyword">import</a> <a id="22274" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="22305" class="Keyword">open</a> <a id="22310" class="Keyword">import</a> <a id="22317" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="22344" class="Keyword">open</a> <a id="22349" class="Keyword">import</a> <a id="22356" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="22414" class="Keyword">open</a> <a id="22419" class="Keyword">import</a> <a id="22426" href="group-theory.html" class="Module">group-theory</a>
<a id="22439" class="Keyword">open</a> <a id="22444" class="Keyword">import</a> <a id="22451" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="22479" class="Keyword">open</a> <a id="22484" class="Keyword">import</a> <a id="22491" href="group-theory.abelian-subgroups.html" class="Module">group-theory.abelian-subgroups</a>
<a id="22522" class="Keyword">open</a> <a id="22527" class="Keyword">import</a> <a id="22534" href="group-theory.abstract-group-torsors.html" class="Module">group-theory.abstract-group-torsors</a>
<a id="22570" class="Keyword">open</a> <a id="22575" class="Keyword">import</a> <a id="22582" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="22633" class="Keyword">open</a> <a id="22638" class="Keyword">import</a> <a id="22645" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="22678" class="Keyword">open</a> <a id="22683" class="Keyword">import</a> <a id="22690" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="22722" class="Keyword">open</a> <a id="22727" class="Keyword">import</a> <a id="22734" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="22770" class="Keyword">open</a> <a id="22775" class="Keyword">import</a> <a id="22782" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="22811" class="Keyword">open</a> <a id="22816" class="Keyword">import</a> <a id="22823" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="22859" class="Keyword">open</a> <a id="22864" class="Keyword">import</a> <a id="22871" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="22900" class="Keyword">open</a> <a id="22905" class="Keyword">import</a> <a id="22912" href="group-theory.concrete-subgroups.html" class="Module">group-theory.concrete-subgroups</a>
<a id="22944" class="Keyword">open</a> <a id="22949" class="Keyword">import</a> <a id="22956" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="22981" class="Keyword">open</a> <a id="22986" class="Keyword">import</a> <a id="22993" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="23024" class="Keyword">open</a> <a id="23029" class="Keyword">import</a> <a id="23036" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="23083" class="Keyword">open</a> <a id="23088" class="Keyword">import</a> <a id="23095" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="23128" class="Keyword">open</a> <a id="23133" class="Keyword">import</a> <a id="23140" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="23180" class="Keyword">open</a> <a id="23185" class="Keyword">import</a> <a id="23192" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="23229" class="Keyword">open</a> <a id="23234" class="Keyword">import</a> <a id="23241" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a>
<a id="23277" class="Keyword">open</a> <a id="23282" class="Keyword">import</a> <a id="23289" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="23321" class="Keyword">open</a> <a id="23326" class="Keyword">import</a> <a id="23333" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="23360" class="Keyword">open</a> <a id="23365" class="Keyword">import</a> <a id="23372" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="23392" class="Keyword">open</a> <a id="23397" class="Keyword">import</a> <a id="23404" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="23431" class="Keyword">open</a> <a id="23436" class="Keyword">import</a> <a id="23443" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="23485" class="Keyword">open</a> <a id="23490" class="Keyword">import</a> <a id="23497" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="23544" class="Keyword">open</a> <a id="23549" class="Keyword">import</a> <a id="23556" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="23597" class="Keyword">open</a> <a id="23602" class="Keyword">import</a> <a id="23609" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="23643" class="Keyword">open</a> <a id="23648" class="Keyword">import</a> <a id="23655" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="23690" class="Keyword">open</a> <a id="23695" class="Keyword">import</a> <a id="23702" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="23740" class="Keyword">open</a> <a id="23745" class="Keyword">import</a> <a id="23752" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="23784" class="Keyword">open</a> <a id="23789" class="Keyword">import</a> <a id="23796" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="23837" class="Keyword">open</a> <a id="23842" class="Keyword">import</a> <a id="23849" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="23890" class="Keyword">open</a> <a id="23895" class="Keyword">import</a> <a id="23902" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="23942" class="Keyword">open</a> <a id="23947" class="Keyword">import</a> <a id="23954" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="23987" class="Keyword">open</a> <a id="23992" class="Keyword">import</a> <a id="23999" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="24036" class="Keyword">open</a> <a id="24041" class="Keyword">import</a> <a id="24048" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="24093" class="Keyword">open</a> <a id="24098" class="Keyword">import</a> <a id="24105" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="24126" class="Keyword">open</a> <a id="24131" class="Keyword">import</a> <a id="24138" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="24172" class="Keyword">open</a> <a id="24177" class="Keyword">import</a> <a id="24184" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="24219" class="Keyword">open</a> <a id="24224" class="Keyword">import</a> <a id="24231" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="24265" class="Keyword">open</a> <a id="24270" class="Keyword">import</a> <a id="24277" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="24319" class="Keyword">open</a> <a id="24324" class="Keyword">import</a> <a id="24331" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="24366" class="Keyword">open</a> <a id="24371" class="Keyword">import</a> <a id="24378" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="24417" class="Keyword">open</a> <a id="24422" class="Keyword">import</a> <a id="24429" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="24466" class="Keyword">open</a> <a id="24471" class="Keyword">import</a> <a id="24478" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="24502" class="Keyword">open</a> <a id="24507" class="Keyword">import</a> <a id="24514" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="24539" class="Keyword">open</a> <a id="24544" class="Keyword">import</a> <a id="24551" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="24582" class="Keyword">open</a> <a id="24587" class="Keyword">import</a> <a id="24594" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="24645" class="Keyword">open</a> <a id="24650" class="Keyword">import</a> <a id="24657" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="24680" class="Keyword">open</a> <a id="24685" class="Keyword">import</a> <a id="24692" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="24740" class="Keyword">open</a> <a id="24745" class="Keyword">import</a> <a id="24752" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="24782" class="Keyword">open</a> <a id="24787" class="Keyword">import</a> <a id="24794" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="24864" class="Keyword">open</a> <a id="24869" class="Keyword">import</a> <a id="24876" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="24891" class="Keyword">open</a> <a id="24896" class="Keyword">import</a> <a id="24903" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="24936" class="Keyword">open</a> <a id="24941" class="Keyword">import</a> <a id="24948" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="24980" class="Keyword">open</a> <a id="24985" class="Keyword">import</a> <a id="24992" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="25034" class="Keyword">open</a> <a id="25039" class="Keyword">import</a> <a id="25046" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="25084" class="Keyword">open</a> <a id="25089" class="Keyword">import</a> <a id="25096" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="25133" class="Keyword">open</a> <a id="25138" class="Keyword">import</a> <a id="25145" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="25178" class="Keyword">open</a> <a id="25183" class="Keyword">import</a> <a id="25190" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="25214" class="Keyword">open</a> <a id="25219" class="Keyword">import</a> <a id="25226" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="25265" class="Keyword">open</a> <a id="25270" class="Keyword">import</a> <a id="25277" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="25323" class="Keyword">open</a> <a id="25328" class="Keyword">import</a> <a id="25335" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="25380" class="Keyword">open</a> <a id="25385" class="Keyword">import</a> <a id="25392" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="25430" class="Keyword">open</a> <a id="25435" class="Keyword">import</a> <a id="25442" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="25474" class="Keyword">open</a> <a id="25479" class="Keyword">import</a> <a id="25486" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="25539" class="Keyword">open</a> <a id="25544" class="Keyword">import</a> <a id="25551" href="order-theory.html" class="Module">order-theory</a>
<a id="25564" class="Keyword">open</a> <a id="25569" class="Keyword">import</a> <a id="25576" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="25603" class="Keyword">open</a> <a id="25608" class="Keyword">import</a> <a id="25615" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="25645" class="Keyword">open</a> <a id="25650" class="Keyword">import</a> <a id="25657" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="25690" class="Keyword">open</a> <a id="25695" class="Keyword">import</a> <a id="25702" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="25738" class="Keyword">open</a> <a id="25743" class="Keyword">import</a> <a id="25750" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="25777" class="Keyword">open</a> <a id="25782" class="Keyword">import</a> <a id="25789" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="25819" class="Keyword">open</a> <a id="25824" class="Keyword">import</a> <a id="25831" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="25867" class="Keyword">open</a> <a id="25872" class="Keyword">import</a> <a id="25879" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="25921" class="Keyword">open</a> <a id="25926" class="Keyword">import</a> <a id="25933" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="25965" class="Keyword">open</a> <a id="25970" class="Keyword">import</a> <a id="25977" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="26008" class="Keyword">open</a> <a id="26013" class="Keyword">import</a> <a id="26020" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="26046" class="Keyword">open</a> <a id="26051" class="Keyword">import</a> <a id="26058" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="26087" class="Keyword">open</a> <a id="26092" class="Keyword">import</a> <a id="26099" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="26136" class="Keyword">open</a> <a id="26141" class="Keyword">import</a> <a id="26148" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="26188" class="Keyword">open</a> <a id="26193" class="Keyword">import</a> <a id="26200" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="26235" class="Keyword">open</a> <a id="26240" class="Keyword">import</a> <a id="26247" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="26285" class="Keyword">open</a> <a id="26290" class="Keyword">import</a> <a id="26297" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="26336" class="Keyword">open</a> <a id="26341" class="Keyword">import</a> <a id="26348" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="26383" class="Keyword">open</a> <a id="26388" class="Keyword">import</a> <a id="26395" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="26430" class="Keyword">open</a> <a id="26435" class="Keyword">import</a> <a id="26442" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="26480" class="Keyword">open</a> <a id="26485" class="Keyword">import</a> <a id="26492" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="26523" class="Keyword">open</a> <a id="26528" class="Keyword">import</a> <a id="26535" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="26568" class="Keyword">open</a> <a id="26573" class="Keyword">import</a> <a id="26580" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="26600" class="Keyword">open</a> <a id="26605" class="Keyword">import</a> <a id="26612" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="26635" class="Keyword">open</a> <a id="26640" class="Keyword">import</a> <a id="26647" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="26670" class="Keyword">open</a> <a id="26675" class="Keyword">import</a> <a id="26682" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="26708" class="Keyword">open</a> <a id="26713" class="Keyword">import</a> <a id="26720" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="26746" class="Keyword">open</a> <a id="26751" class="Keyword">import</a> <a id="26758" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Polytopes

<pre class="Agda"><a id="26814" class="Keyword">open</a> <a id="26819" class="Keyword">import</a> <a id="26826" href="polytopes.html" class="Module">polytopes</a>
<a id="26836" class="Keyword">open</a> <a id="26841" class="Keyword">import</a> <a id="26848" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="26906" class="Keyword">open</a> <a id="26911" class="Keyword">import</a> <a id="26918" href="ring-theory.html" class="Module">ring-theory</a>
<a id="26930" class="Keyword">open</a> <a id="26935" class="Keyword">import</a> <a id="26942" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="26969" class="Keyword">open</a> <a id="26974" class="Keyword">import</a> <a id="26981" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="27013" class="Keyword">open</a> <a id="27018" class="Keyword">import</a> <a id="27025" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="27071" class="Keyword">open</a> <a id="27076" class="Keyword">import</a> <a id="27083" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="27108" class="Keyword">open</a> <a id="27113" class="Keyword">import</a> <a id="27120" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="27158" class="Keyword">open</a> <a id="27163" class="Keyword">import</a> <a id="27170" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="27201" class="Keyword">open</a> <a id="27206" class="Keyword">import</a> <a id="27213" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="27245" class="Keyword">open</a> <a id="27250" class="Keyword">import</a> <a id="27257" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="27286" class="Keyword">open</a> <a id="27291" class="Keyword">import</a> <a id="27298" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="27325" class="Keyword">open</a> <a id="27330" class="Keyword">import</a> <a id="27337" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="27364" class="Keyword">open</a> <a id="27369" class="Keyword">import</a> <a id="27376" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="27394" class="Keyword">open</a> <a id="27399" class="Keyword">import</a> <a id="27406" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Structured types

<pre class="Agda"><a id="27466" class="Keyword">open</a> <a id="27471" class="Keyword">import</a> <a id="27478" href="structured-types.html" class="Module">structured-types</a>
<a id="27495" class="Keyword">open</a> <a id="27500" class="Keyword">import</a> <a id="27507" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="27571" class="Keyword">open</a> <a id="27576" class="Keyword">import</a> <a id="27583" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="27629" class="Keyword">open</a> <a id="27634" class="Keyword">import</a> <a id="27641" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="27665" class="Keyword">open</a> <a id="27670" class="Keyword">import</a> <a id="27677" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="27746" class="Keyword">open</a> <a id="27751" class="Keyword">import</a> <a id="27758" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="27792" class="Keyword">open</a> <a id="27797" class="Keyword">import</a> <a id="27804" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="27865" class="Keyword">open</a> <a id="27870" class="Keyword">import</a> <a id="27877" href="structured-types.morphisms-wild-unital-magmas.html" class="Module">structured-types.morphisms-wild-unital-magmas</a>
<a id="27923" class="Keyword">open</a> <a id="27928" class="Keyword">import</a> <a id="27935" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="27980" class="Keyword">open</a> <a id="27985" class="Keyword">import</a> <a id="27992" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="28030" class="Keyword">open</a> <a id="28035" class="Keyword">import</a> <a id="28042" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="28085" class="Keyword">open</a> <a id="28090" class="Keyword">import</a> <a id="28097" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="28133" class="Keyword">open</a> <a id="28138" class="Keyword">import</a> <a id="28145" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="28175" class="Keyword">open</a> <a id="28180" class="Keyword">import</a> <a id="28187" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="28218" class="Keyword">open</a> <a id="28223" class="Keyword">import</a> <a id="28230" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="28281" class="Keyword">open</a> <a id="28286" class="Keyword">import</a> <a id="28293" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="28348" class="Keyword">open</a> <a id="28353" class="Keyword">import</a> <a id="28360" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="28389" class="Keyword">open</a> <a id="28394" class="Keyword">import</a> <a id="28401" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="28429" class="Keyword">open</a> <a id="28434" class="Keyword">import</a> <a id="28441" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="28471" class="Keyword">open</a> <a id="28476" class="Keyword">import</a> <a id="28483" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="28517" class="Keyword">open</a> <a id="28522" class="Keyword">import</a> <a id="28529" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
<a id="28562" class="Keyword">open</a> <a id="28567" class="Keyword">import</a> <a id="28574" href="structured-types.wild-unital-magmas.html" class="Module">structured-types.wild-unital-magmas</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="28653" class="Keyword">open</a> <a id="28658" class="Keyword">import</a> <a id="28665" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="28691" class="Keyword">open</a> <a id="28696" class="Keyword">import</a> <a id="28703" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a>
<a id="28742" class="Keyword">open</a> <a id="28747" class="Keyword">import</a> <a id="28754" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="28792" class="Keyword">open</a> <a id="28797" class="Keyword">import</a> <a id="28804" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a>
<a id="28850" class="Keyword">open</a> <a id="28855" class="Keyword">import</a> <a id="28862" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="28899" class="Keyword">open</a> <a id="28904" class="Keyword">import</a> <a id="28911" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="28951" class="Keyword">open</a> <a id="28956" class="Keyword">import</a> <a id="28963" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="29002" class="Keyword">open</a> <a id="29007" class="Keyword">import</a> <a id="29014" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="29047" class="Keyword">open</a> <a id="29052" class="Keyword">import</a> <a id="29059" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a>
<a id="29098" class="Keyword">open</a> <a id="29103" class="Keyword">import</a> <a id="29110" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="29155" class="Keyword">open</a> <a id="29160" class="Keyword">import</a> <a id="29167" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="29219" class="Keyword">open</a> <a id="29224" class="Keyword">import</a> <a id="29231" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="29284" class="Keyword">open</a> <a id="29289" class="Keyword">import</a> <a id="29296" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="29344" class="Keyword">open</a> <a id="29349" class="Keyword">import</a> <a id="29356" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="29396" class="Keyword">open</a> <a id="29401" class="Keyword">import</a> <a id="29408" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="29455" class="Keyword">open</a> <a id="29460" class="Keyword">import</a> <a id="29467" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="29505" class="Keyword">open</a> <a id="29510" class="Keyword">import</a> <a id="29517" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a>
<a id="29550" class="Keyword">open</a> <a id="29555" class="Keyword">import</a> <a id="29562" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="29607" class="Keyword">open</a> <a id="29612" class="Keyword">import</a> <a id="29619" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
</pre>
## Tutorials

<pre class="Agda"><a id="29695" class="Keyword">open</a> <a id="29700" class="Keyword">import</a> <a id="29707" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="29759" class="Keyword">open</a> <a id="29764" class="Keyword">import</a> <a id="29771" href="type-theories.html" class="Module">type-theories</a>
<a id="29785" class="Keyword">open</a> <a id="29790" class="Keyword">import</a> <a id="29797" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="29839" class="Keyword">open</a> <a id="29844" class="Keyword">import</a> <a id="29851" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="29889" class="Keyword">open</a> <a id="29894" class="Keyword">import</a> <a id="29901" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="29947" class="Keyword">open</a> <a id="29952" class="Keyword">import</a> <a id="29959" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="30006" class="Keyword">open</a> <a id="30011" class="Keyword">import</a> <a id="30018" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="30053" class="Keyword">open</a> <a id="30058" class="Keyword">import</a> <a id="30065" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="30143" class="Keyword">open</a> <a id="30148" class="Keyword">import</a> <a id="30155" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="30179" class="Keyword">open</a> <a id="30184" class="Keyword">import</a> <a id="30191" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="30244" class="Keyword">open</a> <a id="30249" class="Keyword">import</a> <a id="30256" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="30299" class="Keyword">open</a> <a id="30304" class="Keyword">import</a> <a id="30311" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="30351" class="Keyword">open</a> <a id="30356" class="Keyword">import</a> <a id="30363" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="30402" class="Keyword">open</a> <a id="30407" class="Keyword">import</a> <a id="30414" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="30462" class="Keyword">open</a> <a id="30467" class="Keyword">import</a> <a id="30474" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="30521" class="Keyword">open</a> <a id="30526" class="Keyword">import</a> <a id="30533" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="30585" class="Keyword">open</a> <a id="30590" class="Keyword">import</a> <a id="30597" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="30637" class="Keyword">open</a> <a id="30642" class="Keyword">import</a> <a id="30649" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="30701" class="Keyword">open</a> <a id="30706" class="Keyword">import</a> <a id="30713" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="30767" class="Keyword">open</a> <a id="30772" class="Keyword">import</a> <a id="30779" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="30827" class="Keyword">open</a> <a id="30832" class="Keyword">import</a> <a id="30839" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="30878" class="Keyword">open</a> <a id="30883" class="Keyword">import</a> <a id="30890" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="30923" class="Keyword">open</a> <a id="30928" class="Keyword">import</a> <a id="30935" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="30965" class="Keyword">open</a> <a id="30970" class="Keyword">import</a> <a id="30977" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="31036" class="Keyword">open</a> <a id="31041" class="Keyword">import</a> <a id="31048" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="31103" class="Keyword">open</a> <a id="31108" class="Keyword">import</a> <a id="31115" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="31162" class="Keyword">open</a> <a id="31167" class="Keyword">import</a> <a id="31174" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="31217" class="Keyword">open</a> <a id="31222" class="Keyword">import</a> <a id="31229" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="31274" class="Keyword">open</a> <a id="31279" class="Keyword">import</a> <a id="31286" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="31335" class="Keyword">open</a> <a id="31340" class="Keyword">import</a> <a id="31347" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="31398" class="Keyword">open</a> <a id="31403" class="Keyword">import</a> <a id="31410" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="31488" class="Keyword">open</a> <a id="31493" class="Keyword">import</a> <a id="31500" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="31540" class="Keyword">open</a> <a id="31545" class="Keyword">import</a> <a id="31552" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="31609" class="Keyword">open</a> <a id="31614" class="Keyword">import</a> <a id="31621" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="31656" class="Keyword">open</a> <a id="31661" class="Keyword">import</a> <a id="31668" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="31714" class="Keyword">open</a> <a id="31719" class="Keyword">import</a> <a id="31726" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="31781" class="Keyword">open</a> <a id="31786" class="Keyword">import</a> <a id="31793" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="31836" class="Keyword">open</a> <a id="31841" class="Keyword">import</a> <a id="31848" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="31907" class="Keyword">open</a> <a id="31912" class="Keyword">import</a> <a id="31919" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="31956" class="Keyword">open</a> <a id="31961" class="Keyword">import</a> <a id="31968" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="32009" class="Keyword">open</a> <a id="32014" class="Keyword">import</a> <a id="32021" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="32060" class="Keyword">open</a> <a id="32065" class="Keyword">import</a> <a id="32072" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="32110" class="Keyword">open</a> <a id="32115" class="Keyword">import</a> <a id="32122" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="32174" class="Keyword">open</a> <a id="32179" class="Keyword">import</a> <a id="32186" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="32231" class="Keyword">open</a> <a id="32236" class="Keyword">import</a> <a id="32243" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="32280" class="Keyword">open</a> <a id="32285" class="Keyword">import</a> <a id="32292" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="32341" class="Keyword">open</a> <a id="32346" class="Keyword">import</a> <a id="32353" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="32392" class="Keyword">open</a> <a id="32397" class="Keyword">import</a> <a id="32404" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="32442" class="Keyword">open</a> <a id="32447" class="Keyword">import</a> <a id="32454" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="32509" class="Keyword">open</a> <a id="32514" class="Keyword">import</a> <a id="32521" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="32560" class="Keyword">open</a> <a id="32565" class="Keyword">import</a> <a id="32572" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="32620" class="Keyword">open</a> <a id="32625" class="Keyword">import</a> <a id="32632" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="32679" class="Keyword">open</a> <a id="32684" class="Keyword">import</a> <a id="32691" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="32729" class="Keyword">open</a> <a id="32734" class="Keyword">import</a> <a id="32741" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="32771" class="Keyword">open</a> <a id="32776" class="Keyword">import</a> <a id="32783" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="32840" class="Keyword">open</a> <a id="32845" class="Keyword">import</a> <a id="32852" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="32906" class="Keyword">open</a> <a id="32911" class="Keyword">import</a> <a id="32918" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="32948" class="Keyword">open</a> <a id="32953" class="Keyword">import</a> <a id="32960" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="33023" class="Keyword">open</a> <a id="33028" class="Keyword">import</a> <a id="33035" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="33078" class="Keyword">open</a> <a id="33083" class="Keyword">import</a> <a id="33090" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="33125" class="Keyword">open</a> <a id="33130" class="Keyword">import</a> <a id="33137" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="33177" class="Keyword">open</a> <a id="33182" class="Keyword">import</a> <a id="33189" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="33234" class="Keyword">open</a> <a id="33239" class="Keyword">import</a> <a id="33246" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="33296" class="Keyword">open</a> <a id="33301" class="Keyword">import</a> <a id="33308" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="33346" class="Keyword">open</a> <a id="33351" class="Keyword">import</a> <a id="33358" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="33407" class="Keyword">open</a> <a id="33412" class="Keyword">import</a> <a id="33419" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="33482" class="Keyword">open</a> <a id="33487" class="Keyword">import</a> <a id="33494" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="33526" class="Keyword">open</a> <a id="33531" class="Keyword">import</a> <a id="33538" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="33591" class="Keyword">open</a> <a id="33596" class="Keyword">import</a> <a id="33603" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="33649" class="Keyword">open</a> <a id="33654" class="Keyword">import</a> <a id="33661" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="33707" class="Keyword">open</a> <a id="33712" class="Keyword">import</a> <a id="33719" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="33767" class="Keyword">open</a> <a id="33772" class="Keyword">import</a> <a id="33779" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="33819" class="Keyword">open</a> <a id="33824" class="Keyword">import</a> <a id="33831" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="33876" class="Keyword">open</a> <a id="33881" class="Keyword">import</a> <a id="33888" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>