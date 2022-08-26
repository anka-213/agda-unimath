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
<a id="14081" class="Keyword">open</a> <a id="14086" class="Keyword">import</a> <a id="14093" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="14116" class="Keyword">open</a> <a id="14121" class="Keyword">import</a> <a id="14128" href="foundation.double-negation.html" class="Module">foundation.double-negation</a>
<a id="14155" class="Keyword">open</a> <a id="14160" class="Keyword">import</a> <a id="14167" href="foundation.double-powersets.html" class="Module">foundation.double-powersets</a>
<a id="14195" class="Keyword">open</a> <a id="14200" class="Keyword">import</a> <a id="14207" href="foundation.dubuc-penon-compact-types.html" class="Module">foundation.dubuc-penon-compact-types</a>
<a id="14244" class="Keyword">open</a> <a id="14249" class="Keyword">import</a> <a id="14256" href="foundation.effective-maps-equivalence-relations.html" class="Module">foundation.effective-maps-equivalence-relations</a>
<a id="14304" class="Keyword">open</a> <a id="14309" class="Keyword">import</a> <a id="14316" href="foundation.elementhood-relation-w-types.html" class="Module">foundation.elementhood-relation-w-types</a>
<a id="14356" class="Keyword">open</a> <a id="14361" class="Keyword">import</a> <a id="14368" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="14390" class="Keyword">open</a> <a id="14395" class="Keyword">import</a> <a id="14402" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="14425" class="Keyword">open</a> <a id="14430" class="Keyword">import</a> <a id="14437" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="14462" class="Keyword">open</a> <a id="14467" class="Keyword">import</a> <a id="14474" href="foundation.epimorphisms-with-respect-to-sets.html" class="Module">foundation.epimorphisms-with-respect-to-sets</a>
<a id="14519" class="Keyword">open</a> <a id="14524" class="Keyword">import</a> <a id="14531" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a>
<a id="14575" class="Keyword">open</a> <a id="14580" class="Keyword">import</a> <a id="14587" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="14623" class="Keyword">open</a> <a id="14628" class="Keyword">import</a> <a id="14635" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a>
<a id="14680" class="Keyword">open</a> <a id="14685" class="Keyword">import</a> <a id="14692" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="14733" class="Keyword">open</a> <a id="14738" class="Keyword">import</a> <a id="14745" href="foundation.equality-fibers-of-maps.html" class="Module">foundation.equality-fibers-of-maps</a>
<a id="14780" class="Keyword">open</a> <a id="14785" class="Keyword">import</a> <a id="14792" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a>
<a id="14824" class="Keyword">open</a> <a id="14829" class="Keyword">import</a> <a id="14836" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="14867" class="Keyword">open</a> <a id="14872" class="Keyword">import</a> <a id="14879" href="foundation.equivalence-induction.html" class="Module">foundation.equivalence-induction</a>
<a id="14912" class="Keyword">open</a> <a id="14917" class="Keyword">import</a> <a id="14924" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="14957" class="Keyword">open</a> <a id="14962" class="Keyword">import</a> <a id="14969" href="foundation.equivalences-maybe.html" class="Module">foundation.equivalences-maybe</a>
<a id="14999" class="Keyword">open</a> <a id="15004" class="Keyword">import</a> <a id="15011" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="15035" class="Keyword">open</a> <a id="15040" class="Keyword">import</a> <a id="15047" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="15085" class="Keyword">open</a> <a id="15090" class="Keyword">import</a> <a id="15097" href="foundation.extensional-w-types.html" class="Module">foundation.extensional-w-types</a>
<a id="15128" class="Keyword">open</a> <a id="15133" class="Keyword">import</a> <a id="15140" href="foundation.faithful-maps.html" class="Module">foundation.faithful-maps</a>
<a id="15165" class="Keyword">open</a> <a id="15170" class="Keyword">import</a> <a id="15177" href="foundation.fiber-inclusions.html" class="Module">foundation.fiber-inclusions</a>
<a id="15205" class="Keyword">open</a> <a id="15210" class="Keyword">import</a> <a id="15217" href="foundation.fibered-maps.html" class="Module">foundation.fibered-maps</a>
<a id="15241" class="Keyword">open</a> <a id="15246" class="Keyword">import</a> <a id="15253" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="15279" class="Keyword">open</a> <a id="15284" class="Keyword">import</a> <a id="15291" href="foundation.full-subtypes.html" class="Module">foundation.full-subtypes</a>
<a id="15316" class="Keyword">open</a> <a id="15321" class="Keyword">import</a> <a id="15328" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="15363" class="Keyword">open</a> <a id="15368" class="Keyword">import</a> <a id="15375" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="15396" class="Keyword">open</a> <a id="15401" class="Keyword">import</a> <a id="15408" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="15457" class="Keyword">open</a> <a id="15462" class="Keyword">import</a> <a id="15469" href="foundation.functoriality-coproduct-types.html" class="Module">foundation.functoriality-coproduct-types</a>
<a id="15510" class="Keyword">open</a> <a id="15515" class="Keyword">import</a> <a id="15522" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="15572" class="Keyword">open</a> <a id="15577" class="Keyword">import</a> <a id="15584" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="15630" class="Keyword">open</a> <a id="15635" class="Keyword">import</a> <a id="15642" href="foundation.functoriality-fibers-of-maps.html" class="Module">foundation.functoriality-fibers-of-maps</a>
<a id="15682" class="Keyword">open</a> <a id="15687" class="Keyword">import</a> <a id="15694" href="foundation.functoriality-function-types.html" class="Module">foundation.functoriality-function-types</a>
<a id="15734" class="Keyword">open</a> <a id="15739" class="Keyword">import</a> <a id="15746" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a>
<a id="15796" class="Keyword">open</a> <a id="15801" class="Keyword">import</a> <a id="15808" href="foundation.functoriality-set-quotients.html" class="Module">foundation.functoriality-set-quotients</a>
<a id="15847" class="Keyword">open</a> <a id="15852" class="Keyword">import</a> <a id="15859" href="foundation.functoriality-set-truncation.html" class="Module">foundation.functoriality-set-truncation</a>
<a id="15899" class="Keyword">open</a> <a id="15904" class="Keyword">import</a> <a id="15911" href="foundation.functoriality-w-types.html" class="Module">foundation.functoriality-w-types</a>
<a id="15944" class="Keyword">open</a> <a id="15949" class="Keyword">import</a> <a id="15956" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a>
<a id="16005" class="Keyword">open</a> <a id="16010" class="Keyword">import</a> <a id="16017" href="foundation.global-choice.html" class="Module">foundation.global-choice</a>
<a id="16042" class="Keyword">open</a> <a id="16047" class="Keyword">import</a> <a id="16054" href="foundation.hexagons-of-identifications.html" class="Module">foundation.hexagons-of-identifications</a>
<a id="16093" class="Keyword">open</a> <a id="16098" class="Keyword">import</a> <a id="16105" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a>
<a id="16143" class="Keyword">open</a> <a id="16148" class="Keyword">import</a> <a id="16155" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="16177" class="Keyword">open</a> <a id="16182" class="Keyword">import</a> <a id="16189" href="foundation.identity-systems.html" class="Module">foundation.identity-systems</a>
<a id="16217" class="Keyword">open</a> <a id="16222" class="Keyword">import</a> <a id="16229" href="foundation.identity-truncated-types.html" class="Module">foundation.identity-truncated-types</a>
<a id="16265" class="Keyword">open</a> <a id="16270" class="Keyword">import</a> <a id="16277" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="16303" class="Keyword">open</a> <a id="16308" class="Keyword">import</a> <a id="16315" href="foundation.images.html" class="Module">foundation.images</a>
<a id="16333" class="Keyword">open</a> <a id="16338" class="Keyword">import</a> <a id="16345" href="foundation.impredicative-encodings.html" class="Module">foundation.impredicative-encodings</a>
<a id="16380" class="Keyword">open</a> <a id="16385" class="Keyword">import</a> <a id="16392" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a>
<a id="16427" class="Keyword">open</a> <a id="16432" class="Keyword">import</a> <a id="16439" href="foundation.indexed-w-types.html" class="Module">foundation.indexed-w-types</a>
<a id="16466" class="Keyword">open</a> <a id="16471" class="Keyword">import</a> <a id="16478" href="foundation.induction-principle-propositional-truncation.html" class="Module">foundation.induction-principle-propositional-truncation</a>
<a id="16534" class="Keyword">open</a> <a id="16539" class="Keyword">import</a> <a id="16546" href="foundation.induction-w-types.html" class="Module">foundation.induction-w-types</a>
<a id="16575" class="Keyword">open</a> <a id="16580" class="Keyword">import</a> <a id="16587" href="foundation.inequality-w-types.html" class="Module">foundation.inequality-w-types</a>
<a id="16617" class="Keyword">open</a> <a id="16622" class="Keyword">import</a> <a id="16629" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a>
<a id="16656" class="Keyword">open</a> <a id="16661" class="Keyword">import</a> <a id="16668" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="16694" class="Keyword">open</a> <a id="16699" class="Keyword">import</a> <a id="16706" href="foundation.interchange-law.html" class="Module">foundation.interchange-law</a>
<a id="16733" class="Keyword">open</a> <a id="16738" class="Keyword">import</a> <a id="16745" href="foundation.intersection.html" class="Module">foundation.intersection</a>
<a id="16769" class="Keyword">open</a> <a id="16774" class="Keyword">import</a> <a id="16781" href="foundation.involutions.html" class="Module">foundation.involutions</a>
<a id="16804" class="Keyword">open</a> <a id="16809" class="Keyword">import</a> <a id="16816" href="foundation.isolated-points.html" class="Module">foundation.isolated-points</a>
<a id="16843" class="Keyword">open</a> <a id="16848" class="Keyword">import</a> <a id="16855" href="foundation.isomorphisms-of-sets.html" class="Module">foundation.isomorphisms-of-sets</a>
<a id="16887" class="Keyword">open</a> <a id="16892" class="Keyword">import</a> <a id="16899" href="foundation.iterating-automorphisms.html" class="Module">foundation.iterating-automorphisms</a>
<a id="16934" class="Keyword">open</a> <a id="16939" class="Keyword">import</a> <a id="16946" href="foundation.iterating-functions.html" class="Module">foundation.iterating-functions</a>
<a id="16977" class="Keyword">open</a> <a id="16982" class="Keyword">import</a> <a id="16989" href="foundation.iterating-involutions.html" class="Module">foundation.iterating-involutions</a>
<a id="17022" class="Keyword">open</a> <a id="17027" class="Keyword">import</a> <a id="17034" href="foundation.law-of-excluded-middle.html" class="Module">foundation.law-of-excluded-middle</a>
<a id="17068" class="Keyword">open</a> <a id="17073" class="Keyword">import</a> <a id="17080" href="foundation.lawveres-fixed-point-theorem.html" class="Module">foundation.lawveres-fixed-point-theorem</a>
<a id="17120" class="Keyword">open</a> <a id="17125" class="Keyword">import</a> <a id="17132" href="foundation.lesser-limited-principle-of-omniscience.html" class="Module">foundation.lesser-limited-principle-of-omniscience</a>
<a id="17183" class="Keyword">open</a> <a id="17188" class="Keyword">import</a> <a id="17195" href="foundation.limited-principle-of-omniscience.html" class="Module">foundation.limited-principle-of-omniscience</a>
<a id="17239" class="Keyword">open</a> <a id="17244" class="Keyword">import</a> <a id="17251" href="foundation.locally-small-types.html" class="Module">foundation.locally-small-types</a>
<a id="17282" class="Keyword">open</a> <a id="17287" class="Keyword">import</a> <a id="17294" href="foundation.logical-equivalences.html" class="Module">foundation.logical-equivalences</a>
<a id="17326" class="Keyword">open</a> <a id="17331" class="Keyword">import</a> <a id="17338" href="foundation.lower-types-w-types.html" class="Module">foundation.lower-types-w-types</a>
<a id="17369" class="Keyword">open</a> <a id="17374" class="Keyword">import</a> <a id="17381" href="foundation.maybe.html" class="Module">foundation.maybe</a>
<a id="17398" class="Keyword">open</a> <a id="17403" class="Keyword">import</a> <a id="17410" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="17435" class="Keyword">open</a> <a id="17440" class="Keyword">import</a> <a id="17447" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="17476" class="Keyword">open</a> <a id="17481" class="Keyword">import</a> <a id="17488" href="foundation.monomorphisms.html" class="Module">foundation.monomorphisms</a>
<a id="17513" class="Keyword">open</a> <a id="17518" class="Keyword">import</a> <a id="17525" href="foundation.morphisms-cospans.html" class="Module">foundation.morphisms-cospans</a>
<a id="17554" class="Keyword">open</a> <a id="17559" class="Keyword">import</a> <a id="17566" href="foundation.multisets.html" class="Module">foundation.multisets</a>
<a id="17587" class="Keyword">open</a> <a id="17592" class="Keyword">import</a> <a id="17599" href="foundation.multisubsets.html" class="Module">foundation.multisubsets</a>
<a id="17623" class="Keyword">open</a> <a id="17628" class="Keyword">import</a> <a id="17635" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="17655" class="Keyword">open</a> <a id="17660" class="Keyword">import</a> <a id="17667" href="foundation.noncontractible-types.html" class="Module">foundation.noncontractible-types</a>
<a id="17700" class="Keyword">open</a> <a id="17705" class="Keyword">import</a> <a id="17712" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="17750" class="Keyword">open</a> <a id="17755" class="Keyword">import</a> <a id="17762" href="foundation.partial-elements.html" class="Module">foundation.partial-elements</a>
<a id="17790" class="Keyword">open</a> <a id="17795" class="Keyword">import</a> <a id="17802" href="foundation.path-algebra.html" class="Module">foundation.path-algebra</a>
<a id="17826" class="Keyword">open</a> <a id="17831" class="Keyword">import</a> <a id="17838" href="foundation.path-split-maps.html" class="Module">foundation.path-split-maps</a>
<a id="17865" class="Keyword">open</a> <a id="17870" class="Keyword">import</a> <a id="17877" href="foundation.polynomial-endofunctors.html" class="Module">foundation.polynomial-endofunctors</a>
<a id="17912" class="Keyword">open</a> <a id="17917" class="Keyword">import</a> <a id="17924" href="foundation.powersets.html" class="Module">foundation.powersets</a>
<a id="17945" class="Keyword">open</a> <a id="17950" class="Keyword">import</a> <a id="17957" href="foundation.principle-of-omniscience.html" class="Module">foundation.principle-of-omniscience</a>
<a id="17993" class="Keyword">open</a> <a id="17998" class="Keyword">import</a> <a id="18005" href="foundation.products-unordered-pairs-of-types.html" class="Module">foundation.products-unordered-pairs-of-types</a>
<a id="18050" class="Keyword">open</a> <a id="18055" class="Keyword">import</a> <a id="18062" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a>
<a id="18108" class="Keyword">open</a> <a id="18113" class="Keyword">import</a> <a id="18120" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a>
<a id="18160" class="Keyword">open</a> <a id="18165" class="Keyword">import</a> <a id="18172" href="foundation.propositional-maps.html" class="Module">foundation.propositional-maps</a>
<a id="18202" class="Keyword">open</a> <a id="18207" class="Keyword">import</a> <a id="18214" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a>
<a id="18248" class="Keyword">open</a> <a id="18253" class="Keyword">import</a> <a id="18260" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="18297" class="Keyword">open</a> <a id="18302" class="Keyword">import</a> <a id="18309" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="18333" class="Keyword">open</a> <a id="18338" class="Keyword">import</a> <a id="18345" href="foundation.pullbacks.html" class="Module">foundation.pullbacks</a>
<a id="18366" class="Keyword">open</a> <a id="18371" class="Keyword">import</a> <a id="18378" href="foundation.raising-universe-levels.html" class="Module">foundation.raising-universe-levels</a>
<a id="18413" class="Keyword">open</a> <a id="18418" class="Keyword">import</a> <a id="18425" href="foundation.ranks-of-elements-w-types.html" class="Module">foundation.ranks-of-elements-w-types</a>
<a id="18462" class="Keyword">open</a> <a id="18467" class="Keyword">import</a> <a id="18474" href="foundation.reflecting-maps-equivalence-relations.html" class="Module">foundation.reflecting-maps-equivalence-relations</a>
<a id="18523" class="Keyword">open</a> <a id="18528" class="Keyword">import</a> <a id="18535" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a>
<a id="18568" class="Keyword">open</a> <a id="18573" class="Keyword">import</a> <a id="18580" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="18603" class="Keyword">open</a> <a id="18608" class="Keyword">import</a> <a id="18615" href="foundation.replacement.html" class="Module">foundation.replacement</a>
<a id="18638" class="Keyword">open</a> <a id="18643" class="Keyword">import</a> <a id="18650" href="foundation.retractions.html" class="Module">foundation.retractions</a>
<a id="18673" class="Keyword">open</a> <a id="18678" class="Keyword">import</a> <a id="18685" href="foundation.russells-paradox.html" class="Module">foundation.russells-paradox</a>
<a id="18713" class="Keyword">open</a> <a id="18718" class="Keyword">import</a> <a id="18725" href="foundation.sections.html" class="Module">foundation.sections</a>
<a id="18745" class="Keyword">open</a> <a id="18750" class="Keyword">import</a> <a id="18757" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="18778" class="Keyword">open</a> <a id="18783" class="Keyword">import</a> <a id="18790" href="foundation.set-presented-types.html" class="Module">foundation.set-presented-types</a>
<a id="18821" class="Keyword">open</a> <a id="18826" class="Keyword">import</a> <a id="18833" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="18860" class="Keyword">open</a> <a id="18865" class="Keyword">import</a> <a id="18872" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="18888" class="Keyword">open</a> <a id="18893" class="Keyword">import</a> <a id="18900" href="foundation.sigma-decompositions.html" class="Module">foundation.sigma-decompositions</a>
<a id="18932" class="Keyword">open</a> <a id="18937" class="Keyword">import</a> <a id="18944" href="foundation.singleton-induction.html" class="Module">foundation.singleton-induction</a>
<a id="18975" class="Keyword">open</a> <a id="18980" class="Keyword">import</a> <a id="18987" href="foundation.slice.html" class="Module">foundation.slice</a>
<a id="19004" class="Keyword">open</a> <a id="19009" class="Keyword">import</a> <a id="19016" href="foundation.small-maps.html" class="Module">foundation.small-maps</a>
<a id="19038" class="Keyword">open</a> <a id="19043" class="Keyword">import</a> <a id="19050" href="foundation.small-multisets.html" class="Module">foundation.small-multisets</a>
<a id="19077" class="Keyword">open</a> <a id="19082" class="Keyword">import</a> <a id="19089" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="19112" class="Keyword">open</a> <a id="19117" class="Keyword">import</a> <a id="19124" href="foundation.small-universes.html" class="Module">foundation.small-universes</a>
<a id="19151" class="Keyword">open</a> <a id="19156" class="Keyword">import</a> <a id="19163" href="foundation.split-surjective-maps.html" class="Module">foundation.split-surjective-maps</a>
<a id="19196" class="Keyword">open</a> <a id="19201" class="Keyword">import</a> <a id="19208" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a>
<a id="19248" class="Keyword">open</a> <a id="19253" class="Keyword">import</a> <a id="19260" href="foundation.structure.html" class="Module">foundation.structure</a>
<a id="19281" class="Keyword">open</a> <a id="19286" class="Keyword">import</a> <a id="19293" href="foundation.subterminal-types.html" class="Module">foundation.subterminal-types</a>
<a id="19322" class="Keyword">open</a> <a id="19327" class="Keyword">import</a> <a id="19334" href="foundation.subtype-identity-principle.html" class="Module">foundation.subtype-identity-principle</a>
<a id="19372" class="Keyword">open</a> <a id="19377" class="Keyword">import</a> <a id="19384" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="19404" class="Keyword">open</a> <a id="19409" class="Keyword">import</a> <a id="19416" href="foundation.subuniverses.html" class="Module">foundation.subuniverses</a>
<a id="19440" class="Keyword">open</a> <a id="19445" class="Keyword">import</a> <a id="19452" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="19479" class="Keyword">open</a> <a id="19484" class="Keyword">import</a> <a id="19491" href="foundation.symmetric-difference.html" class="Module">foundation.symmetric-difference</a>
<a id="19523" class="Keyword">open</a> <a id="19528" class="Keyword">import</a> <a id="19535" href="foundation.truncated-equality.html" class="Module">foundation.truncated-equality</a>
<a id="19565" class="Keyword">open</a> <a id="19570" class="Keyword">import</a> <a id="19577" href="foundation.truncated-maps.html" class="Module">foundation.truncated-maps</a>
<a id="19603" class="Keyword">open</a> <a id="19608" class="Keyword">import</a> <a id="19615" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="19642" class="Keyword">open</a> <a id="19647" class="Keyword">import</a> <a id="19654" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="19691" class="Keyword">open</a> <a id="19696" class="Keyword">import</a> <a id="19703" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="19732" class="Keyword">open</a> <a id="19737" class="Keyword">import</a> <a id="19744" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="19767" class="Keyword">open</a> <a id="19772" class="Keyword">import</a> <a id="19779" href="foundation.type-arithmetic-booleans.html" class="Module">foundation.type-arithmetic-booleans</a>
<a id="19815" class="Keyword">open</a> <a id="19820" class="Keyword">import</a> <a id="19827" href="foundation.type-arithmetic-cartesian-product-types.html" class="Module">foundation.type-arithmetic-cartesian-product-types</a>
<a id="19878" class="Keyword">open</a> <a id="19883" class="Keyword">import</a> <a id="19890" href="foundation.type-arithmetic-coproduct-types.html" class="Module">foundation.type-arithmetic-coproduct-types</a>
<a id="19933" class="Keyword">open</a> <a id="19938" class="Keyword">import</a> <a id="19945" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="19997" class="Keyword">open</a> <a id="20002" class="Keyword">import</a> <a id="20009" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a>
<a id="20057" class="Keyword">open</a> <a id="20062" class="Keyword">import</a> <a id="20069" href="foundation.type-arithmetic-empty-type.html" class="Module">foundation.type-arithmetic-empty-type</a>
<a id="20107" class="Keyword">open</a> <a id="20112" class="Keyword">import</a> <a id="20119" href="foundation.type-arithmetic-unit-type.html" class="Module">foundation.type-arithmetic-unit-type</a>
<a id="20156" class="Keyword">open</a> <a id="20161" class="Keyword">import</a> <a id="20168" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="20214" class="Keyword">open</a> <a id="20219" class="Keyword">import</a> <a id="20226" href="foundation.union.html" class="Module">foundation.union</a>
<a id="20243" class="Keyword">open</a> <a id="20248" class="Keyword">import</a> <a id="20255" href="foundation.unique-existence.html" class="Module">foundation.unique-existence</a>
<a id="20283" class="Keyword">open</a> <a id="20288" class="Keyword">import</a> <a id="20295" href="foundation.uniqueness-image.html" class="Module">foundation.uniqueness-image</a>
<a id="20323" class="Keyword">open</a> <a id="20328" class="Keyword">import</a> <a id="20335" href="foundation.uniqueness-set-quotients.html" class="Module">foundation.uniqueness-set-quotients</a>
<a id="20371" class="Keyword">open</a> <a id="20376" class="Keyword">import</a> <a id="20383" href="foundation.uniqueness-set-truncations.html" class="Module">foundation.uniqueness-set-truncations</a>
<a id="20421" class="Keyword">open</a> <a id="20426" class="Keyword">import</a> <a id="20433" href="foundation.uniqueness-truncation.html" class="Module">foundation.uniqueness-truncation</a>
<a id="20466" class="Keyword">open</a> <a id="20471" class="Keyword">import</a> <a id="20478" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="20499" class="Keyword">open</a> <a id="20504" class="Keyword">import</a> <a id="20511" href="foundation.unital-binary-operations.html" class="Module">foundation.unital-binary-operations</a>
<a id="20547" class="Keyword">open</a> <a id="20552" class="Keyword">import</a> <a id="20559" href="foundation.univalence-implies-function-extensionality.html" class="Module">foundation.univalence-implies-function-extensionality</a>
<a id="20613" class="Keyword">open</a> <a id="20618" class="Keyword">import</a> <a id="20625" href="foundation.univalence.html" class="Module">foundation.univalence</a>
<a id="20647" class="Keyword">open</a> <a id="20652" class="Keyword">import</a> <a id="20659" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a>
<a id="20694" class="Keyword">open</a> <a id="20699" class="Keyword">import</a> <a id="20706" href="foundation.universal-multiset.html" class="Module">foundation.universal-multiset</a>
<a id="20736" class="Keyword">open</a> <a id="20741" class="Keyword">import</a> <a id="20748" href="foundation.universal-property-booleans.html" class="Module">foundation.universal-property-booleans</a>
<a id="20787" class="Keyword">open</a> <a id="20792" class="Keyword">import</a> <a id="20799" href="foundation.universal-property-cartesian-product-types.html" class="Module">foundation.universal-property-cartesian-product-types</a>
<a id="20853" class="Keyword">open</a> <a id="20858" class="Keyword">import</a> <a id="20865" href="foundation.universal-property-coproduct-types.html" class="Module">foundation.universal-property-coproduct-types</a>
<a id="20911" class="Keyword">open</a> <a id="20916" class="Keyword">import</a> <a id="20923" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="20974" class="Keyword">open</a> <a id="20979" class="Keyword">import</a> <a id="20986" href="foundation.universal-property-empty-type.html" class="Module">foundation.universal-property-empty-type</a>
<a id="21027" class="Keyword">open</a> <a id="21032" class="Keyword">import</a> <a id="21039" href="foundation.universal-property-fiber-products.html" class="Module">foundation.universal-property-fiber-products</a>
<a id="21084" class="Keyword">open</a> <a id="21089" class="Keyword">import</a> <a id="21096" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="21141" class="Keyword">open</a> <a id="21146" class="Keyword">import</a> <a id="21153" href="foundation.universal-property-image.html" class="Module">foundation.universal-property-image</a>
<a id="21189" class="Keyword">open</a> <a id="21194" class="Keyword">import</a> <a id="21201" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="21237" class="Keyword">open</a> <a id="21242" class="Keyword">import</a> <a id="21249" href="foundation.universal-property-propositional-truncation-into-sets.html" class="Module">foundation.universal-property-propositional-truncation-into-sets</a>
<a id="21314" class="Keyword">open</a> <a id="21319" class="Keyword">import</a> <a id="21326" href="foundation.universal-property-propositional-truncation.html" class="Module">foundation.universal-property-propositional-truncation</a>
<a id="21381" class="Keyword">open</a> <a id="21386" class="Keyword">import</a> <a id="21393" href="foundation.universal-property-pullbacks.html" class="Module">foundation.universal-property-pullbacks</a>
<a id="21433" class="Keyword">open</a> <a id="21438" class="Keyword">import</a> <a id="21445" href="foundation.universal-property-set-quotients.html" class="Module">foundation.universal-property-set-quotients</a>
<a id="21489" class="Keyword">open</a> <a id="21494" class="Keyword">import</a> <a id="21501" href="foundation.universal-property-set-truncation.html" class="Module">foundation.universal-property-set-truncation</a>
<a id="21546" class="Keyword">open</a> <a id="21551" class="Keyword">import</a> <a id="21558" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a>
<a id="21599" class="Keyword">open</a> <a id="21604" class="Keyword">import</a> <a id="21611" href="foundation.universal-property-unit-type.html" class="Module">foundation.universal-property-unit-type</a>
<a id="21651" class="Keyword">open</a> <a id="21656" class="Keyword">import</a> <a id="21663" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="21690" class="Keyword">open</a> <a id="21695" class="Keyword">import</a> <a id="21702" href="foundation.unordered-pairs-of-types.html" class="Module">foundation.unordered-pairs-of-types</a>
<a id="21738" class="Keyword">open</a> <a id="21743" class="Keyword">import</a> <a id="21750" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>
<a id="21777" class="Keyword">open</a> <a id="21782" class="Keyword">import</a> <a id="21789" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>
<a id="21826" class="Keyword">open</a> <a id="21831" class="Keyword">import</a> <a id="21838" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="21866" class="Keyword">open</a> <a id="21871" class="Keyword">import</a> <a id="21878" href="foundation.w-types.html" class="Module">foundation.w-types</a>
<a id="21897" class="Keyword">open</a> <a id="21902" class="Keyword">import</a> <a id="21909" href="foundation.weak-function-extensionality.html" class="Module">foundation.weak-function-extensionality</a>
<a id="21949" class="Keyword">open</a> <a id="21954" class="Keyword">import</a> <a id="21961" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a>
<a id="22010" class="Keyword">open</a> <a id="22015" class="Keyword">import</a> <a id="22022" href="foundation.weakly-constant-maps.html" class="Module">foundation.weakly-constant-maps</a>
<a id="22054" class="Keyword">open</a> <a id="22059" class="Keyword">import</a> <a id="22066" href="foundation.xor.html" class="Module">foundation.xor</a>
</pre>
## Foundation Core

