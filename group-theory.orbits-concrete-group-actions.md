---
title: Orbits of concrete group actions
---

<pre class="Agda"><a id="58" class="Symbol">{-#</a> <a id="62" class="Keyword">OPTIONS</a> <a id="70" class="Pragma">--without-K</a> <a id="82" class="Pragma">--exact-split</a> <a id="96" class="Symbol">#-}</a>

<a id="101" class="Keyword">module</a> <a id="108" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a> <a id="151" class="Keyword">where</a>

<a id="158" class="Keyword">open</a> <a id="163" class="Keyword">import</a> <a id="170" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="202" class="Keyword">open</a> <a id="207" class="Keyword">import</a> <a id="214" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="235" class="Keyword">open</a> <a id="240" class="Keyword">import</a> <a id="247" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="263" class="Keyword">open</a> <a id="268" class="Keyword">import</a> <a id="275" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="303" class="Keyword">open</a> <a id="308" class="Keyword">import</a> <a id="315" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="351" class="Keyword">open</a> <a id="356" class="Keyword">import</a> <a id="363" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
</pre>
## Definition

<pre class="Agda"><a id="orbit-action-Concrete-Group"></a><a id="420" href="group-theory.orbits-concrete-group-actions.html#420" class="Function">orbit-action-Concrete-Group</a> <a id="448" class="Symbol">:</a>
  <a id="452" class="Symbol">{</a><a id="453" href="group-theory.orbits-concrete-group-actions.html#453" class="Bound">l1</a> <a id="456" href="group-theory.orbits-concrete-group-actions.html#456" class="Bound">l2</a> <a id="459" class="Symbol">:</a> <a id="461" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="466" class="Symbol">}</a> <a id="468" class="Symbol">(</a><a id="469" href="group-theory.orbits-concrete-group-actions.html#469" class="Bound">G</a> <a id="471" class="Symbol">:</a> <a id="473" href="group-theory.concrete-groups.html#1988" class="Function">Concrete-Group</a> <a id="488" href="group-theory.orbits-concrete-group-actions.html#453" class="Bound">l1</a><a id="490" class="Symbol">)</a> <a id="492" class="Symbol">(</a><a id="493" href="group-theory.orbits-concrete-group-actions.html#493" class="Bound">X</a> <a id="495" class="Symbol">:</a> <a id="497" href="group-theory.concrete-group-actions.html#794" class="Function">action-Concrete-Group</a> <a id="519" href="group-theory.orbits-concrete-group-actions.html#456" class="Bound">l2</a> <a id="522" href="group-theory.orbits-concrete-group-actions.html#469" class="Bound">G</a><a id="523" class="Symbol">)</a> <a id="525" class="Symbol">→</a>
  <a id="529" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="532" class="Symbol">(</a><a id="533" href="group-theory.orbits-concrete-group-actions.html#453" class="Bound">l1</a> <a id="536" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="538" href="group-theory.orbits-concrete-group-actions.html#456" class="Bound">l2</a><a id="540" class="Symbol">)</a>
<a id="542" href="group-theory.orbits-concrete-group-actions.html#420" class="Function">orbit-action-Concrete-Group</a> <a id="570" href="group-theory.orbits-concrete-group-actions.html#570" class="Bound">G</a> <a id="572" href="group-theory.orbits-concrete-group-actions.html#572" class="Bound">X</a> <a id="574" class="Symbol">=</a>
  <a id="578" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="580" class="Symbol">(</a><a id="581" href="group-theory.concrete-groups.html#2389" class="Function">classifying-type-Concrete-Group</a> <a id="613" href="group-theory.orbits-concrete-group-actions.html#570" class="Bound">G</a><a id="614" class="Symbol">)</a> <a id="616" class="Symbol">(</a><a id="617" href="foundation-core.sets.html#1304" class="Function">type-Set</a> <a id="626" href="foundation-core.functions.html#420" class="Function Operator">∘</a> <a id="628" href="group-theory.orbits-concrete-group-actions.html#572" class="Bound">X</a><a id="629" class="Symbol">)</a>
</pre>