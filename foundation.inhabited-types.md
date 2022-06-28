---
title: Inhabited types
---

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a> <a id="118" class="Keyword">where</a>

<a id="125" class="Keyword">open</a> <a id="130" class="Keyword">import</a> <a id="137" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="169" class="Keyword">open</a> <a id="174" class="Keyword">import</a> <a id="181" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="218" class="Keyword">open</a> <a id="223" class="Keyword">import</a> <a id="230" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

Inhabited types are types equipped with an element of its propositional truncation.

## Definition

<pre class="Agda"><a id="Inhabited-Type"></a><a id="379" href="foundation.inhabited-types.html#379" class="Function">Inhabited-Type</a> <a id="394" class="Symbol">:</a> <a id="396" class="Symbol">(</a><a id="397" href="foundation.inhabited-types.html#397" class="Bound">l</a> <a id="399" class="Symbol">:</a> <a id="401" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="406" class="Symbol">)</a> <a id="408" class="Symbol">→</a> <a id="410" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="413" class="Symbol">(</a><a id="414" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="419" href="foundation.inhabited-types.html#397" class="Bound">l</a><a id="420" class="Symbol">)</a>
<a id="422" href="foundation.inhabited-types.html#379" class="Function">Inhabited-Type</a> <a id="437" href="foundation.inhabited-types.html#437" class="Bound">l</a> <a id="439" class="Symbol">=</a> <a id="441" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="443" class="Symbol">(</a><a id="444" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="447" href="foundation.inhabited-types.html#437" class="Bound">l</a><a id="448" class="Symbol">)</a> <a id="450" href="foundation.propositional-truncations.html#2034" class="Function">type-trunc-Prop</a>

<a id="467" class="Keyword">module</a> <a id="474" href="foundation.inhabited-types.html#474" class="Module">_</a>
  <a id="478" class="Symbol">{</a><a id="479" href="foundation.inhabited-types.html#479" class="Bound">l</a> <a id="481" class="Symbol">:</a> <a id="483" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="488" class="Symbol">}</a> <a id="490" class="Symbol">(</a><a id="491" href="foundation.inhabited-types.html#491" class="Bound">X</a> <a id="493" class="Symbol">:</a> <a id="495" href="foundation.inhabited-types.html#379" class="Function">Inhabited-Type</a> <a id="510" href="foundation.inhabited-types.html#479" class="Bound">l</a><a id="511" class="Symbol">)</a>
  <a id="515" class="Keyword">where</a>

  <a id="524" href="foundation.inhabited-types.html#524" class="Function">type-Inhabited-Type</a> <a id="544" class="Symbol">:</a> <a id="546" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="549" href="foundation.inhabited-types.html#479" class="Bound">l</a>
  <a id="553" href="foundation.inhabited-types.html#524" class="Function">type-Inhabited-Type</a> <a id="573" class="Symbol">=</a> <a id="575" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="579" href="foundation.inhabited-types.html#491" class="Bound">X</a>

  <a id="584" href="foundation.inhabited-types.html#584" class="Function">is-inhabited-type-Inhabited-Type</a> <a id="617" class="Symbol">:</a> <a id="619" href="foundation.propositional-truncations.html#2034" class="Function">type-trunc-Prop</a> <a id="635" href="foundation.inhabited-types.html#524" class="Function">type-Inhabited-Type</a>
  <a id="657" href="foundation.inhabited-types.html#584" class="Function">is-inhabited-type-Inhabited-Type</a> <a id="690" class="Symbol">=</a> <a id="692" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="696" href="foundation.inhabited-types.html#491" class="Bound">X</a>
</pre>