<pre class="Agda"><a id="22114" class="Keyword">open</a> <a id="22119" class="Keyword">import</a> <a id="22126" href="foundation-core.0-maps.html" class="Module">foundation-core.0-maps</a>
<a id="22149" class="Keyword">open</a> <a id="22154" class="Keyword">import</a> <a id="22161" href="foundation-core.1-types.html" class="Module">foundation-core.1-types</a>
<a id="22185" class="Keyword">open</a> <a id="22190" class="Keyword">import</a> <a id="22197" href="foundation-core.automorphisms.html" class="Module">foundation-core.automorphisms</a>
<a id="22227" class="Keyword">open</a> <a id="22232" class="Keyword">import</a> <a id="22239" href="foundation-core.cartesian-product-types.html" class="Module">foundation-core.cartesian-product-types</a>
<a id="22279" class="Keyword">open</a> <a id="22284" class="Keyword">import</a> <a id="22291" href="foundation-core.coherently-invertible-maps.html" class="Module">foundation-core.coherently-invertible-maps</a>
<a id="22334" class="Keyword">open</a> <a id="22339" class="Keyword">import</a> <a id="22346" href="foundation-core.commuting-squares.html" class="Module">foundation-core.commuting-squares</a>
<a id="22380" class="Keyword">open</a> <a id="22385" class="Keyword">import</a> <a id="22392" href="foundation-core.cones-pullbacks.html" class="Module">foundation-core.cones-pullbacks</a>
<a id="22424" class="Keyword">open</a> <a id="22429" class="Keyword">import</a> <a id="22436" href="foundation-core.constant-maps.html" class="Module">foundation-core.constant-maps</a>
<a id="22466" class="Keyword">open</a> <a id="22471" class="Keyword">import</a> <a id="22478" href="foundation-core.contractible-maps.html" class="Module">foundation-core.contractible-maps</a>
<a id="22512" class="Keyword">open</a> <a id="22517" class="Keyword">import</a> <a id="22524" href="foundation-core.contractible-types.html" class="Module">foundation-core.contractible-types</a>
<a id="22559" class="Keyword">open</a> <a id="22564" class="Keyword">import</a> <a id="22571" href="foundation-core.cospans.html" class="Module">foundation-core.cospans</a>
<a id="22595" class="Keyword">open</a> <a id="22600" class="Keyword">import</a> <a id="22607" href="foundation-core.dependent-pair-types.html" class="Module">foundation-core.dependent-pair-types</a>
<a id="22644" class="Keyword">open</a> <a id="22649" class="Keyword">import</a> <a id="22656" href="foundation-core.embeddings.html" class="Module">foundation-core.embeddings</a>
<a id="22683" class="Keyword">open</a> <a id="22688" class="Keyword">import</a> <a id="22695" href="foundation-core.empty-types.html" class="Module">foundation-core.empty-types</a>
<a id="22723" class="Keyword">open</a> <a id="22728" class="Keyword">import</a> <a id="22735" href="foundation-core.endomorphisms.html" class="Module">foundation-core.endomorphisms</a>
<a id="22765" class="Keyword">open</a> <a id="22770" class="Keyword">import</a> <a id="22777" href="foundation-core.equality-cartesian-product-types.html" class="Module">foundation-core.equality-cartesian-product-types</a>
<a id="22826" class="Keyword">open</a> <a id="22831" class="Keyword">import</a> <a id="22838" href="foundation-core.equality-dependent-pair-types.html" class="Module">foundation-core.equality-dependent-pair-types</a>
<a id="22884" class="Keyword">open</a> <a id="22889" class="Keyword">import</a> <a id="22896" href="foundation-core.equality-fibers-of-maps.html" class="Module">foundation-core.equality-fibers-of-maps</a>
<a id="22936" class="Keyword">open</a> <a id="22941" class="Keyword">import</a> <a id="22948" href="foundation-core.equivalence-induction.html" class="Module">foundation-core.equivalence-induction</a>
<a id="22986" class="Keyword">open</a> <a id="22991" class="Keyword">import</a> <a id="22998" href="foundation-core.equivalences.html" class="Module">foundation-core.equivalences</a>
<a id="23027" class="Keyword">open</a> <a id="23032" class="Keyword">import</a> <a id="23039" href="foundation-core.faithful-maps.html" class="Module">foundation-core.faithful-maps</a>
<a id="23069" class="Keyword">open</a> <a id="23074" class="Keyword">import</a> <a id="23081" href="foundation-core.fibers-of-maps.html" class="Module">foundation-core.fibers-of-maps</a>
<a id="23112" class="Keyword">open</a> <a id="23117" class="Keyword">import</a> <a id="23124" href="foundation-core.function-extensionality.html" class="Module">foundation-core.function-extensionality</a>
<a id="23164" class="Keyword">open</a> <a id="23169" class="Keyword">import</a> <a id="23176" href="foundation-core.functions.html" class="Module">foundation-core.functions</a>
<a id="23202" class="Keyword">open</a> <a id="23207" class="Keyword">import</a> <a id="23214" href="foundation-core.functoriality-dependent-function-types.html" class="Module">foundation-core.functoriality-dependent-function-types</a>
<a id="23269" class="Keyword">open</a> <a id="23274" class="Keyword">import</a> <a id="23281" href="foundation-core.functoriality-dependent-pair-types.html" class="Module">foundation-core.functoriality-dependent-pair-types</a>
<a id="23332" class="Keyword">open</a> <a id="23337" class="Keyword">import</a> <a id="23344" href="foundation-core.functoriality-fibers-of-maps.html" class="Module">foundation-core.functoriality-fibers-of-maps</a>
<a id="23389" class="Keyword">open</a> <a id="23394" class="Keyword">import</a> <a id="23401" href="foundation-core.functoriality-function-types.html" class="Module">foundation-core.functoriality-function-types</a>
<a id="23446" class="Keyword">open</a> <a id="23451" class="Keyword">import</a> <a id="23458" href="foundation-core.fundamental-theorem-of-identity-types.html" class="Module">foundation-core.fundamental-theorem-of-identity-types</a>
<a id="23512" class="Keyword">open</a> <a id="23517" class="Keyword">import</a> <a id="23524" href="foundation-core.homotopies.html" class="Module">foundation-core.homotopies</a>
<a id="23551" class="Keyword">open</a> <a id="23556" class="Keyword">import</a> <a id="23563" href="foundation-core.identity-systems.html" class="Module">foundation-core.identity-systems</a>
<a id="23596" class="Keyword">open</a> <a id="23601" class="Keyword">import</a> <a id="23608" href="foundation-core.identity-types.html" class="Module">foundation-core.identity-types</a>
<a id="23639" class="Keyword">open</a> <a id="23644" class="Keyword">import</a> <a id="23651" href="foundation-core.logical-equivalences.html" class="Module">foundation-core.logical-equivalences</a>
<a id="23688" class="Keyword">open</a> <a id="23693" class="Keyword">import</a> <a id="23700" href="foundation-core.morphisms-cospans.html" class="Module">foundation-core.morphisms-cospans</a>
<a id="23734" class="Keyword">open</a> <a id="23739" class="Keyword">import</a> <a id="23746" href="foundation-core.negation.html" class="Module">foundation-core.negation</a>
<a id="23771" class="Keyword">open</a> <a id="23776" class="Keyword">import</a> <a id="23783" href="foundation-core.path-split-maps.html" class="Module">foundation-core.path-split-maps</a>
<a id="23815" class="Keyword">open</a> <a id="23820" class="Keyword">import</a> <a id="23827" href="foundation-core.propositional-maps.html" class="Module">foundation-core.propositional-maps</a>
<a id="23862" class="Keyword">open</a> <a id="23867" class="Keyword">import</a> <a id="23874" href="foundation-core.propositions.html" class="Module">foundation-core.propositions</a>
<a id="23903" class="Keyword">open</a> <a id="23908" class="Keyword">import</a> <a id="23915" href="foundation-core.pullbacks.html" class="Module">foundation-core.pullbacks</a>
<a id="23941" class="Keyword">open</a> <a id="23946" class="Keyword">import</a> <a id="23953" href="foundation-core.retractions.html" class="Module">foundation-core.retractions</a>
<a id="23981" class="Keyword">open</a> <a id="23986" class="Keyword">import</a> <a id="23993" href="foundation-core.sections.html" class="Module">foundation-core.sections</a>
<a id="24018" class="Keyword">open</a> <a id="24023" class="Keyword">import</a> <a id="24030" href="foundation-core.sets.html" class="Module">foundation-core.sets</a>
<a id="24051" class="Keyword">open</a> <a id="24056" class="Keyword">import</a> <a id="24063" href="foundation-core.singleton-induction.html" class="Module">foundation-core.singleton-induction</a>
<a id="24099" class="Keyword">open</a> <a id="24104" class="Keyword">import</a> <a id="24111" href="foundation-core.subtype-identity-principle.html" class="Module">foundation-core.subtype-identity-principle</a>
<a id="24154" class="Keyword">open</a> <a id="24159" class="Keyword">import</a> <a id="24166" href="foundation-core.subtypes.html" class="Module">foundation-core.subtypes</a>
<a id="24191" class="Keyword">open</a> <a id="24196" class="Keyword">import</a> <a id="24203" href="foundation-core.truncated-maps.html" class="Module">foundation-core.truncated-maps</a>
<a id="24234" class="Keyword">open</a> <a id="24239" class="Keyword">import</a> <a id="24246" href="foundation-core.truncated-types.html" class="Module">foundation-core.truncated-types</a>
<a id="24278" class="Keyword">open</a> <a id="24283" class="Keyword">import</a> <a id="24290" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a>
<a id="24324" class="Keyword">open</a> <a id="24329" class="Keyword">import</a> <a id="24336" href="foundation-core.type-arithmetic-cartesian-product-types.html" class="Module">foundation-core.type-arithmetic-cartesian-product-types</a>
<a id="24392" class="Keyword">open</a> <a id="24397" class="Keyword">import</a> <a id="24404" href="foundation-core.type-arithmetic-dependent-pair-types.html" class="Module">foundation-core.type-arithmetic-dependent-pair-types</a>
<a id="24457" class="Keyword">open</a> <a id="24462" class="Keyword">import</a> <a id="24469" href="foundation-core.univalence.html" class="Module">foundation-core.univalence</a>
<a id="24496" class="Keyword">open</a> <a id="24501" class="Keyword">import</a> <a id="24508" href="foundation-core.universal-property-pullbacks.html" class="Module">foundation-core.universal-property-pullbacks</a>
<a id="24553" class="Keyword">open</a> <a id="24558" class="Keyword">import</a> <a id="24565" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a>
</pre>
## Graph theory

