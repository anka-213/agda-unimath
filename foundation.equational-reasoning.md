---
title: Equational reasoning
---

Tom de Jong, 27 May 2022.
Elisabeth Bonnevier, 31 May 2022.

<pre class="Agda"><a id="107" class="Symbol">{-#</a> <a id="111" class="Keyword">OPTIONS</a> <a id="119" class="Pragma">--without-K</a> <a id="131" class="Pragma">--exact-split</a> <a id="145" class="Symbol">#-}</a>

<a id="150" class="Keyword">module</a> <a id="157" href="foundation.equational-reasoning.html" class="Module">foundation.equational-reasoning</a> <a id="189" class="Keyword">where</a>

<a id="196" class="Keyword">open</a> <a id="201" class="Keyword">import</a> <a id="208" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="234" class="Keyword">using</a> <a id="240" class="Symbol">(</a><a id="241" href="foundation-core.identity-types.html#1865" class="Function Operator">_＝_</a><a id="244" class="Symbol">;</a> <a id="246" href="foundation-core.identity-types.html#1820" class="InductiveConstructor">refl</a><a id="250" class="Symbol">;</a> <a id="252" href="foundation-core.identity-types.html#2425" class="Function Operator">_∙_</a><a id="255" class="Symbol">;</a> <a id="257" href="foundation-core.identity-types.html#2729" class="Function">inv</a><a id="260" class="Symbol">)</a>
<a id="262" class="Keyword">open</a> <a id="267" class="Keyword">import</a> <a id="274" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="298" class="Keyword">using</a> <a id="304" class="Symbol">(</a><a id="305" href="foundation-core.equivalences.html#1621" class="Function Operator">_≃_</a><a id="308" class="Symbol">;</a> <a id="310" href="foundation-core.equivalences.html#7869" class="Function Operator">_∘e_</a><a id="314" class="Symbol">;</a> <a id="316" href="foundation-core.equivalences.html#2494" class="Function">id-equiv</a><a id="324" class="Symbol">;</a> <a id="326" href="foundation-core.equivalences.html#5721" class="Function">inv-equiv</a><a id="335" class="Symbol">)</a>
<a id="337" class="Keyword">open</a> <a id="342" class="Keyword">import</a> <a id="349" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="376" class="Keyword">using</a> <a id="382" class="Symbol">(</a><a id="383" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="388" class="Symbol">;</a> <a id="390" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="392" class="Symbol">)</a>
<a id="394" class="Keyword">open</a> <a id="399" class="Keyword">import</a> <a id="406" href="order-theory.preorders.html" class="Module">order-theory.preorders</a> <a id="429" class="Keyword">using</a>
  <a id="437" class="Symbol">(</a> <a id="439" href="order-theory.preorders.html#531" class="Function">Preorder</a><a id="447" class="Symbol">;</a> <a id="449" href="order-theory.preorders.html#873" class="Function">element-Preorder</a><a id="465" class="Symbol">;</a> <a id="467" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a><a id="479" class="Symbol">;</a> <a id="481" href="order-theory.preorders.html#1385" class="Function">transitive-leq-Preorder</a><a id="504" class="Symbol">;</a>
    <a id="510" href="order-theory.preorders.html#1280" class="Function">refl-leq-Preorder</a><a id="527" class="Symbol">)</a>
</pre>
## Idea

Often it's convenient to reason by chains of (in)equalities or equivalences,
i.e., to write a proof in the following form:

```md
X ≃ by equiv-1 to
A ≃ by equiv-2 to
B ≃ by equiv-3 to
Y ∎e
```

or
```md
x ≤ X by ineq-1 to
a ≤ X by ineq-2 to
b ≤ X by ineq-3 to
c ∎ X
```

where `equiv-x` and `ineq-x` are proofs of respectively the equivalences or
inequalities. The symbol ∎ marks the end of a chain.

Because we will want to have equational reasoning for both identifications and
equivalences and we can't use the same symbol twice, we use ∎ for
identifications and ■ for equivalences in the code below.

For inequalities we also need to pass the preorder as an argument.

We write Agda code that allows for such reasoning. The code for equational
reasoning for equalities and equivalences is based on Martín Escardó's Agda code
[1,2] and the Agda standard library [3].


## Definitions

### Equational reasoning for identifications

<pre class="Agda"><a id="1485" class="Keyword">infix</a> <a id="1491" class="Number">1</a> <a id="1493" href="foundation.equational-reasoning.html#1668" class="Function Operator">_∎</a>
<a id="1496" class="Keyword">infixr</a> <a id="1503" class="Number">0</a> <a id="1505" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a>

<a id="step-equational-reasoning"></a><a id="1532" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a> <a id="1558" class="Symbol">:</a>
  <a id="1562" class="Symbol">{</a><a id="1563" href="foundation.equational-reasoning.html#1563" class="Bound">l</a> <a id="1565" class="Symbol">:</a> <a id="1567" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1572" class="Symbol">}</a> <a id="1574" class="Symbol">{</a><a id="1575" href="foundation.equational-reasoning.html#1575" class="Bound">X</a> <a id="1577" class="Symbol">:</a> <a id="1579" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1582" href="foundation.equational-reasoning.html#1563" class="Bound">l</a><a id="1583" class="Symbol">}</a> <a id="1585" class="Symbol">(</a><a id="1586" href="foundation.equational-reasoning.html#1586" class="Bound">x</a> <a id="1588" class="Symbol">:</a> <a id="1590" href="foundation.equational-reasoning.html#1575" class="Bound">X</a><a id="1591" class="Symbol">)</a> <a id="1593" class="Symbol">{</a><a id="1594" href="foundation.equational-reasoning.html#1594" class="Bound">y</a> <a id="1596" href="foundation.equational-reasoning.html#1596" class="Bound">z</a> <a id="1598" class="Symbol">:</a> <a id="1600" href="foundation.equational-reasoning.html#1575" class="Bound">X</a><a id="1601" class="Symbol">}</a> <a id="1603" class="Symbol">→</a> <a id="1605" href="foundation.equational-reasoning.html#1594" class="Bound">y</a> <a id="1607" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1609" href="foundation.equational-reasoning.html#1596" class="Bound">z</a> <a id="1611" class="Symbol">→</a> <a id="1613" href="foundation.equational-reasoning.html#1586" class="Bound">x</a> <a id="1615" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1617" href="foundation.equational-reasoning.html#1594" class="Bound">y</a> <a id="1619" class="Symbol">→</a> <a id="1621" href="foundation.equational-reasoning.html#1586" class="Bound">x</a> <a id="1623" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1625" href="foundation.equational-reasoning.html#1596" class="Bound">z</a>
<a id="1627" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a> <a id="1653" class="Symbol">_</a> <a id="1655" href="foundation.equational-reasoning.html#1655" class="Bound">q</a> <a id="1657" href="foundation.equational-reasoning.html#1657" class="Bound">p</a> <a id="1659" class="Symbol">=</a> <a id="1661" href="foundation.equational-reasoning.html#1657" class="Bound">p</a> <a id="1663" href="foundation-core.identity-types.html#2425" class="Function Operator">∙</a> <a id="1665" href="foundation.equational-reasoning.html#1655" class="Bound">q</a>

<a id="_∎"></a><a id="1668" href="foundation.equational-reasoning.html#1668" class="Function Operator">_∎</a> <a id="1671" class="Symbol">:</a> <a id="1673" class="Symbol">{</a><a id="1674" href="foundation.equational-reasoning.html#1674" class="Bound">l</a> <a id="1676" class="Symbol">:</a> <a id="1678" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1683" class="Symbol">}</a> <a id="1685" class="Symbol">{</a><a id="1686" href="foundation.equational-reasoning.html#1686" class="Bound">X</a> <a id="1688" class="Symbol">:</a> <a id="1690" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1693" href="foundation.equational-reasoning.html#1674" class="Bound">l</a><a id="1694" class="Symbol">}</a> <a id="1696" class="Symbol">(</a><a id="1697" href="foundation.equational-reasoning.html#1697" class="Bound">x</a> <a id="1699" class="Symbol">:</a> <a id="1701" href="foundation.equational-reasoning.html#1686" class="Bound">X</a><a id="1702" class="Symbol">)</a> <a id="1704" class="Symbol">→</a> <a id="1706" href="foundation.equational-reasoning.html#1697" class="Bound">x</a> <a id="1708" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1710" href="foundation.equational-reasoning.html#1697" class="Bound">x</a>
<a id="1712" href="foundation.equational-reasoning.html#1712" class="Bound">x</a> <a id="1714" href="foundation.equational-reasoning.html#1668" class="Function Operator">∎</a> <a id="1716" class="Symbol">=</a> <a id="1718" href="foundation-core.identity-types.html#1820" class="InductiveConstructor">refl</a>

<a id="1724" class="Keyword">syntax</a> <a id="1731" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a> <a id="1757" class="Bound">x</a> <a id="1759" class="Bound">q</a> <a id="1761" class="Bound">p</a> <a id="1763" class="Symbol">=</a> <a id="1765" class="Bound">x</a> <a id="1767" class="Function">＝</a> <a id="1769" class="Function">by</a> <a id="1772" class="Bound">p</a> <a id="1774" class="Function">to</a> <a id="1777" class="Bound">q</a>
</pre>
### Equational reasoning for equivalences

<pre class="Agda"><a id="1835" class="Keyword">infix</a> <a id="1841" class="Number">1</a> <a id="1843" href="foundation.equational-reasoning.html#2040" class="Function Operator">_∎e</a>
<a id="1847" class="Keyword">infixr</a> <a id="1854" class="Number">0</a> <a id="1856" href="foundation.equational-reasoning.html#1884" class="Function">step-equivalence-reasoning</a>

<a id="step-equivalence-reasoning"></a><a id="1884" href="foundation.equational-reasoning.html#1884" class="Function">step-equivalence-reasoning</a> <a id="1911" class="Symbol">:</a>
  <a id="1915" class="Symbol">{</a><a id="1916" href="foundation.equational-reasoning.html#1916" class="Bound">l1</a> <a id="1919" href="foundation.equational-reasoning.html#1919" class="Bound">l2</a> <a id="1922" href="foundation.equational-reasoning.html#1922" class="Bound">l3</a> <a id="1925" class="Symbol">:</a> <a id="1927" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1932" class="Symbol">}</a> <a id="1934" class="Symbol">(</a><a id="1935" href="foundation.equational-reasoning.html#1935" class="Bound">X</a> <a id="1937" class="Symbol">:</a> <a id="1939" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1942" href="foundation.equational-reasoning.html#1916" class="Bound">l1</a><a id="1944" class="Symbol">)</a> <a id="1946" class="Symbol">{</a><a id="1947" href="foundation.equational-reasoning.html#1947" class="Bound">Y</a> <a id="1949" class="Symbol">:</a> <a id="1951" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1954" href="foundation.equational-reasoning.html#1919" class="Bound">l2</a> <a id="1957" class="Symbol">}</a> <a id="1959" class="Symbol">{</a><a id="1960" href="foundation.equational-reasoning.html#1960" class="Bound">Z</a> <a id="1962" class="Symbol">:</a> <a id="1964" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1967" href="foundation.equational-reasoning.html#1922" class="Bound">l3</a><a id="1969" class="Symbol">}</a> <a id="1971" class="Symbol">→</a>
  <a id="1975" href="foundation.equational-reasoning.html#1947" class="Bound">Y</a> <a id="1977" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="1979" href="foundation.equational-reasoning.html#1960" class="Bound">Z</a> <a id="1981" class="Symbol">→</a> <a id="1983" href="foundation.equational-reasoning.html#1935" class="Bound">X</a> <a id="1985" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="1987" href="foundation.equational-reasoning.html#1947" class="Bound">Y</a> <a id="1989" class="Symbol">→</a> <a id="1991" href="foundation.equational-reasoning.html#1935" class="Bound">X</a> <a id="1993" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="1995" href="foundation.equational-reasoning.html#1960" class="Bound">Z</a>
<a id="1997" href="foundation.equational-reasoning.html#1884" class="Function">step-equivalence-reasoning</a> <a id="2024" class="Symbol">_</a> <a id="2026" href="foundation.equational-reasoning.html#2026" class="Bound">g</a> <a id="2028" href="foundation.equational-reasoning.html#2028" class="Bound">f</a> <a id="2030" class="Symbol">=</a> <a id="2032" href="foundation.equational-reasoning.html#2026" class="Bound">g</a> <a id="2034" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a> <a id="2037" href="foundation.equational-reasoning.html#2028" class="Bound">f</a>

<a id="_∎e"></a><a id="2040" href="foundation.equational-reasoning.html#2040" class="Function Operator">_∎e</a> <a id="2044" class="Symbol">:</a> <a id="2046" class="Symbol">{</a><a id="2047" href="foundation.equational-reasoning.html#2047" class="Bound">l</a> <a id="2049" class="Symbol">:</a> <a id="2051" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2056" class="Symbol">}</a> <a id="2058" class="Symbol">(</a><a id="2059" href="foundation.equational-reasoning.html#2059" class="Bound">X</a> <a id="2061" class="Symbol">:</a> <a id="2063" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2066" href="foundation.equational-reasoning.html#2047" class="Bound">l</a><a id="2067" class="Symbol">)</a> <a id="2069" class="Symbol">→</a> <a id="2071" href="foundation.equational-reasoning.html#2059" class="Bound">X</a> <a id="2073" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2075" href="foundation.equational-reasoning.html#2059" class="Bound">X</a>
<a id="2077" href="foundation.equational-reasoning.html#2077" class="Bound">X</a> <a id="2079" href="foundation.equational-reasoning.html#2040" class="Function Operator">∎e</a> <a id="2082" class="Symbol">=</a> <a id="2084" href="foundation-core.equivalences.html#2494" class="Function">id-equiv</a>

<a id="2094" class="Keyword">syntax</a> <a id="2101" href="foundation.equational-reasoning.html#1884" class="Function">step-equivalence-reasoning</a> <a id="2128" class="Bound">X</a> <a id="2130" class="Bound">g</a> <a id="2132" class="Bound">f</a> <a id="2134" class="Symbol">=</a> <a id="2136" class="Bound">X</a> <a id="2138" class="Function">≃</a> <a id="2140" class="Function">by</a> <a id="2143" class="Bound">f</a> <a id="2145" class="Function">to</a> <a id="2148" class="Bound">g</a>
</pre>
### Equational reasoning for preorders

Note: In an equational reasoning argument, the preorder is always specified at the last step. So do we really need to specify it at each of the earlier steps?

<pre class="Agda"><a id="2363" class="Keyword">private</a>
  <a id="transitivity"></a><a id="2373" href="foundation.equational-reasoning.html#2373" class="Function">transitivity</a> <a id="2386" class="Symbol">:</a>
    <a id="2392" class="Symbol">{</a><a id="2393" href="foundation.equational-reasoning.html#2393" class="Bound">l1</a> <a id="2396" href="foundation.equational-reasoning.html#2396" class="Bound">l2</a> <a id="2399" class="Symbol">:</a> <a id="2401" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2406" class="Symbol">}</a> <a id="2408" class="Symbol">(</a><a id="2409" href="foundation.equational-reasoning.html#2409" class="Bound">X</a> <a id="2411" class="Symbol">:</a> <a id="2413" href="order-theory.preorders.html#531" class="Function">Preorder</a> <a id="2422" href="foundation.equational-reasoning.html#2393" class="Bound">l1</a> <a id="2425" href="foundation.equational-reasoning.html#2396" class="Bound">l2</a><a id="2427" class="Symbol">)</a>
    <a id="2433" class="Symbol">(</a><a id="2434" href="foundation.equational-reasoning.html#2434" class="Bound">x</a> <a id="2436" class="Symbol">:</a> <a id="2438" href="order-theory.preorders.html#873" class="Function">element-Preorder</a> <a id="2455" href="foundation.equational-reasoning.html#2409" class="Bound">X</a><a id="2456" class="Symbol">)</a> <a id="2458" class="Symbol">{</a><a id="2459" href="foundation.equational-reasoning.html#2459" class="Bound">y</a> <a id="2461" href="foundation.equational-reasoning.html#2461" class="Bound">z</a> <a id="2463" class="Symbol">:</a> <a id="2465" href="order-theory.preorders.html#873" class="Function">element-Preorder</a> <a id="2482" href="foundation.equational-reasoning.html#2409" class="Bound">X</a><a id="2483" class="Symbol">}</a> <a id="2485" class="Symbol">→</a>
    <a id="2491" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="2504" href="foundation.equational-reasoning.html#2409" class="Bound">X</a> <a id="2506" href="foundation.equational-reasoning.html#2434" class="Bound">x</a> <a id="2508" href="foundation.equational-reasoning.html#2459" class="Bound">y</a> <a id="2510" class="Symbol">→</a> <a id="2512" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="2525" href="foundation.equational-reasoning.html#2409" class="Bound">X</a> <a id="2527" href="foundation.equational-reasoning.html#2459" class="Bound">y</a> <a id="2529" href="foundation.equational-reasoning.html#2461" class="Bound">z</a> <a id="2531" class="Symbol">→</a> <a id="2533" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="2546" href="foundation.equational-reasoning.html#2409" class="Bound">X</a> <a id="2548" href="foundation.equational-reasoning.html#2434" class="Bound">x</a> <a id="2550" href="foundation.equational-reasoning.html#2461" class="Bound">z</a>
  <a id="2554" href="foundation.equational-reasoning.html#2373" class="Function">transitivity</a> <a id="2567" href="foundation.equational-reasoning.html#2567" class="Bound">X</a> <a id="2569" href="foundation.equational-reasoning.html#2569" class="Bound">x</a> <a id="2571" class="Symbol">{</a><a id="2572" href="foundation.equational-reasoning.html#2572" class="Bound">y</a><a id="2573" class="Symbol">}</a> <a id="2575" class="Symbol">{</a><a id="2576" href="foundation.equational-reasoning.html#2576" class="Bound">z</a><a id="2577" class="Symbol">}</a> <a id="2579" href="foundation.equational-reasoning.html#2579" class="Bound">u</a> <a id="2581" href="foundation.equational-reasoning.html#2581" class="Bound">v</a> <a id="2583" class="Symbol">=</a> <a id="2585" href="order-theory.preorders.html#1385" class="Function">transitive-leq-Preorder</a> <a id="2609" href="foundation.equational-reasoning.html#2567" class="Bound">X</a> <a id="2611" href="foundation.equational-reasoning.html#2569" class="Bound">x</a> <a id="2613" href="foundation.equational-reasoning.html#2572" class="Bound">y</a> <a id="2615" href="foundation.equational-reasoning.html#2576" class="Bound">z</a> <a id="2617" href="foundation.equational-reasoning.html#2581" class="Bound">v</a> <a id="2619" href="foundation.equational-reasoning.html#2579" class="Bound">u</a>

<a id="2622" class="Keyword">syntax</a> <a id="2629" href="foundation.equational-reasoning.html#2373" class="Function">transitivity</a> <a id="2642" class="Bound">X</a> <a id="2644" class="Bound">x</a> <a id="2646" class="Bound">u</a> <a id="2648" class="Bound">v</a> <a id="2650" class="Symbol">=</a> <a id="2652" class="Bound">x</a> <a id="2654" class="Function">≤</a> <a id="2656" class="Bound">X</a> <a id="2658" class="Function">by</a> <a id="2661" class="Bound">u</a> <a id="2663" class="Function">to</a> <a id="2666" class="Bound">v</a>
<a id="2668" class="Keyword">infixr</a> <a id="2675" class="Number">0</a> <a id="2677" href="foundation.equational-reasoning.html#2373" class="Function">transitivity</a>

<a id="2691" class="Keyword">private</a>
  <a id="reflexivity"></a><a id="2701" href="foundation.equational-reasoning.html#2701" class="Function">reflexivity</a> <a id="2713" class="Symbol">:</a>
    <a id="2719" class="Symbol">{</a><a id="2720" href="foundation.equational-reasoning.html#2720" class="Bound">l1</a> <a id="2723" href="foundation.equational-reasoning.html#2723" class="Bound">l2</a> <a id="2726" class="Symbol">:</a> <a id="2728" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2733" class="Symbol">}</a> <a id="2735" class="Symbol">(</a><a id="2736" href="foundation.equational-reasoning.html#2736" class="Bound">X</a> <a id="2738" class="Symbol">:</a> <a id="2740" href="order-theory.preorders.html#531" class="Function">Preorder</a> <a id="2749" href="foundation.equational-reasoning.html#2720" class="Bound">l1</a> <a id="2752" href="foundation.equational-reasoning.html#2723" class="Bound">l2</a><a id="2754" class="Symbol">)</a> <a id="2756" class="Symbol">(</a><a id="2757" href="foundation.equational-reasoning.html#2757" class="Bound">x</a> <a id="2759" class="Symbol">:</a> <a id="2761" href="order-theory.preorders.html#873" class="Function">element-Preorder</a> <a id="2778" href="foundation.equational-reasoning.html#2736" class="Bound">X</a><a id="2779" class="Symbol">)</a> <a id="2781" class="Symbol">→</a>
    <a id="2787" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="2800" href="foundation.equational-reasoning.html#2736" class="Bound">X</a> <a id="2802" href="foundation.equational-reasoning.html#2757" class="Bound">x</a> <a id="2804" href="foundation.equational-reasoning.html#2757" class="Bound">x</a>
  <a id="2808" href="foundation.equational-reasoning.html#2701" class="Function">reflexivity</a> <a id="2820" class="Symbol">=</a> <a id="2822" href="order-theory.preorders.html#1280" class="Function">refl-leq-Preorder</a>

<a id="2841" class="Keyword">syntax</a> <a id="2848" href="foundation.equational-reasoning.html#2701" class="Function">reflexivity</a> <a id="2860" class="Bound">X</a> <a id="2862" class="Bound">x</a> <a id="2864" class="Symbol">=</a> <a id="2866" class="Bound">x</a> <a id="2868" class="Function">∎</a> <a id="2870" class="Bound">X</a>
<a id="2872" class="Keyword">infix</a> <a id="2878" class="Number">1</a> <a id="2880" href="foundation.equational-reasoning.html#2701" class="Function">reflexivity</a>
</pre>
For a preorder `X` we thus write the chains as follows

```md
x ≤ X by ineq-1 to
y ≤ X by ineq-2 to
z ∎ X
```

## References

1. Martín Escardó. https://github.com/martinescardo/TypeTopology/blob/master/source/Id.lagda
2. Martín Escardó. https://github.com/martinescardo/TypeTopology/blob/master/source/UF-Equiv.lagda
3. The Agda standard library. https://github.com/agda/agda-stdlib/blob/master/src/Relation/Binary/PropositionalEquality/Core.agda
