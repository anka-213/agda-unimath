---
title: Nilpotent elements in rings
---

<pre class="Agda"><a id="53" class="Symbol">{-#</a> <a id="57" class="Keyword">OPTIONS</a> <a id="65" class="Pragma">--without-K</a> <a id="77" class="Pragma">--exact-split</a> <a id="91" class="Symbol">#-}</a>

<a id="96" class="Keyword">module</a> <a id="103" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a> <a id="140" class="Keyword">where</a>

<a id="147" class="Keyword">open</a> <a id="152" class="Keyword">import</a> <a id="159" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="201" class="Keyword">open</a> <a id="206" class="Keyword">import</a> <a id="213" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="251" class="Keyword">open</a> <a id="256" class="Keyword">import</a> <a id="263" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="289" class="Keyword">open</a> <a id="294" class="Keyword">import</a> <a id="301" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="325" class="Keyword">open</a> <a id="330" class="Keyword">import</a> <a id="337" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="365" class="Keyword">open</a> <a id="370" class="Keyword">import</a> <a id="377" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a>
<a id="414" class="Keyword">open</a> <a id="419" class="Keyword">import</a> <a id="426" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Idea

A nilpotent element in a ring is an element `x` for which there is a natural number `n` such that `x^n = 0`.

## Definition

<pre class="Agda"><a id="is-nilpotent-element-ring-Prop"></a><a id="591" href="ring-theory.nilpotent-elements-rings.html#591" class="Function">is-nilpotent-element-ring-Prop</a> <a id="622" class="Symbol">:</a>
  <a id="626" class="Symbol">{</a><a id="627" href="ring-theory.nilpotent-elements-rings.html#627" class="Bound">l</a> <a id="629" class="Symbol">:</a> <a id="631" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="636" class="Symbol">}</a> <a id="638" class="Symbol">(</a><a id="639" href="ring-theory.nilpotent-elements-rings.html#639" class="Bound">R</a> <a id="641" class="Symbol">:</a> <a id="643" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="648" href="ring-theory.nilpotent-elements-rings.html#627" class="Bound">l</a><a id="649" class="Symbol">)</a> <a id="651" class="Symbol">→</a> <a id="653" href="ring-theory.rings.html#2808" class="Function">type-Ring</a> <a id="663" href="ring-theory.nilpotent-elements-rings.html#639" class="Bound">R</a> <a id="665" class="Symbol">→</a> <a id="667" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="675" href="ring-theory.nilpotent-elements-rings.html#627" class="Bound">l</a>
<a id="677" href="ring-theory.nilpotent-elements-rings.html#591" class="Function">is-nilpotent-element-ring-Prop</a> <a id="708" href="ring-theory.nilpotent-elements-rings.html#708" class="Bound">R</a> <a id="710" href="ring-theory.nilpotent-elements-rings.html#710" class="Bound">x</a> <a id="712" class="Symbol">=</a> <a id="714" href="foundation.existential-quantification.html#1666" class="Function">∃-Prop</a> <a id="721" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="723" class="Symbol">(λ</a> <a id="726" href="ring-theory.nilpotent-elements-rings.html#726" class="Bound">n</a> <a id="728" class="Symbol">→</a> <a id="730" href="foundation-core.identity-types.html#1767" class="Datatype">Id</a> <a id="733" class="Symbol">(</a><a id="734" href="ring-theory.powers-of-elements-rings.html#299" class="Function">power-Ring</a> <a id="745" href="ring-theory.nilpotent-elements-rings.html#708" class="Bound">R</a> <a id="747" href="ring-theory.nilpotent-elements-rings.html#726" class="Bound">n</a> <a id="749" href="ring-theory.nilpotent-elements-rings.html#710" class="Bound">x</a><a id="750" class="Symbol">)</a> <a id="752" class="Symbol">(</a><a id="753" href="ring-theory.rings.html#5170" class="Function">zero-Ring</a> <a id="763" href="ring-theory.nilpotent-elements-rings.html#708" class="Bound">R</a><a id="764" class="Symbol">))</a>

<a id="is-nilpotent-element-Ring"></a><a id="768" href="ring-theory.nilpotent-elements-rings.html#768" class="Function">is-nilpotent-element-Ring</a> <a id="794" class="Symbol">:</a> <a id="796" class="Symbol">{</a><a id="797" href="ring-theory.nilpotent-elements-rings.html#797" class="Bound">l</a> <a id="799" class="Symbol">:</a> <a id="801" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="806" class="Symbol">}</a> <a id="808" class="Symbol">(</a><a id="809" href="ring-theory.nilpotent-elements-rings.html#809" class="Bound">R</a> <a id="811" class="Symbol">:</a> <a id="813" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="818" href="ring-theory.nilpotent-elements-rings.html#797" class="Bound">l</a><a id="819" class="Symbol">)</a> <a id="821" class="Symbol">→</a> <a id="823" href="ring-theory.rings.html#2808" class="Function">type-Ring</a> <a id="833" href="ring-theory.nilpotent-elements-rings.html#809" class="Bound">R</a> <a id="835" class="Symbol">→</a> <a id="837" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="840" href="ring-theory.nilpotent-elements-rings.html#797" class="Bound">l</a>
<a id="842" href="ring-theory.nilpotent-elements-rings.html#768" class="Function">is-nilpotent-element-Ring</a> <a id="868" href="ring-theory.nilpotent-elements-rings.html#868" class="Bound">R</a> <a id="870" href="ring-theory.nilpotent-elements-rings.html#870" class="Bound">x</a> <a id="872" class="Symbol">=</a> <a id="874" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="884" class="Symbol">(</a><a id="885" href="ring-theory.nilpotent-elements-rings.html#591" class="Function">is-nilpotent-element-ring-Prop</a> <a id="916" href="ring-theory.nilpotent-elements-rings.html#868" class="Bound">R</a> <a id="918" href="ring-theory.nilpotent-elements-rings.html#870" class="Bound">x</a><a id="919" class="Symbol">)</a>

<a id="is-prop-is-nilpotent-element-Ring"></a><a id="922" href="ring-theory.nilpotent-elements-rings.html#922" class="Function">is-prop-is-nilpotent-element-Ring</a> <a id="956" class="Symbol">:</a>
  <a id="960" class="Symbol">{</a><a id="961" href="ring-theory.nilpotent-elements-rings.html#961" class="Bound">l</a> <a id="963" class="Symbol">:</a> <a id="965" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="970" class="Symbol">}</a> <a id="972" class="Symbol">(</a><a id="973" href="ring-theory.nilpotent-elements-rings.html#973" class="Bound">R</a> <a id="975" class="Symbol">:</a> <a id="977" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="982" href="ring-theory.nilpotent-elements-rings.html#961" class="Bound">l</a><a id="983" class="Symbol">)</a> <a id="985" class="Symbol">(</a><a id="986" href="ring-theory.nilpotent-elements-rings.html#986" class="Bound">x</a> <a id="988" class="Symbol">:</a> <a id="990" href="ring-theory.rings.html#2808" class="Function">type-Ring</a> <a id="1000" href="ring-theory.nilpotent-elements-rings.html#973" class="Bound">R</a><a id="1001" class="Symbol">)</a> <a id="1003" class="Symbol">→</a>
  <a id="1007" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="1015" class="Symbol">(</a><a id="1016" href="ring-theory.nilpotent-elements-rings.html#768" class="Function">is-nilpotent-element-Ring</a> <a id="1042" href="ring-theory.nilpotent-elements-rings.html#973" class="Bound">R</a> <a id="1044" href="ring-theory.nilpotent-elements-rings.html#986" class="Bound">x</a><a id="1045" class="Symbol">)</a>
<a id="1047" href="ring-theory.nilpotent-elements-rings.html#922" class="Function">is-prop-is-nilpotent-element-Ring</a> <a id="1081" href="ring-theory.nilpotent-elements-rings.html#1081" class="Bound">R</a> <a id="1083" href="ring-theory.nilpotent-elements-rings.html#1083" class="Bound">x</a> <a id="1085" class="Symbol">=</a>
  <a id="1089" href="foundation-core.propositions.html#1562" class="Function">is-prop-type-Prop</a> <a id="1107" class="Symbol">(</a><a id="1108" href="ring-theory.nilpotent-elements-rings.html#591" class="Function">is-nilpotent-element-ring-Prop</a> <a id="1139" href="ring-theory.nilpotent-elements-rings.html#1081" class="Bound">R</a> <a id="1141" href="ring-theory.nilpotent-elements-rings.html#1083" class="Bound">x</a><a id="1142" class="Symbol">)</a>
</pre>