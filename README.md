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
<a id="11962" class="Keyword">open</a> <a id="11967" class="Keyword">import</a> <a id="11974" href="foundation.axiom-of-choice.html" class="Module">foundation.axiom-of-choice</a>
<a id="12001" class="Keyword">open</a> <a id="12006" class="Keyword">import</a> <a id="12013" href="foundation.bands.html" class="Module">foundation.bands</a>
<a id="12030" class="Keyword">open</a> <a id="12035" class="Keyword">import</a> <a id="12042" href="foundation.binary-embeddings.html" class="Module">foundation.binary-embeddings</a>
<a id="12071" class="Keyword">open</a> <a id="12076" class="Keyword">import</a> <a id="12083" href="foundation.binary-equivalences-unordered-pairs-of-types.html" class="Module">foundation.binary-equivalences-unordered-pairs-of-types</a>
<a id="12139" class="Keyword">open</a> <a id="12144" class="Keyword">import</a> <a id="12151" href="foundation.binary-equivalences.html" class="Module">foundation.binary-equivalences</a>
<a id="12182" class="Keyword">open</a> <a id="12187" class="Keyword">import</a> <a id="12194" href="foundation.binary-operations-unordered-pairs-of-types.html" class="Module">foundation.binary-operations-unordered-pairs-of-types</a>
<a id="12248" class="Keyword">open</a> <a id="12253" class="Keyword">import</a> <a id="12260" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="12288" class="Keyword">open</a> <a id="12293" class="Keyword">import</a> <a id="12300" href="foundation.boolean-reflection.html" class="Module">foundation.boolean-reflection</a>
<a id="12330" class="Keyword">open</a> <a id="12335" class="Keyword">import</a> <a id="12342" href="foundation.booleans.html" class="Module">foundation.booleans</a>
<a id="12362" class="Keyword">open</a> <a id="12367" class="Keyword">import</a> <a id="12374" href="foundation.cantor-schroder-bernstein-escardo.html" class="Module">foundation.cantor-schroder-bernstein-escardo</a>
<a id="12419" class="Keyword">open</a> <a id="12424" class="Keyword">import</a> <a id="12431" href="foundation.cantors-diagonal-argument.html" class="Module">foundation.cantors-diagonal-argument</a>
<a id="12468" class="Keyword">open</a> <a id="12473" class="Keyword">import</a> <a id="12480" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="12515" class="Keyword">open</a> <a id="12520" class="Keyword">import</a> <a id="12527" href="foundation.choice-of-representatives-equivalence-relation.html" class="Module">foundation.choice-of-representatives-equivalence-relation</a>
<a id="12585" class="Keyword">open</a> <a id="12590" class="Keyword">import</a> <a id="12597" href="foundation.coherently-invertible-maps.html" class="Module">foundation.coherently-invertible-maps</a>
<a id="12635" class="Keyword">open</a> <a id="12640" class="Keyword">import</a> <a id="12647" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="12681" class="Keyword">open</a> <a id="12686" class="Keyword">import</a> <a id="12693" href="foundation.commuting-cubes.html" class="Module">foundation.commuting-cubes</a>
<a id="12720" class="Keyword">open</a> <a id="12725" class="Keyword">import</a> <a id="12732" href="foundation.commuting-squares.html" class="Module">foundation.commuting-squares</a>
<a id="12761" class="Keyword">open</a> <a id="12766" class="Keyword">import</a> <a id="12773" href="foundation.complements.html" class="Module">foundation.complements</a>
<a id="12796" class="Keyword">open</a> <a id="12801" class="Keyword">import</a> <a id="12808" href="foundation.cones-pullbacks.html" class="Module">foundation.cones-pullbacks</a>
<a id="12835" class="Keyword">open</a> <a id="12840" class="Keyword">import</a> <a id="12847" href="foundation.conjunction.html" class="Module">foundation.conjunction</a>
<a id="12870" class="Keyword">open</a> <a id="12875" class="Keyword">import</a> <a id="12882" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="12924" class="Keyword">open</a> <a id="12929" class="Keyword">import</a> <a id="12936" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="12968" class="Keyword">open</a> <a id="12973" class="Keyword">import</a> <a id="12980" href="foundation.connected-maps.html" class="Module">foundation.connected-maps</a>
<a id="13006" class="Keyword">open</a> <a id="13011" class="Keyword">import</a> <a id="13018" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="13045" class="Keyword">open</a> <a id="13050" class="Keyword">import</a> <a id="13057" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="13082" class="Keyword">open</a> <a id="13087" class="Keyword">import</a> <a id="13094" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="13123" class="Keyword">open</a> <a id="13128" class="Keyword">import</a> <a id="13135" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="13165" class="Keyword">open</a> <a id="13170" class="Keyword">import</a> <a id="13177" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="13204" class="Keyword">open</a> <a id="13209" class="Keyword">import</a> <a id="13216" href="foundation.coslice.html" class="Module">foundation.coslice</a>
<a id="13235" class="Keyword">open</a> <a id="13240" class="Keyword">import</a> <a id="13247" href="foundation.cospans.html" class="Module">foundation.cospans</a>
<a id="13266" class="Keyword">open</a> <a id="13271" class="Keyword">import</a> <a id="13278" href="foundation.decidable-dependent-function-types.html" class="Module">foundation.decidable-dependent-function-types</a>
<a id="13324" class="Keyword">open</a> <a id="13329" class="Keyword">import</a> <a id="13336" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a>
<a id="13378" class="Keyword">open</a> <a id="13383" class="Keyword">import</a> <a id="13390" href="foundation.decidable-embeddings.html" class="Module">foundation.decidable-embeddings</a>
<a id="13422" class="Keyword">open</a> <a id="13427" class="Keyword">import</a> <a id="13434" href="foundation.decidable-equality.html" class="Module">foundation.decidable-equality</a>
<a id="13464" class="Keyword">open</a> <a id="13469" class="Keyword">import</a> <a id="13476" href="foundation.decidable-equivalence-relations.html" class="Module">foundation.decidable-equivalence-relations</a>
<a id="13519" class="Keyword">open</a> <a id="13524" class="Keyword">import</a> <a id="13531" href="foundation.decidable-maps.html" class="Module">foundation.decidable-maps</a>
<a id="13557" class="Keyword">open</a> <a id="13562" class="Keyword">import</a> <a id="13569" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="13603" class="Keyword">open</a> <a id="13608" class="Keyword">import</a> <a id="13615" href="foundation.decidable-relations.html" class="Module">foundation.decidable-relations</a>
<a id="13646" class="Keyword">open</a> <a id="13651" class="Keyword">import</a> <a id="13658" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="13688" class="Keyword">open</a> <a id="13693" class="Keyword">import</a> <a id="13700" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a>
<a id="13727" class="Keyword">open</a> <a id="13732" class="Keyword">import</a> <a id="13739" href="foundation.dependent-binomial-theorem.html" class="Module">foundation.dependent-binomial-theorem</a>
<a id="13777" class="Keyword">open</a> <a id="13782" class="Keyword">import</a> <a id="13789" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="13821" class="Keyword">open</a> <a id="13826" class="Keyword">import</a> <a id="13833" href="foundation.descent-coproduct-types.html" class="Module">foundation.descent-coproduct-types</a>
<a id="13868" class="Keyword">open</a> <a id="13873" class="Keyword">import</a> <a id="13880" href="foundation.descent-dependent-pair-types.html" class="Module">foundation.descent-dependent-pair-types</a>
<a id="13920" class="Keyword">open</a> <a id="13925" class="Keyword">import</a> <a id="13932" href="foundation.descent-empty-types.html" class="Module">foundation.descent-empty-types</a>
<a id="13963" class="Keyword">open</a> <a id="13968" class="Keyword">import</a> <a id="13975" href="foundation.diagonal-maps-of-types.html" class="Module">foundation.diagonal-maps-of-types</a>
<a id="14009" class="Keyword">open</a> <a id="14014" class="Keyword">import</a> <a id="14021" href="foundation.diagonals-of-maps.html" class="Module">foundation.diagonals-of-maps</a>
<a id="14050" class="Keyword">open</a> <a id="14055" class="Keyword">import</a> <a id="14062" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="14085" class="Keyword">open</a> <a id="14090" class="Keyword">import</a> <a id="14097" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="14124" class="Keyword">open</a> <a id="14129" class="Keyword">import</a> <a id="14136" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="14164" class="Keyword">open</a> <a id="14169" class="Keyword">import</a> <a id="14176" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="14213" class="Keyword">open</a> <a id="14218" class="Keyword">import</a> <a id="14225" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="14273" class="Keyword">open</a> <a id="14278" class="Keyword">import</a> <a id="14285" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="14325" class="Keyword">open</a> <a id="14330" class="Keyword">import</a> <a id="14337" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="14359" class="Keyword">open</a> <a id="14364" class="Keyword">import</a> <a id="14371" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="14394" class="Keyword">open</a> <a id="14399" class="Keyword">import</a> <a id="14406" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="14431" class="Keyword">open</a> <a id="14436" class="Keyword">import</a> <a id="14443" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="14488" class="Keyword">open</a> <a id="14493" class="Keyword">import</a> <a id="14500" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="14544" class="Keyword">open</a> <a id="14549" class="Keyword">import</a> <a id="14556" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14592" class="Keyword">open</a> <a id="14597" class="Keyword">import</a> <a id="14604" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14649" class="Keyword">open</a> <a id="14654" class="Keyword">import</a> <a id="14661" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14702" class="Keyword">open</a> <a id="14707" class="Keyword">import</a> <a id="14714" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14749" class="Keyword">open</a> <a id="14754" class="Keyword">import</a> <a id="14761" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14793" class="Keyword">open</a> <a id="14798" class="Keyword">import</a> <a id="14805" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14836" class="Keyword">open</a> <a id="14841" class="Keyword">import</a> <a id="14848" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14881" class="Keyword">open</a> <a id="14886" class="Keyword">import</a> <a id="14893" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14926" class="Keyword">open</a> <a id="14931" class="Keyword">import</a> <a id="14938" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14968" class="Keyword">open</a> <a id="14973" class="Keyword">import</a> <a id="14980" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="15004" class="Keyword">open</a> <a id="15009" class="Keyword">import</a> <a id="15016" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="15054" class="Keyword">open</a> <a id="15059" class="Keyword">import</a> <a id="15066" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="15097" class="Keyword">open</a> <a id="15102" class="Keyword">import</a> <a id="15109" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="15134" class="Keyword">open</a> <a id="15139" class="Keyword">import</a> <a id="15146" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="15174" class="Keyword">open</a> <a id="15179" class="Keyword">import</a> <a id="15186" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="15210" class="Keyword">open</a> <a id="15215" class="Keyword">import</a> <a id="15222" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="15248" class="Keyword">open</a> <a id="15253" class="Keyword">import</a> <a id="15260" href="foundation.full-subtypes.html" class="Module">foundation.full-subtypes</a>
<a id="15285" class="Keyword">open</a> <a id="15290" class="Keyword">import</a> <a id="15297" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="15332" class="Keyword">open</a> <a id="15337" class="Keyword">import</a> <a id="15344" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="15365" class="Keyword">open</a> <a id="15370" class="Keyword">import</a> <a id="15377" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="15426" class="Keyword">open</a> <a id="15431" class="Keyword">import</a> <a id="15438" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="15479" class="Keyword">open</a> <a id="15484" class="Keyword">import</a> <a id="15491" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="15541" class="Keyword">open</a> <a id="15546" class="Keyword">import</a> <a id="15553" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="15599" class="Keyword">open</a> <a id="15604" class="Keyword">import</a> <a id="15611" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15651" class="Keyword">open</a> <a id="15656" class="Keyword">import</a> <a id="15663" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15703" class="Keyword">open</a> <a id="15708" class="Keyword">import</a> <a id="15715" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15765" class="Keyword">open</a> <a id="15770" class="Keyword">import</a> <a id="15777" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15816" class="Keyword">open</a> <a id="15821" class="Keyword">import</a> <a id="15828" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15868" class="Keyword">open</a> <a id="15873" class="Keyword">import</a> <a id="15880" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15913" class="Keyword">open</a> <a id="15918" class="Keyword">import</a> <a id="15925" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="15974" class="Keyword">open</a> <a id="15979" class="Keyword">import</a> <a id="15986" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="16011" class="Keyword">open</a> <a id="16016" class="Keyword">import</a> <a id="16023" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="16062" class="Keyword">open</a> <a id="16067" class="Keyword">import</a> <a id="16074" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="16112" class="Keyword">open</a> <a id="16117" class="Keyword">import</a> <a id="16124" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="16146" class="Keyword">open</a> <a id="16151" class="Keyword">import</a> <a id="16158" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="16186" class="Keyword">open</a> <a id="16191" class="Keyword">import</a> <a id="16198" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="16234" class="Keyword">open</a> <a id="16239" class="Keyword">import</a> <a id="16246" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="16272" class="Keyword">open</a> <a id="16277" class="Keyword">import</a> <a id="16284" href="foundation.images.html" class="Module">foundation.images</a>
<a id="16302" class="Keyword">open</a> <a id="16307" class="Keyword">import</a> <a id="16314" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="16349" class="Keyword">open</a> <a id="16354" class="Keyword">import</a> <a id="16361" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="16396" class="Keyword">open</a> <a id="16401" class="Keyword">import</a> <a id="16408" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="16435" class="Keyword">open</a> <a id="16440" class="Keyword">import</a> <a id="16447" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="16503" class="Keyword">open</a> <a id="16508" class="Keyword">import</a> <a id="16515" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="16544" class="Keyword">open</a> <a id="16549" class="Keyword">import</a> <a id="16556" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="16586" class="Keyword">open</a> <a id="16591" class="Keyword">import</a> <a id="16598" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="16625" class="Keyword">open</a> <a id="16630" class="Keyword">import</a> <a id="16637" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16663" class="Keyword">open</a> <a id="16668" class="Keyword">import</a> <a id="16675" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16702" class="Keyword">open</a> <a id="16707" class="Keyword">import</a> <a id="16714" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16738" class="Keyword">open</a> <a id="16743" class="Keyword">import</a> <a id="16750" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16773" class="Keyword">open</a> <a id="16778" class="Keyword">import</a> <a id="16785" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16812" class="Keyword">open</a> <a id="16817" class="Keyword">import</a> <a id="16824" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16856" class="Keyword">open</a> <a id="16861" class="Keyword">import</a> <a id="16868" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16903" class="Keyword">open</a> <a id="16908" class="Keyword">import</a> <a id="16915" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16946" class="Keyword">open</a> <a id="16951" class="Keyword">import</a> <a id="16958" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="16991" class="Keyword">open</a> <a id="16996" class="Keyword">import</a> <a id="17003" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="17037" class="Keyword">open</a> <a id="17042" class="Keyword">import</a> <a id="17049" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="17089" class="Keyword">open</a> <a id="17094" class="Keyword">import</a> <a id="17101" href="foundation.lesser-limited-principle-of-omniscience.html" class="Module">foundation.lesser-limited-principle-of-omniscience</a>
<a id="17152" class="Keyword">open</a> <a id="17157" class="Keyword">import</a> <a id="17164" href="foundation.limited-principle-of-omniscience.html" class="Module">foundation.limited-principle-of-omniscience</a>
<a id="17208" class="Keyword">open</a> <a id="17213" class="Keyword">import</a> <a id="17220" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="17251" class="Keyword">open</a> <a id="17256" class="Keyword">import</a> <a id="17263" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="17295" class="Keyword">open</a> <a id="17300" class="Keyword">import</a> <a id="17307" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="17338" class="Keyword">open</a> <a id="17343" class="Keyword">import</a> <a id="17350" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="17367" class="Keyword">open</a> <a id="17372" class="Keyword">import</a> <a id="17379" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="17404" class="Keyword">open</a> <a id="17409" class="Keyword">import</a> <a id="17416" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="17445" class="Keyword">open</a> <a id="17450" class="Keyword">import</a> <a id="17457" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="17482" class="Keyword">open</a> <a id="17487" class="Keyword">import</a> <a id="17494" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="17523" class="Keyword">open</a> <a id="17528" class="Keyword">import</a> <a id="17535" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="17556" class="Keyword">open</a> <a id="17561" class="Keyword">import</a> <a id="17568" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="17592" class="Keyword">open</a> <a id="17597" class="Keyword">import</a> <a id="17604" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="17624" class="Keyword">open</a> <a id="17629" class="Keyword">import</a> <a id="17636" href="foundation.noncontractible-types.html" class="Module">foundation.noncontractible-types</a>
<a id="17669" class="Keyword">open</a> <a id="17674" class="Keyword">import</a> <a id="17681" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17719" class="Keyword">open</a> <a id="17724" class="Keyword">import</a> <a id="17731" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17759" class="Keyword">open</a> <a id="17764" class="Keyword">import</a> <a id="17771" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17795" class="Keyword">open</a> <a id="17800" class="Keyword">import</a> <a id="17807" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17834" class="Keyword">open</a> <a id="17839" class="Keyword">import</a> <a id="17846" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17881" class="Keyword">open</a> <a id="17886" class="Keyword">import</a> <a id="17893" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17914" class="Keyword">open</a> <a id="17919" class="Keyword">import</a> <a id="17926" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17962" class="Keyword">open</a> <a id="17967" class="Keyword">import</a> <a id="17974" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="18019" class="Keyword">open</a> <a id="18024" class="Keyword">import</a> <a id="18031" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="18077" class="Keyword">open</a> <a id="18082" class="Keyword">import</a> <a id="18089" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="18129" class="Keyword">open</a> <a id="18134" class="Keyword">import</a> <a id="18141" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="18171" class="Keyword">open</a> <a id="18176" class="Keyword">import</a> <a id="18183" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="18217" class="Keyword">open</a> <a id="18222" class="Keyword">import</a> <a id="18229" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="18266" class="Keyword">open</a> <a id="18271" class="Keyword">import</a> <a id="18278" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="18302" class="Keyword">open</a> <a id="18307" class="Keyword">import</a> <a id="18314" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="18335" class="Keyword">open</a> <a id="18340" class="Keyword">import</a> <a id="18347" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="18382" class="Keyword">open</a> <a id="18387" class="Keyword">import</a> <a id="18394" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="18431" class="Keyword">open</a> <a id="18436" class="Keyword">import</a> <a id="18443" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="18492" class="Keyword">open</a> <a id="18497" class="Keyword">import</a> <a id="18504" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="18537" class="Keyword">open</a> <a id="18542" class="Keyword">import</a> <a id="18549" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="18572" class="Keyword">open</a> <a id="18577" class="Keyword">import</a> <a id="18584" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="18607" class="Keyword">open</a> <a id="18612" class="Keyword">import</a> <a id="18619" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18642" class="Keyword">open</a> <a id="18647" class="Keyword">import</a> <a id="18654" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18682" class="Keyword">open</a> <a id="18687" class="Keyword">import</a> <a id="18694" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18714" class="Keyword">open</a> <a id="18719" class="Keyword">import</a> <a id="18726" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18747" class="Keyword">open</a> <a id="18752" class="Keyword">import</a> <a id="18759" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18790" class="Keyword">open</a> <a id="18795" class="Keyword">import</a> <a id="18802" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18829" class="Keyword">open</a> <a id="18834" class="Keyword">import</a> <a id="18841" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18857" class="Keyword">open</a> <a id="18862" class="Keyword">import</a> <a id="18869" href="foundation.sigma-decompositions.html" class="Module">foundation.sigma-decompositions</a>
<a id="18901" class="Keyword">open</a> <a id="18906" class="Keyword">import</a> <a id="18913" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18944" class="Keyword">open</a> <a id="18949" class="Keyword">import</a> <a id="18956" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18973" class="Keyword">open</a> <a id="18978" class="Keyword">import</a> <a id="18985" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="19007" class="Keyword">open</a> <a id="19012" class="Keyword">import</a> <a id="19019" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="19046" class="Keyword">open</a> <a id="19051" class="Keyword">import</a> <a id="19058" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="19081" class="Keyword">open</a> <a id="19086" class="Keyword">import</a> <a id="19093" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="19120" class="Keyword">open</a> <a id="19125" class="Keyword">import</a> <a id="19132" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="19165" class="Keyword">open</a> <a id="19170" class="Keyword">import</a> <a id="19177" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="19217" class="Keyword">open</a> <a id="19222" class="Keyword">import</a> <a id="19229" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="19250" class="Keyword">open</a> <a id="19255" class="Keyword">import</a> <a id="19262" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="19291" class="Keyword">open</a> <a id="19296" class="Keyword">import</a> <a id="19303" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="19341" class="Keyword">open</a> <a id="19346" class="Keyword">import</a> <a id="19353" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="19373" class="Keyword">open</a> <a id="19378" class="Keyword">import</a> <a id="19385" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="19409" class="Keyword">open</a> <a id="19414" class="Keyword">import</a> <a id="19421" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="19448" class="Keyword">open</a> <a id="19453" class="Keyword">import</a> <a id="19460" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="19492" class="Keyword">open</a> <a id="19497" class="Keyword">import</a> <a id="19504" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="19534" class="Keyword">open</a> <a id="19539" class="Keyword">import</a> <a id="19546" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19572" class="Keyword">open</a> <a id="19577" class="Keyword">import</a> <a id="19584" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19611" class="Keyword">open</a> <a id="19616" class="Keyword">import</a> <a id="19623" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19660" class="Keyword">open</a> <a id="19665" class="Keyword">import</a> <a id="19672" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19701" class="Keyword">open</a> <a id="19706" class="Keyword">import</a> <a id="19713" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19736" class="Keyword">open</a> <a id="19741" class="Keyword">import</a> <a id="19748" href="foundation.type-arithmetic-booleans.html" class="Module">foundation.type-arithmetic-booleans</a>
<a id="19784" class="Keyword">open</a> <a id="19789" class="Keyword">import</a> <a id="19796" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19847" class="Keyword">open</a> <a id="19852" class="Keyword">import</a> <a id="19859" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19902" class="Keyword">open</a> <a id="19907" class="Keyword">import</a> <a id="19914" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19966" class="Keyword">open</a> <a id="19971" class="Keyword">import</a> <a id="19978" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="20026" class="Keyword">open</a> <a id="20031" class="Keyword">import</a> <a id="20038" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="20076" class="Keyword">open</a> <a id="20081" class="Keyword">import</a> <a id="20088" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="20125" class="Keyword">open</a> <a id="20130" class="Keyword">import</a> <a id="20137" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="20183" class="Keyword">open</a> <a id="20188" class="Keyword">import</a> <a id="20195" href="foundation.union.html" class="Module">foundation.union</a>
<a id="20212" class="Keyword">open</a> <a id="20217" class="Keyword">import</a> <a id="20224" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="20252" class="Keyword">open</a> <a id="20257" class="Keyword">import</a> <a id="20264" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="20292" class="Keyword">open</a> <a id="20297" class="Keyword">import</a> <a id="20304" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="20340" class="Keyword">open</a> <a id="20345" class="Keyword">import</a> <a id="20352" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="20390" class="Keyword">open</a> <a id="20395" class="Keyword">import</a> <a id="20402" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="20435" class="Keyword">open</a> <a id="20440" class="Keyword">import</a> <a id="20447" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="20468" class="Keyword">open</a> <a id="20473" class="Keyword">import</a> <a id="20480" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="20516" class="Keyword">open</a> <a id="20521" class="Keyword">import</a> <a id="20528" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="20582" class="Keyword">open</a> <a id="20587" class="Keyword">import</a> <a id="20594" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20616" class="Keyword">open</a> <a id="20621" class="Keyword">import</a> <a id="20628" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20663" class="Keyword">open</a> <a id="20668" class="Keyword">import</a> <a id="20675" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20705" class="Keyword">open</a> <a id="20710" class="Keyword">import</a> <a id="20717" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20756" class="Keyword">open</a> <a id="20761" class="Keyword">import</a> <a id="20768" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20822" class="Keyword">open</a> <a id="20827" class="Keyword">import</a> <a id="20834" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20880" class="Keyword">open</a> <a id="20885" class="Keyword">import</a> <a id="20892" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20943" class="Keyword">open</a> <a id="20948" class="Keyword">import</a> <a id="20955" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20996" class="Keyword">open</a> <a id="21001" class="Keyword">import</a> <a id="21008" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="21053" class="Keyword">open</a> <a id="21058" class="Keyword">import</a> <a id="21065" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="21110" class="Keyword">open</a> <a id="21115" class="Keyword">import</a> <a id="21122" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="21158" class="Keyword">open</a> <a id="21163" class="Keyword">import</a> <a id="21170" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="21206" class="Keyword">open</a> <a id="21211" class="Keyword">import</a> <a id="21218" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="21283" class="Keyword">open</a> <a id="21288" class="Keyword">import</a> <a id="21295" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="21350" class="Keyword">open</a> <a id="21355" class="Keyword">import</a> <a id="21362" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="21402" class="Keyword">open</a> <a id="21407" class="Keyword">import</a> <a id="21414" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="21458" class="Keyword">open</a> <a id="21463" class="Keyword">import</a> <a id="21470" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="21515" class="Keyword">open</a> <a id="21520" class="Keyword">import</a> <a id="21527" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="21568" class="Keyword">open</a> <a id="21573" class="Keyword">import</a> <a id="21580" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21620" class="Keyword">open</a> <a id="21625" class="Keyword">import</a> <a id="21632" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21659" class="Keyword">open</a> <a id="21664" class="Keyword">import</a> <a id="21671" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21707" class="Keyword">open</a> <a id="21712" class="Keyword">import</a> <a id="21719" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21746" class="Keyword">open</a> <a id="21751" class="Keyword">import</a> <a id="21758" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21795" class="Keyword">open</a> <a id="21800" class="Keyword">import</a> <a id="21807" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21835" class="Keyword">open</a> <a id="21840" class="Keyword">import</a> <a id="21847" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21866" class="Keyword">open</a> <a id="21871" class="Keyword">import</a> <a id="21878" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21918" class="Keyword">open</a> <a id="21923" class="Keyword">import</a> <a id="21930" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="21979" class="Keyword">open</a> <a id="21984" class="Keyword">import</a> <a id="21991" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="22023" class="Keyword">open</a> <a id="22028" class="Keyword">import</a> <a id="22035" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="22083" class="Keyword">open</a> <a id="22088" class="Keyword">import</a> <a id="22095" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="22118" class="Keyword">open</a> <a id="22123" class="Keyword">import</a> <a id="22130" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="22154" class="Keyword">open</a> <a id="22159" class="Keyword">import</a> <a id="22166" href="foundation-core.automorphisms.html" class="Module">foundation-core.automorphisms</a>
<a id="22196" class="Keyword">open</a> <a id="22201" class="Keyword">import</a> <a id="22208" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="22248" class="Keyword">open</a> <a id="22253" class="Keyword">import</a> <a id="22260" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22303" class="Keyword">open</a> <a id="22308" class="Keyword">import</a> <a id="22315" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22349" class="Keyword">open</a> <a id="22354" class="Keyword">import</a> <a id="22361" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22393" class="Keyword">open</a> <a id="22398" class="Keyword">import</a> <a id="22405" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22435" class="Keyword">open</a> <a id="22440" class="Keyword">import</a> <a id="22447" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22481" class="Keyword">open</a> <a id="22486" class="Keyword">import</a> <a id="22493" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22528" class="Keyword">open</a> <a id="22533" class="Keyword">import</a> <a id="22540" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22564" class="Keyword">open</a> <a id="22569" class="Keyword">import</a> <a id="22576" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22613" class="Keyword">open</a> <a id="22618" class="Keyword">import</a> <a id="22625" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22652" class="Keyword">open</a> <a id="22657" class="Keyword">import</a> <a id="22664" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22692" class="Keyword">open</a> <a id="22697" class="Keyword">import</a> <a id="22704" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22734" class="Keyword">open</a> <a id="22739" class="Keyword">import</a> <a id="22746" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22795" class="Keyword">open</a> <a id="22800" class="Keyword">import</a> <a id="22807" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22853" class="Keyword">open</a> <a id="22858" class="Keyword">import</a> <a id="22865" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22905" class="Keyword">open</a> <a id="22910" class="Keyword">import</a> <a id="22917" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22955" class="Keyword">open</a> <a id="22960" class="Keyword">import</a> <a id="22967" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22996" class="Keyword">open</a> <a id="23001" class="Keyword">import</a> <a id="23008" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="23038" class="Keyword">open</a> <a id="23043" class="Keyword">import</a> <a id="23050" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="23081" class="Keyword">open</a> <a id="23086" class="Keyword">import</a> <a id="23093" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="23133" class="Keyword">open</a> <a id="23138" class="Keyword">import</a> <a id="23145" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="23171" class="Keyword">open</a> <a id="23176" class="Keyword">import</a> <a id="23183" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="23238" class="Keyword">open</a> <a id="23243" class="Keyword">import</a> <a id="23250" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23301" class="Keyword">open</a> <a id="23306" class="Keyword">import</a> <a id="23313" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23358" class="Keyword">open</a> <a id="23363" class="Keyword">import</a> <a id="23370" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23415" class="Keyword">open</a> <a id="23420" class="Keyword">import</a> <a id="23427" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23481" class="Keyword">open</a> <a id="23486" class="Keyword">import</a> <a id="23493" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23520" class="Keyword">open</a> <a id="23525" class="Keyword">import</a> <a id="23532" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23565" class="Keyword">open</a> <a id="23570" class="Keyword">import</a> <a id="23577" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23608" class="Keyword">open</a> <a id="23613" class="Keyword">import</a> <a id="23620" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23657" class="Keyword">open</a> <a id="23662" class="Keyword">import</a> <a id="23669" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23703" class="Keyword">open</a> <a id="23708" class="Keyword">import</a> <a id="23715" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23740" class="Keyword">open</a> <a id="23745" class="Keyword">import</a> <a id="23752" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23784" class="Keyword">open</a> <a id="23789" class="Keyword">import</a> <a id="23796" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23831" class="Keyword">open</a> <a id="23836" class="Keyword">import</a> <a id="23843" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23872" class="Keyword">open</a> <a id="23877" class="Keyword">import</a> <a id="23884" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23910" class="Keyword">open</a> <a id="23915" class="Keyword">import</a> <a id="23922" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23950" class="Keyword">open</a> <a id="23955" class="Keyword">import</a> <a id="23962" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23987" class="Keyword">open</a> <a id="23992" class="Keyword">import</a> <a id="23999" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="24020" class="Keyword">open</a> <a id="24025" class="Keyword">import</a> <a id="24032" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="24068" class="Keyword">open</a> <a id="24073" class="Keyword">import</a> <a id="24080" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="24123" class="Keyword">open</a> <a id="24128" class="Keyword">import</a> <a id="24135" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="24160" class="Keyword">open</a> <a id="24165" class="Keyword">import</a> <a id="24172" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="24203" class="Keyword">open</a> <a id="24208" class="Keyword">import</a> <a id="24215" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="24247" class="Keyword">open</a> <a id="24252" class="Keyword">import</a> <a id="24259" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24293" class="Keyword">open</a> <a id="24298" class="Keyword">import</a> <a id="24305" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24361" class="Keyword">open</a> <a id="24366" class="Keyword">import</a> <a id="24373" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24426" class="Keyword">open</a> <a id="24431" class="Keyword">import</a> <a id="24438" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24465" class="Keyword">open</a> <a id="24470" class="Keyword">import</a> <a id="24477" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24522" class="Keyword">open</a> <a id="24527" class="Keyword">import</a> <a id="24534" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24596" class="Keyword">open</a> <a id="24601" class="Keyword">import</a> <a id="24608" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24621" class="Keyword">open</a> <a id="24626" class="Keyword">import</a> <a id="24633" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24673" class="Keyword">open</a> <a id="24678" class="Keyword">import</a> <a id="24685" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24729" class="Keyword">open</a> <a id="24734" class="Keyword">import</a> <a id="24741" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24780" class="Keyword">open</a> <a id="24785" class="Keyword">import</a> <a id="24792" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24834" class="Keyword">open</a> <a id="24839" class="Keyword">import</a> <a id="24846" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24886" class="Keyword">open</a> <a id="24891" class="Keyword">import</a> <a id="24898" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24939" class="Keyword">open</a> <a id="24944" class="Keyword">import</a> <a id="24951" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24989" class="Keyword">open</a> <a id="24994" class="Keyword">import</a> <a id="25001" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="25064" class="Keyword">open</a> <a id="25069" class="Keyword">import</a> <a id="25076" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="25105" class="Keyword">open</a> <a id="25110" class="Keyword">import</a> <a id="25117" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="25162" class="Keyword">open</a> <a id="25167" class="Keyword">import</a> <a id="25174" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="25216" class="Keyword">open</a> <a id="25221" class="Keyword">import</a> <a id="25228" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25268" class="Keyword">open</a> <a id="25273" class="Keyword">import</a> <a id="25280" href="graph-theory.equivalences-enriched-undirected-graphs.html" class="Module">graph-theory.equivalences-enriched-undirected-graphs</a>
<a id="25333" class="Keyword">open</a> <a id="25338" class="Keyword">import</a> <a id="25345" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25389" class="Keyword">open</a> <a id="25394" class="Keyword">import</a> <a id="25401" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25450" class="Keyword">open</a> <a id="25455" class="Keyword">import</a> <a id="25462" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25512" class="Keyword">open</a> <a id="25517" class="Keyword">import</a> <a id="25524" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25551" class="Keyword">open</a> <a id="25556" class="Keyword">import</a> <a id="25563" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25588" class="Keyword">open</a> <a id="25593" class="Keyword">import</a> <a id="25600" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25623" class="Keyword">open</a> <a id="25628" class="Keyword">import</a> <a id="25635" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25684" class="Keyword">open</a> <a id="25689" class="Keyword">import</a> <a id="25696" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25735" class="Keyword">open</a> <a id="25740" class="Keyword">import</a> <a id="25747" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25788" class="Keyword">open</a> <a id="25793" class="Keyword">import</a> <a id="25800" href="graph-theory.neighbors-undirected-graphs.html" class="Module">graph-theory.neighbors-undirected-graphs</a>
<a id="25841" class="Keyword">open</a> <a id="25846" class="Keyword">import</a> <a id="25853" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25897" class="Keyword">open</a> <a id="25902" class="Keyword">import</a> <a id="25909" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25946" class="Keyword">open</a> <a id="25951" class="Keyword">import</a> <a id="25958" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="25980" class="Keyword">open</a> <a id="25985" class="Keyword">import</a> <a id="25992" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="26022" class="Keyword">open</a> <a id="26027" class="Keyword">import</a> <a id="26034" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="26073" class="Keyword">open</a> <a id="26078" class="Keyword">import</a> <a id="26085" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="26116" class="Keyword">open</a> <a id="26121" class="Keyword">import</a> <a id="26128" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="26154" class="Keyword">open</a> <a id="26159" class="Keyword">import</a> <a id="26166" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="26204" class="Keyword">open</a> <a id="26209" class="Keyword">import</a> <a id="26216" href="graph-theory.stereoisomerism-enriched-undirected-graphs.html" class="Module">graph-theory.stereoisomerism-enriched-undirected-graphs</a>
<a id="26272" class="Keyword">open</a> <a id="26277" class="Keyword">import</a> <a id="26284" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="26342" class="Keyword">open</a> <a id="26347" class="Keyword">import</a> <a id="26354" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="26392" class="Keyword">open</a> <a id="26397" class="Keyword">import</a> <a id="26404" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26423" class="Keyword">open</a> <a id="26428" class="Keyword">import</a> <a id="26435" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26500" class="Keyword">open</a> <a id="26505" class="Keyword">import</a> <a id="26512" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26543" class="Keyword">open</a> <a id="26548" class="Keyword">import</a> <a id="26555" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26582" class="Keyword">open</a> <a id="26587" class="Keyword">import</a> <a id="26594" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26622" class="Keyword">open</a> <a id="26627" class="Keyword">import</a> <a id="26634" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26701" class="Keyword">open</a> <a id="26706" class="Keyword">import</a> <a id="26713" href="group-theory.html" class="Module">group-theory</a>
<a id="26726" class="Keyword">open</a> <a id="26731" class="Keyword">import</a> <a id="26738" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26766" class="Keyword">open</a> <a id="26771" class="Keyword">import</a> <a id="26778" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26829" class="Keyword">open</a> <a id="26834" class="Keyword">import</a> <a id="26841" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="26874" class="Keyword">open</a> <a id="26879" class="Keyword">import</a> <a id="26886" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26933" class="Keyword">open</a> <a id="26938" class="Keyword">import</a> <a id="26945" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26984" class="Keyword">open</a> <a id="26989" class="Keyword">import</a> <a id="26996" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="27036" class="Keyword">open</a> <a id="27041" class="Keyword">import</a> <a id="27048" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="27091" class="Keyword">open</a> <a id="27096" class="Keyword">import</a> <a id="27103" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="27135" class="Keyword">open</a> <a id="27140" class="Keyword">import</a> <a id="27147" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="27183" class="Keyword">open</a> <a id="27188" class="Keyword">import</a> <a id="27195" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="27224" class="Keyword">open</a> <a id="27229" class="Keyword">import</a> <a id="27236" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="27264" class="Keyword">open</a> <a id="27269" class="Keyword">import</a> <a id="27276" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="27309" class="Keyword">open</a> <a id="27314" class="Keyword">import</a> <a id="27321" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="27357" class="Keyword">open</a> <a id="27362" class="Keyword">import</a> <a id="27369" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27398" class="Keyword">open</a> <a id="27403" class="Keyword">import</a> <a id="27410" href="group-theory.congruence-relations-groups.html" class="Module">group-theory.congruence-relations-groups</a>
<a id="27451" class="Keyword">open</a> <a id="27456" class="Keyword">import</a> <a id="27463" href="group-theory.congruence-relations-monoids.html" class="Module">group-theory.congruence-relations-monoids</a>
<a id="27505" class="Keyword">open</a> <a id="27510" class="Keyword">import</a> <a id="27517" href="group-theory.congruence-relations-semigroups.html" class="Module">group-theory.congruence-relations-semigroups</a>
<a id="27562" class="Keyword">open</a> <a id="27567" class="Keyword">import</a> <a id="27574" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27599" class="Keyword">open</a> <a id="27604" class="Keyword">import</a> <a id="27611" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27673" class="Keyword">open</a> <a id="27678" class="Keyword">import</a> <a id="27685" href="group-theory.decidable-subgroups.html" class="Module">group-theory.decidable-subgroups</a>
<a id="27718" class="Keyword">open</a> <a id="27723" class="Keyword">import</a> <a id="27730" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27771" class="Keyword">open</a> <a id="27776" class="Keyword">import</a> <a id="27783" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27812" class="Keyword">open</a> <a id="27817" class="Keyword">import</a> <a id="27824" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27848" class="Keyword">open</a> <a id="27853" class="Keyword">import</a> <a id="27860" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27891" class="Keyword">open</a> <a id="27896" class="Keyword">import</a> <a id="27903" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27950" class="Keyword">open</a> <a id="27955" class="Keyword">import</a> <a id="27962" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="27995" class="Keyword">open</a> <a id="28000" class="Keyword">import</a> <a id="28007" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="28056" class="Keyword">open</a> <a id="28061" class="Keyword">import</a> <a id="28068" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="28108" class="Keyword">open</a> <a id="28113" class="Keyword">import</a> <a id="28120" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="28160" class="Keyword">open</a> <a id="28165" class="Keyword">import</a> <a id="28172" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="28209" class="Keyword">open</a> <a id="28214" class="Keyword">import</a> <a id="28221" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="28268" class="Keyword">open</a> <a id="28273" class="Keyword">import</a> <a id="28280" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="28321" class="Keyword">open</a> <a id="28326" class="Keyword">import</a> <a id="28333" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="28377" class="Keyword">open</a> <a id="28382" class="Keyword">import</a> <a id="28389" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="28428" class="Keyword">open</a> <a id="28433" class="Keyword">import</a> <a id="28440" href="group-theory.full-subgroups.html" class="Module">group-theory.full-subgroups</a>
<a id="28468" class="Keyword">open</a> <a id="28473" class="Keyword">import</a> <a id="28480" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28512" class="Keyword">open</a> <a id="28517" class="Keyword">import</a> <a id="28524" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28551" class="Keyword">open</a> <a id="28556" class="Keyword">import</a> <a id="28563" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28583" class="Keyword">open</a> <a id="28588" class="Keyword">import</a> <a id="28595" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28629" class="Keyword">open</a> <a id="28634" class="Keyword">import</a> <a id="28641" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28668" class="Keyword">open</a> <a id="28673" class="Keyword">import</a> <a id="28680" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28722" class="Keyword">open</a> <a id="28727" class="Keyword">import</a> <a id="28734" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28784" class="Keyword">open</a> <a id="28789" class="Keyword">import</a> <a id="28796" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28843" class="Keyword">open</a> <a id="28848" class="Keyword">import</a> <a id="28855" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28896" class="Keyword">open</a> <a id="28901" class="Keyword">import</a> <a id="28908" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28942" class="Keyword">open</a> <a id="28947" class="Keyword">import</a> <a id="28954" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="29002" class="Keyword">open</a> <a id="29007" class="Keyword">import</a> <a id="29014" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="29055" class="Keyword">open</a> <a id="29060" class="Keyword">import</a> <a id="29067" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="29102" class="Keyword">open</a> <a id="29107" class="Keyword">import</a> <a id="29114" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="29152" class="Keyword">open</a> <a id="29157" class="Keyword">import</a> <a id="29164" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="29199" class="Keyword">open</a> <a id="29204" class="Keyword">import</a> <a id="29211" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="29243" class="Keyword">open</a> <a id="29248" class="Keyword">import</a> <a id="29255" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="29296" class="Keyword">open</a> <a id="29301" class="Keyword">import</a> <a id="29308" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="29349" class="Keyword">open</a> <a id="29354" class="Keyword">import</a> <a id="29361" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="29401" class="Keyword">open</a> <a id="29406" class="Keyword">import</a> <a id="29413" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="29446" class="Keyword">open</a> <a id="29451" class="Keyword">import</a> <a id="29458" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29495" class="Keyword">open</a> <a id="29500" class="Keyword">import</a> <a id="29507" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29537" class="Keyword">open</a> <a id="29542" class="Keyword">import</a> <a id="29549" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29570" class="Keyword">open</a> <a id="29575" class="Keyword">import</a> <a id="29582" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29636" class="Keyword">open</a> <a id="29641" class="Keyword">import</a> <a id="29648" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29693" class="Keyword">open</a> <a id="29698" class="Keyword">import</a> <a id="29705" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29733" class="Keyword">open</a> <a id="29738" class="Keyword">import</a> <a id="29745" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29766" class="Keyword">open</a> <a id="29771" class="Keyword">import</a> <a id="29778" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29821" class="Keyword">open</a> <a id="29826" class="Keyword">import</a> <a id="29833" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29867" class="Keyword">open</a> <a id="29872" class="Keyword">import</a> <a id="29879" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29909" class="Keyword">open</a> <a id="29914" class="Keyword">import</a> <a id="29921" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29967" class="Keyword">open</a> <a id="29972" class="Keyword">import</a> <a id="29979" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="30033" class="Keyword">open</a> <a id="30038" class="Keyword">import</a> <a id="30045" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="30088" class="Keyword">open</a> <a id="30093" class="Keyword">import</a> <a id="30100" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="30134" class="Keyword">open</a> <a id="30139" class="Keyword">import</a> <a id="30146" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="30187" class="Keyword">open</a> <a id="30192" class="Keyword">import</a> <a id="30199" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="30234" class="Keyword">open</a> <a id="30239" class="Keyword">import</a> <a id="30246" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a>
<a id="30285" class="Keyword">open</a> <a id="30290" class="Keyword">import</a> <a id="30297" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="30339" class="Keyword">open</a> <a id="30344" class="Keyword">import</a> <a id="30351" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="30386" class="Keyword">open</a> <a id="30391" class="Keyword">import</a> <a id="30398" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="30437" class="Keyword">open</a> <a id="30442" class="Keyword">import</a> <a id="30449" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="30486" class="Keyword">open</a> <a id="30491" class="Keyword">import</a> <a id="30498" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30545" class="Keyword">open</a> <a id="30550" class="Keyword">import</a> <a id="30557" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30621" class="Keyword">open</a> <a id="30626" class="Keyword">import</a> <a id="30633" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30678" class="Keyword">open</a> <a id="30683" class="Keyword">import</a> <a id="30690" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30714" class="Keyword">open</a> <a id="30719" class="Keyword">import</a> <a id="30726" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30751" class="Keyword">open</a> <a id="30756" class="Keyword">import</a> <a id="30763" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30806" class="Keyword">open</a> <a id="30811" class="Keyword">import</a> <a id="30818" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30849" class="Keyword">open</a> <a id="30854" class="Keyword">import</a> <a id="30861" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30915" class="Keyword">open</a> <a id="30920" class="Keyword">import</a> <a id="30927" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30950" class="Keyword">open</a> <a id="30955" class="Keyword">import</a> <a id="30962" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="31000" class="Keyword">open</a> <a id="31005" class="Keyword">import</a> <a id="31012" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="31051" class="Keyword">open</a> <a id="31056" class="Keyword">import</a> <a id="31063" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="31114" class="Keyword">open</a> <a id="31119" class="Keyword">import</a> <a id="31126" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="31163" class="Keyword">open</a> <a id="31168" class="Keyword">import</a> <a id="31175" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="31199" class="Keyword">open</a> <a id="31204" class="Keyword">import</a> <a id="31211" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="31238" class="Keyword">open</a> <a id="31243" class="Keyword">import</a> <a id="31250" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="31307" class="Keyword">open</a> <a id="31312" class="Keyword">import</a> <a id="31319" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="31367" class="Keyword">open</a> <a id="31372" class="Keyword">import</a> <a id="31379" href="group-theory.symmetric-concrete-groups.html" class="Module">group-theory.symmetric-concrete-groups</a>
<a id="31418" class="Keyword">open</a> <a id="31423" class="Keyword">import</a> <a id="31430" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="31460" class="Keyword">open</a> <a id="31465" class="Keyword">import</a> <a id="31472" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="31509" class="Keyword">open</a> <a id="31514" class="Keyword">import</a> <a id="31521" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="31542" class="Keyword">open</a> <a id="31547" class="Keyword">import</a> <a id="31554" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31601" class="Keyword">open</a> <a id="31606" class="Keyword">import</a> <a id="31613" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31651" class="Keyword">open</a> <a id="31656" class="Keyword">import</a> <a id="31663" href="group-theory.trivial-subgroups.html" class="Module">group-theory.trivial-subgroups</a>
<a id="31694" class="Keyword">open</a> <a id="31699" class="Keyword">import</a> <a id="31706" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31800" class="Keyword">open</a> <a id="31805" class="Keyword">import</a> <a id="31812" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31827" class="Keyword">open</a> <a id="31832" class="Keyword">import</a> <a id="31839" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31872" class="Keyword">open</a> <a id="31877" class="Keyword">import</a> <a id="31884" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="31916" class="Keyword">open</a> <a id="31921" class="Keyword">import</a> <a id="31928" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="31970" class="Keyword">open</a> <a id="31975" class="Keyword">import</a> <a id="31982" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="32020" class="Keyword">open</a> <a id="32025" class="Keyword">import</a> <a id="32032" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="32069" class="Keyword">open</a> <a id="32074" class="Keyword">import</a> <a id="32081" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="32114" class="Keyword">open</a> <a id="32119" class="Keyword">import</a> <a id="32126" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="32150" class="Keyword">open</a> <a id="32155" class="Keyword">import</a> <a id="32162" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="32201" class="Keyword">open</a> <a id="32206" class="Keyword">import</a> <a id="32213" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="32259" class="Keyword">open</a> <a id="32264" class="Keyword">import</a> <a id="32271" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="32316" class="Keyword">open</a> <a id="32321" class="Keyword">import</a> <a id="32328" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="32366" class="Keyword">open</a> <a id="32371" class="Keyword">import</a> <a id="32378" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="32410" class="Keyword">open</a> <a id="32415" class="Keyword">import</a> <a id="32422" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="32475" class="Keyword">open</a> <a id="32480" class="Keyword">import</a> <a id="32487" href="order-theory.html" class="Module">order-theory</a>
<a id="32500" class="Keyword">open</a> <a id="32505" class="Keyword">import</a> <a id="32512" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="32539" class="Keyword">open</a> <a id="32544" class="Keyword">import</a> <a id="32551" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="32581" class="Keyword">open</a> <a id="32586" class="Keyword">import</a> <a id="32593" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32626" class="Keyword">open</a> <a id="32631" class="Keyword">import</a> <a id="32638" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32674" class="Keyword">open</a> <a id="32679" class="Keyword">import</a> <a id="32686" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32721" class="Keyword">open</a> <a id="32726" class="Keyword">import</a> <a id="32733" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32760" class="Keyword">open</a> <a id="32765" class="Keyword">import</a> <a id="32772" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32802" class="Keyword">open</a> <a id="32807" class="Keyword">import</a> <a id="32814" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32850" class="Keyword">open</a> <a id="32855" class="Keyword">import</a> <a id="32862" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="32904" class="Keyword">open</a> <a id="32909" class="Keyword">import</a> <a id="32916" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32946" class="Keyword">open</a> <a id="32951" class="Keyword">import</a> <a id="32958" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="32990" class="Keyword">open</a> <a id="32995" class="Keyword">import</a> <a id="33002" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="33033" class="Keyword">open</a> <a id="33038" class="Keyword">import</a> <a id="33045" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="33071" class="Keyword">open</a> <a id="33076" class="Keyword">import</a> <a id="33083" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="33112" class="Keyword">open</a> <a id="33117" class="Keyword">import</a> <a id="33124" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="33161" class="Keyword">open</a> <a id="33166" class="Keyword">import</a> <a id="33173" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="33213" class="Keyword">open</a> <a id="33218" class="Keyword">import</a> <a id="33225" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="33247" class="Keyword">open</a> <a id="33252" class="Keyword">import</a> <a id="33259" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="33294" class="Keyword">open</a> <a id="33299" class="Keyword">import</a> <a id="33306" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="33344" class="Keyword">open</a> <a id="33349" class="Keyword">import</a> <a id="33356" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="33395" class="Keyword">open</a> <a id="33400" class="Keyword">import</a> <a id="33407" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="33442" class="Keyword">open</a> <a id="33447" class="Keyword">import</a> <a id="33454" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="33489" class="Keyword">open</a> <a id="33494" class="Keyword">import</a> <a id="33501" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="33536" class="Keyword">open</a> <a id="33541" class="Keyword">import</a> <a id="33548" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="33586" class="Keyword">open</a> <a id="33591" class="Keyword">import</a> <a id="33598" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33629" class="Keyword">open</a> <a id="33634" class="Keyword">import</a> <a id="33641" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33683" class="Keyword">open</a> <a id="33688" class="Keyword">import</a> <a id="33695" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33740" class="Keyword">open</a> <a id="33745" class="Keyword">import</a> <a id="33752" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33785" class="Keyword">open</a> <a id="33790" class="Keyword">import</a> <a id="33797" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33817" class="Keyword">open</a> <a id="33822" class="Keyword">import</a> <a id="33829" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33852" class="Keyword">open</a> <a id="33857" class="Keyword">import</a> <a id="33864" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="33887" class="Keyword">open</a> <a id="33892" class="Keyword">import</a> <a id="33899" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33925" class="Keyword">open</a> <a id="33930" class="Keyword">import</a> <a id="33937" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33963" class="Keyword">open</a> <a id="33968" class="Keyword">import</a> <a id="33975" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="34039" class="Keyword">open</a> <a id="34044" class="Keyword">import</a> <a id="34051" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="34069" class="Keyword">open</a> <a id="34074" class="Keyword">import</a> <a id="34081" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="34108" class="Keyword">open</a> <a id="34113" class="Keyword">import</a> <a id="34120" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="34146" class="Keyword">open</a> <a id="34151" class="Keyword">import</a> <a id="34158" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="34184" class="Keyword">open</a> <a id="34189" class="Keyword">import</a> <a id="34196" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="34222" class="Keyword">open</a> <a id="34227" class="Keyword">import</a> <a id="34234" href="organic-chemistry.ethane.html" class="Module">organic-chemistry.ethane</a>
<a id="34259" class="Keyword">open</a> <a id="34264" class="Keyword">import</a> <a id="34271" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="34302" class="Keyword">open</a> <a id="34307" class="Keyword">import</a> <a id="34314" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="34340" class="Keyword">open</a> <a id="34345" class="Keyword">import</a> <a id="34352" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="34415" class="Keyword">open</a> <a id="34420" class="Keyword">import</a> <a id="34427" href="polytopes.html" class="Module">polytopes</a>
<a id="34437" class="Keyword">open</a> <a id="34442" class="Keyword">import</a> <a id="34449" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="34507" class="Keyword">open</a> <a id="34512" class="Keyword">import</a> <a id="34519" href="ring-theory.html" class="Module">ring-theory</a>
<a id="34531" class="Keyword">open</a> <a id="34536" class="Keyword">import</a> <a id="34543" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="34580" class="Keyword">open</a> <a id="34585" class="Keyword">import</a> <a id="34592" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="34619" class="Keyword">open</a> <a id="34624" class="Keyword">import</a> <a id="34631" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34663" class="Keyword">open</a> <a id="34668" class="Keyword">import</a> <a id="34675" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34721" class="Keyword">open</a> <a id="34726" class="Keyword">import</a> <a id="34733" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34758" class="Keyword">open</a> <a id="34763" class="Keyword">import</a> <a id="34770" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34808" class="Keyword">open</a> <a id="34813" class="Keyword">import</a> <a id="34820" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34863" class="Keyword">open</a> <a id="34868" class="Keyword">import</a> <a id="34875" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="34913" class="Keyword">open</a> <a id="34918" class="Keyword">import</a> <a id="34925" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="34956" class="Keyword">open</a> <a id="34961" class="Keyword">import</a> <a id="34968" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="34992" class="Keyword">open</a> <a id="34997" class="Keyword">import</a> <a id="35004" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="35036" class="Keyword">open</a> <a id="35041" class="Keyword">import</a> <a id="35048" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="35074" class="Keyword">open</a> <a id="35079" class="Keyword">import</a> <a id="35086" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="35115" class="Keyword">open</a> <a id="35120" class="Keyword">import</a> <a id="35127" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="35164" class="Keyword">open</a> <a id="35169" class="Keyword">import</a> <a id="35176" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="35205" class="Keyword">open</a> <a id="35210" class="Keyword">import</a> <a id="35217" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="35244" class="Keyword">open</a> <a id="35249" class="Keyword">import</a> <a id="35256" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="35293" class="Keyword">open</a> <a id="35298" class="Keyword">import</a> <a id="35305" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="35332" class="Keyword">open</a> <a id="35337" class="Keyword">import</a> <a id="35344" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="35377" class="Keyword">open</a> <a id="35382" class="Keyword">import</a> <a id="35389" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="35407" class="Keyword">open</a> <a id="35412" class="Keyword">import</a> <a id="35419" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="35473" class="Keyword">open</a> <a id="35478" class="Keyword">import</a> <a id="35485" href="set-theory.html" class="Module">set-theory</a>
<a id="35496" class="Keyword">open</a> <a id="35501" class="Keyword">import</a> <a id="35508" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="35531" class="Keyword">open</a> <a id="35536" class="Keyword">import</a> <a id="35543" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="35567" class="Keyword">open</a> <a id="35572" class="Keyword">import</a> <a id="35579" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="35604" class="Keyword">open</a> <a id="35609" class="Keyword">import</a> <a id="35616" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="35642" class="Keyword">open</a> <a id="35647" class="Keyword">import</a> <a id="35654" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35716" class="Keyword">open</a> <a id="35721" class="Keyword">import</a> <a id="35728" href="structured-types.html" class="Module">structured-types</a>
<a id="35745" class="Keyword">open</a> <a id="35750" class="Keyword">import</a> <a id="35757" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35792" class="Keyword">open</a> <a id="35797" class="Keyword">import</a> <a id="35804" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35848" class="Keyword">open</a> <a id="35853" class="Keyword">import</a> <a id="35860" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="35924" class="Keyword">open</a> <a id="35929" class="Keyword">import</a> <a id="35936" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="35975" class="Keyword">open</a> <a id="35980" class="Keyword">import</a> <a id="35987" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="36033" class="Keyword">open</a> <a id="36038" class="Keyword">import</a> <a id="36045" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="36110" class="Keyword">open</a> <a id="36115" class="Keyword">import</a> <a id="36122" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="36146" class="Keyword">open</a> <a id="36151" class="Keyword">import</a> <a id="36158" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="36227" class="Keyword">open</a> <a id="36232" class="Keyword">import</a> <a id="36239" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="36284" class="Keyword">open</a> <a id="36289" class="Keyword">import</a> <a id="36296" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="36330" class="Keyword">open</a> <a id="36335" class="Keyword">import</a> <a id="36342" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="36403" class="Keyword">open</a> <a id="36408" class="Keyword">import</a> <a id="36415" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="36460" class="Keyword">open</a> <a id="36465" class="Keyword">import</a> <a id="36472" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="36510" class="Keyword">open</a> <a id="36515" class="Keyword">import</a> <a id="36522" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="36565" class="Keyword">open</a> <a id="36570" class="Keyword">import</a> <a id="36577" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="36613" class="Keyword">open</a> <a id="36618" class="Keyword">import</a> <a id="36625" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36655" class="Keyword">open</a> <a id="36660" class="Keyword">import</a> <a id="36667" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36701" class="Keyword">open</a> <a id="36706" class="Keyword">import</a> <a id="36713" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36744" class="Keyword">open</a> <a id="36749" class="Keyword">import</a> <a id="36756" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36815" class="Keyword">open</a> <a id="36820" class="Keyword">import</a> <a id="36827" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="36878" class="Keyword">open</a> <a id="36883" class="Keyword">import</a> <a id="36890" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="36941" class="Keyword">open</a> <a id="36946" class="Keyword">import</a> <a id="36953" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="37008" class="Keyword">open</a> <a id="37013" class="Keyword">import</a> <a id="37020" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="37052" class="Keyword">open</a> <a id="37057" class="Keyword">import</a> <a id="37064" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="37093" class="Keyword">open</a> <a id="37098" class="Keyword">import</a> <a id="37105" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="37133" class="Keyword">open</a> <a id="37138" class="Keyword">import</a> <a id="37145" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="37175" class="Keyword">open</a> <a id="37180" class="Keyword">import</a> <a id="37187" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="37221" class="Keyword">open</a> <a id="37226" class="Keyword">import</a> <a id="37233" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="37309" class="Keyword">open</a> <a id="37314" class="Keyword">import</a> <a id="37321" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="37347" class="Keyword">open</a> <a id="37352" class="Keyword">import</a> <a id="37359" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="37397" class="Keyword">open</a> <a id="37402" class="Keyword">import</a> <a id="37409" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="37446" class="Keyword">open</a> <a id="37451" class="Keyword">import</a> <a id="37458" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="37498" class="Keyword">open</a> <a id="37503" class="Keyword">import</a> <a id="37510" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="37549" class="Keyword">open</a> <a id="37554" class="Keyword">import</a> <a id="37561" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="37594" class="Keyword">open</a> <a id="37599" class="Keyword">import</a> <a id="37606" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="37649" class="Keyword">open</a> <a id="37654" class="Keyword">import</a> <a id="37661" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37696" class="Keyword">open</a> <a id="37701" class="Keyword">import</a> <a id="37708" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37753" class="Keyword">open</a> <a id="37758" class="Keyword">import</a> <a id="37765" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37802" class="Keyword">open</a> <a id="37807" class="Keyword">import</a> <a id="37814" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37866" class="Keyword">open</a> <a id="37871" class="Keyword">import</a> <a id="37878" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="37931" class="Keyword">open</a> <a id="37936" class="Keyword">import</a> <a id="37943" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="38003" class="Keyword">open</a> <a id="38008" class="Keyword">import</a> <a id="38015" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="38063" class="Keyword">open</a> <a id="38068" class="Keyword">import</a> <a id="38075" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="38115" class="Keyword">open</a> <a id="38120" class="Keyword">import</a> <a id="38127" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="38174" class="Keyword">open</a> <a id="38179" class="Keyword">import</a> <a id="38186" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="38227" class="Keyword">open</a> <a id="38232" class="Keyword">import</a> <a id="38239" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="38277" class="Keyword">open</a> <a id="38282" class="Keyword">import</a> <a id="38289" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="38337" class="Keyword">open</a> <a id="38342" class="Keyword">import</a> <a id="38349" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="38386" class="Keyword">open</a> <a id="38391" class="Keyword">import</a> <a id="38398" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="38433" class="Keyword">open</a> <a id="38438" class="Keyword">import</a> <a id="38445" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="38479" class="Keyword">open</a> <a id="38484" class="Keyword">import</a> <a id="38491" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="38538" class="Keyword">open</a> <a id="38543" class="Keyword">import</a> <a id="38550" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="38595" class="Keyword">open</a> <a id="38600" class="Keyword">import</a> <a id="38607" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38656" class="Keyword">open</a> <a id="38661" class="Keyword">import</a> <a id="38668" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38720" class="Keyword">open</a> <a id="38725" class="Keyword">import</a> <a id="38732" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38786" class="Keyword">open</a> <a id="38791" class="Keyword">import</a> <a id="38798" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Type theories

