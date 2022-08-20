---
title: Univalent mathematics in Agda
---

Welcome to the website of the `agda-unimath` formalization project.

[![CI](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml/badge.svg)](https://github.com/UniMath/agda-unimath/actions/workflows/ci.yaml) [![pages-build-deployment](https://github.com/UniMath/agda-unimath/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/UniMath/agda-unimath/actions/workflows/pages/pages-build-deployment)

The `agda-unimath` library is a new formalisation project for univalent mathematics in Agda. Our goal is to formalize an extensive curriculum of mathematics from the univalent point of view. Furthermore, we think libraries of formalized mathematics have the potential to be useful, and informative resources for mathematicians. Our library is designed to work towards this goal, and we welcome contributions to the library about any topic in mathematics.

The library is built in Agda 2.6.2. It can be compiled by running `make check` from the main folder of the repository.

## Joining the project

Great, you want to contribute something! The best way to start is to find us in our chat channels on the [Univalent Agda discord](https://discord.gg/Zp2e8hYsuX), which is a discord servers shared between the 1Lab, cubical Agda, and agda-unimath. We have a vibing community there, and you're more than welcome to join us just to hang out.

Once you've decided what you want to contribute, the best way to proceed is to make your own fork of the library. Within your fork, make a separate branch in which you will be making your contributions. Now you're ready to start your project! When you've completed your formalization you can proceed by making a pull request. Then we will review your contributions, and merge it when it is ready for the `agda-unimath` library.

## Statement of inclusion

There are many reasons to contribute something to a library of formalized mathematics. Some do it just for fun, some do it for their research, some do it to learn something. Whatever your reason is, we welcome your contributions! To keep the experience of contributing something to our library enjoyable for everyone, we strive for an inclusive community of contributors. You can expect from us that we are kind and respectful in discussions, that we will be mindful of your pronouns and use [inclusive language](https://www.apa.org/about/apa/equity-diversity-inclusion/language-guidelines), and that we value your input regardless of your level of experience or status in the community. We're commited to providing a safe and welcoming environment to people of any gender identity, sexual orientation, race, colour, age, ability, ethnicity, background, or fluency in English -- here on github, in online communication channels, and in person. Homotopy type theory is difficult enough without all the barriers that many of us have to face, so we hope to bring some of those down a bit.

:rainbow: Happy contributing!

Elisabeth Bonnevier
Jonathan Prieto-Cubides
Egbert Rijke

<pre class="Agda"><a id="3062" class="Symbol">{-#</a> <a id="3066" class="Keyword">OPTIONS</a> <a id="3074" class="Pragma">--without-K</a> <a id="3086" class="Pragma">--exact-split</a> <a id="3100" class="Pragma">--guardedness</a> <a id="3114" class="Symbol">#-}</a>
</pre>
See the list of all Agda modules [here](everything.html).

## Category theory

<pre class="Agda"><a id="3210" class="Keyword">open</a> <a id="3215" class="Keyword">import</a> <a id="3222" href="category-theory.html" class="Module">category-theory</a>
<a id="3238" class="Keyword">open</a> <a id="3243" class="Keyword">import</a> <a id="3250" href="category-theory.adjunctions-large-precategories.html" class="Module">category-theory.adjunctions-large-precategories</a>
<a id="3298" class="Keyword">open</a> <a id="3303" class="Keyword">import</a> <a id="3310" href="category-theory.anafunctors.html" class="Module">category-theory.anafunctors</a>
<a id="3338" class="Keyword">open</a> <a id="3343" class="Keyword">import</a> <a id="3350" href="category-theory.categories.html" class="Module">category-theory.categories</a>
<a id="3377" class="Keyword">open</a> <a id="3382" class="Keyword">import</a> <a id="3389" href="category-theory.epimorphisms-large-precategories.html" class="Module">category-theory.epimorphisms-large-precategories</a>
<a id="3438" class="Keyword">open</a> <a id="3443" class="Keyword">import</a> <a id="3450" href="category-theory.equivalences-categories.html" class="Module">category-theory.equivalences-categories</a>
<a id="3490" class="Keyword">open</a> <a id="3495" class="Keyword">import</a> <a id="3502" href="category-theory.equivalences-large-precategories.html" class="Module">category-theory.equivalences-large-precategories</a>
<a id="3551" class="Keyword">open</a> <a id="3556" class="Keyword">import</a> <a id="3563" href="category-theory.equivalences-precategories.html" class="Module">category-theory.equivalences-precategories</a>
<a id="3606" class="Keyword">open</a> <a id="3611" class="Keyword">import</a> <a id="3618" href="category-theory.functors-categories.html" class="Module">category-theory.functors-categories</a>
<a id="3654" class="Keyword">open</a> <a id="3659" class="Keyword">import</a> <a id="3666" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a>
<a id="3711" class="Keyword">open</a> <a id="3716" class="Keyword">import</a> <a id="3723" href="category-theory.functors-precategories.html" class="Module">category-theory.functors-precategories</a>
<a id="3762" class="Keyword">open</a> <a id="3767" class="Keyword">import</a> <a id="3774" href="category-theory.homotopies-natural-transformations-large-precategories.html" class="Module">category-theory.homotopies-natural-transformations-large-precategories</a>
<a id="3845" class="Keyword">open</a> <a id="3850" class="Keyword">import</a> <a id="3857" href="category-theory.initial-objects-precategories.html" class="Module">category-theory.initial-objects-precategories</a>
<a id="3903" class="Keyword">open</a> <a id="3908" class="Keyword">import</a> <a id="3915" href="category-theory.isomorphisms-categories.html" class="Module">category-theory.isomorphisms-categories</a>
<a id="3955" class="Keyword">open</a> <a id="3960" class="Keyword">import</a> <a id="3967" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a>
<a id="4016" class="Keyword">open</a> <a id="4021" class="Keyword">import</a> <a id="4028" href="category-theory.isomorphisms-precategories.html" class="Module">category-theory.isomorphisms-precategories</a>
<a id="4071" class="Keyword">open</a> <a id="4076" class="Keyword">import</a> <a id="4083" href="category-theory.large-categories.html" class="Module">category-theory.large-categories</a>
<a id="4116" class="Keyword">open</a> <a id="4121" class="Keyword">import</a> <a id="4128" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a>
<a id="4164" class="Keyword">open</a> <a id="4169" class="Keyword">import</a> <a id="4176" href="category-theory.monomorphisms-large-precategories.html" class="Module">category-theory.monomorphisms-large-precategories</a>
<a id="4226" class="Keyword">open</a> <a id="4231" class="Keyword">import</a> <a id="4238" href="category-theory.natural-isomorphisms-categories.html" class="Module">category-theory.natural-isomorphisms-categories</a>
<a id="4286" class="Keyword">open</a> <a id="4291" class="Keyword">import</a> <a id="4298" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a>
<a id="4355" class="Keyword">open</a> <a id="4360" class="Keyword">import</a> <a id="4367" href="category-theory.natural-isomorphisms-precategories.html" class="Module">category-theory.natural-isomorphisms-precategories</a>
<a id="4418" class="Keyword">open</a> <a id="4423" class="Keyword">import</a> <a id="4430" href="category-theory.natural-transformations-categories.html" class="Module">category-theory.natural-transformations-categories</a>
<a id="4481" class="Keyword">open</a> <a id="4486" class="Keyword">import</a> <a id="4493" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a>
<a id="4553" class="Keyword">open</a> <a id="4558" class="Keyword">import</a> <a id="4565" href="category-theory.natural-transformations-precategories.html" class="Module">category-theory.natural-transformations-precategories</a>
<a id="4619" class="Keyword">open</a> <a id="4624" class="Keyword">import</a> <a id="4631" href="category-theory.precategories.html" class="Module">category-theory.precategories</a>
<a id="4661" class="Keyword">open</a> <a id="4666" class="Keyword">import</a> <a id="4673" href="category-theory.slice-precategories.html" class="Module">category-theory.slice-precategories</a>
<a id="4709" class="Keyword">open</a> <a id="4714" class="Keyword">import</a> <a id="4721" href="category-theory.terminal-objects-precategories.html" class="Module">category-theory.terminal-objects-precategories</a>
</pre>
## Commutative algebra

<pre class="Agda"><a id="4805" class="Keyword">open</a> <a id="4810" class="Keyword">import</a> <a id="4817" href="commutative-algebra.html" class="Module">commutative-algebra</a>
<a id="4837" class="Keyword">open</a> <a id="4842" class="Keyword">import</a> <a id="4849" href="commutative-algebra.boolean-rings.html" class="Module">commutative-algebra.boolean-rings</a>
<a id="4883" class="Keyword">open</a> <a id="4888" class="Keyword">import</a> <a id="4895" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>
<a id="4933" class="Keyword">open</a> <a id="4938" class="Keyword">import</a> <a id="4945" href="commutative-algebra.discrete-fields.html" class="Module">commutative-algebra.discrete-fields</a>
<a id="4981" class="Keyword">open</a> <a id="4986" class="Keyword">import</a> <a id="4993" href="commutative-algebra.eisenstein-integers.html" class="Module">commutative-algebra.eisenstein-integers</a>
<a id="5033" class="Keyword">open</a> <a id="5038" class="Keyword">import</a> <a id="5045" href="commutative-algebra.gaussian-integers.html" class="Module">commutative-algebra.gaussian-integers</a>
<a id="5083" class="Keyword">open</a> <a id="5088" class="Keyword">import</a> <a id="5095" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a>
<a id="5147" class="Keyword">open</a> <a id="5152" class="Keyword">import</a> <a id="5159" href="commutative-algebra.ideals-commutative-rings.html" class="Module">commutative-algebra.ideals-commutative-rings</a>
<a id="5204" class="Keyword">open</a> <a id="5209" class="Keyword">import</a> <a id="5216" href="commutative-algebra.integral-domains.html" class="Module">commutative-algebra.integral-domains</a>
<a id="5253" class="Keyword">open</a> <a id="5258" class="Keyword">import</a> <a id="5265" href="commutative-algebra.invertible-elements-commutative-rings.html" class="Module">commutative-algebra.invertible-elements-commutative-rings</a>
<a id="5323" class="Keyword">open</a> <a id="5328" class="Keyword">import</a> <a id="5335" href="commutative-algebra.isomorphisms-commutative-rings.html" class="Module">commutative-algebra.isomorphisms-commutative-rings</a>
<a id="5386" class="Keyword">open</a> <a id="5391" class="Keyword">import</a> <a id="5398" href="commutative-algebra.local-commutative-rings.html" class="Module">commutative-algebra.local-commutative-rings</a>
<a id="5442" class="Keyword">open</a> <a id="5447" class="Keyword">import</a> <a id="5454" href="commutative-algebra.maximal-ideals-commutative-rings.html" class="Module">commutative-algebra.maximal-ideals-commutative-rings</a>
<a id="5507" class="Keyword">open</a> <a id="5512" class="Keyword">import</a> <a id="5519" href="commutative-algebra.prime-ideals-commutative-rings.html" class="Module">commutative-algebra.prime-ideals-commutative-rings</a>
<a id="5570" class="Keyword">open</a> <a id="5575" class="Keyword">import</a> <a id="5582" href="commutative-algebra.zariski-topology.html" class="Module">commutative-algebra.zariski-topology</a>
</pre>
## Elementary number theory

<pre class="Agda"><a id="5661" class="Keyword">open</a> <a id="5666" class="Keyword">import</a> <a id="5673" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="5698" class="Keyword">open</a> <a id="5703" class="Keyword">import</a> <a id="5710" href="elementary-number-theory.absolute-value-integers.html" class="Module">elementary-number-theory.absolute-value-integers</a>
<a id="5759" class="Keyword">open</a> <a id="5764" class="Keyword">import</a> <a id="5771" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="5814" class="Keyword">open</a> <a id="5819" class="Keyword">import</a> <a id="5826" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="5876" class="Keyword">open</a> <a id="5881" class="Keyword">import</a> <a id="5888" href="elementary-number-theory.arithmetic-functions.html" class="Module">elementary-number-theory.arithmetic-functions</a>
<a id="5934" class="Keyword">open</a> <a id="5939" class="Keyword">import</a> <a id="5946" href="elementary-number-theory.binomial-coefficients.html" class="Module">elementary-number-theory.binomial-coefficients</a>
<a id="5993" class="Keyword">open</a> <a id="5998" class="Keyword">import</a> <a id="6005" href="elementary-number-theory.bounded-sums-arithmetic-functions.html" class="Module">elementary-number-theory.bounded-sums-arithmetic-functions</a>
<a id="6064" class="Keyword">open</a> <a id="6069" class="Keyword">import</a> <a id="6076" href="elementary-number-theory.catalan-numbers.html" class="Module">elementary-number-theory.catalan-numbers</a>
<a id="6117" class="Keyword">open</a> <a id="6122" class="Keyword">import</a> <a id="6129" href="elementary-number-theory.collatz-bijection.html" class="Module">elementary-number-theory.collatz-bijection</a>
<a id="6172" class="Keyword">open</a> <a id="6177" class="Keyword">import</a> <a id="6184" href="elementary-number-theory.collatz-conjecture.html" class="Module">elementary-number-theory.collatz-conjecture</a>
<a id="6228" class="Keyword">open</a> <a id="6233" class="Keyword">import</a> <a id="6240" href="elementary-number-theory.congruence-integers.html" class="Module">elementary-number-theory.congruence-integers</a>
<a id="6285" class="Keyword">open</a> <a id="6290" class="Keyword">import</a> <a id="6297" href="elementary-number-theory.congruence-natural-numbers.html" class="Module">elementary-number-theory.congruence-natural-numbers</a>
<a id="6349" class="Keyword">open</a> <a id="6354" class="Keyword">import</a> <a id="6361" href="elementary-number-theory.decidable-dependent-function-types.html" class="Module">elementary-number-theory.decidable-dependent-function-types</a>
<a id="6421" class="Keyword">open</a> <a id="6426" class="Keyword">import</a> <a id="6433" href="elementary-number-theory.decidable-types.html" class="Module">elementary-number-theory.decidable-types</a>
<a id="6474" class="Keyword">open</a> <a id="6479" class="Keyword">import</a> <a id="6486" href="elementary-number-theory.difference-integers.html" class="Module">elementary-number-theory.difference-integers</a>
<a id="6531" class="Keyword">open</a> <a id="6536" class="Keyword">import</a> <a id="6543" href="elementary-number-theory.dirichlet-convolution.html" class="Module">elementary-number-theory.dirichlet-convolution</a>
<a id="6590" class="Keyword">open</a> <a id="6595" class="Keyword">import</a> <a id="6602" href="elementary-number-theory.distance-integers.html" class="Module">elementary-number-theory.distance-integers</a>
<a id="6645" class="Keyword">open</a> <a id="6650" class="Keyword">import</a> <a id="6657" href="elementary-number-theory.distance-natural-numbers.html" class="Module">elementary-number-theory.distance-natural-numbers</a>
<a id="6707" class="Keyword">open</a> <a id="6712" class="Keyword">import</a> <a id="6719" href="elementary-number-theory.divisibility-integers.html" class="Module">elementary-number-theory.divisibility-integers</a>
<a id="6766" class="Keyword">open</a> <a id="6771" class="Keyword">import</a> <a id="6778" href="elementary-number-theory.divisibility-modular-arithmetic.html" class="Module">elementary-number-theory.divisibility-modular-arithmetic</a>
<a id="6835" class="Keyword">open</a> <a id="6840" class="Keyword">import</a> <a id="6847" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a>
<a id="6901" class="Keyword">open</a> <a id="6906" class="Keyword">import</a> <a id="6913" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a>
<a id="6973" class="Keyword">open</a> <a id="6978" class="Keyword">import</a> <a id="6985" href="elementary-number-theory.equality-integers.html" class="Module">elementary-number-theory.equality-integers</a>
<a id="7028" class="Keyword">open</a> <a id="7033" class="Keyword">import</a> <a id="7040" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a>
<a id="7090" class="Keyword">open</a> <a id="7095" class="Keyword">import</a> <a id="7102" href="elementary-number-theory.euclidean-division-natural-numbers.html" class="Module">elementary-number-theory.euclidean-division-natural-numbers</a>
<a id="7162" class="Keyword">open</a> <a id="7167" class="Keyword">import</a> <a id="7174" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a>
<a id="7223" class="Keyword">open</a> <a id="7228" class="Keyword">import</a> <a id="7235" href="elementary-number-theory.exponentiation-natural-numbers.html" class="Module">elementary-number-theory.exponentiation-natural-numbers</a>
<a id="7291" class="Keyword">open</a> <a id="7296" class="Keyword">import</a> <a id="7303" href="elementary-number-theory.factorials.html" class="Module">elementary-number-theory.factorials</a>
<a id="7339" class="Keyword">open</a> <a id="7344" class="Keyword">import</a> <a id="7351" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a>
<a id="7395" class="Keyword">open</a> <a id="7400" class="Keyword">import</a> <a id="7407" href="elementary-number-theory.fibonacci-sequence.html" class="Module">elementary-number-theory.fibonacci-sequence</a>
<a id="7451" class="Keyword">open</a> <a id="7456" class="Keyword">import</a> <a id="7463" href="elementary-number-theory.finitary-natural-numbers.html" class="Module">elementary-number-theory.finitary-natural-numbers</a>
<a id="7513" class="Keyword">open</a> <a id="7518" class="Keyword">import</a> <a id="7525" href="elementary-number-theory.finitely-cyclic-maps.html" class="Module">elementary-number-theory.finitely-cyclic-maps</a>
<a id="7571" class="Keyword">open</a> <a id="7576" class="Keyword">import</a> <a id="7583" href="elementary-number-theory.fractions.html" class="Module">elementary-number-theory.fractions</a>
<a id="7618" class="Keyword">open</a> <a id="7623" class="Keyword">import</a> <a id="7630" href="elementary-number-theory.goldbach-conjecture.html" class="Module">elementary-number-theory.goldbach-conjecture</a>
<a id="7675" class="Keyword">open</a> <a id="7680" class="Keyword">import</a> <a id="7687" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a>
<a id="7745" class="Keyword">open</a> <a id="7750" class="Keyword">import</a> <a id="7757" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
<a id="7822" class="Keyword">open</a> <a id="7827" class="Keyword">import</a> <a id="7834" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>
<a id="7877" class="Keyword">open</a> <a id="7882" class="Keyword">import</a> <a id="7889" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="7943" class="Keyword">open</a> <a id="7948" class="Keyword">import</a> <a id="7955" href="elementary-number-theory.half-integers.html" class="Module">elementary-number-theory.half-integers</a>
<a id="7994" class="Keyword">open</a> <a id="7999" class="Keyword">import</a> <a id="8006" href="elementary-number-theory.inequality-integers.html" class="Module">elementary-number-theory.inequality-integers</a>
<a id="8051" class="Keyword">open</a> <a id="8056" class="Keyword">import</a> <a id="8063" href="elementary-number-theory.inequality-natural-numbers.html" class="Module">elementary-number-theory.inequality-natural-numbers</a>
<a id="8115" class="Keyword">open</a> <a id="8120" class="Keyword">import</a> <a id="8127" href="elementary-number-theory.inequality-standard-finite-types.html" class="Module">elementary-number-theory.inequality-standard-finite-types</a>
<a id="8185" class="Keyword">open</a> <a id="8190" class="Keyword">import</a> <a id="8197" href="elementary-number-theory.infinitude-of-primes.html" class="Module">elementary-number-theory.infinitude-of-primes</a>
<a id="8243" class="Keyword">open</a> <a id="8248" class="Keyword">import</a> <a id="8255" href="elementary-number-theory.integer-partitions.html" class="Module">elementary-number-theory.integer-partitions</a>
<a id="8299" class="Keyword">open</a> <a id="8304" class="Keyword">import</a> <a id="8311" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>
<a id="8345" class="Keyword">open</a> <a id="8350" class="Keyword">import</a> <a id="8357" href="elementary-number-theory.lower-bounds-natural-numbers.html" class="Module">elementary-number-theory.lower-bounds-natural-numbers</a>
<a id="8411" class="Keyword">open</a> <a id="8416" class="Keyword">import</a> <a id="8423" href="elementary-number-theory.maximum-natural-numbers.html" class="Module">elementary-number-theory.maximum-natural-numbers</a>
<a id="8472" class="Keyword">open</a> <a id="8477" class="Keyword">import</a> <a id="8484" href="elementary-number-theory.maximum-standard-finite-types.html" class="Module">elementary-number-theory.maximum-standard-finite-types</a>
<a id="8539" class="Keyword">open</a> <a id="8544" class="Keyword">import</a> <a id="8551" href="elementary-number-theory.mersenne-primes.html" class="Module">elementary-number-theory.mersenne-primes</a>
<a id="8592" class="Keyword">open</a> <a id="8597" class="Keyword">import</a> <a id="8604" href="elementary-number-theory.minimum-natural-numbers.html" class="Module">elementary-number-theory.minimum-natural-numbers</a>
<a id="8653" class="Keyword">open</a> <a id="8658" class="Keyword">import</a> <a id="8665" href="elementary-number-theory.minimum-standard-finite-types.html" class="Module">elementary-number-theory.minimum-standard-finite-types</a>
<a id="8720" class="Keyword">open</a> <a id="8725" class="Keyword">import</a> <a id="8732" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a>
<a id="8798" class="Keyword">open</a> <a id="8803" class="Keyword">import</a> <a id="8810" href="elementary-number-theory.modular-arithmetic.html" class="Module">elementary-number-theory.modular-arithmetic</a>
<a id="8854" class="Keyword">open</a> <a id="8859" class="Keyword">import</a> <a id="8866" href="elementary-number-theory.multiplication-integers.html" class="Module">elementary-number-theory.multiplication-integers</a>
<a id="8915" class="Keyword">open</a> <a id="8920" class="Keyword">import</a> <a id="8927" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="8983" class="Keyword">open</a> <a id="8988" class="Keyword">import</a> <a id="8995" href="elementary-number-theory.multiset-coefficients.html" class="Module">elementary-number-theory.multiset-coefficients</a>
<a id="9042" class="Keyword">open</a> <a id="9047" class="Keyword">import</a> <a id="9054" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
<a id="9095" class="Keyword">open</a> <a id="9100" class="Keyword">import</a> <a id="9107" href="elementary-number-theory.nonzero-natural-numbers.html" class="Module">elementary-number-theory.nonzero-natural-numbers</a>
<a id="9156" class="Keyword">open</a> <a id="9161" class="Keyword">import</a> <a id="9168" href="elementary-number-theory.ordinal-induction-natural-numbers.html" class="Module">elementary-number-theory.ordinal-induction-natural-numbers</a>
<a id="9227" class="Keyword">open</a> <a id="9232" class="Keyword">import</a> <a id="9239" href="elementary-number-theory.prime-numbers.html" class="Module">elementary-number-theory.prime-numbers</a>
<a id="9278" class="Keyword">open</a> <a id="9283" class="Keyword">import</a> <a id="9290" href="elementary-number-theory.products-of-natural-numbers.html" class="Module">elementary-number-theory.products-of-natural-numbers</a>
<a id="9343" class="Keyword">open</a> <a id="9348" class="Keyword">import</a> <a id="9355" href="elementary-number-theory.proper-divisors-natural-numbers.html" class="Module">elementary-number-theory.proper-divisors-natural-numbers</a>
<a id="9412" class="Keyword">open</a> <a id="9417" class="Keyword">import</a> <a id="9424" href="elementary-number-theory.pythagorean-triples.html" class="Module">elementary-number-theory.pythagorean-triples</a>
<a id="9469" class="Keyword">open</a> <a id="9474" class="Keyword">import</a> <a id="9481" href="elementary-number-theory.rational-numbers.html" class="Module">elementary-number-theory.rational-numbers</a>
<a id="9523" class="Keyword">open</a> <a id="9528" class="Keyword">import</a> <a id="9535" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a>
<a id="9586" class="Keyword">open</a> <a id="9591" class="Keyword">import</a> <a id="9598" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a>
<a id="9656" class="Keyword">open</a> <a id="9661" class="Keyword">import</a> <a id="9668" href="elementary-number-theory.repeating-element-standard-finite-type.html" class="Module">elementary-number-theory.repeating-element-standard-finite-type</a>
<a id="9732" class="Keyword">open</a> <a id="9737" class="Keyword">import</a> <a id="9744" href="elementary-number-theory.retracts-of-natural-numbers.html" class="Module">elementary-number-theory.retracts-of-natural-numbers</a>
<a id="9797" class="Keyword">open</a> <a id="9802" class="Keyword">import</a> <a id="9809" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a>
<a id="9862" class="Keyword">open</a> <a id="9867" class="Keyword">import</a> <a id="9874" href="elementary-number-theory.stirling-numbers-of-the-second-kind.html" class="Module">elementary-number-theory.stirling-numbers-of-the-second-kind</a>
<a id="9935" class="Keyword">open</a> <a id="9940" class="Keyword">import</a> <a id="9947" href="elementary-number-theory.strong-induction-natural-numbers.html" class="Module">elementary-number-theory.strong-induction-natural-numbers</a>
<a id="10005" class="Keyword">open</a> <a id="10010" class="Keyword">import</a> <a id="10017" href="elementary-number-theory.sums-of-natural-numbers.html" class="Module">elementary-number-theory.sums-of-natural-numbers</a>
<a id="10066" class="Keyword">open</a> <a id="10071" class="Keyword">import</a> <a id="10078" href="elementary-number-theory.telephone-numbers.html" class="Module">elementary-number-theory.telephone-numbers</a>
<a id="10121" class="Keyword">open</a> <a id="10126" class="Keyword">import</a> <a id="10133" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a>
<a id="10177" class="Keyword">open</a> <a id="10182" class="Keyword">import</a> <a id="10189" href="elementary-number-theory.twin-prime-conjecture.html" class="Module">elementary-number-theory.twin-prime-conjecture</a>
<a id="10236" class="Keyword">open</a> <a id="10241" class="Keyword">import</a> <a id="10248" href="elementary-number-theory.unit-elements-standard-finite-types.html" class="Module">elementary-number-theory.unit-elements-standard-finite-types</a>
<a id="10309" class="Keyword">open</a> <a id="10314" class="Keyword">import</a> <a id="10321" href="elementary-number-theory.unit-similarity-standard-finite-types.html" class="Module">elementary-number-theory.unit-similarity-standard-finite-types</a>
<a id="10384" class="Keyword">open</a> <a id="10389" class="Keyword">import</a> <a id="10396" href="elementary-number-theory.universal-property-natural-numbers.html" class="Module">elementary-number-theory.universal-property-natural-numbers</a>
<a id="10456" class="Keyword">open</a> <a id="10461" class="Keyword">import</a> <a id="10468" href="elementary-number-theory.upper-bounds-natural-numbers.html" class="Module">elementary-number-theory.upper-bounds-natural-numbers</a>
<a id="10522" class="Keyword">open</a> <a id="10527" class="Keyword">import</a> <a id="10534" href="elementary-number-theory.well-ordering-principle-natural-numbers.html" class="Module">elementary-number-theory.well-ordering-principle-natural-numbers</a>
<a id="10599" class="Keyword">open</a> <a id="10604" class="Keyword">import</a> <a id="10611" href="elementary-number-theory.well-ordering-principle-standard-finite-types.html" class="Module">elementary-number-theory.well-ordering-principle-standard-finite-types</a>
</pre>
## Finite group theory

<pre class="Agda"><a id="10719" class="Keyword">open</a> <a id="10724" class="Keyword">import</a> <a id="10731" href="finite-group-theory.html" class="Module">finite-group-theory</a>
<a id="10751" class="Keyword">open</a> <a id="10756" class="Keyword">import</a> <a id="10763" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a>
<a id="10809" class="Keyword">open</a> <a id="10814" class="Keyword">import</a> <a id="10821" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a>
<a id="10860" class="Keyword">open</a> <a id="10865" class="Keyword">import</a> <a id="10872" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a>
<a id="10928" class="Keyword">open</a> <a id="10933" class="Keyword">import</a> <a id="10940" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a>
<a id="10986" class="Keyword">open</a> <a id="10991" class="Keyword">import</a> <a id="10998" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>
<a id="11032" class="Keyword">open</a> <a id="11037" class="Keyword">import</a> <a id="11044" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a>
<a id="11079" class="Keyword">open</a> <a id="11084" class="Keyword">import</a> <a id="11091" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a>
<a id="11129" class="Keyword">open</a> <a id="11134" class="Keyword">import</a> <a id="11141" href="finite-group-theory.finite-type-groups.html" class="Module">finite-group-theory.finite-type-groups</a>
<a id="11180" class="Keyword">open</a> <a id="11185" class="Keyword">import</a> <a id="11192" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a>
<a id="11230" class="Keyword">open</a> <a id="11235" class="Keyword">import</a> <a id="11242" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a>
<a id="11282" class="Keyword">open</a> <a id="11287" class="Keyword">import</a> <a id="11294" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a>
<a id="11327" class="Keyword">open</a> <a id="11332" class="Keyword">import</a> <a id="11339" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>
<a id="11377" class="Keyword">open</a> <a id="11382" class="Keyword">import</a> <a id="11389" href="finite-group-theory.simpson-delooping-sign-homomorphism.html" class="Module">finite-group-theory.simpson-delooping-sign-homomorphism</a>
<a id="11445" class="Keyword">open</a> <a id="11450" class="Keyword">import</a> <a id="11457" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="11499" class="Keyword">open</a> <a id="11504" class="Keyword">import</a> <a id="11511" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="11574" class="Keyword">open</a> <a id="11579" class="Keyword">import</a> <a id="11586" href="foundation.html" class="Module">foundation</a>
<a id="11597" class="Keyword">open</a> <a id="11602" class="Keyword">import</a> <a id="11609" href="foundation.0-connected-types.html" class="Module">foundation.0-connected-types</a>
<a id="11638" class="Keyword">open</a> <a id="11643" class="Keyword">import</a> <a id="11650" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a>
<a id="11678" class="Keyword">open</a> <a id="11683" class="Keyword">import</a> <a id="11690" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11708" class="Keyword">open</a> <a id="11713" class="Keyword">import</a> <a id="11720" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11739" class="Keyword">open</a> <a id="11744" class="Keyword">import</a> <a id="11751" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11770" class="Keyword">open</a> <a id="11775" class="Keyword">import</a> <a id="11782" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11826" class="Keyword">open</a> <a id="11831" class="Keyword">import</a> <a id="11838" href="foundation.apartness-relations.html" class="Module">foundation.apartness-relations</a>
<a id="11869" class="Keyword">open</a> <a id="11874" class="Keyword">import</a> <a id="11881" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11906" class="Keyword">open</a> <a id="11911" class="Keyword">import</a> <a id="11918" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="11945" class="Keyword">open</a> <a id="11950" class="Keyword">import</a> <a id="11957" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="11974" class="Keyword">open</a> <a id="11979" class="Keyword">import</a> <a id="11986" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="12015" class="Keyword">open</a> <a id="12020" class="Keyword">import</a> <a id="12027" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="12083" class="Keyword">open</a> <a id="12088" class="Keyword">import</a> <a id="12095" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="12126" class="Keyword">open</a> <a id="12131" class="Keyword">import</a> <a id="12138" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="12192" class="Keyword">open</a> <a id="12197" class="Keyword">import</a> <a id="12204" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="12232" class="Keyword">open</a> <a id="12237" class="Keyword">import</a> <a id="12244" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="12274" class="Keyword">open</a> <a id="12279" class="Keyword">import</a> <a id="12286" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="12306" class="Keyword">open</a> <a id="12311" class="Keyword">import</a> <a id="12318" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="12363" class="Keyword">open</a> <a id="12368" class="Keyword">import</a> <a id="12375" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="12412" class="Keyword">open</a> <a id="12417" class="Keyword">import</a> <a id="12424" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="12459" class="Keyword">open</a> <a id="12464" class="Keyword">import</a> <a id="12471" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="12529" class="Keyword">open</a> <a id="12534" class="Keyword">import</a> <a id="12541" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12579" class="Keyword">open</a> <a id="12584" class="Keyword">import</a> <a id="12591" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12625" class="Keyword">open</a> <a id="12630" class="Keyword">import</a> <a id="12637" href="foundation.commuting-cubes.html" class="Module">foundation.commuting-cubes</a>
<a id="12664" class="Keyword">open</a> <a id="12669" class="Keyword">import</a> <a id="12676" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12705" class="Keyword">open</a> <a id="12710" class="Keyword">import</a> <a id="12717" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12740" class="Keyword">open</a> <a id="12745" class="Keyword">import</a> <a id="12752" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12779" class="Keyword">open</a> <a id="12784" class="Keyword">import</a> <a id="12791" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12814" class="Keyword">open</a> <a id="12819" class="Keyword">import</a> <a id="12826" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12868" class="Keyword">open</a> <a id="12873" class="Keyword">import</a> <a id="12880" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12912" class="Keyword">open</a> <a id="12917" class="Keyword">import</a> <a id="12924" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="12950" class="Keyword">open</a> <a id="12955" class="Keyword">import</a> <a id="12962" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="12989" class="Keyword">open</a> <a id="12994" class="Keyword">import</a> <a id="13001" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="13026" class="Keyword">open</a> <a id="13031" class="Keyword">import</a> <a id="13038" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="13067" class="Keyword">open</a> <a id="13072" class="Keyword">import</a> <a id="13079" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="13109" class="Keyword">open</a> <a id="13114" class="Keyword">import</a> <a id="13121" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="13148" class="Keyword">open</a> <a id="13153" class="Keyword">import</a> <a id="13160" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="13179" class="Keyword">open</a> <a id="13184" class="Keyword">import</a> <a id="13191" href="foundation.cospans.html" class="Module">foundation.cospans</a>
<a id="13210" class="Keyword">open</a> <a id="13215" class="Keyword">import</a> <a id="13222" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="13268" class="Keyword">open</a> <a id="13273" class="Keyword">import</a> <a id="13280" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="13322" class="Keyword">open</a> <a id="13327" class="Keyword">import</a> <a id="13334" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="13366" class="Keyword">open</a> <a id="13371" class="Keyword">import</a> <a id="13378" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="13408" class="Keyword">open</a> <a id="13413" class="Keyword">import</a> <a id="13420" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="13463" class="Keyword">open</a> <a id="13468" class="Keyword">import</a> <a id="13475" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="13501" class="Keyword">open</a> <a id="13506" class="Keyword">import</a> <a id="13513" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="13547" class="Keyword">open</a> <a id="13552" class="Keyword">import</a> <a id="13559" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="13590" class="Keyword">open</a> <a id="13595" class="Keyword">import</a> <a id="13602" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13632" class="Keyword">open</a> <a id="13637" class="Keyword">import</a> <a id="13644" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13671" class="Keyword">open</a> <a id="13676" class="Keyword">import</a> <a id="13683" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13721" class="Keyword">open</a> <a id="13726" class="Keyword">import</a> <a id="13733" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13765" class="Keyword">open</a> <a id="13770" class="Keyword">import</a> <a id="13777" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13812" class="Keyword">open</a> <a id="13817" class="Keyword">import</a> <a id="13824" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13864" class="Keyword">open</a> <a id="13869" class="Keyword">import</a> <a id="13876" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13907" class="Keyword">open</a> <a id="13912" class="Keyword">import</a> <a id="13919" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="13953" class="Keyword">open</a> <a id="13958" class="Keyword">import</a> <a id="13965" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="13994" class="Keyword">open</a> <a id="13999" class="Keyword">import</a> <a id="14006" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="14029" class="Keyword">open</a> <a id="14034" class="Keyword">import</a> <a id="14041" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="14068" class="Keyword">open</a> <a id="14073" class="Keyword">import</a> <a id="14080" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="14108" class="Keyword">open</a> <a id="14113" class="Keyword">import</a> <a id="14120" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="14157" class="Keyword">open</a> <a id="14162" class="Keyword">import</a> <a id="14169" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="14217" class="Keyword">open</a> <a id="14222" class="Keyword">import</a> <a id="14229" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="14269" class="Keyword">open</a> <a id="14274" class="Keyword">import</a> <a id="14281" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="14303" class="Keyword">open</a> <a id="14308" class="Keyword">import</a> <a id="14315" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="14338" class="Keyword">open</a> <a id="14343" class="Keyword">import</a> <a id="14350" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="14375" class="Keyword">open</a> <a id="14380" class="Keyword">import</a> <a id="14387" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="14432" class="Keyword">open</a> <a id="14437" class="Keyword">import</a> <a id="14444" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="14488" class="Keyword">open</a> <a id="14493" class="Keyword">import</a> <a id="14500" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14536" class="Keyword">open</a> <a id="14541" class="Keyword">import</a> <a id="14548" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14593" class="Keyword">open</a> <a id="14598" class="Keyword">import</a> <a id="14605" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14646" class="Keyword">open</a> <a id="14651" class="Keyword">import</a> <a id="14658" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14693" class="Keyword">open</a> <a id="14698" class="Keyword">import</a> <a id="14705" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14737" class="Keyword">open</a> <a id="14742" class="Keyword">import</a> <a id="14749" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14780" class="Keyword">open</a> <a id="14785" class="Keyword">import</a> <a id="14792" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14825" class="Keyword">open</a> <a id="14830" class="Keyword">import</a> <a id="14837" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14870" class="Keyword">open</a> <a id="14875" class="Keyword">import</a> <a id="14882" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14912" class="Keyword">open</a> <a id="14917" class="Keyword">import</a> <a id="14924" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="14948" class="Keyword">open</a> <a id="14953" class="Keyword">import</a> <a id="14960" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="14998" class="Keyword">open</a> <a id="15003" class="Keyword">import</a> <a id="15010" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="15041" class="Keyword">open</a> <a id="15046" class="Keyword">import</a> <a id="15053" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="15078" class="Keyword">open</a> <a id="15083" class="Keyword">import</a> <a id="15090" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="15118" class="Keyword">open</a> <a id="15123" class="Keyword">import</a> <a id="15130" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="15154" class="Keyword">open</a> <a id="15159" class="Keyword">import</a> <a id="15166" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="15192" class="Keyword">open</a> <a id="15197" class="Keyword">import</a> <a id="15204" href="foundation.full-subtypes.html" class="Module">foundation.full-subtypes</a>
<a id="15229" class="Keyword">open</a> <a id="15234" class="Keyword">import</a> <a id="15241" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="15276" class="Keyword">open</a> <a id="15281" class="Keyword">import</a> <a id="15288" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="15309" class="Keyword">open</a> <a id="15314" class="Keyword">import</a> <a id="15321" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="15370" class="Keyword">open</a> <a id="15375" class="Keyword">import</a> <a id="15382" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="15423" class="Keyword">open</a> <a id="15428" class="Keyword">import</a> <a id="15435" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="15485" class="Keyword">open</a> <a id="15490" class="Keyword">import</a> <a id="15497" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="15543" class="Keyword">open</a> <a id="15548" class="Keyword">import</a> <a id="15555" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15595" class="Keyword">open</a> <a id="15600" class="Keyword">import</a> <a id="15607" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15647" class="Keyword">open</a> <a id="15652" class="Keyword">import</a> <a id="15659" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15709" class="Keyword">open</a> <a id="15714" class="Keyword">import</a> <a id="15721" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15760" class="Keyword">open</a> <a id="15765" class="Keyword">import</a> <a id="15772" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15812" class="Keyword">open</a> <a id="15817" class="Keyword">import</a> <a id="15824" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15857" class="Keyword">open</a> <a id="15862" class="Keyword">import</a> <a id="15869" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15918" class="Keyword">open</a> <a id="15923" class="Keyword">import</a> <a id="15930" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="15955" class="Keyword">open</a> <a id="15960" class="Keyword">import</a> <a id="15967" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="16006" class="Keyword">open</a> <a id="16011" class="Keyword">import</a> <a id="16018" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="16056" class="Keyword">open</a> <a id="16061" class="Keyword">import</a> <a id="16068" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="16090" class="Keyword">open</a> <a id="16095" class="Keyword">import</a> <a id="16102" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="16130" class="Keyword">open</a> <a id="16135" class="Keyword">import</a> <a id="16142" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="16178" class="Keyword">open</a> <a id="16183" class="Keyword">import</a> <a id="16190" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="16216" class="Keyword">open</a> <a id="16221" class="Keyword">import</a> <a id="16228" href="foundation.images.html" class="Module">foundation.images</a>
<a id="16246" class="Keyword">open</a> <a id="16251" class="Keyword">import</a> <a id="16258" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="16293" class="Keyword">open</a> <a id="16298" class="Keyword">import</a> <a id="16305" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="16340" class="Keyword">open</a> <a id="16345" class="Keyword">import</a> <a id="16352" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="16379" class="Keyword">open</a> <a id="16384" class="Keyword">import</a> <a id="16391" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="16447" class="Keyword">open</a> <a id="16452" class="Keyword">import</a> <a id="16459" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="16488" class="Keyword">open</a> <a id="16493" class="Keyword">import</a> <a id="16500" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="16530" class="Keyword">open</a> <a id="16535" class="Keyword">import</a> <a id="16542" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="16569" class="Keyword">open</a> <a id="16574" class="Keyword">import</a> <a id="16581" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16607" class="Keyword">open</a> <a id="16612" class="Keyword">import</a> <a id="16619" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16646" class="Keyword">open</a> <a id="16651" class="Keyword">import</a> <a id="16658" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16682" class="Keyword">open</a> <a id="16687" class="Keyword">import</a> <a id="16694" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16717" class="Keyword">open</a> <a id="16722" class="Keyword">import</a> <a id="16729" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16756" class="Keyword">open</a> <a id="16761" class="Keyword">import</a> <a id="16768" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16800" class="Keyword">open</a> <a id="16805" class="Keyword">import</a> <a id="16812" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16847" class="Keyword">open</a> <a id="16852" class="Keyword">import</a> <a id="16859" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16890" class="Keyword">open</a> <a id="16895" class="Keyword">import</a> <a id="16902" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16935" class="Keyword">open</a> <a id="16940" class="Keyword">import</a> <a id="16947" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="16981" class="Keyword">open</a> <a id="16986" class="Keyword">import</a> <a id="16993" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="17033" class="Keyword">open</a> <a id="17038" class="Keyword">import</a> <a id="17045" href="foundation.lesser-limited-principle-of-omniscience.html" class="Module">foundation.lesser-limited-principle-of-omniscience</a>
<a id="17096" class="Keyword">open</a> <a id="17101" class="Keyword">import</a> <a id="17108" href="foundation.limited-principle-of-omniscience.html" class="Module">foundation.limited-principle-of-omniscience</a>
<a id="17152" class="Keyword">open</a> <a id="17157" class="Keyword">import</a> <a id="17164" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="17195" class="Keyword">open</a> <a id="17200" class="Keyword">import</a> <a id="17207" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="17239" class="Keyword">open</a> <a id="17244" class="Keyword">import</a> <a id="17251" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="17282" class="Keyword">open</a> <a id="17287" class="Keyword">import</a> <a id="17294" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="17311" class="Keyword">open</a> <a id="17316" class="Keyword">import</a> <a id="17323" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="17348" class="Keyword">open</a> <a id="17353" class="Keyword">import</a> <a id="17360" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="17389" class="Keyword">open</a> <a id="17394" class="Keyword">import</a> <a id="17401" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="17426" class="Keyword">open</a> <a id="17431" class="Keyword">import</a> <a id="17438" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="17467" class="Keyword">open</a> <a id="17472" class="Keyword">import</a> <a id="17479" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="17500" class="Keyword">open</a> <a id="17505" class="Keyword">import</a> <a id="17512" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="17536" class="Keyword">open</a> <a id="17541" class="Keyword">import</a> <a id="17548" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="17568" class="Keyword">open</a> <a id="17573" class="Keyword">import</a> <a id="17580" href="foundation.noncontractible-types.html" class="Module">foundation.noncontractible-types</a>
<a id="17613" class="Keyword">open</a> <a id="17618" class="Keyword">import</a> <a id="17625" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17663" class="Keyword">open</a> <a id="17668" class="Keyword">import</a> <a id="17675" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17703" class="Keyword">open</a> <a id="17708" class="Keyword">import</a> <a id="17715" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17739" class="Keyword">open</a> <a id="17744" class="Keyword">import</a> <a id="17751" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17778" class="Keyword">open</a> <a id="17783" class="Keyword">import</a> <a id="17790" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17825" class="Keyword">open</a> <a id="17830" class="Keyword">import</a> <a id="17837" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17858" class="Keyword">open</a> <a id="17863" class="Keyword">import</a> <a id="17870" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17906" class="Keyword">open</a> <a id="17911" class="Keyword">import</a> <a id="17918" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="17963" class="Keyword">open</a> <a id="17968" class="Keyword">import</a> <a id="17975" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="18021" class="Keyword">open</a> <a id="18026" class="Keyword">import</a> <a id="18033" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="18073" class="Keyword">open</a> <a id="18078" class="Keyword">import</a> <a id="18085" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="18115" class="Keyword">open</a> <a id="18120" class="Keyword">import</a> <a id="18127" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="18161" class="Keyword">open</a> <a id="18166" class="Keyword">import</a> <a id="18173" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="18210" class="Keyword">open</a> <a id="18215" class="Keyword">import</a> <a id="18222" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="18246" class="Keyword">open</a> <a id="18251" class="Keyword">import</a> <a id="18258" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="18279" class="Keyword">open</a> <a id="18284" class="Keyword">import</a> <a id="18291" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="18326" class="Keyword">open</a> <a id="18331" class="Keyword">import</a> <a id="18338" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="18375" class="Keyword">open</a> <a id="18380" class="Keyword">import</a> <a id="18387" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="18436" class="Keyword">open</a> <a id="18441" class="Keyword">import</a> <a id="18448" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="18481" class="Keyword">open</a> <a id="18486" class="Keyword">import</a> <a id="18493" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="18516" class="Keyword">open</a> <a id="18521" class="Keyword">import</a> <a id="18528" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="18551" class="Keyword">open</a> <a id="18556" class="Keyword">import</a> <a id="18563" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18586" class="Keyword">open</a> <a id="18591" class="Keyword">import</a> <a id="18598" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18626" class="Keyword">open</a> <a id="18631" class="Keyword">import</a> <a id="18638" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18658" class="Keyword">open</a> <a id="18663" class="Keyword">import</a> <a id="18670" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18691" class="Keyword">open</a> <a id="18696" class="Keyword">import</a> <a id="18703" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18734" class="Keyword">open</a> <a id="18739" class="Keyword">import</a> <a id="18746" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18773" class="Keyword">open</a> <a id="18778" class="Keyword">import</a> <a id="18785" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18801" class="Keyword">open</a> <a id="18806" class="Keyword">import</a> <a id="18813" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18844" class="Keyword">open</a> <a id="18849" class="Keyword">import</a> <a id="18856" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18873" class="Keyword">open</a> <a id="18878" class="Keyword">import</a> <a id="18885" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18907" class="Keyword">open</a> <a id="18912" class="Keyword">import</a> <a id="18919" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="18946" class="Keyword">open</a> <a id="18951" class="Keyword">import</a> <a id="18958" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="18981" class="Keyword">open</a> <a id="18986" class="Keyword">import</a> <a id="18993" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="19020" class="Keyword">open</a> <a id="19025" class="Keyword">import</a> <a id="19032" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="19065" class="Keyword">open</a> <a id="19070" class="Keyword">import</a> <a id="19077" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="19117" class="Keyword">open</a> <a id="19122" class="Keyword">import</a> <a id="19129" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="19150" class="Keyword">open</a> <a id="19155" class="Keyword">import</a> <a id="19162" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="19191" class="Keyword">open</a> <a id="19196" class="Keyword">import</a> <a id="19203" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="19241" class="Keyword">open</a> <a id="19246" class="Keyword">import</a> <a id="19253" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="19273" class="Keyword">open</a> <a id="19278" class="Keyword">import</a> <a id="19285" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="19309" class="Keyword">open</a> <a id="19314" class="Keyword">import</a> <a id="19321" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="19348" class="Keyword">open</a> <a id="19353" class="Keyword">import</a> <a id="19360" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="19392" class="Keyword">open</a> <a id="19397" class="Keyword">import</a> <a id="19404" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="19434" class="Keyword">open</a> <a id="19439" class="Keyword">import</a> <a id="19446" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19472" class="Keyword">open</a> <a id="19477" class="Keyword">import</a> <a id="19484" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19511" class="Keyword">open</a> <a id="19516" class="Keyword">import</a> <a id="19523" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19560" class="Keyword">open</a> <a id="19565" class="Keyword">import</a> <a id="19572" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19601" class="Keyword">open</a> <a id="19606" class="Keyword">import</a> <a id="19613" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19636" class="Keyword">open</a> <a id="19641" class="Keyword">import</a> <a id="19648" href="foundation.type-arithmetic-booleans.html" class="Module">foundation.type-arithmetic-booleans</a>
<a id="19684" class="Keyword">open</a> <a id="19689" class="Keyword">import</a> <a id="19696" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19747" class="Keyword">open</a> <a id="19752" class="Keyword">import</a> <a id="19759" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19802" class="Keyword">open</a> <a id="19807" class="Keyword">import</a> <a id="19814" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19866" class="Keyword">open</a> <a id="19871" class="Keyword">import</a> <a id="19878" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19926" class="Keyword">open</a> <a id="19931" class="Keyword">import</a> <a id="19938" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="19976" class="Keyword">open</a> <a id="19981" class="Keyword">import</a> <a id="19988" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="20025" class="Keyword">open</a> <a id="20030" class="Keyword">import</a> <a id="20037" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="20083" class="Keyword">open</a> <a id="20088" class="Keyword">import</a> <a id="20095" href="foundation.union.html" class="Module">foundation.union</a>
<a id="20112" class="Keyword">open</a> <a id="20117" class="Keyword">import</a> <a id="20124" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="20152" class="Keyword">open</a> <a id="20157" class="Keyword">import</a> <a id="20164" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="20192" class="Keyword">open</a> <a id="20197" class="Keyword">import</a> <a id="20204" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="20240" class="Keyword">open</a> <a id="20245" class="Keyword">import</a> <a id="20252" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="20290" class="Keyword">open</a> <a id="20295" class="Keyword">import</a> <a id="20302" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="20335" class="Keyword">open</a> <a id="20340" class="Keyword">import</a> <a id="20347" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="20368" class="Keyword">open</a> <a id="20373" class="Keyword">import</a> <a id="20380" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="20416" class="Keyword">open</a> <a id="20421" class="Keyword">import</a> <a id="20428" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="20482" class="Keyword">open</a> <a id="20487" class="Keyword">import</a> <a id="20494" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20516" class="Keyword">open</a> <a id="20521" class="Keyword">import</a> <a id="20528" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20563" class="Keyword">open</a> <a id="20568" class="Keyword">import</a> <a id="20575" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20605" class="Keyword">open</a> <a id="20610" class="Keyword">import</a> <a id="20617" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20656" class="Keyword">open</a> <a id="20661" class="Keyword">import</a> <a id="20668" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20722" class="Keyword">open</a> <a id="20727" class="Keyword">import</a> <a id="20734" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20780" class="Keyword">open</a> <a id="20785" class="Keyword">import</a> <a id="20792" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20843" class="Keyword">open</a> <a id="20848" class="Keyword">import</a> <a id="20855" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20896" class="Keyword">open</a> <a id="20901" class="Keyword">import</a> <a id="20908" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="20953" class="Keyword">open</a> <a id="20958" class="Keyword">import</a> <a id="20965" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="21010" class="Keyword">open</a> <a id="21015" class="Keyword">import</a> <a id="21022" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="21058" class="Keyword">open</a> <a id="21063" class="Keyword">import</a> <a id="21070" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="21106" class="Keyword">open</a> <a id="21111" class="Keyword">import</a> <a id="21118" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="21183" class="Keyword">open</a> <a id="21188" class="Keyword">import</a> <a id="21195" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="21250" class="Keyword">open</a> <a id="21255" class="Keyword">import</a> <a id="21262" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="21302" class="Keyword">open</a> <a id="21307" class="Keyword">import</a> <a id="21314" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="21358" class="Keyword">open</a> <a id="21363" class="Keyword">import</a> <a id="21370" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="21415" class="Keyword">open</a> <a id="21420" class="Keyword">import</a> <a id="21427" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="21468" class="Keyword">open</a> <a id="21473" class="Keyword">import</a> <a id="21480" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21520" class="Keyword">open</a> <a id="21525" class="Keyword">import</a> <a id="21532" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21559" class="Keyword">open</a> <a id="21564" class="Keyword">import</a> <a id="21571" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21607" class="Keyword">open</a> <a id="21612" class="Keyword">import</a> <a id="21619" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21646" class="Keyword">open</a> <a id="21651" class="Keyword">import</a> <a id="21658" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21695" class="Keyword">open</a> <a id="21700" class="Keyword">import</a> <a id="21707" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21735" class="Keyword">open</a> <a id="21740" class="Keyword">import</a> <a id="21747" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21766" class="Keyword">open</a> <a id="21771" class="Keyword">import</a> <a id="21778" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21818" class="Keyword">open</a> <a id="21823" class="Keyword">import</a> <a id="21830" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="21879" class="Keyword">open</a> <a id="21884" class="Keyword">import</a> <a id="21891" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21923" class="Keyword">open</a> <a id="21928" class="Keyword">import</a> <a id="21935" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="21983" class="Keyword">open</a> <a id="21988" class="Keyword">import</a> <a id="21995" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="22018" class="Keyword">open</a> <a id="22023" class="Keyword">import</a> <a id="22030" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="22054" class="Keyword">open</a> <a id="22059" class="Keyword">import</a> <a id="22066" href="foundation-core.automorphisms.html" class="Module">foundation-core.automorphisms</a>
<a id="22096" class="Keyword">open</a> <a id="22101" class="Keyword">import</a> <a id="22108" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="22148" class="Keyword">open</a> <a id="22153" class="Keyword">import</a> <a id="22160" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22203" class="Keyword">open</a> <a id="22208" class="Keyword">import</a> <a id="22215" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22249" class="Keyword">open</a> <a id="22254" class="Keyword">import</a> <a id="22261" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22293" class="Keyword">open</a> <a id="22298" class="Keyword">import</a> <a id="22305" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22335" class="Keyword">open</a> <a id="22340" class="Keyword">import</a> <a id="22347" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22381" class="Keyword">open</a> <a id="22386" class="Keyword">import</a> <a id="22393" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22428" class="Keyword">open</a> <a id="22433" class="Keyword">import</a> <a id="22440" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22464" class="Keyword">open</a> <a id="22469" class="Keyword">import</a> <a id="22476" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22513" class="Keyword">open</a> <a id="22518" class="Keyword">import</a> <a id="22525" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22552" class="Keyword">open</a> <a id="22557" class="Keyword">import</a> <a id="22564" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22592" class="Keyword">open</a> <a id="22597" class="Keyword">import</a> <a id="22604" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22634" class="Keyword">open</a> <a id="22639" class="Keyword">import</a> <a id="22646" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22695" class="Keyword">open</a> <a id="22700" class="Keyword">import</a> <a id="22707" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22753" class="Keyword">open</a> <a id="22758" class="Keyword">import</a> <a id="22765" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22805" class="Keyword">open</a> <a id="22810" class="Keyword">import</a> <a id="22817" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22855" class="Keyword">open</a> <a id="22860" class="Keyword">import</a> <a id="22867" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22896" class="Keyword">open</a> <a id="22901" class="Keyword">import</a> <a id="22908" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22938" class="Keyword">open</a> <a id="22943" class="Keyword">import</a> <a id="22950" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="22981" class="Keyword">open</a> <a id="22986" class="Keyword">import</a> <a id="22993" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="23033" class="Keyword">open</a> <a id="23038" class="Keyword">import</a> <a id="23045" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="23071" class="Keyword">open</a> <a id="23076" class="Keyword">import</a> <a id="23083" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="23138" class="Keyword">open</a> <a id="23143" class="Keyword">import</a> <a id="23150" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23201" class="Keyword">open</a> <a id="23206" class="Keyword">import</a> <a id="23213" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23258" class="Keyword">open</a> <a id="23263" class="Keyword">import</a> <a id="23270" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23315" class="Keyword">open</a> <a id="23320" class="Keyword">import</a> <a id="23327" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23381" class="Keyword">open</a> <a id="23386" class="Keyword">import</a> <a id="23393" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23420" class="Keyword">open</a> <a id="23425" class="Keyword">import</a> <a id="23432" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23465" class="Keyword">open</a> <a id="23470" class="Keyword">import</a> <a id="23477" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23508" class="Keyword">open</a> <a id="23513" class="Keyword">import</a> <a id="23520" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23557" class="Keyword">open</a> <a id="23562" class="Keyword">import</a> <a id="23569" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23603" class="Keyword">open</a> <a id="23608" class="Keyword">import</a> <a id="23615" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23640" class="Keyword">open</a> <a id="23645" class="Keyword">import</a> <a id="23652" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23684" class="Keyword">open</a> <a id="23689" class="Keyword">import</a> <a id="23696" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23731" class="Keyword">open</a> <a id="23736" class="Keyword">import</a> <a id="23743" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23772" class="Keyword">open</a> <a id="23777" class="Keyword">import</a> <a id="23784" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23810" class="Keyword">open</a> <a id="23815" class="Keyword">import</a> <a id="23822" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23850" class="Keyword">open</a> <a id="23855" class="Keyword">import</a> <a id="23862" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23887" class="Keyword">open</a> <a id="23892" class="Keyword">import</a> <a id="23899" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23920" class="Keyword">open</a> <a id="23925" class="Keyword">import</a> <a id="23932" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="23968" class="Keyword">open</a> <a id="23973" class="Keyword">import</a> <a id="23980" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="24023" class="Keyword">open</a> <a id="24028" class="Keyword">import</a> <a id="24035" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="24060" class="Keyword">open</a> <a id="24065" class="Keyword">import</a> <a id="24072" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="24103" class="Keyword">open</a> <a id="24108" class="Keyword">import</a> <a id="24115" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="24147" class="Keyword">open</a> <a id="24152" class="Keyword">import</a> <a id="24159" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24193" class="Keyword">open</a> <a id="24198" class="Keyword">import</a> <a id="24205" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24261" class="Keyword">open</a> <a id="24266" class="Keyword">import</a> <a id="24273" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24326" class="Keyword">open</a> <a id="24331" class="Keyword">import</a> <a id="24338" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24365" class="Keyword">open</a> <a id="24370" class="Keyword">import</a> <a id="24377" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24422" class="Keyword">open</a> <a id="24427" class="Keyword">import</a> <a id="24434" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24496" class="Keyword">open</a> <a id="24501" class="Keyword">import</a> <a id="24508" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24521" class="Keyword">open</a> <a id="24526" class="Keyword">import</a> <a id="24533" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24573" class="Keyword">open</a> <a id="24578" class="Keyword">import</a> <a id="24585" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24629" class="Keyword">open</a> <a id="24634" class="Keyword">import</a> <a id="24641" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24680" class="Keyword">open</a> <a id="24685" class="Keyword">import</a> <a id="24692" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24734" class="Keyword">open</a> <a id="24739" class="Keyword">import</a> <a id="24746" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24786" class="Keyword">open</a> <a id="24791" class="Keyword">import</a> <a id="24798" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24839" class="Keyword">open</a> <a id="24844" class="Keyword">import</a> <a id="24851" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24889" class="Keyword">open</a> <a id="24894" class="Keyword">import</a> <a id="24901" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="24964" class="Keyword">open</a> <a id="24969" class="Keyword">import</a> <a id="24976" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="25005" class="Keyword">open</a> <a id="25010" class="Keyword">import</a> <a id="25017" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="25062" class="Keyword">open</a> <a id="25067" class="Keyword">import</a> <a id="25074" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="25116" class="Keyword">open</a> <a id="25121" class="Keyword">import</a> <a id="25128" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25168" class="Keyword">open</a> <a id="25173" class="Keyword">import</a> <a id="25180" href="graph-theory.equivalences-enriched-undirected-graphs.html" class="Module">graph-theory.equivalences-enriched-undirected-graphs</a>
<a id="25233" class="Keyword">open</a> <a id="25238" class="Keyword">import</a> <a id="25245" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25289" class="Keyword">open</a> <a id="25294" class="Keyword">import</a> <a id="25301" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25350" class="Keyword">open</a> <a id="25355" class="Keyword">import</a> <a id="25362" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25412" class="Keyword">open</a> <a id="25417" class="Keyword">import</a> <a id="25424" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25451" class="Keyword">open</a> <a id="25456" class="Keyword">import</a> <a id="25463" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25488" class="Keyword">open</a> <a id="25493" class="Keyword">import</a> <a id="25500" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25523" class="Keyword">open</a> <a id="25528" class="Keyword">import</a> <a id="25535" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25584" class="Keyword">open</a> <a id="25589" class="Keyword">import</a> <a id="25596" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25635" class="Keyword">open</a> <a id="25640" class="Keyword">import</a> <a id="25647" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25688" class="Keyword">open</a> <a id="25693" class="Keyword">import</a> <a id="25700" href="graph-theory.neighbors-undirected-graphs.html" class="Module">graph-theory.neighbors-undirected-graphs</a>
<a id="25741" class="Keyword">open</a> <a id="25746" class="Keyword">import</a> <a id="25753" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25797" class="Keyword">open</a> <a id="25802" class="Keyword">import</a> <a id="25809" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25846" class="Keyword">open</a> <a id="25851" class="Keyword">import</a> <a id="25858" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="25880" class="Keyword">open</a> <a id="25885" class="Keyword">import</a> <a id="25892" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="25922" class="Keyword">open</a> <a id="25927" class="Keyword">import</a> <a id="25934" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="25973" class="Keyword">open</a> <a id="25978" class="Keyword">import</a> <a id="25985" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="26016" class="Keyword">open</a> <a id="26021" class="Keyword">import</a> <a id="26028" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="26054" class="Keyword">open</a> <a id="26059" class="Keyword">import</a> <a id="26066" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="26104" class="Keyword">open</a> <a id="26109" class="Keyword">import</a> <a id="26116" href="graph-theory.stereoisomerism-enriched-undirected-graphs.html" class="Module">graph-theory.stereoisomerism-enriched-undirected-graphs</a>
<a id="26172" class="Keyword">open</a> <a id="26177" class="Keyword">import</a> <a id="26184" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="26242" class="Keyword">open</a> <a id="26247" class="Keyword">import</a> <a id="26254" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="26292" class="Keyword">open</a> <a id="26297" class="Keyword">import</a> <a id="26304" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26323" class="Keyword">open</a> <a id="26328" class="Keyword">import</a> <a id="26335" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26400" class="Keyword">open</a> <a id="26405" class="Keyword">import</a> <a id="26412" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26443" class="Keyword">open</a> <a id="26448" class="Keyword">import</a> <a id="26455" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26482" class="Keyword">open</a> <a id="26487" class="Keyword">import</a> <a id="26494" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26522" class="Keyword">open</a> <a id="26527" class="Keyword">import</a> <a id="26534" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26601" class="Keyword">open</a> <a id="26606" class="Keyword">import</a> <a id="26613" href="group-theory.html" class="Module">group-theory</a>
<a id="26626" class="Keyword">open</a> <a id="26631" class="Keyword">import</a> <a id="26638" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26666" class="Keyword">open</a> <a id="26671" class="Keyword">import</a> <a id="26678" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26729" class="Keyword">open</a> <a id="26734" class="Keyword">import</a> <a id="26741" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="26774" class="Keyword">open</a> <a id="26779" class="Keyword">import</a> <a id="26786" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26833" class="Keyword">open</a> <a id="26838" class="Keyword">import</a> <a id="26845" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26884" class="Keyword">open</a> <a id="26889" class="Keyword">import</a> <a id="26896" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="26936" class="Keyword">open</a> <a id="26941" class="Keyword">import</a> <a id="26948" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="26991" class="Keyword">open</a> <a id="26996" class="Keyword">import</a> <a id="27003" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="27035" class="Keyword">open</a> <a id="27040" class="Keyword">import</a> <a id="27047" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="27083" class="Keyword">open</a> <a id="27088" class="Keyword">import</a> <a id="27095" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="27124" class="Keyword">open</a> <a id="27129" class="Keyword">import</a> <a id="27136" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="27164" class="Keyword">open</a> <a id="27169" class="Keyword">import</a> <a id="27176" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="27209" class="Keyword">open</a> <a id="27214" class="Keyword">import</a> <a id="27221" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="27257" class="Keyword">open</a> <a id="27262" class="Keyword">import</a> <a id="27269" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27298" class="Keyword">open</a> <a id="27303" class="Keyword">import</a> <a id="27310" href="group-theory.congruence-relations-groups.html" class="Module">group-theory.congruence-relations-groups</a>
<a id="27351" class="Keyword">open</a> <a id="27356" class="Keyword">import</a> <a id="27363" href="group-theory.congruence-relations-monoids.html" class="Module">group-theory.congruence-relations-monoids</a>
<a id="27405" class="Keyword">open</a> <a id="27410" class="Keyword">import</a> <a id="27417" href="group-theory.congruence-relations-semigroups.html" class="Module">group-theory.congruence-relations-semigroups</a>
<a id="27462" class="Keyword">open</a> <a id="27467" class="Keyword">import</a> <a id="27474" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27499" class="Keyword">open</a> <a id="27504" class="Keyword">import</a> <a id="27511" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27573" class="Keyword">open</a> <a id="27578" class="Keyword">import</a> <a id="27585" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27626" class="Keyword">open</a> <a id="27631" class="Keyword">import</a> <a id="27638" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27667" class="Keyword">open</a> <a id="27672" class="Keyword">import</a> <a id="27679" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27703" class="Keyword">open</a> <a id="27708" class="Keyword">import</a> <a id="27715" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27746" class="Keyword">open</a> <a id="27751" class="Keyword">import</a> <a id="27758" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27805" class="Keyword">open</a> <a id="27810" class="Keyword">import</a> <a id="27817" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="27850" class="Keyword">open</a> <a id="27855" class="Keyword">import</a> <a id="27862" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="27911" class="Keyword">open</a> <a id="27916" class="Keyword">import</a> <a id="27923" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="27963" class="Keyword">open</a> <a id="27968" class="Keyword">import</a> <a id="27975" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="28015" class="Keyword">open</a> <a id="28020" class="Keyword">import</a> <a id="28027" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="28064" class="Keyword">open</a> <a id="28069" class="Keyword">import</a> <a id="28076" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="28123" class="Keyword">open</a> <a id="28128" class="Keyword">import</a> <a id="28135" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="28176" class="Keyword">open</a> <a id="28181" class="Keyword">import</a> <a id="28188" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="28232" class="Keyword">open</a> <a id="28237" class="Keyword">import</a> <a id="28244" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="28283" class="Keyword">open</a> <a id="28288" class="Keyword">import</a> <a id="28295" href="group-theory.full-subgroups.html" class="Module">group-theory.full-subgroups</a>
<a id="28323" class="Keyword">open</a> <a id="28328" class="Keyword">import</a> <a id="28335" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28367" class="Keyword">open</a> <a id="28372" class="Keyword">import</a> <a id="28379" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28406" class="Keyword">open</a> <a id="28411" class="Keyword">import</a> <a id="28418" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28438" class="Keyword">open</a> <a id="28443" class="Keyword">import</a> <a id="28450" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28484" class="Keyword">open</a> <a id="28489" class="Keyword">import</a> <a id="28496" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28523" class="Keyword">open</a> <a id="28528" class="Keyword">import</a> <a id="28535" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28577" class="Keyword">open</a> <a id="28582" class="Keyword">import</a> <a id="28589" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28639" class="Keyword">open</a> <a id="28644" class="Keyword">import</a> <a id="28651" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28698" class="Keyword">open</a> <a id="28703" class="Keyword">import</a> <a id="28710" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28751" class="Keyword">open</a> <a id="28756" class="Keyword">import</a> <a id="28763" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28797" class="Keyword">open</a> <a id="28802" class="Keyword">import</a> <a id="28809" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="28857" class="Keyword">open</a> <a id="28862" class="Keyword">import</a> <a id="28869" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="28910" class="Keyword">open</a> <a id="28915" class="Keyword">import</a> <a id="28922" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="28957" class="Keyword">open</a> <a id="28962" class="Keyword">import</a> <a id="28969" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="29007" class="Keyword">open</a> <a id="29012" class="Keyword">import</a> <a id="29019" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="29054" class="Keyword">open</a> <a id="29059" class="Keyword">import</a> <a id="29066" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="29098" class="Keyword">open</a> <a id="29103" class="Keyword">import</a> <a id="29110" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="29151" class="Keyword">open</a> <a id="29156" class="Keyword">import</a> <a id="29163" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="29204" class="Keyword">open</a> <a id="29209" class="Keyword">import</a> <a id="29216" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="29256" class="Keyword">open</a> <a id="29261" class="Keyword">import</a> <a id="29268" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="29301" class="Keyword">open</a> <a id="29306" class="Keyword">import</a> <a id="29313" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29350" class="Keyword">open</a> <a id="29355" class="Keyword">import</a> <a id="29362" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29392" class="Keyword">open</a> <a id="29397" class="Keyword">import</a> <a id="29404" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29425" class="Keyword">open</a> <a id="29430" class="Keyword">import</a> <a id="29437" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29491" class="Keyword">open</a> <a id="29496" class="Keyword">import</a> <a id="29503" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29548" class="Keyword">open</a> <a id="29553" class="Keyword">import</a> <a id="29560" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29588" class="Keyword">open</a> <a id="29593" class="Keyword">import</a> <a id="29600" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29621" class="Keyword">open</a> <a id="29626" class="Keyword">import</a> <a id="29633" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29676" class="Keyword">open</a> <a id="29681" class="Keyword">import</a> <a id="29688" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29722" class="Keyword">open</a> <a id="29727" class="Keyword">import</a> <a id="29734" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29764" class="Keyword">open</a> <a id="29769" class="Keyword">import</a> <a id="29776" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29822" class="Keyword">open</a> <a id="29827" class="Keyword">import</a> <a id="29834" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="29888" class="Keyword">open</a> <a id="29893" class="Keyword">import</a> <a id="29900" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="29943" class="Keyword">open</a> <a id="29948" class="Keyword">import</a> <a id="29955" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="29989" class="Keyword">open</a> <a id="29994" class="Keyword">import</a> <a id="30001" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="30042" class="Keyword">open</a> <a id="30047" class="Keyword">import</a> <a id="30054" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="30089" class="Keyword">open</a> <a id="30094" class="Keyword">import</a> <a id="30101" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a>
<a id="30140" class="Keyword">open</a> <a id="30145" class="Keyword">import</a> <a id="30152" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="30194" class="Keyword">open</a> <a id="30199" class="Keyword">import</a> <a id="30206" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="30241" class="Keyword">open</a> <a id="30246" class="Keyword">import</a> <a id="30253" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="30292" class="Keyword">open</a> <a id="30297" class="Keyword">import</a> <a id="30304" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="30341" class="Keyword">open</a> <a id="30346" class="Keyword">import</a> <a id="30353" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30400" class="Keyword">open</a> <a id="30405" class="Keyword">import</a> <a id="30412" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30476" class="Keyword">open</a> <a id="30481" class="Keyword">import</a> <a id="30488" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30533" class="Keyword">open</a> <a id="30538" class="Keyword">import</a> <a id="30545" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30569" class="Keyword">open</a> <a id="30574" class="Keyword">import</a> <a id="30581" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30606" class="Keyword">open</a> <a id="30611" class="Keyword">import</a> <a id="30618" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30661" class="Keyword">open</a> <a id="30666" class="Keyword">import</a> <a id="30673" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30704" class="Keyword">open</a> <a id="30709" class="Keyword">import</a> <a id="30716" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30770" class="Keyword">open</a> <a id="30775" class="Keyword">import</a> <a id="30782" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30805" class="Keyword">open</a> <a id="30810" class="Keyword">import</a> <a id="30817" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="30855" class="Keyword">open</a> <a id="30860" class="Keyword">import</a> <a id="30867" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="30906" class="Keyword">open</a> <a id="30911" class="Keyword">import</a> <a id="30918" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="30969" class="Keyword">open</a> <a id="30974" class="Keyword">import</a> <a id="30981" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="31018" class="Keyword">open</a> <a id="31023" class="Keyword">import</a> <a id="31030" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="31054" class="Keyword">open</a> <a id="31059" class="Keyword">import</a> <a id="31066" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="31093" class="Keyword">open</a> <a id="31098" class="Keyword">import</a> <a id="31105" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="31162" class="Keyword">open</a> <a id="31167" class="Keyword">import</a> <a id="31174" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="31222" class="Keyword">open</a> <a id="31227" class="Keyword">import</a> <a id="31234" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="31264" class="Keyword">open</a> <a id="31269" class="Keyword">import</a> <a id="31276" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="31313" class="Keyword">open</a> <a id="31318" class="Keyword">import</a> <a id="31325" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="31346" class="Keyword">open</a> <a id="31351" class="Keyword">import</a> <a id="31358" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31405" class="Keyword">open</a> <a id="31410" class="Keyword">import</a> <a id="31417" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31455" class="Keyword">open</a> <a id="31460" class="Keyword">import</a> <a id="31467" href="group-theory.trivial-subgroups.html" class="Module">group-theory.trivial-subgroups</a>
<a id="31498" class="Keyword">open</a> <a id="31503" class="Keyword">import</a> <a id="31510" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31604" class="Keyword">open</a> <a id="31609" class="Keyword">import</a> <a id="31616" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31631" class="Keyword">open</a> <a id="31636" class="Keyword">import</a> <a id="31643" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31676" class="Keyword">open</a> <a id="31681" class="Keyword">import</a> <a id="31688" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="31720" class="Keyword">open</a> <a id="31725" class="Keyword">import</a> <a id="31732" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="31774" class="Keyword">open</a> <a id="31779" class="Keyword">import</a> <a id="31786" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="31824" class="Keyword">open</a> <a id="31829" class="Keyword">import</a> <a id="31836" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="31873" class="Keyword">open</a> <a id="31878" class="Keyword">import</a> <a id="31885" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="31918" class="Keyword">open</a> <a id="31923" class="Keyword">import</a> <a id="31930" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="31954" class="Keyword">open</a> <a id="31959" class="Keyword">import</a> <a id="31966" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="32005" class="Keyword">open</a> <a id="32010" class="Keyword">import</a> <a id="32017" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="32063" class="Keyword">open</a> <a id="32068" class="Keyword">import</a> <a id="32075" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="32120" class="Keyword">open</a> <a id="32125" class="Keyword">import</a> <a id="32132" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="32170" class="Keyword">open</a> <a id="32175" class="Keyword">import</a> <a id="32182" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="32214" class="Keyword">open</a> <a id="32219" class="Keyword">import</a> <a id="32226" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="32279" class="Keyword">open</a> <a id="32284" class="Keyword">import</a> <a id="32291" href="order-theory.html" class="Module">order-theory</a>
<a id="32304" class="Keyword">open</a> <a id="32309" class="Keyword">import</a> <a id="32316" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="32343" class="Keyword">open</a> <a id="32348" class="Keyword">import</a> <a id="32355" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="32385" class="Keyword">open</a> <a id="32390" class="Keyword">import</a> <a id="32397" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32430" class="Keyword">open</a> <a id="32435" class="Keyword">import</a> <a id="32442" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32478" class="Keyword">open</a> <a id="32483" class="Keyword">import</a> <a id="32490" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32525" class="Keyword">open</a> <a id="32530" class="Keyword">import</a> <a id="32537" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32564" class="Keyword">open</a> <a id="32569" class="Keyword">import</a> <a id="32576" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32606" class="Keyword">open</a> <a id="32611" class="Keyword">import</a> <a id="32618" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32654" class="Keyword">open</a> <a id="32659" class="Keyword">import</a> <a id="32666" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="32708" class="Keyword">open</a> <a id="32713" class="Keyword">import</a> <a id="32720" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32750" class="Keyword">open</a> <a id="32755" class="Keyword">import</a> <a id="32762" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="32794" class="Keyword">open</a> <a id="32799" class="Keyword">import</a> <a id="32806" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="32837" class="Keyword">open</a> <a id="32842" class="Keyword">import</a> <a id="32849" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="32875" class="Keyword">open</a> <a id="32880" class="Keyword">import</a> <a id="32887" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="32916" class="Keyword">open</a> <a id="32921" class="Keyword">import</a> <a id="32928" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="32965" class="Keyword">open</a> <a id="32970" class="Keyword">import</a> <a id="32977" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="33017" class="Keyword">open</a> <a id="33022" class="Keyword">import</a> <a id="33029" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="33051" class="Keyword">open</a> <a id="33056" class="Keyword">import</a> <a id="33063" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="33098" class="Keyword">open</a> <a id="33103" class="Keyword">import</a> <a id="33110" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="33148" class="Keyword">open</a> <a id="33153" class="Keyword">import</a> <a id="33160" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="33199" class="Keyword">open</a> <a id="33204" class="Keyword">import</a> <a id="33211" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="33246" class="Keyword">open</a> <a id="33251" class="Keyword">import</a> <a id="33258" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="33293" class="Keyword">open</a> <a id="33298" class="Keyword">import</a> <a id="33305" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="33340" class="Keyword">open</a> <a id="33345" class="Keyword">import</a> <a id="33352" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="33390" class="Keyword">open</a> <a id="33395" class="Keyword">import</a> <a id="33402" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33433" class="Keyword">open</a> <a id="33438" class="Keyword">import</a> <a id="33445" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33487" class="Keyword">open</a> <a id="33492" class="Keyword">import</a> <a id="33499" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33544" class="Keyword">open</a> <a id="33549" class="Keyword">import</a> <a id="33556" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33589" class="Keyword">open</a> <a id="33594" class="Keyword">import</a> <a id="33601" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33621" class="Keyword">open</a> <a id="33626" class="Keyword">import</a> <a id="33633" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33656" class="Keyword">open</a> <a id="33661" class="Keyword">import</a> <a id="33668" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="33691" class="Keyword">open</a> <a id="33696" class="Keyword">import</a> <a id="33703" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33729" class="Keyword">open</a> <a id="33734" class="Keyword">import</a> <a id="33741" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33767" class="Keyword">open</a> <a id="33772" class="Keyword">import</a> <a id="33779" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="33843" class="Keyword">open</a> <a id="33848" class="Keyword">import</a> <a id="33855" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="33873" class="Keyword">open</a> <a id="33878" class="Keyword">import</a> <a id="33885" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="33912" class="Keyword">open</a> <a id="33917" class="Keyword">import</a> <a id="33924" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="33950" class="Keyword">open</a> <a id="33955" class="Keyword">import</a> <a id="33962" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="33988" class="Keyword">open</a> <a id="33993" class="Keyword">import</a> <a id="34000" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="34026" class="Keyword">open</a> <a id="34031" class="Keyword">import</a> <a id="34038" href="organic-chemistry.ethane.html" class="Module">organic-chemistry.ethane</a>
<a id="34063" class="Keyword">open</a> <a id="34068" class="Keyword">import</a> <a id="34075" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="34106" class="Keyword">open</a> <a id="34111" class="Keyword">import</a> <a id="34118" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="34144" class="Keyword">open</a> <a id="34149" class="Keyword">import</a> <a id="34156" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="34219" class="Keyword">open</a> <a id="34224" class="Keyword">import</a> <a id="34231" href="polytopes.html" class="Module">polytopes</a>
<a id="34241" class="Keyword">open</a> <a id="34246" class="Keyword">import</a> <a id="34253" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="34311" class="Keyword">open</a> <a id="34316" class="Keyword">import</a> <a id="34323" href="ring-theory.html" class="Module">ring-theory</a>
<a id="34335" class="Keyword">open</a> <a id="34340" class="Keyword">import</a> <a id="34347" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="34384" class="Keyword">open</a> <a id="34389" class="Keyword">import</a> <a id="34396" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="34423" class="Keyword">open</a> <a id="34428" class="Keyword">import</a> <a id="34435" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34467" class="Keyword">open</a> <a id="34472" class="Keyword">import</a> <a id="34479" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34525" class="Keyword">open</a> <a id="34530" class="Keyword">import</a> <a id="34537" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34562" class="Keyword">open</a> <a id="34567" class="Keyword">import</a> <a id="34574" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34612" class="Keyword">open</a> <a id="34617" class="Keyword">import</a> <a id="34624" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34667" class="Keyword">open</a> <a id="34672" class="Keyword">import</a> <a id="34679" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="34717" class="Keyword">open</a> <a id="34722" class="Keyword">import</a> <a id="34729" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="34760" class="Keyword">open</a> <a id="34765" class="Keyword">import</a> <a id="34772" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="34796" class="Keyword">open</a> <a id="34801" class="Keyword">import</a> <a id="34808" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="34840" class="Keyword">open</a> <a id="34845" class="Keyword">import</a> <a id="34852" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="34878" class="Keyword">open</a> <a id="34883" class="Keyword">import</a> <a id="34890" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="34919" class="Keyword">open</a> <a id="34924" class="Keyword">import</a> <a id="34931" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="34968" class="Keyword">open</a> <a id="34973" class="Keyword">import</a> <a id="34980" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="35009" class="Keyword">open</a> <a id="35014" class="Keyword">import</a> <a id="35021" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="35048" class="Keyword">open</a> <a id="35053" class="Keyword">import</a> <a id="35060" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="35097" class="Keyword">open</a> <a id="35102" class="Keyword">import</a> <a id="35109" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="35136" class="Keyword">open</a> <a id="35141" class="Keyword">import</a> <a id="35148" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="35181" class="Keyword">open</a> <a id="35186" class="Keyword">import</a> <a id="35193" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="35211" class="Keyword">open</a> <a id="35216" class="Keyword">import</a> <a id="35223" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="35277" class="Keyword">open</a> <a id="35282" class="Keyword">import</a> <a id="35289" href="set-theory.html" class="Module">set-theory</a>
<a id="35300" class="Keyword">open</a> <a id="35305" class="Keyword">import</a> <a id="35312" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="35335" class="Keyword">open</a> <a id="35340" class="Keyword">import</a> <a id="35347" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="35371" class="Keyword">open</a> <a id="35376" class="Keyword">import</a> <a id="35383" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="35408" class="Keyword">open</a> <a id="35413" class="Keyword">import</a> <a id="35420" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="35446" class="Keyword">open</a> <a id="35451" class="Keyword">import</a> <a id="35458" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35520" class="Keyword">open</a> <a id="35525" class="Keyword">import</a> <a id="35532" href="structured-types.html" class="Module">structured-types</a>
<a id="35549" class="Keyword">open</a> <a id="35554" class="Keyword">import</a> <a id="35561" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35596" class="Keyword">open</a> <a id="35601" class="Keyword">import</a> <a id="35608" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35652" class="Keyword">open</a> <a id="35657" class="Keyword">import</a> <a id="35664" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="35728" class="Keyword">open</a> <a id="35733" class="Keyword">import</a> <a id="35740" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="35779" class="Keyword">open</a> <a id="35784" class="Keyword">import</a> <a id="35791" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="35837" class="Keyword">open</a> <a id="35842" class="Keyword">import</a> <a id="35849" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="35914" class="Keyword">open</a> <a id="35919" class="Keyword">import</a> <a id="35926" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="35950" class="Keyword">open</a> <a id="35955" class="Keyword">import</a> <a id="35962" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="36031" class="Keyword">open</a> <a id="36036" class="Keyword">import</a> <a id="36043" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="36088" class="Keyword">open</a> <a id="36093" class="Keyword">import</a> <a id="36100" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="36134" class="Keyword">open</a> <a id="36139" class="Keyword">import</a> <a id="36146" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="36207" class="Keyword">open</a> <a id="36212" class="Keyword">import</a> <a id="36219" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="36264" class="Keyword">open</a> <a id="36269" class="Keyword">import</a> <a id="36276" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="36314" class="Keyword">open</a> <a id="36319" class="Keyword">import</a> <a id="36326" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="36369" class="Keyword">open</a> <a id="36374" class="Keyword">import</a> <a id="36381" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="36417" class="Keyword">open</a> <a id="36422" class="Keyword">import</a> <a id="36429" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36459" class="Keyword">open</a> <a id="36464" class="Keyword">import</a> <a id="36471" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36505" class="Keyword">open</a> <a id="36510" class="Keyword">import</a> <a id="36517" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36548" class="Keyword">open</a> <a id="36553" class="Keyword">import</a> <a id="36560" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36619" class="Keyword">open</a> <a id="36624" class="Keyword">import</a> <a id="36631" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="36682" class="Keyword">open</a> <a id="36687" class="Keyword">import</a> <a id="36694" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="36745" class="Keyword">open</a> <a id="36750" class="Keyword">import</a> <a id="36757" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="36812" class="Keyword">open</a> <a id="36817" class="Keyword">import</a> <a id="36824" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="36856" class="Keyword">open</a> <a id="36861" class="Keyword">import</a> <a id="36868" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="36897" class="Keyword">open</a> <a id="36902" class="Keyword">import</a> <a id="36909" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="36937" class="Keyword">open</a> <a id="36942" class="Keyword">import</a> <a id="36949" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="36979" class="Keyword">open</a> <a id="36984" class="Keyword">import</a> <a id="36991" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="37025" class="Keyword">open</a> <a id="37030" class="Keyword">import</a> <a id="37037" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="37113" class="Keyword">open</a> <a id="37118" class="Keyword">import</a> <a id="37125" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="37151" class="Keyword">open</a> <a id="37156" class="Keyword">import</a> <a id="37163" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="37201" class="Keyword">open</a> <a id="37206" class="Keyword">import</a> <a id="37213" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="37250" class="Keyword">open</a> <a id="37255" class="Keyword">import</a> <a id="37262" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="37302" class="Keyword">open</a> <a id="37307" class="Keyword">import</a> <a id="37314" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="37353" class="Keyword">open</a> <a id="37358" class="Keyword">import</a> <a id="37365" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="37398" class="Keyword">open</a> <a id="37403" class="Keyword">import</a> <a id="37410" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="37453" class="Keyword">open</a> <a id="37458" class="Keyword">import</a> <a id="37465" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37500" class="Keyword">open</a> <a id="37505" class="Keyword">import</a> <a id="37512" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37557" class="Keyword">open</a> <a id="37562" class="Keyword">import</a> <a id="37569" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37606" class="Keyword">open</a> <a id="37611" class="Keyword">import</a> <a id="37618" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37670" class="Keyword">open</a> <a id="37675" class="Keyword">import</a> <a id="37682" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="37735" class="Keyword">open</a> <a id="37740" class="Keyword">import</a> <a id="37747" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="37807" class="Keyword">open</a> <a id="37812" class="Keyword">import</a> <a id="37819" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="37867" class="Keyword">open</a> <a id="37872" class="Keyword">import</a> <a id="37879" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="37919" class="Keyword">open</a> <a id="37924" class="Keyword">import</a> <a id="37931" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="37978" class="Keyword">open</a> <a id="37983" class="Keyword">import</a> <a id="37990" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="38031" class="Keyword">open</a> <a id="38036" class="Keyword">import</a> <a id="38043" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="38081" class="Keyword">open</a> <a id="38086" class="Keyword">import</a> <a id="38093" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="38141" class="Keyword">open</a> <a id="38146" class="Keyword">import</a> <a id="38153" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="38190" class="Keyword">open</a> <a id="38195" class="Keyword">import</a> <a id="38202" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="38237" class="Keyword">open</a> <a id="38242" class="Keyword">import</a> <a id="38249" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="38283" class="Keyword">open</a> <a id="38288" class="Keyword">import</a> <a id="38295" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="38342" class="Keyword">open</a> <a id="38347" class="Keyword">import</a> <a id="38354" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="38399" class="Keyword">open</a> <a id="38404" class="Keyword">import</a> <a id="38411" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38460" class="Keyword">open</a> <a id="38465" class="Keyword">import</a> <a id="38472" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38524" class="Keyword">open</a> <a id="38529" class="Keyword">import</a> <a id="38536" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38590" class="Keyword">open</a> <a id="38595" class="Keyword">import</a> <a id="38602" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Tutorials

<pre class="Agda"><a id="38679" class="Keyword">open</a> <a id="38684" class="Keyword">import</a> <a id="38691" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a>
</pre>
## Type theories

<pre class="Agda"><a id="38743" class="Keyword">open</a> <a id="38748" class="Keyword">import</a> <a id="38755" href="type-theories.html" class="Module">type-theories</a>
<a id="38769" class="Keyword">open</a> <a id="38774" class="Keyword">import</a> <a id="38781" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="38823" class="Keyword">open</a> <a id="38828" class="Keyword">import</a> <a id="38835" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="38873" class="Keyword">open</a> <a id="38878" class="Keyword">import</a> <a id="38885" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="38931" class="Keyword">open</a> <a id="38936" class="Keyword">import</a> <a id="38943" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="38990" class="Keyword">open</a> <a id="38995" class="Keyword">import</a> <a id="39002" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="39037" class="Keyword">open</a> <a id="39042" class="Keyword">import</a> <a id="39049" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="39127" class="Keyword">open</a> <a id="39132" class="Keyword">import</a> <a id="39139" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="39163" class="Keyword">open</a> <a id="39168" class="Keyword">import</a> <a id="39175" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="39228" class="Keyword">open</a> <a id="39233" class="Keyword">import</a> <a id="39240" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="39283" class="Keyword">open</a> <a id="39288" class="Keyword">import</a> <a id="39295" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="39335" class="Keyword">open</a> <a id="39340" class="Keyword">import</a> <a id="39347" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="39386" class="Keyword">open</a> <a id="39391" class="Keyword">import</a> <a id="39398" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="39432" class="Keyword">open</a> <a id="39437" class="Keyword">import</a> <a id="39444" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39492" class="Keyword">open</a> <a id="39497" class="Keyword">import</a> <a id="39504" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39555" class="Keyword">open</a> <a id="39560" class="Keyword">import</a> <a id="39567" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39614" class="Keyword">open</a> <a id="39619" class="Keyword">import</a> <a id="39626" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39678" class="Keyword">open</a> <a id="39683" class="Keyword">import</a> <a id="39690" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39734" class="Keyword">open</a> <a id="39739" class="Keyword">import</a> <a id="39746" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="39786" class="Keyword">open</a> <a id="39791" class="Keyword">import</a> <a id="39798" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="39841" class="Keyword">open</a> <a id="39846" class="Keyword">import</a> <a id="39853" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="39905" class="Keyword">open</a> <a id="39910" class="Keyword">import</a> <a id="39917" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="39971" class="Keyword">open</a> <a id="39976" class="Keyword">import</a> <a id="39983" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="40031" class="Keyword">open</a> <a id="40036" class="Keyword">import</a> <a id="40043" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="40082" class="Keyword">open</a> <a id="40087" class="Keyword">import</a> <a id="40094" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="40127" class="Keyword">open</a> <a id="40132" class="Keyword">import</a> <a id="40139" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="40169" class="Keyword">open</a> <a id="40174" class="Keyword">import</a> <a id="40181" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="40232" class="Keyword">open</a> <a id="40237" class="Keyword">import</a> <a id="40244" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="40285" class="Keyword">open</a> <a id="40290" class="Keyword">import</a> <a id="40297" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="40334" class="Keyword">open</a> <a id="40339" class="Keyword">import</a> <a id="40346" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="40405" class="Keyword">open</a> <a id="40410" class="Keyword">import</a> <a id="40417" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40472" class="Keyword">open</a> <a id="40477" class="Keyword">import</a> <a id="40484" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40540" class="Keyword">open</a> <a id="40545" class="Keyword">import</a> <a id="40552" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40599" class="Keyword">open</a> <a id="40604" class="Keyword">import</a> <a id="40611" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40654" class="Keyword">open</a> <a id="40659" class="Keyword">import</a> <a id="40666" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40711" class="Keyword">open</a> <a id="40716" class="Keyword">import</a> <a id="40723" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="40772" class="Keyword">open</a> <a id="40777" class="Keyword">import</a> <a id="40784" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="40835" class="Keyword">open</a> <a id="40840" class="Keyword">import</a> <a id="40847" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="40891" class="Keyword">open</a> <a id="40896" class="Keyword">import</a> <a id="40903" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="40981" class="Keyword">open</a> <a id="40986" class="Keyword">import</a> <a id="40993" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="41033" class="Keyword">open</a> <a id="41038" class="Keyword">import</a> <a id="41045" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="41102" class="Keyword">open</a> <a id="41107" class="Keyword">import</a> <a id="41114" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="41149" class="Keyword">open</a> <a id="41154" class="Keyword">import</a> <a id="41161" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="41207" class="Keyword">open</a> <a id="41212" class="Keyword">import</a> <a id="41219" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="41274" class="Keyword">open</a> <a id="41279" class="Keyword">import</a> <a id="41286" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="41329" class="Keyword">open</a> <a id="41334" class="Keyword">import</a> <a id="41341" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="41386" class="Keyword">open</a> <a id="41391" class="Keyword">import</a> <a id="41398" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41457" class="Keyword">open</a> <a id="41462" class="Keyword">import</a> <a id="41469" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41506" class="Keyword">open</a> <a id="41511" class="Keyword">import</a> <a id="41518" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41560" class="Keyword">open</a> <a id="41565" class="Keyword">import</a> <a id="41572" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41613" class="Keyword">open</a> <a id="41618" class="Keyword">import</a> <a id="41625" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41664" class="Keyword">open</a> <a id="41669" class="Keyword">import</a> <a id="41676" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41714" class="Keyword">open</a> <a id="41719" class="Keyword">import</a> <a id="41726" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="41778" class="Keyword">open</a> <a id="41783" class="Keyword">import</a> <a id="41790" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="41835" class="Keyword">open</a> <a id="41840" class="Keyword">import</a> <a id="41847" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="41886" class="Keyword">open</a> <a id="41891" class="Keyword">import</a> <a id="41898" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="41935" class="Keyword">open</a> <a id="41940" class="Keyword">import</a> <a id="41947" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="41996" class="Keyword">open</a> <a id="42001" class="Keyword">import</a> <a id="42008" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="42047" class="Keyword">open</a> <a id="42052" class="Keyword">import</a> <a id="42059" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="42097" class="Keyword">open</a> <a id="42102" class="Keyword">import</a> <a id="42109" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="42164" class="Keyword">open</a> <a id="42169" class="Keyword">import</a> <a id="42176" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="42215" class="Keyword">open</a> <a id="42220" class="Keyword">import</a> <a id="42227" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="42275" class="Keyword">open</a> <a id="42280" class="Keyword">import</a> <a id="42287" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="42334" class="Keyword">open</a> <a id="42339" class="Keyword">import</a> <a id="42346" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="42384" class="Keyword">open</a> <a id="42389" class="Keyword">import</a> <a id="42396" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="42426" class="Keyword">open</a> <a id="42431" class="Keyword">import</a> <a id="42438" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42495" class="Keyword">open</a> <a id="42500" class="Keyword">import</a> <a id="42507" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42561" class="Keyword">open</a> <a id="42566" class="Keyword">import</a> <a id="42573" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42603" class="Keyword">open</a> <a id="42608" class="Keyword">import</a> <a id="42615" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42664" class="Keyword">open</a> <a id="42669" class="Keyword">import</a> <a id="42676" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42718" class="Keyword">open</a> <a id="42723" class="Keyword">import</a> <a id="42730" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="42764" class="Keyword">open</a> <a id="42769" class="Keyword">import</a> <a id="42776" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="42839" class="Keyword">open</a> <a id="42844" class="Keyword">import</a> <a id="42851" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="42894" class="Keyword">open</a> <a id="42899" class="Keyword">import</a> <a id="42906" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="42941" class="Keyword">open</a> <a id="42946" class="Keyword">import</a> <a id="42953" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="42988" class="Keyword">open</a> <a id="42993" class="Keyword">import</a> <a id="43000" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="43040" class="Keyword">open</a> <a id="43045" class="Keyword">import</a> <a id="43052" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="43097" class="Keyword">open</a> <a id="43102" class="Keyword">import</a> <a id="43109" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="43150" class="Keyword">open</a> <a id="43155" class="Keyword">import</a> <a id="43162" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="43216" class="Keyword">open</a> <a id="43221" class="Keyword">import</a> <a id="43228" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="43278" class="Keyword">open</a> <a id="43283" class="Keyword">import</a> <a id="43290" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="43337" class="Keyword">open</a> <a id="43342" class="Keyword">import</a> <a id="43349" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="43387" class="Keyword">open</a> <a id="43392" class="Keyword">import</a> <a id="43399" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="43448" class="Keyword">open</a> <a id="43453" class="Keyword">import</a> <a id="43460" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43507" class="Keyword">open</a> <a id="43512" class="Keyword">import</a> <a id="43519" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43582" class="Keyword">open</a> <a id="43587" class="Keyword">import</a> <a id="43594" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43626" class="Keyword">open</a> <a id="43631" class="Keyword">import</a> <a id="43638" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43691" class="Keyword">open</a> <a id="43696" class="Keyword">import</a> <a id="43703" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="43749" class="Keyword">open</a> <a id="43754" class="Keyword">import</a> <a id="43761" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="43807" class="Keyword">open</a> <a id="43812" class="Keyword">import</a> <a id="43819" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="43859" class="Keyword">open</a> <a id="43864" class="Keyword">import</a> <a id="43871" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="43918" class="Keyword">open</a> <a id="43923" class="Keyword">import</a> <a id="43930" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="43978" class="Keyword">open</a> <a id="43983" class="Keyword">import</a> <a id="43990" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="44030" class="Keyword">open</a> <a id="44035" class="Keyword">import</a> <a id="44042" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="44087" class="Keyword">open</a> <a id="44092" class="Keyword">import</a> <a id="44099" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="44164" class="Keyword">open</a> <a id="44169" class="Keyword">import</a> <a id="44176" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="44221" class="Keyword">open</a> <a id="44226" class="Keyword">import</a> <a id="44233" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="44280" class="Keyword">open</a> <a id="44285" class="Keyword">import</a> <a id="44292" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="44345" class="Keyword">open</a> <a id="44350" class="Keyword">import</a> <a id="44357" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>