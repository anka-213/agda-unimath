---
title: Impredicative universes
---

<pre class="Agda"><a id="49" class="Symbol">{-#</a> <a id="53" class="Keyword">OPTIONS</a> <a id="61" class="Pragma">--without-K</a> <a id="73" class="Pragma">--exact-split</a> <a id="87" class="Symbol">#-}</a>

<a id="92" class="Keyword">module</a> <a id="99" href="foundation.impredicative-universes.html" class="Module">foundation.impredicative-universes</a> <a id="134" class="Keyword">where</a>

<a id="141" class="Keyword">open</a> <a id="146" class="Keyword">import</a> <a id="153" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="177" class="Keyword">open</a> <a id="182" class="Keyword">import</a> <a id="189" href="foundation.small-types.html" class="Module">foundation.small-types</a>
<a id="212" class="Keyword">open</a> <a id="217" class="Keyword">import</a> <a id="224" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

A universe `U` is impredicative if the type of propositions in `U` is `U`-small.

## Definition

<pre class="Agda"><a id="is-impredicative-UU"></a><a id="370" href="foundation.impredicative-universes.html#370" class="Function">is-impredicative-UU</a> <a id="390" class="Symbol">:</a> <a id="392" class="Symbol">(</a><a id="393" href="foundation.impredicative-universes.html#393" class="Bound">l</a> <a id="395" class="Symbol">:</a> <a id="397" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="402" class="Symbol">)</a> <a id="404" class="Symbol">→</a> <a id="406" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="409" class="Symbol">(</a><a id="410" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="415" href="foundation.impredicative-universes.html#393" class="Bound">l</a><a id="416" class="Symbol">)</a>
<a id="418" href="foundation.impredicative-universes.html#370" class="Function">is-impredicative-UU</a> <a id="438" href="foundation.impredicative-universes.html#438" class="Bound">l</a> <a id="440" class="Symbol">=</a> <a id="442" href="foundation.small-types.html#1607" class="Function">is-small</a> <a id="451" href="foundation.impredicative-universes.html#438" class="Bound">l</a> <a id="453" class="Symbol">(</a><a id="454" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="462" href="foundation.impredicative-universes.html#438" class="Bound">l</a><a id="463" class="Symbol">)</a>
</pre>