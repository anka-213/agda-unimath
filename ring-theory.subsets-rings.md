---
title: Subsets of rings
---

<pre class="Agda"><a id="42" class="Symbol">{-#</a> <a id="46" class="Keyword">OPTIONS</a> <a id="54" class="Pragma">--without-K</a> <a id="66" class="Pragma">--exact-split</a> <a id="80" class="Symbol">#-}</a>

<a id="85" class="Keyword">module</a> <a id="92" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a> <a id="118" class="Keyword">where</a>

<a id="125" class="Keyword">open</a> <a id="130" class="Keyword">import</a> <a id="137" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="169" class="Keyword">open</a> <a id="174" class="Keyword">import</a> <a id="181" href="foundation.propositional-extensionality.html" class="Module">foundation.propositional-extensionality</a> <a id="221" class="Keyword">using</a> <a id="227" class="Symbol">(</a><a id="228" href="foundation.propositional-extensionality.html#3478" class="Function">is-set-UU-Prop</a><a id="242" class="Symbol">)</a>
<a id="244" class="Keyword">open</a> <a id="249" class="Keyword">import</a> <a id="256" href="foundation.sets.html" class="Module">foundation.sets</a> <a id="272" class="Keyword">using</a> <a id="278" class="Symbol">(</a><a id="279" href="foundation-core.sets.html#1099" class="Function">is-set</a><a id="285" class="Symbol">;</a> <a id="287" href="foundation.sets.html#3467" class="Function">is-set-function-type</a><a id="307" class="Symbol">)</a>
<a id="309" class="Keyword">open</a> <a id="314" class="Keyword">import</a> <a id="321" href="foundation.subtypes.html" class="Module">foundation.subtypes</a> <a id="341" class="Keyword">using</a> <a id="347" class="Symbol">(</a><a id="348" href="foundation-core.subtypes.html#2197" class="Function">subtype</a><a id="355" class="Symbol">;</a> <a id="357" href="foundation-core.subtypes.html#2541" class="Function">type-subtype</a><a id="369" class="Symbol">)</a>
<a id="371" class="Keyword">open</a> <a id="376" class="Keyword">import</a> <a id="383" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="410" class="Keyword">using</a> <a id="416" class="Symbol">(</a><a id="417" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="422" class="Symbol">;</a> <a id="424" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="426" class="Symbol">;</a> <a id="428" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="431" class="Symbol">;</a> <a id="433" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="437" class="Symbol">)</a>

<a id="440" class="Keyword">open</a> <a id="445" class="Keyword">import</a> <a id="452" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="470" class="Keyword">using</a> <a id="476" class="Symbol">(</a><a id="477" href="ring-theory.rings.html#2508" class="Function">Ring</a><a id="481" class="Symbol">;</a> <a id="483" href="ring-theory.rings.html#2765" class="Function">type-Ring</a><a id="492" class="Symbol">)</a>
</pre>
## Idea

A subset of a ring is a subtype of the underlying type of a ring

## Definition

<pre class="Agda"><a id="subset-Ring"></a><a id="597" href="ring-theory.subsets-rings.html#597" class="Function">subset-Ring</a> <a id="609" class="Symbol">:</a>
  <a id="613" class="Symbol">(</a><a id="614" href="ring-theory.subsets-rings.html#614" class="Bound">l</a> <a id="616" class="Symbol">:</a> <a id="618" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="623" class="Symbol">)</a> <a id="625" class="Symbol">{</a><a id="626" href="ring-theory.subsets-rings.html#626" class="Bound">l1</a> <a id="629" class="Symbol">:</a> <a id="631" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="636" class="Symbol">}</a> <a id="638" class="Symbol">(</a><a id="639" href="ring-theory.subsets-rings.html#639" class="Bound">R</a> <a id="641" class="Symbol">:</a> <a id="643" href="ring-theory.rings.html#2508" class="Function">Ring</a> <a id="648" href="ring-theory.subsets-rings.html#626" class="Bound">l1</a><a id="650" class="Symbol">)</a> <a id="652" class="Symbol">→</a> <a id="654" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="657" class="Symbol">((</a><a id="659" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="664" href="ring-theory.subsets-rings.html#614" class="Bound">l</a><a id="665" class="Symbol">)</a> <a id="667" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="669" href="ring-theory.subsets-rings.html#626" class="Bound">l1</a><a id="671" class="Symbol">)</a>
<a id="673" href="ring-theory.subsets-rings.html#597" class="Function">subset-Ring</a> <a id="685" href="ring-theory.subsets-rings.html#685" class="Bound">l</a> <a id="687" href="ring-theory.subsets-rings.html#687" class="Bound">R</a> <a id="689" class="Symbol">=</a> <a id="691" href="foundation-core.subtypes.html#2197" class="Function">subtype</a> <a id="699" href="ring-theory.subsets-rings.html#685" class="Bound">l</a> <a id="701" class="Symbol">(</a><a id="702" href="ring-theory.rings.html#2765" class="Function">type-Ring</a> <a id="712" href="ring-theory.subsets-rings.html#687" class="Bound">R</a><a id="713" class="Symbol">)</a>

<a id="is-set-subset-Ring"></a><a id="716" href="ring-theory.subsets-rings.html#716" class="Function">is-set-subset-Ring</a> <a id="735" class="Symbol">:</a>
  <a id="739" class="Symbol">(</a><a id="740" href="ring-theory.subsets-rings.html#740" class="Bound">l</a> <a id="742" class="Symbol">:</a> <a id="744" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="749" class="Symbol">)</a> <a id="751" class="Symbol">{</a><a id="752" href="ring-theory.subsets-rings.html#752" class="Bound">l1</a> <a id="755" class="Symbol">:</a> <a id="757" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="762" class="Symbol">}</a> <a id="764" class="Symbol">(</a><a id="765" href="ring-theory.subsets-rings.html#765" class="Bound">R</a> <a id="767" class="Symbol">:</a> <a id="769" href="ring-theory.rings.html#2508" class="Function">Ring</a> <a id="774" href="ring-theory.subsets-rings.html#752" class="Bound">l1</a><a id="776" class="Symbol">)</a> <a id="778" class="Symbol">→</a> <a id="780" href="foundation-core.sets.html#1099" class="Function">is-set</a> <a id="787" class="Symbol">(</a><a id="788" href="ring-theory.subsets-rings.html#597" class="Function">subset-Ring</a> <a id="800" href="ring-theory.subsets-rings.html#740" class="Bound">l</a> <a id="802" href="ring-theory.subsets-rings.html#765" class="Bound">R</a><a id="803" class="Symbol">)</a>
<a id="805" href="ring-theory.subsets-rings.html#716" class="Function">is-set-subset-Ring</a> <a id="824" href="ring-theory.subsets-rings.html#824" class="Bound">l</a> <a id="826" href="ring-theory.subsets-rings.html#826" class="Bound">R</a> <a id="828" class="Symbol">=</a>
  <a id="832" href="foundation.sets.html#3467" class="Function">is-set-function-type</a> <a id="853" href="foundation.propositional-extensionality.html#3478" class="Function">is-set-UU-Prop</a>

<a id="869" class="Keyword">module</a> <a id="876" href="ring-theory.subsets-rings.html#876" class="Module">_</a>
  <a id="880" class="Symbol">{</a><a id="881" href="ring-theory.subsets-rings.html#881" class="Bound">l1</a> <a id="884" href="ring-theory.subsets-rings.html#884" class="Bound">l2</a> <a id="887" class="Symbol">:</a> <a id="889" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="894" class="Symbol">}</a> <a id="896" class="Symbol">(</a><a id="897" href="ring-theory.subsets-rings.html#897" class="Bound">R</a> <a id="899" class="Symbol">:</a> <a id="901" href="ring-theory.rings.html#2508" class="Function">Ring</a> <a id="906" href="ring-theory.subsets-rings.html#881" class="Bound">l1</a><a id="908" class="Symbol">)</a> <a id="910" class="Symbol">(</a><a id="911" href="ring-theory.subsets-rings.html#911" class="Bound">S</a> <a id="913" class="Symbol">:</a> <a id="915" href="ring-theory.subsets-rings.html#597" class="Function">subset-Ring</a> <a id="927" href="ring-theory.subsets-rings.html#884" class="Bound">l2</a> <a id="930" href="ring-theory.subsets-rings.html#897" class="Bound">R</a><a id="931" class="Symbol">)</a>
  <a id="935" class="Keyword">where</a>

  <a id="944" href="ring-theory.subsets-rings.html#944" class="Function">type-subset-Ring</a> <a id="961" class="Symbol">:</a> <a id="963" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="966" class="Symbol">(</a><a id="967" href="ring-theory.subsets-rings.html#881" class="Bound">l1</a> <a id="970" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="972" href="ring-theory.subsets-rings.html#884" class="Bound">l2</a><a id="974" class="Symbol">)</a>
  <a id="978" href="ring-theory.subsets-rings.html#944" class="Function">type-subset-Ring</a> <a id="995" class="Symbol">=</a> <a id="997" href="foundation-core.subtypes.html#2541" class="Function">type-subtype</a> <a id="1010" href="ring-theory.subsets-rings.html#911" class="Bound">S</a>

  <a id="1015" href="ring-theory.subsets-rings.html#1015" class="Function">inclusion-subset-Ring</a> <a id="1037" class="Symbol">:</a> <a id="1039" href="ring-theory.subsets-rings.html#944" class="Function">type-subset-Ring</a> <a id="1056" class="Symbol">→</a> <a id="1058" href="ring-theory.rings.html#2765" class="Function">type-Ring</a> <a id="1068" href="ring-theory.subsets-rings.html#897" class="Bound">R</a>
  <a id="1072" href="ring-theory.subsets-rings.html#1015" class="Function">inclusion-subset-Ring</a> <a id="1094" class="Symbol">=</a> <a id="1096" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a>
</pre>