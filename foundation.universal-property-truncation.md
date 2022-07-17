---
title: The universal property of truncations
---

<pre class="Agda"><a id="63" class="Keyword">module</a> <a id="70" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a> <a id="111" class="Keyword">where</a>

<a id="118" class="Keyword">open</a> <a id="123" class="Keyword">import</a> <a id="130" href="foundation-core.universal-property-truncation.html" class="Module">foundation-core.universal-property-truncation</a> <a id="176" class="Keyword">public</a>

<a id="184" class="Keyword">open</a> <a id="189" class="Keyword">import</a> <a id="196" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a>
<a id="225" class="Keyword">open</a> <a id="230" class="Keyword">import</a> <a id="237" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="267" class="Keyword">open</a> <a id="272" class="Keyword">import</a> <a id="279" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="311" class="Keyword">open</a> <a id="316" class="Keyword">import</a> <a id="323" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="347" class="Keyword">open</a> <a id="352" class="Keyword">import</a> <a id="359" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="385" class="Keyword">open</a> <a id="390" class="Keyword">import</a> <a id="397" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a>
<a id="432" class="Keyword">open</a> <a id="437" class="Keyword">import</a> <a id="444" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="465" class="Keyword">open</a> <a id="470" class="Keyword">import</a> <a id="477" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a>
<a id="527" class="Keyword">open</a> <a id="532" class="Keyword">import</a> <a id="539" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="585" class="Keyword">open</a> <a id="590" class="Keyword">import</a> <a id="597" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="623" class="Keyword">open</a> <a id="628" class="Keyword">import</a> <a id="635" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="672" class="Keyword">open</a> <a id="677" class="Keyword">import</a> <a id="684" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="708" class="Keyword">open</a> <a id="713" class="Keyword">import</a> <a id="720" href="foundation.surjective-maps.html" class="Module">foundation.surjective-maps</a>
<a id="747" class="Keyword">open</a> <a id="752" class="Keyword">import</a> <a id="759" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a>
<a id="786" class="Keyword">open</a> <a id="791" class="Keyword">import</a> <a id="798" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="827" class="Keyword">open</a> <a id="832" class="Keyword">import</a> <a id="839" href="foundation.type-arithmetic-dependent-function-types.html" class="Module">foundation.type-arithmetic-dependent-function-types</a>
<a id="891" class="Keyword">open</a> <a id="896" class="Keyword">import</a> <a id="903" href="foundation.type-theoretic-principle-of-choice.html" class="Module">foundation.type-theoretic-principle-of-choice</a>
<a id="949" class="Keyword">open</a> <a id="954" class="Keyword">import</a> <a id="961" href="foundation.universal-property-dependent-pair-types.html" class="Module">foundation.universal-property-dependent-pair-types</a>
<a id="1012" class="Keyword">open</a> <a id="1017" class="Keyword">import</a> <a id="1024" href="foundation.universal-property-identity-types.html" class="Module">foundation.universal-property-identity-types</a>
<a id="1069" class="Keyword">open</a> <a id="1074" class="Keyword">import</a> <a id="1081" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Properties

### A map `f : A → B` is a `k+1`-truncation if and only if it is surjective and `ap f : (x ＝ y) → (f x ＝ f y)` is a `k`-truncation for all `x y : A`

