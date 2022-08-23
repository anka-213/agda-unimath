---
title: Alternating groups
---

<pre class="Agda"><a id="44" class="Symbol">{-#</a> <a id="48" class="Keyword">OPTIONS</a> <a id="56" class="Pragma">--without-K</a> <a id="68" class="Pragma">--exact-split</a> <a id="82" class="Symbol">#-}</a>
<a id="86" class="Keyword">module</a> <a id="93" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a> <a id="132" class="Keyword">where</a>

<a id="139" class="Keyword">open</a> <a id="144" class="Keyword">import</a> <a id="151" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>
<a id="181" class="Keyword">open</a> <a id="186" class="Keyword">import</a> <a id="193" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="214" class="Keyword">open</a> <a id="219" class="Keyword">import</a> <a id="226" href="group-theory.groups.html" class="Module">group-theory.groups</a>

<a id="247" class="Keyword">open</a> <a id="252" class="Keyword">import</a> <a id="259" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a>

<a id="298" class="Keyword">open</a> <a id="303" class="Keyword">import</a> <a id="310" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="351" class="Keyword">using</a> <a id="357" class="Symbol">(</a><a id="358" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="359" class="Symbol">)</a>
<a id="361" class="Keyword">open</a> <a id="366" class="Keyword">import</a> <a id="373" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a> <a id="419" class="Keyword">using</a> <a id="425" class="Symbol">(</a><a id="426" href="univalent-combinatorics.standard-finite-types.html#2284" class="Function">Fin-Set</a><a id="433" class="Symbol">)</a>
<a id="435" class="Keyword">open</a> <a id="440" class="Keyword">import</a> <a id="447" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="484" class="Keyword">using</a> <a id="490" class="Symbol">(</a><a id="491" href="univalent-combinatorics.finite-types.html#5087" class="Function">UU-Fin</a><a id="497" class="Symbol">;</a> <a id="499" href="univalent-combinatorics.finite-types.html#14443" class="Function">set-UU-Fin</a><a id="509" class="Symbol">)</a>
</pre>
## Idea

The alternating group on a finite set `X` is the group of even permutations of `X`, i.e. it is the kernel of the sign homomorphism `Aut(X) → Aut(2)`.

## Definition

<pre class="Agda"><a id="699" class="Keyword">module</a> <a id="706" href="finite-group-theory.alternating-groups.html#706" class="Module">_</a> <a id="708" class="Symbol">{</a><a id="709" href="finite-group-theory.alternating-groups.html#709" class="Bound">l</a><a id="710" class="Symbol">}</a> <a id="712" class="Symbol">(</a><a id="713" href="finite-group-theory.alternating-groups.html#713" class="Bound">n</a> <a id="715" class="Symbol">:</a> <a id="717" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="718" class="Symbol">)</a> <a id="720" class="Symbol">(</a><a id="721" href="finite-group-theory.alternating-groups.html#721" class="Bound">X</a> <a id="723" class="Symbol">:</a> <a id="725" href="univalent-combinatorics.finite-types.html#5087" class="Function">UU-Fin</a> <a id="732" href="finite-group-theory.alternating-groups.html#709" class="Bound">l</a> <a id="734" href="finite-group-theory.alternating-groups.html#713" class="Bound">n</a><a id="735" class="Symbol">)</a> <a id="737" class="Keyword">where</a>
  <a id="745" href="finite-group-theory.alternating-groups.html#745" class="Function">alternating-Group</a> <a id="763" class="Symbol">:</a> <a id="765" href="group-theory.groups.html#2750" class="Function">Group</a> <a id="771" href="finite-group-theory.alternating-groups.html#709" class="Bound">l</a>
  <a id="775" href="finite-group-theory.alternating-groups.html#745" class="Function">alternating-Group</a> <a id="793" class="Symbol">=</a> <a id="795" href="group-theory.kernels.html#2475" class="Function">group-kernel-hom-Group</a>
    <a id="822" class="Symbol">(</a> <a id="824" href="group-theory.symmetric-groups.html#3597" class="Function">symmetric-Group</a> <a id="840" class="Symbol">(</a><a id="841" href="univalent-combinatorics.finite-types.html#14443" class="Function">set-UU-Fin</a> <a id="852" href="finite-group-theory.alternating-groups.html#713" class="Bound">n</a> <a id="854" href="finite-group-theory.alternating-groups.html#721" class="Bound">X</a><a id="855" class="Symbol">))</a>
    <a id="862" class="Symbol">(</a> <a id="864" href="group-theory.symmetric-groups.html#3597" class="Function">symmetric-Group</a> <a id="880" class="Symbol">(</a><a id="881" href="univalent-combinatorics.standard-finite-types.html#2284" class="Function">Fin-Set</a> <a id="889" class="Number">2</a><a id="890" class="Symbol">))</a>
    <a id="897" class="Symbol">(</a> <a id="899" href="finite-group-theory.sign-homomorphism.html#11097" class="Function">sign-homomorphism</a> <a id="917" href="finite-group-theory.alternating-groups.html#713" class="Bound">n</a> <a id="919" href="finite-group-theory.alternating-groups.html#721" class="Bound">X</a><a id="920" class="Symbol">)</a>
</pre>