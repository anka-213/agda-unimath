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
<a id="11445" class="Keyword">open</a> <a id="11450" class="Keyword">import</a> <a id="11457" href="finite-group-theory.subgroups-finite-groups.html" class="Module">finite-group-theory.subgroups-finite-groups</a>
<a id="11501" class="Keyword">open</a> <a id="11506" class="Keyword">import</a> <a id="11513" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a>
<a id="11555" class="Keyword">open</a> <a id="11560" class="Keyword">import</a> <a id="11567" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a>
</pre>
## Foundation

<pre class="Agda"><a id="11630" class="Keyword">open</a> <a id="11635" class="Keyword">import</a> <a id="11642" href="foundation.html" class="Module">foundation</a>
<a id="11653" class="Keyword">open</a> <a id="11658" class="Keyword">import</a> <a id="11665" href="foundation.0-connected-types.html" class="Module">foundation.0-connected-types</a>
<a id="11694" class="Keyword">open</a> <a id="11699" class="Keyword">import</a> <a id="11706" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a>
<a id="11734" class="Keyword">open</a> <a id="11739" class="Keyword">import</a> <a id="11746" href="foundation.0-maps.html" class="Module">foundation.0-maps</a>
<a id="11764" class="Keyword">open</a> <a id="11769" class="Keyword">import</a> <a id="11776" href="foundation.1-types.html" class="Module">foundation.1-types</a>
<a id="11795" class="Keyword">open</a> <a id="11800" class="Keyword">import</a> <a id="11807" href="foundation.2-types.html" class="Module">foundation.2-types</a>
<a id="11826" class="Keyword">open</a> <a id="11831" class="Keyword">import</a> <a id="11838" href="foundation.algebras-polynomial-endofunctors.html" class="Module">foundation.algebras-polynomial-endofunctors</a>
<a id="11882" class="Keyword">open</a> <a id="11887" class="Keyword">import</a> <a id="11894" href="foundation.apartness-relations.html" class="Module">foundation.apartness-relations</a>
<a id="11925" class="Keyword">open</a> <a id="11930" class="Keyword">import</a> <a id="11937" href="foundation.automorphisms.html" class="Module">foundation.automorphisms</a>
<a id="11962" class="Keyword">open</a> <a id="11967" class="Keyword">import</a> <a id="11974" href="foundation.axiom-l.html" class="Module">foundation.axiom-l</a>
<a id="11993" class="Keyword">open</a> <a id="11998" class="Keyword">import</a> <a id="12005" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="12032" class="Keyword">open</a> <a id="12037" class="Keyword">import</a> <a id="12044" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="12061" class="Keyword">open</a> <a id="12066" class="Keyword">import</a> <a id="12073" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="12102" class="Keyword">open</a> <a id="12107" class="Keyword">import</a> <a id="12114" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="12170" class="Keyword">open</a> <a id="12175" class="Keyword">import</a> <a id="12182" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="12213" class="Keyword">open</a> <a id="12218" class="Keyword">import</a> <a id="12225" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="12279" class="Keyword">open</a> <a id="12284" class="Keyword">import</a> <a id="12291" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="12319" class="Keyword">open</a> <a id="12324" class="Keyword">import</a> <a id="12331" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="12361" class="Keyword">open</a> <a id="12366" class="Keyword">import</a> <a id="12373" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="12393" class="Keyword">open</a> <a id="12398" class="Keyword">import</a> <a id="12405" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="12450" class="Keyword">open</a> <a id="12455" class="Keyword">import</a> <a id="12462" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="12499" class="Keyword">open</a> <a id="12504" class="Keyword">import</a> <a id="12511" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="12546" class="Keyword">open</a> <a id="12551" class="Keyword">import</a> <a id="12558" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="12616" class="Keyword">open</a> <a id="12621" class="Keyword">import</a> <a id="12628" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12666" class="Keyword">open</a> <a id="12671" class="Keyword">import</a> <a id="12678" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12712" class="Keyword">open</a> <a id="12717" class="Keyword">import</a> <a id="12724" href="foundation.commuting-cubes.html" class="Module">foundation.commuting-cubes</a>
<a id="12751" class="Keyword">open</a> <a id="12756" class="Keyword">import</a> <a id="12763" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12792" class="Keyword">open</a> <a id="12797" class="Keyword">import</a> <a id="12804" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12827" class="Keyword">open</a> <a id="12832" class="Keyword">import</a> <a id="12839" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12866" class="Keyword">open</a> <a id="12871" class="Keyword">import</a> <a id="12878" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12901" class="Keyword">open</a> <a id="12906" class="Keyword">import</a> <a id="12913" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12955" class="Keyword">open</a> <a id="12960" class="Keyword">import</a> <a id="12967" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12999" class="Keyword">open</a> <a id="13004" class="Keyword">import</a> <a id="13011" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="13037" class="Keyword">open</a> <a id="13042" class="Keyword">import</a> <a id="13049" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="13076" class="Keyword">open</a> <a id="13081" class="Keyword">import</a> <a id="13088" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="13113" class="Keyword">open</a> <a id="13118" class="Keyword">import</a> <a id="13125" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="13154" class="Keyword">open</a> <a id="13159" class="Keyword">import</a> <a id="13166" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="13196" class="Keyword">open</a> <a id="13201" class="Keyword">import</a> <a id="13208" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="13235" class="Keyword">open</a> <a id="13240" class="Keyword">import</a> <a id="13247" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="13266" class="Keyword">open</a> <a id="13271" class="Keyword">import</a> <a id="13278" href="foundation.cospans.html" class="Module">foundation.cospans</a>
<a id="13297" class="Keyword">open</a> <a id="13302" class="Keyword">import</a> <a id="13309" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="13355" class="Keyword">open</a> <a id="13360" class="Keyword">import</a> <a id="13367" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="13409" class="Keyword">open</a> <a id="13414" class="Keyword">import</a> <a id="13421" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="13453" class="Keyword">open</a> <a id="13458" class="Keyword">import</a> <a id="13465" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="13495" class="Keyword">open</a> <a id="13500" class="Keyword">import</a> <a id="13507" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="13550" class="Keyword">open</a> <a id="13555" class="Keyword">import</a> <a id="13562" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="13588" class="Keyword">open</a> <a id="13593" class="Keyword">import</a> <a id="13600" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="13634" class="Keyword">open</a> <a id="13639" class="Keyword">import</a> <a id="13646" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="13677" class="Keyword">open</a> <a id="13682" class="Keyword">import</a> <a id="13689" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13719" class="Keyword">open</a> <a id="13724" class="Keyword">import</a> <a id="13731" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13758" class="Keyword">open</a> <a id="13763" class="Keyword">import</a> <a id="13770" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13808" class="Keyword">open</a> <a id="13813" class="Keyword">import</a> <a id="13820" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13852" class="Keyword">open</a> <a id="13857" class="Keyword">import</a> <a id="13864" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13899" class="Keyword">open</a> <a id="13904" class="Keyword">import</a> <a id="13911" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13951" class="Keyword">open</a> <a id="13956" class="Keyword">import</a> <a id="13963" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13994" class="Keyword">open</a> <a id="13999" class="Keyword">import</a> <a id="14006" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="14040" class="Keyword">open</a> <a id="14045" class="Keyword">import</a> <a id="14052" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="14081" class="Keyword">open</a> <a id="14086" class="Keyword">import</a> <a id="14093" href="foundation.discrete-reflexive-relations.html" class="Module">foundation.discrete-reflexive-relations</a>
<a id="14133" class="Keyword">open</a> <a id="14138" class="Keyword">import</a> <a id="14145" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="14168" class="Keyword">open</a> <a id="14173" class="Keyword">import</a> <a id="14180" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="14207" class="Keyword">open</a> <a id="14212" class="Keyword">import</a> <a id="14219" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="14247" class="Keyword">open</a> <a id="14252" class="Keyword">import</a> <a id="14259" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="14296" class="Keyword">open</a> <a id="14301" class="Keyword">import</a> <a id="14308" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="14356" class="Keyword">open</a> <a id="14361" class="Keyword">import</a> <a id="14368" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="14408" class="Keyword">open</a> <a id="14413" class="Keyword">import</a> <a id="14420" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="14442" class="Keyword">open</a> <a id="14447" class="Keyword">import</a> <a id="14454" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="14477" class="Keyword">open</a> <a id="14482" class="Keyword">import</a> <a id="14489" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="14514" class="Keyword">open</a> <a id="14519" class="Keyword">import</a> <a id="14526" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="14571" class="Keyword">open</a> <a id="14576" class="Keyword">import</a> <a id="14583" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="14627" class="Keyword">open</a> <a id="14632" class="Keyword">import</a> <a id="14639" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14675" class="Keyword">open</a> <a id="14680" class="Keyword">import</a> <a id="14687" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14732" class="Keyword">open</a> <a id="14737" class="Keyword">import</a> <a id="14744" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14785" class="Keyword">open</a> <a id="14790" class="Keyword">import</a> <a id="14797" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14832" class="Keyword">open</a> <a id="14837" class="Keyword">import</a> <a id="14844" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14876" class="Keyword">open</a> <a id="14881" class="Keyword">import</a> <a id="14888" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14919" class="Keyword">open</a> <a id="14924" class="Keyword">import</a> <a id="14931" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14964" class="Keyword">open</a> <a id="14969" class="Keyword">import</a> <a id="14976" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="15009" class="Keyword">open</a> <a id="15014" class="Keyword">import</a> <a id="15021" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="15051" class="Keyword">open</a> <a id="15056" class="Keyword">import</a> <a id="15063" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="15087" class="Keyword">open</a> <a id="15092" class="Keyword">import</a> <a id="15099" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="15137" class="Keyword">open</a> <a id="15142" class="Keyword">import</a> <a id="15149" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="15180" class="Keyword">open</a> <a id="15185" class="Keyword">import</a> <a id="15192" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="15217" class="Keyword">open</a> <a id="15222" class="Keyword">import</a> <a id="15229" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="15257" class="Keyword">open</a> <a id="15262" class="Keyword">import</a> <a id="15269" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="15293" class="Keyword">open</a> <a id="15298" class="Keyword">import</a> <a id="15305" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="15331" class="Keyword">open</a> <a id="15336" class="Keyword">import</a> <a id="15343" href="foundation.full-subtypes.html" class="Module">foundation.full-subtypes</a>
<a id="15368" class="Keyword">open</a> <a id="15373" class="Keyword">import</a> <a id="15380" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="15415" class="Keyword">open</a> <a id="15420" class="Keyword">import</a> <a id="15427" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="15448" class="Keyword">open</a> <a id="15453" class="Keyword">import</a> <a id="15460" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="15509" class="Keyword">open</a> <a id="15514" class="Keyword">import</a> <a id="15521" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="15562" class="Keyword">open</a> <a id="15567" class="Keyword">import</a> <a id="15574" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="15624" class="Keyword">open</a> <a id="15629" class="Keyword">import</a> <a id="15636" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="15682" class="Keyword">open</a> <a id="15687" class="Keyword">import</a> <a id="15694" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15734" class="Keyword">open</a> <a id="15739" class="Keyword">import</a> <a id="15746" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15786" class="Keyword">open</a> <a id="15791" class="Keyword">import</a> <a id="15798" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15848" class="Keyword">open</a> <a id="15853" class="Keyword">import</a> <a id="15860" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15899" class="Keyword">open</a> <a id="15904" class="Keyword">import</a> <a id="15911" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15951" class="Keyword">open</a> <a id="15956" class="Keyword">import</a> <a id="15963" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15996" class="Keyword">open</a> <a id="16001" class="Keyword">import</a> <a id="16008" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="16057" class="Keyword">open</a> <a id="16062" class="Keyword">import</a> <a id="16069" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="16094" class="Keyword">open</a> <a id="16099" class="Keyword">import</a> <a id="16106" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="16145" class="Keyword">open</a> <a id="16150" class="Keyword">import</a> <a id="16157" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="16195" class="Keyword">open</a> <a id="16200" class="Keyword">import</a> <a id="16207" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="16229" class="Keyword">open</a> <a id="16234" class="Keyword">import</a> <a id="16241" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="16269" class="Keyword">open</a> <a id="16274" class="Keyword">import</a> <a id="16281" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="16317" class="Keyword">open</a> <a id="16322" class="Keyword">import</a> <a id="16329" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="16355" class="Keyword">open</a> <a id="16360" class="Keyword">import</a> <a id="16367" href="foundation.images.html" class="Module">foundation.images</a>
<a id="16385" class="Keyword">open</a> <a id="16390" class="Keyword">import</a> <a id="16397" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="16432" class="Keyword">open</a> <a id="16437" class="Keyword">import</a> <a id="16444" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="16479" class="Keyword">open</a> <a id="16484" class="Keyword">import</a> <a id="16491" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="16518" class="Keyword">open</a> <a id="16523" class="Keyword">import</a> <a id="16530" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="16586" class="Keyword">open</a> <a id="16591" class="Keyword">import</a> <a id="16598" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="16627" class="Keyword">open</a> <a id="16632" class="Keyword">import</a> <a id="16639" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="16669" class="Keyword">open</a> <a id="16674" class="Keyword">import</a> <a id="16681" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="16708" class="Keyword">open</a> <a id="16713" class="Keyword">import</a> <a id="16720" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16746" class="Keyword">open</a> <a id="16751" class="Keyword">import</a> <a id="16758" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16785" class="Keyword">open</a> <a id="16790" class="Keyword">import</a> <a id="16797" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16821" class="Keyword">open</a> <a id="16826" class="Keyword">import</a> <a id="16833" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16856" class="Keyword">open</a> <a id="16861" class="Keyword">import</a> <a id="16868" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16895" class="Keyword">open</a> <a id="16900" class="Keyword">import</a> <a id="16907" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16939" class="Keyword">open</a> <a id="16944" class="Keyword">import</a> <a id="16951" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16986" class="Keyword">open</a> <a id="16991" class="Keyword">import</a> <a id="16998" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="17029" class="Keyword">open</a> <a id="17034" class="Keyword">import</a> <a id="17041" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="17074" class="Keyword">open</a> <a id="17079" class="Keyword">import</a> <a id="17086" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="17120" class="Keyword">open</a> <a id="17125" class="Keyword">import</a> <a id="17132" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="17172" class="Keyword">open</a> <a id="17177" class="Keyword">import</a> <a id="17184" href="foundation.lesser-limited-principle-of-omniscience.html" class="Module">foundation.lesser-limited-principle-of-omniscience</a>
<a id="17235" class="Keyword">open</a> <a id="17240" class="Keyword">import</a> <a id="17247" href="foundation.limited-principle-of-omniscience.html" class="Module">foundation.limited-principle-of-omniscience</a>
<a id="17291" class="Keyword">open</a> <a id="17296" class="Keyword">import</a> <a id="17303" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="17334" class="Keyword">open</a> <a id="17339" class="Keyword">import</a> <a id="17346" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="17378" class="Keyword">open</a> <a id="17383" class="Keyword">import</a> <a id="17390" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="17421" class="Keyword">open</a> <a id="17426" class="Keyword">import</a> <a id="17433" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="17450" class="Keyword">open</a> <a id="17455" class="Keyword">import</a> <a id="17462" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="17487" class="Keyword">open</a> <a id="17492" class="Keyword">import</a> <a id="17499" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="17528" class="Keyword">open</a> <a id="17533" class="Keyword">import</a> <a id="17540" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="17565" class="Keyword">open</a> <a id="17570" class="Keyword">import</a> <a id="17577" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="17606" class="Keyword">open</a> <a id="17611" class="Keyword">import</a> <a id="17618" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="17639" class="Keyword">open</a> <a id="17644" class="Keyword">import</a> <a id="17651" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="17675" class="Keyword">open</a> <a id="17680" class="Keyword">import</a> <a id="17687" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="17707" class="Keyword">open</a> <a id="17712" class="Keyword">import</a> <a id="17719" href="foundation.noncontractible-types.html" class="Module">foundation.noncontractible-types</a>
<a id="17752" class="Keyword">open</a> <a id="17757" class="Keyword">import</a> <a id="17764" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17802" class="Keyword">open</a> <a id="17807" class="Keyword">import</a> <a id="17814" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17842" class="Keyword">open</a> <a id="17847" class="Keyword">import</a> <a id="17854" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17878" class="Keyword">open</a> <a id="17883" class="Keyword">import</a> <a id="17890" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17917" class="Keyword">open</a> <a id="17922" class="Keyword">import</a> <a id="17929" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17964" class="Keyword">open</a> <a id="17969" class="Keyword">import</a> <a id="17976" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17997" class="Keyword">open</a> <a id="18002" class="Keyword">import</a> <a id="18009" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="18045" class="Keyword">open</a> <a id="18050" class="Keyword">import</a> <a id="18057" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="18102" class="Keyword">open</a> <a id="18107" class="Keyword">import</a> <a id="18114" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="18160" class="Keyword">open</a> <a id="18165" class="Keyword">import</a> <a id="18172" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="18212" class="Keyword">open</a> <a id="18217" class="Keyword">import</a> <a id="18224" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="18254" class="Keyword">open</a> <a id="18259" class="Keyword">import</a> <a id="18266" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="18300" class="Keyword">open</a> <a id="18305" class="Keyword">import</a> <a id="18312" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="18349" class="Keyword">open</a> <a id="18354" class="Keyword">import</a> <a id="18361" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="18385" class="Keyword">open</a> <a id="18390" class="Keyword">import</a> <a id="18397" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="18418" class="Keyword">open</a> <a id="18423" class="Keyword">import</a> <a id="18430" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="18465" class="Keyword">open</a> <a id="18470" class="Keyword">import</a> <a id="18477" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="18514" class="Keyword">open</a> <a id="18519" class="Keyword">import</a> <a id="18526" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="18575" class="Keyword">open</a> <a id="18580" class="Keyword">import</a> <a id="18587" href="foundation.reflexive-relations.html" class="Module">foundation.reflexive-relations</a>
<a id="18618" class="Keyword">open</a> <a id="18623" class="Keyword">import</a> <a id="18630" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="18663" class="Keyword">open</a> <a id="18668" class="Keyword">import</a> <a id="18675" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="18698" class="Keyword">open</a> <a id="18703" class="Keyword">import</a> <a id="18710" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="18733" class="Keyword">open</a> <a id="18738" class="Keyword">import</a> <a id="18745" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18768" class="Keyword">open</a> <a id="18773" class="Keyword">import</a> <a id="18780" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18808" class="Keyword">open</a> <a id="18813" class="Keyword">import</a> <a id="18820" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18840" class="Keyword">open</a> <a id="18845" class="Keyword">import</a> <a id="18852" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18873" class="Keyword">open</a> <a id="18878" class="Keyword">import</a> <a id="18885" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18916" class="Keyword">open</a> <a id="18921" class="Keyword">import</a> <a id="18928" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18955" class="Keyword">open</a> <a id="18960" class="Keyword">import</a> <a id="18967" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18983" class="Keyword">open</a> <a id="18988" class="Keyword">import</a> <a id="18995" href="foundation.sigma-decompositions.html" class="Module">foundation.sigma-decompositions</a>
<a id="19027" class="Keyword">open</a> <a id="19032" class="Keyword">import</a> <a id="19039" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="19070" class="Keyword">open</a> <a id="19075" class="Keyword">import</a> <a id="19082" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="19099" class="Keyword">open</a> <a id="19104" class="Keyword">import</a> <a id="19111" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="19133" class="Keyword">open</a> <a id="19138" class="Keyword">import</a> <a id="19145" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="19172" class="Keyword">open</a> <a id="19177" class="Keyword">import</a> <a id="19184" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="19207" class="Keyword">open</a> <a id="19212" class="Keyword">import</a> <a id="19219" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="19246" class="Keyword">open</a> <a id="19251" class="Keyword">import</a> <a id="19258" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="19291" class="Keyword">open</a> <a id="19296" class="Keyword">import</a> <a id="19303" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="19343" class="Keyword">open</a> <a id="19348" class="Keyword">import</a> <a id="19355" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="19376" class="Keyword">open</a> <a id="19381" class="Keyword">import</a> <a id="19388" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="19417" class="Keyword">open</a> <a id="19422" class="Keyword">import</a> <a id="19429" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="19467" class="Keyword">open</a> <a id="19472" class="Keyword">import</a> <a id="19479" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="19499" class="Keyword">open</a> <a id="19504" class="Keyword">import</a> <a id="19511" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="19535" class="Keyword">open</a> <a id="19540" class="Keyword">import</a> <a id="19547" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="19574" class="Keyword">open</a> <a id="19579" class="Keyword">import</a> <a id="19586" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="19618" class="Keyword">open</a> <a id="19623" class="Keyword">import</a> <a id="19630" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="19660" class="Keyword">open</a> <a id="19665" class="Keyword">import</a> <a id="19672" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19698" class="Keyword">open</a> <a id="19703" class="Keyword">import</a> <a id="19710" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19737" class="Keyword">open</a> <a id="19742" class="Keyword">import</a> <a id="19749" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19786" class="Keyword">open</a> <a id="19791" class="Keyword">import</a> <a id="19798" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19827" class="Keyword">open</a> <a id="19832" class="Keyword">import</a> <a id="19839" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19862" class="Keyword">open</a> <a id="19867" class="Keyword">import</a> <a id="19874" href="foundation.type-arithmetic-booleans.html" class="Module">foundation.type-arithmetic-booleans</a>
<a id="19910" class="Keyword">open</a> <a id="19915" class="Keyword">import</a> <a id="19922" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19973" class="Keyword">open</a> <a id="19978" class="Keyword">import</a> <a id="19985" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="20028" class="Keyword">open</a> <a id="20033" class="Keyword">import</a> <a id="20040" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="20092" class="Keyword">open</a> <a id="20097" class="Keyword">import</a> <a id="20104" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="20152" class="Keyword">open</a> <a id="20157" class="Keyword">import</a> <a id="20164" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="20202" class="Keyword">open</a> <a id="20207" class="Keyword">import</a> <a id="20214" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="20251" class="Keyword">open</a> <a id="20256" class="Keyword">import</a> <a id="20263" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="20309" class="Keyword">open</a> <a id="20314" class="Keyword">import</a> <a id="20321" href="foundation.union.html" class="Module">foundation.union</a>
<a id="20338" class="Keyword">open</a> <a id="20343" class="Keyword">import</a> <a id="20350" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="20378" class="Keyword">open</a> <a id="20383" class="Keyword">import</a> <a id="20390" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="20418" class="Keyword">open</a> <a id="20423" class="Keyword">import</a> <a id="20430" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="20466" class="Keyword">open</a> <a id="20471" class="Keyword">import</a> <a id="20478" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="20516" class="Keyword">open</a> <a id="20521" class="Keyword">import</a> <a id="20528" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="20561" class="Keyword">open</a> <a id="20566" class="Keyword">import</a> <a id="20573" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="20594" class="Keyword">open</a> <a id="20599" class="Keyword">import</a> <a id="20606" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="20642" class="Keyword">open</a> <a id="20647" class="Keyword">import</a> <a id="20654" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="20708" class="Keyword">open</a> <a id="20713" class="Keyword">import</a> <a id="20720" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20742" class="Keyword">open</a> <a id="20747" class="Keyword">import</a> <a id="20754" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20789" class="Keyword">open</a> <a id="20794" class="Keyword">import</a> <a id="20801" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20831" class="Keyword">open</a> <a id="20836" class="Keyword">import</a> <a id="20843" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20882" class="Keyword">open</a> <a id="20887" class="Keyword">import</a> <a id="20894" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20948" class="Keyword">open</a> <a id="20953" class="Keyword">import</a> <a id="20960" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="21006" class="Keyword">open</a> <a id="21011" class="Keyword">import</a> <a id="21018" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="21069" class="Keyword">open</a> <a id="21074" class="Keyword">import</a> <a id="21081" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="21122" class="Keyword">open</a> <a id="21127" class="Keyword">import</a> <a id="21134" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="21179" class="Keyword">open</a> <a id="21184" class="Keyword">import</a> <a id="21191" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="21236" class="Keyword">open</a> <a id="21241" class="Keyword">import</a> <a id="21248" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="21284" class="Keyword">open</a> <a id="21289" class="Keyword">import</a> <a id="21296" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="21332" class="Keyword">open</a> <a id="21337" class="Keyword">import</a> <a id="21344" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="21409" class="Keyword">open</a> <a id="21414" class="Keyword">import</a> <a id="21421" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="21476" class="Keyword">open</a> <a id="21481" class="Keyword">import</a> <a id="21488" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="21528" class="Keyword">open</a> <a id="21533" class="Keyword">import</a> <a id="21540" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="21584" class="Keyword">open</a> <a id="21589" class="Keyword">import</a> <a id="21596" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="21641" class="Keyword">open</a> <a id="21646" class="Keyword">import</a> <a id="21653" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="21694" class="Keyword">open</a> <a id="21699" class="Keyword">import</a> <a id="21706" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21746" class="Keyword">open</a> <a id="21751" class="Keyword">import</a> <a id="21758" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21785" class="Keyword">open</a> <a id="21790" class="Keyword">import</a> <a id="21797" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21833" class="Keyword">open</a> <a id="21838" class="Keyword">import</a> <a id="21845" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21872" class="Keyword">open</a> <a id="21877" class="Keyword">import</a> <a id="21884" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21921" class="Keyword">open</a> <a id="21926" class="Keyword">import</a> <a id="21933" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21961" class="Keyword">open</a> <a id="21966" class="Keyword">import</a> <a id="21973" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21992" class="Keyword">open</a> <a id="21997" class="Keyword">import</a> <a id="22004" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="22044" class="Keyword">open</a> <a id="22049" class="Keyword">import</a> <a id="22056" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="22105" class="Keyword">open</a> <a id="22110" class="Keyword">import</a> <a id="22117" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="22149" class="Keyword">open</a> <a id="22154" class="Keyword">import</a> <a id="22161" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="22209" class="Keyword">open</a> <a id="22214" class="Keyword">import</a> <a id="22221" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="22244" class="Keyword">open</a> <a id="22249" class="Keyword">import</a> <a id="22256" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="22280" class="Keyword">open</a> <a id="22285" class="Keyword">import</a> <a id="22292" href="foundation-core.automorphisms.html" class="Module">foundation-core.automorphisms</a>
<a id="22322" class="Keyword">open</a> <a id="22327" class="Keyword">import</a> <a id="22334" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="22374" class="Keyword">open</a> <a id="22379" class="Keyword">import</a> <a id="22386" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22429" class="Keyword">open</a> <a id="22434" class="Keyword">import</a> <a id="22441" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22475" class="Keyword">open</a> <a id="22480" class="Keyword">import</a> <a id="22487" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22519" class="Keyword">open</a> <a id="22524" class="Keyword">import</a> <a id="22531" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22561" class="Keyword">open</a> <a id="22566" class="Keyword">import</a> <a id="22573" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22607" class="Keyword">open</a> <a id="22612" class="Keyword">import</a> <a id="22619" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22654" class="Keyword">open</a> <a id="22659" class="Keyword">import</a> <a id="22666" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22690" class="Keyword">open</a> <a id="22695" class="Keyword">import</a> <a id="22702" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22739" class="Keyword">open</a> <a id="22744" class="Keyword">import</a> <a id="22751" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22778" class="Keyword">open</a> <a id="22783" class="Keyword">import</a> <a id="22790" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22818" class="Keyword">open</a> <a id="22823" class="Keyword">import</a> <a id="22830" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22860" class="Keyword">open</a> <a id="22865" class="Keyword">import</a> <a id="22872" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22921" class="Keyword">open</a> <a id="22926" class="Keyword">import</a> <a id="22933" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22979" class="Keyword">open</a> <a id="22984" class="Keyword">import</a> <a id="22991" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="23031" class="Keyword">open</a> <a id="23036" class="Keyword">import</a> <a id="23043" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="23081" class="Keyword">open</a> <a id="23086" class="Keyword">import</a> <a id="23093" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="23122" class="Keyword">open</a> <a id="23127" class="Keyword">import</a> <a id="23134" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="23164" class="Keyword">open</a> <a id="23169" class="Keyword">import</a> <a id="23176" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="23207" class="Keyword">open</a> <a id="23212" class="Keyword">import</a> <a id="23219" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="23259" class="Keyword">open</a> <a id="23264" class="Keyword">import</a> <a id="23271" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="23297" class="Keyword">open</a> <a id="23302" class="Keyword">import</a> <a id="23309" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="23364" class="Keyword">open</a> <a id="23369" class="Keyword">import</a> <a id="23376" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23427" class="Keyword">open</a> <a id="23432" class="Keyword">import</a> <a id="23439" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23484" class="Keyword">open</a> <a id="23489" class="Keyword">import</a> <a id="23496" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23541" class="Keyword">open</a> <a id="23546" class="Keyword">import</a> <a id="23553" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23607" class="Keyword">open</a> <a id="23612" class="Keyword">import</a> <a id="23619" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23646" class="Keyword">open</a> <a id="23651" class="Keyword">import</a> <a id="23658" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23691" class="Keyword">open</a> <a id="23696" class="Keyword">import</a> <a id="23703" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23734" class="Keyword">open</a> <a id="23739" class="Keyword">import</a> <a id="23746" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23783" class="Keyword">open</a> <a id="23788" class="Keyword">import</a> <a id="23795" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23829" class="Keyword">open</a> <a id="23834" class="Keyword">import</a> <a id="23841" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23866" class="Keyword">open</a> <a id="23871" class="Keyword">import</a> <a id="23878" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23910" class="Keyword">open</a> <a id="23915" class="Keyword">import</a> <a id="23922" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23957" class="Keyword">open</a> <a id="23962" class="Keyword">import</a> <a id="23969" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23998" class="Keyword">open</a> <a id="24003" class="Keyword">import</a> <a id="24010" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="24036" class="Keyword">open</a> <a id="24041" class="Keyword">import</a> <a id="24048" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="24076" class="Keyword">open</a> <a id="24081" class="Keyword">import</a> <a id="24088" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="24113" class="Keyword">open</a> <a id="24118" class="Keyword">import</a> <a id="24125" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="24146" class="Keyword">open</a> <a id="24151" class="Keyword">import</a> <a id="24158" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="24194" class="Keyword">open</a> <a id="24199" class="Keyword">import</a> <a id="24206" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="24249" class="Keyword">open</a> <a id="24254" class="Keyword">import</a> <a id="24261" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="24286" class="Keyword">open</a> <a id="24291" class="Keyword">import</a> <a id="24298" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="24329" class="Keyword">open</a> <a id="24334" class="Keyword">import</a> <a id="24341" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="24373" class="Keyword">open</a> <a id="24378" class="Keyword">import</a> <a id="24385" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24419" class="Keyword">open</a> <a id="24424" class="Keyword">import</a> <a id="24431" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24487" class="Keyword">open</a> <a id="24492" class="Keyword">import</a> <a id="24499" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24552" class="Keyword">open</a> <a id="24557" class="Keyword">import</a> <a id="24564" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24591" class="Keyword">open</a> <a id="24596" class="Keyword">import</a> <a id="24603" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24648" class="Keyword">open</a> <a id="24653" class="Keyword">import</a> <a id="24660" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24722" class="Keyword">open</a> <a id="24727" class="Keyword">import</a> <a id="24734" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24747" class="Keyword">open</a> <a id="24752" class="Keyword">import</a> <a id="24759" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24799" class="Keyword">open</a> <a id="24804" class="Keyword">import</a> <a id="24811" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24855" class="Keyword">open</a> <a id="24860" class="Keyword">import</a> <a id="24867" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24906" class="Keyword">open</a> <a id="24911" class="Keyword">import</a> <a id="24918" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24960" class="Keyword">open</a> <a id="24965" class="Keyword">import</a> <a id="24972" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="25012" class="Keyword">open</a> <a id="25017" class="Keyword">import</a> <a id="25024" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="25065" class="Keyword">open</a> <a id="25070" class="Keyword">import</a> <a id="25077" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="25115" class="Keyword">open</a> <a id="25120" class="Keyword">import</a> <a id="25127" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="25190" class="Keyword">open</a> <a id="25195" class="Keyword">import</a> <a id="25202" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="25231" class="Keyword">open</a> <a id="25236" class="Keyword">import</a> <a id="25243" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="25288" class="Keyword">open</a> <a id="25293" class="Keyword">import</a> <a id="25300" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="25342" class="Keyword">open</a> <a id="25347" class="Keyword">import</a> <a id="25354" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25394" class="Keyword">open</a> <a id="25399" class="Keyword">import</a> <a id="25406" href="graph-theory.equivalences-enriched-undirected-graphs.html" class="Module">graph-theory.equivalences-enriched-undirected-graphs</a>
<a id="25459" class="Keyword">open</a> <a id="25464" class="Keyword">import</a> <a id="25471" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25515" class="Keyword">open</a> <a id="25520" class="Keyword">import</a> <a id="25527" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25576" class="Keyword">open</a> <a id="25581" class="Keyword">import</a> <a id="25588" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25638" class="Keyword">open</a> <a id="25643" class="Keyword">import</a> <a id="25650" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25677" class="Keyword">open</a> <a id="25682" class="Keyword">import</a> <a id="25689" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25714" class="Keyword">open</a> <a id="25719" class="Keyword">import</a> <a id="25726" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25749" class="Keyword">open</a> <a id="25754" class="Keyword">import</a> <a id="25761" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25810" class="Keyword">open</a> <a id="25815" class="Keyword">import</a> <a id="25822" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25861" class="Keyword">open</a> <a id="25866" class="Keyword">import</a> <a id="25873" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25914" class="Keyword">open</a> <a id="25919" class="Keyword">import</a> <a id="25926" href="graph-theory.neighbors-undirected-graphs.html" class="Module">graph-theory.neighbors-undirected-graphs</a>
<a id="25967" class="Keyword">open</a> <a id="25972" class="Keyword">import</a> <a id="25979" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="26023" class="Keyword">open</a> <a id="26028" class="Keyword">import</a> <a id="26035" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="26072" class="Keyword">open</a> <a id="26077" class="Keyword">import</a> <a id="26084" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="26106" class="Keyword">open</a> <a id="26111" class="Keyword">import</a> <a id="26118" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="26148" class="Keyword">open</a> <a id="26153" class="Keyword">import</a> <a id="26160" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="26199" class="Keyword">open</a> <a id="26204" class="Keyword">import</a> <a id="26211" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="26242" class="Keyword">open</a> <a id="26247" class="Keyword">import</a> <a id="26254" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="26280" class="Keyword">open</a> <a id="26285" class="Keyword">import</a> <a id="26292" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="26330" class="Keyword">open</a> <a id="26335" class="Keyword">import</a> <a id="26342" href="graph-theory.stereoisomerism-enriched-undirected-graphs.html" class="Module">graph-theory.stereoisomerism-enriched-undirected-graphs</a>
<a id="26398" class="Keyword">open</a> <a id="26403" class="Keyword">import</a> <a id="26410" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="26468" class="Keyword">open</a> <a id="26473" class="Keyword">import</a> <a id="26480" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="26518" class="Keyword">open</a> <a id="26523" class="Keyword">import</a> <a id="26530" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26549" class="Keyword">open</a> <a id="26554" class="Keyword">import</a> <a id="26561" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26626" class="Keyword">open</a> <a id="26631" class="Keyword">import</a> <a id="26638" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26669" class="Keyword">open</a> <a id="26674" class="Keyword">import</a> <a id="26681" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26708" class="Keyword">open</a> <a id="26713" class="Keyword">import</a> <a id="26720" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26748" class="Keyword">open</a> <a id="26753" class="Keyword">import</a> <a id="26760" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26827" class="Keyword">open</a> <a id="26832" class="Keyword">import</a> <a id="26839" href="group-theory.html" class="Module">group-theory</a>
<a id="26852" class="Keyword">open</a> <a id="26857" class="Keyword">import</a> <a id="26864" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26892" class="Keyword">open</a> <a id="26897" class="Keyword">import</a> <a id="26904" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26955" class="Keyword">open</a> <a id="26960" class="Keyword">import</a> <a id="26967" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="27000" class="Keyword">open</a> <a id="27005" class="Keyword">import</a> <a id="27012" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="27059" class="Keyword">open</a> <a id="27064" class="Keyword">import</a> <a id="27071" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="27110" class="Keyword">open</a> <a id="27115" class="Keyword">import</a> <a id="27122" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="27162" class="Keyword">open</a> <a id="27167" class="Keyword">import</a> <a id="27174" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="27217" class="Keyword">open</a> <a id="27222" class="Keyword">import</a> <a id="27229" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="27261" class="Keyword">open</a> <a id="27266" class="Keyword">import</a> <a id="27273" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="27309" class="Keyword">open</a> <a id="27314" class="Keyword">import</a> <a id="27321" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="27350" class="Keyword">open</a> <a id="27355" class="Keyword">import</a> <a id="27362" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="27390" class="Keyword">open</a> <a id="27395" class="Keyword">import</a> <a id="27402" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="27435" class="Keyword">open</a> <a id="27440" class="Keyword">import</a> <a id="27447" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="27483" class="Keyword">open</a> <a id="27488" class="Keyword">import</a> <a id="27495" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27524" class="Keyword">open</a> <a id="27529" class="Keyword">import</a> <a id="27536" href="group-theory.congruence-relations-groups.html" class="Module">group-theory.congruence-relations-groups</a>
<a id="27577" class="Keyword">open</a> <a id="27582" class="Keyword">import</a> <a id="27589" href="group-theory.congruence-relations-monoids.html" class="Module">group-theory.congruence-relations-monoids</a>
<a id="27631" class="Keyword">open</a> <a id="27636" class="Keyword">import</a> <a id="27643" href="group-theory.congruence-relations-semigroups.html" class="Module">group-theory.congruence-relations-semigroups</a>
<a id="27688" class="Keyword">open</a> <a id="27693" class="Keyword">import</a> <a id="27700" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27725" class="Keyword">open</a> <a id="27730" class="Keyword">import</a> <a id="27737" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27799" class="Keyword">open</a> <a id="27804" class="Keyword">import</a> <a id="27811" href="group-theory.decidable-subgroups.html" class="Module">group-theory.decidable-subgroups</a>
<a id="27844" class="Keyword">open</a> <a id="27849" class="Keyword">import</a> <a id="27856" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27897" class="Keyword">open</a> <a id="27902" class="Keyword">import</a> <a id="27909" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27938" class="Keyword">open</a> <a id="27943" class="Keyword">import</a> <a id="27950" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27974" class="Keyword">open</a> <a id="27979" class="Keyword">import</a> <a id="27986" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="28017" class="Keyword">open</a> <a id="28022" class="Keyword">import</a> <a id="28029" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="28076" class="Keyword">open</a> <a id="28081" class="Keyword">import</a> <a id="28088" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="28121" class="Keyword">open</a> <a id="28126" class="Keyword">import</a> <a id="28133" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="28182" class="Keyword">open</a> <a id="28187" class="Keyword">import</a> <a id="28194" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="28234" class="Keyword">open</a> <a id="28239" class="Keyword">import</a> <a id="28246" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="28286" class="Keyword">open</a> <a id="28291" class="Keyword">import</a> <a id="28298" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="28335" class="Keyword">open</a> <a id="28340" class="Keyword">import</a> <a id="28347" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="28394" class="Keyword">open</a> <a id="28399" class="Keyword">import</a> <a id="28406" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="28447" class="Keyword">open</a> <a id="28452" class="Keyword">import</a> <a id="28459" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="28503" class="Keyword">open</a> <a id="28508" class="Keyword">import</a> <a id="28515" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="28554" class="Keyword">open</a> <a id="28559" class="Keyword">import</a> <a id="28566" href="group-theory.full-subgroups.html" class="Module">group-theory.full-subgroups</a>
<a id="28594" class="Keyword">open</a> <a id="28599" class="Keyword">import</a> <a id="28606" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28638" class="Keyword">open</a> <a id="28643" class="Keyword">import</a> <a id="28650" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28677" class="Keyword">open</a> <a id="28682" class="Keyword">import</a> <a id="28689" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28709" class="Keyword">open</a> <a id="28714" class="Keyword">import</a> <a id="28721" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28755" class="Keyword">open</a> <a id="28760" class="Keyword">import</a> <a id="28767" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28794" class="Keyword">open</a> <a id="28799" class="Keyword">import</a> <a id="28806" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28848" class="Keyword">open</a> <a id="28853" class="Keyword">import</a> <a id="28860" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28910" class="Keyword">open</a> <a id="28915" class="Keyword">import</a> <a id="28922" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28969" class="Keyword">open</a> <a id="28974" class="Keyword">import</a> <a id="28981" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="29022" class="Keyword">open</a> <a id="29027" class="Keyword">import</a> <a id="29034" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="29068" class="Keyword">open</a> <a id="29073" class="Keyword">import</a> <a id="29080" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="29128" class="Keyword">open</a> <a id="29133" class="Keyword">import</a> <a id="29140" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="29181" class="Keyword">open</a> <a id="29186" class="Keyword">import</a> <a id="29193" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="29228" class="Keyword">open</a> <a id="29233" class="Keyword">import</a> <a id="29240" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="29278" class="Keyword">open</a> <a id="29283" class="Keyword">import</a> <a id="29290" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="29325" class="Keyword">open</a> <a id="29330" class="Keyword">import</a> <a id="29337" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="29369" class="Keyword">open</a> <a id="29374" class="Keyword">import</a> <a id="29381" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="29422" class="Keyword">open</a> <a id="29427" class="Keyword">import</a> <a id="29434" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="29475" class="Keyword">open</a> <a id="29480" class="Keyword">import</a> <a id="29487" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="29527" class="Keyword">open</a> <a id="29532" class="Keyword">import</a> <a id="29539" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="29572" class="Keyword">open</a> <a id="29577" class="Keyword">import</a> <a id="29584" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29621" class="Keyword">open</a> <a id="29626" class="Keyword">import</a> <a id="29633" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29663" class="Keyword">open</a> <a id="29668" class="Keyword">import</a> <a id="29675" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29696" class="Keyword">open</a> <a id="29701" class="Keyword">import</a> <a id="29708" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29762" class="Keyword">open</a> <a id="29767" class="Keyword">import</a> <a id="29774" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29819" class="Keyword">open</a> <a id="29824" class="Keyword">import</a> <a id="29831" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29859" class="Keyword">open</a> <a id="29864" class="Keyword">import</a> <a id="29871" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29892" class="Keyword">open</a> <a id="29897" class="Keyword">import</a> <a id="29904" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29947" class="Keyword">open</a> <a id="29952" class="Keyword">import</a> <a id="29959" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29993" class="Keyword">open</a> <a id="29998" class="Keyword">import</a> <a id="30005" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="30035" class="Keyword">open</a> <a id="30040" class="Keyword">import</a> <a id="30047" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="30093" class="Keyword">open</a> <a id="30098" class="Keyword">import</a> <a id="30105" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="30159" class="Keyword">open</a> <a id="30164" class="Keyword">import</a> <a id="30171" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="30214" class="Keyword">open</a> <a id="30219" class="Keyword">import</a> <a id="30226" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="30260" class="Keyword">open</a> <a id="30265" class="Keyword">import</a> <a id="30272" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="30313" class="Keyword">open</a> <a id="30318" class="Keyword">import</a> <a id="30325" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="30360" class="Keyword">open</a> <a id="30365" class="Keyword">import</a> <a id="30372" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a>
<a id="30411" class="Keyword">open</a> <a id="30416" class="Keyword">import</a> <a id="30423" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="30465" class="Keyword">open</a> <a id="30470" class="Keyword">import</a> <a id="30477" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="30512" class="Keyword">open</a> <a id="30517" class="Keyword">import</a> <a id="30524" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="30563" class="Keyword">open</a> <a id="30568" class="Keyword">import</a> <a id="30575" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="30612" class="Keyword">open</a> <a id="30617" class="Keyword">import</a> <a id="30624" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30671" class="Keyword">open</a> <a id="30676" class="Keyword">import</a> <a id="30683" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30747" class="Keyword">open</a> <a id="30752" class="Keyword">import</a> <a id="30759" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30804" class="Keyword">open</a> <a id="30809" class="Keyword">import</a> <a id="30816" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30840" class="Keyword">open</a> <a id="30845" class="Keyword">import</a> <a id="30852" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30877" class="Keyword">open</a> <a id="30882" class="Keyword">import</a> <a id="30889" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30932" class="Keyword">open</a> <a id="30937" class="Keyword">import</a> <a id="30944" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30975" class="Keyword">open</a> <a id="30980" class="Keyword">import</a> <a id="30987" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="31041" class="Keyword">open</a> <a id="31046" class="Keyword">import</a> <a id="31053" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="31076" class="Keyword">open</a> <a id="31081" class="Keyword">import</a> <a id="31088" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="31126" class="Keyword">open</a> <a id="31131" class="Keyword">import</a> <a id="31138" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="31177" class="Keyword">open</a> <a id="31182" class="Keyword">import</a> <a id="31189" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="31240" class="Keyword">open</a> <a id="31245" class="Keyword">import</a> <a id="31252" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="31289" class="Keyword">open</a> <a id="31294" class="Keyword">import</a> <a id="31301" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="31325" class="Keyword">open</a> <a id="31330" class="Keyword">import</a> <a id="31337" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="31364" class="Keyword">open</a> <a id="31369" class="Keyword">import</a> <a id="31376" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="31433" class="Keyword">open</a> <a id="31438" class="Keyword">import</a> <a id="31445" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="31493" class="Keyword">open</a> <a id="31498" class="Keyword">import</a> <a id="31505" href="group-theory.symmetric-concrete-groups.html" class="Module">group-theory.symmetric-concrete-groups</a>
<a id="31544" class="Keyword">open</a> <a id="31549" class="Keyword">import</a> <a id="31556" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="31586" class="Keyword">open</a> <a id="31591" class="Keyword">import</a> <a id="31598" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="31635" class="Keyword">open</a> <a id="31640" class="Keyword">import</a> <a id="31647" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="31668" class="Keyword">open</a> <a id="31673" class="Keyword">import</a> <a id="31680" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31727" class="Keyword">open</a> <a id="31732" class="Keyword">import</a> <a id="31739" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31777" class="Keyword">open</a> <a id="31782" class="Keyword">import</a> <a id="31789" href="group-theory.trivial-subgroups.html" class="Module">group-theory.trivial-subgroups</a>
<a id="31820" class="Keyword">open</a> <a id="31825" class="Keyword">import</a> <a id="31832" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31926" class="Keyword">open</a> <a id="31931" class="Keyword">import</a> <a id="31938" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31953" class="Keyword">open</a> <a id="31958" class="Keyword">import</a> <a id="31965" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31998" class="Keyword">open</a> <a id="32003" class="Keyword">import</a> <a id="32010" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="32042" class="Keyword">open</a> <a id="32047" class="Keyword">import</a> <a id="32054" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="32096" class="Keyword">open</a> <a id="32101" class="Keyword">import</a> <a id="32108" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="32146" class="Keyword">open</a> <a id="32151" class="Keyword">import</a> <a id="32158" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="32195" class="Keyword">open</a> <a id="32200" class="Keyword">import</a> <a id="32207" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="32240" class="Keyword">open</a> <a id="32245" class="Keyword">import</a> <a id="32252" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="32276" class="Keyword">open</a> <a id="32281" class="Keyword">import</a> <a id="32288" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="32327" class="Keyword">open</a> <a id="32332" class="Keyword">import</a> <a id="32339" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="32385" class="Keyword">open</a> <a id="32390" class="Keyword">import</a> <a id="32397" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="32442" class="Keyword">open</a> <a id="32447" class="Keyword">import</a> <a id="32454" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="32492" class="Keyword">open</a> <a id="32497" class="Keyword">import</a> <a id="32504" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="32536" class="Keyword">open</a> <a id="32541" class="Keyword">import</a> <a id="32548" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="32601" class="Keyword">open</a> <a id="32606" class="Keyword">import</a> <a id="32613" href="order-theory.html" class="Module">order-theory</a>
<a id="32626" class="Keyword">open</a> <a id="32631" class="Keyword">import</a> <a id="32638" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="32665" class="Keyword">open</a> <a id="32670" class="Keyword">import</a> <a id="32677" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="32707" class="Keyword">open</a> <a id="32712" class="Keyword">import</a> <a id="32719" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32752" class="Keyword">open</a> <a id="32757" class="Keyword">import</a> <a id="32764" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32800" class="Keyword">open</a> <a id="32805" class="Keyword">import</a> <a id="32812" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32847" class="Keyword">open</a> <a id="32852" class="Keyword">import</a> <a id="32859" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32886" class="Keyword">open</a> <a id="32891" class="Keyword">import</a> <a id="32898" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32928" class="Keyword">open</a> <a id="32933" class="Keyword">import</a> <a id="32940" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32976" class="Keyword">open</a> <a id="32981" class="Keyword">import</a> <a id="32988" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="33030" class="Keyword">open</a> <a id="33035" class="Keyword">import</a> <a id="33042" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="33072" class="Keyword">open</a> <a id="33077" class="Keyword">import</a> <a id="33084" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="33116" class="Keyword">open</a> <a id="33121" class="Keyword">import</a> <a id="33128" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="33159" class="Keyword">open</a> <a id="33164" class="Keyword">import</a> <a id="33171" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="33197" class="Keyword">open</a> <a id="33202" class="Keyword">import</a> <a id="33209" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="33238" class="Keyword">open</a> <a id="33243" class="Keyword">import</a> <a id="33250" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="33287" class="Keyword">open</a> <a id="33292" class="Keyword">import</a> <a id="33299" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="33339" class="Keyword">open</a> <a id="33344" class="Keyword">import</a> <a id="33351" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="33373" class="Keyword">open</a> <a id="33378" class="Keyword">import</a> <a id="33385" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="33420" class="Keyword">open</a> <a id="33425" class="Keyword">import</a> <a id="33432" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="33470" class="Keyword">open</a> <a id="33475" class="Keyword">import</a> <a id="33482" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="33521" class="Keyword">open</a> <a id="33526" class="Keyword">import</a> <a id="33533" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="33568" class="Keyword">open</a> <a id="33573" class="Keyword">import</a> <a id="33580" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="33615" class="Keyword">open</a> <a id="33620" class="Keyword">import</a> <a id="33627" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="33662" class="Keyword">open</a> <a id="33667" class="Keyword">import</a> <a id="33674" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="33712" class="Keyword">open</a> <a id="33717" class="Keyword">import</a> <a id="33724" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33755" class="Keyword">open</a> <a id="33760" class="Keyword">import</a> <a id="33767" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33809" class="Keyword">open</a> <a id="33814" class="Keyword">import</a> <a id="33821" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33866" class="Keyword">open</a> <a id="33871" class="Keyword">import</a> <a id="33878" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33911" class="Keyword">open</a> <a id="33916" class="Keyword">import</a> <a id="33923" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33943" class="Keyword">open</a> <a id="33948" class="Keyword">import</a> <a id="33955" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33978" class="Keyword">open</a> <a id="33983" class="Keyword">import</a> <a id="33990" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="34013" class="Keyword">open</a> <a id="34018" class="Keyword">import</a> <a id="34025" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="34051" class="Keyword">open</a> <a id="34056" class="Keyword">import</a> <a id="34063" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="34089" class="Keyword">open</a> <a id="34094" class="Keyword">import</a> <a id="34101" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="34165" class="Keyword">open</a> <a id="34170" class="Keyword">import</a> <a id="34177" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="34195" class="Keyword">open</a> <a id="34200" class="Keyword">import</a> <a id="34207" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="34234" class="Keyword">open</a> <a id="34239" class="Keyword">import</a> <a id="34246" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="34272" class="Keyword">open</a> <a id="34277" class="Keyword">import</a> <a id="34284" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="34310" class="Keyword">open</a> <a id="34315" class="Keyword">import</a> <a id="34322" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="34348" class="Keyword">open</a> <a id="34353" class="Keyword">import</a> <a id="34360" href="organic-chemistry.ethane.html" class="Module">organic-chemistry.ethane</a>
<a id="34385" class="Keyword">open</a> <a id="34390" class="Keyword">import</a> <a id="34397" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="34428" class="Keyword">open</a> <a id="34433" class="Keyword">import</a> <a id="34440" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="34466" class="Keyword">open</a> <a id="34471" class="Keyword">import</a> <a id="34478" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="34541" class="Keyword">open</a> <a id="34546" class="Keyword">import</a> <a id="34553" href="polytopes.html" class="Module">polytopes</a>
<a id="34563" class="Keyword">open</a> <a id="34568" class="Keyword">import</a> <a id="34575" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="34633" class="Keyword">open</a> <a id="34638" class="Keyword">import</a> <a id="34645" href="ring-theory.html" class="Module">ring-theory</a>
<a id="34657" class="Keyword">open</a> <a id="34662" class="Keyword">import</a> <a id="34669" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="34706" class="Keyword">open</a> <a id="34711" class="Keyword">import</a> <a id="34718" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="34745" class="Keyword">open</a> <a id="34750" class="Keyword">import</a> <a id="34757" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34789" class="Keyword">open</a> <a id="34794" class="Keyword">import</a> <a id="34801" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34847" class="Keyword">open</a> <a id="34852" class="Keyword">import</a> <a id="34859" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34884" class="Keyword">open</a> <a id="34889" class="Keyword">import</a> <a id="34896" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34934" class="Keyword">open</a> <a id="34939" class="Keyword">import</a> <a id="34946" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34989" class="Keyword">open</a> <a id="34994" class="Keyword">import</a> <a id="35001" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="35039" class="Keyword">open</a> <a id="35044" class="Keyword">import</a> <a id="35051" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="35082" class="Keyword">open</a> <a id="35087" class="Keyword">import</a> <a id="35094" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="35118" class="Keyword">open</a> <a id="35123" class="Keyword">import</a> <a id="35130" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="35162" class="Keyword">open</a> <a id="35167" class="Keyword">import</a> <a id="35174" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="35200" class="Keyword">open</a> <a id="35205" class="Keyword">import</a> <a id="35212" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="35241" class="Keyword">open</a> <a id="35246" class="Keyword">import</a> <a id="35253" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="35290" class="Keyword">open</a> <a id="35295" class="Keyword">import</a> <a id="35302" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="35331" class="Keyword">open</a> <a id="35336" class="Keyword">import</a> <a id="35343" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="35370" class="Keyword">open</a> <a id="35375" class="Keyword">import</a> <a id="35382" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="35419" class="Keyword">open</a> <a id="35424" class="Keyword">import</a> <a id="35431" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="35458" class="Keyword">open</a> <a id="35463" class="Keyword">import</a> <a id="35470" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="35503" class="Keyword">open</a> <a id="35508" class="Keyword">import</a> <a id="35515" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="35533" class="Keyword">open</a> <a id="35538" class="Keyword">import</a> <a id="35545" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="35599" class="Keyword">open</a> <a id="35604" class="Keyword">import</a> <a id="35611" href="set-theory.html" class="Module">set-theory</a>
<a id="35622" class="Keyword">open</a> <a id="35627" class="Keyword">import</a> <a id="35634" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="35657" class="Keyword">open</a> <a id="35662" class="Keyword">import</a> <a id="35669" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="35693" class="Keyword">open</a> <a id="35698" class="Keyword">import</a> <a id="35705" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="35730" class="Keyword">open</a> <a id="35735" class="Keyword">import</a> <a id="35742" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="35768" class="Keyword">open</a> <a id="35773" class="Keyword">import</a> <a id="35780" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35842" class="Keyword">open</a> <a id="35847" class="Keyword">import</a> <a id="35854" href="structured-types.html" class="Module">structured-types</a>
<a id="35871" class="Keyword">open</a> <a id="35876" class="Keyword">import</a> <a id="35883" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35918" class="Keyword">open</a> <a id="35923" class="Keyword">import</a> <a id="35930" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35974" class="Keyword">open</a> <a id="35979" class="Keyword">import</a> <a id="35986" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="36050" class="Keyword">open</a> <a id="36055" class="Keyword">import</a> <a id="36062" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="36101" class="Keyword">open</a> <a id="36106" class="Keyword">import</a> <a id="36113" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="36159" class="Keyword">open</a> <a id="36164" class="Keyword">import</a> <a id="36171" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="36236" class="Keyword">open</a> <a id="36241" class="Keyword">import</a> <a id="36248" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="36272" class="Keyword">open</a> <a id="36277" class="Keyword">import</a> <a id="36284" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="36353" class="Keyword">open</a> <a id="36358" class="Keyword">import</a> <a id="36365" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="36410" class="Keyword">open</a> <a id="36415" class="Keyword">import</a> <a id="36422" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="36456" class="Keyword">open</a> <a id="36461" class="Keyword">import</a> <a id="36468" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="36529" class="Keyword">open</a> <a id="36534" class="Keyword">import</a> <a id="36541" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="36586" class="Keyword">open</a> <a id="36591" class="Keyword">import</a> <a id="36598" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="36636" class="Keyword">open</a> <a id="36641" class="Keyword">import</a> <a id="36648" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="36691" class="Keyword">open</a> <a id="36696" class="Keyword">import</a> <a id="36703" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="36739" class="Keyword">open</a> <a id="36744" class="Keyword">import</a> <a id="36751" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36781" class="Keyword">open</a> <a id="36786" class="Keyword">import</a> <a id="36793" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36827" class="Keyword">open</a> <a id="36832" class="Keyword">import</a> <a id="36839" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36870" class="Keyword">open</a> <a id="36875" class="Keyword">import</a> <a id="36882" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36941" class="Keyword">open</a> <a id="36946" class="Keyword">import</a> <a id="36953" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="37004" class="Keyword">open</a> <a id="37009" class="Keyword">import</a> <a id="37016" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="37067" class="Keyword">open</a> <a id="37072" class="Keyword">import</a> <a id="37079" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="37134" class="Keyword">open</a> <a id="37139" class="Keyword">import</a> <a id="37146" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="37178" class="Keyword">open</a> <a id="37183" class="Keyword">import</a> <a id="37190" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="37219" class="Keyword">open</a> <a id="37224" class="Keyword">import</a> <a id="37231" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="37259" class="Keyword">open</a> <a id="37264" class="Keyword">import</a> <a id="37271" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="37301" class="Keyword">open</a> <a id="37306" class="Keyword">import</a> <a id="37313" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="37347" class="Keyword">open</a> <a id="37352" class="Keyword">import</a> <a id="37359" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="37435" class="Keyword">open</a> <a id="37440" class="Keyword">import</a> <a id="37447" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="37473" class="Keyword">open</a> <a id="37478" class="Keyword">import</a> <a id="37485" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="37523" class="Keyword">open</a> <a id="37528" class="Keyword">import</a> <a id="37535" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="37572" class="Keyword">open</a> <a id="37577" class="Keyword">import</a> <a id="37584" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="37624" class="Keyword">open</a> <a id="37629" class="Keyword">import</a> <a id="37636" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="37675" class="Keyword">open</a> <a id="37680" class="Keyword">import</a> <a id="37687" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="37720" class="Keyword">open</a> <a id="37725" class="Keyword">import</a> <a id="37732" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="37775" class="Keyword">open</a> <a id="37780" class="Keyword">import</a> <a id="37787" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37822" class="Keyword">open</a> <a id="37827" class="Keyword">import</a> <a id="37834" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37879" class="Keyword">open</a> <a id="37884" class="Keyword">import</a> <a id="37891" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37928" class="Keyword">open</a> <a id="37933" class="Keyword">import</a> <a id="37940" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37992" class="Keyword">open</a> <a id="37997" class="Keyword">import</a> <a id="38004" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="38057" class="Keyword">open</a> <a id="38062" class="Keyword">import</a> <a id="38069" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="38129" class="Keyword">open</a> <a id="38134" class="Keyword">import</a> <a id="38141" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="38189" class="Keyword">open</a> <a id="38194" class="Keyword">import</a> <a id="38201" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="38241" class="Keyword">open</a> <a id="38246" class="Keyword">import</a> <a id="38253" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="38300" class="Keyword">open</a> <a id="38305" class="Keyword">import</a> <a id="38312" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="38353" class="Keyword">open</a> <a id="38358" class="Keyword">import</a> <a id="38365" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="38403" class="Keyword">open</a> <a id="38408" class="Keyword">import</a> <a id="38415" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="38463" class="Keyword">open</a> <a id="38468" class="Keyword">import</a> <a id="38475" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="38512" class="Keyword">open</a> <a id="38517" class="Keyword">import</a> <a id="38524" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="38559" class="Keyword">open</a> <a id="38564" class="Keyword">import</a> <a id="38571" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="38605" class="Keyword">open</a> <a id="38610" class="Keyword">import</a> <a id="38617" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="38664" class="Keyword">open</a> <a id="38669" class="Keyword">import</a> <a id="38676" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="38721" class="Keyword">open</a> <a id="38726" class="Keyword">import</a> <a id="38733" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38782" class="Keyword">open</a> <a id="38787" class="Keyword">import</a> <a id="38794" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38846" class="Keyword">open</a> <a id="38851" class="Keyword">import</a> <a id="38858" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38912" class="Keyword">open</a> <a id="38917" class="Keyword">import</a> <a id="38924" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Type theories

