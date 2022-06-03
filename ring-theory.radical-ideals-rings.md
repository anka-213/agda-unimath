---
title: Radical ideals in rings
---

<pre class="Agda"><a id="49" class="Symbol">{-#</a> <a id="53" class="Keyword">OPTIONS</a> <a id="61" class="Pragma">--without-K</a> <a id="73" class="Pragma">--exact-split</a> <a id="87" class="Symbol">#-}</a>

<a id="92" class="Keyword">module</a> <a id="99" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a> <a id="132" class="Keyword">where</a>

<a id="139" class="Keyword">open</a> <a id="144" class="Keyword">import</a> <a id="151" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="175" class="Keyword">open</a> <a id="180" class="Keyword">import</a> <a id="187" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="215" class="Keyword">open</a> <a id="220" class="Keyword">import</a> <a id="227" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="252" class="Keyword">open</a> <a id="257" class="Keyword">import</a> <a id="264" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="302" class="Keyword">open</a> <a id="307" class="Keyword">import</a> <a id="314" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Idea

A radical ideal in a ring R is a two-sided ideal I such that `1 + x` is a multiplicative unit for every `x ∈ I`.

## Definition

<pre class="Agda"><a id="483" class="Keyword">module</a> <a id="490" href="ring-theory.radical-ideals-rings.html#490" class="Module">_</a>
  <a id="494" class="Symbol">{</a><a id="495" href="ring-theory.radical-ideals-rings.html#495" class="Bound">l1</a> <a id="498" href="ring-theory.radical-ideals-rings.html#498" class="Bound">l2</a> <a id="501" class="Symbol">:</a> <a id="503" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="508" class="Symbol">}</a> <a id="510" class="Symbol">(</a><a id="511" href="ring-theory.radical-ideals-rings.html#511" class="Bound">R</a> <a id="513" class="Symbol">:</a> <a id="515" href="ring-theory.rings.html#2508" class="Function">Ring</a> <a id="520" href="ring-theory.radical-ideals-rings.html#495" class="Bound">l1</a><a id="522" class="Symbol">)</a> <a id="524" class="Symbol">(</a><a id="525" href="ring-theory.radical-ideals-rings.html#525" class="Bound">I</a> <a id="527" class="Symbol">:</a> <a id="529" href="ring-theory.ideals-rings.html#5897" class="Function">two-sided-ideal-Ring</a> <a id="550" href="ring-theory.radical-ideals-rings.html#498" class="Bound">l2</a> <a id="553" href="ring-theory.radical-ideals-rings.html#511" class="Bound">R</a><a id="554" class="Symbol">)</a>
  <a id="558" class="Keyword">where</a>
  
  <a id="569" href="ring-theory.radical-ideals-rings.html#569" class="Function">is-radical-two-sided-ideal-ring-Prop</a> <a id="606" class="Symbol">:</a> <a id="608" href="foundation-core.propositions.html#1380" class="Function">UU-Prop</a> <a id="616" class="Symbol">(</a><a id="617" href="ring-theory.radical-ideals-rings.html#495" class="Bound">l1</a> <a id="620" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="622" href="ring-theory.radical-ideals-rings.html#498" class="Bound">l2</a><a id="624" class="Symbol">)</a>
  <a id="628" href="ring-theory.radical-ideals-rings.html#569" class="Function">is-radical-two-sided-ideal-ring-Prop</a> <a id="665" class="Symbol">=</a>
    <a id="671" href="foundation-core.propositions.html#6683" class="Function">Π-Prop</a>
      <a id="684" class="Symbol">(</a> <a id="686" href="ring-theory.ideals-rings.html#6366" class="Function">type-two-sided-ideal-Ring</a> <a id="712" href="ring-theory.radical-ideals-rings.html#511" class="Bound">R</a> <a id="714" href="ring-theory.radical-ideals-rings.html#525" class="Bound">I</a><a id="715" class="Symbol">)</a>
      <a id="723" class="Symbol">(</a> <a id="725" class="Symbol">λ</a> <a id="727" href="ring-theory.radical-ideals-rings.html#727" class="Bound">x</a> <a id="729" class="Symbol">→</a>
        <a id="739" href="ring-theory.invertible-elements-rings.html#1321" class="Function">is-invertible-element-ring-Prop</a> <a id="771" href="ring-theory.radical-ideals-rings.html#511" class="Bound">R</a>
          <a id="783" class="Symbol">(</a> <a id="785" href="ring-theory.rings.html#3110" class="Function">add-Ring</a> <a id="794" href="ring-theory.radical-ideals-rings.html#511" class="Bound">R</a> <a id="796" class="Symbol">(</a><a id="797" href="ring-theory.rings.html#8015" class="Function">one-Ring</a> <a id="806" href="ring-theory.radical-ideals-rings.html#511" class="Bound">R</a><a id="807" class="Symbol">)</a> <a id="809" class="Symbol">(</a><a id="810" href="ring-theory.ideals-rings.html#6487" class="Function">inclusion-two-sided-ideal-Ring</a> <a id="841" href="ring-theory.radical-ideals-rings.html#511" class="Bound">R</a> <a id="843" href="ring-theory.radical-ideals-rings.html#525" class="Bound">I</a> <a id="845" href="ring-theory.radical-ideals-rings.html#727" class="Bound">x</a><a id="846" class="Symbol">)))</a>

  <a id="853" href="ring-theory.radical-ideals-rings.html#853" class="Function">is-radical-two-sided-ideal-Ring</a> <a id="885" class="Symbol">:</a> <a id="887" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="890" class="Symbol">(</a><a id="891" href="ring-theory.radical-ideals-rings.html#495" class="Bound">l1</a> <a id="894" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="896" href="ring-theory.radical-ideals-rings.html#498" class="Bound">l2</a><a id="898" class="Symbol">)</a>
  <a id="902" href="ring-theory.radical-ideals-rings.html#853" class="Function">is-radical-two-sided-ideal-Ring</a> <a id="934" class="Symbol">=</a>
    <a id="940" href="foundation-core.propositions.html#1482" class="Function">type-Prop</a> <a id="950" href="ring-theory.radical-ideals-rings.html#569" class="Function">is-radical-two-sided-ideal-ring-Prop</a>

  <a id="990" href="ring-theory.radical-ideals-rings.html#990" class="Function">is-prop-is-radical-two-sided-ideal-Ring</a> <a id="1030" class="Symbol">:</a>
    <a id="1036" href="foundation-core.propositions.html#1295" class="Function">is-prop</a> <a id="1044" href="ring-theory.radical-ideals-rings.html#853" class="Function">is-radical-two-sided-ideal-Ring</a>
  <a id="1078" href="ring-theory.radical-ideals-rings.html#990" class="Function">is-prop-is-radical-two-sided-ideal-Ring</a> <a id="1118" class="Symbol">=</a>
    <a id="1124" href="foundation-core.propositions.html#1549" class="Function">is-prop-type-Prop</a> <a id="1142" href="ring-theory.radical-ideals-rings.html#569" class="Function">is-radical-two-sided-ideal-ring-Prop</a>
</pre>