<pre class="Agda"><a id="24627" class="Keyword">open</a> <a id="24632" class="Keyword">import</a> <a id="24639" href="graph-theory.html" class="Module">graph-theory</a>
<a id="24652" class="Keyword">open</a> <a id="24657" class="Keyword">import</a> <a id="24664" href="graph-theory.circuits-undirected-graphs.html" class="Module">graph-theory.circuits-undirected-graphs</a>
<a id="24704" class="Keyword">open</a> <a id="24709" class="Keyword">import</a> <a id="24716" href="graph-theory.closed-walks-undirected-graphs.html" class="Module">graph-theory.closed-walks-undirected-graphs</a>
<a id="24760" class="Keyword">open</a> <a id="24765" class="Keyword">import</a> <a id="24772" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a>
<a id="24811" class="Keyword">open</a> <a id="24816" class="Keyword">import</a> <a id="24823" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="24865" class="Keyword">open</a> <a id="24870" class="Keyword">import</a> <a id="24877" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a>
<a id="24917" class="Keyword">open</a> <a id="24922" class="Keyword">import</a> <a id="24929" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a>
<a id="24970" class="Keyword">open</a> <a id="24975" class="Keyword">import</a> <a id="24982" href="graph-theory.cycles-undirected-graphs.html" class="Module">graph-theory.cycles-undirected-graphs</a>
<a id="25020" class="Keyword">open</a> <a id="25025" class="Keyword">import</a> <a id="25032" href="graph-theory.directed-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.directed-graph-structures-on-standard-finite-sets</a>
<a id="25095" class="Keyword">open</a> <a id="25100" class="Keyword">import</a> <a id="25107" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>
<a id="25136" class="Keyword">open</a> <a id="25141" class="Keyword">import</a> <a id="25148" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a>
<a id="25193" class="Keyword">open</a> <a id="25198" class="Keyword">import</a> <a id="25205" href="graph-theory.embeddings-undirected-graphs.html" class="Module">graph-theory.embeddings-undirected-graphs</a>
<a id="25247" class="Keyword">open</a> <a id="25252" class="Keyword">import</a> <a id="25259" href="graph-theory.enriched-undirected-graphs.html" class="Module">graph-theory.enriched-undirected-graphs</a>
<a id="25299" class="Keyword">open</a> <a id="25304" class="Keyword">import</a> <a id="25311" href="graph-theory.equivalences-enriched-undirected-graphs.html" class="Module">graph-theory.equivalences-enriched-undirected-graphs</a>
<a id="25364" class="Keyword">open</a> <a id="25369" class="Keyword">import</a> <a id="25376" href="graph-theory.equivalences-undirected-graphs.html" class="Module">graph-theory.equivalences-undirected-graphs</a>
<a id="25420" class="Keyword">open</a> <a id="25425" class="Keyword">import</a> <a id="25432" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a>
<a id="25481" class="Keyword">open</a> <a id="25486" class="Keyword">import</a> <a id="25493" href="graph-theory.faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.faithful-morphisms-undirected-graphs</a>
<a id="25543" class="Keyword">open</a> <a id="25548" class="Keyword">import</a> <a id="25555" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>
<a id="25582" class="Keyword">open</a> <a id="25587" class="Keyword">import</a> <a id="25594" href="graph-theory.hypergraphs.html" class="Module">graph-theory.hypergraphs</a>
<a id="25619" class="Keyword">open</a> <a id="25624" class="Keyword">import</a> <a id="25631" href="graph-theory.matchings.html" class="Module">graph-theory.matchings</a>
<a id="25654" class="Keyword">open</a> <a id="25659" class="Keyword">import</a> <a id="25666" href="graph-theory.mere-equivalences-undirected-graphs.html" class="Module">graph-theory.mere-equivalences-undirected-graphs</a>
<a id="25715" class="Keyword">open</a> <a id="25720" class="Keyword">import</a> <a id="25727" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a>
<a id="25766" class="Keyword">open</a> <a id="25771" class="Keyword">import</a> <a id="25778" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="25819" class="Keyword">open</a> <a id="25824" class="Keyword">import</a> <a id="25831" href="graph-theory.neighbors-undirected-graphs.html" class="Module">graph-theory.neighbors-undirected-graphs</a>
<a id="25872" class="Keyword">open</a> <a id="25877" class="Keyword">import</a> <a id="25884" href="graph-theory.orientations-undirected-graphs.html" class="Module">graph-theory.orientations-undirected-graphs</a>
<a id="25928" class="Keyword">open</a> <a id="25933" class="Keyword">import</a> <a id="25940" href="graph-theory.paths-undirected-graphs.html" class="Module">graph-theory.paths-undirected-graphs</a>
<a id="25977" class="Keyword">open</a> <a id="25982" class="Keyword">import</a> <a id="25989" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="26011" class="Keyword">open</a> <a id="26016" class="Keyword">import</a> <a id="26023" href="graph-theory.reflexive-graphs.html" class="Module">graph-theory.reflexive-graphs</a>
<a id="26053" class="Keyword">open</a> <a id="26058" class="Keyword">import</a> <a id="26065" href="graph-theory.regular-undirected-graphs.html" class="Module">graph-theory.regular-undirected-graphs</a>
<a id="26104" class="Keyword">open</a> <a id="26109" class="Keyword">import</a> <a id="26116" href="graph-theory.rooted-quasitrees.html" class="Module">graph-theory.rooted-quasitrees</a>
<a id="26147" class="Keyword">open</a> <a id="26152" class="Keyword">import</a> <a id="26159" href="graph-theory.rooted-trees.html" class="Module">graph-theory.rooted-trees</a>
<a id="26185" class="Keyword">open</a> <a id="26190" class="Keyword">import</a> <a id="26197" href="graph-theory.simple-undirected-graphs.html" class="Module">graph-theory.simple-undirected-graphs</a>
<a id="26235" class="Keyword">open</a> <a id="26240" class="Keyword">import</a> <a id="26247" href="graph-theory.stereoisomerism-enriched-undirected-graphs.html" class="Module">graph-theory.stereoisomerism-enriched-undirected-graphs</a>
<a id="26303" class="Keyword">open</a> <a id="26308" class="Keyword">import</a> <a id="26315" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a>
<a id="26373" class="Keyword">open</a> <a id="26378" class="Keyword">import</a> <a id="26385" href="graph-theory.trails-undirected-graphs.html" class="Module">graph-theory.trails-undirected-graphs</a>
<a id="26423" class="Keyword">open</a> <a id="26428" class="Keyword">import</a> <a id="26435" href="graph-theory.trees.html" class="Module">graph-theory.trees</a>
<a id="26454" class="Keyword">open</a> <a id="26459" class="Keyword">import</a> <a id="26466" href="graph-theory.undirected-graph-structures-on-standard-finite-sets.html" class="Module">graph-theory.undirected-graph-structures-on-standard-finite-sets</a>
<a id="26531" class="Keyword">open</a> <a id="26536" class="Keyword">import</a> <a id="26543" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
<a id="26574" class="Keyword">open</a> <a id="26579" class="Keyword">import</a> <a id="26586" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a>
<a id="26613" class="Keyword">open</a> <a id="26618" class="Keyword">import</a> <a id="26625" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a>
<a id="26653" class="Keyword">open</a> <a id="26658" class="Keyword">import</a> <a id="26665" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a>
</pre>
## Group theory

