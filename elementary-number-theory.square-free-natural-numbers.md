---
title: Square-free natural numbers
---

<pre class="Agda"><a id="53" class="Symbol">{-#</a> <a id="57" class="Keyword">OPTIONS</a> <a id="65" class="Pragma">--without-K</a> <a id="77" class="Pragma">--exact-split</a> <a id="91" class="Symbol">#-}</a>

<a id="96" class="Keyword">module</a> <a id="103" href="elementary-number-theory.square-free-natural-numbers.html" class="Module">elementary-number-theory.square-free-natural-numbers</a> <a id="156" class="Keyword">where</a>

<a id="163" class="Keyword">open</a> <a id="168" class="Keyword">import</a> <a id="175" href="elementary-number-theory.divisibility-natural-numbers.html" class="Module">elementary-number-theory.divisibility-natural-numbers</a> <a id="229" class="Keyword">using</a> <a id="235" class="Symbol">(</a><a id="236" href="elementary-number-theory.divisibility-natural-numbers.html#1608" class="Function">div-ℕ</a><a id="241" class="Symbol">)</a>
<a id="243" class="Keyword">open</a> <a id="248" class="Keyword">import</a> <a id="255" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="296" class="Keyword">using</a> <a id="302" class="Symbol">(</a><a id="303" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a><a id="304" class="Symbol">;</a> <a id="306" href="elementary-number-theory.natural-numbers.html#2073" class="Function">is-one-ℕ</a><a id="314" class="Symbol">)</a>
<a id="316" class="Keyword">open</a> <a id="321" class="Keyword">import</a> <a id="328" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a> <a id="384" class="Keyword">using</a>
  <a id="392" class="Symbol">(</a> <a id="394" href="elementary-number-theory.multiplication-natural-numbers.html#1594" class="Function">square-ℕ</a><a id="402" class="Symbol">)</a>

<a id="405" class="Keyword">open</a> <a id="410" class="Keyword">import</a> <a id="417" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="444" class="Keyword">using</a> <a id="450" class="Symbol">(</a><a id="451" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="453" class="Symbol">;</a> <a id="455" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="460" class="Symbol">)</a>
</pre>
## Idea

A natural number `n` is said to be square-free if `x² | n ⇒ x = 1` for any natural number `x`.

## Definition

<pre class="Agda"><a id="is-square-free-ℕ"></a><a id="595" href="elementary-number-theory.square-free-natural-numbers.html#595" class="Function">is-square-free-ℕ</a> <a id="612" class="Symbol">:</a> <a id="614" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="616" class="Symbol">→</a> <a id="618" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="621" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="627" href="elementary-number-theory.square-free-natural-numbers.html#595" class="Function">is-square-free-ℕ</a> <a id="644" href="elementary-number-theory.square-free-natural-numbers.html#644" class="Bound">n</a> <a id="646" class="Symbol">=</a> <a id="648" class="Symbol">(</a><a id="649" href="elementary-number-theory.square-free-natural-numbers.html#649" class="Bound">x</a> <a id="651" class="Symbol">:</a> <a id="653" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a><a id="654" class="Symbol">)</a> <a id="656" class="Symbol">→</a> <a id="658" href="elementary-number-theory.divisibility-natural-numbers.html#1608" class="Function">div-ℕ</a> <a id="664" class="Symbol">(</a><a id="665" href="elementary-number-theory.multiplication-natural-numbers.html#1594" class="Function">square-ℕ</a> <a id="674" href="elementary-number-theory.square-free-natural-numbers.html#649" class="Bound">x</a><a id="675" class="Symbol">)</a> <a id="677" href="elementary-number-theory.square-free-natural-numbers.html#644" class="Bound">n</a> <a id="679" class="Symbol">→</a> <a id="681" href="elementary-number-theory.natural-numbers.html#2073" class="Function">is-one-ℕ</a> <a id="690" href="elementary-number-theory.square-free-natural-numbers.html#649" class="Bound">x</a>
</pre>