<pre class="Agda"><a id="1286" class="Keyword">module</a> <a id="1293" href="foundation.universal-property-truncation.html#1293" class="Module">_</a>
  <a id="1297" class="Symbol">{</a><a id="1298" href="foundation.universal-property-truncation.html#1298" class="Bound">l1</a> <a id="1301" href="foundation.universal-property-truncation.html#1301" class="Bound">l2</a> <a id="1304" class="Symbol">:</a> <a id="1306" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1311" class="Symbol">}</a> <a id="1313" class="Symbol">{</a><a id="1314" href="foundation.universal-property-truncation.html#1314" class="Bound">k</a> <a id="1316" class="Symbol">:</a> <a id="1318" href="foundation-core.truncation-levels.html#395" class="Datatype">𝕋</a><a id="1319" class="Symbol">}</a> <a id="1321" class="Symbol">{</a><a id="1322" href="foundation.universal-property-truncation.html#1322" class="Bound">A</a> <a id="1324" class="Symbol">:</a> <a id="1326" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1329" href="foundation.universal-property-truncation.html#1298" class="Bound">l1</a><a id="1331" class="Symbol">}</a> <a id="1333" class="Symbol">(</a><a id="1334" href="foundation.universal-property-truncation.html#1334" class="Bound">B</a> <a id="1336" class="Symbol">:</a> <a id="1338" href="foundation-core.truncated-types.html#1925" class="Function">Truncated-Type</a> <a id="1353" href="foundation.universal-property-truncation.html#1301" class="Bound">l2</a> <a id="1356" class="Symbol">(</a><a id="1357" href="foundation-core.truncation-levels.html#432" class="InductiveConstructor">succ-𝕋</a> <a id="1364" href="foundation.universal-property-truncation.html#1314" class="Bound">k</a><a id="1365" class="Symbol">))</a>
  <a id="1370" class="Symbol">{</a><a id="1371" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="1373" class="Symbol">:</a> <a id="1375" href="foundation.universal-property-truncation.html#1322" class="Bound">A</a> <a id="1377" class="Symbol">→</a> <a id="1379" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="1399" href="foundation.universal-property-truncation.html#1334" class="Bound">B</a><a id="1400" class="Symbol">}</a> <a id="1402" class="Symbol">(</a><a id="1403" href="foundation.universal-property-truncation.html#1403" class="Bound">H</a> <a id="1405" class="Symbol">:</a> <a id="1407" href="foundation.surjective-maps.html#1938" class="Function">is-surjective</a> <a id="1421" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a><a id="1422" class="Symbol">)</a>
  <a id="1426" class="Symbol">(</a> <a id="1428" href="foundation.universal-property-truncation.html#1428" class="Bound">K</a> <a id="1430" class="Symbol">:</a>
    <a id="1436" class="Symbol">{</a><a id="1437" href="foundation.universal-property-truncation.html#1437" class="Bound">l</a> <a id="1439" class="Symbol">:</a> <a id="1441" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1446" class="Symbol">}</a> <a id="1448" class="Symbol">(</a><a id="1449" href="foundation.universal-property-truncation.html#1449" class="Bound">x</a> <a id="1451" href="foundation.universal-property-truncation.html#1451" class="Bound">y</a> <a id="1453" class="Symbol">:</a> <a id="1455" href="foundation.universal-property-truncation.html#1322" class="Bound">A</a><a id="1456" class="Symbol">)</a> <a id="1458" class="Symbol">→</a>
    <a id="1464" href="foundation-core.universal-property-truncation.html#1946" class="Function">is-truncation</a> <a id="1478" href="foundation.universal-property-truncation.html#1437" class="Bound">l</a> <a id="1480" class="Symbol">(</a><a id="1481" href="foundation-core.truncated-types.html#3222" class="Function">Id-Truncated-Type</a> <a id="1499" href="foundation.universal-property-truncation.html#1334" class="Bound">B</a> <a id="1501" class="Symbol">(</a><a id="1502" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="1504" href="foundation.universal-property-truncation.html#1449" class="Bound">x</a><a id="1505" class="Symbol">)</a> <a id="1507" class="Symbol">(</a><a id="1508" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="1510" href="foundation.universal-property-truncation.html#1451" class="Bound">y</a><a id="1511" class="Symbol">))</a> <a id="1514" class="Symbol">(</a><a id="1515" href="foundation-core.identity-types.html#4003" class="Function">ap</a> <a id="1518" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="1520" class="Symbol">{</a><a id="1521" href="foundation.universal-property-truncation.html#1449" class="Bound">x</a><a id="1522" class="Symbol">}</a> <a id="1524" class="Symbol">{</a><a id="1525" href="foundation.universal-property-truncation.html#1451" class="Bound">y</a><a id="1526" class="Symbol">}))</a>
  <a id="1532" class="Keyword">where</a>

  <a id="1541" href="foundation.universal-property-truncation.html#1541" class="Function">unique-extension-fib-is-truncation-is-truncation-ap</a> <a id="1593" class="Symbol">:</a>
    <a id="1599" class="Symbol">{</a><a id="1600" href="foundation.universal-property-truncation.html#1600" class="Bound">l</a> <a id="1602" class="Symbol">:</a> <a id="1604" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1609" class="Symbol">}</a> <a id="1611" class="Symbol">(</a><a id="1612" href="foundation.universal-property-truncation.html#1612" class="Bound">C</a> <a id="1614" class="Symbol">:</a> <a id="1616" href="foundation-core.truncated-types.html#1925" class="Function">Truncated-Type</a> <a id="1631" href="foundation.universal-property-truncation.html#1600" class="Bound">l</a> <a id="1633" class="Symbol">(</a><a id="1634" href="foundation-core.truncation-levels.html#432" class="InductiveConstructor">succ-𝕋</a> <a id="1641" href="foundation.universal-property-truncation.html#1314" class="Bound">k</a><a id="1642" class="Symbol">))</a>
    <a id="1649" class="Symbol">(</a><a id="1650" href="foundation.universal-property-truncation.html#1650" class="Bound">g</a> <a id="1652" class="Symbol">:</a> <a id="1654" href="foundation.universal-property-truncation.html#1322" class="Bound">A</a> <a id="1656" class="Symbol">→</a> <a id="1658" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="1678" href="foundation.universal-property-truncation.html#1612" class="Bound">C</a><a id="1679" class="Symbol">)</a> <a id="1681" class="Symbol">(</a><a id="1682" href="foundation.universal-property-truncation.html#1682" class="Bound">y</a> <a id="1684" class="Symbol">:</a> <a id="1686" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="1706" href="foundation.universal-property-truncation.html#1334" class="Bound">B</a><a id="1707" class="Symbol">)</a> <a id="1709" class="Symbol">→</a>
    <a id="1715" href="foundation-core.contractible-types.html#1006" class="Function">is-contr</a>
      <a id="1730" class="Symbol">(</a> <a id="1732" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1734" class="Symbol">(</a> <a id="1736" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="1756" href="foundation.universal-property-truncation.html#1612" class="Bound">C</a><a id="1757" class="Symbol">)</a>
          <a id="1769" class="Symbol">(</a> <a id="1771" class="Symbol">λ</a> <a id="1773" href="foundation.universal-property-truncation.html#1773" class="Bound">z</a> <a id="1775" class="Symbol">→</a> <a id="1777" class="Symbol">(</a><a id="1778" href="foundation.universal-property-truncation.html#1778" class="Bound">t</a> <a id="1780" class="Symbol">:</a> <a id="1782" href="foundation-core.fibers-of-maps.html#942" class="Function">fib</a> <a id="1786" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="1788" href="foundation.universal-property-truncation.html#1682" class="Bound">y</a><a id="1789" class="Symbol">)</a> <a id="1791" class="Symbol">→</a> <a id="1793" href="foundation-core.identity-types.html#1767" class="Datatype">Id</a> <a id="1796" class="Symbol">(</a><a id="1797" href="foundation.universal-property-truncation.html#1650" class="Bound">g</a> <a id="1799" class="Symbol">(</a><a id="1800" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1804" href="foundation.universal-property-truncation.html#1778" class="Bound">t</a><a id="1805" class="Symbol">))</a> <a id="1808" href="foundation.universal-property-truncation.html#1773" class="Bound">z</a><a id="1809" class="Symbol">))</a>
  <a id="1814" href="foundation.universal-property-truncation.html#1541" class="Function">unique-extension-fib-is-truncation-is-truncation-ap</a> <a id="1866" href="foundation.universal-property-truncation.html#1866" class="Bound">C</a> <a id="1868" href="foundation.universal-property-truncation.html#1868" class="Bound">g</a> <a id="1870" class="Symbol">=</a>
    <a id="1876" href="foundation.surjective-maps.html#5517" class="Function">apply-dependent-universal-property-surj-is-surjective</a> <a id="1930" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="1932" href="foundation.universal-property-truncation.html#1403" class="Bound">H</a>
      <a id="1940" class="Symbol">(</a> <a id="1942" class="Symbol">λ</a> <a id="1944" href="foundation.universal-property-truncation.html#1944" class="Bound">y</a> <a id="1946" class="Symbol">→</a> <a id="1948" href="foundation.contractible-types.html#1563" class="Function">is-contr-Prop</a> <a id="1962" class="Symbol">_)</a>
      <a id="1971" class="Symbol">(</a> <a id="1973" class="Symbol">λ</a> <a id="1975" href="foundation.universal-property-truncation.html#1975" class="Bound">x</a> <a id="1977" class="Symbol">→</a>
        <a id="1987" href="foundation-core.contractible-types.html#3304" class="Function">is-contr-equiv</a>
          <a id="2012" class="Symbol">(</a> <a id="2014" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="2016" class="Symbol">(</a><a id="2017" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="2037" href="foundation.universal-property-truncation.html#1866" class="Bound">C</a><a id="2038" class="Symbol">)</a> <a id="2040" class="Symbol">(λ</a> <a id="2043" href="foundation.universal-property-truncation.html#2043" class="Bound">z</a> <a id="2045" class="Symbol">→</a> <a id="2047" href="foundation.universal-property-truncation.html#1868" class="Bound">g</a> <a id="2049" href="foundation.universal-property-truncation.html#1975" class="Bound">x</a> <a id="2051" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="2053" href="foundation.universal-property-truncation.html#2043" class="Bound">z</a><a id="2054" class="Symbol">))</a>
          <a id="2067" class="Symbol">(</a> <a id="2069" href="foundation-core.functoriality-dependent-pair-types.html#6817" class="Function">equiv-tot</a>
            <a id="2091" class="Symbol">(</a> <a id="2093" class="Symbol">λ</a> <a id="2095" href="foundation.universal-property-truncation.html#2095" class="Bound">z</a> <a id="2097" class="Symbol">→</a>
              <a id="2113" class="Symbol">(</a> <a id="2115" class="Symbol">(</a> <a id="2117" href="foundation.universal-property-identity-types.html#1566" class="Function">equiv-ev-refl&#39;</a> <a id="2132" href="foundation.universal-property-truncation.html#1975" class="Bound">x</a><a id="2133" class="Symbol">)</a> <a id="2135" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a>
                <a id="2154" class="Symbol">(</a> <a id="2156" href="foundation-core.functoriality-dependent-function-types.html#2227" class="Function">equiv-map-Π</a>
                  <a id="2186" class="Symbol">(</a> <a id="2188" class="Symbol">λ</a> <a id="2190" href="foundation.universal-property-truncation.html#2190" class="Bound">x&#39;</a> <a id="2193" class="Symbol">→</a>
                    <a id="2215" href="foundation-core.universal-property-truncation.html#2185" class="Function">equiv-is-truncation</a>
                      <a id="2257" class="Symbol">(</a> <a id="2259" href="foundation-core.truncated-types.html#3222" class="Function">Id-Truncated-Type</a> <a id="2277" href="foundation.universal-property-truncation.html#1334" class="Bound">B</a> <a id="2279" class="Symbol">(</a><a id="2280" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="2282" href="foundation.universal-property-truncation.html#2190" class="Bound">x&#39;</a><a id="2284" class="Symbol">)</a> <a id="2286" class="Symbol">(</a><a id="2287" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="2289" href="foundation.universal-property-truncation.html#1975" class="Bound">x</a><a id="2290" class="Symbol">))</a>
                      <a id="2315" class="Symbol">(</a> <a id="2317" href="foundation-core.identity-types.html#4003" class="Function">ap</a> <a id="2320" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a><a id="2321" class="Symbol">)</a>
                      <a id="2345" class="Symbol">(</a> <a id="2347" href="foundation.universal-property-truncation.html#1428" class="Bound">K</a> <a id="2349" href="foundation.universal-property-truncation.html#2190" class="Bound">x&#39;</a> <a id="2352" href="foundation.universal-property-truncation.html#1975" class="Bound">x</a><a id="2353" class="Symbol">)</a>
                      <a id="2377" class="Symbol">(</a> <a id="2379" href="foundation-core.truncated-types.html#3222" class="Function">Id-Truncated-Type</a> <a id="2397" href="foundation.universal-property-truncation.html#1866" class="Bound">C</a> <a id="2399" class="Symbol">(</a><a id="2400" href="foundation.universal-property-truncation.html#1868" class="Bound">g</a> <a id="2402" href="foundation.universal-property-truncation.html#2190" class="Bound">x&#39;</a><a id="2404" class="Symbol">)</a> <a id="2406" href="foundation.universal-property-truncation.html#2095" class="Bound">z</a><a id="2407" class="Symbol">))))</a> <a id="2412" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a>
              <a id="2429" class="Symbol">(</a> <a id="2431" href="foundation.universal-property-dependent-pair-types.html#1013" class="Function">equiv-ev-pair</a><a id="2444" class="Symbol">)))</a>
          <a id="2458" class="Symbol">(</a> <a id="2460" href="foundation-core.contractible-types.html#2046" class="Function">is-contr-total-path</a> <a id="2480" class="Symbol">(</a><a id="2481" href="foundation.universal-property-truncation.html#1868" class="Bound">g</a> <a id="2483" href="foundation.universal-property-truncation.html#1975" class="Bound">x</a><a id="2484" class="Symbol">)))</a>
  
  <a id="2493" href="foundation.universal-property-truncation.html#2493" class="Function">is-truncation-is-truncation-ap</a> <a id="2524" class="Symbol">:</a>
    <a id="2530" class="Symbol">{</a><a id="2531" href="foundation.universal-property-truncation.html#2531" class="Bound">l</a> <a id="2533" class="Symbol">:</a> <a id="2535" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2540" class="Symbol">}</a> <a id="2542" class="Symbol">→</a> <a id="2544" href="foundation-core.universal-property-truncation.html#1946" class="Function">is-truncation</a> <a id="2558" href="foundation.universal-property-truncation.html#2531" class="Bound">l</a> <a id="2560" href="foundation.universal-property-truncation.html#1334" class="Bound">B</a> <a id="2562" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a>
  <a id="2566" href="foundation.universal-property-truncation.html#2493" class="Function">is-truncation-is-truncation-ap</a> <a id="2597" href="foundation.universal-property-truncation.html#2597" class="Bound">C</a> <a id="2599" class="Symbol">=</a>
    <a id="2605" href="foundation-core.contractible-maps.html#2380" class="Function">is-equiv-is-contr-map</a>
      <a id="2633" class="Symbol">(</a> <a id="2635" class="Symbol">λ</a> <a id="2637" href="foundation.universal-property-truncation.html#2637" class="Bound">g</a> <a id="2639" class="Symbol">→</a>
        <a id="2649" href="foundation-core.contractible-types.html#3813" class="Function">is-contr-equiv&#39;</a>
          <a id="2675" class="Symbol">(</a> <a id="2677" class="Symbol">(</a><a id="2678" href="foundation.universal-property-truncation.html#2678" class="Bound">y</a> <a id="2680" class="Symbol">:</a> <a id="2682" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="2702" href="foundation.universal-property-truncation.html#1334" class="Bound">B</a><a id="2703" class="Symbol">)</a> <a id="2705" class="Symbol">→</a>
            <a id="2719" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="2721" class="Symbol">(</a> <a id="2723" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="2743" href="foundation.universal-property-truncation.html#2597" class="Bound">C</a><a id="2744" class="Symbol">)</a>
              <a id="2760" class="Symbol">(</a> <a id="2762" class="Symbol">λ</a> <a id="2764" href="foundation.universal-property-truncation.html#2764" class="Bound">z</a> <a id="2766" class="Symbol">→</a> <a id="2768" class="Symbol">(</a><a id="2769" href="foundation.universal-property-truncation.html#2769" class="Bound">t</a> <a id="2771" class="Symbol">:</a> <a id="2773" href="foundation-core.fibers-of-maps.html#942" class="Function">fib</a> <a id="2777" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="2779" href="foundation.universal-property-truncation.html#2678" class="Bound">y</a><a id="2780" class="Symbol">)</a> <a id="2782" class="Symbol">→</a> <a id="2784" class="Symbol">(</a><a id="2785" href="foundation.universal-property-truncation.html#2637" class="Bound">g</a> <a id="2787" class="Symbol">(</a><a id="2788" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="2792" href="foundation.universal-property-truncation.html#2769" class="Bound">t</a><a id="2793" class="Symbol">)</a> <a id="2795" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="2797" href="foundation.universal-property-truncation.html#2764" class="Bound">z</a><a id="2798" class="Symbol">)))</a>
          <a id="2812" class="Symbol">(</a> <a id="2814" class="Symbol">(</a> <a id="2816" href="foundation-core.functoriality-dependent-pair-types.html#6817" class="Function">equiv-tot</a>
              <a id="2840" class="Symbol">(</a> <a id="2842" class="Symbol">λ</a> <a id="2844" href="foundation.universal-property-truncation.html#2844" class="Bound">h</a> <a id="2846" class="Symbol">→</a>
                <a id="2864" class="Symbol">(</a> <a id="2866" class="Symbol">(</a> <a id="2868" class="Symbol">(</a> <a id="2870" href="foundation-core.equivalences.html#5721" class="Function">inv-equiv</a> <a id="2880" class="Symbol">(</a><a id="2881" href="foundation-core.function-extensionality.html#1301" class="Function">equiv-funext</a><a id="2893" class="Symbol">))</a> <a id="2896" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a>
                    <a id="2919" class="Symbol">(</a> <a id="2921" href="foundation-core.functoriality-dependent-function-types.html#2227" class="Function">equiv-map-Π</a>
                      <a id="2955" class="Symbol">(</a> <a id="2957" class="Symbol">λ</a> <a id="2959" href="foundation.universal-property-truncation.html#2959" class="Bound">x</a> <a id="2961" class="Symbol">→</a>
                        <a id="2987" href="foundation.identity-types.html#1228" class="Function">equiv-inv</a> <a id="2997" class="Symbol">(</a><a id="2998" href="foundation.universal-property-truncation.html#2637" class="Bound">g</a> <a id="3000" href="foundation.universal-property-truncation.html#2959" class="Bound">x</a><a id="3001" class="Symbol">)</a> <a id="3003" class="Symbol">(</a><a id="3004" href="foundation.universal-property-truncation.html#2844" class="Bound">h</a> <a id="3006" class="Symbol">(</a><a id="3007" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="3009" href="foundation.universal-property-truncation.html#2959" class="Bound">x</a><a id="3010" class="Symbol">))</a> <a id="3013" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a> <a id="3016" href="foundation.universal-property-identity-types.html#1357" class="Function">equiv-ev-refl</a> <a id="3030" class="Symbol">(</a><a id="3031" href="foundation.universal-property-truncation.html#1371" class="Bound">f</a> <a id="3033" href="foundation.universal-property-truncation.html#2959" class="Bound">x</a><a id="3034" class="Symbol">))))</a> <a id="3039" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a>
                  <a id="3060" class="Symbol">(</a> <a id="3062" href="foundation.type-arithmetic-dependent-function-types.html#789" class="Function">equiv-swap-Π</a><a id="3074" class="Symbol">))</a> <a id="3077" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a>
                <a id="3096" class="Symbol">(</a> <a id="3098" href="foundation-core.functoriality-dependent-function-types.html#2227" class="Function">equiv-map-Π</a> <a id="3110" class="Symbol">(λ</a> <a id="3113" href="foundation.universal-property-truncation.html#3113" class="Bound">x</a> <a id="3115" class="Symbol">→</a> <a id="3117" href="foundation.universal-property-dependent-pair-types.html#1013" class="Function">equiv-ev-pair</a><a id="3130" class="Symbol">))))</a> <a id="3135" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a>
            <a id="3150" class="Symbol">(</a> <a id="3152" href="foundation.type-theoretic-principle-of-choice.html#4367" class="Function">distributive-Π-Σ</a><a id="3168" class="Symbol">))</a>
          <a id="3181" class="Symbol">(</a> <a id="3183" href="foundation-core.contractible-types.html#6898" class="Function">is-contr-Π</a>
            <a id="3206" class="Symbol">(</a> <a id="3208" href="foundation.universal-property-truncation.html#1541" class="Function">unique-extension-fib-is-truncation-is-truncation-ap</a> <a id="3260" href="foundation.universal-property-truncation.html#2597" class="Bound">C</a> <a id="3262" href="foundation.universal-property-truncation.html#2637" class="Bound">g</a><a id="3263" class="Symbol">)))</a>
  
<a id="3270" class="Keyword">module</a> <a id="3277" href="foundation.universal-property-truncation.html#3277" class="Module">_</a>
  <a id="3281" class="Symbol">{</a><a id="3282" href="foundation.universal-property-truncation.html#3282" class="Bound">l1</a> <a id="3285" href="foundation.universal-property-truncation.html#3285" class="Bound">l2</a> <a id="3288" class="Symbol">:</a> <a id="3290" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3295" class="Symbol">}</a> <a id="3297" class="Symbol">{</a><a id="3298" href="foundation.universal-property-truncation.html#3298" class="Bound">k</a> <a id="3300" class="Symbol">:</a> <a id="3302" href="foundation-core.truncation-levels.html#395" class="Datatype">𝕋</a><a id="3303" class="Symbol">}</a> <a id="3305" class="Symbol">{</a><a id="3306" href="foundation.universal-property-truncation.html#3306" class="Bound">A</a> <a id="3308" class="Symbol">:</a> <a id="3310" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="3313" href="foundation.universal-property-truncation.html#3282" class="Bound">l1</a><a id="3315" class="Symbol">}</a> <a id="3317" class="Symbol">(</a><a id="3318" href="foundation.universal-property-truncation.html#3318" class="Bound">B</a> <a id="3320" class="Symbol">:</a> <a id="3322" href="foundation-core.truncated-types.html#1925" class="Function">Truncated-Type</a> <a id="3337" href="foundation.universal-property-truncation.html#3285" class="Bound">l2</a> <a id="3340" class="Symbol">(</a><a id="3341" href="foundation-core.truncation-levels.html#432" class="InductiveConstructor">succ-𝕋</a> <a id="3348" href="foundation.universal-property-truncation.html#3298" class="Bound">k</a><a id="3349" class="Symbol">))</a>
  <a id="3354" class="Symbol">{</a><a id="3355" href="foundation.universal-property-truncation.html#3355" class="Bound">f</a> <a id="3357" class="Symbol">:</a> <a id="3359" href="foundation.universal-property-truncation.html#3306" class="Bound">A</a> <a id="3361" class="Symbol">→</a> <a id="3363" href="foundation-core.truncated-types.html#2060" class="Function">type-Truncated-Type</a> <a id="3383" href="foundation.universal-property-truncation.html#3318" class="Bound">B</a><a id="3384" class="Symbol">}</a>
  <a id="3388" class="Keyword">where</a>

  <a id="3397" href="foundation.universal-property-truncation.html#3397" class="Function">is-surjective-is-truncation</a> <a id="3425" class="Symbol">:</a>
    <a id="3431" class="Symbol">({</a><a id="3433" href="foundation.universal-property-truncation.html#3433" class="Bound">l</a> <a id="3435" class="Symbol">:</a> <a id="3437" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3442" class="Symbol">}</a> <a id="3444" class="Symbol">→</a> <a id="3446" href="foundation-core.universal-property-truncation.html#1946" class="Function">is-truncation</a> <a id="3460" href="foundation.universal-property-truncation.html#3433" class="Bound">l</a> <a id="3462" href="foundation.universal-property-truncation.html#3318" class="Bound">B</a> <a id="3464" href="foundation.universal-property-truncation.html#3355" class="Bound">f</a><a id="3465" class="Symbol">)</a> <a id="3467" class="Symbol">→</a> <a id="3469" href="foundation.surjective-maps.html#1938" class="Function">is-surjective</a> <a id="3483" href="foundation.universal-property-truncation.html#3355" class="Bound">f</a>
  <a id="3487" href="foundation.universal-property-truncation.html#3397" class="Function">is-surjective-is-truncation</a> <a id="3515" href="foundation.universal-property-truncation.html#3515" class="Bound">H</a> <a id="3517" class="Symbol">=</a>
    <a id="3523" href="foundation-core.equivalences.html#4187" class="Function">map-inv-is-equiv</a>
      <a id="3546" class="Symbol">(</a> <a id="3548" href="foundation-core.universal-property-truncation.html#6140" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="3602" href="foundation.universal-property-truncation.html#3318" class="Bound">B</a> <a id="3604" href="foundation.universal-property-truncation.html#3355" class="Bound">f</a> <a id="3606" href="foundation.universal-property-truncation.html#3515" class="Bound">H</a>
        <a id="3616" class="Symbol">(</a> <a id="3618" class="Symbol">λ</a> <a id="3620" href="foundation.universal-property-truncation.html#3620" class="Bound">y</a> <a id="3622" class="Symbol">→</a> <a id="3624" href="foundation.propositional-truncations.html#6249" class="Function">truncated-type-trunc-Prop</a> <a id="3650" href="foundation.universal-property-truncation.html#3298" class="Bound">k</a> <a id="3652" class="Symbol">(</a><a id="3653" href="foundation-core.fibers-of-maps.html#942" class="Function">fib</a> <a id="3657" href="foundation.universal-property-truncation.html#3355" class="Bound">f</a> <a id="3659" href="foundation.universal-property-truncation.html#3620" class="Bound">y</a><a id="3660" class="Symbol">)))</a>
      <a id="3670" class="Symbol">(</a> <a id="3672" class="Symbol">λ</a> <a id="3674" href="foundation.universal-property-truncation.html#3674" class="Bound">x</a> <a id="3676" class="Symbol">→</a> <a id="3678" href="foundation.propositional-truncations.html#2290" class="Function">unit-trunc-Prop</a> <a id="3694" class="Symbol">(</a><a id="3695" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="3700" href="foundation.universal-property-truncation.html#3674" class="Bound">x</a> <a id="3702" href="foundation-core.identity-types.html#1820" class="InductiveConstructor">refl</a><a id="3706" class="Symbol">))</a>
<a id="3709" class="Comment">{-
-- Corollary 18.5.4

reflecting-map-mere-eq-unit-trunc-Set :
  {l : Level} (A : UU l) →
  reflecting-map-Eq-Rel (mere-eq-Eq-Rel A) (type-trunc-Set A)
reflecting-map-mere-eq-unit-trunc-Set A =
  pair unit-trunc-Set (reflects-mere-eq (trunc-Set A) unit-trunc-Set)

abstract
  is-set-quotient-trunc-Set :
    {l1 l2 : Level} (A : UU l1) →
    is-set-quotient l2
      ( mere-eq-Eq-Rel A)
      ( trunc-Set A)
      ( reflecting-map-mere-eq-unit-trunc-Set A)
  is-set-quotient-trunc-Set A =
    is-set-quotient-is-set-truncation
      ( trunc-Set A)
      ( unit-trunc-Set)
      ( λ {l} → is-set-truncation-trunc-Set A)

abstract
  is-surjective-and-effective-unit-trunc-Set :
    {l1 : Level} (A : UU l1) →
    is-surjective-and-effective (mere-eq-Eq-Rel A) unit-trunc-Set
  is-surjective-and-effective-unit-trunc-Set A =
    is-surjective-and-effective-is-set-quotient
      ( mere-eq-Eq-Rel A)
      ( trunc-Set A)
      ( unit-trunc-Set)
      ( reflects-mere-eq (trunc-Set A) unit-trunc-Set)
      ( λ {l} → is-set-quotient-trunc-Set A)

abstract
  is-surjective-unit-trunc-Set :
    {l1 : Level} (A : UU l1) → is-surjective (unit-trunc-Set {A = A})
  is-surjective-unit-trunc-Set A =
    pr1 (is-surjective-and-effective-unit-trunc-Set A)

abstract
  is-effective-unit-trunc-Set :
    {l1 : Level} (A : UU l1) →
    is-effective (mere-eq-Eq-Rel A) (unit-trunc-Set {A = A})
  is-effective-unit-trunc-Set A =
    pr2 (is-surjective-and-effective-unit-trunc-Set A)

abstract
  apply-effectiveness-unit-trunc-Set :
    {l1 : Level} {A : UU l1} {x y : A} →
    Id (unit-trunc-Set x) (unit-trunc-Set y) → mere-eq x y
  apply-effectiveness-unit-trunc-Set {A = A} {x} {y} =
    map-equiv (is-effective-unit-trunc-Set A x y)

abstract
  apply-effectiveness-unit-trunc-Set&#39; :
    {l1 : Level} {A : UU l1} {x y : A} →
    mere-eq x y → Id (unit-trunc-Set x) (unit-trunc-Set y)
  apply-effectiveness-unit-trunc-Set&#39; {A = A} {x} {y} =
    map-inv-equiv (is-effective-unit-trunc-Set A x y)

emb-trunc-Set :
  {l1 : Level} (A : UU l1) → type-trunc-Set A ↪ (A → UU-Prop l1)
emb-trunc-Set A =
  emb-is-surjective-and-effective
    ( mere-eq-Eq-Rel A)
    ( trunc-Set A)
    ( unit-trunc-Set)
    ( is-surjective-and-effective-unit-trunc-Set A)

hom-slice-trunc-Set :
  {l1 : Level} (A : UU l1) →
  hom-slice (mere-eq-Prop {A = A}) (map-emb (emb-trunc-Set A))
hom-slice-trunc-Set A =
  pair
    ( unit-trunc-Set)
    ( triangle-emb-is-surjective-and-effective
      ( mere-eq-Eq-Rel A)
      ( trunc-Set A)
      ( unit-trunc-Set)
      ( is-surjective-and-effective-unit-trunc-Set A))

abstract
  is-image-trunc-Set :
    {l1 l2 : Level} (A : UU l1) →
    is-image l2
      ( mere-eq-Prop {A = A})
      ( emb-trunc-Set A)
      ( hom-slice-trunc-Set A)
  is-image-trunc-Set A =
    is-image-is-surjective-and-effective
      ( mere-eq-Eq-Rel A)
      ( trunc-Set A)
      ( unit-trunc-Set)
      ( is-surjective-and-effective-unit-trunc-Set A)

-- Uniqueness of trunc-Set

module _
  {l1 l2 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B)
  {h : type-hom-Set B (trunc-Set A)} (H : (h ∘ f) ~ unit-trunc-Set)
  where

  abstract
    is-equiv-is-set-truncation&#39; :
      ({l : Level} → is-set-truncation l B f) → is-equiv h
    is-equiv-is-set-truncation&#39; Sf =
      is-equiv-is-set-truncation-is-set-truncation
        ( B)
        ( f)
        ( trunc-Set A)
        ( unit-trunc-Set)
        ( H)
        ( Sf)
        ( λ {h} → is-set-truncation-trunc-Set A)

  abstract
    is-set-truncation-is-equiv&#39; :
      is-equiv h → ({l : Level} → is-set-truncation l B f)
    is-set-truncation-is-equiv&#39; Eh =
      is-set-truncation-is-equiv-is-set-truncation
        ( B)
        ( f)
        ( trunc-Set A)
        ( unit-trunc-Set)
        ( H)
        ( λ {l} → is-set-truncation-trunc-Set A)
        ( Eh)

module _
  {l1 l2 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B)
  {h : type-hom-Set (trunc-Set A) B} (H : (h ∘ unit-trunc-Set) ~ f)
  where

  abstract
    is-equiv-is-set-truncation :
      ({l : Level} → is-set-truncation l B f) → is-equiv h
    is-equiv-is-set-truncation Sf =
      is-equiv-is-set-truncation-is-set-truncation
        ( trunc-Set A)
        ( unit-trunc-Set)
        ( B)
        ( f)
        ( H)
        ( λ {l} → is-set-truncation-trunc-Set A)
        ( Sf)

  abstract
    is-set-truncation-is-equiv :
      is-equiv h → ({l : Level} → is-set-truncation l B f)
    is-set-truncation-is-equiv Eh =
      is-set-truncation-is-set-truncation-is-equiv
        ( trunc-Set A)
        ( unit-trunc-Set)
        ( B)
        ( f)
        ( H)
        ( Eh)
        ( λ {l} → is-set-truncation-trunc-Set A)

abstract
  is-equiv-unit-trunc-Set :
    {l : Level} (A : UU-Set l) → is-equiv (unit-trunc-Set {A = type-Set A})
  is-equiv-unit-trunc-Set A =
    is-equiv-is-set-truncation&#39; A id refl-htpy
      ( is-set-truncation-id (is-set-type-Set A))

equiv-unit-trunc-Set :
  {l : Level} (A : UU-Set l) → type-Set A ≃ type-trunc-Set (type-Set A)
equiv-unit-trunc-Set A =
  pair unit-trunc-Set (is-equiv-unit-trunc-Set A)

equiv-unit-trunc-empty-Set : empty ≃ type-trunc-Set empty
equiv-unit-trunc-empty-Set = equiv-unit-trunc-Set empty-Set

abstract
  is-empty-trunc-Set :
    {l : Level} {A : UU l} → is-empty A → is-empty (type-trunc-Set A)
  is-empty-trunc-Set f x = apply-universal-property-trunc-Set x empty-Set f

abstract
  is-empty-is-empty-trunc-Set :
    {l : Level} {A : UU l} → is-empty (type-trunc-Set A) → is-empty A
  is-empty-is-empty-trunc-Set f = f ∘ unit-trunc-Set

equiv-unit-trunc-unit-Set : unit ≃ type-trunc-Set unit
equiv-unit-trunc-unit-Set = equiv-unit-trunc-Set unit-Set

equiv-unit-trunc-ℕ-Set : ℕ ≃ type-trunc-Set ℕ
equiv-unit-trunc-ℕ-Set = equiv-unit-trunc-Set ℕ-Set

equiv-unit-trunc-ℤ-Set : ℤ ≃ type-trunc-Set ℤ
equiv-unit-trunc-ℤ-Set = equiv-unit-trunc-Set ℤ-Set

equiv-unit-trunc-Fin-Set : (k : ℕ) → Fin k ≃ type-trunc-Set (Fin k)
equiv-unit-trunc-Fin-Set k = equiv-unit-trunc-Set (Fin-Set k)

abstract
  is-contr-trunc-Set :
    {l : Level} {A : UU l} → is-contr A → is-contr (type-trunc-Set A)
  is-contr-trunc-Set {l} {A} H =
    is-contr-equiv&#39;
      ( A)
      ( equiv-unit-trunc-Set (pair A (is-set-is-contr H)))
      ( H)

module _
  {l1 l2 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B)
  (Sf : {l : Level} → is-set-truncation l B f)
  where

  abstract
    uniqueness-trunc-Set :
      is-contr
        ( Σ (type-trunc-Set A ≃ type-Set B)
        ( λ e → (map-equiv e ∘ unit-trunc-Set) ~ f))
    uniqueness-trunc-Set =
      uniqueness-set-truncation (trunc-Set A) unit-trunc-Set B f
        ( λ {l} → is-set-truncation-trunc-Set A)
        ( Sf)

  equiv-uniqueness-trunc-Set : type-trunc-Set A ≃ type-Set B
  equiv-uniqueness-trunc-Set =
    pr1 (center uniqueness-trunc-Set)

  map-equiv-uniqueness-trunc-Set : type-trunc-Set A → type-Set B
  map-equiv-uniqueness-trunc-Set =
    map-equiv equiv-uniqueness-trunc-Set

  triangle-uniqueness-trunc-Set :
    (map-equiv-uniqueness-trunc-Set ∘ unit-trunc-Set) ~ f
  triangle-uniqueness-trunc-Set =
    pr2 (center uniqueness-trunc-Set)

module _
  {l1 l2 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B)
  (Sf : {l : Level} → is-set-truncation l B f)
  where

  abstract
    uniqueness-trunc-Set&#39; :
      is-contr
        ( Σ ( type-Set B ≃ type-trunc-Set A)
            ( λ e → (map-equiv e ∘ f) ~ unit-trunc-Set))
    uniqueness-trunc-Set&#39; =
      uniqueness-set-truncation B f (trunc-Set A) unit-trunc-Set Sf
        ( λ {l} → is-set-truncation-trunc-Set A)

  equiv-uniqueness-trunc-Set&#39; : type-Set B ≃ type-trunc-Set A
  equiv-uniqueness-trunc-Set&#39; =
    pr1 (center uniqueness-trunc-Set&#39;)

  map-equiv-uniqueness-trunc-Set&#39; : type-Set B → type-trunc-Set A
  map-equiv-uniqueness-trunc-Set&#39; =
    map-equiv equiv-uniqueness-trunc-Set&#39;
  
  triangle-uniqueness-trunc-Set&#39; :
    (map-equiv-uniqueness-trunc-Set&#39; ∘ f) ~ unit-trunc-Set
  triangle-uniqueness-trunc-Set&#39; =
    pr2 (center uniqueness-trunc-Set&#39;)

-- Proposition 18.5.5

module _
  {l1 l2 : Level} {A : UU l1} {B : UU l2} (f : A → B)
  where

  abstract
    unique-map-trunc-Set :
      is-contr
        ( Σ ( type-trunc-Set A → type-trunc-Set B)
            ( λ h → (h ∘ unit-trunc-Set) ~ (unit-trunc-Set ∘ f)))
    unique-map-trunc-Set =
      universal-property-trunc-Set A (trunc-Set B) (unit-trunc-Set ∘ f)

  map-trunc-Set :
    type-trunc-Set A → type-trunc-Set B
  map-trunc-Set =
    pr1 (center unique-map-trunc-Set)

  naturality-trunc-Set :
    (map-trunc-Set ∘ unit-trunc-Set) ~ (unit-trunc-Set ∘ f)
  naturality-trunc-Set =
    pr2 (center unique-map-trunc-Set)

  htpy-map-trunc-Set :
    (h : type-trunc-Set A → type-trunc-Set B) →
    (H : (h ∘ unit-trunc-Set) ~ (unit-trunc-Set ∘ f)) →
    map-trunc-Set ~ h
  htpy-map-trunc-Set h H =
    htpy-eq
      ( ap pr1
        ( eq-is-contr unique-map-trunc-Set
          { pair map-trunc-Set naturality-trunc-Set}
          { pair h H}))

map-id-trunc-Set :
  {l1 : Level} {A : UU l1} → map-trunc-Set (id {A = A}) ~ id
map-id-trunc-Set {l1} {A} =
  htpy-eq
    ( ap pr1
      ( eq-is-contr
        ( universal-property-trunc-Set A (trunc-Set A) unit-trunc-Set)
        { pair (map-trunc-Set id) (naturality-trunc-Set id)}
        { pair id refl-htpy}))

map-comp-trunc-Set :
  {l1 l2 l3 : Level} {A : UU l1} {B : UU l2} {C : UU l3}
  (g : B → C) (f : A → B) →
  map-trunc-Set (g ∘ f) ~ (map-trunc-Set g ∘ map-trunc-Set f)
map-comp-trunc-Set {A = A} {C = C} g f =
  htpy-eq
    ( ap pr1
      ( eq-is-contr
        ( universal-property-trunc-Set
          A
          (trunc-Set C)
          (unit-trunc-Set ∘ (g ∘ f)))
        { pair (map-trunc-Set (g ∘ f)) (naturality-trunc-Set (g ∘ f))}
        { pair ( map-trunc-Set g ∘ map-trunc-Set f)
               ( ( map-trunc-Set g ·l naturality-trunc-Set f) ∙h
                 ( naturality-trunc-Set g ·r f))}))

htpy-trunc-Set :
  {l1 l2 : Level} {A : UU l1} {B : UU l2} {f g : A → B} →
  (f ~ g) → (map-trunc-Set f ~ map-trunc-Set g)
htpy-trunc-Set {B = B} {f = f} {g} H =
  map-inv-is-equiv
    ( dependent-universal-property-trunc-Set
      ( λ x →
        set-Prop
          ( Id-Prop (trunc-Set B) (map-trunc-Set f x) (map-trunc-Set g x))))
    ( λ a →
      ( naturality-trunc-Set f a) ∙
      ( ( ap unit-trunc-Set (H a)) ∙
        ( inv (naturality-trunc-Set g a))))

abstract
  is-equiv-map-trunc-Set :
    {l1 l2 : Level} {A : UU l1} {B : UU l2} {f : A → B} →
    is-equiv f → is-equiv (map-trunc-Set f)
  is-equiv-map-trunc-Set {f = f} H =
    pair
      ( pair
        ( map-trunc-Set (pr1 (pr1 H)))
        ( ( inv-htpy (map-comp-trunc-Set f (pr1 (pr1 H)))) ∙h
          ( ( htpy-trunc-Set (pr2 (pr1 H))) ∙h
            ( map-id-trunc-Set))))
      ( pair
        ( map-trunc-Set (pr1 (pr2 H)))
        ( ( inv-htpy (map-comp-trunc-Set (pr1 (pr2 H)) f)) ∙h
          ( ( htpy-trunc-Set (pr2 (pr2 H))) ∙h
            ( map-id-trunc-Set))))

equiv-trunc-Set :
  {l1 l2 : Level} {A : UU l1} {B : UU l2} →
  (A ≃ B) → (type-trunc-Set A ≃ type-trunc-Set B)
equiv-trunc-Set e =
  pair
    ( map-trunc-Set (map-equiv e))
    ( is-equiv-map-trunc-Set (is-equiv-map-equiv e))

map-equiv-trunc-Set :
  {l1 l2 : Level} {A : UU l1} {B : UU l2} →
  (A ≃ B) → type-trunc-Set A → type-trunc-Set B
map-equiv-trunc-Set e = map-equiv (equiv-trunc-Set e)

--------------------------------------------------------------------------------

module _
  {l1 l2 : Level} (A : UU l1) (B : UU l2)
  where

  abstract
    distributive-trunc-coprod-Set :
      is-contr
        ( Σ ( type-equiv-Set
              ( trunc-Set (coprod A B))
              ( coprod-Set (trunc-Set A) (trunc-Set B)))
            ( λ e →
              ( map-equiv e ∘ unit-trunc-Set) ~
              ( map-coprod unit-trunc-Set unit-trunc-Set)))
    distributive-trunc-coprod-Set =
      uniqueness-trunc-Set
        ( coprod-Set (trunc-Set A) (trunc-Set B))
        ( map-coprod unit-trunc-Set unit-trunc-Set)
        ( λ {l} C →
          is-equiv-right-factor&#39;
            ( ev-inl-inr (λ x → type-Set C))
            ( precomp-Set (map-coprod unit-trunc-Set unit-trunc-Set) C)
            ( universal-property-coprod (type-Set C))
            ( is-equiv-comp&#39;
              ( map-prod
                ( precomp-Set unit-trunc-Set C)
                ( precomp-Set unit-trunc-Set C))
              ( ev-inl-inr (λ x → type-Set C))
              ( universal-property-coprod (type-Set C))
              ( is-equiv-map-prod
                ( precomp-Set unit-trunc-Set C)
                ( precomp-Set unit-trunc-Set C)
                ( is-set-truncation-trunc-Set A C)
                ( is-set-truncation-trunc-Set B C))))

  equiv-distributive-trunc-coprod-Set :
    type-equiv-Set
      ( trunc-Set (coprod A B))
      ( coprod-Set (trunc-Set A) (trunc-Set B))
  equiv-distributive-trunc-coprod-Set =
    pr1 (center distributive-trunc-coprod-Set)

  map-equiv-distributive-trunc-coprod-Set :
    type-hom-Set
      ( trunc-Set (coprod A B))
      ( coprod-Set (trunc-Set A) (trunc-Set B))
  map-equiv-distributive-trunc-coprod-Set =
    map-equiv equiv-distributive-trunc-coprod-Set

  triangle-distributive-trunc-coprod-Set :
    ( map-equiv-distributive-trunc-coprod-Set ∘ unit-trunc-Set) ~
    ( map-coprod unit-trunc-Set unit-trunc-Set)
  triangle-distributive-trunc-coprod-Set =
    pr2 (center distributive-trunc-coprod-Set)

-- Set truncations of Σ-types

module _
  {l1 l2 : Level} (A : UU l1) (B : A → UU l2)
  where

  abstract
    trunc-Σ-Set :
      is-contr
        ( Σ ( type-trunc-Set (Σ A B) ≃
              type-trunc-Set (Σ A (λ x → type-trunc-Set (B x))))
            ( λ e →
              ( map-equiv e ∘ unit-trunc-Set) ~
              ( unit-trunc-Set ∘ tot (λ x → unit-trunc-Set))))
    trunc-Σ-Set =
      uniqueness-trunc-Set
        ( trunc-Set (Σ A (λ x → type-trunc-Set (B x))))
        ( unit-trunc-Set ∘ tot (λ x → unit-trunc-Set))
        ( λ {l} C →
          is-equiv-right-factor&#39;
            ( ev-pair)
            ( precomp-Set (unit-trunc-Set ∘ tot (λ x → unit-trunc-Set)) C)
            ( is-equiv-ev-pair)
            ( is-equiv-htpy-equiv
              ( ( equiv-map-Π
                  ( λ x → equiv-universal-property-trunc-Set (B x) C)) ∘e
                ( ( equiv-ev-pair) ∘e
                  ( equiv-universal-property-trunc-Set
                    ( Σ A (type-trunc-Set ∘ B)) C)))
              ( refl-htpy)))

  equiv-trunc-Σ-Set :
    type-trunc-Set (Σ A B) ≃ type-trunc-Set (Σ A (λ x → type-trunc-Set (B x)))
  equiv-trunc-Σ-Set =
    pr1 (center trunc-Σ-Set)

  map-equiv-trunc-Σ-Set :
    type-trunc-Set (Σ A B) → type-trunc-Set (Σ A (λ x → type-trunc-Set (B x)))
  map-equiv-trunc-Σ-Set =
    map-equiv equiv-trunc-Σ-Set

  square-trunc-Σ-Set :
    ( map-equiv-trunc-Σ-Set ∘ unit-trunc-Set) ~
    ( unit-trunc-Set ∘ tot (λ x → unit-trunc-Set))
  square-trunc-Σ-Set =
    pr2 (center trunc-Σ-Set)

  htpy-map-equiv-trunc-Σ-Set :
    map-trunc-Set (tot (λ x → unit-trunc-Set)) ~ map-equiv-trunc-Σ-Set
  htpy-map-equiv-trunc-Σ-Set =
    htpy-map-trunc-Set
      ( tot (λ x → unit-trunc-Set))
      ( map-equiv-trunc-Σ-Set)
      ( square-trunc-Σ-Set)

  abstract
    is-equiv-map-trunc-tot-unit-trunc-Set :
      is-equiv (map-trunc-Set (tot (λ (x : A) → unit-trunc-Set {A = B x})))
    is-equiv-map-trunc-tot-unit-trunc-Set =
      is-equiv-htpy-equiv
        ( equiv-trunc-Σ-Set)
        ( htpy-map-equiv-trunc-Σ-Set)

-- trunc-Set distributes over products

module _
  {l1 l2 : Level} (A : UU l1) (B : UU l2)
  where

  abstract
    distributive-trunc-prod-Set :
      is-contr
        ( Σ ( type-trunc-Set (A × B) ≃ ( type-trunc-Set A × type-trunc-Set B))
            ( λ e →
              ( map-equiv e ∘ unit-trunc-Set) ~
              ( map-prod unit-trunc-Set unit-trunc-Set)))
    distributive-trunc-prod-Set =
      uniqueness-trunc-Set
        ( prod-Set (trunc-Set A) (trunc-Set B))
        ( map-prod unit-trunc-Set unit-trunc-Set)
        ( λ {l} C →
          is-equiv-right-factor&#39;
            ( ev-pair)
            ( precomp-Set (map-prod unit-trunc-Set unit-trunc-Set) C)
            ( is-equiv-ev-pair)
            ( is-equiv-htpy-equiv
              ( ( equiv-universal-property-trunc-Set A (Π-Set&#39; B (λ y → C))) ∘e
                ( ( equiv-postcomp
                    ( type-trunc-Set A)
                    (equiv-universal-property-trunc-Set B C)) ∘e
                  ( equiv-ev-pair)))
              ( refl-htpy)))

  equiv-distributive-trunc-prod-Set :
    type-trunc-Set (A × B) ≃ ( type-trunc-Set A × type-trunc-Set B)
  equiv-distributive-trunc-prod-Set =
    pr1 (center distributive-trunc-prod-Set)

  map-equiv-distributive-trunc-prod-Set :
    type-trunc-Set (A × B) → type-trunc-Set A × type-trunc-Set B
  map-equiv-distributive-trunc-prod-Set =
    map-equiv equiv-distributive-trunc-prod-Set

  triangle-distributive-trunc-prod-Set :
    ( map-equiv-distributive-trunc-prod-Set ∘ unit-trunc-Set) ~
    ( map-prod unit-trunc-Set unit-trunc-Set)
  triangle-distributive-trunc-prod-Set =
    pr2 (center distributive-trunc-prod-Set)

-- trunc-Set distributes over Π indexed by Fin

abstract
  distributive-trunc-Π-Fin-Set :
    {l : Level} (k : ℕ) (A : Fin k → UU l) →
    is-contr
      ( Σ ( ( type-trunc-Set ((x : Fin k) → A x)) ≃
            ( (x : Fin k) → type-trunc-Set (A x)))
          ( λ e →
            ( map-equiv e ∘ unit-trunc-Set) ~
            ( map-Π (λ x → unit-trunc-Set))))
  distributive-trunc-Π-Fin-Set zero-ℕ A =
    uniqueness-trunc-Set
      ( Π-Set empty-Set (λ x → trunc-Set (A x)))
      ( map-Π (λ x → unit-trunc-Set))
      ( λ {l} B →
        is-equiv-precomp-is-equiv
          ( map-Π (λ x → unit-trunc-Set))
          ( is-equiv-is-contr
            ( map-Π (λ x → unit-trunc-Set))
            ( dependent-universal-property-empty&#39; A)
            ( dependent-universal-property-empty&#39; (type-trunc-Set ∘ A)))
          ( type-Set B))
  distributive-trunc-Π-Fin-Set (succ-ℕ k) A =
    uniqueness-trunc-Set
      ( Π-Set (Fin-Set (succ-ℕ k)) (λ x → trunc-Set (A x)))
      ( map-Π (λ x → unit-trunc-Set))
      ( λ {l} B →
        is-equiv-left-factor&#39;
          ( precomp (map-Π (λ x → unit-trunc-Set)) (type-Set B))
          ( precomp (ev-Maybe {B = type-trunc-Set ∘ A}) (type-Set B))
          ( is-equiv-comp&#39;
            ( precomp ev-Maybe (type-Set B))
            ( precomp
              ( map-prod (map-Π (λ x → unit-trunc-Set)) unit-trunc-Set)
              ( type-Set B))
            ( is-equiv-right-factor&#39;
              ( ev-pair)
              ( precomp
                ( map-prod (map-Π (λ x → unit-trunc-Set)) unit-trunc-Set)
                ( type-Set B))
              ( is-equiv-ev-pair)
              ( is-equiv-htpy-equiv
                ( ( ( pair
                      ( precomp
                        ( (map-Π (λ x → unit-trunc-Set)))
                        ( A (inr star) → type-Set B))
                      ( is-set-truncation-is-equiv
                        ( Π-Set (Fin-Set k) (λ x → trunc-Set (A (inl x))))
                        ( map-Π (λ x → unit-trunc-Set))
                        { map-equiv
                          ( pr1
                            ( center
                              ( distributive-trunc-Π-Fin-Set k (A ∘ inl))))}
                        ( pr2
                          ( center (distributive-trunc-Π-Fin-Set k (A ∘ inl))))
                        ( is-equiv-map-equiv
                          ( pr1
                            ( center
                              ( distributive-trunc-Π-Fin-Set k (A ∘ inl)))))
                        ( Π-Set&#39; (A (inr star)) (λ a → B)))) ∘e
                    ( equiv-postcomp
                      ( (x : Fin k) → type-trunc-Set (A (inl x)))
                      ( equiv-universal-property-trunc-Set
                        ( A (inr star))
                        ( B)))) ∘e
                  ( equiv-ev-pair))
                ( refl-htpy)))
            ( is-equiv-precomp-is-equiv
              ( ev-Maybe)
              ( dependent-universal-property-Maybe)
              ( type-Set B)))
          ( is-equiv-precomp-is-equiv
            ( ev-Maybe)
            ( dependent-universal-property-Maybe)
            ( type-Set B)))

module _
  {l : Level} (k : ℕ) (A : Fin k → UU l)
  where

  equiv-distributive-trunc-Π-Fin-Set :
    type-trunc-Set ((x : Fin k) → A x) ≃ ((x : Fin k) → type-trunc-Set (A x))
  equiv-distributive-trunc-Π-Fin-Set =
    pr1 (center (distributive-trunc-Π-Fin-Set k A))

  map-equiv-distributive-trunc-Π-Fin-Set :
    type-trunc-Set ((x : Fin k) → A x) → ((x : Fin k) → type-trunc-Set (A x))
  map-equiv-distributive-trunc-Π-Fin-Set =
    map-equiv equiv-distributive-trunc-Π-Fin-Set

  triangle-distributive-trunc-Π-Fin-Set :
    ( map-equiv-distributive-trunc-Π-Fin-Set ∘ unit-trunc-Set) ~
    ( map-Π (λ x → unit-trunc-Set))
  triangle-distributive-trunc-Π-Fin-Set =
    pr2 (center (distributive-trunc-Π-Fin-Set k A))

module _
  {l1 l2 : Level} {A : UU l1} (B : A → UU l2)
  where

  abstract
    distributive-trunc-Π-count-Set :
      count A → 
      is-contr
        ( Σ ( ( type-trunc-Set ((x : A) → B x)) ≃
              ( (x : A) → type-trunc-Set (B x)))
            ( λ e →
              ( map-equiv e ∘ unit-trunc-Set) ~
              ( map-Π (λ x → unit-trunc-Set))))
    distributive-trunc-Π-count-Set (pair k e) =
      is-contr-equiv
        ( Σ ( ( type-trunc-Set ((x : A) → B x)) ≃
              ( (x : Fin k) → type-trunc-Set (B (map-equiv e x))))
            ( λ f →
              ( map-equiv f ∘ unit-trunc-Set) ~
              ( map-Π (λ x → unit-trunc-Set) ∘ precomp-Π (map-equiv e) B)))
        ( equiv-Σ
          ( λ f →
            ( map-equiv f ∘ unit-trunc-Set) ~
            ( map-Π (λ x → unit-trunc-Set) ∘ precomp-Π (map-equiv e) B))
          ( equiv-postcomp-equiv
            ( equiv-precomp-Π e (type-trunc-Set ∘ B))
            ( type-trunc-Set ((x : A) → B x)))
          ( λ f →
            equiv-map-Π
              ( λ h →
                ( ( inv-equiv equiv-funext) ∘e
                  ( equiv-precomp-Π e
                    ( λ x → Id ((map-equiv f ∘ unit-trunc-Set) h x)
                    ( map-Π (λ y → unit-trunc-Set) h x)))) ∘e
                ( equiv-funext))))
        ( is-contr-equiv&#39;
          ( Σ ( ( type-trunc-Set ((x : Fin k) → B (map-equiv e x))) ≃
                ( (x : Fin k) → type-trunc-Set (B (map-equiv e x))))
              ( λ f →
                ( map-equiv f ∘ unit-trunc-Set) ~
                ( map-Π (λ x → unit-trunc-Set))))
          ( equiv-Σ
            ( λ f →
              ( map-equiv f ∘ unit-trunc-Set) ~
              ( map-Π (λ x → unit-trunc-Set) ∘ precomp-Π (map-equiv e) B))
            ( equiv-precomp-equiv
              ( equiv-trunc-Set (equiv-precomp-Π e B))
              ( (x : Fin k) → type-trunc-Set (B (map-equiv e x))))
            ( λ f →
              equiv-Π
                ( λ h →
                  Id ( map-equiv f
                       ( map-equiv
                         ( equiv-trunc-Set (equiv-precomp-Π e B))
                         ( unit-trunc-Set h)))
                     ( map-Π (λ x → unit-trunc-Set) (λ x → h (map-equiv e x))))
                ( equiv-Π B e (λ x → id-equiv))
                ( λ h →
                  ( ( inv-equiv equiv-funext) ∘e
                    ( equiv-Π
                      ( λ x →
                        Id ( map-equiv f
                             ( map-equiv-trunc-Set
                               ( equiv-precomp-Π e B)
                               ( unit-trunc-Set
                                 ( map-equiv-Π B e (λ x → id-equiv) h)))
                             ( x))
                           ( unit-trunc-Set
                             ( map-equiv-Π B e
                               ( λ z → id-equiv)
                               ( h)
                               ( map-equiv e x))))
                      ( id-equiv)
                      ( λ x →
                        ( equiv-concat
                          ( ap
                            ( λ t → map-equiv f t x)
                            ( ( naturality-trunc-Set (precomp-Π (map-equiv e) B)
                                ( map-equiv-Π B e (λ _ → id-equiv) h)) ∙
                              ( ap
                                ( unit-trunc-Set)
                                ( eq-htpy
                                  ( compute-map-equiv-Π B e
                                    ( λ _ → id-equiv)
                                    ( h))))))
                          ( unit-trunc-Set
                            ( map-equiv-Π B e
                              ( λ _ → id-equiv)
                              ( h)
                              ( map-equiv e x)))) ∘e
                        ( equiv-concat&#39;
                          ( map-equiv f (unit-trunc-Set h) x)
                          ( ap unit-trunc-Set
                            ( inv
                              ( compute-map-equiv-Π B e
                                ( λ _ → id-equiv)
                                ( h)
                                ( x)))))))) ∘e
                  ( equiv-funext))))
          ( distributive-trunc-Π-Fin-Set k (B ∘ map-equiv e)))

module _
  {l1 l2 : Level} {A : UU l1} (B : A → UU l2) (c : count A)
  where

  equiv-distributive-trunc-Π-count-Set :
    ( type-trunc-Set ((x : A) → B x)) ≃ ((x : A) → type-trunc-Set (B x))
  equiv-distributive-trunc-Π-count-Set =
    pr1 (center (distributive-trunc-Π-count-Set B c))

  map-equiv-distributive-trunc-Π-count-Set :
    ( type-trunc-Set ((x : A) → B x)) → ((x : A) → type-trunc-Set (B x))
  map-equiv-distributive-trunc-Π-count-Set =
    map-equiv equiv-distributive-trunc-Π-count-Set

  triangle-distributive-trunc-Π-count-Set :
    ( map-equiv-distributive-trunc-Π-count-Set ∘ unit-trunc-Set) ~
    ( map-Π (λ x → unit-trunc-Set))
  triangle-distributive-trunc-Π-count-Set =
    pr2 (center (distributive-trunc-Π-count-Set B c))

module _
  {l1 l2 : Level} {A : UU l1} (B : A → UU l2) (H : is-finite A)
  where

  abstract
    distributive-trunc-Π-is-finite-Set :
      is-contr
        ( Σ ( ( type-trunc-Set ((x : A) → B x)) ≃
              ( (x : A) → type-trunc-Set (B x)))
            ( λ e →
              ( map-equiv e ∘ unit-trunc-Set) ~
              ( map-Π (λ x → unit-trunc-Set))))
    distributive-trunc-Π-is-finite-Set =
      apply-universal-property-trunc-Prop H
        ( is-contr-Prop _)
        ( distributive-trunc-Π-count-Set B)

  equiv-distributive-trunc-Π-is-finite-Set :
    ( type-trunc-Set ((x : A) → B x)) ≃ ((x : A) → type-trunc-Set (B x))
  equiv-distributive-trunc-Π-is-finite-Set =
    pr1 (center distributive-trunc-Π-is-finite-Set)

  map-equiv-distributive-trunc-Π-is-finite-Set :
    ( type-trunc-Set ((x : A) → B x)) → ((x : A) → type-trunc-Set (B x))
  map-equiv-distributive-trunc-Π-is-finite-Set =
    map-equiv equiv-distributive-trunc-Π-is-finite-Set

  triangle-distributive-trunc-Π-is-finite-Set :
    ( map-equiv-distributive-trunc-Π-is-finite-Set ∘ unit-trunc-Set) ~
    ( map-Π (λ x → unit-trunc-Set))
  triangle-distributive-trunc-Π-is-finite-Set =
    pr2 (center distributive-trunc-Π-is-finite-Set)
    -}</a>
</pre>