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
<a id="18857" class="Keyword">open</a> <a id="18862" class="Keyword">import</a> <a id="18869" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18900" class="Keyword">open</a> <a id="18905" class="Keyword">import</a> <a id="18912" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="18929" class="Keyword">open</a> <a id="18934" class="Keyword">import</a> <a id="18941" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="18963" class="Keyword">open</a> <a id="18968" class="Keyword">import</a> <a id="18975" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="19002" class="Keyword">open</a> <a id="19007" class="Keyword">import</a> <a id="19014" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="19037" class="Keyword">open</a> <a id="19042" class="Keyword">import</a> <a id="19049" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="19076" class="Keyword">open</a> <a id="19081" class="Keyword">import</a> <a id="19088" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="19121" class="Keyword">open</a> <a id="19126" class="Keyword">import</a> <a id="19133" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="19173" class="Keyword">open</a> <a id="19178" class="Keyword">import</a> <a id="19185" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="19206" class="Keyword">open</a> <a id="19211" class="Keyword">import</a> <a id="19218" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="19247" class="Keyword">open</a> <a id="19252" class="Keyword">import</a> <a id="19259" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="19297" class="Keyword">open</a> <a id="19302" class="Keyword">import</a> <a id="19309" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="19329" class="Keyword">open</a> <a id="19334" class="Keyword">import</a> <a id="19341" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="19365" class="Keyword">open</a> <a id="19370" class="Keyword">import</a> <a id="19377" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="19404" class="Keyword">open</a> <a id="19409" class="Keyword">import</a> <a id="19416" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="19448" class="Keyword">open</a> <a id="19453" class="Keyword">import</a> <a id="19460" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="19490" class="Keyword">open</a> <a id="19495" class="Keyword">import</a> <a id="19502" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19528" class="Keyword">open</a> <a id="19533" class="Keyword">import</a> <a id="19540" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19567" class="Keyword">open</a> <a id="19572" class="Keyword">import</a> <a id="19579" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19616" class="Keyword">open</a> <a id="19621" class="Keyword">import</a> <a id="19628" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19657" class="Keyword">open</a> <a id="19662" class="Keyword">import</a> <a id="19669" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19692" class="Keyword">open</a> <a id="19697" class="Keyword">import</a> <a id="19704" href="foundation.type-arithmetic-booleans.html" class="Module">foundation.type-arithmetic-booleans</a>
<a id="19740" class="Keyword">open</a> <a id="19745" class="Keyword">import</a> <a id="19752" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19803" class="Keyword">open</a> <a id="19808" class="Keyword">import</a> <a id="19815" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19858" class="Keyword">open</a> <a id="19863" class="Keyword">import</a> <a id="19870" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19922" class="Keyword">open</a> <a id="19927" class="Keyword">import</a> <a id="19934" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="19982" class="Keyword">open</a> <a id="19987" class="Keyword">import</a> <a id="19994" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="20032" class="Keyword">open</a> <a id="20037" class="Keyword">import</a> <a id="20044" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="20081" class="Keyword">open</a> <a id="20086" class="Keyword">import</a> <a id="20093" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="20139" class="Keyword">open</a> <a id="20144" class="Keyword">import</a> <a id="20151" href="foundation.union.html" class="Module">foundation.union</a>
<a id="20168" class="Keyword">open</a> <a id="20173" class="Keyword">import</a> <a id="20180" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="20208" class="Keyword">open</a> <a id="20213" class="Keyword">import</a> <a id="20220" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="20248" class="Keyword">open</a> <a id="20253" class="Keyword">import</a> <a id="20260" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="20296" class="Keyword">open</a> <a id="20301" class="Keyword">import</a> <a id="20308" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="20346" class="Keyword">open</a> <a id="20351" class="Keyword">import</a> <a id="20358" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="20391" class="Keyword">open</a> <a id="20396" class="Keyword">import</a> <a id="20403" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="20424" class="Keyword">open</a> <a id="20429" class="Keyword">import</a> <a id="20436" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="20472" class="Keyword">open</a> <a id="20477" class="Keyword">import</a> <a id="20484" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="20538" class="Keyword">open</a> <a id="20543" class="Keyword">import</a> <a id="20550" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20572" class="Keyword">open</a> <a id="20577" class="Keyword">import</a> <a id="20584" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20619" class="Keyword">open</a> <a id="20624" class="Keyword">import</a> <a id="20631" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20661" class="Keyword">open</a> <a id="20666" class="Keyword">import</a> <a id="20673" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20712" class="Keyword">open</a> <a id="20717" class="Keyword">import</a> <a id="20724" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20778" class="Keyword">open</a> <a id="20783" class="Keyword">import</a> <a id="20790" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20836" class="Keyword">open</a> <a id="20841" class="Keyword">import</a> <a id="20848" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20899" class="Keyword">open</a> <a id="20904" class="Keyword">import</a> <a id="20911" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="20952" class="Keyword">open</a> <a id="20957" class="Keyword">import</a> <a id="20964" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="21009" class="Keyword">open</a> <a id="21014" class="Keyword">import</a> <a id="21021" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="21066" class="Keyword">open</a> <a id="21071" class="Keyword">import</a> <a id="21078" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="21114" class="Keyword">open</a> <a id="21119" class="Keyword">import</a> <a id="21126" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="21162" class="Keyword">open</a> <a id="21167" class="Keyword">import</a> <a id="21174" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="21239" class="Keyword">open</a> <a id="21244" class="Keyword">import</a> <a id="21251" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="21306" class="Keyword">open</a> <a id="21311" class="Keyword">import</a> <a id="21318" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="21358" class="Keyword">open</a> <a id="21363" class="Keyword">import</a> <a id="21370" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="21414" class="Keyword">open</a> <a id="21419" class="Keyword">import</a> <a id="21426" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="21471" class="Keyword">open</a> <a id="21476" class="Keyword">import</a> <a id="21483" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="21524" class="Keyword">open</a> <a id="21529" class="Keyword">import</a> <a id="21536" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21576" class="Keyword">open</a> <a id="21581" class="Keyword">import</a> <a id="21588" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21615" class="Keyword">open</a> <a id="21620" class="Keyword">import</a> <a id="21627" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21663" class="Keyword">open</a> <a id="21668" class="Keyword">import</a> <a id="21675" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21702" class="Keyword">open</a> <a id="21707" class="Keyword">import</a> <a id="21714" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21751" class="Keyword">open</a> <a id="21756" class="Keyword">import</a> <a id="21763" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21791" class="Keyword">open</a> <a id="21796" class="Keyword">import</a> <a id="21803" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21822" class="Keyword">open</a> <a id="21827" class="Keyword">import</a> <a id="21834" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21874" class="Keyword">open</a> <a id="21879" class="Keyword">import</a> <a id="21886" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="21935" class="Keyword">open</a> <a id="21940" class="Keyword">import</a> <a id="21947" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="21979" class="Keyword">open</a> <a id="21984" class="Keyword">import</a> <a id="21991" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="22039" class="Keyword">open</a> <a id="22044" class="Keyword">import</a> <a id="22051" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="22074" class="Keyword">open</a> <a id="22079" class="Keyword">import</a> <a id="22086" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="22110" class="Keyword">open</a> <a id="22115" class="Keyword">import</a> <a id="22122" href="foundation-core.automorphisms.html" class="Module">foundation-core.automorphisms</a>
<a id="22152" class="Keyword">open</a> <a id="22157" class="Keyword">import</a> <a id="22164" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="22204" class="Keyword">open</a> <a id="22209" class="Keyword">import</a> <a id="22216" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22259" class="Keyword">open</a> <a id="22264" class="Keyword">import</a> <a id="22271" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22305" class="Keyword">open</a> <a id="22310" class="Keyword">import</a> <a id="22317" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22349" class="Keyword">open</a> <a id="22354" class="Keyword">import</a> <a id="22361" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22391" class="Keyword">open</a> <a id="22396" class="Keyword">import</a> <a id="22403" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22437" class="Keyword">open</a> <a id="22442" class="Keyword">import</a> <a id="22449" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22484" class="Keyword">open</a> <a id="22489" class="Keyword">import</a> <a id="22496" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22520" class="Keyword">open</a> <a id="22525" class="Keyword">import</a> <a id="22532" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22569" class="Keyword">open</a> <a id="22574" class="Keyword">import</a> <a id="22581" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22608" class="Keyword">open</a> <a id="22613" class="Keyword">import</a> <a id="22620" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22648" class="Keyword">open</a> <a id="22653" class="Keyword">import</a> <a id="22660" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22690" class="Keyword">open</a> <a id="22695" class="Keyword">import</a> <a id="22702" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22751" class="Keyword">open</a> <a id="22756" class="Keyword">import</a> <a id="22763" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22809" class="Keyword">open</a> <a id="22814" class="Keyword">import</a> <a id="22821" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22861" class="Keyword">open</a> <a id="22866" class="Keyword">import</a> <a id="22873" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22911" class="Keyword">open</a> <a id="22916" class="Keyword">import</a> <a id="22923" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="22952" class="Keyword">open</a> <a id="22957" class="Keyword">import</a> <a id="22964" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="22994" class="Keyword">open</a> <a id="22999" class="Keyword">import</a> <a id="23006" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="23037" class="Keyword">open</a> <a id="23042" class="Keyword">import</a> <a id="23049" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="23089" class="Keyword">open</a> <a id="23094" class="Keyword">import</a> <a id="23101" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="23127" class="Keyword">open</a> <a id="23132" class="Keyword">import</a> <a id="23139" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="23194" class="Keyword">open</a> <a id="23199" class="Keyword">import</a> <a id="23206" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23257" class="Keyword">open</a> <a id="23262" class="Keyword">import</a> <a id="23269" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23314" class="Keyword">open</a> <a id="23319" class="Keyword">import</a> <a id="23326" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23371" class="Keyword">open</a> <a id="23376" class="Keyword">import</a> <a id="23383" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23437" class="Keyword">open</a> <a id="23442" class="Keyword">import</a> <a id="23449" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23476" class="Keyword">open</a> <a id="23481" class="Keyword">import</a> <a id="23488" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23521" class="Keyword">open</a> <a id="23526" class="Keyword">import</a> <a id="23533" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23564" class="Keyword">open</a> <a id="23569" class="Keyword">import</a> <a id="23576" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23613" class="Keyword">open</a> <a id="23618" class="Keyword">import</a> <a id="23625" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23659" class="Keyword">open</a> <a id="23664" class="Keyword">import</a> <a id="23671" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23696" class="Keyword">open</a> <a id="23701" class="Keyword">import</a> <a id="23708" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23740" class="Keyword">open</a> <a id="23745" class="Keyword">import</a> <a id="23752" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23787" class="Keyword">open</a> <a id="23792" class="Keyword">import</a> <a id="23799" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23828" class="Keyword">open</a> <a id="23833" class="Keyword">import</a> <a id="23840" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23866" class="Keyword">open</a> <a id="23871" class="Keyword">import</a> <a id="23878" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23906" class="Keyword">open</a> <a id="23911" class="Keyword">import</a> <a id="23918" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="23943" class="Keyword">open</a> <a id="23948" class="Keyword">import</a> <a id="23955" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="23976" class="Keyword">open</a> <a id="23981" class="Keyword">import</a> <a id="23988" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="24024" class="Keyword">open</a> <a id="24029" class="Keyword">import</a> <a id="24036" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="24079" class="Keyword">open</a> <a id="24084" class="Keyword">import</a> <a id="24091" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="24116" class="Keyword">open</a> <a id="24121" class="Keyword">import</a> <a id="24128" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="24159" class="Keyword">open</a> <a id="24164" class="Keyword">import</a> <a id="24171" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="24203" class="Keyword">open</a> <a id="24208" class="Keyword">import</a> <a id="24215" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24249" class="Keyword">open</a> <a id="24254" class="Keyword">import</a> <a id="24261" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24317" class="Keyword">open</a> <a id="24322" class="Keyword">import</a> <a id="24329" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24382" class="Keyword">open</a> <a id="24387" class="Keyword">import</a> <a id="24394" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24421" class="Keyword">open</a> <a id="24426" class="Keyword">import</a> <a id="24433" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24478" class="Keyword">open</a> <a id="24483" class="Keyword">import</a> <a id="24490" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24552" class="Keyword">open</a> <a id="24557" class="Keyword">import</a> <a id="24564" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24577" class="Keyword">open</a> <a id="24582" class="Keyword">import</a> <a id="24589" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24629" class="Keyword">open</a> <a id="24634" class="Keyword">import</a> <a id="24641" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24685" class="Keyword">open</a> <a id="24690" class="Keyword">import</a> <a id="24697" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24736" class="Keyword">open</a> <a id="24741" class="Keyword">import</a> <a id="24748" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24790" class="Keyword">open</a> <a id="24795" class="Keyword">import</a> <a id="24802" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24842" class="Keyword">open</a> <a id="24847" class="Keyword">import</a> <a id="24854" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24895" class="Keyword">open</a> <a id="24900" class="Keyword">import</a> <a id="24907" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="24945" class="Keyword">open</a> <a id="24950" class="Keyword">import</a> <a id="24957" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="25020" class="Keyword">open</a> <a id="25025" class="Keyword">import</a> <a id="25032" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="25061" class="Keyword">open</a> <a id="25066" class="Keyword">import</a> <a id="25073" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="25118" class="Keyword">open</a> <a id="25123" class="Keyword">import</a> <a id="25130" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="25172" class="Keyword">open</a> <a id="25177" class="Keyword">import</a> <a id="25184" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25224" class="Keyword">open</a> <a id="25229" class="Keyword">import</a> <a id="25236" href="graph-theory.equivalences-enriched-undirected-graphs.html" class="Module">graph-theory.equivalences-enriched-undirected-graphs</a>
<a id="25289" class="Keyword">open</a> <a id="25294" class="Keyword">import</a> <a id="25301" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25345" class="Keyword">open</a> <a id="25350" class="Keyword">import</a> <a id="25357" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25406" class="Keyword">open</a> <a id="25411" class="Keyword">import</a> <a id="25418" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25468" class="Keyword">open</a> <a id="25473" class="Keyword">import</a> <a id="25480" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25507" class="Keyword">open</a> <a id="25512" class="Keyword">import</a> <a id="25519" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25544" class="Keyword">open</a> <a id="25549" class="Keyword">import</a> <a id="25556" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25579" class="Keyword">open</a> <a id="25584" class="Keyword">import</a> <a id="25591" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25640" class="Keyword">open</a> <a id="25645" class="Keyword">import</a> <a id="25652" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25691" class="Keyword">open</a> <a id="25696" class="Keyword">import</a> <a id="25703" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25744" class="Keyword">open</a> <a id="25749" class="Keyword">import</a> <a id="25756" href="graph-theory.neighbors-undirected-graphs.html" class="Module">graph-theory.neighbors-undirected-graphs</a>
<a id="25797" class="Keyword">open</a> <a id="25802" class="Keyword">import</a> <a id="25809" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25853" class="Keyword">open</a> <a id="25858" class="Keyword">import</a> <a id="25865" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25902" class="Keyword">open</a> <a id="25907" class="Keyword">import</a> <a id="25914" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="25936" class="Keyword">open</a> <a id="25941" class="Keyword">import</a> <a id="25948" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="25978" class="Keyword">open</a> <a id="25983" class="Keyword">import</a> <a id="25990" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="26029" class="Keyword">open</a> <a id="26034" class="Keyword">import</a> <a id="26041" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="26072" class="Keyword">open</a> <a id="26077" class="Keyword">import</a> <a id="26084" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="26110" class="Keyword">open</a> <a id="26115" class="Keyword">import</a> <a id="26122" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="26160" class="Keyword">open</a> <a id="26165" class="Keyword">import</a> <a id="26172" href="graph-theory.stereoisomerism-enriched-undirected-graphs.html" class="Module">graph-theory.stereoisomerism-enriched-undirected-graphs</a>
<a id="26228" class="Keyword">open</a> <a id="26233" class="Keyword">import</a> <a id="26240" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="26298" class="Keyword">open</a> <a id="26303" class="Keyword">import</a> <a id="26310" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="26348" class="Keyword">open</a> <a id="26353" class="Keyword">import</a> <a id="26360" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26379" class="Keyword">open</a> <a id="26384" class="Keyword">import</a> <a id="26391" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26456" class="Keyword">open</a> <a id="26461" class="Keyword">import</a> <a id="26468" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26499" class="Keyword">open</a> <a id="26504" class="Keyword">import</a> <a id="26511" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26538" class="Keyword">open</a> <a id="26543" class="Keyword">import</a> <a id="26550" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26578" class="Keyword">open</a> <a id="26583" class="Keyword">import</a> <a id="26590" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26657" class="Keyword">open</a> <a id="26662" class="Keyword">import</a> <a id="26669" href="group-theory.html" class="Module">group-theory</a>
<a id="26682" class="Keyword">open</a> <a id="26687" class="Keyword">import</a> <a id="26694" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26722" class="Keyword">open</a> <a id="26727" class="Keyword">import</a> <a id="26734" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26785" class="Keyword">open</a> <a id="26790" class="Keyword">import</a> <a id="26797" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="26830" class="Keyword">open</a> <a id="26835" class="Keyword">import</a> <a id="26842" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26889" class="Keyword">open</a> <a id="26894" class="Keyword">import</a> <a id="26901" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="26940" class="Keyword">open</a> <a id="26945" class="Keyword">import</a> <a id="26952" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="26992" class="Keyword">open</a> <a id="26997" class="Keyword">import</a> <a id="27004" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="27047" class="Keyword">open</a> <a id="27052" class="Keyword">import</a> <a id="27059" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="27091" class="Keyword">open</a> <a id="27096" class="Keyword">import</a> <a id="27103" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="27139" class="Keyword">open</a> <a id="27144" class="Keyword">import</a> <a id="27151" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="27180" class="Keyword">open</a> <a id="27185" class="Keyword">import</a> <a id="27192" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="27220" class="Keyword">open</a> <a id="27225" class="Keyword">import</a> <a id="27232" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="27265" class="Keyword">open</a> <a id="27270" class="Keyword">import</a> <a id="27277" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="27313" class="Keyword">open</a> <a id="27318" class="Keyword">import</a> <a id="27325" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27354" class="Keyword">open</a> <a id="27359" class="Keyword">import</a> <a id="27366" href="group-theory.congruence-relations-groups.html" class="Module">group-theory.congruence-relations-groups</a>
<a id="27407" class="Keyword">open</a> <a id="27412" class="Keyword">import</a> <a id="27419" href="group-theory.congruence-relations-monoids.html" class="Module">group-theory.congruence-relations-monoids</a>
<a id="27461" class="Keyword">open</a> <a id="27466" class="Keyword">import</a> <a id="27473" href="group-theory.congruence-relations-semigroups.html" class="Module">group-theory.congruence-relations-semigroups</a>
<a id="27518" class="Keyword">open</a> <a id="27523" class="Keyword">import</a> <a id="27530" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27555" class="Keyword">open</a> <a id="27560" class="Keyword">import</a> <a id="27567" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27629" class="Keyword">open</a> <a id="27634" class="Keyword">import</a> <a id="27641" href="group-theory.decidable-subgroups.html" class="Module">group-theory.decidable-subgroups</a>
<a id="27674" class="Keyword">open</a> <a id="27679" class="Keyword">import</a> <a id="27686" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27727" class="Keyword">open</a> <a id="27732" class="Keyword">import</a> <a id="27739" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27768" class="Keyword">open</a> <a id="27773" class="Keyword">import</a> <a id="27780" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27804" class="Keyword">open</a> <a id="27809" class="Keyword">import</a> <a id="27816" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27847" class="Keyword">open</a> <a id="27852" class="Keyword">import</a> <a id="27859" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27906" class="Keyword">open</a> <a id="27911" class="Keyword">import</a> <a id="27918" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="27951" class="Keyword">open</a> <a id="27956" class="Keyword">import</a> <a id="27963" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="28012" class="Keyword">open</a> <a id="28017" class="Keyword">import</a> <a id="28024" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="28064" class="Keyword">open</a> <a id="28069" class="Keyword">import</a> <a id="28076" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="28116" class="Keyword">open</a> <a id="28121" class="Keyword">import</a> <a id="28128" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="28165" class="Keyword">open</a> <a id="28170" class="Keyword">import</a> <a id="28177" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="28224" class="Keyword">open</a> <a id="28229" class="Keyword">import</a> <a id="28236" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="28277" class="Keyword">open</a> <a id="28282" class="Keyword">import</a> <a id="28289" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="28333" class="Keyword">open</a> <a id="28338" class="Keyword">import</a> <a id="28345" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="28384" class="Keyword">open</a> <a id="28389" class="Keyword">import</a> <a id="28396" href="group-theory.full-subgroups.html" class="Module">group-theory.full-subgroups</a>
<a id="28424" class="Keyword">open</a> <a id="28429" class="Keyword">import</a> <a id="28436" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28468" class="Keyword">open</a> <a id="28473" class="Keyword">import</a> <a id="28480" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28507" class="Keyword">open</a> <a id="28512" class="Keyword">import</a> <a id="28519" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28539" class="Keyword">open</a> <a id="28544" class="Keyword">import</a> <a id="28551" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28585" class="Keyword">open</a> <a id="28590" class="Keyword">import</a> <a id="28597" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28624" class="Keyword">open</a> <a id="28629" class="Keyword">import</a> <a id="28636" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28678" class="Keyword">open</a> <a id="28683" class="Keyword">import</a> <a id="28690" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28740" class="Keyword">open</a> <a id="28745" class="Keyword">import</a> <a id="28752" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28799" class="Keyword">open</a> <a id="28804" class="Keyword">import</a> <a id="28811" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28852" class="Keyword">open</a> <a id="28857" class="Keyword">import</a> <a id="28864" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28898" class="Keyword">open</a> <a id="28903" class="Keyword">import</a> <a id="28910" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="28958" class="Keyword">open</a> <a id="28963" class="Keyword">import</a> <a id="28970" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="29011" class="Keyword">open</a> <a id="29016" class="Keyword">import</a> <a id="29023" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="29058" class="Keyword">open</a> <a id="29063" class="Keyword">import</a> <a id="29070" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="29108" class="Keyword">open</a> <a id="29113" class="Keyword">import</a> <a id="29120" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="29155" class="Keyword">open</a> <a id="29160" class="Keyword">import</a> <a id="29167" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="29199" class="Keyword">open</a> <a id="29204" class="Keyword">import</a> <a id="29211" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="29252" class="Keyword">open</a> <a id="29257" class="Keyword">import</a> <a id="29264" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="29305" class="Keyword">open</a> <a id="29310" class="Keyword">import</a> <a id="29317" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="29357" class="Keyword">open</a> <a id="29362" class="Keyword">import</a> <a id="29369" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="29402" class="Keyword">open</a> <a id="29407" class="Keyword">import</a> <a id="29414" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29451" class="Keyword">open</a> <a id="29456" class="Keyword">import</a> <a id="29463" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29493" class="Keyword">open</a> <a id="29498" class="Keyword">import</a> <a id="29505" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29526" class="Keyword">open</a> <a id="29531" class="Keyword">import</a> <a id="29538" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29592" class="Keyword">open</a> <a id="29597" class="Keyword">import</a> <a id="29604" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29649" class="Keyword">open</a> <a id="29654" class="Keyword">import</a> <a id="29661" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29689" class="Keyword">open</a> <a id="29694" class="Keyword">import</a> <a id="29701" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29722" class="Keyword">open</a> <a id="29727" class="Keyword">import</a> <a id="29734" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29777" class="Keyword">open</a> <a id="29782" class="Keyword">import</a> <a id="29789" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29823" class="Keyword">open</a> <a id="29828" class="Keyword">import</a> <a id="29835" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29865" class="Keyword">open</a> <a id="29870" class="Keyword">import</a> <a id="29877" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29923" class="Keyword">open</a> <a id="29928" class="Keyword">import</a> <a id="29935" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="29989" class="Keyword">open</a> <a id="29994" class="Keyword">import</a> <a id="30001" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="30044" class="Keyword">open</a> <a id="30049" class="Keyword">import</a> <a id="30056" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="30090" class="Keyword">open</a> <a id="30095" class="Keyword">import</a> <a id="30102" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="30143" class="Keyword">open</a> <a id="30148" class="Keyword">import</a> <a id="30155" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="30190" class="Keyword">open</a> <a id="30195" class="Keyword">import</a> <a id="30202" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a>
<a id="30241" class="Keyword">open</a> <a id="30246" class="Keyword">import</a> <a id="30253" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="30295" class="Keyword">open</a> <a id="30300" class="Keyword">import</a> <a id="30307" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="30342" class="Keyword">open</a> <a id="30347" class="Keyword">import</a> <a id="30354" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="30393" class="Keyword">open</a> <a id="30398" class="Keyword">import</a> <a id="30405" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="30442" class="Keyword">open</a> <a id="30447" class="Keyword">import</a> <a id="30454" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30501" class="Keyword">open</a> <a id="30506" class="Keyword">import</a> <a id="30513" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30577" class="Keyword">open</a> <a id="30582" class="Keyword">import</a> <a id="30589" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30634" class="Keyword">open</a> <a id="30639" class="Keyword">import</a> <a id="30646" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30670" class="Keyword">open</a> <a id="30675" class="Keyword">import</a> <a id="30682" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30707" class="Keyword">open</a> <a id="30712" class="Keyword">import</a> <a id="30719" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30762" class="Keyword">open</a> <a id="30767" class="Keyword">import</a> <a id="30774" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30805" class="Keyword">open</a> <a id="30810" class="Keyword">import</a> <a id="30817" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30871" class="Keyword">open</a> <a id="30876" class="Keyword">import</a> <a id="30883" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30906" class="Keyword">open</a> <a id="30911" class="Keyword">import</a> <a id="30918" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="30956" class="Keyword">open</a> <a id="30961" class="Keyword">import</a> <a id="30968" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="31007" class="Keyword">open</a> <a id="31012" class="Keyword">import</a> <a id="31019" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="31070" class="Keyword">open</a> <a id="31075" class="Keyword">import</a> <a id="31082" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="31119" class="Keyword">open</a> <a id="31124" class="Keyword">import</a> <a id="31131" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="31155" class="Keyword">open</a> <a id="31160" class="Keyword">import</a> <a id="31167" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="31194" class="Keyword">open</a> <a id="31199" class="Keyword">import</a> <a id="31206" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="31263" class="Keyword">open</a> <a id="31268" class="Keyword">import</a> <a id="31275" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="31323" class="Keyword">open</a> <a id="31328" class="Keyword">import</a> <a id="31335" href="group-theory.symmetric-concrete-groups.html" class="Module">group-theory.symmetric-concrete-groups</a>
<a id="31374" class="Keyword">open</a> <a id="31379" class="Keyword">import</a> <a id="31386" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="31416" class="Keyword">open</a> <a id="31421" class="Keyword">import</a> <a id="31428" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="31465" class="Keyword">open</a> <a id="31470" class="Keyword">import</a> <a id="31477" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="31498" class="Keyword">open</a> <a id="31503" class="Keyword">import</a> <a id="31510" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31557" class="Keyword">open</a> <a id="31562" class="Keyword">import</a> <a id="31569" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31607" class="Keyword">open</a> <a id="31612" class="Keyword">import</a> <a id="31619" href="group-theory.trivial-subgroups.html" class="Module">group-theory.trivial-subgroups</a>
<a id="31650" class="Keyword">open</a> <a id="31655" class="Keyword">import</a> <a id="31662" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31756" class="Keyword">open</a> <a id="31761" class="Keyword">import</a> <a id="31768" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31783" class="Keyword">open</a> <a id="31788" class="Keyword">import</a> <a id="31795" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31828" class="Keyword">open</a> <a id="31833" class="Keyword">import</a> <a id="31840" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="31872" class="Keyword">open</a> <a id="31877" class="Keyword">import</a> <a id="31884" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="31926" class="Keyword">open</a> <a id="31931" class="Keyword">import</a> <a id="31938" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="31976" class="Keyword">open</a> <a id="31981" class="Keyword">import</a> <a id="31988" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="32025" class="Keyword">open</a> <a id="32030" class="Keyword">import</a> <a id="32037" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="32070" class="Keyword">open</a> <a id="32075" class="Keyword">import</a> <a id="32082" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="32106" class="Keyword">open</a> <a id="32111" class="Keyword">import</a> <a id="32118" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="32157" class="Keyword">open</a> <a id="32162" class="Keyword">import</a> <a id="32169" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="32215" class="Keyword">open</a> <a id="32220" class="Keyword">import</a> <a id="32227" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="32272" class="Keyword">open</a> <a id="32277" class="Keyword">import</a> <a id="32284" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="32322" class="Keyword">open</a> <a id="32327" class="Keyword">import</a> <a id="32334" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="32366" class="Keyword">open</a> <a id="32371" class="Keyword">import</a> <a id="32378" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="32431" class="Keyword">open</a> <a id="32436" class="Keyword">import</a> <a id="32443" href="order-theory.html" class="Module">order-theory</a>
<a id="32456" class="Keyword">open</a> <a id="32461" class="Keyword">import</a> <a id="32468" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="32495" class="Keyword">open</a> <a id="32500" class="Keyword">import</a> <a id="32507" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="32537" class="Keyword">open</a> <a id="32542" class="Keyword">import</a> <a id="32549" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32582" class="Keyword">open</a> <a id="32587" class="Keyword">import</a> <a id="32594" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32630" class="Keyword">open</a> <a id="32635" class="Keyword">import</a> <a id="32642" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32677" class="Keyword">open</a> <a id="32682" class="Keyword">import</a> <a id="32689" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32716" class="Keyword">open</a> <a id="32721" class="Keyword">import</a> <a id="32728" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32758" class="Keyword">open</a> <a id="32763" class="Keyword">import</a> <a id="32770" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32806" class="Keyword">open</a> <a id="32811" class="Keyword">import</a> <a id="32818" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="32860" class="Keyword">open</a> <a id="32865" class="Keyword">import</a> <a id="32872" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32902" class="Keyword">open</a> <a id="32907" class="Keyword">import</a> <a id="32914" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="32946" class="Keyword">open</a> <a id="32951" class="Keyword">import</a> <a id="32958" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="32989" class="Keyword">open</a> <a id="32994" class="Keyword">import</a> <a id="33001" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="33027" class="Keyword">open</a> <a id="33032" class="Keyword">import</a> <a id="33039" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="33068" class="Keyword">open</a> <a id="33073" class="Keyword">import</a> <a id="33080" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="33117" class="Keyword">open</a> <a id="33122" class="Keyword">import</a> <a id="33129" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="33169" class="Keyword">open</a> <a id="33174" class="Keyword">import</a> <a id="33181" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="33203" class="Keyword">open</a> <a id="33208" class="Keyword">import</a> <a id="33215" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="33250" class="Keyword">open</a> <a id="33255" class="Keyword">import</a> <a id="33262" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="33300" class="Keyword">open</a> <a id="33305" class="Keyword">import</a> <a id="33312" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="33351" class="Keyword">open</a> <a id="33356" class="Keyword">import</a> <a id="33363" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="33398" class="Keyword">open</a> <a id="33403" class="Keyword">import</a> <a id="33410" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="33445" class="Keyword">open</a> <a id="33450" class="Keyword">import</a> <a id="33457" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="33492" class="Keyword">open</a> <a id="33497" class="Keyword">import</a> <a id="33504" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="33542" class="Keyword">open</a> <a id="33547" class="Keyword">import</a> <a id="33554" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33585" class="Keyword">open</a> <a id="33590" class="Keyword">import</a> <a id="33597" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33639" class="Keyword">open</a> <a id="33644" class="Keyword">import</a> <a id="33651" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33696" class="Keyword">open</a> <a id="33701" class="Keyword">import</a> <a id="33708" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33741" class="Keyword">open</a> <a id="33746" class="Keyword">import</a> <a id="33753" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33773" class="Keyword">open</a> <a id="33778" class="Keyword">import</a> <a id="33785" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33808" class="Keyword">open</a> <a id="33813" class="Keyword">import</a> <a id="33820" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="33843" class="Keyword">open</a> <a id="33848" class="Keyword">import</a> <a id="33855" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33881" class="Keyword">open</a> <a id="33886" class="Keyword">import</a> <a id="33893" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33919" class="Keyword">open</a> <a id="33924" class="Keyword">import</a> <a id="33931" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="33995" class="Keyword">open</a> <a id="34000" class="Keyword">import</a> <a id="34007" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="34025" class="Keyword">open</a> <a id="34030" class="Keyword">import</a> <a id="34037" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="34064" class="Keyword">open</a> <a id="34069" class="Keyword">import</a> <a id="34076" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="34102" class="Keyword">open</a> <a id="34107" class="Keyword">import</a> <a id="34114" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="34140" class="Keyword">open</a> <a id="34145" class="Keyword">import</a> <a id="34152" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="34178" class="Keyword">open</a> <a id="34183" class="Keyword">import</a> <a id="34190" href="organic-chemistry.ethane.html" class="Module">organic-chemistry.ethane</a>
<a id="34215" class="Keyword">open</a> <a id="34220" class="Keyword">import</a> <a id="34227" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="34258" class="Keyword">open</a> <a id="34263" class="Keyword">import</a> <a id="34270" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="34296" class="Keyword">open</a> <a id="34301" class="Keyword">import</a> <a id="34308" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="34371" class="Keyword">open</a> <a id="34376" class="Keyword">import</a> <a id="34383" href="polytopes.html" class="Module">polytopes</a>
<a id="34393" class="Keyword">open</a> <a id="34398" class="Keyword">import</a> <a id="34405" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="34463" class="Keyword">open</a> <a id="34468" class="Keyword">import</a> <a id="34475" href="ring-theory.html" class="Module">ring-theory</a>
<a id="34487" class="Keyword">open</a> <a id="34492" class="Keyword">import</a> <a id="34499" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="34536" class="Keyword">open</a> <a id="34541" class="Keyword">import</a> <a id="34548" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="34575" class="Keyword">open</a> <a id="34580" class="Keyword">import</a> <a id="34587" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34619" class="Keyword">open</a> <a id="34624" class="Keyword">import</a> <a id="34631" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34677" class="Keyword">open</a> <a id="34682" class="Keyword">import</a> <a id="34689" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34714" class="Keyword">open</a> <a id="34719" class="Keyword">import</a> <a id="34726" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34764" class="Keyword">open</a> <a id="34769" class="Keyword">import</a> <a id="34776" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34819" class="Keyword">open</a> <a id="34824" class="Keyword">import</a> <a id="34831" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="34869" class="Keyword">open</a> <a id="34874" class="Keyword">import</a> <a id="34881" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="34912" class="Keyword">open</a> <a id="34917" class="Keyword">import</a> <a id="34924" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="34948" class="Keyword">open</a> <a id="34953" class="Keyword">import</a> <a id="34960" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="34992" class="Keyword">open</a> <a id="34997" class="Keyword">import</a> <a id="35004" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="35030" class="Keyword">open</a> <a id="35035" class="Keyword">import</a> <a id="35042" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="35071" class="Keyword">open</a> <a id="35076" class="Keyword">import</a> <a id="35083" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="35120" class="Keyword">open</a> <a id="35125" class="Keyword">import</a> <a id="35132" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="35161" class="Keyword">open</a> <a id="35166" class="Keyword">import</a> <a id="35173" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="35200" class="Keyword">open</a> <a id="35205" class="Keyword">import</a> <a id="35212" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="35249" class="Keyword">open</a> <a id="35254" class="Keyword">import</a> <a id="35261" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="35288" class="Keyword">open</a> <a id="35293" class="Keyword">import</a> <a id="35300" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="35333" class="Keyword">open</a> <a id="35338" class="Keyword">import</a> <a id="35345" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="35363" class="Keyword">open</a> <a id="35368" class="Keyword">import</a> <a id="35375" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="35429" class="Keyword">open</a> <a id="35434" class="Keyword">import</a> <a id="35441" href="set-theory.html" class="Module">set-theory</a>
<a id="35452" class="Keyword">open</a> <a id="35457" class="Keyword">import</a> <a id="35464" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="35487" class="Keyword">open</a> <a id="35492" class="Keyword">import</a> <a id="35499" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="35523" class="Keyword">open</a> <a id="35528" class="Keyword">import</a> <a id="35535" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="35560" class="Keyword">open</a> <a id="35565" class="Keyword">import</a> <a id="35572" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="35598" class="Keyword">open</a> <a id="35603" class="Keyword">import</a> <a id="35610" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35672" class="Keyword">open</a> <a id="35677" class="Keyword">import</a> <a id="35684" href="structured-types.html" class="Module">structured-types</a>
<a id="35701" class="Keyword">open</a> <a id="35706" class="Keyword">import</a> <a id="35713" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35748" class="Keyword">open</a> <a id="35753" class="Keyword">import</a> <a id="35760" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35804" class="Keyword">open</a> <a id="35809" class="Keyword">import</a> <a id="35816" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="35880" class="Keyword">open</a> <a id="35885" class="Keyword">import</a> <a id="35892" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="35931" class="Keyword">open</a> <a id="35936" class="Keyword">import</a> <a id="35943" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="35989" class="Keyword">open</a> <a id="35994" class="Keyword">import</a> <a id="36001" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="36066" class="Keyword">open</a> <a id="36071" class="Keyword">import</a> <a id="36078" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="36102" class="Keyword">open</a> <a id="36107" class="Keyword">import</a> <a id="36114" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="36183" class="Keyword">open</a> <a id="36188" class="Keyword">import</a> <a id="36195" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="36240" class="Keyword">open</a> <a id="36245" class="Keyword">import</a> <a id="36252" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="36286" class="Keyword">open</a> <a id="36291" class="Keyword">import</a> <a id="36298" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="36359" class="Keyword">open</a> <a id="36364" class="Keyword">import</a> <a id="36371" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="36416" class="Keyword">open</a> <a id="36421" class="Keyword">import</a> <a id="36428" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="36466" class="Keyword">open</a> <a id="36471" class="Keyword">import</a> <a id="36478" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="36521" class="Keyword">open</a> <a id="36526" class="Keyword">import</a> <a id="36533" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="36569" class="Keyword">open</a> <a id="36574" class="Keyword">import</a> <a id="36581" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36611" class="Keyword">open</a> <a id="36616" class="Keyword">import</a> <a id="36623" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36657" class="Keyword">open</a> <a id="36662" class="Keyword">import</a> <a id="36669" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36700" class="Keyword">open</a> <a id="36705" class="Keyword">import</a> <a id="36712" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36771" class="Keyword">open</a> <a id="36776" class="Keyword">import</a> <a id="36783" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="36834" class="Keyword">open</a> <a id="36839" class="Keyword">import</a> <a id="36846" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="36897" class="Keyword">open</a> <a id="36902" class="Keyword">import</a> <a id="36909" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="36964" class="Keyword">open</a> <a id="36969" class="Keyword">import</a> <a id="36976" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="37008" class="Keyword">open</a> <a id="37013" class="Keyword">import</a> <a id="37020" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="37049" class="Keyword">open</a> <a id="37054" class="Keyword">import</a> <a id="37061" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="37089" class="Keyword">open</a> <a id="37094" class="Keyword">import</a> <a id="37101" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="37131" class="Keyword">open</a> <a id="37136" class="Keyword">import</a> <a id="37143" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="37177" class="Keyword">open</a> <a id="37182" class="Keyword">import</a> <a id="37189" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="37265" class="Keyword">open</a> <a id="37270" class="Keyword">import</a> <a id="37277" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="37303" class="Keyword">open</a> <a id="37308" class="Keyword">import</a> <a id="37315" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="37353" class="Keyword">open</a> <a id="37358" class="Keyword">import</a> <a id="37365" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="37402" class="Keyword">open</a> <a id="37407" class="Keyword">import</a> <a id="37414" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="37454" class="Keyword">open</a> <a id="37459" class="Keyword">import</a> <a id="37466" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="37505" class="Keyword">open</a> <a id="37510" class="Keyword">import</a> <a id="37517" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="37550" class="Keyword">open</a> <a id="37555" class="Keyword">import</a> <a id="37562" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="37605" class="Keyword">open</a> <a id="37610" class="Keyword">import</a> <a id="37617" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37652" class="Keyword">open</a> <a id="37657" class="Keyword">import</a> <a id="37664" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37709" class="Keyword">open</a> <a id="37714" class="Keyword">import</a> <a id="37721" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37758" class="Keyword">open</a> <a id="37763" class="Keyword">import</a> <a id="37770" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37822" class="Keyword">open</a> <a id="37827" class="Keyword">import</a> <a id="37834" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="37887" class="Keyword">open</a> <a id="37892" class="Keyword">import</a> <a id="37899" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="37959" class="Keyword">open</a> <a id="37964" class="Keyword">import</a> <a id="37971" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="38019" class="Keyword">open</a> <a id="38024" class="Keyword">import</a> <a id="38031" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="38071" class="Keyword">open</a> <a id="38076" class="Keyword">import</a> <a id="38083" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="38130" class="Keyword">open</a> <a id="38135" class="Keyword">import</a> <a id="38142" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="38183" class="Keyword">open</a> <a id="38188" class="Keyword">import</a> <a id="38195" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="38233" class="Keyword">open</a> <a id="38238" class="Keyword">import</a> <a id="38245" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="38293" class="Keyword">open</a> <a id="38298" class="Keyword">import</a> <a id="38305" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="38342" class="Keyword">open</a> <a id="38347" class="Keyword">import</a> <a id="38354" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="38389" class="Keyword">open</a> <a id="38394" class="Keyword">import</a> <a id="38401" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="38435" class="Keyword">open</a> <a id="38440" class="Keyword">import</a> <a id="38447" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="38494" class="Keyword">open</a> <a id="38499" class="Keyword">import</a> <a id="38506" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="38551" class="Keyword">open</a> <a id="38556" class="Keyword">import</a> <a id="38563" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38612" class="Keyword">open</a> <a id="38617" class="Keyword">import</a> <a id="38624" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38676" class="Keyword">open</a> <a id="38681" class="Keyword">import</a> <a id="38688" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38742" class="Keyword">open</a> <a id="38747" class="Keyword">import</a> <a id="38754" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Type theories

