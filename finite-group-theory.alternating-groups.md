---
title: Alternating groups
---

<pre class="Agda"><a id="44" class="Symbol">{-#</a> <a id="48" class="Keyword">OPTIONS</a> <a id="56" class="Pragma">--without-K</a> <a id="68" class="Pragma">--exact-split</a> <a id="82" class="Symbol">#-}</a>
<a id="86" class="Keyword">module</a> <a id="93" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a> <a id="132" class="Keyword">where</a>

<a id="139" class="Keyword">open</a> <a id="144" class="Keyword">import</a> <a id="151" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="181" class="Keyword">open</a> <a id="186" class="Keyword">import</a> <a id="193" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="214" class="Keyword">open</a> <a id="219" class="Keyword">import</a> <a id="226" href="group-theory.groups.html" class="Module">group-theory.groups</a>

<a id="247" class="Keyword">open</a> <a id="252" class="Keyword">import</a> <a id="259" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>

<a id="298" class="Keyword">open</a> <a id="303" class="Keyword">import</a> <a id="310" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="351" class="Keyword">using</a> <a id="357" class="Symbol">(</a><a id="358" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a><a id="359" class="Symbol">)</a>
<a id="361" class="Keyword">open</a> <a id="366" class="Keyword">import</a> <a id="373" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a> <a id="419" class="Keyword">using</a> <a id="425" class="Symbol">(</a><a id="426" href="univalent-combinatorics.standard-finite-types.html#2285" class="Function">Fin-Set</a><a id="433" class="Symbol">)</a>
<a id="435" class="Keyword">open</a> <a id="440" class="Keyword">import</a> <a id="447" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="484" class="Keyword">using</a> <a id="490" class="Symbol">(</a><a id="491" href="univalent-combinatorics.finite-types.html#5385" class="Function">UU-Fin-Level</a><a id="503" class="Symbol">;</a> <a id="505" href="univalent-combinatorics.finite-types.html#15248" class="Function">set-UU-Fin-Level</a><a id="521" class="Symbol">)</a>
</pre>
## Idea

The alternating group on a finite set `X` is the group of even permutations of `X`, i.e. it is the kernel of the sign homomorphism `Aut(X) → Aut(2)`.

## Definition

<pre class="Agda"><a id="711" class="Keyword">module</a> <a id="718" href="finite-group-theory.alternating-groups.html#718" class="Module">_</a> <a id="720" class="Symbol">{</a><a id="721" href="finite-group-theory.alternating-groups.html#721" class="Bound">l</a><a id="722" class="Symbol">}</a> <a id="724" class="Symbol">(</a><a id="725" href="finite-group-theory.alternating-groups.html#725" class="Bound">n</a> <a id="727" class="Symbol">:</a> <a id="729" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a><a id="730" class="Symbol">)</a> <a id="732" class="Symbol">(</a><a id="733" href="finite-group-theory.alternating-groups.html#733" class="Bound">X</a> <a id="735" class="Symbol">:</a> <a id="737" href="univalent-combinatorics.finite-types.html#5385" class="Function">UU-Fin-Level</a> <a id="750" href="finite-group-theory.alternating-groups.html#721" class="Bound">l</a> <a id="752" href="finite-group-theory.alternating-groups.html#725" class="Bound">n</a><a id="753" class="Symbol">)</a> <a id="755" class="Keyword">where</a>
  <a id="763" href="finite-group-theory.alternating-groups.html#763" class="Function">alternating-Group</a> <a id="781" class="Symbol">:</a> <a id="783" href="group-theory.groups.html#2481" class="Function">Group</a> <a id="789" href="finite-group-theory.alternating-groups.html#721" class="Bound">l</a>
  <a id="793" href="finite-group-theory.alternating-groups.html#763" class="Function">alternating-Group</a> <a id="811" class="Symbol">=</a> <a id="813" href="group-theory.kernels.html#2482" class="Function">group-kernel-hom-Group</a>
    <a id="840" class="Symbol">(</a> <a id="842" href="group-theory.symmetric-groups.html#3569" class="Function">symmetric-Group</a> <a id="858" class="Symbol">(</a><a id="859" href="univalent-combinatorics.finite-types.html#15248" class="Function">set-UU-Fin-Level</a> <a id="876" href="finite-group-theory.alternating-groups.html#725" class="Bound">n</a> <a id="878" href="finite-group-theory.alternating-groups.html#733" class="Bound">X</a><a id="879" class="Symbol">))</a>
    <a id="886" class="Symbol">(</a> <a id="888" href="group-theory.symmetric-groups.html#3569" class="Function">symmetric-Group</a> <a id="904" class="Symbol">(</a><a id="905" href="univalent-combinatorics.standard-finite-types.html#2285" class="Function">Fin-Set</a> <a id="913" class="Number">2</a><a id="914" class="Symbol">))</a>
    <a id="921" class="Symbol">(</a> <a id="923" href="finite-group-theory.sign-homomorphism.html#11247" class="Function">sign-homomorphism</a> <a id="941" href="finite-group-theory.alternating-groups.html#725" class="Bound">n</a> <a id="943" href="finite-group-theory.alternating-groups.html#733" class="Bound">X</a><a id="944" class="Symbol">)</a>
</pre>