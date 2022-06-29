---
title: Relatively prime integers
---

<pre class="Agda"><a id="51" class="Symbol">{-#</a> <a id="55" class="Keyword">OPTIONS</a> <a id="63" class="Pragma">--without-K</a> <a id="75" class="Pragma">--exact-split</a> <a id="89" class="Symbol">#-}</a>

<a id="94" class="Keyword">module</a> <a id="101" href="elementary-number-theory.relatively-prime-integers.html" class="Module">elementary-number-theory.relatively-prime-integers</a> <a id="152" class="Keyword">where</a>

<a id="159" class="Keyword">open</a> <a id="164" class="Keyword">import</a> <a id="171" href="elementary-number-theory.greatest-common-divisor-integers.html" class="Module">elementary-number-theory.greatest-common-divisor-integers</a> <a id="229" class="Keyword">using</a>
  <a id="237" class="Symbol">(</a> <a id="239" href="elementary-number-theory.greatest-common-divisor-integers.html#4623" class="Function">gcd-ℤ</a><a id="244" class="Symbol">)</a>
<a id="246" class="Keyword">open</a> <a id="251" class="Keyword">import</a> <a id="258" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a> <a id="292" class="Keyword">using</a> <a id="298" class="Symbol">(</a><a id="299" href="elementary-number-theory.integers.html#1910" class="Function">ℤ</a><a id="300" class="Symbol">;</a> <a id="302" href="elementary-number-theory.integers.html#2438" class="Function">is-one-ℤ</a><a id="310" class="Symbol">)</a>

<a id="313" class="Keyword">open</a> <a id="318" class="Keyword">import</a> <a id="325" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="352" class="Keyword">using</a> <a id="358" class="Symbol">(</a><a id="359" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="361" class="Symbol">;</a> <a id="363" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="368" class="Symbol">)</a>
</pre>
## Idea

Two integers are said to be relatively prime if their greatest common divisor is 1.

## Definition

<pre class="Agda"><a id="is-relative-prime-ℤ"></a><a id="492" href="elementary-number-theory.relatively-prime-integers.html#492" class="Function">is-relative-prime-ℤ</a> <a id="512" class="Symbol">:</a> <a id="514" href="elementary-number-theory.integers.html#1910" class="Function">ℤ</a> <a id="516" class="Symbol">→</a> <a id="518" href="elementary-number-theory.integers.html#1910" class="Function">ℤ</a> <a id="520" class="Symbol">→</a> <a id="522" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="525" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="531" href="elementary-number-theory.relatively-prime-integers.html#492" class="Function">is-relative-prime-ℤ</a> <a id="551" href="elementary-number-theory.relatively-prime-integers.html#551" class="Bound">x</a> <a id="553" href="elementary-number-theory.relatively-prime-integers.html#553" class="Bound">y</a> <a id="555" class="Symbol">=</a> <a id="557" href="elementary-number-theory.integers.html#2438" class="Function">is-one-ℤ</a> <a id="566" class="Symbol">(</a><a id="567" href="elementary-number-theory.greatest-common-divisor-integers.html#4623" class="Function">gcd-ℤ</a> <a id="573" href="elementary-number-theory.relatively-prime-integers.html#551" class="Bound">x</a> <a id="575" href="elementary-number-theory.relatively-prime-integers.html#553" class="Bound">y</a><a id="576" class="Symbol">)</a>
</pre>
## Properties