<pre class="Agda"><a id="26732" class="Keyword">open</a> <a id="26737" class="Keyword">import</a> <a id="26744" href="group-theory.html" class="Module">group-theory</a>
<a id="26757" class="Keyword">open</a> <a id="26762" class="Keyword">import</a> <a id="26769" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>
<a id="26797" class="Keyword">open</a> <a id="26802" class="Keyword">import</a> <a id="26809" href="group-theory.addition-homomorphisms-abelian-groups.html" class="Module">group-theory.addition-homomorphisms-abelian-groups</a>
<a id="26860" class="Keyword">open</a> <a id="26865" class="Keyword">import</a> <a id="26872" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="26905" class="Keyword">open</a> <a id="26910" class="Keyword">import</a> <a id="26917" href="group-theory.cartesian-products-abelian-groups.html" class="Module">group-theory.cartesian-products-abelian-groups</a>
<a id="26964" class="Keyword">open</a> <a id="26969" class="Keyword">import</a> <a id="26976" href="group-theory.cartesian-products-groups.html" class="Module">group-theory.cartesian-products-groups</a>
<a id="27015" class="Keyword">open</a> <a id="27020" class="Keyword">import</a> <a id="27027" href="group-theory.cartesian-products-monoids.html" class="Module">group-theory.cartesian-products-monoids</a>
<a id="27067" class="Keyword">open</a> <a id="27072" class="Keyword">import</a> <a id="27079" href="group-theory.cartesian-products-semigroups.html" class="Module">group-theory.cartesian-products-semigroups</a>
<a id="27122" class="Keyword">open</a> <a id="27127" class="Keyword">import</a> <a id="27134" href="group-theory.category-of-groups.html" class="Module">group-theory.category-of-groups</a>
<a id="27166" class="Keyword">open</a> <a id="27171" class="Keyword">import</a> <a id="27178" href="group-theory.category-of-semigroups.html" class="Module">group-theory.category-of-semigroups</a>
<a id="27214" class="Keyword">open</a> <a id="27219" class="Keyword">import</a> <a id="27226" href="group-theory.cayleys-theorem.html" class="Module">group-theory.cayleys-theorem</a>
<a id="27255" class="Keyword">open</a> <a id="27260" class="Keyword">import</a> <a id="27267" href="group-theory.centers-groups.html" class="Module">group-theory.centers-groups</a>
<a id="27295" class="Keyword">open</a> <a id="27300" class="Keyword">import</a> <a id="27307" href="group-theory.commutative-monoids.html" class="Module">group-theory.commutative-monoids</a>
<a id="27340" class="Keyword">open</a> <a id="27345" class="Keyword">import</a> <a id="27352" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="27388" class="Keyword">open</a> <a id="27393" class="Keyword">import</a> <a id="27400" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="27429" class="Keyword">open</a> <a id="27434" class="Keyword">import</a> <a id="27441" href="group-theory.congruence-relations-groups.html" class="Module">group-theory.congruence-relations-groups</a>
<a id="27482" class="Keyword">open</a> <a id="27487" class="Keyword">import</a> <a id="27494" href="group-theory.congruence-relations-monoids.html" class="Module">group-theory.congruence-relations-monoids</a>
<a id="27536" class="Keyword">open</a> <a id="27541" class="Keyword">import</a> <a id="27548" href="group-theory.congruence-relations-semigroups.html" class="Module">group-theory.congruence-relations-semigroups</a>
<a id="27593" class="Keyword">open</a> <a id="27598" class="Keyword">import</a> <a id="27605" href="group-theory.conjugation.html" class="Module">group-theory.conjugation</a>
<a id="27630" class="Keyword">open</a> <a id="27635" class="Keyword">import</a> <a id="27642" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a>
<a id="27704" class="Keyword">open</a> <a id="27709" class="Keyword">import</a> <a id="27716" href="group-theory.decidable-subgroups.html" class="Module">group-theory.decidable-subgroups</a>
<a id="27749" class="Keyword">open</a> <a id="27754" class="Keyword">import</a> <a id="27761" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="27802" class="Keyword">open</a> <a id="27807" class="Keyword">import</a> <a id="27814" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a>
<a id="27843" class="Keyword">open</a> <a id="27848" class="Keyword">import</a> <a id="27855" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a>
<a id="27879" class="Keyword">open</a> <a id="27884" class="Keyword">import</a> <a id="27891" href="group-theory.embeddings-groups.html" class="Module">group-theory.embeddings-groups</a>
<a id="27922" class="Keyword">open</a> <a id="27927" class="Keyword">import</a> <a id="27934" href="group-theory.endomorphism-rings-abelian-groups.html" class="Module">group-theory.endomorphism-rings-abelian-groups</a>
<a id="27981" class="Keyword">open</a> <a id="27986" class="Keyword">import</a> <a id="27993" href="group-theory.epimorphisms-groups.html" class="Module">group-theory.epimorphisms-groups</a>
<a id="28026" class="Keyword">open</a> <a id="28031" class="Keyword">import</a> <a id="28038" href="group-theory.equivalences-concrete-group-actions.html" class="Module">group-theory.equivalences-concrete-group-actions</a>
<a id="28087" class="Keyword">open</a> <a id="28092" class="Keyword">import</a> <a id="28099" href="group-theory.equivalences-group-actions.html" class="Module">group-theory.equivalences-group-actions</a>
<a id="28139" class="Keyword">open</a> <a id="28144" class="Keyword">import</a> <a id="28151" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a>
<a id="28191" class="Keyword">open</a> <a id="28196" class="Keyword">import</a> <a id="28203" href="group-theory.equivalences-semigroups.html" class="Module">group-theory.equivalences-semigroups</a>
<a id="28240" class="Keyword">open</a> <a id="28245" class="Keyword">import</a> <a id="28252" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a>
<a id="28299" class="Keyword">open</a> <a id="28304" class="Keyword">import</a> <a id="28311" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a>
<a id="28352" class="Keyword">open</a> <a id="28357" class="Keyword">import</a> <a id="28364" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="28408" class="Keyword">open</a> <a id="28413" class="Keyword">import</a> <a id="28420" href="group-theory.free-higher-group-actions.html" class="Module">group-theory.free-higher-group-actions</a>
<a id="28459" class="Keyword">open</a> <a id="28464" class="Keyword">import</a> <a id="28471" href="group-theory.full-subgroups.html" class="Module">group-theory.full-subgroups</a>
<a id="28499" class="Keyword">open</a> <a id="28504" class="Keyword">import</a> <a id="28511" href="group-theory.furstenberg-groups.html" class="Module">group-theory.furstenberg-groups</a>
<a id="28543" class="Keyword">open</a> <a id="28548" class="Keyword">import</a> <a id="28555" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a>
<a id="28582" class="Keyword">open</a> <a id="28587" class="Keyword">import</a> <a id="28594" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="28614" class="Keyword">open</a> <a id="28619" class="Keyword">import</a> <a id="28626" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="28660" class="Keyword">open</a> <a id="28665" class="Keyword">import</a> <a id="28672" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="28699" class="Keyword">open</a> <a id="28704" class="Keyword">import</a> <a id="28711" href="group-theory.homomorphisms-abelian-groups.html" class="Module">group-theory.homomorphisms-abelian-groups</a>
<a id="28753" class="Keyword">open</a> <a id="28758" class="Keyword">import</a> <a id="28765" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="28815" class="Keyword">open</a> <a id="28820" class="Keyword">import</a> <a id="28827" href="group-theory.homomorphisms-generated-subgroups.html" class="Module">group-theory.homomorphisms-generated-subgroups</a>
<a id="28874" class="Keyword">open</a> <a id="28879" class="Keyword">import</a> <a id="28886" href="group-theory.homomorphisms-group-actions.html" class="Module">group-theory.homomorphisms-group-actions</a>
<a id="28927" class="Keyword">open</a> <a id="28932" class="Keyword">import</a> <a id="28939" href="group-theory.homomorphisms-groups.html" class="Module">group-theory.homomorphisms-groups</a>
<a id="28973" class="Keyword">open</a> <a id="28978" class="Keyword">import</a> <a id="28985" href="group-theory.homomorphisms-higher-group-actions.html" class="Module">group-theory.homomorphisms-higher-group-actions</a>
<a id="29033" class="Keyword">open</a> <a id="29038" class="Keyword">import</a> <a id="29045" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>
<a id="29086" class="Keyword">open</a> <a id="29091" class="Keyword">import</a> <a id="29098" href="group-theory.homomorphisms-monoids.html" class="Module">group-theory.homomorphisms-monoids</a>
<a id="29133" class="Keyword">open</a> <a id="29138" class="Keyword">import</a> <a id="29145" href="group-theory.homomorphisms-semigroups.html" class="Module">group-theory.homomorphisms-semigroups</a>
<a id="29183" class="Keyword">open</a> <a id="29188" class="Keyword">import</a> <a id="29195" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a>
<a id="29230" class="Keyword">open</a> <a id="29235" class="Keyword">import</a> <a id="29242" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a>
<a id="29274" class="Keyword">open</a> <a id="29279" class="Keyword">import</a> <a id="29286" href="group-theory.invertible-elements-monoids.html" class="Module">group-theory.invertible-elements-monoids</a>
<a id="29327" class="Keyword">open</a> <a id="29332" class="Keyword">import</a> <a id="29339" href="group-theory.isomorphisms-abelian-groups.html" class="Module">group-theory.isomorphisms-abelian-groups</a>
<a id="29380" class="Keyword">open</a> <a id="29385" class="Keyword">import</a> <a id="29392" href="group-theory.isomorphisms-group-actions.html" class="Module">group-theory.isomorphisms-group-actions</a>
<a id="29432" class="Keyword">open</a> <a id="29437" class="Keyword">import</a> <a id="29444" href="group-theory.isomorphisms-groups.html" class="Module">group-theory.isomorphisms-groups</a>
<a id="29477" class="Keyword">open</a> <a id="29482" class="Keyword">import</a> <a id="29489" href="group-theory.isomorphisms-semigroups.html" class="Module">group-theory.isomorphisms-semigroups</a>
<a id="29526" class="Keyword">open</a> <a id="29531" class="Keyword">import</a> <a id="29538" href="group-theory.loop-groups-sets.html" class="Module">group-theory.loop-groups-sets</a>
<a id="29568" class="Keyword">open</a> <a id="29573" class="Keyword">import</a> <a id="29580" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="29601" class="Keyword">open</a> <a id="29606" class="Keyword">import</a> <a id="29613" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="29667" class="Keyword">open</a> <a id="29672" class="Keyword">import</a> <a id="29679" href="group-theory.mere-equivalences-group-actions.html" class="Module">group-theory.mere-equivalences-group-actions</a>
<a id="29724" class="Keyword">open</a> <a id="29729" class="Keyword">import</a> <a id="29736" href="group-theory.monoid-actions.html" class="Module">group-theory.monoid-actions</a>
<a id="29764" class="Keyword">open</a> <a id="29769" class="Keyword">import</a> <a id="29776" href="group-theory.monoids.html" class="Module">group-theory.monoids</a>
<a id="29797" class="Keyword">open</a> <a id="29802" class="Keyword">import</a> <a id="29809" href="group-theory.monomorphisms-concrete-groups.html" class="Module">group-theory.monomorphisms-concrete-groups</a>
<a id="29852" class="Keyword">open</a> <a id="29857" class="Keyword">import</a> <a id="29864" href="group-theory.monomorphisms-groups.html" class="Module">group-theory.monomorphisms-groups</a>
<a id="29898" class="Keyword">open</a> <a id="29903" class="Keyword">import</a> <a id="29910" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
<a id="29940" class="Keyword">open</a> <a id="29945" class="Keyword">import</a> <a id="29952" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>
<a id="29998" class="Keyword">open</a> <a id="30003" class="Keyword">import</a> <a id="30010" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a>
<a id="30064" class="Keyword">open</a> <a id="30069" class="Keyword">import</a> <a id="30076" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
<a id="30119" class="Keyword">open</a> <a id="30124" class="Keyword">import</a> <a id="30131" href="group-theory.orbits-group-actions.html" class="Module">group-theory.orbits-group-actions</a>
<a id="30165" class="Keyword">open</a> <a id="30170" class="Keyword">import</a> <a id="30177" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a>
<a id="30218" class="Keyword">open</a> <a id="30223" class="Keyword">import</a> <a id="30230" href="group-theory.orbits-monoid-actions.html" class="Module">group-theory.orbits-monoid-actions</a>
<a id="30265" class="Keyword">open</a> <a id="30270" class="Keyword">import</a> <a id="30277" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a>
<a id="30316" class="Keyword">open</a> <a id="30321" class="Keyword">import</a> <a id="30328" href="group-theory.precategory-of-group-actions.html" class="Module">group-theory.precategory-of-group-actions</a>
<a id="30370" class="Keyword">open</a> <a id="30375" class="Keyword">import</a> <a id="30382" href="group-theory.precategory-of-groups.html" class="Module">group-theory.precategory-of-groups</a>
<a id="30417" class="Keyword">open</a> <a id="30422" class="Keyword">import</a> <a id="30429" href="group-theory.precategory-of-semigroups.html" class="Module">group-theory.precategory-of-semigroups</a>
<a id="30468" class="Keyword">open</a> <a id="30473" class="Keyword">import</a> <a id="30480" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a>
<a id="30517" class="Keyword">open</a> <a id="30522" class="Keyword">import</a> <a id="30529" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a>
<a id="30576" class="Keyword">open</a> <a id="30581" class="Keyword">import</a> <a id="30588" href="group-theory.products-of-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.products-of-tuples-of-elements-commutative-monoids</a>
<a id="30652" class="Keyword">open</a> <a id="30657" class="Keyword">import</a> <a id="30664" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a>
<a id="30709" class="Keyword">open</a> <a id="30714" class="Keyword">import</a> <a id="30721" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
<a id="30745" class="Keyword">open</a> <a id="30750" class="Keyword">import</a> <a id="30757" href="group-theory.sheargroups.html" class="Module">group-theory.sheargroups</a>
<a id="30782" class="Keyword">open</a> <a id="30787" class="Keyword">import</a> <a id="30794" href="group-theory.shriek-concrete-group-actions.html" class="Module">group-theory.shriek-concrete-group-actions</a>
<a id="30837" class="Keyword">open</a> <a id="30842" class="Keyword">import</a> <a id="30849" href="group-theory.stabilizer-groups.html" class="Module">group-theory.stabilizer-groups</a>
<a id="30880" class="Keyword">open</a> <a id="30885" class="Keyword">import</a> <a id="30892" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a>
<a id="30946" class="Keyword">open</a> <a id="30951" class="Keyword">import</a> <a id="30958" href="group-theory.subgroups.html" class="Module">group-theory.subgroups</a>
<a id="30981" class="Keyword">open</a> <a id="30986" class="Keyword">import</a> <a id="30993" href="group-theory.subgroups-abelian-groups.html" class="Module">group-theory.subgroups-abelian-groups</a>
<a id="31031" class="Keyword">open</a> <a id="31036" class="Keyword">import</a> <a id="31043" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
<a id="31082" class="Keyword">open</a> <a id="31087" class="Keyword">import</a> <a id="31094" href="group-theory.subgroups-generated-by-subsets-groups.html" class="Module">group-theory.subgroups-generated-by-subsets-groups</a>
<a id="31145" class="Keyword">open</a> <a id="31150" class="Keyword">import</a> <a id="31157" href="group-theory.subgroups-higher-groups.html" class="Module">group-theory.subgroups-higher-groups</a>
<a id="31194" class="Keyword">open</a> <a id="31199" class="Keyword">import</a> <a id="31206" href="group-theory.submonoids.html" class="Module">group-theory.submonoids</a>
<a id="31230" class="Keyword">open</a> <a id="31235" class="Keyword">import</a> <a id="31242" href="group-theory.subsemigroups.html" class="Module">group-theory.subsemigroups</a>
<a id="31269" class="Keyword">open</a> <a id="31274" class="Keyword">import</a> <a id="31281" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
<a id="31338" class="Keyword">open</a> <a id="31343" class="Keyword">import</a> <a id="31350" href="group-theory.substitution-functor-group-actions.html" class="Module">group-theory.substitution-functor-group-actions</a>
<a id="31398" class="Keyword">open</a> <a id="31403" class="Keyword">import</a> <a id="31410" href="group-theory.symmetric-concrete-groups.html" class="Module">group-theory.symmetric-concrete-groups</a>
<a id="31449" class="Keyword">open</a> <a id="31454" class="Keyword">import</a> <a id="31461" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="31491" class="Keyword">open</a> <a id="31496" class="Keyword">import</a> <a id="31503" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a>
<a id="31540" class="Keyword">open</a> <a id="31545" class="Keyword">import</a> <a id="31552" href="group-theory.torsors.html" class="Module">group-theory.torsors</a>
<a id="31573" class="Keyword">open</a> <a id="31578" class="Keyword">import</a> <a id="31585" href="group-theory.transitive-concrete-group-actions.html" class="Module">group-theory.transitive-concrete-group-actions</a>
<a id="31632" class="Keyword">open</a> <a id="31637" class="Keyword">import</a> <a id="31644" href="group-theory.transitive-group-actions.html" class="Module">group-theory.transitive-group-actions</a>
<a id="31682" class="Keyword">open</a> <a id="31687" class="Keyword">import</a> <a id="31694" href="group-theory.trivial-subgroups.html" class="Module">group-theory.trivial-subgroups</a>
<a id="31725" class="Keyword">open</a> <a id="31730" class="Keyword">import</a> <a id="31737" href="group-theory.unordered-tuples-of-elements-commutative-monoids.html" class="Module">group-theory.unordered-tuples-of-elements-commutative-monoids</a>
</pre>
## Linear algebra

