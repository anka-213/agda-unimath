---
title: Prespectra
---

<pre class="Agda"><a id="36" class="Symbol">{-#</a> <a id="40" class="Keyword">OPTIONS</a> <a id="48" class="Pragma">--without-K</a> <a id="60" class="Pragma">--exact-split</a> <a id="74" class="Symbol">#-}</a>

<a id="79" class="Keyword">module</a> <a id="86" href="synthetic-homotopy-theory.prespectra.html" class="Module">synthetic-homotopy-theory.prespectra</a> <a id="123" class="Keyword">where</a>

<a id="130" class="Keyword">open</a> <a id="135" class="Keyword">import</a> <a id="142" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="184" class="Keyword">open</a> <a id="189" class="Keyword">import</a> <a id="196" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="228" class="Keyword">open</a> <a id="233" class="Keyword">import</a> <a id="240" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="268" class="Keyword">open</a> <a id="273" class="Keyword">import</a> <a id="280" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="310" class="Keyword">open</a> <a id="315" class="Keyword">import</a> <a id="322" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>

<a id="354" class="Keyword">open</a> <a id="359" class="Keyword">import</a> <a id="366" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a>
</pre>
## Idea

A prespectrum is a sequence of pointed types `A n` equipped with pointed maps `ε : A n →* Ω (A (n+1))`.

## Definition

<pre class="Agda"><a id="Prespectrum"></a><a id="546" href="synthetic-homotopy-theory.prespectra.html#546" class="Function">Prespectrum</a> <a id="558" class="Symbol">:</a> <a id="560" class="Symbol">(</a><a id="561" href="synthetic-homotopy-theory.prespectra.html#561" class="Bound">l</a> <a id="563" class="Symbol">:</a> <a id="565" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="570" class="Symbol">)</a> <a id="572" class="Symbol">→</a> <a id="574" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="577" class="Symbol">(</a><a id="578" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="583" href="synthetic-homotopy-theory.prespectra.html#561" class="Bound">l</a><a id="584" class="Symbol">)</a>
<a id="586" href="synthetic-homotopy-theory.prespectra.html#546" class="Function">Prespectrum</a> <a id="598" href="synthetic-homotopy-theory.prespectra.html#598" class="Bound">l</a> <a id="600" class="Symbol">=</a>
  <a id="604" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="606" class="Symbol">(</a><a id="607" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="609" class="Symbol">→</a> <a id="611" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="624" href="synthetic-homotopy-theory.prespectra.html#598" class="Bound">l</a><a id="625" class="Symbol">)</a> <a id="627" class="Symbol">(λ</a> <a id="630" href="synthetic-homotopy-theory.prespectra.html#630" class="Bound">A</a> <a id="632" class="Symbol">→</a> <a id="634" class="Symbol">(</a><a id="635" href="synthetic-homotopy-theory.prespectra.html#635" class="Bound">n</a> <a id="637" class="Symbol">:</a> <a id="639" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a><a id="640" class="Symbol">)</a> <a id="642" class="Symbol">→</a> <a id="644" href="synthetic-homotopy-theory.prespectra.html#630" class="Bound">A</a> <a id="646" href="synthetic-homotopy-theory.prespectra.html#635" class="Bound">n</a> <a id="648" href="structured-types.pointed-maps.html#967" class="Function Operator">→*</a> <a id="651" href="synthetic-homotopy-theory.loop-spaces.html#1221" class="Function">Ω</a> <a id="653" class="Symbol">(</a><a id="654" href="synthetic-homotopy-theory.prespectra.html#630" class="Bound">A</a> <a id="656" class="Symbol">(</a><a id="657" href="elementary-number-theory.natural-numbers.html#1564" class="InductiveConstructor">succ-ℕ</a> <a id="664" href="synthetic-homotopy-theory.prespectra.html#635" class="Bound">n</a><a id="665" class="Symbol">)))</a>
</pre>