---
title: Free concrete group actions
---

<pre class="Agda"><a id="53" class="Symbol">{-#</a> <a id="57" class="Keyword">OPTIONS</a> <a id="65" class="Pragma">--without-K</a> <a id="77" class="Pragma">--exact-split</a> <a id="91" class="Symbol">#-}</a>

<a id="96" class="Keyword">module</a> <a id="103" href="group-theory.free-concrete-group-actions.html" class="Module">group-theory.free-concrete-group-actions</a> <a id="144" class="Keyword">where</a>

<a id="151" class="Keyword">open</a> <a id="156" class="Keyword">import</a> <a id="163" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="187" class="Keyword">open</a> <a id="192" class="Keyword">import</a> <a id="199" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="215" class="Keyword">open</a> <a id="220" class="Keyword">import</a> <a id="227" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="255" class="Keyword">open</a> <a id="260" class="Keyword">import</a> <a id="267" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="303" class="Keyword">open</a> <a id="308" class="Keyword">import</a> <a id="315" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="344" class="Keyword">open</a> <a id="349" class="Keyword">import</a> <a id="356" href="group-theory.orbits-concrete-group-actions.html" class="Module">group-theory.orbits-concrete-group-actions</a>
</pre>
## Definition

<pre class="Agda"><a id="is-free-action-Concrete-Group-Prop"></a><a id="427" href="group-theory.free-concrete-group-actions.html#427" class="Function">is-free-action-Concrete-Group-Prop</a> <a id="462" class="Symbol">:</a>
  <a id="466" class="Symbol">{</a><a id="467" href="group-theory.free-concrete-group-actions.html#467" class="Bound">l1</a> <a id="470" href="group-theory.free-concrete-group-actions.html#470" class="Bound">l2</a> <a id="473" class="Symbol">:</a> <a id="475" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="480" class="Symbol">}</a> <a id="482" class="Symbol">(</a><a id="483" href="group-theory.free-concrete-group-actions.html#483" class="Bound">G</a> <a id="485" class="Symbol">:</a> <a id="487" href="group-theory.concrete-groups.html#2030" class="Function">Concrete-Group</a> <a id="502" href="group-theory.free-concrete-group-actions.html#467" class="Bound">l1</a><a id="504" class="Symbol">)</a> <a id="506" class="Symbol">→</a> <a id="508" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="530" href="group-theory.free-concrete-group-actions.html#470" class="Bound">l2</a> <a id="533" href="group-theory.free-concrete-group-actions.html#483" class="Bound">G</a> <a id="535" class="Symbol">→</a>
  <a id="539" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="547" class="Symbol">(</a><a id="548" href="group-theory.free-concrete-group-actions.html#467" class="Bound">l1</a> <a id="551" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="553" href="group-theory.free-concrete-group-actions.html#470" class="Bound">l2</a><a id="555" class="Symbol">)</a>
<a id="557" href="group-theory.free-concrete-group-actions.html#427" class="Function">is-free-action-Concrete-Group-Prop</a> <a id="592" href="group-theory.free-concrete-group-actions.html#592" class="Bound">G</a> <a id="594" href="group-theory.free-concrete-group-actions.html#594" class="Bound">X</a> <a id="596" class="Symbol">=</a>
  <a id="600" href="foundation.sets.html#2542" class="Function">is-set-Prop</a> <a id="612" class="Symbol">(</a><a id="613" href="group-theory.orbits-concrete-group-actions.html#420" class="Function">orbit-action-Concrete-Group</a> <a id="641" href="group-theory.free-concrete-group-actions.html#592" class="Bound">G</a> <a id="643" href="group-theory.free-concrete-group-actions.html#594" class="Bound">X</a><a id="644" class="Symbol">)</a>

<a id="is-free-action-Concrete-Group"></a><a id="647" href="group-theory.free-concrete-group-actions.html#647" class="Function">is-free-action-Concrete-Group</a> <a id="677" class="Symbol">:</a>
  <a id="681" class="Symbol">{</a><a id="682" href="group-theory.free-concrete-group-actions.html#682" class="Bound">l1</a> <a id="685" href="group-theory.free-concrete-group-actions.html#685" class="Bound">l2</a> <a id="688" class="Symbol">:</a> <a id="690" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="695" class="Symbol">}</a> <a id="697" class="Symbol">(</a><a id="698" href="group-theory.free-concrete-group-actions.html#698" class="Bound">G</a> <a id="700" class="Symbol">:</a> <a id="702" href="group-theory.concrete-groups.html#2030" class="Function">Concrete-Group</a> <a id="717" href="group-theory.free-concrete-group-actions.html#682" class="Bound">l1</a><a id="719" class="Symbol">)</a> <a id="721" class="Symbol">→</a> <a id="723" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="745" href="group-theory.free-concrete-group-actions.html#685" class="Bound">l2</a> <a id="748" href="group-theory.free-concrete-group-actions.html#698" class="Bound">G</a> <a id="750" class="Symbol">→</a>
  <a id="754" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="757" class="Symbol">(</a><a id="758" href="group-theory.free-concrete-group-actions.html#682" class="Bound">l1</a> <a id="761" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="763" href="group-theory.free-concrete-group-actions.html#685" class="Bound">l2</a><a id="765" class="Symbol">)</a>
<a id="767" href="group-theory.free-concrete-group-actions.html#647" class="Function">is-free-action-Concrete-Group</a> <a id="797" href="group-theory.free-concrete-group-actions.html#797" class="Bound">G</a> <a id="799" href="group-theory.free-concrete-group-actions.html#799" class="Bound">X</a> <a id="801" class="Symbol">=</a>
  <a id="805" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="815" class="Symbol">(</a><a id="816" href="group-theory.free-concrete-group-actions.html#427" class="Function">is-free-action-Concrete-Group-Prop</a> <a id="851" href="group-theory.free-concrete-group-actions.html#797" class="Bound">G</a> <a id="853" href="group-theory.free-concrete-group-actions.html#799" class="Bound">X</a><a id="854" class="Symbol">)</a>

<a id="is-prop-is-free-action-Concrete-Group"></a><a id="857" href="group-theory.free-concrete-group-actions.html#857" class="Function">is-prop-is-free-action-Concrete-Group</a> <a id="895" class="Symbol">:</a>
  <a id="899" class="Symbol">{</a><a id="900" href="group-theory.free-concrete-group-actions.html#900" class="Bound">l1</a> <a id="903" href="group-theory.free-concrete-group-actions.html#903" class="Bound">l2</a> <a id="906" class="Symbol">:</a> <a id="908" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="913" class="Symbol">}</a> <a id="915" class="Symbol">(</a><a id="916" href="group-theory.free-concrete-group-actions.html#916" class="Bound">G</a> <a id="918" class="Symbol">:</a> <a id="920" href="group-theory.concrete-groups.html#2030" class="Function">Concrete-Group</a> <a id="935" href="group-theory.free-concrete-group-actions.html#900" class="Bound">l1</a><a id="937" class="Symbol">)</a> <a id="939" class="Symbol">(</a><a id="940" href="group-theory.free-concrete-group-actions.html#940" class="Bound">X</a> <a id="942" class="Symbol">:</a> <a id="944" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="966" href="group-theory.free-concrete-group-actions.html#903" class="Bound">l2</a> <a id="969" href="group-theory.free-concrete-group-actions.html#916" class="Bound">G</a><a id="970" class="Symbol">)</a> <a id="972" class="Symbol">→</a>
  <a id="976" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="984" class="Symbol">(</a><a id="985" href="group-theory.free-concrete-group-actions.html#647" class="Function">is-free-action-Concrete-Group</a> <a id="1015" href="group-theory.free-concrete-group-actions.html#916" class="Bound">G</a> <a id="1017" href="group-theory.free-concrete-group-actions.html#940" class="Bound">X</a><a id="1018" class="Symbol">)</a>
<a id="1020" href="group-theory.free-concrete-group-actions.html#857" class="Function">is-prop-is-free-action-Concrete-Group</a> <a id="1058" href="group-theory.free-concrete-group-actions.html#1058" class="Bound">G</a> <a id="1060" href="group-theory.free-concrete-group-actions.html#1060" class="Bound">X</a> <a id="1062" class="Symbol">=</a>
  <a id="1066" href="foundation-core.propositions.html#1562" class="Function">is-prop-type-Prop</a> <a id="1084" class="Symbol">(</a><a id="1085" href="group-theory.free-concrete-group-actions.html#427" class="Function">is-free-action-Concrete-Group-Prop</a> <a id="1120" href="group-theory.free-concrete-group-actions.html#1058" class="Bound">G</a> <a id="1122" href="group-theory.free-concrete-group-actions.html#1060" class="Bound">X</a><a id="1123" class="Symbol">)</a>
</pre>