<pre class="Agda"><a id="31831" class="Keyword">open</a> <a id="31836" class="Keyword">import</a> <a id="31843" href="linear-algebra.html" class="Module">linear-algebra</a>
<a id="31858" class="Keyword">open</a> <a id="31863" class="Keyword">import</a> <a id="31870" href="linear-algebra.constant-matrices.html" class="Module">linear-algebra.constant-matrices</a>
<a id="31903" class="Keyword">open</a> <a id="31908" class="Keyword">import</a> <a id="31915" href="linear-algebra.constant-vectors.html" class="Module">linear-algebra.constant-vectors</a>
<a id="31947" class="Keyword">open</a> <a id="31952" class="Keyword">import</a> <a id="31959" href="linear-algebra.diagonal-matrices-on-rings.html" class="Module">linear-algebra.diagonal-matrices-on-rings</a>
<a id="32001" class="Keyword">open</a> <a id="32006" class="Keyword">import</a> <a id="32013" href="linear-algebra.functoriality-matrices.html" class="Module">linear-algebra.functoriality-matrices</a>
<a id="32051" class="Keyword">open</a> <a id="32056" class="Keyword">import</a> <a id="32063" href="linear-algebra.functoriality-vectors.html" class="Module">linear-algebra.functoriality-vectors</a>
<a id="32100" class="Keyword">open</a> <a id="32105" class="Keyword">import</a> <a id="32112" href="linear-algebra.matrices-on-rings.html" class="Module">linear-algebra.matrices-on-rings</a>
<a id="32145" class="Keyword">open</a> <a id="32150" class="Keyword">import</a> <a id="32157" href="linear-algebra.matrices.html" class="Module">linear-algebra.matrices</a>
<a id="32181" class="Keyword">open</a> <a id="32186" class="Keyword">import</a> <a id="32193" href="linear-algebra.multiplication-matrices.html" class="Module">linear-algebra.multiplication-matrices</a>
<a id="32232" class="Keyword">open</a> <a id="32237" class="Keyword">import</a> <a id="32244" href="linear-algebra.scalar-multiplication-matrices.html" class="Module">linear-algebra.scalar-multiplication-matrices</a>
<a id="32290" class="Keyword">open</a> <a id="32295" class="Keyword">import</a> <a id="32302" href="linear-algebra.scalar-multiplication-vectors.html" class="Module">linear-algebra.scalar-multiplication-vectors</a>
<a id="32347" class="Keyword">open</a> <a id="32352" class="Keyword">import</a> <a id="32359" href="linear-algebra.transposition-matrices.html" class="Module">linear-algebra.transposition-matrices</a>
<a id="32397" class="Keyword">open</a> <a id="32402" class="Keyword">import</a> <a id="32409" href="linear-algebra.vectors-on-rings.html" class="Module">linear-algebra.vectors-on-rings</a>
<a id="32441" class="Keyword">open</a> <a id="32446" class="Keyword">import</a> <a id="32453" href="linear-algebra.vectors.html" class="Module">linear-algebra.vectors</a>
</pre>
## Order theory

