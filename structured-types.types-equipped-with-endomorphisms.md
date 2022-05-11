---
title: Types equipped with endomorphisms
---

<pre class="Agda"><a id="59" class="Symbol">{-#</a> <a id="63" class="Keyword">OPTIONS</a> <a id="71" class="Pragma">--without-K</a> <a id="83" class="Pragma">--exact-split</a> <a id="97" class="Symbol">#-}</a>

<a id="102" class="Keyword">module</a> <a id="109" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a> <a id="160" class="Keyword">where</a>

<a id="167" class="Keyword">open</a> <a id="172" class="Keyword">import</a> <a id="179" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="211" class="Keyword">open</a> <a id="216" class="Keyword">import</a> <a id="223" href="foundation.endomorphisms.html" class="Module">foundation.endomorphisms</a>
<a id="248" class="Keyword">open</a> <a id="253" class="Keyword">import</a> <a id="260" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

A type equipped with an endomorphism consists of a type `A` equipped with a map `A → A`.

## Definitions

### Types equipped with endomorphisms

<pre class="Agda"><a id="Endo"></a><a id="454" href="structured-types.types-equipped-with-endomorphisms.html#454" class="Function">Endo</a> <a id="459" class="Symbol">:</a> <a id="461" class="Symbol">(</a><a id="462" href="structured-types.types-equipped-with-endomorphisms.html#462" class="Bound">l</a> <a id="464" class="Symbol">:</a> <a id="466" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="471" class="Symbol">)</a> <a id="473" class="Symbol">→</a> <a id="475" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="478" class="Symbol">(</a><a id="479" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="484" href="structured-types.types-equipped-with-endomorphisms.html#462" class="Bound">l</a><a id="485" class="Symbol">)</a>
<a id="487" href="structured-types.types-equipped-with-endomorphisms.html#454" class="Function">Endo</a> <a id="492" href="structured-types.types-equipped-with-endomorphisms.html#492" class="Bound">l</a> <a id="494" class="Symbol">=</a> <a id="496" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="498" class="Symbol">(</a><a id="499" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="502" href="structured-types.types-equipped-with-endomorphisms.html#492" class="Bound">l</a><a id="503" class="Symbol">)</a> <a id="505" href="foundation.endomorphisms.html#792" class="Function">endo</a>

<a id="511" class="Keyword">module</a> <a id="518" href="structured-types.types-equipped-with-endomorphisms.html#518" class="Module">_</a>
  <a id="522" class="Symbol">{</a><a id="523" href="structured-types.types-equipped-with-endomorphisms.html#523" class="Bound">l</a> <a id="525" class="Symbol">:</a> <a id="527" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="532" class="Symbol">}</a> <a id="534" class="Symbol">(</a><a id="535" href="structured-types.types-equipped-with-endomorphisms.html#535" class="Bound">X</a> <a id="537" class="Symbol">:</a> <a id="539" href="structured-types.types-equipped-with-endomorphisms.html#454" class="Function">Endo</a> <a id="544" href="structured-types.types-equipped-with-endomorphisms.html#523" class="Bound">l</a><a id="545" class="Symbol">)</a>
  <a id="549" class="Keyword">where</a>

  <a id="558" href="structured-types.types-equipped-with-endomorphisms.html#558" class="Function">type-Endo</a> <a id="568" class="Symbol">:</a> <a id="570" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="573" href="structured-types.types-equipped-with-endomorphisms.html#523" class="Bound">l</a>
  <a id="577" href="structured-types.types-equipped-with-endomorphisms.html#558" class="Function">type-Endo</a> <a id="587" class="Symbol">=</a> <a id="589" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="593" href="structured-types.types-equipped-with-endomorphisms.html#535" class="Bound">X</a>

  <a id="598" href="structured-types.types-equipped-with-endomorphisms.html#598" class="Function">endomorphism-Endo</a> <a id="616" class="Symbol">:</a> <a id="618" href="structured-types.types-equipped-with-endomorphisms.html#558" class="Function">type-Endo</a> <a id="628" class="Symbol">→</a> <a id="630" href="structured-types.types-equipped-with-endomorphisms.html#558" class="Function">type-Endo</a>
  <a id="642" href="structured-types.types-equipped-with-endomorphisms.html#598" class="Function">endomorphism-Endo</a> <a id="660" class="Symbol">=</a> <a id="662" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="666" href="structured-types.types-equipped-with-endomorphisms.html#535" class="Bound">X</a>
</pre>