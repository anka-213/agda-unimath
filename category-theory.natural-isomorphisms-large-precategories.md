# Natural isomorphisms between functors on large precategories

<pre class="Agda"><a id="73" class="Symbol">{-#</a> <a id="77" class="Keyword">OPTIONS</a> <a id="85" class="Pragma">--without-K</a> <a id="97" class="Pragma">--exact-split</a> <a id="111" class="Symbol">#-}</a>

<a id="116" class="Keyword">module</a> <a id="123" href="category-theory.natural-isomorphisms-large-precategories.html" class="Module">category-theory.natural-isomorphisms-large-precategories</a> <a id="180" class="Keyword">where</a>

<a id="187" class="Keyword">open</a> <a id="192" class="Keyword">import</a> <a id="199" href="Agda.Primitive.html" class="Module">Agda.Primitive</a> <a id="214" class="Keyword">using</a> <a id="220" class="Symbol">(</a><a id="221" href="Agda.Primitive.html#381" class="Primitive">Setω</a><a id="225" class="Symbol">)</a>
<a id="227" class="Keyword">open</a> <a id="232" class="Keyword">import</a> <a id="239" href="category-theory.functors-large-precategories.html" class="Module">category-theory.functors-large-precategories</a> <a id="284" class="Keyword">using</a>
  <a id="292" class="Symbol">(</a> <a id="294" href="category-theory.functors-large-precategories.html#968" class="Record">functor-Large-Precat</a><a id="314" class="Symbol">;</a> <a id="316" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a><a id="340" class="Symbol">;</a>
    <a id="346" href="category-theory.functors-large-precategories.html#1177" class="Field">hom-functor-Large-Precat</a><a id="370" class="Symbol">)</a>
<a id="372" class="Keyword">open</a> <a id="377" class="Keyword">import</a> <a id="384" href="category-theory.isomorphisms-large-precategories.html" class="Module">category-theory.isomorphisms-large-precategories</a> <a id="433" class="Keyword">using</a>
  <a id="441" class="Symbol">(</a> <a id="443" href="category-theory.isomorphisms-large-precategories.html#1875" class="Function">iso-Large-Precat</a><a id="459" class="Symbol">;</a> <a id="461" href="category-theory.isomorphisms-large-precategories.html#2021" class="Function">hom-iso-Large-Precat</a><a id="481" class="Symbol">)</a>
<a id="483" class="Keyword">open</a> <a id="488" class="Keyword">import</a> <a id="495" href="category-theory.large-precategories.html" class="Module">category-theory.large-precategories</a> <a id="531" class="Keyword">using</a>
  <a id="539" class="Symbol">(</a> <a id="541" href="category-theory.large-precategories.html#654" class="Record">Large-Precat</a><a id="553" class="Symbol">;</a> <a id="555" href="category-theory.large-precategories.html#772" class="Field">obj-Large-Precat</a><a id="571" class="Symbol">;</a> <a id="573" href="category-theory.large-precategories.html#2369" class="Function">type-hom-Large-Precat</a><a id="594" class="Symbol">)</a>
<a id="596" class="Keyword">open</a> <a id="601" class="Keyword">import</a> <a id="608" href="category-theory.natural-transformations-large-precategories.html" class="Module">category-theory.natural-transformations-large-precategories</a> <a id="668" class="Keyword">using</a>
  <a id="676" class="Symbol">(</a> <a id="678" href="category-theory.natural-transformations-large-precategories.html#1056" class="Function">square-Large-Precat</a><a id="697" class="Symbol">;</a> <a id="699" href="category-theory.natural-transformations-large-precategories.html#1820" class="Record">natural-transformation-Large-Precat</a><a id="734" class="Symbol">;</a>
    <a id="740" href="category-theory.natural-transformations-large-precategories.html#1933" class="Field">obj-natural-transformation-Large-Precat</a><a id="779" class="Symbol">;</a>
    <a id="785" href="category-theory.natural-transformations-large-precategories.html#2148" class="Field">coherence-square-natural-transformation-Large-Precat</a><a id="837" class="Symbol">)</a>
<a id="839" class="Keyword">open</a> <a id="844" class="Keyword">import</a> <a id="851" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="878" class="Keyword">using</a> <a id="884" class="Symbol">(</a><a id="885" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="890" class="Symbol">)</a>
</pre>
## Idea

A natural isomorphism `γ` from functor `F : C → D` to `G : C → D` is a natural transformation from `F` to `G` such that the morphism `γ x : hom (F x) (G x)` is an isomorphism, for every object `x` in `C`.

## Definition

<pre class="Agda"><a id="1135" class="Keyword">module</a> <a id="1142" href="category-theory.natural-isomorphisms-large-precategories.html#1142" class="Module">_</a>
  <a id="1146" class="Symbol">{</a><a id="1147" href="category-theory.natural-isomorphisms-large-precategories.html#1147" class="Bound">αC</a> <a id="1150" href="category-theory.natural-isomorphisms-large-precategories.html#1150" class="Bound">αD</a> <a id="1153" href="category-theory.natural-isomorphisms-large-precategories.html#1153" class="Bound">γF</a> <a id="1156" href="category-theory.natural-isomorphisms-large-precategories.html#1156" class="Bound">γG</a> <a id="1159" class="Symbol">:</a> <a id="1161" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="1167" class="Symbol">→</a> <a id="1169" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1174" class="Symbol">}</a> <a id="1176" class="Symbol">{</a><a id="1177" href="category-theory.natural-isomorphisms-large-precategories.html#1177" class="Bound">βC</a> <a id="1180" href="category-theory.natural-isomorphisms-large-precategories.html#1180" class="Bound">βD</a> <a id="1183" class="Symbol">:</a> <a id="1185" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="1191" class="Symbol">→</a> <a id="1193" href="Agda.Primitive.html#597" class="Postulate">Level</a> <a id="1199" class="Symbol">→</a> <a id="1201" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1206" class="Symbol">}</a>
  <a id="1210" class="Symbol">{</a><a id="1211" href="category-theory.natural-isomorphisms-large-precategories.html#1211" class="Bound">C</a> <a id="1213" class="Symbol">:</a> <a id="1215" href="category-theory.large-precategories.html#654" class="Record">Large-Precat</a> <a id="1228" href="category-theory.natural-isomorphisms-large-precategories.html#1147" class="Bound">αC</a> <a id="1231" href="category-theory.natural-isomorphisms-large-precategories.html#1177" class="Bound">βC</a><a id="1233" class="Symbol">}</a> <a id="1235" class="Symbol">{</a><a id="1236" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a> <a id="1238" class="Symbol">:</a> <a id="1240" href="category-theory.large-precategories.html#654" class="Record">Large-Precat</a> <a id="1253" href="category-theory.natural-isomorphisms-large-precategories.html#1150" class="Bound">αD</a> <a id="1256" href="category-theory.natural-isomorphisms-large-precategories.html#1180" class="Bound">βD</a><a id="1258" class="Symbol">}</a>
  <a id="1262" class="Symbol">(</a><a id="1263" href="category-theory.natural-isomorphisms-large-precategories.html#1263" class="Bound">F</a> <a id="1265" class="Symbol">:</a> <a id="1267" href="category-theory.functors-large-precategories.html#968" class="Record">functor-Large-Precat</a> <a id="1288" href="category-theory.natural-isomorphisms-large-precategories.html#1211" class="Bound">C</a> <a id="1290" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a> <a id="1292" href="category-theory.natural-isomorphisms-large-precategories.html#1153" class="Bound">γF</a><a id="1294" class="Symbol">)</a> <a id="1296" class="Symbol">(</a><a id="1297" href="category-theory.natural-isomorphisms-large-precategories.html#1297" class="Bound">G</a> <a id="1299" class="Symbol">:</a> <a id="1301" href="category-theory.functors-large-precategories.html#968" class="Record">functor-Large-Precat</a> <a id="1322" href="category-theory.natural-isomorphisms-large-precategories.html#1211" class="Bound">C</a> <a id="1324" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a> <a id="1326" href="category-theory.natural-isomorphisms-large-precategories.html#1156" class="Bound">γG</a><a id="1328" class="Symbol">)</a>
  <a id="1332" class="Keyword">where</a>

  <a id="1341" class="Keyword">record</a> <a id="1348" href="category-theory.natural-isomorphisms-large-precategories.html#1348" class="Record">natural-isomorphism-Large-Precat</a> <a id="1381" class="Symbol">:</a> <a id="1383" href="Agda.Primitive.html#381" class="Primitive">Setω</a>
    <a id="1392" class="Keyword">where</a>
    <a id="1402" class="Keyword">constructor</a> <a id="1414" href="category-theory.natural-isomorphisms-large-precategories.html#1414" class="InductiveConstructor">make-natural-isomorphism</a>
    <a id="1443" class="Keyword">field</a>
      <a id="1455" href="category-theory.natural-isomorphisms-large-precategories.html#1455" class="Field">obj-natural-isomorphism-Large-Precat</a> <a id="1492" class="Symbol">:</a>
        <a id="1502" class="Symbol">{</a><a id="1503" href="category-theory.natural-isomorphisms-large-precategories.html#1503" class="Bound">l1</a> <a id="1506" class="Symbol">:</a> <a id="1508" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1513" class="Symbol">}</a> <a id="1515" class="Symbol">(</a><a id="1516" href="category-theory.natural-isomorphisms-large-precategories.html#1516" class="Bound">X</a> <a id="1518" class="Symbol">:</a> <a id="1520" href="category-theory.large-precategories.html#772" class="Field">obj-Large-Precat</a> <a id="1537" href="category-theory.natural-isomorphisms-large-precategories.html#1211" class="Bound">C</a> <a id="1539" href="category-theory.natural-isomorphisms-large-precategories.html#1503" class="Bound">l1</a><a id="1541" class="Symbol">)</a> <a id="1543" class="Symbol">→</a>
        <a id="1553" href="category-theory.isomorphisms-large-precategories.html#1875" class="Function">iso-Large-Precat</a> <a id="1570" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a>
          <a id="1582" class="Symbol">(</a> <a id="1584" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="1609" href="category-theory.natural-isomorphisms-large-precategories.html#1263" class="Bound">F</a> <a id="1611" href="category-theory.natural-isomorphisms-large-precategories.html#1516" class="Bound">X</a><a id="1612" class="Symbol">)</a>
          <a id="1624" class="Symbol">(</a> <a id="1626" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="1651" href="category-theory.natural-isomorphisms-large-precategories.html#1297" class="Bound">G</a> <a id="1653" href="category-theory.natural-isomorphisms-large-precategories.html#1516" class="Bound">X</a><a id="1654" class="Symbol">)</a>
      <a id="1662" href="category-theory.natural-isomorphisms-large-precategories.html#1662" class="Field">coherence-square-natural-isomorphism-Large-Precat</a> <a id="1712" class="Symbol">:</a>
        <a id="1722" class="Symbol">{</a><a id="1723" href="category-theory.natural-isomorphisms-large-precategories.html#1723" class="Bound">l1</a> <a id="1726" href="category-theory.natural-isomorphisms-large-precategories.html#1726" class="Bound">l2</a> <a id="1729" class="Symbol">:</a> <a id="1731" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1736" class="Symbol">}</a> <a id="1738" class="Symbol">{</a><a id="1739" href="category-theory.natural-isomorphisms-large-precategories.html#1739" class="Bound">X</a> <a id="1741" class="Symbol">:</a> <a id="1743" href="category-theory.large-precategories.html#772" class="Field">obj-Large-Precat</a> <a id="1760" href="category-theory.natural-isomorphisms-large-precategories.html#1211" class="Bound">C</a> <a id="1762" href="category-theory.natural-isomorphisms-large-precategories.html#1723" class="Bound">l1</a><a id="1764" class="Symbol">}</a>
        <a id="1774" class="Symbol">{</a><a id="1775" href="category-theory.natural-isomorphisms-large-precategories.html#1775" class="Bound">Y</a> <a id="1777" class="Symbol">:</a> <a id="1779" href="category-theory.large-precategories.html#772" class="Field">obj-Large-Precat</a> <a id="1796" href="category-theory.natural-isomorphisms-large-precategories.html#1211" class="Bound">C</a> <a id="1798" href="category-theory.natural-isomorphisms-large-precategories.html#1726" class="Bound">l2</a><a id="1800" class="Symbol">}</a> <a id="1802" class="Symbol">(</a><a id="1803" href="category-theory.natural-isomorphisms-large-precategories.html#1803" class="Bound">f</a> <a id="1805" class="Symbol">:</a> <a id="1807" href="category-theory.large-precategories.html#2369" class="Function">type-hom-Large-Precat</a> <a id="1829" href="category-theory.natural-isomorphisms-large-precategories.html#1211" class="Bound">C</a> <a id="1831" href="category-theory.natural-isomorphisms-large-precategories.html#1739" class="Bound">X</a> <a id="1833" href="category-theory.natural-isomorphisms-large-precategories.html#1775" class="Bound">Y</a><a id="1834" class="Symbol">)</a> <a id="1836" class="Symbol">→</a>
        <a id="1846" href="category-theory.natural-transformations-large-precategories.html#1056" class="Function">square-Large-Precat</a> <a id="1866" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a>
          <a id="1878" class="Symbol">(</a> <a id="1880" href="category-theory.isomorphisms-large-precategories.html#2021" class="Function">hom-iso-Large-Precat</a> <a id="1901" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a>
            <a id="1915" class="Symbol">(</a> <a id="1917" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="1942" href="category-theory.natural-isomorphisms-large-precategories.html#1263" class="Bound">F</a> <a id="1944" href="category-theory.natural-isomorphisms-large-precategories.html#1739" class="Bound">X</a><a id="1945" class="Symbol">)</a>
            <a id="1959" class="Symbol">(</a> <a id="1961" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="1986" href="category-theory.natural-isomorphisms-large-precategories.html#1297" class="Bound">G</a> <a id="1988" href="category-theory.natural-isomorphisms-large-precategories.html#1739" class="Bound">X</a><a id="1989" class="Symbol">)</a>
            <a id="2003" class="Symbol">(</a> <a id="2005" href="category-theory.natural-isomorphisms-large-precategories.html#1455" class="Field">obj-natural-isomorphism-Large-Precat</a> <a id="2042" href="category-theory.natural-isomorphisms-large-precategories.html#1739" class="Bound">X</a><a id="2043" class="Symbol">))</a>
          <a id="2056" class="Symbol">(</a> <a id="2058" href="category-theory.functors-large-precategories.html#1177" class="Field">hom-functor-Large-Precat</a> <a id="2083" href="category-theory.natural-isomorphisms-large-precategories.html#1263" class="Bound">F</a> <a id="2085" href="category-theory.natural-isomorphisms-large-precategories.html#1803" class="Bound">f</a><a id="2086" class="Symbol">)</a>
          <a id="2098" class="Symbol">(</a> <a id="2100" href="category-theory.functors-large-precategories.html#1177" class="Field">hom-functor-Large-Precat</a> <a id="2125" href="category-theory.natural-isomorphisms-large-precategories.html#1297" class="Bound">G</a> <a id="2127" href="category-theory.natural-isomorphisms-large-precategories.html#1803" class="Bound">f</a><a id="2128" class="Symbol">)</a>
          <a id="2140" class="Symbol">(</a> <a id="2142" href="category-theory.isomorphisms-large-precategories.html#2021" class="Function">hom-iso-Large-Precat</a> <a id="2163" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a>
            <a id="2177" class="Symbol">(</a> <a id="2179" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="2204" href="category-theory.natural-isomorphisms-large-precategories.html#1263" class="Bound">F</a> <a id="2206" href="category-theory.natural-isomorphisms-large-precategories.html#1775" class="Bound">Y</a><a id="2207" class="Symbol">)</a>
            <a id="2221" class="Symbol">(</a> <a id="2223" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="2248" href="category-theory.natural-isomorphisms-large-precategories.html#1297" class="Bound">G</a> <a id="2250" href="category-theory.natural-isomorphisms-large-precategories.html#1775" class="Bound">Y</a><a id="2251" class="Symbol">)</a>
            <a id="2265" class="Symbol">(</a> <a id="2267" href="category-theory.natural-isomorphisms-large-precategories.html#1455" class="Field">obj-natural-isomorphism-Large-Precat</a> <a id="2304" href="category-theory.natural-isomorphisms-large-precategories.html#1775" class="Bound">Y</a><a id="2305" class="Symbol">))</a>
               
  <a id="2326" class="Keyword">open</a> <a id="2331" href="category-theory.natural-isomorphisms-large-precategories.html#1348" class="Module">natural-isomorphism-Large-Precat</a> <a id="2364" class="Keyword">public</a>

  <a id="2374" href="category-theory.natural-isomorphisms-large-precategories.html#2374" class="Function">natural-transformation-natural-isomorphism-Large-Precat</a> <a id="2430" class="Symbol">:</a>
    <a id="2436" href="category-theory.natural-isomorphisms-large-precategories.html#1348" class="Record">natural-isomorphism-Large-Precat</a> <a id="2469" class="Symbol">→</a> <a id="2471" class="Symbol">(</a><a id="2472" href="category-theory.natural-transformations-large-precategories.html#1820" class="Record">natural-transformation-Large-Precat</a> <a id="2508" href="category-theory.natural-isomorphisms-large-precategories.html#1263" class="Bound">F</a> <a id="2510" href="category-theory.natural-isomorphisms-large-precategories.html#1297" class="Bound">G</a><a id="2511" class="Symbol">)</a>
  <a id="2515" href="category-theory.natural-transformations-large-precategories.html#1933" class="Field">obj-natural-transformation-Large-Precat</a>
    <a id="2559" class="Symbol">(</a><a id="2560" href="category-theory.natural-isomorphisms-large-precategories.html#2374" class="Function">natural-transformation-natural-isomorphism-Large-Precat</a> <a id="2616" href="category-theory.natural-isomorphisms-large-precategories.html#2616" class="Bound">γ</a><a id="2617" class="Symbol">)</a> <a id="2619" href="category-theory.natural-isomorphisms-large-precategories.html#2619" class="Bound">X</a> <a id="2621" class="Symbol">=</a>
      <a id="2629" href="category-theory.isomorphisms-large-precategories.html#2021" class="Function">hom-iso-Large-Precat</a> <a id="2650" href="category-theory.natural-isomorphisms-large-precategories.html#1236" class="Bound">D</a>
        <a id="2660" class="Symbol">(</a> <a id="2662" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="2687" href="category-theory.natural-isomorphisms-large-precategories.html#1263" class="Bound">F</a> <a id="2689" href="category-theory.natural-isomorphisms-large-precategories.html#2619" class="Bound">X</a><a id="2690" class="Symbol">)</a>
        <a id="2700" class="Symbol">(</a> <a id="2702" href="category-theory.functors-large-precategories.html#1071" class="Field">obj-functor-Large-Precat</a> <a id="2727" href="category-theory.natural-isomorphisms-large-precategories.html#1297" class="Bound">G</a> <a id="2729" href="category-theory.natural-isomorphisms-large-precategories.html#2619" class="Bound">X</a><a id="2730" class="Symbol">)</a>
        <a id="2740" class="Symbol">(</a> <a id="2742" href="category-theory.natural-isomorphisms-large-precategories.html#1455" class="Field">obj-natural-isomorphism-Large-Precat</a> <a id="2779" href="category-theory.natural-isomorphisms-large-precategories.html#2616" class="Bound">γ</a> <a id="2781" href="category-theory.natural-isomorphisms-large-precategories.html#2619" class="Bound">X</a><a id="2782" class="Symbol">)</a>
  <a id="2786" href="category-theory.natural-transformations-large-precategories.html#2148" class="Field">coherence-square-natural-transformation-Large-Precat</a>
    <a id="2843" class="Symbol">(</a><a id="2844" href="category-theory.natural-isomorphisms-large-precategories.html#2374" class="Function">natural-transformation-natural-isomorphism-Large-Precat</a> <a id="2900" href="category-theory.natural-isomorphisms-large-precategories.html#2900" class="Bound">γ</a><a id="2901" class="Symbol">)</a> <a id="2903" class="Symbol">=</a>
      <a id="2911" href="category-theory.natural-isomorphisms-large-precategories.html#1662" class="Field">coherence-square-natural-isomorphism-Large-Precat</a> <a id="2961" href="category-theory.natural-isomorphisms-large-precategories.html#2900" class="Bound">γ</a>
</pre>