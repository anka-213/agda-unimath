---
title: Products of unordered tuples of types
---

<pre class="Agda"><a id="63" class="Symbol">{-#</a> <a id="67" class="Keyword">OPTIONS</a> <a id="75" class="Pragma">--without-K</a> <a id="87" class="Pragma">--exact-split</a> <a id="101" class="Symbol">#-}</a>

<a id="106" class="Keyword">module</a> <a id="113" href="foundation.products-unordered-tuples-of-types.html" class="Module">foundation.products-unordered-tuples-of-types</a> <a id="159" class="Keyword">where</a>

<a id="166" class="Keyword">open</a> <a id="171" class="Keyword">import</a> <a id="178" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="220" class="Keyword">open</a> <a id="225" class="Keyword">import</a> <a id="232" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="267" class="Keyword">open</a> <a id="272" class="Keyword">import</a> <a id="279" href="foundation.commutative-operations.html" class="Module">foundation.commutative-operations</a>
<a id="313" class="Keyword">open</a> <a id="318" class="Keyword">import</a> <a id="325" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="352" class="Keyword">open</a> <a id="357" class="Keyword">import</a> <a id="364" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="396" class="Keyword">open</a> <a id="401" class="Keyword">import</a> <a id="408" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="432" class="Keyword">open</a> <a id="437" class="Keyword">import</a> <a id="444" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="465" class="Keyword">open</a> <a id="470" class="Keyword">import</a> <a id="477" href="foundation.functoriality-cartesian-product-types.html" class="Module">foundation.functoriality-cartesian-product-types</a>
<a id="526" class="Keyword">open</a> <a id="531" class="Keyword">import</a> <a id="538" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="588" class="Keyword">open</a> <a id="593" class="Keyword">import</a> <a id="600" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="626" class="Keyword">open</a> <a id="631" class="Keyword">import</a> <a id="638" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="659" class="Keyword">open</a> <a id="664" class="Keyword">import</a> <a id="671" href="foundation.universal-property-maybe.html" class="Module">foundation.universal-property-maybe</a>
<a id="707" class="Keyword">open</a> <a id="712" class="Keyword">import</a> <a id="719" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="746" class="Keyword">open</a> <a id="751" class="Keyword">import</a> <a id="758" href="foundation.unordered-tuples.html" class="Module">foundation.unordered-tuples</a>
<a id="786" class="Keyword">open</a> <a id="791" class="Keyword">import</a> <a id="798" href="foundation.unordered-tuples-of-types.html" class="Module">foundation.unordered-tuples-of-types</a>

<a id="836" class="Keyword">open</a> <a id="841" class="Keyword">import</a> <a id="848" href="univalent-combinatorics.complements-isolated-points.html" class="Module">univalent-combinatorics.complements-isolated-points</a>
<a id="900" class="Keyword">open</a> <a id="905" class="Keyword">import</a> <a id="912" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
<a id="949" class="Keyword">open</a> <a id="954" class="Keyword">import</a> <a id="961" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
<a id="1007" class="Keyword">open</a> <a id="1012" class="Keyword">import</a> <a id="1019" href="univalent-combinatorics.universal-property-standard-finite-types.html" class="Module">univalent-combinatorics.universal-property-standard-finite-types</a>
</pre>
## Idea

Given an unordered pair of types, we can take their product. This is a commutative version of the cartesian product operation on types.

## Definition

<pre class="Agda"><a id="product-unordered-tuple-types"></a><a id="1258" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a> <a id="1288" class="Symbol">:</a>
  <a id="1292" class="Symbol">{</a><a id="1293" href="foundation.products-unordered-tuples-of-types.html#1293" class="Bound">l</a> <a id="1295" class="Symbol">:</a> <a id="1297" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1302" class="Symbol">}</a> <a id="1304" class="Symbol">{</a><a id="1305" href="foundation.products-unordered-tuples-of-types.html#1305" class="Bound">n</a> <a id="1307" class="Symbol">:</a> <a id="1309" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="1310" class="Symbol">}</a> <a id="1312" class="Symbol">→</a> <a id="1314" href="foundation.unordered-tuples.html#1180" class="Function">unordered-tuple</a> <a id="1330" href="foundation.products-unordered-tuples-of-types.html#1305" class="Bound">n</a> <a id="1332" class="Symbol">(</a><a id="1333" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1336" href="foundation.products-unordered-tuples-of-types.html#1293" class="Bound">l</a><a id="1337" class="Symbol">)</a> <a id="1339" class="Symbol">→</a> <a id="1341" class="Symbol">(</a><a id="1342" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1345" href="foundation.products-unordered-tuples-of-types.html#1293" class="Bound">l</a><a id="1346" class="Symbol">)</a>
<a id="1348" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a> <a id="1378" href="foundation.products-unordered-tuples-of-types.html#1378" class="Bound">p</a> <a id="1380" class="Symbol">=</a>
  <a id="1384" class="Symbol">(</a><a id="1385" href="foundation.products-unordered-tuples-of-types.html#1385" class="Bound">x</a> <a id="1387" class="Symbol">:</a> <a id="1389" href="foundation.unordered-tuples.html#1474" class="Function">type-unordered-tuple</a> <a id="1410" href="foundation.products-unordered-tuples-of-types.html#1378" class="Bound">p</a><a id="1411" class="Symbol">)</a> <a id="1413" class="Symbol">→</a> <a id="1415" href="foundation.unordered-tuples.html#2150" class="Function">element-unordered-tuple</a> <a id="1439" href="foundation.products-unordered-tuples-of-types.html#1378" class="Bound">p</a> <a id="1441" href="foundation.products-unordered-tuples-of-types.html#1385" class="Bound">x</a>

<a id="pr-product-unordered-tuple-types"></a><a id="1444" href="foundation.products-unordered-tuples-of-types.html#1444" class="Function">pr-product-unordered-tuple-types</a> <a id="1477" class="Symbol">:</a>
  <a id="1481" class="Symbol">{</a><a id="1482" href="foundation.products-unordered-tuples-of-types.html#1482" class="Bound">l</a> <a id="1484" class="Symbol">:</a> <a id="1486" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1491" class="Symbol">}</a> <a id="1493" class="Symbol">{</a><a id="1494" href="foundation.products-unordered-tuples-of-types.html#1494" class="Bound">n</a> <a id="1496" class="Symbol">:</a> <a id="1498" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="1499" class="Symbol">}</a> <a id="1501" class="Symbol">(</a><a id="1502" href="foundation.products-unordered-tuples-of-types.html#1502" class="Bound">A</a> <a id="1504" class="Symbol">:</a> <a id="1506" href="foundation.unordered-tuples-of-types.html#780" class="Function">unordered-tuple-types</a> <a id="1528" href="foundation.products-unordered-tuples-of-types.html#1482" class="Bound">l</a> <a id="1530" href="foundation.products-unordered-tuples-of-types.html#1494" class="Bound">n</a><a id="1531" class="Symbol">)</a>
  <a id="1535" class="Symbol">(</a><a id="1536" href="foundation.products-unordered-tuples-of-types.html#1536" class="Bound">i</a> <a id="1538" class="Symbol">:</a> <a id="1540" href="foundation.unordered-tuples.html#1474" class="Function">type-unordered-tuple</a> <a id="1561" href="foundation.products-unordered-tuples-of-types.html#1502" class="Bound">A</a><a id="1562" class="Symbol">)</a> <a id="1564" class="Symbol">→</a>
  <a id="1568" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a> <a id="1598" href="foundation.products-unordered-tuples-of-types.html#1502" class="Bound">A</a> <a id="1600" class="Symbol">→</a> <a id="1602" href="foundation.unordered-tuples.html#2150" class="Function">element-unordered-tuple</a> <a id="1626" href="foundation.products-unordered-tuples-of-types.html#1502" class="Bound">A</a> <a id="1628" href="foundation.products-unordered-tuples-of-types.html#1536" class="Bound">i</a>
<a id="1630" href="foundation.products-unordered-tuples-of-types.html#1444" class="Function">pr-product-unordered-tuple-types</a> <a id="1663" href="foundation.products-unordered-tuples-of-types.html#1663" class="Bound">A</a> <a id="1665" href="foundation.products-unordered-tuples-of-types.html#1665" class="Bound">i</a> <a id="1667" href="foundation.products-unordered-tuples-of-types.html#1667" class="Bound">f</a> <a id="1669" class="Symbol">=</a> <a id="1671" href="foundation.products-unordered-tuples-of-types.html#1667" class="Bound">f</a> <a id="1673" href="foundation.products-unordered-tuples-of-types.html#1665" class="Bound">i</a>

<a id="equiv-pr-product-unordered-tuple-types"></a><a id="1676" href="foundation.products-unordered-tuples-of-types.html#1676" class="Function">equiv-pr-product-unordered-tuple-types</a> <a id="1715" class="Symbol">:</a>
  <a id="1719" class="Symbol">{</a><a id="1720" href="foundation.products-unordered-tuples-of-types.html#1720" class="Bound">l</a> <a id="1722" class="Symbol">:</a> <a id="1724" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1729" class="Symbol">}</a> <a id="1731" class="Symbol">{</a><a id="1732" href="foundation.products-unordered-tuples-of-types.html#1732" class="Bound">n</a> <a id="1734" class="Symbol">:</a> <a id="1736" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="1737" class="Symbol">}</a> <a id="1739" class="Symbol">(</a><a id="1740" href="foundation.products-unordered-tuples-of-types.html#1740" class="Bound">A</a> <a id="1742" class="Symbol">:</a> <a id="1744" href="foundation.unordered-tuples-of-types.html#780" class="Function">unordered-tuple-types</a> <a id="1766" href="foundation.products-unordered-tuples-of-types.html#1720" class="Bound">l</a> <a id="1768" class="Symbol">(</a><a id="1769" href="elementary-number-theory.natural-numbers.html#1492" class="InductiveConstructor">succ-ℕ</a> <a id="1776" href="foundation.products-unordered-tuples-of-types.html#1732" class="Bound">n</a><a id="1777" class="Symbol">))</a>
  <a id="1782" class="Symbol">(</a><a id="1783" href="foundation.products-unordered-tuples-of-types.html#1783" class="Bound">i</a> <a id="1785" class="Symbol">:</a> <a id="1787" href="foundation.unordered-tuples.html#1474" class="Function">type-unordered-tuple</a> <a id="1808" href="foundation.products-unordered-tuples-of-types.html#1740" class="Bound">A</a><a id="1809" class="Symbol">)</a> <a id="1811" class="Symbol">→</a>
  <a id="1815" class="Symbol">(</a> <a id="1817" class="Symbol">(</a> <a id="1819" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a>
      <a id="1855" class="Symbol">(</a> <a id="1857" href="foundation.unordered-tuples.html#2981" class="Function">unordered-tuple-complement-point-type-unordered-tuple</a> <a id="1911" href="foundation.products-unordered-tuples-of-types.html#1740" class="Bound">A</a> <a id="1913" href="foundation.products-unordered-tuples-of-types.html#1783" class="Bound">i</a><a id="1914" class="Symbol">))</a> <a id="1917" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a>
    <a id="1923" class="Symbol">(</a> <a id="1925" href="foundation.unordered-tuples.html#2150" class="Function">element-unordered-tuple</a> <a id="1949" href="foundation.products-unordered-tuples-of-types.html#1740" class="Bound">A</a> <a id="1951" href="foundation.products-unordered-tuples-of-types.html#1783" class="Bound">i</a><a id="1952" class="Symbol">))</a> <a id="1955" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a>
  <a id="1959" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a> <a id="1989" href="foundation.products-unordered-tuples-of-types.html#1740" class="Bound">A</a>
<a id="1991" href="foundation.products-unordered-tuples-of-types.html#1676" class="Function">equiv-pr-product-unordered-tuple-types</a> <a id="2030" href="foundation.products-unordered-tuples-of-types.html#2030" class="Bound">A</a> <a id="2032" href="foundation.products-unordered-tuples-of-types.html#2032" class="Bound">i</a> <a id="2034" class="Symbol">=</a>
  <a id="2038" class="Symbol">(</a> <a id="2040" href="foundation.functoriality-dependent-function-types.html#4207" class="Function">equiv-Π</a>
    <a id="2052" class="Symbol">(</a> <a id="2054" href="foundation.unordered-tuples.html#2150" class="Function">element-unordered-tuple</a> <a id="2078" href="foundation.products-unordered-tuples-of-types.html#2030" class="Bound">A</a><a id="2079" class="Symbol">)</a>
    <a id="2085" class="Symbol">(</a> <a id="2087" href="univalent-combinatorics.complements-isolated-points.html#4210" class="Function">equiv-maybe-structure-point-UU-Fin</a> <a id="2122" class="Symbol">(</a><a id="2123" href="foundation.unordered-tuples.html#1394" class="Function">type-unordered-tuple-UU-Fin</a> <a id="2151" href="foundation.products-unordered-tuples-of-types.html#2030" class="Bound">A</a><a id="2152" class="Symbol">)</a> <a id="2154" href="foundation.products-unordered-tuples-of-types.html#2032" class="Bound">i</a><a id="2155" class="Symbol">)</a>
    <a id="2161" class="Symbol">(</a> <a id="2163" class="Symbol">λ</a> <a id="2165" href="foundation.products-unordered-tuples-of-types.html#2165" class="Bound">x</a> <a id="2167" class="Symbol">→</a> <a id="2169" href="foundation-core.equivalences.html#2494" class="Function">id-equiv</a><a id="2177" class="Symbol">))</a> <a id="2180" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a>
  <a id="2185" class="Symbol">(</a> <a id="2187" href="foundation-core.equivalences.html#5721" class="Function">inv-equiv</a>
    <a id="2201" class="Symbol">(</a> <a id="2203" href="foundation.universal-property-maybe.html#1978" class="Function">equiv-dependent-universal-property-Maybe</a>
      <a id="2250" class="Symbol">(</a> <a id="2252" class="Symbol">λ</a> <a id="2254" href="foundation.products-unordered-tuples-of-types.html#2254" class="Bound">j</a> <a id="2256" class="Symbol">→</a>
        <a id="2266" href="foundation.unordered-tuples.html#2150" class="Function">element-unordered-tuple</a> <a id="2290" href="foundation.products-unordered-tuples-of-types.html#2030" class="Bound">A</a>
          <a id="2302" class="Symbol">(</a> <a id="2304" href="foundation-core.equivalences.html#1821" class="Function">map-equiv</a> <a id="2314" class="Symbol">(</a><a id="2315" href="univalent-combinatorics.complements-isolated-points.html#4210" class="Function">equiv-maybe-structure-point-UU-Fin</a>
            <a id="2362" class="Symbol">(</a> <a id="2364" href="foundation.unordered-tuples.html#1394" class="Function">type-unordered-tuple-UU-Fin</a> <a id="2392" href="foundation.products-unordered-tuples-of-types.html#2030" class="Bound">A</a><a id="2393" class="Symbol">)</a> <a id="2395" href="foundation.products-unordered-tuples-of-types.html#2032" class="Bound">i</a><a id="2396" class="Symbol">)</a>
            <a id="2410" class="Symbol">(</a> <a id="2412" href="foundation.products-unordered-tuples-of-types.html#2254" class="Bound">j</a><a id="2413" class="Symbol">)))))</a>

<a id="map-equiv-pr-product-unordered-tuple-types"></a><a id="2420" href="foundation.products-unordered-tuples-of-types.html#2420" class="Function">map-equiv-pr-product-unordered-tuple-types</a> <a id="2463" class="Symbol">:</a>
  <a id="2467" class="Symbol">{</a><a id="2468" href="foundation.products-unordered-tuples-of-types.html#2468" class="Bound">l</a> <a id="2470" class="Symbol">:</a> <a id="2472" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2477" class="Symbol">}</a> <a id="2479" class="Symbol">{</a><a id="2480" href="foundation.products-unordered-tuples-of-types.html#2480" class="Bound">n</a> <a id="2482" class="Symbol">:</a> <a id="2484" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="2485" class="Symbol">}</a> <a id="2487" class="Symbol">(</a><a id="2488" href="foundation.products-unordered-tuples-of-types.html#2488" class="Bound">A</a> <a id="2490" class="Symbol">:</a> <a id="2492" href="foundation.unordered-tuples-of-types.html#780" class="Function">unordered-tuple-types</a> <a id="2514" href="foundation.products-unordered-tuples-of-types.html#2468" class="Bound">l</a> <a id="2516" class="Symbol">(</a><a id="2517" href="elementary-number-theory.natural-numbers.html#1492" class="InductiveConstructor">succ-ℕ</a> <a id="2524" href="foundation.products-unordered-tuples-of-types.html#2480" class="Bound">n</a><a id="2525" class="Symbol">))</a>
  <a id="2530" class="Symbol">(</a><a id="2531" href="foundation.products-unordered-tuples-of-types.html#2531" class="Bound">i</a> <a id="2533" class="Symbol">:</a> <a id="2535" href="foundation.unordered-tuples.html#1474" class="Function">type-unordered-tuple</a> <a id="2556" href="foundation.products-unordered-tuples-of-types.html#2488" class="Bound">A</a><a id="2557" class="Symbol">)</a> <a id="2559" class="Symbol">→</a>
  <a id="2563" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a>
    <a id="2597" class="Symbol">(</a> <a id="2599" href="foundation.unordered-tuples.html#2981" class="Function">unordered-tuple-complement-point-type-unordered-tuple</a> <a id="2653" href="foundation.products-unordered-tuples-of-types.html#2488" class="Bound">A</a> <a id="2655" href="foundation.products-unordered-tuples-of-types.html#2531" class="Bound">i</a><a id="2656" class="Symbol">)</a> <a id="2658" class="Symbol">→</a>
  <a id="2662" href="foundation.unordered-tuples.html#2150" class="Function">element-unordered-tuple</a> <a id="2686" href="foundation.products-unordered-tuples-of-types.html#2488" class="Bound">A</a> <a id="2688" href="foundation.products-unordered-tuples-of-types.html#2531" class="Bound">i</a> <a id="2690" class="Symbol">→</a> <a id="2692" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a> <a id="2722" href="foundation.products-unordered-tuples-of-types.html#2488" class="Bound">A</a>
<a id="2724" href="foundation.products-unordered-tuples-of-types.html#2420" class="Function">map-equiv-pr-product-unordered-tuple-types</a> <a id="2767" href="foundation.products-unordered-tuples-of-types.html#2767" class="Bound">A</a> <a id="2769" href="foundation.products-unordered-tuples-of-types.html#2769" class="Bound">i</a> <a id="2771" href="foundation.products-unordered-tuples-of-types.html#2771" class="Bound">f</a> <a id="2773" href="foundation.products-unordered-tuples-of-types.html#2773" class="Bound">a</a> <a id="2775" class="Symbol">=</a>
  <a id="2779" href="foundation-core.equivalences.html#1821" class="Function">map-equiv</a> <a id="2789" class="Symbol">(</a><a id="2790" href="foundation.products-unordered-tuples-of-types.html#1676" class="Function">equiv-pr-product-unordered-tuple-types</a> <a id="2829" href="foundation.products-unordered-tuples-of-types.html#2767" class="Bound">A</a> <a id="2831" href="foundation.products-unordered-tuples-of-types.html#2769" class="Bound">i</a><a id="2832" class="Symbol">)</a> <a id="2834" class="Symbol">(</a><a id="2835" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="2840" href="foundation.products-unordered-tuples-of-types.html#2771" class="Bound">f</a> <a id="2842" href="foundation.products-unordered-tuples-of-types.html#2773" class="Bound">a</a><a id="2843" class="Symbol">)</a>
</pre>
### Equivalences of products of unordered pairs of types

<pre class="Agda"><a id="2916" class="Keyword">module</a> <a id="2923" href="foundation.products-unordered-tuples-of-types.html#2923" class="Module">_</a>
  <a id="2927" class="Symbol">{</a><a id="2928" href="foundation.products-unordered-tuples-of-types.html#2928" class="Bound">l1</a> <a id="2931" href="foundation.products-unordered-tuples-of-types.html#2931" class="Bound">l2</a> <a id="2934" class="Symbol">:</a> <a id="2936" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2941" class="Symbol">}</a> <a id="2943" class="Symbol">{</a><a id="2944" href="foundation.products-unordered-tuples-of-types.html#2944" class="Bound">n</a> <a id="2946" class="Symbol">:</a> <a id="2948" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="2949" class="Symbol">}</a> <a id="2951" class="Symbol">(</a><a id="2952" href="foundation.products-unordered-tuples-of-types.html#2952" class="Bound">A</a> <a id="2954" class="Symbol">:</a> <a id="2956" href="foundation.unordered-tuples-of-types.html#780" class="Function">unordered-tuple-types</a> <a id="2978" href="foundation.products-unordered-tuples-of-types.html#2928" class="Bound">l1</a> <a id="2981" href="foundation.products-unordered-tuples-of-types.html#2944" class="Bound">n</a><a id="2982" class="Symbol">)</a>
  <a id="2986" class="Symbol">(</a><a id="2987" href="foundation.products-unordered-tuples-of-types.html#2987" class="Bound">B</a> <a id="2989" class="Symbol">:</a> <a id="2991" href="foundation.unordered-tuples-of-types.html#780" class="Function">unordered-tuple-types</a> <a id="3013" href="foundation.products-unordered-tuples-of-types.html#2931" class="Bound">l2</a> <a id="3016" href="foundation.products-unordered-tuples-of-types.html#2944" class="Bound">n</a><a id="3017" class="Symbol">)</a>
  <a id="3021" class="Keyword">where</a>

  <a id="3030" href="foundation.products-unordered-tuples-of-types.html#3030" class="Function">equiv-product-unordered-tuple-types</a> <a id="3066" class="Symbol">:</a>
    <a id="3072" href="foundation.unordered-tuples-of-types.html#946" class="Function">equiv-unordered-tuple-types</a> <a id="3100" href="foundation.products-unordered-tuples-of-types.html#2952" class="Bound">A</a> <a id="3102" href="foundation.products-unordered-tuples-of-types.html#2987" class="Bound">B</a> <a id="3104" class="Symbol">→</a>
    <a id="3110" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a> <a id="3140" href="foundation.products-unordered-tuples-of-types.html#2952" class="Bound">A</a> <a id="3142" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="3144" href="foundation.products-unordered-tuples-of-types.html#1258" class="Function">product-unordered-tuple-types</a> <a id="3174" href="foundation.products-unordered-tuples-of-types.html#2987" class="Bound">B</a>
  <a id="3178" href="foundation.products-unordered-tuples-of-types.html#3030" class="Function">equiv-product-unordered-tuple-types</a> <a id="3214" href="foundation.products-unordered-tuples-of-types.html#3214" class="Bound">e</a> <a id="3216" class="Symbol">=</a>
    <a id="3222" href="foundation.functoriality-dependent-function-types.html#4207" class="Function">equiv-Π</a>
      <a id="3236" class="Symbol">(</a> <a id="3238" href="foundation.unordered-tuples.html#2150" class="Function">element-unordered-tuple</a> <a id="3262" href="foundation.products-unordered-tuples-of-types.html#2987" class="Bound">B</a><a id="3263" class="Symbol">)</a>
      <a id="3271" class="Symbol">(</a> <a id="3273" href="foundation.unordered-tuples-of-types.html#1449" class="Function">equiv-type-equiv-unordered-tuple-types</a> <a id="3312" href="foundation.products-unordered-tuples-of-types.html#2952" class="Bound">A</a> <a id="3314" href="foundation.products-unordered-tuples-of-types.html#2987" class="Bound">B</a> <a id="3316" href="foundation.products-unordered-tuples-of-types.html#3214" class="Bound">e</a><a id="3317" class="Symbol">)</a>
      <a id="3325" class="Symbol">(</a> <a id="3327" href="foundation.unordered-tuples-of-types.html#1794" class="Function">equiv-element-equiv-unordered-tuple-types</a> <a id="3369" href="foundation.products-unordered-tuples-of-types.html#2952" class="Bound">A</a> <a id="3371" href="foundation.products-unordered-tuples-of-types.html#2987" class="Bound">B</a> <a id="3373" href="foundation.products-unordered-tuples-of-types.html#3214" class="Bound">e</a><a id="3374" class="Symbol">)</a>
</pre>