<pre class="Agda"><a id="38835" class="Keyword">open</a> <a id="38840" class="Keyword">import</a> <a id="38847" href="type-theories.html" class="Module">type-theories</a>
<a id="38861" class="Keyword">open</a> <a id="38866" class="Keyword">import</a> <a id="38873" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="38915" class="Keyword">open</a> <a id="38920" class="Keyword">import</a> <a id="38927" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="38965" class="Keyword">open</a> <a id="38970" class="Keyword">import</a> <a id="38977" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="39023" class="Keyword">open</a> <a id="39028" class="Keyword">import</a> <a id="39035" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="39082" class="Keyword">open</a> <a id="39087" class="Keyword">import</a> <a id="39094" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="39129" class="Keyword">open</a> <a id="39134" class="Keyword">import</a> <a id="39141" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="39219" class="Keyword">open</a> <a id="39224" class="Keyword">import</a> <a id="39231" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="39255" class="Keyword">open</a> <a id="39260" class="Keyword">import</a> <a id="39267" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="39320" class="Keyword">open</a> <a id="39325" class="Keyword">import</a> <a id="39332" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="39375" class="Keyword">open</a> <a id="39380" class="Keyword">import</a> <a id="39387" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="39427" class="Keyword">open</a> <a id="39432" class="Keyword">import</a> <a id="39439" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="39478" class="Keyword">open</a> <a id="39483" class="Keyword">import</a> <a id="39490" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="39524" class="Keyword">open</a> <a id="39529" class="Keyword">import</a> <a id="39536" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39584" class="Keyword">open</a> <a id="39589" class="Keyword">import</a> <a id="39596" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39647" class="Keyword">open</a> <a id="39652" class="Keyword">import</a> <a id="39659" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39706" class="Keyword">open</a> <a id="39711" class="Keyword">import</a> <a id="39718" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39770" class="Keyword">open</a> <a id="39775" class="Keyword">import</a> <a id="39782" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39826" class="Keyword">open</a> <a id="39831" class="Keyword">import</a> <a id="39838" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="39878" class="Keyword">open</a> <a id="39883" class="Keyword">import</a> <a id="39890" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="39933" class="Keyword">open</a> <a id="39938" class="Keyword">import</a> <a id="39945" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="39997" class="Keyword">open</a> <a id="40002" class="Keyword">import</a> <a id="40009" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="40063" class="Keyword">open</a> <a id="40068" class="Keyword">import</a> <a id="40075" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="40123" class="Keyword">open</a> <a id="40128" class="Keyword">import</a> <a id="40135" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="40174" class="Keyword">open</a> <a id="40179" class="Keyword">import</a> <a id="40186" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="40219" class="Keyword">open</a> <a id="40224" class="Keyword">import</a> <a id="40231" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="40261" class="Keyword">open</a> <a id="40266" class="Keyword">import</a> <a id="40273" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="40324" class="Keyword">open</a> <a id="40329" class="Keyword">import</a> <a id="40336" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="40377" class="Keyword">open</a> <a id="40382" class="Keyword">import</a> <a id="40389" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="40426" class="Keyword">open</a> <a id="40431" class="Keyword">import</a> <a id="40438" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="40497" class="Keyword">open</a> <a id="40502" class="Keyword">import</a> <a id="40509" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40564" class="Keyword">open</a> <a id="40569" class="Keyword">import</a> <a id="40576" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40632" class="Keyword">open</a> <a id="40637" class="Keyword">import</a> <a id="40644" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40691" class="Keyword">open</a> <a id="40696" class="Keyword">import</a> <a id="40703" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40746" class="Keyword">open</a> <a id="40751" class="Keyword">import</a> <a id="40758" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40803" class="Keyword">open</a> <a id="40808" class="Keyword">import</a> <a id="40815" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="40864" class="Keyword">open</a> <a id="40869" class="Keyword">import</a> <a id="40876" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="40927" class="Keyword">open</a> <a id="40932" class="Keyword">import</a> <a id="40939" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="40983" class="Keyword">open</a> <a id="40988" class="Keyword">import</a> <a id="40995" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="41073" class="Keyword">open</a> <a id="41078" class="Keyword">import</a> <a id="41085" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="41125" class="Keyword">open</a> <a id="41130" class="Keyword">import</a> <a id="41137" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="41194" class="Keyword">open</a> <a id="41199" class="Keyword">import</a> <a id="41206" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="41241" class="Keyword">open</a> <a id="41246" class="Keyword">import</a> <a id="41253" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="41299" class="Keyword">open</a> <a id="41304" class="Keyword">import</a> <a id="41311" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="41366" class="Keyword">open</a> <a id="41371" class="Keyword">import</a> <a id="41378" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="41421" class="Keyword">open</a> <a id="41426" class="Keyword">import</a> <a id="41433" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="41478" class="Keyword">open</a> <a id="41483" class="Keyword">import</a> <a id="41490" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41549" class="Keyword">open</a> <a id="41554" class="Keyword">import</a> <a id="41561" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41598" class="Keyword">open</a> <a id="41603" class="Keyword">import</a> <a id="41610" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41652" class="Keyword">open</a> <a id="41657" class="Keyword">import</a> <a id="41664" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41705" class="Keyword">open</a> <a id="41710" class="Keyword">import</a> <a id="41717" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41756" class="Keyword">open</a> <a id="41761" class="Keyword">import</a> <a id="41768" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41806" class="Keyword">open</a> <a id="41811" class="Keyword">import</a> <a id="41818" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="41870" class="Keyword">open</a> <a id="41875" class="Keyword">import</a> <a id="41882" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="41927" class="Keyword">open</a> <a id="41932" class="Keyword">import</a> <a id="41939" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="41978" class="Keyword">open</a> <a id="41983" class="Keyword">import</a> <a id="41990" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="42027" class="Keyword">open</a> <a id="42032" class="Keyword">import</a> <a id="42039" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="42088" class="Keyword">open</a> <a id="42093" class="Keyword">import</a> <a id="42100" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="42139" class="Keyword">open</a> <a id="42144" class="Keyword">import</a> <a id="42151" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="42189" class="Keyword">open</a> <a id="42194" class="Keyword">import</a> <a id="42201" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="42256" class="Keyword">open</a> <a id="42261" class="Keyword">import</a> <a id="42268" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="42307" class="Keyword">open</a> <a id="42312" class="Keyword">import</a> <a id="42319" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="42367" class="Keyword">open</a> <a id="42372" class="Keyword">import</a> <a id="42379" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="42426" class="Keyword">open</a> <a id="42431" class="Keyword">import</a> <a id="42438" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="42476" class="Keyword">open</a> <a id="42481" class="Keyword">import</a> <a id="42488" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="42518" class="Keyword">open</a> <a id="42523" class="Keyword">import</a> <a id="42530" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42587" class="Keyword">open</a> <a id="42592" class="Keyword">import</a> <a id="42599" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42653" class="Keyword">open</a> <a id="42658" class="Keyword">import</a> <a id="42665" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42695" class="Keyword">open</a> <a id="42700" class="Keyword">import</a> <a id="42707" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42756" class="Keyword">open</a> <a id="42761" class="Keyword">import</a> <a id="42768" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42810" class="Keyword">open</a> <a id="42815" class="Keyword">import</a> <a id="42822" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="42856" class="Keyword">open</a> <a id="42861" class="Keyword">import</a> <a id="42868" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="42931" class="Keyword">open</a> <a id="42936" class="Keyword">import</a> <a id="42943" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="42986" class="Keyword">open</a> <a id="42991" class="Keyword">import</a> <a id="42998" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="43033" class="Keyword">open</a> <a id="43038" class="Keyword">import</a> <a id="43045" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="43080" class="Keyword">open</a> <a id="43085" class="Keyword">import</a> <a id="43092" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="43132" class="Keyword">open</a> <a id="43137" class="Keyword">import</a> <a id="43144" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="43189" class="Keyword">open</a> <a id="43194" class="Keyword">import</a> <a id="43201" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="43242" class="Keyword">open</a> <a id="43247" class="Keyword">import</a> <a id="43254" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="43308" class="Keyword">open</a> <a id="43313" class="Keyword">import</a> <a id="43320" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="43370" class="Keyword">open</a> <a id="43375" class="Keyword">import</a> <a id="43382" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="43429" class="Keyword">open</a> <a id="43434" class="Keyword">import</a> <a id="43441" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="43479" class="Keyword">open</a> <a id="43484" class="Keyword">import</a> <a id="43491" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="43540" class="Keyword">open</a> <a id="43545" class="Keyword">import</a> <a id="43552" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43599" class="Keyword">open</a> <a id="43604" class="Keyword">import</a> <a id="43611" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43674" class="Keyword">open</a> <a id="43679" class="Keyword">import</a> <a id="43686" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43718" class="Keyword">open</a> <a id="43723" class="Keyword">import</a> <a id="43730" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43783" class="Keyword">open</a> <a id="43788" class="Keyword">import</a> <a id="43795" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="43841" class="Keyword">open</a> <a id="43846" class="Keyword">import</a> <a id="43853" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="43899" class="Keyword">open</a> <a id="43904" class="Keyword">import</a> <a id="43911" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="43951" class="Keyword">open</a> <a id="43956" class="Keyword">import</a> <a id="43963" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="44010" class="Keyword">open</a> <a id="44015" class="Keyword">import</a> <a id="44022" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="44070" class="Keyword">open</a> <a id="44075" class="Keyword">import</a> <a id="44082" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="44122" class="Keyword">open</a> <a id="44127" class="Keyword">import</a> <a id="44134" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="44179" class="Keyword">open</a> <a id="44184" class="Keyword">import</a> <a id="44191" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="44256" class="Keyword">open</a> <a id="44261" class="Keyword">import</a> <a id="44268" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="44313" class="Keyword">open</a> <a id="44318" class="Keyword">import</a> <a id="44325" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="44372" class="Keyword">open</a> <a id="44377" class="Keyword">import</a> <a id="44384" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="44437" class="Keyword">open</a> <a id="44442" class="Keyword">import</a> <a id="44449" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>