<pre class="Agda"><a id="32506" class="Keyword">open</a> <a id="32511" class="Keyword">import</a> <a id="32518" href="order-theory.html" class="Module">order-theory</a>
<a id="32531" class="Keyword">open</a> <a id="32536" class="Keyword">import</a> <a id="32543" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a>
<a id="32570" class="Keyword">open</a> <a id="32575" class="Keyword">import</a> <a id="32582" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a>
<a id="32612" class="Keyword">open</a> <a id="32617" class="Keyword">import</a> <a id="32624" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a>
<a id="32657" class="Keyword">open</a> <a id="32662" class="Keyword">import</a> <a id="32669" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a>
<a id="32705" class="Keyword">open</a> <a id="32710" class="Keyword">import</a> <a id="32717" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a>
<a id="32752" class="Keyword">open</a> <a id="32757" class="Keyword">import</a> <a id="32764" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a>
<a id="32791" class="Keyword">open</a> <a id="32796" class="Keyword">import</a> <a id="32803" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a>
<a id="32833" class="Keyword">open</a> <a id="32838" class="Keyword">import</a> <a id="32845" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a>
<a id="32881" class="Keyword">open</a> <a id="32886" class="Keyword">import</a> <a id="32893" href="order-theory.greatest-lower-bounds-posets.html" class="Module">order-theory.greatest-lower-bounds-posets</a>
<a id="32935" class="Keyword">open</a> <a id="32940" class="Keyword">import</a> <a id="32947" href="order-theory.ideals-preorders.html" class="Module">order-theory.ideals-preorders</a>
<a id="32977" class="Keyword">open</a> <a id="32982" class="Keyword">import</a> <a id="32989" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a>
<a id="33021" class="Keyword">open</a> <a id="33026" class="Keyword">import</a> <a id="33033" href="order-theory.join-semilattices.html" class="Module">order-theory.join-semilattices</a>
<a id="33064" class="Keyword">open</a> <a id="33069" class="Keyword">import</a> <a id="33076" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a>
<a id="33102" class="Keyword">open</a> <a id="33107" class="Keyword">import</a> <a id="33114" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="33143" class="Keyword">open</a> <a id="33148" class="Keyword">import</a> <a id="33155" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a>
<a id="33192" class="Keyword">open</a> <a id="33197" class="Keyword">import</a> <a id="33204" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a>
<a id="33244" class="Keyword">open</a> <a id="33249" class="Keyword">import</a> <a id="33256" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
<a id="33278" class="Keyword">open</a> <a id="33283" class="Keyword">import</a> <a id="33290" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a>
<a id="33325" class="Keyword">open</a> <a id="33330" class="Keyword">import</a> <a id="33337" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a>
<a id="33375" class="Keyword">open</a> <a id="33380" class="Keyword">import</a> <a id="33387" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a>
<a id="33426" class="Keyword">open</a> <a id="33431" class="Keyword">import</a> <a id="33438" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a>
<a id="33473" class="Keyword">open</a> <a id="33478" class="Keyword">import</a> <a id="33485" href="order-theory.lower-types-preorders.html" class="Module">order-theory.lower-types-preorders</a>
<a id="33520" class="Keyword">open</a> <a id="33525" class="Keyword">import</a> <a id="33532" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a>
<a id="33567" class="Keyword">open</a> <a id="33572" class="Keyword">import</a> <a id="33579" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a>
<a id="33617" class="Keyword">open</a> <a id="33622" class="Keyword">import</a> <a id="33629" href="order-theory.meet-semilattices.html" class="Module">order-theory.meet-semilattices</a>
<a id="33660" class="Keyword">open</a> <a id="33665" class="Keyword">import</a> <a id="33672" href="order-theory.order-preserving-maps-posets.html" class="Module">order-theory.order-preserving-maps-posets</a>
<a id="33714" class="Keyword">open</a> <a id="33719" class="Keyword">import</a> <a id="33726" href="order-theory.order-preserving-maps-preorders.html" class="Module">order-theory.order-preserving-maps-preorders</a>
<a id="33771" class="Keyword">open</a> <a id="33776" class="Keyword">import</a> <a id="33783" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a>
<a id="33816" class="Keyword">open</a> <a id="33821" class="Keyword">import</a> <a id="33828" href="order-theory.posets.html" class="Module">order-theory.posets</a>
<a id="33848" class="Keyword">open</a> <a id="33853" class="Keyword">import</a> <a id="33860" href="order-theory.preorders.html" class="Module">order-theory.preorders</a>
<a id="33883" class="Keyword">open</a> <a id="33888" class="Keyword">import</a> <a id="33895" href="order-theory.subposets.html" class="Module">order-theory.subposets</a>
<a id="33918" class="Keyword">open</a> <a id="33923" class="Keyword">import</a> <a id="33930" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a>
<a id="33956" class="Keyword">open</a> <a id="33961" class="Keyword">import</a> <a id="33968" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a>
<a id="33994" class="Keyword">open</a> <a id="33999" class="Keyword">import</a> <a id="34006" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a>
</pre>
## Organic chemistry

<pre class="Agda"><a id="34070" class="Keyword">open</a> <a id="34075" class="Keyword">import</a> <a id="34082" href="organic-chemistry.html" class="Module">organic-chemistry</a>
<a id="34100" class="Keyword">open</a> <a id="34105" class="Keyword">import</a> <a id="34112" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a>
<a id="34139" class="Keyword">open</a> <a id="34144" class="Keyword">import</a> <a id="34151" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a>
<a id="34177" class="Keyword">open</a> <a id="34182" class="Keyword">import</a> <a id="34189" href="organic-chemistry.alkenes.html" class="Module">organic-chemistry.alkenes</a>
<a id="34215" class="Keyword">open</a> <a id="34220" class="Keyword">import</a> <a id="34227" href="organic-chemistry.alkynes.html" class="Module">organic-chemistry.alkynes</a>
<a id="34253" class="Keyword">open</a> <a id="34258" class="Keyword">import</a> <a id="34265" href="organic-chemistry.ethane.html" class="Module">organic-chemistry.ethane</a>
<a id="34290" class="Keyword">open</a> <a id="34295" class="Keyword">import</a> <a id="34302" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
<a id="34333" class="Keyword">open</a> <a id="34338" class="Keyword">import</a> <a id="34345" href="organic-chemistry.methane.html" class="Module">organic-chemistry.methane</a>
<a id="34371" class="Keyword">open</a> <a id="34376" class="Keyword">import</a> <a id="34383" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
</pre>
## Polytopes

<pre class="Agda"><a id="34446" class="Keyword">open</a> <a id="34451" class="Keyword">import</a> <a id="34458" href="polytopes.html" class="Module">polytopes</a>
<a id="34468" class="Keyword">open</a> <a id="34473" class="Keyword">import</a> <a id="34480" href="polytopes.abstract-polytopes.html" class="Module">polytopes.abstract-polytopes</a>
</pre>
## Ring theory

<pre class="Agda"><a id="34538" class="Keyword">open</a> <a id="34543" class="Keyword">import</a> <a id="34550" href="ring-theory.html" class="Module">ring-theory</a>
<a id="34562" class="Keyword">open</a> <a id="34567" class="Keyword">import</a> <a id="34574" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a>
<a id="34611" class="Keyword">open</a> <a id="34616" class="Keyword">import</a> <a id="34623" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a>
<a id="34650" class="Keyword">open</a> <a id="34655" class="Keyword">import</a> <a id="34662" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a>
<a id="34694" class="Keyword">open</a> <a id="34699" class="Keyword">import</a> <a id="34706" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a>
<a id="34752" class="Keyword">open</a> <a id="34757" class="Keyword">import</a> <a id="34764" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="34789" class="Keyword">open</a> <a id="34794" class="Keyword">import</a> <a id="34801" href="ring-theory.idempotent-elements-rings.html" class="Module">ring-theory.idempotent-elements-rings</a>
<a id="34839" class="Keyword">open</a> <a id="34844" class="Keyword">import</a> <a id="34851" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a>
<a id="34894" class="Keyword">open</a> <a id="34899" class="Keyword">import</a> <a id="34906" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="34944" class="Keyword">open</a> <a id="34949" class="Keyword">import</a> <a id="34956" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a>
<a id="34987" class="Keyword">open</a> <a id="34992" class="Keyword">import</a> <a id="34999" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a>
<a id="35023" class="Keyword">open</a> <a id="35028" class="Keyword">import</a> <a id="35035" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a>
<a id="35067" class="Keyword">open</a> <a id="35072" class="Keyword">import</a> <a id="35079" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a>
<a id="35105" class="Keyword">open</a> <a id="35110" class="Keyword">import</a> <a id="35117" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a>
<a id="35146" class="Keyword">open</a> <a id="35151" class="Keyword">import</a> <a id="35158" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="35195" class="Keyword">open</a> <a id="35200" class="Keyword">import</a> <a id="35207" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="35236" class="Keyword">open</a> <a id="35241" class="Keyword">import</a> <a id="35248" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a>
<a id="35275" class="Keyword">open</a> <a id="35280" class="Keyword">import</a> <a id="35287" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="35324" class="Keyword">open</a> <a id="35329" class="Keyword">import</a> <a id="35336" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a>
<a id="35363" class="Keyword">open</a> <a id="35368" class="Keyword">import</a> <a id="35375" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a>
<a id="35408" class="Keyword">open</a> <a id="35413" class="Keyword">import</a> <a id="35420" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
<a id="35438" class="Keyword">open</a> <a id="35443" class="Keyword">import</a> <a id="35450" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a>
</pre>
## Set theory

<pre class="Agda"><a id="35504" class="Keyword">open</a> <a id="35509" class="Keyword">import</a> <a id="35516" href="set-theory.html" class="Module">set-theory</a>
<a id="35527" class="Keyword">open</a> <a id="35532" class="Keyword">import</a> <a id="35539" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a>
<a id="35562" class="Keyword">open</a> <a id="35567" class="Keyword">import</a> <a id="35574" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a>
<a id="35598" class="Keyword">open</a> <a id="35603" class="Keyword">import</a> <a id="35610" href="set-theory.cardinalities.html" class="Module">set-theory.cardinalities</a>
<a id="35635" class="Keyword">open</a> <a id="35640" class="Keyword">import</a> <a id="35647" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
<a id="35673" class="Keyword">open</a> <a id="35678" class="Keyword">import</a> <a id="35685" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a>
</pre>
## Structured types

