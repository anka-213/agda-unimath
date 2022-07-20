---
title: Local rings
---

<pre class="Agda"><a id="37" class="Symbol">{-#</a> <a id="41" class="Keyword">OPTIONS</a> <a id="49" class="Pragma">--without-K</a> <a id="61" class="Pragma">--exact-split</a> <a id="75" class="Symbol">#-}</a>

<a id="80" class="Keyword">module</a> <a id="87" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a> <a id="111" class="Keyword">where</a>

<a id="118" class="Keyword">open</a> <a id="123" class="Keyword">import</a> <a id="130" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="165" class="Keyword">open</a> <a id="170" class="Keyword">import</a> <a id="177" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="209" class="Keyword">open</a> <a id="214" class="Keyword">import</a> <a id="221" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="244" class="Keyword">open</a> <a id="249" class="Keyword">import</a> <a id="256" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="280" class="Keyword">open</a> <a id="285" class="Keyword">import</a> <a id="292" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="308" class="Keyword">open</a> <a id="313" class="Keyword">import</a> <a id="320" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="348" class="Keyword">open</a> <a id="353" class="Keyword">import</a> <a id="360" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a>
<a id="398" class="Keyword">open</a> <a id="403" class="Keyword">import</a> <a id="410" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a>
<a id="439" class="Keyword">open</a> <a id="444" class="Keyword">import</a> <a id="451" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Idea

A local ring is a ring such that whenever a sum of elements is invertible, then one of its summands is invertible. This implies that the non-invertible elements form an ideal. However, the law of excluded middle is needed to show that any ring of which the non-invertible elements form an ideal is a local ring.

## Definition

<pre class="Agda"><a id="is-local-ring-Prop"></a><a id="819" href="ring-theory.local-rings.html#819" class="Function">is-local-ring-Prop</a> <a id="838" class="Symbol">:</a> <a id="840" class="Symbol">{</a><a id="841" href="ring-theory.local-rings.html#841" class="Bound">l</a> <a id="843" class="Symbol">:</a> <a id="845" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="850" class="Symbol">}</a> <a id="852" class="Symbol">(</a><a id="853" href="ring-theory.local-rings.html#853" class="Bound">R</a> <a id="855" class="Symbol">:</a> <a id="857" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="862" href="ring-theory.local-rings.html#841" class="Bound">l</a><a id="863" class="Symbol">)</a> <a id="865" class="Symbol">→</a> <a id="867" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="875" href="ring-theory.local-rings.html#841" class="Bound">l</a>
<a id="877" href="ring-theory.local-rings.html#819" class="Function">is-local-ring-Prop</a> <a id="896" href="ring-theory.local-rings.html#896" class="Bound">R</a> <a id="898" class="Symbol">=</a>
  <a id="902" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
    <a id="913" class="Symbol">(</a> <a id="915" href="ring-theory.rings.html#2808" class="Function">type-Ring</a> <a id="925" href="ring-theory.local-rings.html#896" class="Bound">R</a><a id="926" class="Symbol">)</a>
    <a id="932" class="Symbol">(</a> <a id="934" class="Symbol">λ</a> <a id="936" href="ring-theory.local-rings.html#936" class="Bound">a</a> <a id="938" class="Symbol">→</a>
      <a id="946" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
        <a id="961" class="Symbol">(</a> <a id="963" href="ring-theory.rings.html#2808" class="Function">type-Ring</a> <a id="973" href="ring-theory.local-rings.html#896" class="Bound">R</a><a id="974" class="Symbol">)</a>
        <a id="984" class="Symbol">(</a> <a id="986" class="Symbol">λ</a> <a id="988" href="ring-theory.local-rings.html#988" class="Bound">b</a> <a id="990" class="Symbol">→</a>
          <a id="1002" href="foundation-core.propositions.html#8294" class="Function">function-Prop</a>
            <a id="1028" class="Symbol">(</a> <a id="1030" href="ring-theory.invertible-elements-rings.html#1491" class="Function">is-invertible-element-Ring</a> <a id="1057" href="ring-theory.local-rings.html#896" class="Bound">R</a> <a id="1059" class="Symbol">(</a><a id="1060" href="ring-theory.rings.html#3153" class="Function">add-Ring</a> <a id="1069" href="ring-theory.local-rings.html#896" class="Bound">R</a> <a id="1071" href="ring-theory.local-rings.html#936" class="Bound">a</a> <a id="1073" href="ring-theory.local-rings.html#988" class="Bound">b</a><a id="1074" class="Symbol">))</a>
            <a id="1089" class="Symbol">(</a> <a id="1091" href="foundation.disjunction.html#1145" class="Function">disj-Prop</a>
              <a id="1115" class="Symbol">(</a> <a id="1117" href="ring-theory.invertible-elements-rings.html#1321" class="Function">is-invertible-element-ring-Prop</a> <a id="1149" href="ring-theory.local-rings.html#896" class="Bound">R</a> <a id="1151" href="ring-theory.local-rings.html#936" class="Bound">a</a><a id="1152" class="Symbol">)</a>
              <a id="1168" class="Symbol">(</a> <a id="1170" href="ring-theory.invertible-elements-rings.html#1321" class="Function">is-invertible-element-ring-Prop</a> <a id="1202" href="ring-theory.local-rings.html#896" class="Bound">R</a> <a id="1204" href="ring-theory.local-rings.html#988" class="Bound">b</a><a id="1205" class="Symbol">))))</a>

<a id="is-local-Ring"></a><a id="1211" href="ring-theory.local-rings.html#1211" class="Function">is-local-Ring</a> <a id="1225" class="Symbol">:</a> <a id="1227" class="Symbol">{</a><a id="1228" href="ring-theory.local-rings.html#1228" class="Bound">l</a> <a id="1230" class="Symbol">:</a> <a id="1232" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1237" class="Symbol">}</a> <a id="1239" class="Symbol">→</a> <a id="1241" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="1246" href="ring-theory.local-rings.html#1228" class="Bound">l</a> <a id="1248" class="Symbol">→</a> <a id="1250" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1253" href="ring-theory.local-rings.html#1228" class="Bound">l</a>
<a id="1255" href="ring-theory.local-rings.html#1211" class="Function">is-local-Ring</a> <a id="1269" href="ring-theory.local-rings.html#1269" class="Bound">R</a> <a id="1271" class="Symbol">=</a> <a id="1273" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="1283" class="Symbol">(</a><a id="1284" href="ring-theory.local-rings.html#819" class="Function">is-local-ring-Prop</a> <a id="1303" href="ring-theory.local-rings.html#1269" class="Bound">R</a><a id="1304" class="Symbol">)</a>

<a id="is-prop-is-local-Ring"></a><a id="1307" href="ring-theory.local-rings.html#1307" class="Function">is-prop-is-local-Ring</a> <a id="1329" class="Symbol">:</a> <a id="1331" class="Symbol">{</a><a id="1332" href="ring-theory.local-rings.html#1332" class="Bound">l</a> <a id="1334" class="Symbol">:</a> <a id="1336" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1341" class="Symbol">}</a> <a id="1343" class="Symbol">(</a><a id="1344" href="ring-theory.local-rings.html#1344" class="Bound">R</a> <a id="1346" class="Symbol">:</a> <a id="1348" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="1353" href="ring-theory.local-rings.html#1332" class="Bound">l</a><a id="1354" class="Symbol">)</a> <a id="1356" class="Symbol">→</a> <a id="1358" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="1366" class="Symbol">(</a><a id="1367" href="ring-theory.local-rings.html#1211" class="Function">is-local-Ring</a> <a id="1381" href="ring-theory.local-rings.html#1344" class="Bound">R</a><a id="1382" class="Symbol">)</a>
<a id="1384" href="ring-theory.local-rings.html#1307" class="Function">is-prop-is-local-Ring</a> <a id="1406" href="ring-theory.local-rings.html#1406" class="Bound">R</a> <a id="1408" class="Symbol">=</a> <a id="1410" href="foundation-core.propositions.html#1562" class="Function">is-prop-type-Prop</a> <a id="1428" class="Symbol">(</a><a id="1429" href="ring-theory.local-rings.html#819" class="Function">is-local-ring-Prop</a> <a id="1448" href="ring-theory.local-rings.html#1406" class="Bound">R</a><a id="1449" class="Symbol">)</a>

<a id="Local-Ring"></a><a id="1452" href="ring-theory.local-rings.html#1452" class="Function">Local-Ring</a> <a id="1463" class="Symbol">:</a> <a id="1465" class="Symbol">(</a><a id="1466" href="ring-theory.local-rings.html#1466" class="Bound">l</a> <a id="1468" class="Symbol">:</a> <a id="1470" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1475" class="Symbol">)</a> <a id="1477" class="Symbol">→</a> <a id="1479" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1482" class="Symbol">(</a><a id="1483" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1488" href="ring-theory.local-rings.html#1466" class="Bound">l</a><a id="1489" class="Symbol">)</a>
<a id="1491" href="ring-theory.local-rings.html#1452" class="Function">Local-Ring</a> <a id="1502" href="ring-theory.local-rings.html#1502" class="Bound">l</a> <a id="1504" class="Symbol">=</a> <a id="1506" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1508" class="Symbol">(</a><a id="1509" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="1514" href="ring-theory.local-rings.html#1502" class="Bound">l</a><a id="1515" class="Symbol">)</a> <a id="1517" href="ring-theory.local-rings.html#1211" class="Function">is-local-Ring</a>

<a id="1532" class="Keyword">module</a> <a id="1539" href="ring-theory.local-rings.html#1539" class="Module">_</a>
  <a id="1543" class="Symbol">{</a><a id="1544" href="ring-theory.local-rings.html#1544" class="Bound">l</a> <a id="1546" class="Symbol">:</a> <a id="1548" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1553" class="Symbol">}</a> <a id="1555" class="Symbol">(</a><a id="1556" href="ring-theory.local-rings.html#1556" class="Bound">R</a> <a id="1558" class="Symbol">:</a> <a id="1560" href="ring-theory.local-rings.html#1452" class="Function">Local-Ring</a> <a id="1571" href="ring-theory.local-rings.html#1544" class="Bound">l</a><a id="1572" class="Symbol">)</a>
  <a id="1576" class="Keyword">where</a>

  <a id="1585" href="ring-theory.local-rings.html#1585" class="Function">ring-Local-Ring</a> <a id="1601" class="Symbol">:</a> <a id="1603" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="1608" href="ring-theory.local-rings.html#1544" class="Bound">l</a>
  <a id="1612" href="ring-theory.local-rings.html#1585" class="Function">ring-Local-Ring</a> <a id="1628" class="Symbol">=</a> <a id="1630" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1634" href="ring-theory.local-rings.html#1556" class="Bound">R</a>

  <a id="1639" href="ring-theory.local-rings.html#1639" class="Function">set-Local-Ring</a> <a id="1654" class="Symbol">:</a> <a id="1656" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="1663" href="ring-theory.local-rings.html#1544" class="Bound">l</a>
  <a id="1667" href="ring-theory.local-rings.html#1639" class="Function">set-Local-Ring</a> <a id="1682" class="Symbol">=</a> <a id="1684" href="ring-theory.rings.html#2757" class="Function">set-Ring</a> <a id="1693" href="ring-theory.local-rings.html#1585" class="Function">ring-Local-Ring</a>

  <a id="1712" href="ring-theory.local-rings.html#1712" class="Function">type-Local-Ring</a> <a id="1728" class="Symbol">:</a> <a id="1730" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1733" href="ring-theory.local-rings.html#1544" class="Bound">l</a>
  <a id="1737" href="ring-theory.local-rings.html#1712" class="Function">type-Local-Ring</a> <a id="1753" class="Symbol">=</a> <a id="1755" href="ring-theory.rings.html#2808" class="Function">type-Ring</a> <a id="1765" href="ring-theory.local-rings.html#1585" class="Function">ring-Local-Ring</a>

  <a id="1784" href="ring-theory.local-rings.html#1784" class="Function">is-local-ring-Local-Ring</a> <a id="1809" class="Symbol">:</a> <a id="1811" href="ring-theory.local-rings.html#1211" class="Function">is-local-Ring</a> <a id="1825" href="ring-theory.local-rings.html#1585" class="Function">ring-Local-Ring</a>
  <a id="1843" href="ring-theory.local-rings.html#1784" class="Function">is-local-ring-Local-Ring</a> <a id="1868" class="Symbol">=</a> <a id="1870" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="1874" href="ring-theory.local-rings.html#1556" class="Bound">R</a>
</pre>