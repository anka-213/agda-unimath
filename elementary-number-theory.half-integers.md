---
title: The half-integers
---

<pre class="Agda"><a id="43" class="Keyword">module</a> <a id="50" href="elementary-number-theory.half-integers.html" class="Module">elementary-number-theory.half-integers</a> <a id="89" class="Keyword">where</a>

<a id="96" class="Keyword">open</a> <a id="101" class="Keyword">import</a> <a id="108" href="elementary-number-theory.addition-integers.html" class="Module">elementary-number-theory.addition-integers</a>
<a id="151" class="Keyword">open</a> <a id="156" class="Keyword">import</a> <a id="163" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>

<a id="198" class="Keyword">open</a> <a id="203" class="Keyword">import</a> <a id="210" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="237" class="Keyword">open</a> <a id="242" class="Keyword">import</a> <a id="249" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

The **half-integers** are the numbers of the form `x + ½`, where `x : ℤ`.

## Definition

### The half-integers

<pre class="Agda"><a id="ℤ+½"></a><a id="411" href="elementary-number-theory.half-integers.html#411" class="Function">ℤ+½</a> <a id="415" class="Symbol">:</a> <a id="417" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="420" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="426" href="elementary-number-theory.half-integers.html#411" class="Function">ℤ+½</a> <a id="430" class="Symbol">=</a> <a id="432" href="elementary-number-theory.integers.html#2078" class="Function">ℤ</a>
</pre>
### The disjoint union of the half-integers with the integers

<pre class="Agda"><a id="½ℤ"></a><a id="510" href="elementary-number-theory.half-integers.html#510" class="Function">½ℤ</a> <a id="513" class="Symbol">:</a> <a id="515" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="518" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="524" href="elementary-number-theory.half-integers.html#510" class="Function">½ℤ</a> <a id="527" class="Symbol">=</a> <a id="529" href="elementary-number-theory.half-integers.html#411" class="Function">ℤ+½</a> <a id="533" href="foundation.coproduct-types.html#1182" class="Datatype Operator">+</a> <a id="535" href="elementary-number-theory.integers.html#2078" class="Function">ℤ</a>
</pre>
### The zero element of `½ℤ`

<pre class="Agda"><a id="zero-½ℤ"></a><a id="580" href="elementary-number-theory.half-integers.html#580" class="Function">zero-½ℤ</a> <a id="588" class="Symbol">:</a> <a id="590" href="elementary-number-theory.half-integers.html#510" class="Function">½ℤ</a>
<a id="593" href="elementary-number-theory.half-integers.html#580" class="Function">zero-½ℤ</a> <a id="601" class="Symbol">=</a> <a id="603" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="607" href="elementary-number-theory.integers.html#2321" class="Function">zero-ℤ</a>
</pre>
### Addition on `½ℤ`

<pre class="Agda"><a id="add-½ℤ"></a><a id="649" href="elementary-number-theory.half-integers.html#649" class="Function">add-½ℤ</a> <a id="656" class="Symbol">:</a> <a id="658" href="elementary-number-theory.half-integers.html#510" class="Function">½ℤ</a> <a id="661" class="Symbol">→</a> <a id="663" href="elementary-number-theory.half-integers.html#510" class="Function">½ℤ</a> <a id="666" class="Symbol">→</a> <a id="668" href="elementary-number-theory.half-integers.html#510" class="Function">½ℤ</a>
<a id="671" href="elementary-number-theory.half-integers.html#649" class="Function">add-½ℤ</a> <a id="678" class="Symbol">(</a><a id="679" href="foundation.coproduct-types.html#1250" class="InductiveConstructor">inl</a> <a id="683" href="elementary-number-theory.half-integers.html#683" class="Bound">x</a><a id="684" class="Symbol">)</a> <a id="686" class="Symbol">(</a><a id="687" href="foundation.coproduct-types.html#1250" class="InductiveConstructor">inl</a> <a id="691" href="elementary-number-theory.half-integers.html#691" class="Bound">y</a><a id="692" class="Symbol">)</a> <a id="694" class="Symbol">=</a> <a id="696" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="700" class="Symbol">(</a><a id="701" href="elementary-number-theory.integers.html#3662" class="Function">succ-ℤ</a> <a id="708" class="Symbol">(</a><a id="709" href="elementary-number-theory.addition-integers.html#1505" class="Function">add-ℤ</a> <a id="715" href="elementary-number-theory.half-integers.html#683" class="Bound">x</a> <a id="717" href="elementary-number-theory.half-integers.html#691" class="Bound">y</a><a id="718" class="Symbol">))</a>
<a id="721" href="elementary-number-theory.half-integers.html#649" class="Function">add-½ℤ</a> <a id="728" class="Symbol">(</a><a id="729" href="foundation.coproduct-types.html#1250" class="InductiveConstructor">inl</a> <a id="733" href="elementary-number-theory.half-integers.html#733" class="Bound">x</a><a id="734" class="Symbol">)</a> <a id="736" class="Symbol">(</a><a id="737" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="741" href="elementary-number-theory.half-integers.html#741" class="Bound">y</a><a id="742" class="Symbol">)</a> <a id="744" class="Symbol">=</a> <a id="746" href="foundation.coproduct-types.html#1250" class="InductiveConstructor">inl</a> <a id="750" class="Symbol">(</a><a id="751" href="elementary-number-theory.addition-integers.html#1505" class="Function">add-ℤ</a> <a id="757" href="elementary-number-theory.half-integers.html#733" class="Bound">x</a> <a id="759" href="elementary-number-theory.half-integers.html#741" class="Bound">y</a><a id="760" class="Symbol">)</a>
<a id="762" href="elementary-number-theory.half-integers.html#649" class="Function">add-½ℤ</a> <a id="769" class="Symbol">(</a><a id="770" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="774" href="elementary-number-theory.half-integers.html#774" class="Bound">x</a><a id="775" class="Symbol">)</a> <a id="777" class="Symbol">(</a><a id="778" href="foundation.coproduct-types.html#1250" class="InductiveConstructor">inl</a> <a id="782" href="elementary-number-theory.half-integers.html#782" class="Bound">y</a><a id="783" class="Symbol">)</a> <a id="785" class="Symbol">=</a> <a id="787" href="foundation.coproduct-types.html#1250" class="InductiveConstructor">inl</a> <a id="791" class="Symbol">(</a><a id="792" href="elementary-number-theory.addition-integers.html#1505" class="Function">add-ℤ</a> <a id="798" href="elementary-number-theory.half-integers.html#774" class="Bound">x</a> <a id="800" href="elementary-number-theory.half-integers.html#782" class="Bound">y</a><a id="801" class="Symbol">)</a>
<a id="803" href="elementary-number-theory.half-integers.html#649" class="Function">add-½ℤ</a> <a id="810" class="Symbol">(</a><a id="811" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="815" href="elementary-number-theory.half-integers.html#815" class="Bound">x</a><a id="816" class="Symbol">)</a> <a id="818" class="Symbol">(</a><a id="819" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="823" href="elementary-number-theory.half-integers.html#823" class="Bound">y</a><a id="824" class="Symbol">)</a> <a id="826" class="Symbol">=</a> <a id="828" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="832" class="Symbol">(</a><a id="833" href="elementary-number-theory.addition-integers.html#1505" class="Function">add-ℤ</a> <a id="839" href="elementary-number-theory.half-integers.html#815" class="Bound">x</a> <a id="841" href="elementary-number-theory.half-integers.html#823" class="Bound">y</a><a id="842" class="Symbol">)</a>
</pre>