<pre class="Agda"><a id="35747" class="Keyword">open</a> <a id="35752" class="Keyword">import</a> <a id="35759" href="structured-types.html" class="Module">structured-types</a>
<a id="35776" class="Keyword">open</a> <a id="35781" class="Keyword">import</a> <a id="35788" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a>
<a id="35823" class="Keyword">open</a> <a id="35828" class="Keyword">import</a> <a id="35835" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a>
<a id="35879" class="Keyword">open</a> <a id="35884" class="Keyword">import</a> <a id="35891" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a>
<a id="35955" class="Keyword">open</a> <a id="35960" class="Keyword">import</a> <a id="35967" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a>
<a id="36006" class="Keyword">open</a> <a id="36011" class="Keyword">import</a> <a id="36018" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a>
<a id="36064" class="Keyword">open</a> <a id="36069" class="Keyword">import</a> <a id="36076" href="structured-types.initial-pointed-type-equipped-with-automorphism.html" class="Module">structured-types.initial-pointed-type-equipped-with-automorphism</a>
<a id="36141" class="Keyword">open</a> <a id="36146" class="Keyword">import</a> <a id="36153" href="structured-types.magmas.html" class="Module">structured-types.magmas</a>
<a id="36177" class="Keyword">open</a> <a id="36182" class="Keyword">import</a> <a id="36189" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a>
<a id="36258" class="Keyword">open</a> <a id="36263" class="Keyword">import</a> <a id="36270" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a>
<a id="36315" class="Keyword">open</a> <a id="36320" class="Keyword">import</a> <a id="36327" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a>
<a id="36361" class="Keyword">open</a> <a id="36366" class="Keyword">import</a> <a id="36373" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a>
<a id="36434" class="Keyword">open</a> <a id="36439" class="Keyword">import</a> <a id="36446" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a>
<a id="36491" class="Keyword">open</a> <a id="36496" class="Keyword">import</a> <a id="36503" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="36541" class="Keyword">open</a> <a id="36546" class="Keyword">import</a> <a id="36553" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a>
<a id="36596" class="Keyword">open</a> <a id="36601" class="Keyword">import</a> <a id="36608" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="36644" class="Keyword">open</a> <a id="36649" class="Keyword">import</a> <a id="36656" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="36686" class="Keyword">open</a> <a id="36691" class="Keyword">import</a> <a id="36698" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a>
<a id="36732" class="Keyword">open</a> <a id="36737" class="Keyword">import</a> <a id="36744" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
<a id="36775" class="Keyword">open</a> <a id="36780" class="Keyword">import</a> <a id="36787" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a>
<a id="36846" class="Keyword">open</a> <a id="36851" class="Keyword">import</a> <a id="36858" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a>
<a id="36909" class="Keyword">open</a> <a id="36914" class="Keyword">import</a> <a id="36921" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a>
<a id="36972" class="Keyword">open</a> <a id="36977" class="Keyword">import</a> <a id="36984" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a>
<a id="37039" class="Keyword">open</a> <a id="37044" class="Keyword">import</a> <a id="37051" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a>
<a id="37083" class="Keyword">open</a> <a id="37088" class="Keyword">import</a> <a id="37095" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a>
<a id="37124" class="Keyword">open</a> <a id="37129" class="Keyword">import</a> <a id="37136" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a>
<a id="37164" class="Keyword">open</a> <a id="37169" class="Keyword">import</a> <a id="37176" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a>
<a id="37206" class="Keyword">open</a> <a id="37211" class="Keyword">import</a> <a id="37218" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a>
<a id="37252" class="Keyword">open</a> <a id="37257" class="Keyword">import</a> <a id="37264" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a>
</pre>
## Synthetic homotopy theory

<pre class="Agda"><a id="37340" class="Keyword">open</a> <a id="37345" class="Keyword">import</a> <a id="37352" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a>
<a id="37378" class="Keyword">open</a> <a id="37383" class="Keyword">import</a> <a id="37390" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="37428" class="Keyword">open</a> <a id="37433" class="Keyword">import</a> <a id="37440" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a>
<a id="37477" class="Keyword">open</a> <a id="37482" class="Keyword">import</a> <a id="37489" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a>
<a id="37529" class="Keyword">open</a> <a id="37534" class="Keyword">import</a> <a id="37541" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a>
<a id="37580" class="Keyword">open</a> <a id="37585" class="Keyword">import</a> <a id="37592" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
<a id="37625" class="Keyword">open</a> <a id="37630" class="Keyword">import</a> <a id="37637" href="synthetic-homotopy-theory.cocones-pushouts.html" class="Module">synthetic-homotopy-theory.cocones-pushouts</a>
<a id="37680" class="Keyword">open</a> <a id="37685" class="Keyword">import</a> <a id="37692" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
<a id="37727" class="Keyword">open</a> <a id="37732" class="Keyword">import</a> <a id="37739" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a>
<a id="37784" class="Keyword">open</a> <a id="37789" class="Keyword">import</a> <a id="37796" href="synthetic-homotopy-theory.free-loops.html" class="Module">synthetic-homotopy-theory.free-loops</a>
<a id="37833" class="Keyword">open</a> <a id="37838" class="Keyword">import</a> <a id="37845" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a>
<a id="37897" class="Keyword">open</a> <a id="37902" class="Keyword">import</a> <a id="37909" href="synthetic-homotopy-theory.groups-of-loops-in-1-types.html" class="Module">synthetic-homotopy-theory.groups-of-loops-in-1-types</a>
<a id="37962" class="Keyword">open</a> <a id="37967" class="Keyword">import</a> <a id="37974" href="synthetic-homotopy-theory.infinite-complex-projective-space.html" class="Module">synthetic-homotopy-theory.infinite-complex-projective-space</a>
<a id="38034" class="Keyword">open</a> <a id="38039" class="Keyword">import</a> <a id="38046" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a>
<a id="38094" class="Keyword">open</a> <a id="38099" class="Keyword">import</a> <a id="38106" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a>
<a id="38146" class="Keyword">open</a> <a id="38151" class="Keyword">import</a> <a id="38158" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a>
<a id="38205" class="Keyword">open</a> <a id="38210" class="Keyword">import</a> <a id="38217" href="synthetic-homotopy-theory.joins-of-types.html" class="Module">synthetic-homotopy-theory.joins-of-types</a>
<a id="38258" class="Keyword">open</a> <a id="38263" class="Keyword">import</a> <a id="38270" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
<a id="38308" class="Keyword">open</a> <a id="38313" class="Keyword">import</a> <a id="38320" href="synthetic-homotopy-theory.multiplication-circle.html" class="Module">synthetic-homotopy-theory.multiplication-circle</a>
<a id="38368" class="Keyword">open</a> <a id="38373" class="Keyword">import</a> <a id="38380" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a>
<a id="38417" class="Keyword">open</a> <a id="38422" class="Keyword">import</a> <a id="38429" href="synthetic-homotopy-theory.pushouts.html" class="Module">synthetic-homotopy-theory.pushouts</a>
<a id="38464" class="Keyword">open</a> <a id="38469" class="Keyword">import</a> <a id="38476" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a>
<a id="38510" class="Keyword">open</a> <a id="38515" class="Keyword">import</a> <a id="38522" href="synthetic-homotopy-theory.suspensions-of-types.html" class="Module">synthetic-homotopy-theory.suspensions-of-types</a>
<a id="38569" class="Keyword">open</a> <a id="38574" class="Keyword">import</a> <a id="38581" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a>
<a id="38626" class="Keyword">open</a> <a id="38631" class="Keyword">import</a> <a id="38638" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a>
<a id="38687" class="Keyword">open</a> <a id="38692" class="Keyword">import</a> <a id="38699" href="synthetic-homotopy-theory.universal-property-circle.html" class="Module">synthetic-homotopy-theory.universal-property-circle</a>
<a id="38751" class="Keyword">open</a> <a id="38756" class="Keyword">import</a> <a id="38763" href="synthetic-homotopy-theory.universal-property-pushouts.html" class="Module">synthetic-homotopy-theory.universal-property-pushouts</a>
<a id="38817" class="Keyword">open</a> <a id="38822" class="Keyword">import</a> <a id="38829" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a>
</pre>
## Type theories

<pre class="Agda"><a id="38910" class="Keyword">open</a> <a id="38915" class="Keyword">import</a> <a id="38922" href="type-theories.html" class="Module">type-theories</a>
<a id="38936" class="Keyword">open</a> <a id="38941" class="Keyword">import</a> <a id="38948" href="type-theories.comprehension-type-theories.html" class="Module">type-theories.comprehension-type-theories</a>
<a id="38990" class="Keyword">open</a> <a id="38995" class="Keyword">import</a> <a id="39002" href="type-theories.dependent-type-theories.html" class="Module">type-theories.dependent-type-theories</a>
<a id="39040" class="Keyword">open</a> <a id="39045" class="Keyword">import</a> <a id="39052" href="type-theories.fibered-dependent-type-theories.html" class="Module">type-theories.fibered-dependent-type-theories</a>
<a id="39098" class="Keyword">open</a> <a id="39103" class="Keyword">import</a> <a id="39110" href="type-theories.sections-dependent-type-theories.html" class="Module">type-theories.sections-dependent-type-theories</a>
<a id="39157" class="Keyword">open</a> <a id="39162" class="Keyword">import</a> <a id="39169" href="type-theories.simple-type-theories.html" class="Module">type-theories.simple-type-theories</a>
<a id="39204" class="Keyword">open</a> <a id="39209" class="Keyword">import</a> <a id="39216" href="type-theories.unityped-type-theories.html" class="Module">type-theories.unityped-type-theories</a>
</pre>
## Univalent combinatorics