<pre class="Agda"><a id="38879" class="Keyword">open</a> <a id="38884" class="Keyword">import</a> <a id="38891" href="type-theories.html" class="Module">type-theories</a>
<a id="38905" class="Keyword">open</a> <a id="38910" class="Keyword">import</a> <a id="38917" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="38959" class="Keyword">open</a> <a id="38964" class="Keyword">import</a> <a id="38971" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="39009" class="Keyword">open</a> <a id="39014" class="Keyword">import</a> <a id="39021" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="39067" class="Keyword">open</a> <a id="39072" class="Keyword">import</a> <a id="39079" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="39126" class="Keyword">open</a> <a id="39131" class="Keyword">import</a> <a id="39138" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="39173" class="Keyword">open</a> <a id="39178" class="Keyword">import</a> <a id="39185" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="39263" class="Keyword">open</a> <a id="39268" class="Keyword">import</a> <a id="39275" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="39299" class="Keyword">open</a> <a id="39304" class="Keyword">import</a> <a id="39311" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="39364" class="Keyword">open</a> <a id="39369" class="Keyword">import</a> <a id="39376" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="39419" class="Keyword">open</a> <a id="39424" class="Keyword">import</a> <a id="39431" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="39471" class="Keyword">open</a> <a id="39476" class="Keyword">import</a> <a id="39483" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="39522" class="Keyword">open</a> <a id="39527" class="Keyword">import</a> <a id="39534" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="39568" class="Keyword">open</a> <a id="39573" class="Keyword">import</a> <a id="39580" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39628" class="Keyword">open</a> <a id="39633" class="Keyword">import</a> <a id="39640" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39691" class="Keyword">open</a> <a id="39696" class="Keyword">import</a> <a id="39703" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39750" class="Keyword">open</a> <a id="39755" class="Keyword">import</a> <a id="39762" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39814" class="Keyword">open</a> <a id="39819" class="Keyword">import</a> <a id="39826" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39870" class="Keyword">open</a> <a id="39875" class="Keyword">import</a> <a id="39882" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="39922" class="Keyword">open</a> <a id="39927" class="Keyword">import</a> <a id="39934" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="39977" class="Keyword">open</a> <a id="39982" class="Keyword">import</a> <a id="39989" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="40041" class="Keyword">open</a> <a id="40046" class="Keyword">import</a> <a id="40053" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="40107" class="Keyword">open</a> <a id="40112" class="Keyword">import</a> <a id="40119" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="40167" class="Keyword">open</a> <a id="40172" class="Keyword">import</a> <a id="40179" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="40218" class="Keyword">open</a> <a id="40223" class="Keyword">import</a> <a id="40230" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="40263" class="Keyword">open</a> <a id="40268" class="Keyword">import</a> <a id="40275" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="40305" class="Keyword">open</a> <a id="40310" class="Keyword">import</a> <a id="40317" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="40368" class="Keyword">open</a> <a id="40373" class="Keyword">import</a> <a id="40380" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="40421" class="Keyword">open</a> <a id="40426" class="Keyword">import</a> <a id="40433" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="40470" class="Keyword">open</a> <a id="40475" class="Keyword">import</a> <a id="40482" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="40541" class="Keyword">open</a> <a id="40546" class="Keyword">import</a> <a id="40553" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40608" class="Keyword">open</a> <a id="40613" class="Keyword">import</a> <a id="40620" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40676" class="Keyword">open</a> <a id="40681" class="Keyword">import</a> <a id="40688" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40735" class="Keyword">open</a> <a id="40740" class="Keyword">import</a> <a id="40747" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40790" class="Keyword">open</a> <a id="40795" class="Keyword">import</a> <a id="40802" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40847" class="Keyword">open</a> <a id="40852" class="Keyword">import</a> <a id="40859" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="40908" class="Keyword">open</a> <a id="40913" class="Keyword">import</a> <a id="40920" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="40971" class="Keyword">open</a> <a id="40976" class="Keyword">import</a> <a id="40983" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="41027" class="Keyword">open</a> <a id="41032" class="Keyword">import</a> <a id="41039" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="41117" class="Keyword">open</a> <a id="41122" class="Keyword">import</a> <a id="41129" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="41169" class="Keyword">open</a> <a id="41174" class="Keyword">import</a> <a id="41181" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="41238" class="Keyword">open</a> <a id="41243" class="Keyword">import</a> <a id="41250" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="41285" class="Keyword">open</a> <a id="41290" class="Keyword">import</a> <a id="41297" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="41343" class="Keyword">open</a> <a id="41348" class="Keyword">import</a> <a id="41355" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="41410" class="Keyword">open</a> <a id="41415" class="Keyword">import</a> <a id="41422" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="41465" class="Keyword">open</a> <a id="41470" class="Keyword">import</a> <a id="41477" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="41522" class="Keyword">open</a> <a id="41527" class="Keyword">import</a> <a id="41534" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41593" class="Keyword">open</a> <a id="41598" class="Keyword">import</a> <a id="41605" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41642" class="Keyword">open</a> <a id="41647" class="Keyword">import</a> <a id="41654" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41696" class="Keyword">open</a> <a id="41701" class="Keyword">import</a> <a id="41708" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41749" class="Keyword">open</a> <a id="41754" class="Keyword">import</a> <a id="41761" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41800" class="Keyword">open</a> <a id="41805" class="Keyword">import</a> <a id="41812" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41850" class="Keyword">open</a> <a id="41855" class="Keyword">import</a> <a id="41862" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="41914" class="Keyword">open</a> <a id="41919" class="Keyword">import</a> <a id="41926" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="41971" class="Keyword">open</a> <a id="41976" class="Keyword">import</a> <a id="41983" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="42022" class="Keyword">open</a> <a id="42027" class="Keyword">import</a> <a id="42034" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="42071" class="Keyword">open</a> <a id="42076" class="Keyword">import</a> <a id="42083" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="42132" class="Keyword">open</a> <a id="42137" class="Keyword">import</a> <a id="42144" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="42183" class="Keyword">open</a> <a id="42188" class="Keyword">import</a> <a id="42195" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="42233" class="Keyword">open</a> <a id="42238" class="Keyword">import</a> <a id="42245" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="42300" class="Keyword">open</a> <a id="42305" class="Keyword">import</a> <a id="42312" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="42351" class="Keyword">open</a> <a id="42356" class="Keyword">import</a> <a id="42363" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="42411" class="Keyword">open</a> <a id="42416" class="Keyword">import</a> <a id="42423" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="42470" class="Keyword">open</a> <a id="42475" class="Keyword">import</a> <a id="42482" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="42520" class="Keyword">open</a> <a id="42525" class="Keyword">import</a> <a id="42532" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="42562" class="Keyword">open</a> <a id="42567" class="Keyword">import</a> <a id="42574" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42631" class="Keyword">open</a> <a id="42636" class="Keyword">import</a> <a id="42643" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42697" class="Keyword">open</a> <a id="42702" class="Keyword">import</a> <a id="42709" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42739" class="Keyword">open</a> <a id="42744" class="Keyword">import</a> <a id="42751" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42800" class="Keyword">open</a> <a id="42805" class="Keyword">import</a> <a id="42812" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42854" class="Keyword">open</a> <a id="42859" class="Keyword">import</a> <a id="42866" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="42900" class="Keyword">open</a> <a id="42905" class="Keyword">import</a> <a id="42912" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="42975" class="Keyword">open</a> <a id="42980" class="Keyword">import</a> <a id="42987" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="43030" class="Keyword">open</a> <a id="43035" class="Keyword">import</a> <a id="43042" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="43077" class="Keyword">open</a> <a id="43082" class="Keyword">import</a> <a id="43089" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="43124" class="Keyword">open</a> <a id="43129" class="Keyword">import</a> <a id="43136" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="43176" class="Keyword">open</a> <a id="43181" class="Keyword">import</a> <a id="43188" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="43233" class="Keyword">open</a> <a id="43238" class="Keyword">import</a> <a id="43245" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="43286" class="Keyword">open</a> <a id="43291" class="Keyword">import</a> <a id="43298" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="43352" class="Keyword">open</a> <a id="43357" class="Keyword">import</a> <a id="43364" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="43414" class="Keyword">open</a> <a id="43419" class="Keyword">import</a> <a id="43426" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="43473" class="Keyword">open</a> <a id="43478" class="Keyword">import</a> <a id="43485" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="43523" class="Keyword">open</a> <a id="43528" class="Keyword">import</a> <a id="43535" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="43584" class="Keyword">open</a> <a id="43589" class="Keyword">import</a> <a id="43596" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43643" class="Keyword">open</a> <a id="43648" class="Keyword">import</a> <a id="43655" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43718" class="Keyword">open</a> <a id="43723" class="Keyword">import</a> <a id="43730" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43762" class="Keyword">open</a> <a id="43767" class="Keyword">import</a> <a id="43774" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43827" class="Keyword">open</a> <a id="43832" class="Keyword">import</a> <a id="43839" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="43885" class="Keyword">open</a> <a id="43890" class="Keyword">import</a> <a id="43897" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="43943" class="Keyword">open</a> <a id="43948" class="Keyword">import</a> <a id="43955" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="43995" class="Keyword">open</a> <a id="44000" class="Keyword">import</a> <a id="44007" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="44054" class="Keyword">open</a> <a id="44059" class="Keyword">import</a> <a id="44066" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="44114" class="Keyword">open</a> <a id="44119" class="Keyword">import</a> <a id="44126" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="44166" class="Keyword">open</a> <a id="44171" class="Keyword">import</a> <a id="44178" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="44223" class="Keyword">open</a> <a id="44228" class="Keyword">import</a> <a id="44235" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="44300" class="Keyword">open</a> <a id="44305" class="Keyword">import</a> <a id="44312" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="44357" class="Keyword">open</a> <a id="44362" class="Keyword">import</a> <a id="44369" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="44416" class="Keyword">open</a> <a id="44421" class="Keyword">import</a> <a id="44428" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="44481" class="Keyword">open</a> <a id="44486" class="Keyword">import</a> <a id="44493" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>