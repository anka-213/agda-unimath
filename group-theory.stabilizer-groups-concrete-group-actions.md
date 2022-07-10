---
title: Stabilizers of concrete group actions
---

<pre class="Agda"><a id="63" class="Symbol">{-#</a> <a id="67" class="Keyword">OPTIONS</a> <a id="75" class="Pragma">--without-K</a> <a id="87" class="Pragma">--exact-split</a> <a id="101" class="Symbol">#-}</a>

<a id="106" class="Keyword">module</a> <a id="113" href="group-theory.stabilizer-groups-concrete-group-actions.html" class="Module">group-theory.stabilizer-groups-concrete-group-actions</a> <a id="167" class="Keyword">where</a>

<a id="174" class="Keyword">open</a> <a id="179" class="Keyword">import</a> <a id="186" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="218" class="Keyword">open</a> <a id="223" class="Keyword">import</a> <a id="230" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="262" class="Keyword">open</a> <a id="267" class="Keyword">import</a> <a id="274" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="302" class="Keyword">open</a> <a id="307" class="Keyword">import</a> <a id="314" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="343" class="Keyword">open</a> <a id="348" class="Keyword">import</a> <a id="355" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="391" class="Keyword">open</a> <a id="396" class="Keyword">import</a> <a id="403" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
</pre>
## Idea

The stabilizer of an element `x : X pt` of a concrete G-set `X : BG → UU-Set` is the connected component of `pair pt x` in the type of orbits of `X`. Its loop space is indeed the type of elements `g : G` such that `g x = x`.

## Definition

<pre class="Agda"><a id="stabilizer-action-Concrete-Group"></a><a id="709" href="group-theory.stabilizer-groups-concrete-group-actions.html#709" class="Function">stabilizer-action-Concrete-Group</a> <a id="742" class="Symbol">:</a>
  <a id="746" class="Symbol">{</a><a id="747" href="group-theory.stabilizer-groups-concrete-group-actions.html#747" class="Bound">l1</a> <a id="750" href="group-theory.stabilizer-groups-concrete-group-actions.html#750" class="Bound">l2</a> <a id="753" class="Symbol">:</a> <a id="755" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="760" class="Symbol">}</a> <a id="762" class="Symbol">(</a><a id="763" href="group-theory.stabilizer-groups-concrete-group-actions.html#763" class="Bound">G</a> <a id="765" class="Symbol">:</a> <a id="767" href="group-theory.concrete-groups.html#2028" class="Function">Concrete-Group</a> <a id="782" href="group-theory.stabilizer-groups-concrete-group-actions.html#747" class="Bound">l1</a><a id="784" class="Symbol">)</a>
  <a id="788" class="Symbol">(</a><a id="789" href="group-theory.stabilizer-groups-concrete-group-actions.html#789" class="Bound">X</a> <a id="791" class="Symbol">:</a> <a id="793" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="815" href="group-theory.stabilizer-groups-concrete-group-actions.html#750" class="Bound">l2</a> <a id="818" href="group-theory.stabilizer-groups-concrete-group-actions.html#763" class="Bound">G</a><a id="819" class="Symbol">)</a> <a id="821" class="Symbol">→</a> <a id="823" href="group-theory.concrete-group-actions.html#1115" class="Function">type-action-Concrete-Group</a> <a id="850" href="group-theory.stabilizer-groups-concrete-group-actions.html#763" class="Bound">G</a> <a id="852" href="group-theory.stabilizer-groups-concrete-group-actions.html#789" class="Bound">X</a> <a id="854" class="Symbol">→</a>
  <a id="858" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="861" class="Symbol">(</a><a id="862" href="group-theory.stabilizer-groups-concrete-group-actions.html#747" class="Bound">l1</a> <a id="865" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="867" href="group-theory.stabilizer-groups-concrete-group-actions.html#750" class="Bound">l2</a><a id="869" class="Symbol">)</a>
<a id="871" href="group-theory.stabilizer-groups-concrete-group-actions.html#709" class="Function">stabilizer-action-Concrete-Group</a> <a id="904" href="group-theory.stabilizer-groups-concrete-group-actions.html#904" class="Bound">G</a> <a id="906" href="group-theory.stabilizer-groups-concrete-group-actions.html#906" class="Bound">X</a> <a id="908" href="group-theory.stabilizer-groups-concrete-group-actions.html#908" class="Bound">x</a> <a id="910" class="Symbol">=</a>
  <a id="914" href="foundation.connected-components.html#1098" class="Function">connected-component</a>
    <a id="938" class="Symbol">(</a> <a id="940" href="group-theory.orbits-concrete-group-actions.html#420" class="Function">orbit-action-Concrete-Group</a> <a id="968" href="group-theory.stabilizer-groups-concrete-group-actions.html#904" class="Bound">G</a> <a id="970" href="group-theory.stabilizer-groups-concrete-group-actions.html#906" class="Bound">X</a><a id="971" class="Symbol">)</a>
    <a id="977" class="Symbol">(</a> <a id="979" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="984" class="Symbol">(</a><a id="985" href="group-theory.concrete-groups.html#2559" class="Function">shape-Concrete-Group</a> <a id="1006" href="group-theory.stabilizer-groups-concrete-group-actions.html#904" class="Bound">G</a><a id="1007" class="Symbol">)</a> <a id="1009" href="group-theory.stabilizer-groups-concrete-group-actions.html#908" class="Bound">x</a><a id="1010" class="Symbol">)</a>
</pre>