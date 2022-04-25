# Least upper bounds in posets

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="order-theory.least-upper-bounds-posets.html" class="Module">order-theory.least-upper-bounds-posets</a> <a id="130" class="Keyword">where</a>

<a id="137" class="Keyword">open</a> <a id="142" class="Keyword">import</a> <a id="149" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a> <a id="184" class="Keyword">using</a> <a id="190" class="Symbol">(</a><a id="191" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">_×_</a><a id="194" class="Symbol">)</a>
<a id="196" class="Keyword">open</a> <a id="201" class="Keyword">import</a> <a id="208" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="240" class="Keyword">using</a> <a id="246" class="Symbol">(</a><a id="247" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="248" class="Symbol">;</a> <a id="250" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="254" class="Symbol">;</a> <a id="256" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="259" class="Symbol">;</a> <a id="261" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="264" class="Symbol">)</a>
<a id="266" class="Keyword">open</a> <a id="271" class="Keyword">import</a> <a id="278" href="foundation.propositions.html" class="Module">foundation.propositions</a> <a id="302" class="Keyword">using</a>
  <a id="310" class="Symbol">(</a> <a id="312" href="foundation-core.propositions.html#1322" class="Function">UU-Prop</a><a id="319" class="Symbol">;</a> <a id="321" href="foundation-core.propositions.html#1246" class="Function">is-prop</a><a id="328" class="Symbol">;</a> <a id="330" href="foundation-core.propositions.html#1424" class="Function">type-Prop</a><a id="339" class="Symbol">;</a> <a id="341" href="foundation-core.propositions.html#1491" class="Function">is-prop-type-Prop</a><a id="358" class="Symbol">;</a> <a id="360" href="foundation-core.propositions.html#2135" class="Function">all-elements-equal</a><a id="378" class="Symbol">;</a>
    <a id="384" href="foundation-core.propositions.html#2335" class="Function">is-prop-all-elements-equal</a><a id="410" class="Symbol">;</a> <a id="412" href="foundation-core.propositions.html#5805" class="Function">prod-Prop</a><a id="421" class="Symbol">;</a> <a id="423" href="foundation.propositions.html#1941" class="Function">Π-Prop</a><a id="429" class="Symbol">;</a> <a id="431" href="foundation.propositions.html#3552" class="Function">function-Prop</a><a id="444" class="Symbol">)</a>
<a id="446" class="Keyword">open</a> <a id="451" class="Keyword">import</a> <a id="458" href="foundation.subtypes.html" class="Module">foundation.subtypes</a> <a id="478" class="Keyword">using</a> <a id="484" class="Symbol">(</a><a id="485" href="foundation-core.subtypes.html#3381" class="Function">eq-subtype</a><a id="495" class="Symbol">)</a>
<a id="497" class="Keyword">open</a> <a id="502" class="Keyword">import</a> <a id="509" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="536" class="Keyword">using</a> <a id="542" class="Symbol">(</a><a id="543" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="548" class="Symbol">;</a> <a id="550" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="552" class="Symbol">;</a> <a id="554" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="557" class="Symbol">)</a>

<a id="560" class="Keyword">open</a> <a id="565" class="Keyword">import</a> <a id="572" href="order-theory.posets.html" class="Module">order-theory.posets</a> <a id="592" class="Keyword">using</a>
  <a id="600" class="Symbol">(</a> <a id="602" href="order-theory.posets.html#731" class="Function">Poset</a><a id="607" class="Symbol">;</a> <a id="609" href="order-theory.posets.html#1145" class="Function">element-Poset</a><a id="622" class="Symbol">;</a> <a id="624" href="order-theory.posets.html#1194" class="Function">leq-poset-Prop</a><a id="638" class="Symbol">;</a> <a id="640" href="order-theory.posets.html#1983" class="Function">antisymmetric-leq-Poset</a><a id="663" class="Symbol">)</a>
</pre>
## Idea

An upper bound of two elements `x` and `y` in a poset `P` is an element `z` such that both `x ≤ z` and `y ≤ z` hold. A least upper bound of `x` and `y` is an upper bound `z` of `x` and `y` such that `z ≤ w` holds for any upper bound `w` of `x` and `y`.

## Definitions

### Lower bounds of pairs of elements in a poset

<pre class="Agda"><a id="1007" class="Keyword">module</a> <a id="1014" href="order-theory.least-upper-bounds-posets.html#1014" class="Module">_</a>
  <a id="1018" class="Symbol">{</a><a id="1019" href="order-theory.least-upper-bounds-posets.html#1019" class="Bound">l1</a> <a id="1022" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a> <a id="1025" class="Symbol">:</a> <a id="1027" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1032" class="Symbol">}</a> <a id="1034" class="Symbol">(</a><a id="1035" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a> <a id="1037" class="Symbol">:</a> <a id="1039" href="order-theory.posets.html#731" class="Function">Poset</a> <a id="1045" href="order-theory.least-upper-bounds-posets.html#1019" class="Bound">l1</a> <a id="1048" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a><a id="1050" class="Symbol">)</a>
  <a id="1054" class="Keyword">where</a>

  <a id="1063" href="order-theory.least-upper-bounds-posets.html#1063" class="Function">is-upper-bound-poset-Prop</a> <a id="1089" class="Symbol">:</a>
    <a id="1095" class="Symbol">(</a><a id="1096" href="order-theory.least-upper-bounds-posets.html#1096" class="Bound">x</a> <a id="1098" href="order-theory.least-upper-bounds-posets.html#1098" class="Bound">y</a> <a id="1100" href="order-theory.least-upper-bounds-posets.html#1100" class="Bound">z</a> <a id="1102" class="Symbol">:</a> <a id="1104" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="1118" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="1119" class="Symbol">)</a> <a id="1121" class="Symbol">→</a> <a id="1123" href="foundation-core.propositions.html#1322" class="Function">UU-Prop</a> <a id="1131" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a>
  <a id="1136" href="order-theory.least-upper-bounds-posets.html#1063" class="Function">is-upper-bound-poset-Prop</a> <a id="1162" href="order-theory.least-upper-bounds-posets.html#1162" class="Bound">x</a> <a id="1164" href="order-theory.least-upper-bounds-posets.html#1164" class="Bound">y</a> <a id="1166" href="order-theory.least-upper-bounds-posets.html#1166" class="Bound">z</a> <a id="1168" class="Symbol">=</a>
    <a id="1174" href="foundation-core.propositions.html#5805" class="Function">prod-Prop</a> <a id="1184" class="Symbol">(</a><a id="1185" href="order-theory.posets.html#1194" class="Function">leq-poset-Prop</a> <a id="1200" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a> <a id="1202" href="order-theory.least-upper-bounds-posets.html#1162" class="Bound">x</a> <a id="1204" href="order-theory.least-upper-bounds-posets.html#1166" class="Bound">z</a><a id="1205" class="Symbol">)</a> <a id="1207" class="Symbol">(</a><a id="1208" href="order-theory.posets.html#1194" class="Function">leq-poset-Prop</a> <a id="1223" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a> <a id="1225" href="order-theory.least-upper-bounds-posets.html#1164" class="Bound">y</a> <a id="1227" href="order-theory.least-upper-bounds-posets.html#1166" class="Bound">z</a><a id="1228" class="Symbol">)</a>

  <a id="1233" href="order-theory.least-upper-bounds-posets.html#1233" class="Function">is-upper-bound-Poset</a> <a id="1254" class="Symbol">:</a>
    <a id="1260" class="Symbol">(</a><a id="1261" href="order-theory.least-upper-bounds-posets.html#1261" class="Bound">x</a> <a id="1263" href="order-theory.least-upper-bounds-posets.html#1263" class="Bound">y</a> <a id="1265" href="order-theory.least-upper-bounds-posets.html#1265" class="Bound">z</a> <a id="1267" class="Symbol">:</a> <a id="1269" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="1283" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="1284" class="Symbol">)</a> <a id="1286" class="Symbol">→</a> <a id="1288" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1291" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a>
  <a id="1296" href="order-theory.least-upper-bounds-posets.html#1233" class="Function">is-upper-bound-Poset</a> <a id="1317" href="order-theory.least-upper-bounds-posets.html#1317" class="Bound">x</a> <a id="1319" href="order-theory.least-upper-bounds-posets.html#1319" class="Bound">y</a> <a id="1321" href="order-theory.least-upper-bounds-posets.html#1321" class="Bound">z</a> <a id="1323" class="Symbol">=</a> <a id="1325" href="foundation-core.propositions.html#1424" class="Function">type-Prop</a> <a id="1335" class="Symbol">(</a><a id="1336" href="order-theory.least-upper-bounds-posets.html#1063" class="Function">is-upper-bound-poset-Prop</a> <a id="1362" href="order-theory.least-upper-bounds-posets.html#1317" class="Bound">x</a> <a id="1364" href="order-theory.least-upper-bounds-posets.html#1319" class="Bound">y</a> <a id="1366" href="order-theory.least-upper-bounds-posets.html#1321" class="Bound">z</a><a id="1367" class="Symbol">)</a>

  <a id="1372" href="order-theory.least-upper-bounds-posets.html#1372" class="Function">is-prop-is-upper-bound-Poset</a> <a id="1401" class="Symbol">:</a>
    <a id="1407" class="Symbol">(</a><a id="1408" href="order-theory.least-upper-bounds-posets.html#1408" class="Bound">x</a> <a id="1410" href="order-theory.least-upper-bounds-posets.html#1410" class="Bound">y</a> <a id="1412" href="order-theory.least-upper-bounds-posets.html#1412" class="Bound">z</a> <a id="1414" class="Symbol">:</a> <a id="1416" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="1430" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="1431" class="Symbol">)</a> <a id="1433" class="Symbol">→</a> <a id="1435" href="foundation-core.propositions.html#1246" class="Function">is-prop</a> <a id="1443" class="Symbol">(</a><a id="1444" href="order-theory.least-upper-bounds-posets.html#1233" class="Function">is-upper-bound-Poset</a> <a id="1465" href="order-theory.least-upper-bounds-posets.html#1408" class="Bound">x</a> <a id="1467" href="order-theory.least-upper-bounds-posets.html#1410" class="Bound">y</a> <a id="1469" href="order-theory.least-upper-bounds-posets.html#1412" class="Bound">z</a><a id="1470" class="Symbol">)</a>
  <a id="1474" href="order-theory.least-upper-bounds-posets.html#1372" class="Function">is-prop-is-upper-bound-Poset</a> <a id="1503" href="order-theory.least-upper-bounds-posets.html#1503" class="Bound">x</a> <a id="1505" href="order-theory.least-upper-bounds-posets.html#1505" class="Bound">y</a> <a id="1507" href="order-theory.least-upper-bounds-posets.html#1507" class="Bound">z</a> <a id="1509" class="Symbol">=</a>
    <a id="1515" href="foundation-core.propositions.html#1491" class="Function">is-prop-type-Prop</a> <a id="1533" class="Symbol">(</a><a id="1534" href="order-theory.least-upper-bounds-posets.html#1063" class="Function">is-upper-bound-poset-Prop</a> <a id="1560" href="order-theory.least-upper-bounds-posets.html#1503" class="Bound">x</a> <a id="1562" href="order-theory.least-upper-bounds-posets.html#1505" class="Bound">y</a> <a id="1564" href="order-theory.least-upper-bounds-posets.html#1507" class="Bound">z</a><a id="1565" class="Symbol">)</a>

  <a id="1570" href="order-theory.least-upper-bounds-posets.html#1570" class="Function">is-least-upper-bound-poset-Prop</a> <a id="1602" class="Symbol">:</a>
    <a id="1608" class="Symbol">(</a><a id="1609" href="order-theory.least-upper-bounds-posets.html#1609" class="Bound">x</a> <a id="1611" href="order-theory.least-upper-bounds-posets.html#1611" class="Bound">y</a> <a id="1613" href="order-theory.least-upper-bounds-posets.html#1613" class="Bound">z</a> <a id="1615" class="Symbol">:</a> <a id="1617" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="1631" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="1632" class="Symbol">)</a> <a id="1634" class="Symbol">→</a> <a id="1636" href="foundation-core.propositions.html#1322" class="Function">UU-Prop</a> <a id="1644" class="Symbol">(</a><a id="1645" href="order-theory.least-upper-bounds-posets.html#1019" class="Bound">l1</a> <a id="1648" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1650" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a><a id="1652" class="Symbol">)</a>
  <a id="1656" href="order-theory.least-upper-bounds-posets.html#1570" class="Function">is-least-upper-bound-poset-Prop</a> <a id="1688" href="order-theory.least-upper-bounds-posets.html#1688" class="Bound">x</a> <a id="1690" href="order-theory.least-upper-bounds-posets.html#1690" class="Bound">y</a> <a id="1692" href="order-theory.least-upper-bounds-posets.html#1692" class="Bound">z</a> <a id="1694" class="Symbol">=</a>
    <a id="1700" href="foundation-core.propositions.html#5805" class="Function">prod-Prop</a>
      <a id="1716" class="Symbol">(</a> <a id="1718" href="order-theory.least-upper-bounds-posets.html#1063" class="Function">is-upper-bound-poset-Prop</a> <a id="1744" href="order-theory.least-upper-bounds-posets.html#1688" class="Bound">x</a> <a id="1746" href="order-theory.least-upper-bounds-posets.html#1690" class="Bound">y</a> <a id="1748" href="order-theory.least-upper-bounds-posets.html#1692" class="Bound">z</a><a id="1749" class="Symbol">)</a>
      <a id="1757" class="Symbol">(</a> <a id="1759" href="foundation.propositions.html#1941" class="Function">Π-Prop</a>
        <a id="1774" class="Symbol">(</a> <a id="1776" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="1790" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="1791" class="Symbol">)</a>
        <a id="1801" class="Symbol">(</a> <a id="1803" class="Symbol">λ</a> <a id="1805" href="order-theory.least-upper-bounds-posets.html#1805" class="Bound">w</a> <a id="1807" class="Symbol">→</a>
          <a id="1819" href="foundation.propositions.html#3552" class="Function">function-Prop</a>
            <a id="1845" class="Symbol">(</a> <a id="1847" href="order-theory.least-upper-bounds-posets.html#1233" class="Function">is-upper-bound-Poset</a> <a id="1868" href="order-theory.least-upper-bounds-posets.html#1688" class="Bound">x</a> <a id="1870" href="order-theory.least-upper-bounds-posets.html#1690" class="Bound">y</a> <a id="1872" href="order-theory.least-upper-bounds-posets.html#1805" class="Bound">w</a><a id="1873" class="Symbol">)</a>
            <a id="1887" class="Symbol">(</a> <a id="1889" href="order-theory.posets.html#1194" class="Function">leq-poset-Prop</a> <a id="1904" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a> <a id="1906" href="order-theory.least-upper-bounds-posets.html#1692" class="Bound">z</a> <a id="1908" href="order-theory.least-upper-bounds-posets.html#1805" class="Bound">w</a><a id="1909" class="Symbol">)))</a>

  <a id="1916" href="order-theory.least-upper-bounds-posets.html#1916" class="Function">is-least-upper-bound-Poset</a> <a id="1943" class="Symbol">:</a>
    <a id="1949" class="Symbol">(</a><a id="1950" href="order-theory.least-upper-bounds-posets.html#1950" class="Bound">x</a> <a id="1952" href="order-theory.least-upper-bounds-posets.html#1952" class="Bound">y</a> <a id="1954" href="order-theory.least-upper-bounds-posets.html#1954" class="Bound">z</a> <a id="1956" class="Symbol">:</a> <a id="1958" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="1972" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="1973" class="Symbol">)</a> <a id="1975" class="Symbol">→</a> <a id="1977" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1980" class="Symbol">(</a><a id="1981" href="order-theory.least-upper-bounds-posets.html#1019" class="Bound">l1</a> <a id="1984" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1986" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a><a id="1988" class="Symbol">)</a>
  <a id="1992" href="order-theory.least-upper-bounds-posets.html#1916" class="Function">is-least-upper-bound-Poset</a> <a id="2019" href="order-theory.least-upper-bounds-posets.html#2019" class="Bound">x</a> <a id="2021" href="order-theory.least-upper-bounds-posets.html#2021" class="Bound">y</a> <a id="2023" href="order-theory.least-upper-bounds-posets.html#2023" class="Bound">z</a> <a id="2025" class="Symbol">=</a>
    <a id="2031" href="foundation-core.propositions.html#1424" class="Function">type-Prop</a> <a id="2041" class="Symbol">(</a><a id="2042" href="order-theory.least-upper-bounds-posets.html#1570" class="Function">is-least-upper-bound-poset-Prop</a> <a id="2074" href="order-theory.least-upper-bounds-posets.html#2019" class="Bound">x</a> <a id="2076" href="order-theory.least-upper-bounds-posets.html#2021" class="Bound">y</a> <a id="2078" href="order-theory.least-upper-bounds-posets.html#2023" class="Bound">z</a><a id="2079" class="Symbol">)</a>

  <a id="2084" href="order-theory.least-upper-bounds-posets.html#2084" class="Function">is-prop-is-least-upper-bound-Poset</a> <a id="2119" class="Symbol">:</a>
    <a id="2125" class="Symbol">(</a><a id="2126" href="order-theory.least-upper-bounds-posets.html#2126" class="Bound">x</a> <a id="2128" href="order-theory.least-upper-bounds-posets.html#2128" class="Bound">y</a> <a id="2130" href="order-theory.least-upper-bounds-posets.html#2130" class="Bound">z</a> <a id="2132" class="Symbol">:</a> <a id="2134" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="2148" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="2149" class="Symbol">)</a> <a id="2151" class="Symbol">→</a> <a id="2153" href="foundation-core.propositions.html#1246" class="Function">is-prop</a> <a id="2161" class="Symbol">(</a><a id="2162" href="order-theory.least-upper-bounds-posets.html#1916" class="Function">is-least-upper-bound-Poset</a> <a id="2189" href="order-theory.least-upper-bounds-posets.html#2126" class="Bound">x</a> <a id="2191" href="order-theory.least-upper-bounds-posets.html#2128" class="Bound">y</a> <a id="2193" href="order-theory.least-upper-bounds-posets.html#2130" class="Bound">z</a><a id="2194" class="Symbol">)</a>
  <a id="2198" href="order-theory.least-upper-bounds-posets.html#2084" class="Function">is-prop-is-least-upper-bound-Poset</a> <a id="2233" href="order-theory.least-upper-bounds-posets.html#2233" class="Bound">x</a> <a id="2235" href="order-theory.least-upper-bounds-posets.html#2235" class="Bound">y</a> <a id="2237" href="order-theory.least-upper-bounds-posets.html#2237" class="Bound">z</a> <a id="2239" class="Symbol">=</a>
    <a id="2245" href="foundation-core.propositions.html#1491" class="Function">is-prop-type-Prop</a> <a id="2263" class="Symbol">(</a><a id="2264" href="order-theory.least-upper-bounds-posets.html#1570" class="Function">is-least-upper-bound-poset-Prop</a> <a id="2296" href="order-theory.least-upper-bounds-posets.html#2233" class="Bound">x</a> <a id="2298" href="order-theory.least-upper-bounds-posets.html#2235" class="Bound">y</a> <a id="2300" href="order-theory.least-upper-bounds-posets.html#2237" class="Bound">z</a><a id="2301" class="Symbol">)</a>

  <a id="2306" href="order-theory.least-upper-bounds-posets.html#2306" class="Function">has-least-upper-bound-Poset</a> <a id="2334" class="Symbol">:</a>
    <a id="2340" class="Symbol">(</a><a id="2341" href="order-theory.least-upper-bounds-posets.html#2341" class="Bound">x</a> <a id="2343" href="order-theory.least-upper-bounds-posets.html#2343" class="Bound">y</a> <a id="2345" class="Symbol">:</a> <a id="2347" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="2361" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="2362" class="Symbol">)</a> <a id="2364" class="Symbol">→</a> <a id="2366" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2369" class="Symbol">(</a><a id="2370" href="order-theory.least-upper-bounds-posets.html#1019" class="Bound">l1</a> <a id="2373" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2375" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a><a id="2377" class="Symbol">)</a>
  <a id="2381" href="order-theory.least-upper-bounds-posets.html#2306" class="Function">has-least-upper-bound-Poset</a> <a id="2409" href="order-theory.least-upper-bounds-posets.html#2409" class="Bound">x</a> <a id="2411" href="order-theory.least-upper-bounds-posets.html#2411" class="Bound">y</a> <a id="2413" class="Symbol">=</a>
    <a id="2419" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="2421" class="Symbol">(</a><a id="2422" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="2436" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="2437" class="Symbol">)</a> <a id="2439" class="Symbol">(</a><a id="2440" href="order-theory.least-upper-bounds-posets.html#1916" class="Function">is-least-upper-bound-Poset</a> <a id="2467" href="order-theory.least-upper-bounds-posets.html#2409" class="Bound">x</a> <a id="2469" href="order-theory.least-upper-bounds-posets.html#2411" class="Bound">y</a><a id="2470" class="Symbol">)</a>

  <a id="2475" href="order-theory.least-upper-bounds-posets.html#2475" class="Function">all-elements-equal-has-least-upper-bound-Poset</a> <a id="2522" class="Symbol">:</a>
    <a id="2528" class="Symbol">(</a><a id="2529" href="order-theory.least-upper-bounds-posets.html#2529" class="Bound">x</a> <a id="2531" href="order-theory.least-upper-bounds-posets.html#2531" class="Bound">y</a> <a id="2533" class="Symbol">:</a> <a id="2535" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="2549" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="2550" class="Symbol">)</a> <a id="2552" class="Symbol">→</a>
    <a id="2558" href="foundation-core.propositions.html#2135" class="Function">all-elements-equal</a> <a id="2577" class="Symbol">(</a><a id="2578" href="order-theory.least-upper-bounds-posets.html#2306" class="Function">has-least-upper-bound-Poset</a> <a id="2606" href="order-theory.least-upper-bounds-posets.html#2529" class="Bound">x</a> <a id="2608" href="order-theory.least-upper-bounds-posets.html#2531" class="Bound">y</a><a id="2609" class="Symbol">)</a>
  <a id="2613" href="order-theory.least-upper-bounds-posets.html#2475" class="Function">all-elements-equal-has-least-upper-bound-Poset</a> <a id="2660" href="order-theory.least-upper-bounds-posets.html#2660" class="Bound">x</a> <a id="2662" href="order-theory.least-upper-bounds-posets.html#2662" class="Bound">y</a> <a id="2664" class="Symbol">(</a><a id="2665" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2670" href="order-theory.least-upper-bounds-posets.html#2670" class="Bound">u</a> <a id="2672" href="order-theory.least-upper-bounds-posets.html#2672" class="Bound">H</a><a id="2673" class="Symbol">)</a> <a id="2675" class="Symbol">(</a><a id="2676" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2681" href="order-theory.least-upper-bounds-posets.html#2681" class="Bound">v</a> <a id="2683" href="order-theory.least-upper-bounds-posets.html#2683" class="Bound">K</a><a id="2684" class="Symbol">)</a> <a id="2686" class="Symbol">=</a>
    <a id="2692" href="foundation-core.subtypes.html#3381" class="Function">eq-subtype</a>
      <a id="2709" class="Symbol">(</a> <a id="2711" href="order-theory.least-upper-bounds-posets.html#1570" class="Function">is-least-upper-bound-poset-Prop</a> <a id="2743" href="order-theory.least-upper-bounds-posets.html#2660" class="Bound">x</a> <a id="2745" href="order-theory.least-upper-bounds-posets.html#2662" class="Bound">y</a><a id="2746" class="Symbol">)</a>
      <a id="2754" class="Symbol">(</a> <a id="2756" href="order-theory.posets.html#1983" class="Function">antisymmetric-leq-Poset</a> <a id="2780" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a> <a id="2782" href="order-theory.least-upper-bounds-posets.html#2670" class="Bound">u</a> <a id="2784" href="order-theory.least-upper-bounds-posets.html#2681" class="Bound">v</a>
        <a id="2794" class="Symbol">(</a> <a id="2796" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2800" href="order-theory.least-upper-bounds-posets.html#2672" class="Bound">H</a> <a id="2802" href="order-theory.least-upper-bounds-posets.html#2681" class="Bound">v</a> <a id="2804" class="Symbol">(</a><a id="2805" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2809" href="order-theory.least-upper-bounds-posets.html#2683" class="Bound">K</a><a id="2810" class="Symbol">))</a>
        <a id="2821" class="Symbol">(</a> <a id="2823" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2827" href="order-theory.least-upper-bounds-posets.html#2683" class="Bound">K</a> <a id="2829" href="order-theory.least-upper-bounds-posets.html#2670" class="Bound">u</a> <a id="2831" class="Symbol">(</a><a id="2832" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2836" href="order-theory.least-upper-bounds-posets.html#2672" class="Bound">H</a><a id="2837" class="Symbol">)))</a>

  <a id="2844" href="order-theory.least-upper-bounds-posets.html#2844" class="Function">is-prop-has-least-upper-bound-Poset</a> <a id="2880" class="Symbol">:</a>
    <a id="2886" class="Symbol">(</a><a id="2887" href="order-theory.least-upper-bounds-posets.html#2887" class="Bound">x</a> <a id="2889" href="order-theory.least-upper-bounds-posets.html#2889" class="Bound">y</a> <a id="2891" class="Symbol">:</a> <a id="2893" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="2907" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="2908" class="Symbol">)</a> <a id="2910" class="Symbol">→</a> <a id="2912" href="foundation-core.propositions.html#1246" class="Function">is-prop</a> <a id="2920" class="Symbol">(</a><a id="2921" href="order-theory.least-upper-bounds-posets.html#2306" class="Function">has-least-upper-bound-Poset</a> <a id="2949" href="order-theory.least-upper-bounds-posets.html#2887" class="Bound">x</a> <a id="2951" href="order-theory.least-upper-bounds-posets.html#2889" class="Bound">y</a><a id="2952" class="Symbol">)</a>
  <a id="2956" href="order-theory.least-upper-bounds-posets.html#2844" class="Function">is-prop-has-least-upper-bound-Poset</a> <a id="2992" href="order-theory.least-upper-bounds-posets.html#2992" class="Bound">x</a> <a id="2994" href="order-theory.least-upper-bounds-posets.html#2994" class="Bound">y</a> <a id="2996" class="Symbol">=</a>
    <a id="3002" href="foundation-core.propositions.html#2335" class="Function">is-prop-all-elements-equal</a>
      <a id="3035" class="Symbol">(</a> <a id="3037" href="order-theory.least-upper-bounds-posets.html#2475" class="Function">all-elements-equal-has-least-upper-bound-Poset</a> <a id="3084" href="order-theory.least-upper-bounds-posets.html#2992" class="Bound">x</a> <a id="3086" href="order-theory.least-upper-bounds-posets.html#2994" class="Bound">y</a><a id="3087" class="Symbol">)</a>

  <a id="3092" href="order-theory.least-upper-bounds-posets.html#3092" class="Function">has-least-upper-bound-poset-Prop</a> <a id="3125" class="Symbol">:</a>
    <a id="3131" class="Symbol">(</a><a id="3132" href="order-theory.least-upper-bounds-posets.html#3132" class="Bound">x</a> <a id="3134" href="order-theory.least-upper-bounds-posets.html#3134" class="Bound">y</a> <a id="3136" class="Symbol">:</a> <a id="3138" href="order-theory.posets.html#1145" class="Function">element-Poset</a> <a id="3152" href="order-theory.least-upper-bounds-posets.html#1035" class="Bound">P</a><a id="3153" class="Symbol">)</a> <a id="3155" class="Symbol">→</a> <a id="3157" href="foundation-core.propositions.html#1322" class="Function">UU-Prop</a> <a id="3165" class="Symbol">(</a><a id="3166" href="order-theory.least-upper-bounds-posets.html#1019" class="Bound">l1</a> <a id="3169" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3171" href="order-theory.least-upper-bounds-posets.html#1022" class="Bound">l2</a><a id="3173" class="Symbol">)</a>
  <a id="3177" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="3181" class="Symbol">(</a><a id="3182" href="order-theory.least-upper-bounds-posets.html#3092" class="Function">has-least-upper-bound-poset-Prop</a> <a id="3215" href="order-theory.least-upper-bounds-posets.html#3215" class="Bound">x</a> <a id="3217" href="order-theory.least-upper-bounds-posets.html#3217" class="Bound">y</a><a id="3218" class="Symbol">)</a> <a id="3220" class="Symbol">=</a>
    <a id="3226" href="order-theory.least-upper-bounds-posets.html#2306" class="Function">has-least-upper-bound-Poset</a> <a id="3254" href="order-theory.least-upper-bounds-posets.html#3215" class="Bound">x</a> <a id="3256" href="order-theory.least-upper-bounds-posets.html#3217" class="Bound">y</a>
  <a id="3260" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="3264" class="Symbol">(</a><a id="3265" href="order-theory.least-upper-bounds-posets.html#3092" class="Function">has-least-upper-bound-poset-Prop</a> <a id="3298" href="order-theory.least-upper-bounds-posets.html#3298" class="Bound">x</a> <a id="3300" href="order-theory.least-upper-bounds-posets.html#3300" class="Bound">y</a><a id="3301" class="Symbol">)</a> <a id="3303" class="Symbol">=</a>
    <a id="3309" href="order-theory.least-upper-bounds-posets.html#2844" class="Function">is-prop-has-least-upper-bound-Poset</a> <a id="3345" href="order-theory.least-upper-bounds-posets.html#3298" class="Bound">x</a> <a id="3347" href="order-theory.least-upper-bounds-posets.html#3300" class="Bound">y</a>
</pre>