<pre class="Agda"><a id="39005" class="Keyword">open</a> <a id="39010" class="Keyword">import</a> <a id="39017" href="type-theories.html" class="Module">type-theories</a>
<a id="39031" class="Keyword">open</a> <a id="39036" class="Keyword">import</a> <a id="39043" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="39085" class="Keyword">open</a> <a id="39090" class="Keyword">import</a> <a id="39097" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="39135" class="Keyword">open</a> <a id="39140" class="Keyword">import</a> <a id="39147" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="39193" class="Keyword">open</a> <a id="39198" class="Keyword">import</a> <a id="39205" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="39252" class="Keyword">open</a> <a id="39257" class="Keyword">import</a> <a id="39264" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="39299" class="Keyword">open</a> <a id="39304" class="Keyword">import</a> <a id="39311" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="39389" class="Keyword">open</a> <a id="39394" class="Keyword">import</a> <a id="39401" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="39425" class="Keyword">open</a> <a id="39430" class="Keyword">import</a> <a id="39437" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="39490" class="Keyword">open</a> <a id="39495" class="Keyword">import</a> <a id="39502" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="39545" class="Keyword">open</a> <a id="39550" class="Keyword">import</a> <a id="39557" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="39597" class="Keyword">open</a> <a id="39602" class="Keyword">import</a> <a id="39609" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="39648" class="Keyword">open</a> <a id="39653" class="Keyword">import</a> <a id="39660" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="39694" class="Keyword">open</a> <a id="39699" class="Keyword">import</a> <a id="39706" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39754" class="Keyword">open</a> <a id="39759" class="Keyword">import</a> <a id="39766" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39817" class="Keyword">open</a> <a id="39822" class="Keyword">import</a> <a id="39829" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39876" class="Keyword">open</a> <a id="39881" class="Keyword">import</a> <a id="39888" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39940" class="Keyword">open</a> <a id="39945" class="Keyword">import</a> <a id="39952" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39996" class="Keyword">open</a> <a id="40001" class="Keyword">import</a> <a id="40008" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="40048" class="Keyword">open</a> <a id="40053" class="Keyword">import</a> <a id="40060" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="40103" class="Keyword">open</a> <a id="40108" class="Keyword">import</a> <a id="40115" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="40167" class="Keyword">open</a> <a id="40172" class="Keyword">import</a> <a id="40179" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="40233" class="Keyword">open</a> <a id="40238" class="Keyword">import</a> <a id="40245" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="40293" class="Keyword">open</a> <a id="40298" class="Keyword">import</a> <a id="40305" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="40344" class="Keyword">open</a> <a id="40349" class="Keyword">import</a> <a id="40356" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="40389" class="Keyword">open</a> <a id="40394" class="Keyword">import</a> <a id="40401" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="40431" class="Keyword">open</a> <a id="40436" class="Keyword">import</a> <a id="40443" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="40494" class="Keyword">open</a> <a id="40499" class="Keyword">import</a> <a id="40506" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="40547" class="Keyword">open</a> <a id="40552" class="Keyword">import</a> <a id="40559" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="40596" class="Keyword">open</a> <a id="40601" class="Keyword">import</a> <a id="40608" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="40667" class="Keyword">open</a> <a id="40672" class="Keyword">import</a> <a id="40679" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40734" class="Keyword">open</a> <a id="40739" class="Keyword">import</a> <a id="40746" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40802" class="Keyword">open</a> <a id="40807" class="Keyword">import</a> <a id="40814" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40861" class="Keyword">open</a> <a id="40866" class="Keyword">import</a> <a id="40873" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40916" class="Keyword">open</a> <a id="40921" class="Keyword">import</a> <a id="40928" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40973" class="Keyword">open</a> <a id="40978" class="Keyword">import</a> <a id="40985" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="41034" class="Keyword">open</a> <a id="41039" class="Keyword">import</a> <a id="41046" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="41097" class="Keyword">open</a> <a id="41102" class="Keyword">import</a> <a id="41109" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="41153" class="Keyword">open</a> <a id="41158" class="Keyword">import</a> <a id="41165" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="41243" class="Keyword">open</a> <a id="41248" class="Keyword">import</a> <a id="41255" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="41295" class="Keyword">open</a> <a id="41300" class="Keyword">import</a> <a id="41307" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="41364" class="Keyword">open</a> <a id="41369" class="Keyword">import</a> <a id="41376" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="41411" class="Keyword">open</a> <a id="41416" class="Keyword">import</a> <a id="41423" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="41469" class="Keyword">open</a> <a id="41474" class="Keyword">import</a> <a id="41481" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="41536" class="Keyword">open</a> <a id="41541" class="Keyword">import</a> <a id="41548" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="41591" class="Keyword">open</a> <a id="41596" class="Keyword">import</a> <a id="41603" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="41648" class="Keyword">open</a> <a id="41653" class="Keyword">import</a> <a id="41660" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41719" class="Keyword">open</a> <a id="41724" class="Keyword">import</a> <a id="41731" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41768" class="Keyword">open</a> <a id="41773" class="Keyword">import</a> <a id="41780" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41822" class="Keyword">open</a> <a id="41827" class="Keyword">import</a> <a id="41834" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41875" class="Keyword">open</a> <a id="41880" class="Keyword">import</a> <a id="41887" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41926" class="Keyword">open</a> <a id="41931" class="Keyword">import</a> <a id="41938" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41976" class="Keyword">open</a> <a id="41981" class="Keyword">import</a> <a id="41988" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="42040" class="Keyword">open</a> <a id="42045" class="Keyword">import</a> <a id="42052" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="42097" class="Keyword">open</a> <a id="42102" class="Keyword">import</a> <a id="42109" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="42148" class="Keyword">open</a> <a id="42153" class="Keyword">import</a> <a id="42160" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="42197" class="Keyword">open</a> <a id="42202" class="Keyword">import</a> <a id="42209" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="42258" class="Keyword">open</a> <a id="42263" class="Keyword">import</a> <a id="42270" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="42309" class="Keyword">open</a> <a id="42314" class="Keyword">import</a> <a id="42321" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="42359" class="Keyword">open</a> <a id="42364" class="Keyword">import</a> <a id="42371" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="42426" class="Keyword">open</a> <a id="42431" class="Keyword">import</a> <a id="42438" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="42477" class="Keyword">open</a> <a id="42482" class="Keyword">import</a> <a id="42489" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="42537" class="Keyword">open</a> <a id="42542" class="Keyword">import</a> <a id="42549" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="42596" class="Keyword">open</a> <a id="42601" class="Keyword">import</a> <a id="42608" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="42646" class="Keyword">open</a> <a id="42651" class="Keyword">import</a> <a id="42658" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="42688" class="Keyword">open</a> <a id="42693" class="Keyword">import</a> <a id="42700" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42757" class="Keyword">open</a> <a id="42762" class="Keyword">import</a> <a id="42769" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42823" class="Keyword">open</a> <a id="42828" class="Keyword">import</a> <a id="42835" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42865" class="Keyword">open</a> <a id="42870" class="Keyword">import</a> <a id="42877" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42926" class="Keyword">open</a> <a id="42931" class="Keyword">import</a> <a id="42938" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42980" class="Keyword">open</a> <a id="42985" class="Keyword">import</a> <a id="42992" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="43026" class="Keyword">open</a> <a id="43031" class="Keyword">import</a> <a id="43038" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="43101" class="Keyword">open</a> <a id="43106" class="Keyword">import</a> <a id="43113" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="43156" class="Keyword">open</a> <a id="43161" class="Keyword">import</a> <a id="43168" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="43203" class="Keyword">open</a> <a id="43208" class="Keyword">import</a> <a id="43215" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="43250" class="Keyword">open</a> <a id="43255" class="Keyword">import</a> <a id="43262" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="43302" class="Keyword">open</a> <a id="43307" class="Keyword">import</a> <a id="43314" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="43359" class="Keyword">open</a> <a id="43364" class="Keyword">import</a> <a id="43371" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="43412" class="Keyword">open</a> <a id="43417" class="Keyword">import</a> <a id="43424" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="43478" class="Keyword">open</a> <a id="43483" class="Keyword">import</a> <a id="43490" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="43540" class="Keyword">open</a> <a id="43545" class="Keyword">import</a> <a id="43552" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="43599" class="Keyword">open</a> <a id="43604" class="Keyword">import</a> <a id="43611" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="43649" class="Keyword">open</a> <a id="43654" class="Keyword">import</a> <a id="43661" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="43710" class="Keyword">open</a> <a id="43715" class="Keyword">import</a> <a id="43722" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43769" class="Keyword">open</a> <a id="43774" class="Keyword">import</a> <a id="43781" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43844" class="Keyword">open</a> <a id="43849" class="Keyword">import</a> <a id="43856" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43888" class="Keyword">open</a> <a id="43893" class="Keyword">import</a> <a id="43900" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43953" class="Keyword">open</a> <a id="43958" class="Keyword">import</a> <a id="43965" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="44011" class="Keyword">open</a> <a id="44016" class="Keyword">import</a> <a id="44023" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="44069" class="Keyword">open</a> <a id="44074" class="Keyword">import</a> <a id="44081" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="44121" class="Keyword">open</a> <a id="44126" class="Keyword">import</a> <a id="44133" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="44180" class="Keyword">open</a> <a id="44185" class="Keyword">import</a> <a id="44192" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="44240" class="Keyword">open</a> <a id="44245" class="Keyword">import</a> <a id="44252" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="44292" class="Keyword">open</a> <a id="44297" class="Keyword">import</a> <a id="44304" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="44349" class="Keyword">open</a> <a id="44354" class="Keyword">import</a> <a id="44361" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="44426" class="Keyword">open</a> <a id="44431" class="Keyword">import</a> <a id="44438" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="44483" class="Keyword">open</a> <a id="44488" class="Keyword">import</a> <a id="44495" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="44542" class="Keyword">open</a> <a id="44547" class="Keyword">import</a> <a id="44554" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="44607" class="Keyword">open</a> <a id="44612" class="Keyword">import</a> <a id="44619" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>