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
X ≃⟨ equiv-1 ⟩
A ≃⟨ equiv-2 ⟩
B ≃⟨ equiv-3 ⟩
Y ∎
```

or
```md
x ≤⟨ ineq-1 ⟩
a ≤⟨ ineq-2 ⟩
b ≤⟨ ineq-3 ⟩
c ∎
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

<pre class="Agda"><a id="1458" class="Keyword">infix</a> <a id="1464" class="Number">1</a> <a id="1466" href="foundation.equational-reasoning.html#1810" class="Function Operator">_∎</a>
<a id="1469" class="Keyword">infixr</a> <a id="1476" class="Number">0</a> <a id="1478" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a> <a id="1504" href="foundation.equational-reasoning.html#1668" class="Function">step-equational-reasoning˘</a>

<a id="step-equational-reasoning"></a><a id="1532" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a> <a id="1558" class="Symbol">:</a>
  <a id="1562" class="Symbol">{</a><a id="1563" href="foundation.equational-reasoning.html#1563" class="Bound">l</a> <a id="1565" class="Symbol">:</a> <a id="1567" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1572" class="Symbol">}</a> <a id="1574" class="Symbol">{</a><a id="1575" href="foundation.equational-reasoning.html#1575" class="Bound">X</a> <a id="1577" class="Symbol">:</a> <a id="1579" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1582" href="foundation.equational-reasoning.html#1563" class="Bound">l</a><a id="1583" class="Symbol">}</a> <a id="1585" class="Symbol">(</a><a id="1586" href="foundation.equational-reasoning.html#1586" class="Bound">x</a> <a id="1588" class="Symbol">:</a> <a id="1590" href="foundation.equational-reasoning.html#1575" class="Bound">X</a><a id="1591" class="Symbol">)</a> <a id="1593" class="Symbol">{</a><a id="1594" href="foundation.equational-reasoning.html#1594" class="Bound">y</a> <a id="1596" href="foundation.equational-reasoning.html#1596" class="Bound">z</a> <a id="1598" class="Symbol">:</a> <a id="1600" href="foundation.equational-reasoning.html#1575" class="Bound">X</a><a id="1601" class="Symbol">}</a> <a id="1603" class="Symbol">→</a> <a id="1605" href="foundation.equational-reasoning.html#1594" class="Bound">y</a> <a id="1607" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1609" href="foundation.equational-reasoning.html#1596" class="Bound">z</a> <a id="1611" class="Symbol">→</a> <a id="1613" href="foundation.equational-reasoning.html#1586" class="Bound">x</a> <a id="1615" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1617" href="foundation.equational-reasoning.html#1594" class="Bound">y</a> <a id="1619" class="Symbol">→</a> <a id="1621" href="foundation.equational-reasoning.html#1586" class="Bound">x</a> <a id="1623" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1625" href="foundation.equational-reasoning.html#1596" class="Bound">z</a>
<a id="1627" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a> <a id="1653" class="Symbol">_</a> <a id="1655" href="foundation.equational-reasoning.html#1655" class="Bound">q</a> <a id="1657" href="foundation.equational-reasoning.html#1657" class="Bound">p</a> <a id="1659" class="Symbol">=</a> <a id="1661" href="foundation.equational-reasoning.html#1657" class="Bound">p</a> <a id="1663" href="foundation-core.identity-types.html#2425" class="Function Operator">∙</a> <a id="1665" href="foundation.equational-reasoning.html#1655" class="Bound">q</a>

<a id="step-equational-reasoning˘"></a><a id="1668" href="foundation.equational-reasoning.html#1668" class="Function">step-equational-reasoning˘</a> <a id="1695" class="Symbol">:</a>
  <a id="1699" class="Symbol">{</a><a id="1700" href="foundation.equational-reasoning.html#1700" class="Bound">l</a> <a id="1702" class="Symbol">:</a> <a id="1704" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1709" class="Symbol">}</a> <a id="1711" class="Symbol">{</a><a id="1712" href="foundation.equational-reasoning.html#1712" class="Bound">X</a> <a id="1714" class="Symbol">:</a> <a id="1716" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1719" href="foundation.equational-reasoning.html#1700" class="Bound">l</a><a id="1720" class="Symbol">}</a> <a id="1722" class="Symbol">(</a><a id="1723" href="foundation.equational-reasoning.html#1723" class="Bound">x</a> <a id="1725" class="Symbol">:</a> <a id="1727" href="foundation.equational-reasoning.html#1712" class="Bound">X</a><a id="1728" class="Symbol">)</a> <a id="1730" class="Symbol">{</a><a id="1731" href="foundation.equational-reasoning.html#1731" class="Bound">y</a> <a id="1733" href="foundation.equational-reasoning.html#1733" class="Bound">z</a> <a id="1735" class="Symbol">:</a> <a id="1737" href="foundation.equational-reasoning.html#1712" class="Bound">X</a><a id="1738" class="Symbol">}</a> <a id="1740" class="Symbol">→</a> <a id="1742" href="foundation.equational-reasoning.html#1731" class="Bound">y</a> <a id="1744" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1746" href="foundation.equational-reasoning.html#1733" class="Bound">z</a> <a id="1748" class="Symbol">→</a> <a id="1750" href="foundation.equational-reasoning.html#1731" class="Bound">y</a> <a id="1752" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1754" href="foundation.equational-reasoning.html#1723" class="Bound">x</a> <a id="1756" class="Symbol">→</a> <a id="1758" href="foundation.equational-reasoning.html#1723" class="Bound">x</a> <a id="1760" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1762" href="foundation.equational-reasoning.html#1733" class="Bound">z</a>
<a id="1764" href="foundation.equational-reasoning.html#1668" class="Function">step-equational-reasoning˘</a> <a id="1791" class="Symbol">_</a> <a id="1793" href="foundation.equational-reasoning.html#1793" class="Bound">q</a> <a id="1795" href="foundation.equational-reasoning.html#1795" class="Bound">p</a> <a id="1797" class="Symbol">=</a> <a id="1799" href="foundation-core.identity-types.html#2729" class="Function">inv</a> <a id="1803" href="foundation.equational-reasoning.html#1795" class="Bound">p</a> <a id="1805" href="foundation-core.identity-types.html#2425" class="Function Operator">∙</a> <a id="1807" href="foundation.equational-reasoning.html#1793" class="Bound">q</a>

<a id="_∎"></a><a id="1810" href="foundation.equational-reasoning.html#1810" class="Function Operator">_∎</a> <a id="1813" class="Symbol">:</a> <a id="1815" class="Symbol">{</a><a id="1816" href="foundation.equational-reasoning.html#1816" class="Bound">l</a> <a id="1818" class="Symbol">:</a> <a id="1820" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1825" class="Symbol">}</a> <a id="1827" class="Symbol">{</a><a id="1828" href="foundation.equational-reasoning.html#1828" class="Bound">X</a> <a id="1830" class="Symbol">:</a> <a id="1832" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1835" href="foundation.equational-reasoning.html#1816" class="Bound">l</a><a id="1836" class="Symbol">}</a> <a id="1838" class="Symbol">(</a><a id="1839" href="foundation.equational-reasoning.html#1839" class="Bound">x</a> <a id="1841" class="Symbol">:</a> <a id="1843" href="foundation.equational-reasoning.html#1828" class="Bound">X</a><a id="1844" class="Symbol">)</a> <a id="1846" class="Symbol">→</a> <a id="1848" href="foundation.equational-reasoning.html#1839" class="Bound">x</a> <a id="1850" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1852" href="foundation.equational-reasoning.html#1839" class="Bound">x</a>
<a id="1854" href="foundation.equational-reasoning.html#1854" class="Bound">x</a> <a id="1856" href="foundation.equational-reasoning.html#1810" class="Function Operator">∎</a> <a id="1858" class="Symbol">=</a> <a id="1860" href="foundation-core.identity-types.html#1820" class="InductiveConstructor">refl</a>

<a id="1866" class="Keyword">syntax</a> <a id="1873" href="foundation.equational-reasoning.html#1532" class="Function">step-equational-reasoning</a> <a id="1899" class="Bound">x</a> <a id="1901" class="Bound">q</a> <a id="1903" class="Bound">p</a> <a id="1905" class="Symbol">=</a> <a id="1907" class="Bound">x</a> <a id="1909" class="Function">=⟨</a> <a id="1912" class="Bound">p</a> <a id="1914" class="Function">⟩</a> <a id="1916" class="Bound">q</a>
<a id="1918" class="Keyword">syntax</a> <a id="1925" href="foundation.equational-reasoning.html#1668" class="Function">step-equational-reasoning˘</a> <a id="1952" class="Bound">x</a> <a id="1954" class="Bound">q</a> <a id="1956" class="Bound">p</a> <a id="1958" class="Symbol">=</a> <a id="1960" class="Bound">x</a> <a id="1962" class="Function">=˘⟨</a> <a id="1966" class="Bound">p</a> <a id="1968" class="Function">⟩</a> <a id="1970" class="Bound">q</a>
</pre>
### Equational reasoning for equivalences

<pre class="Agda"><a id="2028" class="Keyword">infix</a> <a id="2034" class="Number">1</a> <a id="2036" href="foundation.equational-reasoning.html#2429" class="Function Operator">_∎e</a>
<a id="2040" class="Keyword">infixr</a> <a id="2047" class="Number">0</a> <a id="2049" href="foundation.equational-reasoning.html#2105" class="Function">step-equivalence-reasoning</a> <a id="2076" href="foundation.equational-reasoning.html#2261" class="Function">step-equivalence-reasoning˘</a>

<a id="step-equivalence-reasoning"></a><a id="2105" href="foundation.equational-reasoning.html#2105" class="Function">step-equivalence-reasoning</a> <a id="2132" class="Symbol">:</a>
  <a id="2136" class="Symbol">{</a><a id="2137" href="foundation.equational-reasoning.html#2137" class="Bound">l1</a> <a id="2140" href="foundation.equational-reasoning.html#2140" class="Bound">l2</a> <a id="2143" href="foundation.equational-reasoning.html#2143" class="Bound">l3</a> <a id="2146" class="Symbol">:</a> <a id="2148" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2153" class="Symbol">}</a> <a id="2155" class="Symbol">(</a><a id="2156" href="foundation.equational-reasoning.html#2156" class="Bound">X</a> <a id="2158" class="Symbol">:</a> <a id="2160" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2163" href="foundation.equational-reasoning.html#2137" class="Bound">l1</a><a id="2165" class="Symbol">)</a> <a id="2167" class="Symbol">{</a><a id="2168" href="foundation.equational-reasoning.html#2168" class="Bound">Y</a> <a id="2170" class="Symbol">:</a> <a id="2172" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2175" href="foundation.equational-reasoning.html#2140" class="Bound">l2</a> <a id="2178" class="Symbol">}</a> <a id="2180" class="Symbol">{</a><a id="2181" href="foundation.equational-reasoning.html#2181" class="Bound">Z</a> <a id="2183" class="Symbol">:</a> <a id="2185" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2188" href="foundation.equational-reasoning.html#2143" class="Bound">l3</a><a id="2190" class="Symbol">}</a> <a id="2192" class="Symbol">→</a>
  <a id="2196" href="foundation.equational-reasoning.html#2168" class="Bound">Y</a> <a id="2198" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2200" href="foundation.equational-reasoning.html#2181" class="Bound">Z</a> <a id="2202" class="Symbol">→</a> <a id="2204" href="foundation.equational-reasoning.html#2156" class="Bound">X</a> <a id="2206" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2208" href="foundation.equational-reasoning.html#2168" class="Bound">Y</a> <a id="2210" class="Symbol">→</a> <a id="2212" href="foundation.equational-reasoning.html#2156" class="Bound">X</a> <a id="2214" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2216" href="foundation.equational-reasoning.html#2181" class="Bound">Z</a>
<a id="2218" href="foundation.equational-reasoning.html#2105" class="Function">step-equivalence-reasoning</a> <a id="2245" class="Symbol">_</a> <a id="2247" href="foundation.equational-reasoning.html#2247" class="Bound">g</a> <a id="2249" href="foundation.equational-reasoning.html#2249" class="Bound">f</a> <a id="2251" class="Symbol">=</a> <a id="2253" href="foundation.equational-reasoning.html#2247" class="Bound">g</a> <a id="2255" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a> <a id="2258" href="foundation.equational-reasoning.html#2249" class="Bound">f</a>

<a id="step-equivalence-reasoning˘"></a><a id="2261" href="foundation.equational-reasoning.html#2261" class="Function">step-equivalence-reasoning˘</a> <a id="2289" class="Symbol">:</a>
  <a id="2293" class="Symbol">{</a><a id="2294" href="foundation.equational-reasoning.html#2294" class="Bound">l1</a> <a id="2297" href="foundation.equational-reasoning.html#2297" class="Bound">l2</a> <a id="2300" href="foundation.equational-reasoning.html#2300" class="Bound">l3</a> <a id="2303" class="Symbol">:</a> <a id="2305" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2310" class="Symbol">}</a> <a id="2312" class="Symbol">(</a><a id="2313" href="foundation.equational-reasoning.html#2313" class="Bound">X</a> <a id="2315" class="Symbol">:</a> <a id="2317" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2320" href="foundation.equational-reasoning.html#2294" class="Bound">l1</a><a id="2322" class="Symbol">)</a> <a id="2324" class="Symbol">{</a><a id="2325" href="foundation.equational-reasoning.html#2325" class="Bound">Y</a> <a id="2327" class="Symbol">:</a> <a id="2329" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2332" href="foundation.equational-reasoning.html#2297" class="Bound">l2</a> <a id="2335" class="Symbol">}</a> <a id="2337" class="Symbol">{</a><a id="2338" href="foundation.equational-reasoning.html#2338" class="Bound">Z</a> <a id="2340" class="Symbol">:</a> <a id="2342" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2345" href="foundation.equational-reasoning.html#2300" class="Bound">l3</a><a id="2347" class="Symbol">}</a> <a id="2349" class="Symbol">→</a>
  <a id="2353" href="foundation.equational-reasoning.html#2325" class="Bound">Y</a> <a id="2355" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2357" href="foundation.equational-reasoning.html#2338" class="Bound">Z</a> <a id="2359" class="Symbol">→</a> <a id="2361" href="foundation.equational-reasoning.html#2325" class="Bound">Y</a> <a id="2363" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2365" href="foundation.equational-reasoning.html#2313" class="Bound">X</a> <a id="2367" class="Symbol">→</a> <a id="2369" href="foundation.equational-reasoning.html#2313" class="Bound">X</a> <a id="2371" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2373" href="foundation.equational-reasoning.html#2338" class="Bound">Z</a>
<a id="2375" href="foundation.equational-reasoning.html#2261" class="Function">step-equivalence-reasoning˘</a> <a id="2403" class="Symbol">_</a> <a id="2405" href="foundation.equational-reasoning.html#2405" class="Bound">g</a> <a id="2407" href="foundation.equational-reasoning.html#2407" class="Bound">f</a> <a id="2409" class="Symbol">=</a> <a id="2411" href="foundation.equational-reasoning.html#2405" class="Bound">g</a> <a id="2413" href="foundation-core.equivalences.html#7869" class="Function Operator">∘e</a> <a id="2416" href="foundation-core.equivalences.html#5721" class="Function">inv-equiv</a> <a id="2426" href="foundation.equational-reasoning.html#2407" class="Bound">f</a>

<a id="_∎e"></a><a id="2429" href="foundation.equational-reasoning.html#2429" class="Function Operator">_∎e</a> <a id="2433" class="Symbol">:</a> <a id="2435" class="Symbol">{</a><a id="2436" href="foundation.equational-reasoning.html#2436" class="Bound">l</a> <a id="2438" class="Symbol">:</a> <a id="2440" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2445" class="Symbol">}</a> <a id="2447" class="Symbol">(</a><a id="2448" href="foundation.equational-reasoning.html#2448" class="Bound">X</a> <a id="2450" class="Symbol">:</a> <a id="2452" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2455" href="foundation.equational-reasoning.html#2436" class="Bound">l</a><a id="2456" class="Symbol">)</a> <a id="2458" class="Symbol">→</a> <a id="2460" href="foundation.equational-reasoning.html#2448" class="Bound">X</a> <a id="2462" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2464" href="foundation.equational-reasoning.html#2448" class="Bound">X</a>
<a id="2466" href="foundation.equational-reasoning.html#2466" class="Bound">X</a> <a id="2468" href="foundation.equational-reasoning.html#2429" class="Function Operator">∎e</a> <a id="2471" class="Symbol">=</a> <a id="2473" href="foundation-core.equivalences.html#2494" class="Function">id-equiv</a>

<a id="2483" class="Keyword">syntax</a> <a id="2490" href="foundation.equational-reasoning.html#2105" class="Function">step-equivalence-reasoning</a> <a id="2517" class="Bound">X</a> <a id="2519" class="Bound">g</a> <a id="2521" class="Bound">f</a> <a id="2523" class="Symbol">=</a> <a id="2525" class="Bound">X</a> <a id="2527" class="Function">≃⟨</a> <a id="2530" class="Bound">f</a> <a id="2532" class="Function">⟩</a> <a id="2534" class="Bound">g</a>
<a id="2536" class="Keyword">syntax</a> <a id="2543" href="foundation.equational-reasoning.html#2261" class="Function">step-equivalence-reasoning˘</a> <a id="2571" class="Bound">X</a> <a id="2573" class="Bound">g</a> <a id="2575" class="Bound">f</a> <a id="2577" class="Symbol">=</a> <a id="2579" class="Bound">X</a> <a id="2581" class="Function">≃˘⟨</a> <a id="2585" class="Bound">f</a> <a id="2587" class="Function">⟩</a> <a id="2589" class="Bound">g</a>
</pre>
### Equational reasoning for preorders

<pre class="Agda"><a id="2644" class="Keyword">private</a>
  <a id="transitivity"></a><a id="2654" href="foundation.equational-reasoning.html#2654" class="Function">transitivity</a> <a id="2667" class="Symbol">:</a>
    <a id="2673" class="Symbol">{</a><a id="2674" href="foundation.equational-reasoning.html#2674" class="Bound">l1</a> <a id="2677" href="foundation.equational-reasoning.html#2677" class="Bound">l2</a> <a id="2680" class="Symbol">:</a> <a id="2682" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2687" class="Symbol">}</a> <a id="2689" class="Symbol">(</a><a id="2690" href="foundation.equational-reasoning.html#2690" class="Bound">X</a> <a id="2692" class="Symbol">:</a> <a id="2694" href="order-theory.preorders.html#531" class="Function">Preorder</a> <a id="2703" href="foundation.equational-reasoning.html#2674" class="Bound">l1</a> <a id="2706" href="foundation.equational-reasoning.html#2677" class="Bound">l2</a><a id="2708" class="Symbol">)</a>
    <a id="2714" class="Symbol">(</a><a id="2715" href="foundation.equational-reasoning.html#2715" class="Bound">x</a> <a id="2717" class="Symbol">:</a> <a id="2719" href="order-theory.preorders.html#873" class="Function">element-Preorder</a> <a id="2736" href="foundation.equational-reasoning.html#2690" class="Bound">X</a><a id="2737" class="Symbol">)</a> <a id="2739" class="Symbol">{</a><a id="2740" href="foundation.equational-reasoning.html#2740" class="Bound">y</a> <a id="2742" href="foundation.equational-reasoning.html#2742" class="Bound">z</a> <a id="2744" class="Symbol">:</a> <a id="2746" href="order-theory.preorders.html#873" class="Function">element-Preorder</a> <a id="2763" href="foundation.equational-reasoning.html#2690" class="Bound">X</a><a id="2764" class="Symbol">}</a> <a id="2766" class="Symbol">→</a>
    <a id="2772" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="2785" href="foundation.equational-reasoning.html#2690" class="Bound">X</a> <a id="2787" href="foundation.equational-reasoning.html#2715" class="Bound">x</a> <a id="2789" href="foundation.equational-reasoning.html#2740" class="Bound">y</a> <a id="2791" class="Symbol">→</a> <a id="2793" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="2806" href="foundation.equational-reasoning.html#2690" class="Bound">X</a> <a id="2808" href="foundation.equational-reasoning.html#2740" class="Bound">y</a> <a id="2810" href="foundation.equational-reasoning.html#2742" class="Bound">z</a> <a id="2812" class="Symbol">→</a> <a id="2814" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="2827" href="foundation.equational-reasoning.html#2690" class="Bound">X</a> <a id="2829" href="foundation.equational-reasoning.html#2715" class="Bound">x</a> <a id="2831" href="foundation.equational-reasoning.html#2742" class="Bound">z</a>
  <a id="2835" href="foundation.equational-reasoning.html#2654" class="Function">transitivity</a> <a id="2848" href="foundation.equational-reasoning.html#2848" class="Bound">X</a> <a id="2850" href="foundation.equational-reasoning.html#2850" class="Bound">x</a> <a id="2852" class="Symbol">{</a><a id="2853" href="foundation.equational-reasoning.html#2853" class="Bound">y</a><a id="2854" class="Symbol">}</a> <a id="2856" class="Symbol">{</a><a id="2857" href="foundation.equational-reasoning.html#2857" class="Bound">z</a><a id="2858" class="Symbol">}</a> <a id="2860" href="foundation.equational-reasoning.html#2860" class="Bound">u</a> <a id="2862" href="foundation.equational-reasoning.html#2862" class="Bound">v</a> <a id="2864" class="Symbol">=</a> <a id="2866" href="order-theory.preorders.html#1385" class="Function">transitive-leq-Preorder</a> <a id="2890" href="foundation.equational-reasoning.html#2848" class="Bound">X</a> <a id="2892" href="foundation.equational-reasoning.html#2850" class="Bound">x</a> <a id="2894" href="foundation.equational-reasoning.html#2853" class="Bound">y</a> <a id="2896" href="foundation.equational-reasoning.html#2857" class="Bound">z</a> <a id="2898" href="foundation.equational-reasoning.html#2862" class="Bound">v</a> <a id="2900" href="foundation.equational-reasoning.html#2860" class="Bound">u</a>

<a id="2903" class="Keyword">syntax</a> <a id="2910" href="foundation.equational-reasoning.html#2654" class="Function">transitivity</a> <a id="2923" class="Bound">X</a> <a id="2925" class="Bound">x</a> <a id="2927" class="Bound">u</a> <a id="2929" class="Bound">v</a> <a id="2931" class="Symbol">=</a> <a id="2933" class="Bound">x</a> <a id="2935" class="Function">≤[</a> <a id="2938" class="Bound">X</a> <a id="2940" class="Function">]⟨</a> <a id="2943" class="Bound">u</a> <a id="2945" class="Function">⟩</a> <a id="2947" class="Bound">v</a>
<a id="2949" class="Keyword">infixr</a> <a id="2956" class="Number">0</a> <a id="2958" href="foundation.equational-reasoning.html#2654" class="Function">transitivity</a>

<a id="2972" class="Keyword">private</a>
  <a id="reflexivity"></a><a id="2982" href="foundation.equational-reasoning.html#2982" class="Function">reflexivity</a> <a id="2994" class="Symbol">:</a>
    <a id="3000" class="Symbol">{</a><a id="3001" href="foundation.equational-reasoning.html#3001" class="Bound">l1</a> <a id="3004" href="foundation.equational-reasoning.html#3004" class="Bound">l2</a> <a id="3007" class="Symbol">:</a> <a id="3009" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3014" class="Symbol">}</a> <a id="3016" class="Symbol">(</a><a id="3017" href="foundation.equational-reasoning.html#3017" class="Bound">X</a> <a id="3019" class="Symbol">:</a> <a id="3021" href="order-theory.preorders.html#531" class="Function">Preorder</a> <a id="3030" href="foundation.equational-reasoning.html#3001" class="Bound">l1</a> <a id="3033" href="foundation.equational-reasoning.html#3004" class="Bound">l2</a><a id="3035" class="Symbol">)</a> <a id="3037" class="Symbol">(</a><a id="3038" href="foundation.equational-reasoning.html#3038" class="Bound">x</a> <a id="3040" class="Symbol">:</a> <a id="3042" href="order-theory.preorders.html#873" class="Function">element-Preorder</a> <a id="3059" href="foundation.equational-reasoning.html#3017" class="Bound">X</a><a id="3060" class="Symbol">)</a> <a id="3062" class="Symbol">→</a>
    <a id="3068" href="order-theory.preorders.html#1023" class="Function">leq-Preorder</a> <a id="3081" href="foundation.equational-reasoning.html#3017" class="Bound">X</a> <a id="3083" href="foundation.equational-reasoning.html#3038" class="Bound">x</a> <a id="3085" href="foundation.equational-reasoning.html#3038" class="Bound">x</a>
  <a id="3089" href="foundation.equational-reasoning.html#2982" class="Function">reflexivity</a> <a id="3101" class="Symbol">=</a> <a id="3103" href="order-theory.preorders.html#1280" class="Function">refl-leq-Preorder</a>

<a id="3122" class="Keyword">syntax</a> <a id="3129" href="foundation.equational-reasoning.html#2982" class="Function">reflexivity</a> <a id="3141" class="Bound">X</a> <a id="3143" class="Bound">x</a> <a id="3145" class="Symbol">=</a> <a id="3147" class="Bound">x</a> <a id="3149" class="Function">∎[</a> <a id="3152" class="Bound">X</a> <a id="3154" class="Function">]</a>
<a id="3156" class="Keyword">infix</a> <a id="3162" class="Number">1</a> <a id="3164" href="foundation.equational-reasoning.html#2982" class="Function">reflexivity</a>
</pre>
For a preorder `X` we thus write the chains as follows

```md
x ≤[ X ]⟨ ineq-1 ⟩
y ≤[ X ]⟨ ineq-2 ⟩
z ∎[ X ]
```

## References

1. Martín Escardó. https://github.com/martinescardo/TypeTopology/blob/master/source/Id.lagda
2. Martín Escardó. https://github.com/martinescardo/TypeTopology/blob/master/source/UF-Equiv.lagda
3. The Agda standard library. https://github.com/agda/agda-stdlib/blob/master/src/Relation/Binary/PropositionalEquality/Core.agda