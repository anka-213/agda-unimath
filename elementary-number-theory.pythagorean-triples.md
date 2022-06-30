---
title: Pythagorean triples
---

<pre class="Agda"><a id="45" class="Symbol">{-#</a> <a id="49" class="Keyword">OPTIONS</a> <a id="57" class="Pragma">--without-K</a> <a id="69" class="Pragma">--exact-split</a> <a id="83" class="Symbol">#-}</a>

<a id="88" class="Keyword">module</a> <a id="95" href="elementary-number-theory.pythagorean-triples.html" class="Module">elementary-number-theory.pythagorean-triples</a> <a id="140" class="Keyword">where</a>

<a id="147" class="Keyword">open</a> <a id="152" class="Keyword">import</a> <a id="159" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="209" class="Keyword">open</a> <a id="214" class="Keyword">import</a> <a id="221" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a>
<a id="277" class="Keyword">open</a> <a id="282" class="Keyword">import</a> <a id="289" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="331" class="Keyword">open</a> <a id="336" class="Keyword">import</a> <a id="343" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="369" class="Keyword">open</a> <a id="374" class="Keyword">import</a> <a id="381" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

A Pythagorean triple is a triple `(a,b,c)` of natural numbers such that `a² + b² = c²`.

## Definition

<pre class="Agda"><a id="is-pythagorean-triple"></a><a id="534" href="elementary-number-theory.pythagorean-triples.html#534" class="Function">is-pythagorean-triple</a> <a id="556" class="Symbol">:</a> <a id="558" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a> <a id="560" class="Symbol">→</a> <a id="562" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a> <a id="564" class="Symbol">→</a> <a id="566" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a> <a id="568" class="Symbol">→</a> <a id="570" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="573" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="579" href="elementary-number-theory.pythagorean-triples.html#534" class="Function">is-pythagorean-triple</a> <a id="601" href="elementary-number-theory.pythagorean-triples.html#601" class="Bound">a</a> <a id="603" href="elementary-number-theory.pythagorean-triples.html#603" class="Bound">b</a> <a id="605" href="elementary-number-theory.pythagorean-triples.html#605" class="Bound">c</a> <a id="607" class="Symbol">=</a> <a id="609" class="Symbol">(</a><a id="610" href="elementary-number-theory.addition-natural-numbers.html#1164" class="Function">add-ℕ</a> <a id="616" class="Symbol">(</a><a id="617" href="elementary-number-theory.multiplication-natural-numbers.html#1666" class="Function">square-ℕ</a> <a id="626" href="elementary-number-theory.pythagorean-triples.html#601" class="Bound">a</a><a id="627" class="Symbol">)</a> <a id="629" class="Symbol">(</a><a id="630" href="elementary-number-theory.multiplication-natural-numbers.html#1666" class="Function">square-ℕ</a> <a id="639" href="elementary-number-theory.pythagorean-triples.html#603" class="Bound">b</a><a id="640" class="Symbol">)</a> <a id="642" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="644" href="elementary-number-theory.multiplication-natural-numbers.html#1666" class="Function">square-ℕ</a> <a id="653" href="elementary-number-theory.pythagorean-triples.html#605" class="Bound">c</a><a id="654" class="Symbol">)</a>
</pre>