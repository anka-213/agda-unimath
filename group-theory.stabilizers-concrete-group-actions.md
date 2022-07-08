---
title: Stabilizers of concrete group actions
---

<pre class="Agda"><a id="63" class="Symbol">{-#</a> <a id="67" class="Keyword">OPTIONS</a> <a id="75" class="Pragma">--without-K</a> <a id="87" class="Pragma">--exact-split</a> <a id="101" class="Symbol">#-}</a>

<a id="106" class="Keyword">module</a> <a id="113" href="group-theory.stabilizers-concrete-group-actions.html" class="Module">group-theory.stabilizers-concrete-group-actions</a> <a id="161" class="Keyword">where</a>

<a id="168" class="Keyword">open</a> <a id="173" class="Keyword">import</a> <a id="180" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="212" class="Keyword">open</a> <a id="217" class="Keyword">import</a> <a id="224" href="foundation.connected-components.html" class="Module">foundation.connected-components</a>
<a id="256" class="Keyword">open</a> <a id="261" class="Keyword">import</a> <a id="268" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="296" class="Keyword">open</a> <a id="301" class="Keyword">import</a> <a id="308" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="337" class="Keyword">open</a> <a id="342" class="Keyword">import</a> <a id="349" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="385" class="Keyword">open</a> <a id="390" class="Keyword">import</a> <a id="397" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
</pre>
## Idea

The stabilizer of an element `x : X pt` of a concrete G-set `X : BG → UU-Set` is the connected component of `pair pt x` in the type of orbits of `X`. Its loop space is indeed the type of elements `g : G` such that `g x = x`.

## Definition

<pre class="Agda"><a id="stabilizer-Concrete-Group-Action"></a><a id="703" href="group-theory.stabilizers-concrete-group-actions.html#703" class="Function">stabilizer-Concrete-Group-Action</a> <a id="736" class="Symbol">:</a>
  <a id="740" class="Symbol">{</a><a id="741" href="group-theory.stabilizers-concrete-group-actions.html#741" class="Bound">l1</a> <a id="744" href="group-theory.stabilizers-concrete-group-actions.html#744" class="Bound">l2</a> <a id="747" class="Symbol">:</a> <a id="749" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="754" class="Symbol">}</a> <a id="756" class="Symbol">(</a><a id="757" href="group-theory.stabilizers-concrete-group-actions.html#757" class="Bound">G</a> <a id="759" class="Symbol">:</a> <a id="761" href="group-theory.concrete-groups.html#1988" class="Function">Concrete-Group</a> <a id="776" href="group-theory.stabilizers-concrete-group-actions.html#741" class="Bound">l1</a><a id="778" class="Symbol">)</a>
  <a id="782" class="Symbol">(</a><a id="783" href="group-theory.stabilizers-concrete-group-actions.html#783" class="Bound">X</a> <a id="785" class="Symbol">:</a> <a id="787" href="group-theory.concrete-group-actions.html#794" class="Function">action-Concrete-Group</a> <a id="809" href="group-theory.stabilizers-concrete-group-actions.html#744" class="Bound">l2</a> <a id="812" href="group-theory.stabilizers-concrete-group-actions.html#757" class="Bound">G</a><a id="813" class="Symbol">)</a> <a id="815" class="Symbol">→</a> <a id="817" href="group-theory.concrete-group-actions.html#1102" class="Function">type-action-Concrete-Group</a> <a id="844" href="group-theory.stabilizers-concrete-group-actions.html#757" class="Bound">G</a> <a id="846" href="group-theory.stabilizers-concrete-group-actions.html#783" class="Bound">X</a> <a id="848" class="Symbol">→</a>
  <a id="852" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="855" class="Symbol">(</a><a id="856" href="group-theory.stabilizers-concrete-group-actions.html#741" class="Bound">l1</a> <a id="859" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="861" href="group-theory.stabilizers-concrete-group-actions.html#744" class="Bound">l2</a><a id="863" class="Symbol">)</a>
<a id="865" href="group-theory.stabilizers-concrete-group-actions.html#703" class="Function">stabilizer-Concrete-Group-Action</a> <a id="898" href="group-theory.stabilizers-concrete-group-actions.html#898" class="Bound">G</a> <a id="900" href="group-theory.stabilizers-concrete-group-actions.html#900" class="Bound">X</a> <a id="902" href="group-theory.stabilizers-concrete-group-actions.html#902" class="Bound">x</a> <a id="904" class="Symbol">=</a>
  <a id="908" href="foundation.connected-components.html#1098" class="Function">connected-component</a>
    <a id="932" class="Symbol">(</a> <a id="934" href="group-theory.orbits-concrete-group-actions.html#420" class="Function">orbit-action-Concrete-Group</a> <a id="962" href="group-theory.stabilizers-concrete-group-actions.html#898" class="Bound">G</a> <a id="964" href="group-theory.stabilizers-concrete-group-actions.html#900" class="Bound">X</a><a id="965" class="Symbol">)</a>
    <a id="971" class="Symbol">(</a> <a id="973" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="978" class="Symbol">(</a><a id="979" href="group-theory.concrete-groups.html#2519" class="Function">shape-Concrete-Group</a> <a id="1000" href="group-theory.stabilizers-concrete-group-actions.html#898" class="Bound">G</a><a id="1001" class="Symbol">)</a> <a id="1003" href="group-theory.stabilizers-concrete-group-actions.html#902" class="Bound">x</a><a id="1004" class="Symbol">)</a>
</pre>