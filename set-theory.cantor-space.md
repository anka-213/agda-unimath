---
title: Cantor space
---

<pre class="Agda"><a id="38" class="Symbol">{-#</a> <a id="42" class="Keyword">OPTIONS</a> <a id="50" class="Pragma">--without-K</a> <a id="62" class="Pragma">--exact-split</a> <a id="76" class="Symbol">#-}</a>

<a id="81" class="Keyword">module</a> <a id="88" href="set-theory.cantor-space.html" class="Module">set-theory.cantor-space</a> <a id="112" class="Keyword">where</a>

<a id="119" class="Keyword">open</a> <a id="124" class="Keyword">import</a> <a id="131" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="173" class="Keyword">open</a> <a id="178" class="Keyword">import</a> <a id="185" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="213" class="Keyword">open</a> <a id="218" class="Keyword">import</a> <a id="225" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Idea

The Cantor space is the type of functions `ℕ → Fin 2`.

## Definition

<pre class="Agda"><a id="cantor-space"></a><a id="364" href="set-theory.cantor-space.html#364" class="Function">cantor-space</a> <a id="377" class="Symbol">:</a> <a id="379" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="382" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="388" href="set-theory.cantor-space.html#364" class="Function">cantor-space</a> <a id="401" class="Symbol">=</a> <a id="403" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a> <a id="405" class="Symbol">→</a> <a id="407" href="univalent-combinatorics.standard-finite-types.html#2149" class="Function">Fin</a> <a id="411" class="Number">2</a>
</pre>