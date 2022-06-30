---
title: Invertible elements in commutative rings
---

<pre class="Agda"><a id="66" class="Symbol">{-#</a> <a id="70" class="Keyword">OPTIONS</a> <a id="78" class="Pragma">--without-K</a> <a id="90" class="Pragma">--exact-split</a> <a id="104" class="Symbol">#-}</a>

<a id="109" class="Keyword">module</a> <a id="116" href="commutative-algebra.invertible-elements-commutative-rings.html" class="Module">commutative-algebra.invertible-elements-commutative-rings</a> <a id="174" class="Keyword">where</a>

<a id="181" class="Keyword">open</a> <a id="186" class="Keyword">import</a> <a id="193" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>

<a id="232" class="Keyword">open</a> <a id="237" class="Keyword">import</a> <a id="244" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="268" class="Keyword">open</a> <a id="273" class="Keyword">import</a> <a id="280" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="308" class="Keyword">open</a> <a id="313" class="Keyword">import</a> <a id="320" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="358" class="Keyword">open</a> <a id="363" class="Keyword">import</a> <a id="370" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Idea

Invertible elements are elements that have a two-sided multiplicative inverse. Such elements are also called the units of the Ring. The set of units of any ring forms a group.

## Definition

<pre class="Agda"><a id="602" class="Keyword">module</a> <a id="609" href="commutative-algebra.invertible-elements-commutative-rings.html#609" class="Module">_</a>
  <a id="613" class="Symbol">{</a><a id="614" href="commutative-algebra.invertible-elements-commutative-rings.html#614" class="Bound">l</a> <a id="616" class="Symbol">:</a> <a id="618" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="623" class="Symbol">}</a> <a id="625" class="Symbol">(</a><a id="626" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a> <a id="628" class="Symbol">:</a> <a id="630" href="commutative-algebra.commutative-rings.html#1514" class="Function">Commutative-Ring</a> <a id="647" href="commutative-algebra.invertible-elements-commutative-rings.html#614" class="Bound">l</a><a id="648" class="Symbol">)</a>
  <a id="652" class="Keyword">where</a>
  
  <a id="663" href="commutative-algebra.invertible-elements-commutative-rings.html#663" class="Function">has-left-inverse-Commutative-Ring</a> <a id="697" class="Symbol">:</a> <a id="699" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="721" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a> <a id="723" class="Symbol">→</a> <a id="725" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="728" href="commutative-algebra.invertible-elements-commutative-rings.html#614" class="Bound">l</a>
  <a id="732" href="commutative-algebra.invertible-elements-commutative-rings.html#663" class="Function">has-left-inverse-Commutative-Ring</a> <a id="766" class="Symbol">=</a>
    <a id="772" href="ring-theory.invertible-elements-rings.html#901" class="Function">has-left-inverse-Ring</a> <a id="794" class="Symbol">(</a><a id="795" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="817" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a><a id="818" class="Symbol">)</a>
  
  <a id="825" href="commutative-algebra.invertible-elements-commutative-rings.html#825" class="Function">has-right-inverse-Commutative-Ring</a> <a id="860" class="Symbol">:</a> <a id="862" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="884" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a> <a id="886" class="Symbol">→</a> <a id="888" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="891" href="commutative-algebra.invertible-elements-commutative-rings.html#614" class="Bound">l</a>
  <a id="895" href="commutative-algebra.invertible-elements-commutative-rings.html#825" class="Function">has-right-inverse-Commutative-Ring</a> <a id="930" class="Symbol">=</a>
    <a id="936" href="ring-theory.invertible-elements-rings.html#1038" class="Function">has-right-inverse-Ring</a> <a id="959" class="Symbol">(</a><a id="960" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="982" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a><a id="983" class="Symbol">)</a>
  
  <a id="990" href="commutative-algebra.invertible-elements-commutative-rings.html#990" class="Function">has-two-sided-inverse-Commutative-Ring</a> <a id="1029" class="Symbol">:</a> <a id="1031" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="1053" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a> <a id="1055" class="Symbol">→</a> <a id="1057" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1060" href="commutative-algebra.invertible-elements-commutative-rings.html#614" class="Bound">l</a>
  <a id="1064" href="commutative-algebra.invertible-elements-commutative-rings.html#990" class="Function">has-two-sided-inverse-Commutative-Ring</a> <a id="1103" class="Symbol">=</a>
    <a id="1109" href="ring-theory.invertible-elements-rings.html#1177" class="Function">has-two-sided-inverse-Ring</a> <a id="1136" class="Symbol">(</a><a id="1137" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="1159" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a><a id="1160" class="Symbol">)</a>

  <a id="1165" href="commutative-algebra.invertible-elements-commutative-rings.html#1165" class="Function">is-invertible-element-commutative-ring-Prop</a> <a id="1209" class="Symbol">:</a>
    <a id="1215" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="1237" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a> <a id="1239" class="Symbol">→</a> <a id="1241" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="1249" href="commutative-algebra.invertible-elements-commutative-rings.html#614" class="Bound">l</a>
  <a id="1253" href="commutative-algebra.invertible-elements-commutative-rings.html#1165" class="Function">is-invertible-element-commutative-ring-Prop</a> <a id="1297" class="Symbol">=</a>
    <a id="1303" href="ring-theory.invertible-elements-rings.html#1321" class="Function">is-invertible-element-ring-Prop</a> <a id="1335" class="Symbol">(</a><a id="1336" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="1358" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a><a id="1359" class="Symbol">)</a>

  <a id="1364" href="commutative-algebra.invertible-elements-commutative-rings.html#1364" class="Function">is-invertible-element-Commutative-Ring</a> <a id="1403" class="Symbol">:</a> <a id="1405" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="1427" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a> <a id="1429" class="Symbol">→</a> <a id="1431" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1434" href="commutative-algebra.invertible-elements-commutative-rings.html#614" class="Bound">l</a>
  <a id="1438" href="commutative-algebra.invertible-elements-commutative-rings.html#1364" class="Function">is-invertible-element-Commutative-Ring</a> <a id="1477" class="Symbol">=</a>
    <a id="1483" href="ring-theory.invertible-elements-rings.html#1491" class="Function">is-invertible-element-Ring</a> <a id="1510" class="Symbol">(</a><a id="1511" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="1533" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a><a id="1534" class="Symbol">)</a>

  <a id="1539" href="commutative-algebra.invertible-elements-commutative-rings.html#1539" class="Function">is-prop-is-invertible-element-Commutative-Ring</a> <a id="1586" class="Symbol">:</a>
    <a id="1592" class="Symbol">(</a><a id="1593" href="commutative-algebra.invertible-elements-commutative-rings.html#1593" class="Bound">x</a> <a id="1595" class="Symbol">:</a> <a id="1597" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="1619" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a><a id="1620" class="Symbol">)</a> <a id="1622" class="Symbol">→</a>
    <a id="1628" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="1636" class="Symbol">(</a><a id="1637" href="commutative-algebra.invertible-elements-commutative-rings.html#1364" class="Function">is-invertible-element-Commutative-Ring</a> <a id="1676" href="commutative-algebra.invertible-elements-commutative-rings.html#1593" class="Bound">x</a><a id="1677" class="Symbol">)</a>
  <a id="1681" href="commutative-algebra.invertible-elements-commutative-rings.html#1539" class="Function">is-prop-is-invertible-element-Commutative-Ring</a> <a id="1728" class="Symbol">=</a>
    <a id="1734" href="ring-theory.invertible-elements-rings.html#1625" class="Function">is-prop-is-invertible-element-Ring</a> <a id="1769" class="Symbol">(</a><a id="1770" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="1792" href="commutative-algebra.invertible-elements-commutative-rings.html#626" class="Bound">R</a><a id="1793" class="Symbol">)</a>
</pre>