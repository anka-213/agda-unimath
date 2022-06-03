---
title: Large Posets
---

<pre class="Agda"><a id="38" class="Symbol">{-#</a> <a id="42" class="Keyword">OPTIONS</a> <a id="50" class="Pragma">--without-K</a> <a id="62" class="Pragma">--exact-split</a> <a id="76" class="Symbol">#-}</a>

<a id="81" class="Keyword">module</a> <a id="88" href="order-theory.large-posets.html" class="Module">order-theory.large-posets</a> <a id="114" class="Keyword">where</a>

<a id="121" class="Keyword">open</a> <a id="126" class="Keyword">import</a> <a id="133" href="Agda.Primitive.html" class="Module">Agda.Primitive</a> <a id="148" class="Keyword">using</a> <a id="154" class="Symbol">(</a><a id="155" href="Agda.Primitive.html#381" class="Primitive">Setω</a><a id="159" class="Symbol">)</a>

<a id="162" class="Keyword">open</a> <a id="167" class="Keyword">import</a> <a id="174" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="206" class="Keyword">open</a> <a id="211" class="Keyword">import</a> <a id="218" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="244" class="Keyword">open</a> <a id="249" class="Keyword">import</a> <a id="256" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="280" class="Keyword">open</a> <a id="285" class="Keyword">import</a> <a id="292" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="320" class="Keyword">open</a> <a id="325" class="Keyword">import</a> <a id="332" href="order-theory.large-preorders.html" class="Module">order-theory.large-preorders</a>
<a id="361" class="Keyword">open</a> <a id="366" class="Keyword">import</a> <a id="373" href="order-theory.posets.html" class="Module">order-theory.posets</a>
</pre>
## Idea

A large poset is a large preorder such that the restriction of the ordering relation to any particular universe level is antisymmetric

## Definition

<pre class="Agda"><a id="566" class="Keyword">record</a>
  <a id="Large-Poset"></a><a id="575" href="order-theory.large-posets.html#575" class="Record">Large-Poset</a> <a id="587" class="Symbol">(</a><a id="588" href="order-theory.large-posets.html#588" class="Bound">α</a> <a id="590" class="Symbol">:</a> <a id="592" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="598" class="Symbol">→</a> <a id="600" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="605" class="Symbol">)</a> <a id="607" class="Symbol">(</a><a id="608" href="order-theory.large-posets.html#608" class="Bound">β</a> <a id="610" class="Symbol">:</a> <a id="612" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="618" class="Symbol">→</a> <a id="620" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="626" class="Symbol">→</a> <a id="628" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="633" class="Symbol">)</a> <a id="635" class="Symbol">:</a> <a id="637" href="Agda.Primitive.html#381" class="Primitive">Setω</a> <a id="642" class="Keyword">where</a>
  <a id="650" class="Keyword">constructor</a>
    <a id="make-Large-Poset"></a><a id="666" href="order-theory.large-posets.html#666" class="InductiveConstructor">make-Large-Poset</a>
  <a id="685" class="Keyword">field</a>
    <a id="Large-Poset.large-preorder-Large-Poset"></a><a id="695" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="722" class="Symbol">:</a> <a id="724" href="order-theory.large-preorders.html#744" class="Record">Large-Preorder</a> <a id="739" href="order-theory.large-posets.html#588" class="Bound">α</a> <a id="741" href="order-theory.large-posets.html#608" class="Bound">β</a>
    <a id="Large-Poset.antisymmetric-leq-Large-Poset"></a><a id="747" href="order-theory.large-posets.html#747" class="Field">antisymmetric-leq-Large-Poset</a> <a id="777" class="Symbol">:</a>
      <a id="785" class="Symbol">{</a><a id="786" href="order-theory.large-posets.html#786" class="Bound">l</a> <a id="788" class="Symbol">:</a> <a id="790" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="795" class="Symbol">}</a> <a id="797" class="Symbol">(</a><a id="798" href="order-theory.large-posets.html#798" class="Bound">x</a> <a id="800" href="order-theory.large-posets.html#800" class="Bound">y</a> <a id="802" class="Symbol">:</a> <a id="804" href="order-theory.large-preorders.html#870" class="Field">type-Large-Preorder</a> <a id="824" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="851" href="order-theory.large-posets.html#786" class="Bound">l</a><a id="852" class="Symbol">)</a> <a id="854" class="Symbol">→</a>
      <a id="862" href="order-theory.large-preorders.html#1586" class="Function">leq-Large-Preorder</a> <a id="881" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="908" href="order-theory.large-posets.html#798" class="Bound">x</a> <a id="910" href="order-theory.large-posets.html#800" class="Bound">y</a> <a id="912" class="Symbol">→</a>
      <a id="920" href="order-theory.large-preorders.html#1586" class="Function">leq-Large-Preorder</a> <a id="939" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="966" href="order-theory.large-posets.html#800" class="Bound">y</a> <a id="968" href="order-theory.large-posets.html#798" class="Bound">x</a> <a id="970" class="Symbol">→</a> <a id="972" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="975" href="order-theory.large-posets.html#798" class="Bound">x</a> <a id="977" href="order-theory.large-posets.html#800" class="Bound">y</a>

<a id="980" class="Keyword">open</a> <a id="985" href="order-theory.large-posets.html#575" class="Module">Large-Poset</a> <a id="997" class="Keyword">public</a>

<a id="1005" class="Keyword">module</a> <a id="1012" href="order-theory.large-posets.html#1012" class="Module">_</a>
  <a id="1016" class="Symbol">{</a><a id="1017" href="order-theory.large-posets.html#1017" class="Bound">α</a> <a id="1019" class="Symbol">:</a> <a id="1021" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="1027" class="Symbol">→</a> <a id="1029" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1034" class="Symbol">}</a> <a id="1036" class="Symbol">{</a><a id="1037" href="order-theory.large-posets.html#1037" class="Bound">β</a> <a id="1039" class="Symbol">:</a> <a id="1041" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="1047" class="Symbol">→</a> <a id="1049" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="1055" class="Symbol">→</a> <a id="1057" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1062" class="Symbol">}</a> <a id="1064" class="Symbol">(</a><a id="1065" href="order-theory.large-posets.html#1065" class="Bound">X</a> <a id="1067" class="Symbol">:</a> <a id="1069" href="order-theory.large-posets.html#575" class="Record">Large-Poset</a> <a id="1081" href="order-theory.large-posets.html#1017" class="Bound">α</a> <a id="1083" href="order-theory.large-posets.html#1037" class="Bound">β</a><a id="1084" class="Symbol">)</a>
  <a id="1088" class="Keyword">where</a>

  <a id="1097" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1114" class="Symbol">:</a> <a id="1116" class="Symbol">(</a><a id="1117" href="order-theory.large-posets.html#1117" class="Bound">l</a> <a id="1119" class="Symbol">:</a> <a id="1121" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1126" class="Symbol">)</a> <a id="1128" class="Symbol">→</a> <a id="1130" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1133" class="Symbol">(</a><a id="1134" href="order-theory.large-posets.html#1017" class="Bound">α</a> <a id="1136" href="order-theory.large-posets.html#1117" class="Bound">l</a><a id="1137" class="Symbol">)</a>
  <a id="1141" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1158" class="Symbol">=</a> <a id="1160" href="order-theory.large-preorders.html#870" class="Field">type-Large-Preorder</a> <a id="1180" class="Symbol">(</a><a id="1181" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="1208" href="order-theory.large-posets.html#1065" class="Bound">X</a><a id="1209" class="Symbol">)</a>

  <a id="1214" href="order-theory.large-posets.html#1214" class="Function">leq-large-poset-Prop</a> <a id="1235" class="Symbol">:</a>
    <a id="1241" class="Symbol">{</a><a id="1242" href="order-theory.large-posets.html#1242" class="Bound">l1</a> <a id="1245" href="order-theory.large-posets.html#1245" class="Bound">l2</a> <a id="1248" class="Symbol">:</a> <a id="1250" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1255" class="Symbol">}</a> <a id="1257" class="Symbol">→</a> <a id="1259" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1276" href="order-theory.large-posets.html#1242" class="Bound">l1</a> <a id="1279" class="Symbol">→</a> <a id="1281" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1298" href="order-theory.large-posets.html#1245" class="Bound">l2</a> <a id="1301" class="Symbol">→</a>
    <a id="1307" href="foundation-core.propositions.html#1380" class="Function">UU-Prop</a> <a id="1315" class="Symbol">(</a><a id="1316" href="order-theory.large-posets.html#1037" class="Bound">β</a> <a id="1318" href="order-theory.large-posets.html#1242" class="Bound">l1</a> <a id="1321" href="order-theory.large-posets.html#1245" class="Bound">l2</a><a id="1323" class="Symbol">)</a>
  <a id="1327" href="order-theory.large-posets.html#1214" class="Function">leq-large-poset-Prop</a> <a id="1348" class="Symbol">=</a> <a id="1350" href="order-theory.large-preorders.html#919" class="Field">leq-large-preorder-Prop</a> <a id="1374" class="Symbol">(</a><a id="1375" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="1402" href="order-theory.large-posets.html#1065" class="Bound">X</a><a id="1403" class="Symbol">)</a>

  <a id="1408" href="order-theory.large-posets.html#1408" class="Function">leq-Large-Poset</a> <a id="1424" class="Symbol">:</a>
    <a id="1430" class="Symbol">{</a><a id="1431" href="order-theory.large-posets.html#1431" class="Bound">l1</a> <a id="1434" href="order-theory.large-posets.html#1434" class="Bound">l2</a> <a id="1437" class="Symbol">:</a> <a id="1439" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1444" class="Symbol">}</a> <a id="1446" class="Symbol">→</a> <a id="1448" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1465" href="order-theory.large-posets.html#1431" class="Bound">l1</a> <a id="1468" class="Symbol">→</a> <a id="1470" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1487" href="order-theory.large-posets.html#1434" class="Bound">l2</a> <a id="1490" class="Symbol">→</a> <a id="1492" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1495" class="Symbol">(</a><a id="1496" href="order-theory.large-posets.html#1037" class="Bound">β</a> <a id="1498" href="order-theory.large-posets.html#1431" class="Bound">l1</a> <a id="1501" href="order-theory.large-posets.html#1434" class="Bound">l2</a><a id="1503" class="Symbol">)</a>
  <a id="1507" href="order-theory.large-posets.html#1408" class="Function">leq-Large-Poset</a> <a id="1523" class="Symbol">=</a> <a id="1525" href="order-theory.large-preorders.html#1586" class="Function">leq-Large-Preorder</a> <a id="1544" class="Symbol">(</a><a id="1545" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="1572" href="order-theory.large-posets.html#1065" class="Bound">X</a><a id="1573" class="Symbol">)</a>

  <a id="1578" href="order-theory.large-posets.html#1578" class="Function">is-prop-leq-Large-Poset</a> <a id="1602" class="Symbol">:</a>
    <a id="1608" class="Symbol">{</a><a id="1609" href="order-theory.large-posets.html#1609" class="Bound">l1</a> <a id="1612" href="order-theory.large-posets.html#1612" class="Bound">l2</a> <a id="1615" class="Symbol">:</a> <a id="1617" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1622" class="Symbol">}</a> <a id="1624" class="Symbol">(</a><a id="1625" href="order-theory.large-posets.html#1625" class="Bound">x</a> <a id="1627" class="Symbol">:</a> <a id="1629" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1646" href="order-theory.large-posets.html#1609" class="Bound">l1</a><a id="1648" class="Symbol">)</a> <a id="1650" class="Symbol">(</a><a id="1651" href="order-theory.large-posets.html#1651" class="Bound">y</a> <a id="1653" class="Symbol">:</a> <a id="1655" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1672" href="order-theory.large-posets.html#1612" class="Bound">l2</a><a id="1674" class="Symbol">)</a> <a id="1676" class="Symbol">→</a>
    <a id="1682" href="foundation-core.propositions.html#1295" class="Function">is-prop</a> <a id="1690" class="Symbol">(</a><a id="1691" href="order-theory.large-posets.html#1408" class="Function">leq-Large-Poset</a> <a id="1707" href="order-theory.large-posets.html#1625" class="Bound">x</a> <a id="1709" href="order-theory.large-posets.html#1651" class="Bound">y</a><a id="1710" class="Symbol">)</a>
  <a id="1714" href="order-theory.large-posets.html#1578" class="Function">is-prop-leq-Large-Poset</a> <a id="1738" class="Symbol">=</a>
    <a id="1744" href="order-theory.large-preorders.html#1772" class="Function">is-prop-leq-Large-Preorder</a> <a id="1771" class="Symbol">(</a><a id="1772" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="1799" href="order-theory.large-posets.html#1065" class="Bound">X</a><a id="1800" class="Symbol">)</a>

  <a id="1805" href="order-theory.large-posets.html#1805" class="Function">refl-leq-Large-Poset</a> <a id="1826" class="Symbol">:</a>
    <a id="1832" class="Symbol">{</a><a id="1833" href="order-theory.large-posets.html#1833" class="Bound">l1</a> <a id="1836" class="Symbol">:</a> <a id="1838" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1843" class="Symbol">}</a> <a id="1845" class="Symbol">(</a><a id="1846" href="order-theory.large-posets.html#1846" class="Bound">x</a> <a id="1848" class="Symbol">:</a> <a id="1850" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="1867" href="order-theory.large-posets.html#1833" class="Bound">l1</a><a id="1869" class="Symbol">)</a> <a id="1871" class="Symbol">→</a> <a id="1873" href="order-theory.large-posets.html#1408" class="Function">leq-Large-Poset</a> <a id="1889" href="order-theory.large-posets.html#1846" class="Bound">x</a> <a id="1891" href="order-theory.large-posets.html#1846" class="Bound">x</a>
  <a id="1895" href="order-theory.large-posets.html#1805" class="Function">refl-leq-Large-Poset</a> <a id="1916" class="Symbol">=</a> <a id="1918" href="order-theory.large-preorders.html#1047" class="Field">refl-leq-Large-Preorder</a> <a id="1942" class="Symbol">(</a><a id="1943" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="1970" href="order-theory.large-posets.html#1065" class="Bound">X</a><a id="1971" class="Symbol">)</a>

  <a id="1976" href="order-theory.large-posets.html#1976" class="Function">trans-leq-Large-Poset</a> <a id="1998" class="Symbol">:</a>
    <a id="2004" class="Symbol">{</a><a id="2005" href="order-theory.large-posets.html#2005" class="Bound">l1</a> <a id="2008" href="order-theory.large-posets.html#2008" class="Bound">l2</a> <a id="2011" href="order-theory.large-posets.html#2011" class="Bound">l3</a> <a id="2014" class="Symbol">:</a> <a id="2016" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2021" class="Symbol">}</a> <a id="2023" class="Symbol">(</a><a id="2024" href="order-theory.large-posets.html#2024" class="Bound">x</a> <a id="2026" class="Symbol">:</a> <a id="2028" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="2045" href="order-theory.large-posets.html#2005" class="Bound">l1</a><a id="2047" class="Symbol">)</a> <a id="2049" class="Symbol">(</a><a id="2050" href="order-theory.large-posets.html#2050" class="Bound">y</a> <a id="2052" class="Symbol">:</a> <a id="2054" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="2071" href="order-theory.large-posets.html#2008" class="Bound">l2</a><a id="2073" class="Symbol">)</a>
    <a id="2079" class="Symbol">(</a><a id="2080" href="order-theory.large-posets.html#2080" class="Bound">z</a> <a id="2082" class="Symbol">:</a> <a id="2084" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="2101" href="order-theory.large-posets.html#2011" class="Bound">l3</a><a id="2103" class="Symbol">)</a> <a id="2105" class="Symbol">→</a>
    <a id="2111" href="order-theory.large-posets.html#1408" class="Function">leq-Large-Poset</a> <a id="2127" href="order-theory.large-posets.html#2050" class="Bound">y</a> <a id="2129" href="order-theory.large-posets.html#2080" class="Bound">z</a> <a id="2131" class="Symbol">→</a> <a id="2133" href="order-theory.large-posets.html#1408" class="Function">leq-Large-Poset</a> <a id="2149" href="order-theory.large-posets.html#2024" class="Bound">x</a> <a id="2151" href="order-theory.large-posets.html#2050" class="Bound">y</a> <a id="2153" class="Symbol">→</a> <a id="2155" href="order-theory.large-posets.html#1408" class="Function">leq-Large-Poset</a> <a id="2171" href="order-theory.large-posets.html#2024" class="Bound">x</a> <a id="2173" href="order-theory.large-posets.html#2080" class="Bound">z</a>
  <a id="2177" href="order-theory.large-posets.html#1976" class="Function">trans-leq-Large-Poset</a> <a id="2199" class="Symbol">=</a>
    <a id="2205" href="order-theory.large-preorders.html#1173" class="Field">trans-leq-Large-Preorder</a> <a id="2230" class="Symbol">(</a><a id="2231" href="order-theory.large-posets.html#695" class="Field">large-preorder-Large-Poset</a> <a id="2258" href="order-theory.large-posets.html#1065" class="Bound">X</a><a id="2259" class="Symbol">)</a>

  <a id="2264" href="order-theory.large-posets.html#2264" class="Function">poset-Large-Poset</a> <a id="2282" class="Symbol">:</a> <a id="2284" class="Symbol">(</a><a id="2285" href="order-theory.large-posets.html#2285" class="Bound">l</a> <a id="2287" class="Symbol">:</a> <a id="2289" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2294" class="Symbol">)</a> <a id="2296" class="Symbol">→</a> <a id="2298" href="order-theory.posets.html#731" class="Function">Poset</a> <a id="2304" class="Symbol">(</a><a id="2305" href="order-theory.large-posets.html#1017" class="Bound">α</a> <a id="2307" href="order-theory.large-posets.html#2285" class="Bound">l</a><a id="2308" class="Symbol">)</a> <a id="2310" class="Symbol">(</a><a id="2311" href="order-theory.large-posets.html#1037" class="Bound">β</a> <a id="2313" href="order-theory.large-posets.html#2285" class="Bound">l</a> <a id="2315" href="order-theory.large-posets.html#2285" class="Bound">l</a><a id="2316" class="Symbol">)</a>
  <a id="2320" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2324" class="Symbol">(</a><a id="2325" href="order-theory.large-posets.html#2264" class="Function">poset-Large-Poset</a> <a id="2343" href="order-theory.large-posets.html#2343" class="Bound">l</a><a id="2344" class="Symbol">)</a> <a id="2346" class="Symbol">=</a> <a id="2348" href="order-theory.large-posets.html#1097" class="Function">type-Large-Poset</a> <a id="2365" href="order-theory.large-posets.html#2343" class="Bound">l</a>
  <a id="2369" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2373" class="Symbol">(</a><a id="2374" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2378" class="Symbol">(</a><a id="2379" href="order-theory.large-posets.html#2264" class="Function">poset-Large-Poset</a> <a id="2397" href="order-theory.large-posets.html#2397" class="Bound">l</a><a id="2398" class="Symbol">))</a> <a id="2401" class="Symbol">=</a> <a id="2403" href="order-theory.large-posets.html#1214" class="Function">leq-large-poset-Prop</a>
  <a id="2426" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2430" class="Symbol">(</a><a id="2431" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2435" class="Symbol">(</a><a id="2436" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2440" class="Symbol">(</a><a id="2441" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2445" class="Symbol">(</a><a id="2446" href="order-theory.large-posets.html#2264" class="Function">poset-Large-Poset</a> <a id="2464" href="order-theory.large-posets.html#2464" class="Bound">l</a><a id="2465" class="Symbol">))))</a> <a id="2470" class="Symbol">=</a> <a id="2472" href="order-theory.large-posets.html#1805" class="Function">refl-leq-Large-Poset</a>
  <a id="2495" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2499" class="Symbol">(</a><a id="2500" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2504" class="Symbol">(</a><a id="2505" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2509" class="Symbol">(</a><a id="2510" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2514" class="Symbol">(</a><a id="2515" href="order-theory.large-posets.html#2264" class="Function">poset-Large-Poset</a> <a id="2533" href="order-theory.large-posets.html#2533" class="Bound">l</a><a id="2534" class="Symbol">))))</a> <a id="2539" class="Symbol">=</a> <a id="2541" href="order-theory.large-posets.html#1976" class="Function">trans-leq-Large-Poset</a>
  <a id="2565" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2569" class="Symbol">(</a><a id="2570" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2574" class="Symbol">(</a><a id="2575" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2579" class="Symbol">(</a><a id="2580" href="order-theory.large-posets.html#2264" class="Function">poset-Large-Poset</a> <a id="2598" href="order-theory.large-posets.html#2598" class="Bound">l</a><a id="2599" class="Symbol">)))</a> <a id="2603" class="Symbol">=</a> <a id="2605" href="order-theory.large-posets.html#747" class="Field">antisymmetric-leq-Large-Poset</a> <a id="2635" href="order-theory.large-posets.html#1065" class="Bound">X</a>
</pre>