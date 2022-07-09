---
title: Spectra
---

<pre class="Agda"><a id="33" class="Symbol">{-#</a> <a id="37" class="Keyword">OPTIONS</a> <a id="45" class="Pragma">--without-K</a> <a id="57" class="Pragma">--exact-split</a> <a id="71" class="Symbol">#-}</a>

<a id="76" class="Keyword">module</a> <a id="83" href="synthetic-homotopy-theory.spectra.html" class="Module">synthetic-homotopy-theory.spectra</a> <a id="117" class="Keyword">where</a>

<a id="124" class="Keyword">open</a> <a id="129" class="Keyword">import</a> <a id="136" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="178" class="Keyword">open</a> <a id="183" class="Keyword">import</a> <a id="190" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="222" class="Keyword">open</a> <a id="227" class="Keyword">import</a> <a id="234" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="262" class="Keyword">open</a> <a id="267" class="Keyword">import</a> <a id="274" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
<a id="312" class="Keyword">open</a> <a id="317" class="Keyword">import</a> <a id="324" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>

<a id="356" class="Keyword">open</a> <a id="361" class="Keyword">import</a> <a id="368" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
</pre>
## Idea

A spectrum is an infinite sequence of pointed types `A` such that `A n ≃* Ω (A (n+1))` for each `n : ℕ`.

## Definition

<pre class="Agda"><a id="Spectrum"></a><a id="549" href="synthetic-homotopy-theory.spectra.html#549" class="Function">Spectrum</a> <a id="558" class="Symbol">:</a> <a id="560" class="Symbol">(</a><a id="561" href="synthetic-homotopy-theory.spectra.html#561" class="Bound">l</a> <a id="563" class="Symbol">:</a> <a id="565" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="570" class="Symbol">)</a> <a id="572" class="Symbol">→</a> <a id="574" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="577" class="Symbol">(</a><a id="578" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="583" href="synthetic-homotopy-theory.spectra.html#561" class="Bound">l</a><a id="584" class="Symbol">)</a>
<a id="586" href="synthetic-homotopy-theory.spectra.html#549" class="Function">Spectrum</a> <a id="595" href="synthetic-homotopy-theory.spectra.html#595" class="Bound">l</a> <a id="597" class="Symbol">=</a>
  <a id="601" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="603" class="Symbol">(</a><a id="604" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="606" class="Symbol">→</a> <a id="608" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="621" href="synthetic-homotopy-theory.spectra.html#595" class="Bound">l</a><a id="622" class="Symbol">)</a> <a id="624" class="Symbol">(λ</a> <a id="627" href="synthetic-homotopy-theory.spectra.html#627" class="Bound">A</a> <a id="629" class="Symbol">→</a> <a id="631" class="Symbol">(</a><a id="632" href="synthetic-homotopy-theory.spectra.html#632" class="Bound">n</a> <a id="634" class="Symbol">:</a> <a id="636" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a><a id="637" class="Symbol">)</a> <a id="639" class="Symbol">→</a> <a id="641" href="synthetic-homotopy-theory.spectra.html#627" class="Bound">A</a> <a id="643" href="synthetic-homotopy-theory.spectra.html#632" class="Bound">n</a> <a id="645" href="structured-types.pointed-equivalences.html#7578" class="Function Operator">≃*</a> <a id="648" href="synthetic-homotopy-theory.loop-spaces.html#1221" class="Function">Ω</a> <a id="650" class="Symbol">(</a><a id="651" href="synthetic-homotopy-theory.spectra.html#627" class="Bound">A</a> <a id="653" class="Symbol">(</a><a id="654" href="elementary-number-theory.natural-numbers.html#1564" class="InductiveConstructor">succ-ℕ</a> <a id="661" href="synthetic-homotopy-theory.spectra.html#632" class="Bound">n</a><a id="662" class="Symbol">)))</a>
</pre>