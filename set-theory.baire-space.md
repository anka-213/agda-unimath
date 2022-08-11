---
title: Baire space
---

<pre class="Agda"><a id="37" class="Symbol">{-#</a> <a id="41" class="Keyword">OPTIONS</a> <a id="49" class="Pragma">--without-K</a> <a id="61" class="Pragma">--exact-split</a> <a id="75" class="Symbol">#-}</a>

<a id="80" class="Keyword">module</a> <a id="87" href="set-theory.baire-space.html" class="Module">set-theory.baire-space</a> <a id="110" class="Keyword">where</a>

<a id="117" class="Keyword">open</a> <a id="122" class="Keyword">import</a> <a id="129" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="171" class="Keyword">open</a> <a id="176" class="Keyword">import</a> <a id="183" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

The Baire space is the type of functions `ℕ → ℕ`.

## Definition

<pre class="Agda"><a id="baire-space"></a><a id="298" href="set-theory.baire-space.html#298" class="Function">baire-space</a> <a id="310" class="Symbol">:</a> <a id="312" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="315" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="321" href="set-theory.baire-space.html#298" class="Function">baire-space</a> <a id="333" class="Symbol">=</a> <a id="335" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="337" class="Symbol">→</a> <a id="339" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a>
</pre>