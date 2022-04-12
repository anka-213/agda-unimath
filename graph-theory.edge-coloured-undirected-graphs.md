# Edge-coloured undirected graphs

<pre class="Agda"><a id="44" class="Symbol">{-#</a> <a id="48" class="Keyword">OPTIONS</a> <a id="56" class="Pragma">--without-K</a> <a id="68" class="Pragma">--exact-split</a> <a id="82" class="Symbol">#-}</a>

<a id="87" class="Keyword">module</a> <a id="94" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a> <a id="139" class="Keyword">where</a>

<a id="146" class="Keyword">open</a> <a id="151" class="Keyword">import</a> <a id="158" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="190" class="Keyword">using</a> <a id="196" class="Symbol">(</a><a id="197" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="198" class="Symbol">;</a> <a id="200" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="204" class="Symbol">;</a> <a id="206" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="209" class="Symbol">;</a> <a id="211" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="214" class="Symbol">)</a>
<a id="216" class="Keyword">open</a> <a id="221" class="Keyword">import</a> <a id="228" href="foundation.embeddings.html" class="Module">foundation.embeddings</a> <a id="250" class="Keyword">using</a> <a id="256" class="Symbol">(</a><a id="257" href="foundation-core.embeddings.html#980" class="Function">is-emb</a><a id="263" class="Symbol">)</a>
<a id="265" class="Keyword">open</a> <a id="270" class="Keyword">import</a> <a id="277" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="304" class="Keyword">using</a> <a id="310" class="Symbol">(</a><a id="311" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="316" class="Symbol">;</a> <a id="318" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="320" class="Symbol">;</a> <a id="322" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="325" class="Symbol">;</a> <a id="327" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="331" class="Symbol">;</a> <a id="333" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="338" class="Symbol">)</a>
<a id="340" class="Keyword">open</a> <a id="345" class="Keyword">import</a> <a id="352" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a> <a id="379" class="Keyword">using</a> <a id="385" class="Symbol">(</a><a id="386" href="foundation.unordered-pairs.html#4308" class="Function">standard-unordered-pair</a><a id="409" class="Symbol">)</a>

<a id="412" class="Keyword">open</a> <a id="417" class="Keyword">import</a> <a id="424" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a> <a id="465" class="Keyword">using</a>
  <a id="473" class="Symbol">(</a> <a id="475" href="graph-theory.incidence-undirected-graphs.html#695" class="Function">incidence-Undirected-Graph</a><a id="501" class="Symbol">)</a>
<a id="503" class="Keyword">open</a> <a id="508" class="Keyword">import</a> <a id="515" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a> <a id="546" class="Keyword">using</a>
  <a id="554" class="Symbol">(</a> <a id="556" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a><a id="572" class="Symbol">;</a> <a id="574" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a><a id="614" class="Symbol">;</a>
    <a id="620" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a><a id="643" class="Symbol">;</a> <a id="645" href="graph-theory.undirected-graphs.html#1205" class="Function">edge-Undirected-Graph</a><a id="666" class="Symbol">)</a>

<a id="669" class="Keyword">open</a> <a id="674" class="Keyword">import</a> <a id="681" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="718" class="Keyword">using</a> <a id="724" class="Symbol">(</a><a id="725" href="univalent-combinatorics.finite-types.html#4106" class="Function">𝔽</a><a id="726" class="Symbol">;</a> <a id="728" href="univalent-combinatorics.finite-types.html#4154" class="Function">type-𝔽</a><a id="734" class="Symbol">)</a>
</pre>
## Idea

An edge-coloured undirected graph is an undirected graph equipped with a family of maps `E p → X` from the edges at unordered pairs `p` into a type `C` of colours, such that the induced map `incident-Undirected-Graph G x → C` is injective for each vertex `x`.

## Definition

<pre class="Agda"><a id="1034" class="Keyword">module</a> <a id="1041" href="graph-theory.edge-coloured-undirected-graphs.html#1041" class="Module">_</a>
  <a id="1045" class="Symbol">{</a><a id="1046" href="graph-theory.edge-coloured-undirected-graphs.html#1046" class="Bound">l1</a> <a id="1049" href="graph-theory.edge-coloured-undirected-graphs.html#1049" class="Bound">l2</a> <a id="1052" href="graph-theory.edge-coloured-undirected-graphs.html#1052" class="Bound">l3</a> <a id="1055" class="Symbol">:</a> <a id="1057" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1062" class="Symbol">}</a> <a id="1064" class="Symbol">(</a><a id="1065" href="graph-theory.edge-coloured-undirected-graphs.html#1065" class="Bound">C</a> <a id="1067" class="Symbol">:</a> <a id="1069" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1072" href="graph-theory.edge-coloured-undirected-graphs.html#1046" class="Bound">l1</a><a id="1074" class="Symbol">)</a> <a id="1076" class="Symbol">(</a><a id="1077" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a> <a id="1079" class="Symbol">:</a> <a id="1081" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="1098" href="graph-theory.edge-coloured-undirected-graphs.html#1049" class="Bound">l2</a> <a id="1101" href="graph-theory.edge-coloured-undirected-graphs.html#1052" class="Bound">l3</a><a id="1103" class="Symbol">)</a>
  <a id="1107" class="Keyword">where</a>

  <a id="1116" href="graph-theory.edge-coloured-undirected-graphs.html#1116" class="Function">incidence-edge-colouring-Undirected-Graph</a> <a id="1158" class="Symbol">:</a>
    <a id="1164" class="Symbol">(</a> <a id="1166" class="Symbol">(</a><a id="1167" href="graph-theory.edge-coloured-undirected-graphs.html#1167" class="Bound">p</a> <a id="1169" class="Symbol">:</a> <a id="1171" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a> <a id="1212" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a><a id="1213" class="Symbol">)</a> <a id="1215" class="Symbol">→</a>
      <a id="1223" href="graph-theory.undirected-graphs.html#1205" class="Function">edge-Undirected-Graph</a> <a id="1245" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a> <a id="1247" href="graph-theory.edge-coloured-undirected-graphs.html#1167" class="Bound">p</a> <a id="1249" class="Symbol">→</a> <a id="1251" href="graph-theory.edge-coloured-undirected-graphs.html#1065" class="Bound">C</a><a id="1252" class="Symbol">)</a> <a id="1254" class="Symbol">→</a>
    <a id="1260" class="Symbol">(</a><a id="1261" href="graph-theory.edge-coloured-undirected-graphs.html#1261" class="Bound">x</a> <a id="1263" class="Symbol">:</a> <a id="1265" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a> <a id="1289" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a><a id="1290" class="Symbol">)</a> <a id="1292" class="Symbol">→</a> <a id="1294" href="graph-theory.incidence-undirected-graphs.html#695" class="Function">incidence-Undirected-Graph</a> <a id="1321" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a> <a id="1323" href="graph-theory.edge-coloured-undirected-graphs.html#1261" class="Bound">x</a> <a id="1325" class="Symbol">→</a> <a id="1327" href="graph-theory.edge-coloured-undirected-graphs.html#1065" class="Bound">C</a>
  <a id="1331" href="graph-theory.edge-coloured-undirected-graphs.html#1116" class="Function">incidence-edge-colouring-Undirected-Graph</a> <a id="1373" href="graph-theory.edge-coloured-undirected-graphs.html#1373" class="Bound">f</a> <a id="1375" href="graph-theory.edge-coloured-undirected-graphs.html#1375" class="Bound">x</a> <a id="1377" class="Symbol">(</a><a id="1378" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1383" href="graph-theory.edge-coloured-undirected-graphs.html#1383" class="Bound">y</a> <a id="1385" href="graph-theory.edge-coloured-undirected-graphs.html#1385" class="Bound">e</a><a id="1386" class="Symbol">)</a> <a id="1388" class="Symbol">=</a>
    <a id="1394" href="graph-theory.edge-coloured-undirected-graphs.html#1373" class="Bound">f</a> <a id="1396" class="Symbol">(</a><a id="1397" href="foundation.unordered-pairs.html#4308" class="Function">standard-unordered-pair</a> <a id="1421" href="graph-theory.edge-coloured-undirected-graphs.html#1375" class="Bound">x</a> <a id="1423" href="graph-theory.edge-coloured-undirected-graphs.html#1383" class="Bound">y</a><a id="1424" class="Symbol">)</a> <a id="1426" href="graph-theory.edge-coloured-undirected-graphs.html#1385" class="Bound">e</a>
  
  <a id="1433" href="graph-theory.edge-coloured-undirected-graphs.html#1433" class="Function">edge-colouring-Undirected-Graph</a> <a id="1465" class="Symbol">:</a> <a id="1467" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1470" class="Symbol">(</a><a id="1471" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1476" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="1482" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1484" href="graph-theory.edge-coloured-undirected-graphs.html#1046" class="Bound">l1</a> <a id="1487" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1489" href="graph-theory.edge-coloured-undirected-graphs.html#1049" class="Bound">l2</a> <a id="1492" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1494" href="graph-theory.edge-coloured-undirected-graphs.html#1052" class="Bound">l3</a><a id="1496" class="Symbol">)</a>
  <a id="1500" href="graph-theory.edge-coloured-undirected-graphs.html#1433" class="Function">edge-colouring-Undirected-Graph</a> <a id="1532" class="Symbol">=</a>
    <a id="1538" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1540" class="Symbol">(</a> <a id="1542" class="Symbol">(</a><a id="1543" href="graph-theory.edge-coloured-undirected-graphs.html#1543" class="Bound">p</a> <a id="1545" class="Symbol">:</a> <a id="1547" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a> <a id="1588" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a><a id="1589" class="Symbol">)</a> <a id="1591" class="Symbol">→</a>
        <a id="1601" href="graph-theory.undirected-graphs.html#1205" class="Function">edge-Undirected-Graph</a> <a id="1623" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a> <a id="1625" href="graph-theory.edge-coloured-undirected-graphs.html#1543" class="Bound">p</a> <a id="1627" class="Symbol">→</a> <a id="1629" href="graph-theory.edge-coloured-undirected-graphs.html#1065" class="Bound">C</a><a id="1630" class="Symbol">)</a>
      <a id="1638" class="Symbol">(</a> <a id="1640" class="Symbol">λ</a> <a id="1642" href="graph-theory.edge-coloured-undirected-graphs.html#1642" class="Bound">f</a> <a id="1644" class="Symbol">→</a>
        <a id="1654" class="Symbol">(</a><a id="1655" href="graph-theory.edge-coloured-undirected-graphs.html#1655" class="Bound">x</a> <a id="1657" class="Symbol">:</a> <a id="1659" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a> <a id="1683" href="graph-theory.edge-coloured-undirected-graphs.html#1077" class="Bound">G</a><a id="1684" class="Symbol">)</a> <a id="1686" class="Symbol">→</a>
        <a id="1696" href="foundation-core.embeddings.html#980" class="Function">is-emb</a> <a id="1703" class="Symbol">(</a><a id="1704" href="graph-theory.edge-coloured-undirected-graphs.html#1116" class="Function">incidence-edge-colouring-Undirected-Graph</a> <a id="1746" href="graph-theory.edge-coloured-undirected-graphs.html#1642" class="Bound">f</a> <a id="1748" href="graph-theory.edge-coloured-undirected-graphs.html#1655" class="Bound">x</a><a id="1749" class="Symbol">))</a>

<a id="Edge-Coloured-Undirected-Graph"></a><a id="1753" href="graph-theory.edge-coloured-undirected-graphs.html#1753" class="Function">Edge-Coloured-Undirected-Graph</a> <a id="1784" class="Symbol">:</a>
  <a id="1788" class="Symbol">{</a><a id="1789" href="graph-theory.edge-coloured-undirected-graphs.html#1789" class="Bound">l</a> <a id="1791" class="Symbol">:</a> <a id="1793" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1798" class="Symbol">}</a> <a id="1800" class="Symbol">(</a><a id="1801" href="graph-theory.edge-coloured-undirected-graphs.html#1801" class="Bound">l1</a> <a id="1804" href="graph-theory.edge-coloured-undirected-graphs.html#1804" class="Bound">l2</a> <a id="1807" class="Symbol">:</a> <a id="1809" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1814" class="Symbol">)</a> <a id="1816" class="Symbol">(</a><a id="1817" href="graph-theory.edge-coloured-undirected-graphs.html#1817" class="Bound">C</a> <a id="1819" class="Symbol">:</a> <a id="1821" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1824" href="graph-theory.edge-coloured-undirected-graphs.html#1789" class="Bound">l</a><a id="1825" class="Symbol">)</a> <a id="1827" class="Symbol">→</a> <a id="1829" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1832" class="Symbol">(</a><a id="1833" href="graph-theory.edge-coloured-undirected-graphs.html#1789" class="Bound">l</a> <a id="1835" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1837" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1842" href="graph-theory.edge-coloured-undirected-graphs.html#1801" class="Bound">l1</a> <a id="1845" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1847" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1852" href="graph-theory.edge-coloured-undirected-graphs.html#1804" class="Bound">l2</a><a id="1854" class="Symbol">)</a>
<a id="1856" href="graph-theory.edge-coloured-undirected-graphs.html#1753" class="Function">Edge-Coloured-Undirected-Graph</a> <a id="1887" href="graph-theory.edge-coloured-undirected-graphs.html#1887" class="Bound">l1</a> <a id="1890" href="graph-theory.edge-coloured-undirected-graphs.html#1890" class="Bound">l2</a> <a id="1893" href="graph-theory.edge-coloured-undirected-graphs.html#1893" class="Bound">C</a> <a id="1895" class="Symbol">=</a>
  <a id="1899" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1901" class="Symbol">(</a> <a id="1903" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="1920" href="graph-theory.edge-coloured-undirected-graphs.html#1887" class="Bound">l1</a> <a id="1923" href="graph-theory.edge-coloured-undirected-graphs.html#1890" class="Bound">l2</a><a id="1925" class="Symbol">)</a>
    <a id="1931" class="Symbol">(</a> <a id="1933" href="graph-theory.edge-coloured-undirected-graphs.html#1433" class="Function">edge-colouring-Undirected-Graph</a> <a id="1965" href="graph-theory.edge-coloured-undirected-graphs.html#1893" class="Bound">C</a><a id="1966" class="Symbol">)</a>

<a id="1969" class="Keyword">module</a> <a id="1976" href="graph-theory.edge-coloured-undirected-graphs.html#1976" class="Module">_</a>
  <a id="1980" class="Symbol">{</a><a id="1981" href="graph-theory.edge-coloured-undirected-graphs.html#1981" class="Bound">l1</a> <a id="1984" href="graph-theory.edge-coloured-undirected-graphs.html#1984" class="Bound">l2</a> <a id="1987" href="graph-theory.edge-coloured-undirected-graphs.html#1987" class="Bound">l3</a> <a id="1990" class="Symbol">:</a> <a id="1992" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1997" class="Symbol">}</a> <a id="1999" class="Symbol">{</a><a id="2000" href="graph-theory.edge-coloured-undirected-graphs.html#2000" class="Bound">C</a> <a id="2002" class="Symbol">:</a> <a id="2004" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2007" href="graph-theory.edge-coloured-undirected-graphs.html#1981" class="Bound">l1</a><a id="2009" class="Symbol">}</a> <a id="2011" class="Symbol">(</a><a id="2012" href="graph-theory.edge-coloured-undirected-graphs.html#2012" class="Bound">G</a> <a id="2014" class="Symbol">:</a> <a id="2016" href="graph-theory.edge-coloured-undirected-graphs.html#1753" class="Function">Edge-Coloured-Undirected-Graph</a> <a id="2047" href="graph-theory.edge-coloured-undirected-graphs.html#1984" class="Bound">l2</a> <a id="2050" href="graph-theory.edge-coloured-undirected-graphs.html#1987" class="Bound">l3</a> <a id="2053" href="graph-theory.edge-coloured-undirected-graphs.html#2000" class="Bound">C</a><a id="2054" class="Symbol">)</a>
  <a id="2058" class="Keyword">where</a>
  
  <a id="2069" href="graph-theory.edge-coloured-undirected-graphs.html#2069" class="Function">undirected-graph-Edge-Coloured-Undirected-Graph</a> <a id="2117" class="Symbol">:</a> <a id="2119" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="2136" href="graph-theory.edge-coloured-undirected-graphs.html#1984" class="Bound">l2</a> <a id="2139" href="graph-theory.edge-coloured-undirected-graphs.html#1987" class="Bound">l3</a>
  <a id="2144" href="graph-theory.edge-coloured-undirected-graphs.html#2069" class="Function">undirected-graph-Edge-Coloured-Undirected-Graph</a> <a id="2192" class="Symbol">=</a> <a id="2194" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2198" href="graph-theory.edge-coloured-undirected-graphs.html#2012" class="Bound">G</a>

  <a id="2203" href="graph-theory.edge-coloured-undirected-graphs.html#2203" class="Function">vertex-Edge-Coloured-Undirected-Graph</a> <a id="2241" class="Symbol">:</a> <a id="2243" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2246" href="graph-theory.edge-coloured-undirected-graphs.html#1984" class="Bound">l2</a>
  <a id="2251" href="graph-theory.edge-coloured-undirected-graphs.html#2203" class="Function">vertex-Edge-Coloured-Undirected-Graph</a> <a id="2289" class="Symbol">=</a>
    <a id="2295" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a> <a id="2319" href="graph-theory.edge-coloured-undirected-graphs.html#2069" class="Function">undirected-graph-Edge-Coloured-Undirected-Graph</a>

  <a id="2370" href="graph-theory.edge-coloured-undirected-graphs.html#2370" class="Function">unordered-pair-vertices-Edge-Coloured-Undirected-Graph</a> <a id="2425" class="Symbol">:</a> <a id="2427" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2430" class="Symbol">(</a><a id="2431" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="2436" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="2442" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2444" href="graph-theory.edge-coloured-undirected-graphs.html#1984" class="Bound">l2</a><a id="2446" class="Symbol">)</a>
  <a id="2450" href="graph-theory.edge-coloured-undirected-graphs.html#2370" class="Function">unordered-pair-vertices-Edge-Coloured-Undirected-Graph</a> <a id="2505" class="Symbol">=</a>
    <a id="2511" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a>
      <a id="2558" href="graph-theory.edge-coloured-undirected-graphs.html#2069" class="Function">undirected-graph-Edge-Coloured-Undirected-Graph</a>

  <a id="2609" href="graph-theory.edge-coloured-undirected-graphs.html#2609" class="Function">edge-Edge-Coloured-Undirected-Graph</a> <a id="2645" class="Symbol">:</a>
    <a id="2651" href="graph-theory.edge-coloured-undirected-graphs.html#2370" class="Function">unordered-pair-vertices-Edge-Coloured-Undirected-Graph</a> <a id="2706" class="Symbol">→</a> <a id="2708" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2711" href="graph-theory.edge-coloured-undirected-graphs.html#1987" class="Bound">l3</a>
  <a id="2716" href="graph-theory.edge-coloured-undirected-graphs.html#2609" class="Function">edge-Edge-Coloured-Undirected-Graph</a> <a id="2752" class="Symbol">=</a>
    <a id="2758" href="graph-theory.undirected-graphs.html#1205" class="Function">edge-Undirected-Graph</a> <a id="2780" href="graph-theory.edge-coloured-undirected-graphs.html#2069" class="Function">undirected-graph-Edge-Coloured-Undirected-Graph</a>

  <a id="2831" href="graph-theory.edge-coloured-undirected-graphs.html#2831" class="Function">incidence-Edge-Coloured-Undirected-Graph</a> <a id="2872" class="Symbol">:</a>
    <a id="2878" href="graph-theory.edge-coloured-undirected-graphs.html#2203" class="Function">vertex-Edge-Coloured-Undirected-Graph</a> <a id="2916" class="Symbol">→</a> <a id="2918" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2921" class="Symbol">(</a><a id="2922" href="graph-theory.edge-coloured-undirected-graphs.html#1984" class="Bound">l2</a> <a id="2925" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2927" href="graph-theory.edge-coloured-undirected-graphs.html#1987" class="Bound">l3</a><a id="2929" class="Symbol">)</a>
  <a id="2933" href="graph-theory.edge-coloured-undirected-graphs.html#2831" class="Function">incidence-Edge-Coloured-Undirected-Graph</a> <a id="2974" class="Symbol">=</a>
    <a id="2980" href="graph-theory.incidence-undirected-graphs.html#695" class="Function">incidence-Undirected-Graph</a> <a id="3007" href="graph-theory.edge-coloured-undirected-graphs.html#2069" class="Function">undirected-graph-Edge-Coloured-Undirected-Graph</a>

  <a id="3058" href="graph-theory.edge-coloured-undirected-graphs.html#3058" class="Function">colouring-Edge-Coloured-Undirected-Graph</a> <a id="3099" class="Symbol">:</a>
    <a id="3105" class="Symbol">(</a><a id="3106" href="graph-theory.edge-coloured-undirected-graphs.html#3106" class="Bound">p</a> <a id="3108" class="Symbol">:</a> <a id="3110" href="graph-theory.edge-coloured-undirected-graphs.html#2370" class="Function">unordered-pair-vertices-Edge-Coloured-Undirected-Graph</a><a id="3164" class="Symbol">)</a> <a id="3166" class="Symbol">→</a>
    <a id="3172" href="graph-theory.edge-coloured-undirected-graphs.html#2609" class="Function">edge-Edge-Coloured-Undirected-Graph</a> <a id="3208" href="graph-theory.edge-coloured-undirected-graphs.html#3106" class="Bound">p</a> <a id="3210" class="Symbol">→</a> <a id="3212" href="graph-theory.edge-coloured-undirected-graphs.html#2000" class="Bound">C</a>
  <a id="3216" href="graph-theory.edge-coloured-undirected-graphs.html#3058" class="Function">colouring-Edge-Coloured-Undirected-Graph</a> <a id="3257" class="Symbol">=</a>
    <a id="3263" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="3267" class="Symbol">(</a><a id="3268" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="3272" href="graph-theory.edge-coloured-undirected-graphs.html#2012" class="Bound">G</a><a id="3273" class="Symbol">)</a>

  <a id="3278" href="graph-theory.edge-coloured-undirected-graphs.html#3278" class="Function">incidence-colouring-Edge-Coloured-Undirected-Graph</a> <a id="3329" class="Symbol">:</a>
    <a id="3335" class="Symbol">(</a><a id="3336" href="graph-theory.edge-coloured-undirected-graphs.html#3336" class="Bound">x</a> <a id="3338" class="Symbol">:</a> <a id="3340" href="graph-theory.edge-coloured-undirected-graphs.html#2203" class="Function">vertex-Edge-Coloured-Undirected-Graph</a><a id="3377" class="Symbol">)</a> <a id="3379" class="Symbol">→</a>
    <a id="3385" href="graph-theory.edge-coloured-undirected-graphs.html#2831" class="Function">incidence-Edge-Coloured-Undirected-Graph</a> <a id="3426" href="graph-theory.edge-coloured-undirected-graphs.html#3336" class="Bound">x</a> <a id="3428" class="Symbol">→</a> <a id="3430" href="graph-theory.edge-coloured-undirected-graphs.html#2000" class="Bound">C</a>
  <a id="3434" href="graph-theory.edge-coloured-undirected-graphs.html#3278" class="Function">incidence-colouring-Edge-Coloured-Undirected-Graph</a> <a id="3485" class="Symbol">=</a>
    <a id="3491" href="graph-theory.edge-coloured-undirected-graphs.html#1116" class="Function">incidence-edge-colouring-Undirected-Graph</a> <a id="3533" href="graph-theory.edge-coloured-undirected-graphs.html#2000" class="Bound">C</a>
      <a id="3541" href="graph-theory.edge-coloured-undirected-graphs.html#2069" class="Function">undirected-graph-Edge-Coloured-Undirected-Graph</a>
      <a id="3595" href="graph-theory.edge-coloured-undirected-graphs.html#3058" class="Function">colouring-Edge-Coloured-Undirected-Graph</a>

  <a id="3639" href="graph-theory.edge-coloured-undirected-graphs.html#3639" class="Function">is-emb-colouring-Edge-Coloured-Undirected-Graph</a> <a id="3687" class="Symbol">:</a>
    <a id="3693" class="Symbol">(</a><a id="3694" href="graph-theory.edge-coloured-undirected-graphs.html#3694" class="Bound">x</a> <a id="3696" class="Symbol">:</a> <a id="3698" href="graph-theory.edge-coloured-undirected-graphs.html#2203" class="Function">vertex-Edge-Coloured-Undirected-Graph</a><a id="3735" class="Symbol">)</a> <a id="3737" class="Symbol">→</a>
    <a id="3743" href="foundation-core.embeddings.html#980" class="Function">is-emb</a> <a id="3750" class="Symbol">(</a><a id="3751" href="graph-theory.edge-coloured-undirected-graphs.html#3278" class="Function">incidence-colouring-Edge-Coloured-Undirected-Graph</a> <a id="3802" href="graph-theory.edge-coloured-undirected-graphs.html#3694" class="Bound">x</a><a id="3803" class="Symbol">)</a>
  <a id="3807" href="graph-theory.edge-coloured-undirected-graphs.html#3639" class="Function">is-emb-colouring-Edge-Coloured-Undirected-Graph</a> <a id="3855" class="Symbol">=</a>
    <a id="3861" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="3865" class="Symbol">(</a><a id="3866" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="3870" href="graph-theory.edge-coloured-undirected-graphs.html#2012" class="Bound">G</a><a id="3871" class="Symbol">)</a>
</pre>
## Properties