---
title: Nil ideals
---

<pre class="Agda"><a id="36" class="Symbol">{-#</a> <a id="40" class="Keyword">OPTIONS</a> <a id="48" class="Pragma">--without-K</a> <a id="60" class="Pragma">--exact-split</a> <a id="74" class="Symbol">#-}</a>

<a id="79" class="Keyword">module</a> <a id="86" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a> <a id="115" class="Keyword">where</a>

<a id="122" class="Keyword">open</a> <a id="127" class="Keyword">import</a> <a id="134" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="158" class="Keyword">open</a> <a id="163" class="Keyword">import</a> <a id="170" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="198" class="Keyword">open</a> <a id="203" class="Keyword">import</a> <a id="210" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a>
<a id="235" class="Keyword">open</a> <a id="240" class="Keyword">import</a> <a id="247" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a>
<a id="284" class="Keyword">open</a> <a id="289" class="Keyword">import</a> <a id="296" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Idea

A nil ideal in a ring is an ideal in which every element is nilpotent

## Definition

### Nil left ideals

<pre class="Agda"><a id="443" class="Keyword">module</a> <a id="450" href="ring-theory.nil-ideals-rings.html#450" class="Module">_</a>
  <a id="454" class="Symbol">{</a><a id="455" href="ring-theory.nil-ideals-rings.html#455" class="Bound">l1</a> <a id="458" href="ring-theory.nil-ideals-rings.html#458" class="Bound">l2</a> <a id="461" class="Symbol">:</a> <a id="463" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="468" class="Symbol">}</a> <a id="470" class="Symbol">(</a><a id="471" href="ring-theory.nil-ideals-rings.html#471" class="Bound">R</a> <a id="473" class="Symbol">:</a> <a id="475" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="480" href="ring-theory.nil-ideals-rings.html#455" class="Bound">l1</a><a id="482" class="Symbol">)</a> <a id="484" class="Symbol">(</a><a id="485" href="ring-theory.nil-ideals-rings.html#485" class="Bound">I</a> <a id="487" class="Symbol">:</a> <a id="489" href="ring-theory.ideals-rings.html#1753" class="Function">left-ideal-Ring</a> <a id="505" href="ring-theory.nil-ideals-rings.html#458" class="Bound">l2</a> <a id="508" href="ring-theory.nil-ideals-rings.html#471" class="Bound">R</a><a id="509" class="Symbol">)</a>
  <a id="513" class="Keyword">where</a>
  
  <a id="524" href="ring-theory.nil-ideals-rings.html#524" class="Function">is-nil-left-ideal-ring-Prop</a> <a id="552" class="Symbol">:</a> <a id="554" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="562" class="Symbol">(</a><a id="563" href="ring-theory.nil-ideals-rings.html#455" class="Bound">l1</a> <a id="566" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="568" href="ring-theory.nil-ideals-rings.html#458" class="Bound">l2</a><a id="570" class="Symbol">)</a>
  <a id="574" href="ring-theory.nil-ideals-rings.html#524" class="Function">is-nil-left-ideal-ring-Prop</a> <a id="602" class="Symbol">=</a>
    <a id="608" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
      <a id="621" class="Symbol">(</a> <a id="623" href="ring-theory.ideals-rings.html#2175" class="Function">type-left-ideal-Ring</a> <a id="644" href="ring-theory.nil-ideals-rings.html#471" class="Bound">R</a> <a id="646" href="ring-theory.nil-ideals-rings.html#485" class="Bound">I</a><a id="647" class="Symbol">)</a>
      <a id="655" class="Symbol">(</a> <a id="657" class="Symbol">λ</a> <a id="659" href="ring-theory.nil-ideals-rings.html#659" class="Bound">x</a> <a id="661" class="Symbol">→</a>
        <a id="671" href="ring-theory.nilpotent-elements-rings.html#591" class="Function">is-nilpotent-element-ring-Prop</a> <a id="702" href="ring-theory.nil-ideals-rings.html#471" class="Bound">R</a> <a id="704" class="Symbol">(</a><a id="705" href="ring-theory.ideals-rings.html#2281" class="Function">inclusion-left-ideal-Ring</a> <a id="731" href="ring-theory.nil-ideals-rings.html#471" class="Bound">R</a> <a id="733" href="ring-theory.nil-ideals-rings.html#485" class="Bound">I</a> <a id="735" href="ring-theory.nil-ideals-rings.html#659" class="Bound">x</a><a id="736" class="Symbol">))</a>

  <a id="742" href="ring-theory.nil-ideals-rings.html#742" class="Function">is-nil-left-ideal-Ring</a> <a id="765" class="Symbol">:</a> <a id="767" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="770" class="Symbol">(</a><a id="771" href="ring-theory.nil-ideals-rings.html#455" class="Bound">l1</a> <a id="774" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="776" href="ring-theory.nil-ideals-rings.html#458" class="Bound">l2</a><a id="778" class="Symbol">)</a>
  <a id="782" href="ring-theory.nil-ideals-rings.html#742" class="Function">is-nil-left-ideal-Ring</a> <a id="805" class="Symbol">=</a> <a id="807" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="817" href="ring-theory.nil-ideals-rings.html#524" class="Function">is-nil-left-ideal-ring-Prop</a>

  <a id="848" href="ring-theory.nil-ideals-rings.html#848" class="Function">is-prop-is-nil-left-ideal-Ring</a> <a id="879" class="Symbol">:</a> <a id="881" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="889" href="ring-theory.nil-ideals-rings.html#742" class="Function">is-nil-left-ideal-Ring</a>
  <a id="914" href="ring-theory.nil-ideals-rings.html#848" class="Function">is-prop-is-nil-left-ideal-Ring</a> <a id="945" class="Symbol">=</a>
    <a id="951" href="foundation-core.propositions.html#1562" class="Function">is-prop-type-Prop</a> <a id="969" href="ring-theory.nil-ideals-rings.html#524" class="Function">is-nil-left-ideal-ring-Prop</a>
</pre>
### Nil right ideals

<pre class="Agda"><a id="1032" class="Keyword">module</a> <a id="1039" href="ring-theory.nil-ideals-rings.html#1039" class="Module">_</a>
  <a id="1043" class="Symbol">{</a><a id="1044" href="ring-theory.nil-ideals-rings.html#1044" class="Bound">l1</a> <a id="1047" href="ring-theory.nil-ideals-rings.html#1047" class="Bound">l2</a> <a id="1050" class="Symbol">:</a> <a id="1052" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1057" class="Symbol">}</a> <a id="1059" class="Symbol">(</a><a id="1060" href="ring-theory.nil-ideals-rings.html#1060" class="Bound">R</a> <a id="1062" class="Symbol">:</a> <a id="1064" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="1069" href="ring-theory.nil-ideals-rings.html#1044" class="Bound">l1</a><a id="1071" class="Symbol">)</a> <a id="1073" class="Symbol">(</a><a id="1074" href="ring-theory.nil-ideals-rings.html#1074" class="Bound">I</a> <a id="1076" class="Symbol">:</a> <a id="1078" href="ring-theory.ideals-rings.html#3906" class="Function">right-ideal-Ring</a> <a id="1095" href="ring-theory.nil-ideals-rings.html#1047" class="Bound">l2</a> <a id="1098" href="ring-theory.nil-ideals-rings.html#1060" class="Bound">R</a><a id="1099" class="Symbol">)</a>
  <a id="1103" class="Keyword">where</a>
  
  <a id="1114" href="ring-theory.nil-ideals-rings.html#1114" class="Function">is-nil-right-ideal-ring-Prop</a> <a id="1143" class="Symbol">:</a> <a id="1145" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="1153" class="Symbol">(</a><a id="1154" href="ring-theory.nil-ideals-rings.html#1044" class="Bound">l1</a> <a id="1157" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1159" href="ring-theory.nil-ideals-rings.html#1047" class="Bound">l2</a><a id="1161" class="Symbol">)</a>
  <a id="1165" href="ring-theory.nil-ideals-rings.html#1114" class="Function">is-nil-right-ideal-ring-Prop</a> <a id="1194" class="Symbol">=</a>
    <a id="1200" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
      <a id="1213" class="Symbol">(</a> <a id="1215" href="ring-theory.ideals-rings.html#4337" class="Function">type-right-ideal-Ring</a> <a id="1237" href="ring-theory.nil-ideals-rings.html#1060" class="Bound">R</a> <a id="1239" href="ring-theory.nil-ideals-rings.html#1074" class="Bound">I</a><a id="1240" class="Symbol">)</a>
      <a id="1248" class="Symbol">(</a> <a id="1250" class="Symbol">λ</a> <a id="1252" href="ring-theory.nil-ideals-rings.html#1252" class="Bound">x</a> <a id="1254" class="Symbol">→</a>
        <a id="1264" href="ring-theory.nilpotent-elements-rings.html#591" class="Function">is-nilpotent-element-ring-Prop</a> <a id="1295" href="ring-theory.nil-ideals-rings.html#1060" class="Bound">R</a> <a id="1297" class="Symbol">(</a><a id="1298" href="ring-theory.ideals-rings.html#4446" class="Function">inclusion-right-ideal-Ring</a> <a id="1325" href="ring-theory.nil-ideals-rings.html#1060" class="Bound">R</a> <a id="1327" href="ring-theory.nil-ideals-rings.html#1074" class="Bound">I</a> <a id="1329" href="ring-theory.nil-ideals-rings.html#1252" class="Bound">x</a><a id="1330" class="Symbol">))</a>

  <a id="1336" href="ring-theory.nil-ideals-rings.html#1336" class="Function">is-nil-right-ideal-Ring</a> <a id="1360" class="Symbol">:</a> <a id="1362" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1365" class="Symbol">(</a><a id="1366" href="ring-theory.nil-ideals-rings.html#1044" class="Bound">l1</a> <a id="1369" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1371" href="ring-theory.nil-ideals-rings.html#1047" class="Bound">l2</a><a id="1373" class="Symbol">)</a>
  <a id="1377" href="ring-theory.nil-ideals-rings.html#1336" class="Function">is-nil-right-ideal-Ring</a> <a id="1401" class="Symbol">=</a> <a id="1403" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="1413" href="ring-theory.nil-ideals-rings.html#1114" class="Function">is-nil-right-ideal-ring-Prop</a>

  <a id="1445" href="ring-theory.nil-ideals-rings.html#1445" class="Function">is-prop-is-nil-right-ideal-Ring</a> <a id="1477" class="Symbol">:</a> <a id="1479" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="1487" href="ring-theory.nil-ideals-rings.html#1336" class="Function">is-nil-right-ideal-Ring</a>
  <a id="1513" href="ring-theory.nil-ideals-rings.html#1445" class="Function">is-prop-is-nil-right-ideal-Ring</a> <a id="1545" class="Symbol">=</a>
    <a id="1551" href="foundation-core.propositions.html#1562" class="Function">is-prop-type-Prop</a> <a id="1569" href="ring-theory.nil-ideals-rings.html#1114" class="Function">is-nil-right-ideal-ring-Prop</a>
</pre>
### Nil two-sided ideals

<pre class="Agda"><a id="1637" class="Keyword">module</a> <a id="1644" href="ring-theory.nil-ideals-rings.html#1644" class="Module">_</a>
  <a id="1648" class="Symbol">{</a><a id="1649" href="ring-theory.nil-ideals-rings.html#1649" class="Bound">l1</a> <a id="1652" href="ring-theory.nil-ideals-rings.html#1652" class="Bound">l2</a> <a id="1655" class="Symbol">:</a> <a id="1657" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1662" class="Symbol">}</a> <a id="1664" class="Symbol">(</a><a id="1665" href="ring-theory.nil-ideals-rings.html#1665" class="Bound">R</a> <a id="1667" class="Symbol">:</a> <a id="1669" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="1674" href="ring-theory.nil-ideals-rings.html#1649" class="Bound">l1</a><a id="1676" class="Symbol">)</a> <a id="1678" class="Symbol">(</a><a id="1679" href="ring-theory.nil-ideals-rings.html#1679" class="Bound">I</a> <a id="1681" class="Symbol">:</a> <a id="1683" href="ring-theory.ideals-rings.html#5897" class="Function">two-sided-ideal-Ring</a> <a id="1704" href="ring-theory.nil-ideals-rings.html#1652" class="Bound">l2</a> <a id="1707" href="ring-theory.nil-ideals-rings.html#1665" class="Bound">R</a><a id="1708" class="Symbol">)</a>
  <a id="1712" class="Keyword">where</a>
  
  <a id="1723" href="ring-theory.nil-ideals-rings.html#1723" class="Function">is-nil-two-sided-ideal-ring-Prop</a> <a id="1756" class="Symbol">:</a> <a id="1758" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="1766" class="Symbol">(</a><a id="1767" href="ring-theory.nil-ideals-rings.html#1649" class="Bound">l1</a> <a id="1770" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1772" href="ring-theory.nil-ideals-rings.html#1652" class="Bound">l2</a><a id="1774" class="Symbol">)</a>
  <a id="1778" href="ring-theory.nil-ideals-rings.html#1723" class="Function">is-nil-two-sided-ideal-ring-Prop</a> <a id="1811" class="Symbol">=</a>
    <a id="1817" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
      <a id="1830" class="Symbol">(</a> <a id="1832" href="ring-theory.ideals-rings.html#6366" class="Function">type-two-sided-ideal-Ring</a> <a id="1858" href="ring-theory.nil-ideals-rings.html#1665" class="Bound">R</a> <a id="1860" href="ring-theory.nil-ideals-rings.html#1679" class="Bound">I</a><a id="1861" class="Symbol">)</a>
      <a id="1869" class="Symbol">(</a> <a id="1871" class="Symbol">λ</a> <a id="1873" href="ring-theory.nil-ideals-rings.html#1873" class="Bound">x</a> <a id="1875" class="Symbol">→</a>
        <a id="1885" href="ring-theory.nilpotent-elements-rings.html#591" class="Function">is-nilpotent-element-ring-Prop</a> <a id="1916" href="ring-theory.nil-ideals-rings.html#1665" class="Bound">R</a> <a id="1918" class="Symbol">(</a><a id="1919" href="ring-theory.ideals-rings.html#6487" class="Function">inclusion-two-sided-ideal-Ring</a> <a id="1950" href="ring-theory.nil-ideals-rings.html#1665" class="Bound">R</a> <a id="1952" href="ring-theory.nil-ideals-rings.html#1679" class="Bound">I</a> <a id="1954" href="ring-theory.nil-ideals-rings.html#1873" class="Bound">x</a><a id="1955" class="Symbol">))</a>

  <a id="1961" href="ring-theory.nil-ideals-rings.html#1961" class="Function">is-nil-two-sided-ideal-Ring</a> <a id="1989" class="Symbol">:</a> <a id="1991" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1994" class="Symbol">(</a><a id="1995" href="ring-theory.nil-ideals-rings.html#1649" class="Bound">l1</a> <a id="1998" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2000" href="ring-theory.nil-ideals-rings.html#1652" class="Bound">l2</a><a id="2002" class="Symbol">)</a>
  <a id="2006" href="ring-theory.nil-ideals-rings.html#1961" class="Function">is-nil-two-sided-ideal-Ring</a> <a id="2034" class="Symbol">=</a> <a id="2036" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="2046" href="ring-theory.nil-ideals-rings.html#1723" class="Function">is-nil-two-sided-ideal-ring-Prop</a>

  <a id="2082" href="ring-theory.nil-ideals-rings.html#2082" class="Function">is-prop-is-nil-two-sided-ideal-Ring</a> <a id="2118" class="Symbol">:</a> <a id="2120" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="2128" href="ring-theory.nil-ideals-rings.html#1961" class="Function">is-nil-two-sided-ideal-Ring</a>
  <a id="2158" href="ring-theory.nil-ideals-rings.html#2082" class="Function">is-prop-is-nil-two-sided-ideal-Ring</a> <a id="2194" class="Symbol">=</a>
    <a id="2200" href="foundation-core.propositions.html#1562" class="Function">is-prop-type-Prop</a> <a id="2218" href="ring-theory.nil-ideals-rings.html#1723" class="Function">is-nil-two-sided-ideal-ring-Prop</a>
</pre>