---
title: Inhabited types
---

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="foundation.inhabited-types.html" class="Module">foundation.inhabited-types</a> <a id="118" class="Keyword">where</a>

<a id="125" class="Keyword">open</a> <a id="130" class="Keyword">import</a> <a id="137" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="169" class="Keyword">open</a> <a id="174" class="Keyword">import</a> <a id="181" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="218" class="Keyword">open</a> <a id="223" class="Keyword">import</a> <a id="230" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="254" class="Keyword">open</a> <a id="259" class="Keyword">import</a> <a id="266" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

Inhabited types are types equipped with an element of its propositional truncation.

## Definition

<pre class="Agda"><a id="is-inhabited-Prop"></a><a id="415" href="foundation.inhabited-types.html#415" class="Function">is-inhabited-Prop</a> <a id="433" class="Symbol">:</a> <a id="435" class="Symbol">{</a><a id="436" href="foundation.inhabited-types.html#436" class="Bound">l</a> <a id="438" class="Symbol">:</a> <a id="440" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="445" class="Symbol">}</a> <a id="447" class="Symbol">→</a> <a id="449" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="452" href="foundation.inhabited-types.html#436" class="Bound">l</a> <a id="454" class="Symbol">→</a> <a id="456" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="464" href="foundation.inhabited-types.html#436" class="Bound">l</a>
<a id="466" href="foundation.inhabited-types.html#415" class="Function">is-inhabited-Prop</a> <a id="484" href="foundation.inhabited-types.html#484" class="Bound">X</a> <a id="486" class="Symbol">=</a> <a id="488" href="foundation.propositional-truncations.html#2707" class="Function">trunc-Prop</a> <a id="499" href="foundation.inhabited-types.html#484" class="Bound">X</a>

<a id="is-inhabited"></a><a id="502" href="foundation.inhabited-types.html#502" class="Function">is-inhabited</a> <a id="515" class="Symbol">:</a> <a id="517" class="Symbol">{</a><a id="518" href="foundation.inhabited-types.html#518" class="Bound">l</a> <a id="520" class="Symbol">:</a> <a id="522" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="527" class="Symbol">}</a> <a id="529" class="Symbol">→</a> <a id="531" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="534" href="foundation.inhabited-types.html#518" class="Bound">l</a> <a id="536" class="Symbol">→</a> <a id="538" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="541" href="foundation.inhabited-types.html#518" class="Bound">l</a>
<a id="543" href="foundation.inhabited-types.html#502" class="Function">is-inhabited</a> <a id="556" href="foundation.inhabited-types.html#556" class="Bound">X</a> <a id="558" class="Symbol">=</a> <a id="560" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="570" class="Symbol">(</a><a id="571" href="foundation.inhabited-types.html#415" class="Function">is-inhabited-Prop</a> <a id="589" href="foundation.inhabited-types.html#556" class="Bound">X</a><a id="590" class="Symbol">)</a>

<a id="Inhabited-Type"></a><a id="593" href="foundation.inhabited-types.html#593" class="Function">Inhabited-Type</a> <a id="608" class="Symbol">:</a> <a id="610" class="Symbol">(</a><a id="611" href="foundation.inhabited-types.html#611" class="Bound">l</a> <a id="613" class="Symbol">:</a> <a id="615" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="620" class="Symbol">)</a> <a id="622" class="Symbol">→</a> <a id="624" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="627" class="Symbol">(</a><a id="628" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="633" href="foundation.inhabited-types.html#611" class="Bound">l</a><a id="634" class="Symbol">)</a>
<a id="636" href="foundation.inhabited-types.html#593" class="Function">Inhabited-Type</a> <a id="651" href="foundation.inhabited-types.html#651" class="Bound">l</a> <a id="653" class="Symbol">=</a> <a id="655" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="657" class="Symbol">(</a><a id="658" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="661" href="foundation.inhabited-types.html#651" class="Bound">l</a><a id="662" class="Symbol">)</a> <a id="664" href="foundation.inhabited-types.html#502" class="Function">is-inhabited</a>

<a id="678" class="Keyword">module</a> <a id="685" href="foundation.inhabited-types.html#685" class="Module">_</a>
  <a id="689" class="Symbol">{</a><a id="690" href="foundation.inhabited-types.html#690" class="Bound">l</a> <a id="692" class="Symbol">:</a> <a id="694" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="699" class="Symbol">}</a> <a id="701" class="Symbol">(</a><a id="702" href="foundation.inhabited-types.html#702" class="Bound">X</a> <a id="704" class="Symbol">:</a> <a id="706" href="foundation.inhabited-types.html#593" class="Function">Inhabited-Type</a> <a id="721" href="foundation.inhabited-types.html#690" class="Bound">l</a><a id="722" class="Symbol">)</a>
  <a id="726" class="Keyword">where</a>

  <a id="735" href="foundation.inhabited-types.html#735" class="Function">type-Inhabited-Type</a> <a id="755" class="Symbol">:</a> <a id="757" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="760" href="foundation.inhabited-types.html#690" class="Bound">l</a>
  <a id="764" href="foundation.inhabited-types.html#735" class="Function">type-Inhabited-Type</a> <a id="784" class="Symbol">=</a> <a id="786" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="790" href="foundation.inhabited-types.html#702" class="Bound">X</a>

  <a id="795" href="foundation.inhabited-types.html#795" class="Function">is-inhabited-type-Inhabited-Type</a> <a id="828" class="Symbol">:</a> <a id="830" href="foundation.propositional-truncations.html#2209" class="Function">type-trunc-Prop</a> <a id="846" href="foundation.inhabited-types.html#735" class="Function">type-Inhabited-Type</a>
  <a id="868" href="foundation.inhabited-types.html#795" class="Function">is-inhabited-type-Inhabited-Type</a> <a id="901" class="Symbol">=</a> <a id="903" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="907" href="foundation.inhabited-types.html#702" class="Bound">X</a>
</pre>