<pre class="Agda"><a id="39294" class="Keyword">open</a> <a id="39299" class="Keyword">import</a> <a id="39306" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="39330" class="Keyword">open</a> <a id="39335" class="Keyword">import</a> <a id="39342" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="39395" class="Keyword">open</a> <a id="39400" class="Keyword">import</a> <a id="39407" href="univalent-combinatorics.2-element-subtypes.html" class="Module">univalent-combinatorics.2-element-subtypes</a>
<a id="39450" class="Keyword">open</a> <a id="39455" class="Keyword">import</a> <a id="39462" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="39502" class="Keyword">open</a> <a id="39507" class="Keyword">import</a> <a id="39514" href="univalent-combinatorics.binomial-types.html" class="Module">univalent-combinatorics.binomial-types</a>
<a id="39553" class="Keyword">open</a> <a id="39558" class="Keyword">import</a> <a id="39565" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a>
<a id="39599" class="Keyword">open</a> <a id="39604" class="Keyword">import</a> <a id="39611" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="39659" class="Keyword">open</a> <a id="39664" class="Keyword">import</a> <a id="39671" href="univalent-combinatorics.cartesian-products-species.html" class="Module">univalent-combinatorics.cartesian-products-species</a>
<a id="39722" class="Keyword">open</a> <a id="39727" class="Keyword">import</a> <a id="39734" href="univalent-combinatorics.classical-finite-types.html" class="Module">univalent-combinatorics.classical-finite-types</a>
<a id="39781" class="Keyword">open</a> <a id="39786" class="Keyword">import</a> <a id="39793" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="39845" class="Keyword">open</a> <a id="39850" class="Keyword">import</a> <a id="39857" href="univalent-combinatorics.composition-species.html" class="Module">univalent-combinatorics.composition-species</a>
<a id="39901" class="Keyword">open</a> <a id="39906" class="Keyword">import</a> <a id="39913" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="39953" class="Keyword">open</a> <a id="39958" class="Keyword">import</a> <a id="39965" href="univalent-combinatorics.coproducts-species.html" class="Module">univalent-combinatorics.coproducts-species</a>
<a id="40008" class="Keyword">open</a> <a id="40013" class="Keyword">import</a> <a id="40020" href="univalent-combinatorics.counting-decidable-subtypes.html" class="Module">univalent-combinatorics.counting-decidable-subtypes</a>
<a id="40072" class="Keyword">open</a> <a id="40077" class="Keyword">import</a> <a id="40084" href="univalent-combinatorics.counting-dependent-pair-types.html" class="Module">univalent-combinatorics.counting-dependent-pair-types</a>
<a id="40138" class="Keyword">open</a> <a id="40143" class="Keyword">import</a> <a id="40150" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a>
<a id="40198" class="Keyword">open</a> <a id="40203" class="Keyword">import</a> <a id="40210" href="univalent-combinatorics.counting-maybe.html" class="Module">univalent-combinatorics.counting-maybe</a>
<a id="40249" class="Keyword">open</a> <a id="40254" class="Keyword">import</a> <a id="40261" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a>
<a id="40294" class="Keyword">open</a> <a id="40299" class="Keyword">import</a> <a id="40306" href="univalent-combinatorics.cubes.html" class="Module">univalent-combinatorics.cubes</a>
<a id="40336" class="Keyword">open</a> <a id="40341" class="Keyword">import</a> <a id="40348" href="univalent-combinatorics.cycle-index-series-species.html" class="Module">univalent-combinatorics.cycle-index-series-species</a>
<a id="40399" class="Keyword">open</a> <a id="40404" class="Keyword">import</a> <a id="40411" href="univalent-combinatorics.cycle-partitions.html" class="Module">univalent-combinatorics.cycle-partitions</a>
<a id="40452" class="Keyword">open</a> <a id="40457" class="Keyword">import</a> <a id="40464" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="40501" class="Keyword">open</a> <a id="40506" class="Keyword">import</a> <a id="40513" href="univalent-combinatorics.decidable-dependent-function-types.html" class="Module">univalent-combinatorics.decidable-dependent-function-types</a>
<a id="40572" class="Keyword">open</a> <a id="40577" class="Keyword">import</a> <a id="40584" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a>
<a id="40639" class="Keyword">open</a> <a id="40644" class="Keyword">import</a> <a id="40651" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="40707" class="Keyword">open</a> <a id="40712" class="Keyword">import</a> <a id="40719" href="univalent-combinatorics.decidable-propositions.html" class="Module">univalent-combinatorics.decidable-propositions</a>
<a id="40766" class="Keyword">open</a> <a id="40771" class="Keyword">import</a> <a id="40778" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="40821" class="Keyword">open</a> <a id="40826" class="Keyword">import</a> <a id="40833" href="univalent-combinatorics.dedekind-finite-sets.html" class="Module">univalent-combinatorics.dedekind-finite-sets</a>
<a id="40878" class="Keyword">open</a> <a id="40883" class="Keyword">import</a> <a id="40890" href="univalent-combinatorics.dependent-function-types.html" class="Module">univalent-combinatorics.dependent-function-types</a>
<a id="40939" class="Keyword">open</a> <a id="40944" class="Keyword">import</a> <a id="40951" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="41002" class="Keyword">open</a> <a id="41007" class="Keyword">import</a> <a id="41014" href="univalent-combinatorics.derivatives-species.html" class="Module">univalent-combinatorics.derivatives-species</a>
<a id="41058" class="Keyword">open</a> <a id="41063" class="Keyword">import</a> <a id="41070" href="univalent-combinatorics.distributivity-of-set-truncation-over-finite-products.html" class="Module">univalent-combinatorics.distributivity-of-set-truncation-over-finite-products</a>
<a id="41148" class="Keyword">open</a> <a id="41153" class="Keyword">import</a> <a id="41160" href="univalent-combinatorics.double-counting.html" class="Module">univalent-combinatorics.double-counting</a>
<a id="41200" class="Keyword">open</a> <a id="41205" class="Keyword">import</a> <a id="41212" href="univalent-combinatorics.embeddings-standard-finite-types.html" class="Module">univalent-combinatorics.embeddings-standard-finite-types</a>
<a id="41269" class="Keyword">open</a> <a id="41274" class="Keyword">import</a> <a id="41281" href="univalent-combinatorics.embeddings.html" class="Module">univalent-combinatorics.embeddings</a>
<a id="41316" class="Keyword">open</a> <a id="41321" class="Keyword">import</a> <a id="41328" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="41374" class="Keyword">open</a> <a id="41379" class="Keyword">import</a> <a id="41386" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="41441" class="Keyword">open</a> <a id="41446" class="Keyword">import</a> <a id="41453" href="univalent-combinatorics.equivalences-cubes.html" class="Module">univalent-combinatorics.equivalences-cubes</a>
<a id="41496" class="Keyword">open</a> <a id="41501" class="Keyword">import</a> <a id="41508" href="univalent-combinatorics.equivalences-species.html" class="Module">univalent-combinatorics.equivalences-species</a>
<a id="41553" class="Keyword">open</a> <a id="41558" class="Keyword">import</a> <a id="41565" href="univalent-combinatorics.equivalences-standard-finite-types.html" class="Module">univalent-combinatorics.equivalences-standard-finite-types</a>
<a id="41624" class="Keyword">open</a> <a id="41629" class="Keyword">import</a> <a id="41636" href="univalent-combinatorics.equivalences.html" class="Module">univalent-combinatorics.equivalences</a>
<a id="41673" class="Keyword">open</a> <a id="41678" class="Keyword">import</a> <a id="41685" href="univalent-combinatorics.exponents-species.html" class="Module">univalent-combinatorics.exponents-species</a>
<a id="41727" class="Keyword">open</a> <a id="41732" class="Keyword">import</a> <a id="41739" href="univalent-combinatorics.ferrers-diagrams.html" class="Module">univalent-combinatorics.ferrers-diagrams</a>
<a id="41780" class="Keyword">open</a> <a id="41785" class="Keyword">import</a> <a id="41792" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="41831" class="Keyword">open</a> <a id="41836" class="Keyword">import</a> <a id="41843" href="univalent-combinatorics.finite-choice.html" class="Module">univalent-combinatorics.finite-choice</a>
<a id="41881" class="Keyword">open</a> <a id="41886" class="Keyword">import</a> <a id="41893" href="univalent-combinatorics.finite-connected-components.html" class="Module">univalent-combinatorics.finite-connected-components</a>
<a id="41945" class="Keyword">open</a> <a id="41950" class="Keyword">import</a> <a id="41957" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a>
<a id="42002" class="Keyword">open</a> <a id="42007" class="Keyword">import</a> <a id="42014" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a>
<a id="42053" class="Keyword">open</a> <a id="42058" class="Keyword">import</a> <a id="42065" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="42102" class="Keyword">open</a> <a id="42107" class="Keyword">import</a> <a id="42114" href="univalent-combinatorics.finitely-presented-types.html" class="Module">univalent-combinatorics.finitely-presented-types</a>
<a id="42163" class="Keyword">open</a> <a id="42168" class="Keyword">import</a> <a id="42175" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="42214" class="Keyword">open</a> <a id="42219" class="Keyword">import</a> <a id="42226" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="42264" class="Keyword">open</a> <a id="42269" class="Keyword">import</a> <a id="42276" href="univalent-combinatorics.inequality-types-with-counting.html" class="Module">univalent-combinatorics.inequality-types-with-counting</a>
<a id="42331" class="Keyword">open</a> <a id="42336" class="Keyword">import</a> <a id="42343" href="univalent-combinatorics.injective-maps.html" class="Module">univalent-combinatorics.injective-maps</a>
<a id="42382" class="Keyword">open</a> <a id="42387" class="Keyword">import</a> <a id="42394" href="univalent-combinatorics.isotopies-latin-squares.html" class="Module">univalent-combinatorics.isotopies-latin-squares</a>
<a id="42442" class="Keyword">open</a> <a id="42447" class="Keyword">import</a> <a id="42454" href="univalent-combinatorics.kuratowsky-finite-sets.html" class="Module">univalent-combinatorics.kuratowsky-finite-sets</a>
<a id="42501" class="Keyword">open</a> <a id="42506" class="Keyword">import</a> <a id="42513" href="univalent-combinatorics.latin-squares.html" class="Module">univalent-combinatorics.latin-squares</a>
<a id="42551" class="Keyword">open</a> <a id="42556" class="Keyword">import</a> <a id="42563" href="univalent-combinatorics.lists.html" class="Module">univalent-combinatorics.lists</a>
<a id="42593" class="Keyword">open</a> <a id="42598" class="Keyword">import</a> <a id="42605" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="42662" class="Keyword">open</a> <a id="42667" class="Keyword">import</a> <a id="42674" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a>
<a id="42728" class="Keyword">open</a> <a id="42733" class="Keyword">import</a> <a id="42740" href="univalent-combinatorics.maybe.html" class="Module">univalent-combinatorics.maybe</a>
<a id="42770" class="Keyword">open</a> <a id="42775" class="Keyword">import</a> <a id="42782" href="univalent-combinatorics.morphisms-finite-species.html" class="Module">univalent-combinatorics.morphisms-finite-species</a>
<a id="42831" class="Keyword">open</a> <a id="42836" class="Keyword">import</a> <a id="42843" href="univalent-combinatorics.morphisms-species.html" class="Module">univalent-combinatorics.morphisms-species</a>
<a id="42885" class="Keyword">open</a> <a id="42890" class="Keyword">import</a> <a id="42897" href="univalent-combinatorics.necklaces.html" class="Module">univalent-combinatorics.necklaces</a>
<a id="42931" class="Keyword">open</a> <a id="42936" class="Keyword">import</a> <a id="42943" href="univalent-combinatorics.orientations-complete-undirected-graph.html" class="Module">univalent-combinatorics.orientations-complete-undirected-graph</a>
<a id="43006" class="Keyword">open</a> <a id="43011" class="Keyword">import</a> <a id="43018" href="univalent-combinatorics.orientations-cubes.html" class="Module">univalent-combinatorics.orientations-cubes</a>
<a id="43061" class="Keyword">open</a> <a id="43066" class="Keyword">import</a> <a id="43073" href="univalent-combinatorics.partitions.html" class="Module">univalent-combinatorics.partitions</a>
<a id="43108" class="Keyword">open</a> <a id="43113" class="Keyword">import</a> <a id="43120" href="univalent-combinatorics.petri-nets.html" class="Module">univalent-combinatorics.petri-nets</a>
<a id="43155" class="Keyword">open</a> <a id="43160" class="Keyword">import</a> <a id="43167" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="43207" class="Keyword">open</a> <a id="43212" class="Keyword">import</a> <a id="43219" href="univalent-combinatorics.pigeonhole-principle.html" class="Module">univalent-combinatorics.pigeonhole-principle</a>
<a id="43264" class="Keyword">open</a> <a id="43269" class="Keyword">import</a> <a id="43276" href="univalent-combinatorics.pointing-species.html" class="Module">univalent-combinatorics.pointing-species</a>
<a id="43317" class="Keyword">open</a> <a id="43322" class="Keyword">import</a> <a id="43329" href="univalent-combinatorics.precategory-of-finite-species.html" class="Module">univalent-combinatorics.precategory-of-finite-species</a>
<a id="43383" class="Keyword">open</a> <a id="43388" class="Keyword">import</a> <a id="43395" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a>
<a id="43445" class="Keyword">open</a> <a id="43450" class="Keyword">import</a> <a id="43457" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a>
<a id="43504" class="Keyword">open</a> <a id="43509" class="Keyword">import</a> <a id="43516" href="univalent-combinatorics.ramsey-theory.html" class="Module">univalent-combinatorics.ramsey-theory</a>
<a id="43554" class="Keyword">open</a> <a id="43559" class="Keyword">import</a> <a id="43566" href="univalent-combinatorics.retracts-of-finite-types.html" class="Module">univalent-combinatorics.retracts-of-finite-types</a>
<a id="43615" class="Keyword">open</a> <a id="43620" class="Keyword">import</a> <a id="43627" href="univalent-combinatorics.sequences-finite-types.html" class="Module">univalent-combinatorics.sequences-finite-types</a>
<a id="43674" class="Keyword">open</a> <a id="43679" class="Keyword">import</a> <a id="43686" href="univalent-combinatorics.skipping-element-standard-finite-types.html" class="Module">univalent-combinatorics.skipping-element-standard-finite-types</a>
<a id="43749" class="Keyword">open</a> <a id="43754" class="Keyword">import</a> <a id="43761" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a>
<a id="43793" class="Keyword">open</a> <a id="43798" class="Keyword">import</a> <a id="43805" href="univalent-combinatorics.standard-finite-pruned-trees.html" class="Module">univalent-combinatorics.standard-finite-pruned-trees</a>
<a id="43858" class="Keyword">open</a> <a id="43863" class="Keyword">import</a> <a id="43870" href="univalent-combinatorics.standard-finite-trees.html" class="Module">univalent-combinatorics.standard-finite-trees</a>
<a id="43916" class="Keyword">open</a> <a id="43921" class="Keyword">import</a> <a id="43928" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="43974" class="Keyword">open</a> <a id="43979" class="Keyword">import</a> <a id="43986" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
<a id="44026" class="Keyword">open</a> <a id="44031" class="Keyword">import</a> <a id="44038" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a>
<a id="44085" class="Keyword">open</a> <a id="44090" class="Keyword">import</a> <a id="44097" href="univalent-combinatorics.sums-of-natural-numbers.html" class="Module">univalent-combinatorics.sums-of-natural-numbers</a>
<a id="44145" class="Keyword">open</a> <a id="44150" class="Keyword">import</a> <a id="44157" href="univalent-combinatorics.surjective-maps.html" class="Module">univalent-combinatorics.surjective-maps</a>
<a id="44197" class="Keyword">open</a> <a id="44202" class="Keyword">import</a> <a id="44209" href="univalent-combinatorics.symmetric-difference.html" class="Module">univalent-combinatorics.symmetric-difference</a>
<a id="44254" class="Keyword">open</a> <a id="44259" class="Keyword">import</a> <a id="44266" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
<a id="44331" class="Keyword">open</a> <a id="44336" class="Keyword">import</a> <a id="44343" href="univalent-combinatorics.unlabeled-partitions.html" class="Module">univalent-combinatorics.unlabeled-partitions</a>
<a id="44388" class="Keyword">open</a> <a id="44393" class="Keyword">import</a> <a id="44400" href="univalent-combinatorics.unlabeled-rooted-trees.html" class="Module">univalent-combinatorics.unlabeled-rooted-trees</a>
<a id="44447" class="Keyword">open</a> <a id="44452" class="Keyword">import</a> <a id="44459" href="univalent-combinatorics.unlabeled-structures-species.html" class="Module">univalent-combinatorics.unlabeled-structures-species</a>
<a id="44512" class="Keyword">open</a> <a id="44517" class="Keyword">import</a> <a id="44524" href="univalent-combinatorics.unlabeled-trees.html" class="Module">univalent-combinatorics.unlabeled-trees</a>
</pre>