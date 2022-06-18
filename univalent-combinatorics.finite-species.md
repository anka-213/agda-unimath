---
title: Finite species
---

<pre class="Agda"><a id="40" class="Symbol">{-#</a> <a id="44" class="Keyword">OPTIONS</a> <a id="52" class="Pragma">--without-K</a> <a id="64" class="Pragma">--exact-split</a> <a id="78" class="Symbol">#-}</a>

<a id="83" class="Keyword">module</a> <a id="90" href="univalent-combinatorics.finite-species.html" class="Module">univalent-combinatorics.finite-species</a> <a id="129" class="Keyword">where</a>

<a id="136" class="Keyword">open</a> <a id="141" class="Keyword">import</a> <a id="148" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="176" class="Keyword">open</a> <a id="181" class="Keyword">import</a> <a id="188" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Definition

<pre class="Agda"><a id="finite-species"></a><a id="253" href="univalent-combinatorics.finite-species.html#253" class="Function">finite-species</a> <a id="268" class="Symbol">:</a> <a id="270" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="273" class="Symbol">(</a><a id="274" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="279" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="284" class="Symbol">)</a>
<a id="286" href="univalent-combinatorics.finite-species.html#253" class="Function">finite-species</a> <a id="301" class="Symbol">=</a> <a id="303" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a> <a id="305" class="Symbol">→</a> <a id="307" href="univalent-combinatorics.finite-types.html#4455" class="Function">𝔽</a>
</pre>