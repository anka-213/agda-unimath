# The universal property of truncations

<pre class="Agda"><a id="50" class="Symbol">{-#</a> <a id="54" class="Keyword">OPTIONS</a> <a id="62" class="Pragma">--without-K</a> <a id="74" class="Pragma">--exact-split</a> <a id="88" class="Symbol">#-}</a>

<a id="93" class="Keyword">module</a> <a id="100" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a> <a id="141" class="Keyword">where</a>

<a id="148" class="Keyword">open</a> <a id="153" class="Keyword">import</a> <a id="160" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a> <a id="189" class="Keyword">using</a>
  <a id="197" class="Symbol">(</a> <a id="199" href="foundation-core.contractible-maps.html#2368" class="Function">is-equiv-is-contr-map</a><a id="220" class="Symbol">;</a> <a id="222" href="foundation-core.contractible-maps.html#3850" class="Function">is-contr-map-is-equiv</a><a id="243" class="Symbol">)</a>
<a id="245" class="Keyword">open</a> <a id="250" class="Keyword">import</a> <a id="257" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a> <a id="287" class="Keyword">using</a>
  <a id="295" class="Symbol">(</a> <a id="297" href="foundation-core.contractible-types.html#925" class="Function">is-contr</a><a id="305" class="Symbol">;</a> <a id="307" href="foundation-core.contractible-types.html#3230" class="Function">is-contr-equiv</a><a id="321" class="Symbol">;</a> <a id="323" href="foundation-core.contractible-types.html#3739" class="Function">is-contr-equiv&#39;</a><a id="338" class="Symbol">;</a> <a id="340" href="foundation-core.contractible-types.html#1018" class="Function">center</a><a id="346" class="Symbol">)</a>
<a id="348" class="Keyword">open</a> <a id="353" class="Keyword">import</a> <a id="360" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="392" class="Keyword">using</a> <a id="398" class="Symbol">(</a><a id="399" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="400" class="Symbol">;</a> <a id="402" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="406" class="Symbol">;</a> <a id="408" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="411" class="Symbol">;</a> <a id="413" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="416" class="Symbol">;</a> <a id="418" href="foundation-core.dependent-pair-types.html#687" class="Function">ind-Σ</a><a id="423" class="Symbol">)</a>
<a id="425" class="Keyword">open</a> <a id="430" class="Keyword">import</a>
  <a id="439" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a> <a id="509" class="Keyword">using</a>
  <a id="517" class="Symbol">(</a> <a id="519" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="539" class="Symbol">;</a> <a id="541" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#2808" class="Function">map-distributive-Π-Σ</a><a id="561" class="Symbol">)</a>
<a id="563" class="Keyword">open</a> <a id="568" class="Keyword">import</a> <a id="575" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="599" class="Keyword">using</a>
  <a id="607" class="Symbol">(</a> <a id="609" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a><a id="617" class="Symbol">;</a> <a id="619" href="foundation-core.equivalences.html#12773" class="Function">is-equiv-equiv</a><a id="633" class="Symbol">;</a> <a id="635" href="foundation-core.equivalences.html#4173" class="Function">map-inv-is-equiv</a><a id="651" class="Symbol">;</a> <a id="653" href="foundation.equivalences.html#9061" class="Function">is-equiv-precomp-is-equiv</a><a id="678" class="Symbol">;</a>
    <a id="684" href="foundation-core.equivalences.html#2309" class="Function">is-equiv-id</a><a id="695" class="Symbol">;</a> <a id="697" href="foundation-core.equivalences.html#1607" class="Function Operator">_≃_</a><a id="700" class="Symbol">;</a> <a id="702" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a><a id="711" class="Symbol">;</a> <a id="713" href="foundation-core.equivalences.html#1862" class="Function">is-equiv-map-equiv</a><a id="731" class="Symbol">)</a>
<a id="733" class="Keyword">open</a> <a id="738" class="Keyword">import</a> <a id="745" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a> <a id="780" class="Keyword">using</a> <a id="786" class="Symbol">(</a><a id="787" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="799" class="Symbol">)</a>
<a id="801" class="Keyword">open</a> <a id="806" class="Keyword">import</a> <a id="813" href="foundation.functions.html" class="Module">foundation.functions</a> <a id="834" class="Keyword">using</a> <a id="840" class="Symbol">(</a><a id="841" href="foundation-core.functions.html#925" class="Function">precomp</a><a id="848" class="Symbol">;</a> <a id="850" href="foundation-core.functions.html#407" class="Function Operator">_∘_</a><a id="853" class="Symbol">;</a> <a id="855" href="foundation-core.functions.html#309" class="Function">id</a><a id="857" class="Symbol">)</a>
<a id="859" class="Keyword">open</a> <a id="864" class="Keyword">import</a> <a id="871" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a> <a id="917" class="Keyword">using</a>
  <a id="925" class="Symbol">(</a> <a id="927" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a><a id="936" class="Symbol">;</a> <a id="938" href="foundation-core.functoriality-dependent-pair-types.html#10750" class="Function">is-fiberwise-equiv-is-equiv-map-Σ</a><a id="971" class="Symbol">)</a>
<a id="973" class="Keyword">open</a> <a id="978" class="Keyword">import</a> <a id="985" href="foundation.homotopies.html" class="Module">foundation.homotopies</a> <a id="1007" class="Keyword">using</a> <a id="1013" class="Symbol">(</a><a id="1014" href="foundation-core.homotopies.html#467" class="Function Operator">_~_</a><a id="1017" class="Symbol">)</a>
<a id="1019" class="Keyword">open</a> <a id="1024" class="Keyword">import</a> <a id="1031" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="1057" class="Keyword">using</a> <a id="1063" class="Symbol">(</a><a id="1064" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="1066" class="Symbol">;</a> <a id="1068" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="1072" class="Symbol">;</a> <a id="1074" href="foundation-core.identity-types.html#1552" class="Function">inv</a><a id="1077" class="Symbol">)</a>
<a id="1079" class="Keyword">open</a> <a id="1084" class="Keyword">import</a> <a id="1091" href="foundation.sections.html" class="Module">foundation.sections</a> <a id="1111" class="Keyword">using</a> <a id="1117" class="Symbol">(</a><a id="1118" href="foundation-core.sections.html#521" class="Function">sec</a><a id="1121" class="Symbol">)</a>
<a id="1123" class="Keyword">open</a> <a id="1128" class="Keyword">import</a> <a id="1135" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a> <a id="1162" class="Keyword">using</a>
  <a id="1170" class="Symbol">(</a> <a id="1172" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a><a id="1186" class="Symbol">;</a> <a id="1188" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a><a id="1207" class="Symbol">;</a> <a id="1209" href="foundation.truncated-types.html#3483" class="Function">type-hom-Truncated-Type</a><a id="1232" class="Symbol">;</a>
    <a id="1238" href="foundation-core.truncated-types.html#6022" class="Function">Σ-Truncated-Type</a><a id="1254" class="Symbol">;</a> <a id="1256" href="foundation-core.truncated-types.html#6396" class="Function">fib-Truncated-Type</a><a id="1274" class="Symbol">;</a> <a id="1276" href="foundation-core.truncated-types.html#1466" class="Function">is-trunc</a><a id="1284" class="Symbol">)</a>
<a id="1286" class="Keyword">open</a> <a id="1291" class="Keyword">import</a> <a id="1298" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a> <a id="1332" class="Keyword">using</a> <a id="1338" class="Symbol">(</a><a id="1339" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="1340" class="Symbol">)</a>
<a id="1342" class="Keyword">open</a> <a id="1347" class="Keyword">import</a> <a id="1354" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="1381" class="Keyword">using</a> <a id="1387" class="Symbol">(</a><a id="1388" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="1390" class="Symbol">;</a> <a id="1392" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1397" class="Symbol">;</a> <a id="1399" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="1402" class="Symbol">;</a> <a id="1404" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="1408" class="Symbol">)</a>
</pre>
## Idea

We say that a map `f : A → B` into a `k`-truncated type `B` is a `k`-truncation of `A` -- or that it satisfies the universal property of the `k`-truncation of `A` -- if any map `g : A → C` into a `k`-truncated type `C` extends uniquely along `f` to a map `B → C`.

## Definition

### The condition on a map to be a truncation

<pre class="Agda"><a id="precomp-Trunc"></a><a id="1759" href="foundation.universal-property-truncation.html#1759" class="Function">precomp-Trunc</a> <a id="1773" class="Symbol">:</a>
  <a id="1777" class="Symbol">{</a><a id="1778" href="foundation.universal-property-truncation.html#1778" class="Bound">l1</a> <a id="1781" href="foundation.universal-property-truncation.html#1781" class="Bound">l2</a> <a id="1784" href="foundation.universal-property-truncation.html#1784" class="Bound">l3</a> <a id="1787" class="Symbol">:</a> <a id="1789" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1794" class="Symbol">}</a> <a id="1796" class="Symbol">{</a><a id="1797" href="foundation.universal-property-truncation.html#1797" class="Bound">k</a> <a id="1799" class="Symbol">:</a> <a id="1801" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="1802" class="Symbol">}</a> <a id="1804" class="Symbol">{</a><a id="1805" href="foundation.universal-property-truncation.html#1805" class="Bound">A</a> <a id="1807" class="Symbol">:</a> <a id="1809" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1812" href="foundation.universal-property-truncation.html#1778" class="Bound">l1</a><a id="1814" class="Symbol">}</a> <a id="1816" class="Symbol">{</a><a id="1817" href="foundation.universal-property-truncation.html#1817" class="Bound">B</a> <a id="1819" class="Symbol">:</a> <a id="1821" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1824" href="foundation.universal-property-truncation.html#1781" class="Bound">l2</a><a id="1826" class="Symbol">}</a> <a id="1828" class="Symbol">(</a><a id="1829" href="foundation.universal-property-truncation.html#1829" class="Bound">f</a> <a id="1831" class="Symbol">:</a> <a id="1833" href="foundation.universal-property-truncation.html#1805" class="Bound">A</a> <a id="1835" class="Symbol">→</a> <a id="1837" href="foundation.universal-property-truncation.html#1817" class="Bound">B</a><a id="1838" class="Symbol">)</a>
  <a id="1842" class="Symbol">(</a><a id="1843" href="foundation.universal-property-truncation.html#1843" class="Bound">C</a> <a id="1845" class="Symbol">:</a> <a id="1847" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="1862" href="foundation.universal-property-truncation.html#1784" class="Bound">l3</a> <a id="1865" href="foundation.universal-property-truncation.html#1797" class="Bound">k</a><a id="1866" class="Symbol">)</a> <a id="1868" class="Symbol">→</a>
  <a id="1872" class="Symbol">(</a><a id="1873" href="foundation.universal-property-truncation.html#1817" class="Bound">B</a> <a id="1875" class="Symbol">→</a> <a id="1877" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="1897" href="foundation.universal-property-truncation.html#1843" class="Bound">C</a><a id="1898" class="Symbol">)</a> <a id="1900" class="Symbol">→</a> <a id="1902" class="Symbol">(</a><a id="1903" href="foundation.universal-property-truncation.html#1805" class="Bound">A</a> <a id="1905" class="Symbol">→</a> <a id="1907" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="1927" href="foundation.universal-property-truncation.html#1843" class="Bound">C</a><a id="1928" class="Symbol">)</a>
<a id="1930" href="foundation.universal-property-truncation.html#1759" class="Function">precomp-Trunc</a> <a id="1944" href="foundation.universal-property-truncation.html#1944" class="Bound">f</a> <a id="1946" href="foundation.universal-property-truncation.html#1946" class="Bound">C</a> <a id="1948" class="Symbol">=</a> <a id="1950" href="foundation-core.functions.html#925" class="Function">precomp</a> <a id="1958" href="foundation.universal-property-truncation.html#1944" class="Bound">f</a> <a id="1960" class="Symbol">(</a><a id="1961" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="1981" href="foundation.universal-property-truncation.html#1946" class="Bound">C</a><a id="1982" class="Symbol">)</a>

<a id="is-truncation"></a><a id="1985" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="1999" class="Symbol">:</a>
  <a id="2003" class="Symbol">{</a><a id="2004" href="foundation.universal-property-truncation.html#2004" class="Bound">l1</a> <a id="2007" href="foundation.universal-property-truncation.html#2007" class="Bound">l2</a> <a id="2010" class="Symbol">:</a> <a id="2012" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2017" class="Symbol">}</a> <a id="2019" class="Symbol">(</a><a id="2020" href="foundation.universal-property-truncation.html#2020" class="Bound">l</a> <a id="2022" class="Symbol">:</a> <a id="2024" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2029" class="Symbol">)</a> <a id="2031" class="Symbol">{</a><a id="2032" href="foundation.universal-property-truncation.html#2032" class="Bound">k</a> <a id="2034" class="Symbol">:</a> <a id="2036" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="2037" class="Symbol">}</a> <a id="2039" class="Symbol">{</a><a id="2040" href="foundation.universal-property-truncation.html#2040" class="Bound">A</a> <a id="2042" class="Symbol">:</a> <a id="2044" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2047" href="foundation.universal-property-truncation.html#2004" class="Bound">l1</a><a id="2049" class="Symbol">}</a>
  <a id="2053" class="Symbol">(</a><a id="2054" href="foundation.universal-property-truncation.html#2054" class="Bound">B</a> <a id="2056" class="Symbol">:</a> <a id="2058" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="2073" href="foundation.universal-property-truncation.html#2007" class="Bound">l2</a> <a id="2076" href="foundation.universal-property-truncation.html#2032" class="Bound">k</a><a id="2077" class="Symbol">)</a> <a id="2079" class="Symbol">→</a> <a id="2081" class="Symbol">(</a><a id="2082" href="foundation.universal-property-truncation.html#2040" class="Bound">A</a> <a id="2084" class="Symbol">→</a> <a id="2086" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="2106" href="foundation.universal-property-truncation.html#2054" class="Bound">B</a><a id="2107" class="Symbol">)</a> <a id="2109" class="Symbol">→</a>
  <a id="2113" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2116" class="Symbol">(</a><a id="2117" href="foundation.universal-property-truncation.html#2004" class="Bound">l1</a> <a id="2120" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2122" href="foundation.universal-property-truncation.html#2007" class="Bound">l2</a> <a id="2125" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2127" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="2132" href="foundation.universal-property-truncation.html#2020" class="Bound">l</a><a id="2133" class="Symbol">)</a>
<a id="2135" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="2149" href="foundation.universal-property-truncation.html#2149" class="Bound">l</a> <a id="2151" class="Symbol">{</a><a id="2152" href="foundation.universal-property-truncation.html#2152" class="Bound">k</a><a id="2153" class="Symbol">}</a> <a id="2155" href="foundation.universal-property-truncation.html#2155" class="Bound">B</a> <a id="2157" href="foundation.universal-property-truncation.html#2157" class="Bound">f</a> <a id="2159" class="Symbol">=</a>
  <a id="2163" class="Symbol">(</a><a id="2164" href="foundation.universal-property-truncation.html#2164" class="Bound">C</a> <a id="2166" class="Symbol">:</a> <a id="2168" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="2183" href="foundation.universal-property-truncation.html#2149" class="Bound">l</a> <a id="2185" href="foundation.universal-property-truncation.html#2152" class="Bound">k</a><a id="2186" class="Symbol">)</a> <a id="2188" class="Symbol">→</a> <a id="2190" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="2199" class="Symbol">(</a><a id="2200" href="foundation.universal-property-truncation.html#1759" class="Function">precomp-Trunc</a> <a id="2214" href="foundation.universal-property-truncation.html#2157" class="Bound">f</a> <a id="2216" href="foundation.universal-property-truncation.html#2164" class="Bound">C</a><a id="2217" class="Symbol">)</a>
</pre>
### The universal property of truncations

<pre class="Agda"><a id="universal-property-truncation"></a><a id="2275" href="foundation.universal-property-truncation.html#2275" class="Function">universal-property-truncation</a> <a id="2305" class="Symbol">:</a>
  <a id="2309" class="Symbol">(</a><a id="2310" href="foundation.universal-property-truncation.html#2310" class="Bound">l</a> <a id="2312" class="Symbol">:</a> <a id="2314" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2319" class="Symbol">)</a> <a id="2321" class="Symbol">{</a><a id="2322" href="foundation.universal-property-truncation.html#2322" class="Bound">l1</a> <a id="2325" href="foundation.universal-property-truncation.html#2325" class="Bound">l2</a> <a id="2328" class="Symbol">:</a> <a id="2330" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2335" class="Symbol">}</a> <a id="2337" class="Symbol">{</a><a id="2338" href="foundation.universal-property-truncation.html#2338" class="Bound">k</a> <a id="2340" class="Symbol">:</a> <a id="2342" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="2343" class="Symbol">}</a> <a id="2345" class="Symbol">{</a><a id="2346" href="foundation.universal-property-truncation.html#2346" class="Bound">A</a> <a id="2348" class="Symbol">:</a> <a id="2350" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2353" href="foundation.universal-property-truncation.html#2322" class="Bound">l1</a><a id="2355" class="Symbol">}</a>
  <a id="2359" class="Symbol">(</a><a id="2360" href="foundation.universal-property-truncation.html#2360" class="Bound">B</a> <a id="2362" class="Symbol">:</a> <a id="2364" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="2379" href="foundation.universal-property-truncation.html#2325" class="Bound">l2</a> <a id="2382" href="foundation.universal-property-truncation.html#2338" class="Bound">k</a><a id="2383" class="Symbol">)</a> <a id="2385" class="Symbol">(</a><a id="2386" href="foundation.universal-property-truncation.html#2386" class="Bound">f</a> <a id="2388" class="Symbol">:</a> <a id="2390" href="foundation.universal-property-truncation.html#2346" class="Bound">A</a> <a id="2392" class="Symbol">→</a> <a id="2394" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="2414" href="foundation.universal-property-truncation.html#2360" class="Bound">B</a><a id="2415" class="Symbol">)</a> <a id="2417" class="Symbol">→</a>
  <a id="2421" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2424" class="Symbol">(</a><a id="2425" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="2430" href="foundation.universal-property-truncation.html#2310" class="Bound">l</a> <a id="2432" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2434" href="foundation.universal-property-truncation.html#2322" class="Bound">l1</a> <a id="2437" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2439" href="foundation.universal-property-truncation.html#2325" class="Bound">l2</a><a id="2441" class="Symbol">)</a>
<a id="2443" href="foundation.universal-property-truncation.html#2275" class="Function">universal-property-truncation</a> <a id="2473" href="foundation.universal-property-truncation.html#2473" class="Bound">l</a> <a id="2475" class="Symbol">{</a><a id="2476" class="Argument">k</a> <a id="2478" class="Symbol">=</a> <a id="2480" href="foundation.universal-property-truncation.html#2480" class="Bound">k</a><a id="2481" class="Symbol">}</a> <a id="2483" class="Symbol">{</a><a id="2484" href="foundation.universal-property-truncation.html#2484" class="Bound">A</a><a id="2485" class="Symbol">}</a> <a id="2487" href="foundation.universal-property-truncation.html#2487" class="Bound">B</a> <a id="2489" href="foundation.universal-property-truncation.html#2489" class="Bound">f</a> <a id="2491" class="Symbol">=</a>
  <a id="2495" class="Symbol">(</a><a id="2496" href="foundation.universal-property-truncation.html#2496" class="Bound">C</a> <a id="2498" class="Symbol">:</a> <a id="2500" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="2515" href="foundation.universal-property-truncation.html#2473" class="Bound">l</a> <a id="2517" href="foundation.universal-property-truncation.html#2480" class="Bound">k</a><a id="2518" class="Symbol">)</a> <a id="2520" class="Symbol">(</a><a id="2521" href="foundation.universal-property-truncation.html#2521" class="Bound">g</a> <a id="2523" class="Symbol">:</a> <a id="2525" href="foundation.universal-property-truncation.html#2484" class="Bound">A</a> <a id="2527" class="Symbol">→</a> <a id="2529" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="2549" href="foundation.universal-property-truncation.html#2496" class="Bound">C</a><a id="2550" class="Symbol">)</a> <a id="2552" class="Symbol">→</a>
  <a id="2556" href="foundation-core.contractible-types.html#925" class="Function">is-contr</a> <a id="2565" class="Symbol">(</a><a id="2566" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="2568" class="Symbol">(</a><a id="2569" href="foundation.truncated-types.html#3483" class="Function">type-hom-Truncated-Type</a> <a id="2593" href="foundation.universal-property-truncation.html#2480" class="Bound">k</a> <a id="2595" href="foundation.universal-property-truncation.html#2487" class="Bound">B</a> <a id="2597" href="foundation.universal-property-truncation.html#2496" class="Bound">C</a><a id="2598" class="Symbol">)</a> <a id="2600" class="Symbol">(λ</a> <a id="2603" href="foundation.universal-property-truncation.html#2603" class="Bound">h</a> <a id="2605" class="Symbol">→</a> <a id="2607" class="Symbol">(</a><a id="2608" href="foundation.universal-property-truncation.html#2603" class="Bound">h</a> <a id="2610" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="2612" href="foundation.universal-property-truncation.html#2489" class="Bound">f</a><a id="2613" class="Symbol">)</a> <a id="2615" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="2617" href="foundation.universal-property-truncation.html#2521" class="Bound">g</a><a id="2618" class="Symbol">))</a>
</pre>
### The dependent universal property of truncations

<pre class="Agda"><a id="precomp-Π-Truncated-Type"></a><a id="2683" href="foundation.universal-property-truncation.html#2683" class="Function">precomp-Π-Truncated-Type</a> <a id="2708" class="Symbol">:</a>
  <a id="2712" class="Symbol">{</a><a id="2713" href="foundation.universal-property-truncation.html#2713" class="Bound">l1</a> <a id="2716" href="foundation.universal-property-truncation.html#2716" class="Bound">l2</a> <a id="2719" href="foundation.universal-property-truncation.html#2719" class="Bound">l3</a> <a id="2722" class="Symbol">:</a> <a id="2724" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2729" class="Symbol">}</a> <a id="2731" class="Symbol">{</a><a id="2732" href="foundation.universal-property-truncation.html#2732" class="Bound">k</a> <a id="2734" class="Symbol">:</a> <a id="2736" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="2737" class="Symbol">}</a> <a id="2739" class="Symbol">{</a><a id="2740" href="foundation.universal-property-truncation.html#2740" class="Bound">A</a> <a id="2742" class="Symbol">:</a> <a id="2744" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2747" href="foundation.universal-property-truncation.html#2713" class="Bound">l1</a><a id="2749" class="Symbol">}</a> <a id="2751" class="Symbol">{</a><a id="2752" href="foundation.universal-property-truncation.html#2752" class="Bound">B</a> <a id="2754" class="Symbol">:</a> <a id="2756" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2759" href="foundation.universal-property-truncation.html#2716" class="Bound">l2</a><a id="2761" class="Symbol">}</a> <a id="2763" class="Symbol">(</a><a id="2764" href="foundation.universal-property-truncation.html#2764" class="Bound">f</a> <a id="2766" class="Symbol">:</a> <a id="2768" href="foundation.universal-property-truncation.html#2740" class="Bound">A</a> <a id="2770" class="Symbol">→</a> <a id="2772" href="foundation.universal-property-truncation.html#2752" class="Bound">B</a><a id="2773" class="Symbol">)</a>
  <a id="2777" class="Symbol">(</a><a id="2778" href="foundation.universal-property-truncation.html#2778" class="Bound">C</a> <a id="2780" class="Symbol">:</a> <a id="2782" href="foundation.universal-property-truncation.html#2752" class="Bound">B</a> <a id="2784" class="Symbol">→</a> <a id="2786" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="2801" href="foundation.universal-property-truncation.html#2719" class="Bound">l3</a> <a id="2804" href="foundation.universal-property-truncation.html#2732" class="Bound">k</a><a id="2805" class="Symbol">)</a> <a id="2807" class="Symbol">→</a>
  <a id="2811" class="Symbol">((</a><a id="2813" href="foundation.universal-property-truncation.html#2813" class="Bound">b</a> <a id="2815" class="Symbol">:</a> <a id="2817" href="foundation.universal-property-truncation.html#2752" class="Bound">B</a><a id="2818" class="Symbol">)</a> <a id="2820" class="Symbol">→</a> <a id="2822" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="2842" class="Symbol">(</a><a id="2843" href="foundation.universal-property-truncation.html#2778" class="Bound">C</a> <a id="2845" href="foundation.universal-property-truncation.html#2813" class="Bound">b</a><a id="2846" class="Symbol">))</a> <a id="2849" class="Symbol">→</a>
  <a id="2853" class="Symbol">((</a><a id="2855" href="foundation.universal-property-truncation.html#2855" class="Bound">a</a> <a id="2857" class="Symbol">:</a> <a id="2859" href="foundation.universal-property-truncation.html#2740" class="Bound">A</a><a id="2860" class="Symbol">)</a> <a id="2862" class="Symbol">→</a> <a id="2864" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="2884" class="Symbol">(</a><a id="2885" href="foundation.universal-property-truncation.html#2778" class="Bound">C</a> <a id="2887" class="Symbol">(</a><a id="2888" href="foundation.universal-property-truncation.html#2764" class="Bound">f</a> <a id="2890" href="foundation.universal-property-truncation.html#2855" class="Bound">a</a><a id="2891" class="Symbol">)))</a>
<a id="2895" href="foundation.universal-property-truncation.html#2683" class="Function">precomp-Π-Truncated-Type</a> <a id="2920" href="foundation.universal-property-truncation.html#2920" class="Bound">f</a> <a id="2922" href="foundation.universal-property-truncation.html#2922" class="Bound">C</a> <a id="2924" href="foundation.universal-property-truncation.html#2924" class="Bound">h</a> <a id="2926" href="foundation.universal-property-truncation.html#2926" class="Bound">a</a> <a id="2928" class="Symbol">=</a> <a id="2930" href="foundation.universal-property-truncation.html#2924" class="Bound">h</a> <a id="2932" class="Symbol">(</a><a id="2933" href="foundation.universal-property-truncation.html#2920" class="Bound">f</a> <a id="2935" href="foundation.universal-property-truncation.html#2926" class="Bound">a</a><a id="2936" class="Symbol">)</a>

<a id="dependent-universal-property-truncation"></a><a id="2939" href="foundation.universal-property-truncation.html#2939" class="Function">dependent-universal-property-truncation</a> <a id="2979" class="Symbol">:</a>
  <a id="2983" class="Symbol">{</a><a id="2984" href="foundation.universal-property-truncation.html#2984" class="Bound">l1</a> <a id="2987" href="foundation.universal-property-truncation.html#2987" class="Bound">l2</a> <a id="2990" class="Symbol">:</a> <a id="2992" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2997" class="Symbol">}</a> <a id="2999" class="Symbol">(</a><a id="3000" href="foundation.universal-property-truncation.html#3000" class="Bound">l</a> <a id="3002" class="Symbol">:</a> <a id="3004" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3009" class="Symbol">)</a> <a id="3011" class="Symbol">{</a><a id="3012" href="foundation.universal-property-truncation.html#3012" class="Bound">k</a> <a id="3014" class="Symbol">:</a> <a id="3016" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3017" class="Symbol">}</a> <a id="3019" class="Symbol">{</a><a id="3020" href="foundation.universal-property-truncation.html#3020" class="Bound">A</a> <a id="3022" class="Symbol">:</a> <a id="3024" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3027" href="foundation.universal-property-truncation.html#2984" class="Bound">l1</a><a id="3029" class="Symbol">}</a> <a id="3031" class="Symbol">(</a><a id="3032" href="foundation.universal-property-truncation.html#3032" class="Bound">B</a> <a id="3034" class="Symbol">:</a> <a id="3036" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="3051" href="foundation.universal-property-truncation.html#2987" class="Bound">l2</a> <a id="3054" href="foundation.universal-property-truncation.html#3012" class="Bound">k</a><a id="3055" class="Symbol">)</a>
  <a id="3059" class="Symbol">(</a><a id="3060" href="foundation.universal-property-truncation.html#3060" class="Bound">f</a> <a id="3062" class="Symbol">:</a> <a id="3064" href="foundation.universal-property-truncation.html#3020" class="Bound">A</a> <a id="3066" class="Symbol">→</a> <a id="3068" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="3088" href="foundation.universal-property-truncation.html#3032" class="Bound">B</a><a id="3089" class="Symbol">)</a> <a id="3091" class="Symbol">→</a> <a id="3093" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3096" class="Symbol">(</a><a id="3097" href="foundation.universal-property-truncation.html#2984" class="Bound">l1</a> <a id="3100" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3102" href="foundation.universal-property-truncation.html#2987" class="Bound">l2</a> <a id="3105" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3107" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="3112" href="foundation.universal-property-truncation.html#3000" class="Bound">l</a><a id="3113" class="Symbol">)</a>
<a id="3115" href="foundation.universal-property-truncation.html#2939" class="Function">dependent-universal-property-truncation</a> <a id="3155" href="foundation.universal-property-truncation.html#3155" class="Bound">l</a> <a id="3157" class="Symbol">{</a><a id="3158" href="foundation.universal-property-truncation.html#3158" class="Bound">k</a><a id="3159" class="Symbol">}</a> <a id="3161" href="foundation.universal-property-truncation.html#3161" class="Bound">B</a> <a id="3163" href="foundation.universal-property-truncation.html#3163" class="Bound">f</a> <a id="3165" class="Symbol">=</a>
  <a id="3169" class="Symbol">(</a><a id="3170" href="foundation.universal-property-truncation.html#3170" class="Bound">X</a> <a id="3172" class="Symbol">:</a> <a id="3174" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="3194" href="foundation.universal-property-truncation.html#3161" class="Bound">B</a> <a id="3196" class="Symbol">→</a> <a id="3198" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="3213" href="foundation.universal-property-truncation.html#3155" class="Bound">l</a> <a id="3215" href="foundation.universal-property-truncation.html#3158" class="Bound">k</a><a id="3216" class="Symbol">)</a> <a id="3218" class="Symbol">→</a>
  <a id="3222" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="3231" class="Symbol">(</a><a id="3232" href="foundation.universal-property-truncation.html#2683" class="Function">precomp-Π-Truncated-Type</a> <a id="3257" href="foundation.universal-property-truncation.html#3163" class="Bound">f</a> <a id="3259" href="foundation.universal-property-truncation.html#3170" class="Bound">X</a><a id="3260" class="Symbol">)</a>
</pre>
## Properties

### Equivalences into `k`-truncated types are truncations

<pre class="Agda"><a id="3349" class="Keyword">abstract</a>
  <a id="is-truncation-id"></a><a id="3360" href="foundation.universal-property-truncation.html#3360" class="Function">is-truncation-id</a> <a id="3377" class="Symbol">:</a>
    <a id="3383" class="Symbol">{</a><a id="3384" href="foundation.universal-property-truncation.html#3384" class="Bound">l1</a> <a id="3387" class="Symbol">:</a> <a id="3389" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3394" class="Symbol">}</a> <a id="3396" class="Symbol">{</a><a id="3397" href="foundation.universal-property-truncation.html#3397" class="Bound">k</a> <a id="3399" class="Symbol">:</a> <a id="3401" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3402" class="Symbol">}</a> <a id="3404" class="Symbol">{</a><a id="3405" href="foundation.universal-property-truncation.html#3405" class="Bound">A</a> <a id="3407" class="Symbol">:</a> <a id="3409" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3412" href="foundation.universal-property-truncation.html#3384" class="Bound">l1</a><a id="3414" class="Symbol">}</a> <a id="3416" class="Symbol">(</a><a id="3417" href="foundation.universal-property-truncation.html#3417" class="Bound">H</a> <a id="3419" class="Symbol">:</a> <a id="3421" href="foundation-core.truncated-types.html#1466" class="Function">is-trunc</a> <a id="3430" href="foundation.universal-property-truncation.html#3397" class="Bound">k</a> <a id="3432" href="foundation.universal-property-truncation.html#3405" class="Bound">A</a><a id="3433" class="Symbol">)</a> <a id="3435" class="Symbol">→</a>
    <a id="3441" class="Symbol">{</a><a id="3442" href="foundation.universal-property-truncation.html#3442" class="Bound">l</a> <a id="3444" class="Symbol">:</a> <a id="3446" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3451" class="Symbol">}</a> <a id="3453" class="Symbol">→</a> <a id="3455" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="3469" href="foundation.universal-property-truncation.html#3442" class="Bound">l</a> <a id="3471" class="Symbol">(</a><a id="3472" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="3477" href="foundation.universal-property-truncation.html#3405" class="Bound">A</a> <a id="3479" href="foundation.universal-property-truncation.html#3417" class="Bound">H</a><a id="3480" class="Symbol">)</a> <a id="3482" href="foundation-core.functions.html#309" class="Function">id</a>
  <a id="3487" href="foundation.universal-property-truncation.html#3360" class="Function">is-truncation-id</a> <a id="3504" href="foundation.universal-property-truncation.html#3504" class="Bound">H</a> <a id="3506" href="foundation.universal-property-truncation.html#3506" class="Bound">B</a> <a id="3508" class="Symbol">=</a>
    <a id="3514" href="foundation.equivalences.html#9061" class="Function">is-equiv-precomp-is-equiv</a> <a id="3540" href="foundation-core.functions.html#309" class="Function">id</a> <a id="3543" href="foundation-core.equivalences.html#2309" class="Function">is-equiv-id</a> <a id="3555" class="Symbol">(</a><a id="3556" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="3576" href="foundation.universal-property-truncation.html#3506" class="Bound">B</a><a id="3577" class="Symbol">)</a>

<a id="3580" class="Keyword">abstract</a>
  <a id="is-truncation-equiv"></a><a id="3591" href="foundation.universal-property-truncation.html#3591" class="Function">is-truncation-equiv</a> <a id="3611" class="Symbol">:</a>
    <a id="3617" class="Symbol">{</a><a id="3618" href="foundation.universal-property-truncation.html#3618" class="Bound">l1</a> <a id="3621" href="foundation.universal-property-truncation.html#3621" class="Bound">l2</a> <a id="3624" class="Symbol">:</a> <a id="3626" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3631" class="Symbol">}</a> <a id="3633" class="Symbol">{</a><a id="3634" href="foundation.universal-property-truncation.html#3634" class="Bound">k</a> <a id="3636" class="Symbol">:</a> <a id="3638" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3639" class="Symbol">}</a> <a id="3641" class="Symbol">{</a><a id="3642" href="foundation.universal-property-truncation.html#3642" class="Bound">A</a> <a id="3644" class="Symbol">:</a> <a id="3646" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3649" href="foundation.universal-property-truncation.html#3618" class="Bound">l1</a><a id="3651" class="Symbol">}</a> <a id="3653" class="Symbol">(</a><a id="3654" href="foundation.universal-property-truncation.html#3654" class="Bound">B</a> <a id="3656" class="Symbol">:</a> <a id="3658" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="3673" href="foundation.universal-property-truncation.html#3621" class="Bound">l2</a> <a id="3676" href="foundation.universal-property-truncation.html#3634" class="Bound">k</a><a id="3677" class="Symbol">)</a>
    <a id="3683" class="Symbol">(</a><a id="3684" href="foundation.universal-property-truncation.html#3684" class="Bound">e</a> <a id="3686" class="Symbol">:</a> <a id="3688" href="foundation.universal-property-truncation.html#3642" class="Bound">A</a> <a id="3690" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="3692" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="3712" href="foundation.universal-property-truncation.html#3654" class="Bound">B</a><a id="3713" class="Symbol">)</a> <a id="3715" class="Symbol">→</a>
    <a id="3721" class="Symbol">{</a><a id="3722" href="foundation.universal-property-truncation.html#3722" class="Bound">l</a> <a id="3724" class="Symbol">:</a> <a id="3726" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3731" class="Symbol">}</a> <a id="3733" class="Symbol">→</a> <a id="3735" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="3749" href="foundation.universal-property-truncation.html#3722" class="Bound">l</a> <a id="3751" href="foundation.universal-property-truncation.html#3654" class="Bound">B</a> <a id="3753" class="Symbol">(</a><a id="3754" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a> <a id="3764" href="foundation.universal-property-truncation.html#3684" class="Bound">e</a><a id="3765" class="Symbol">)</a>
  <a id="3769" href="foundation.universal-property-truncation.html#3591" class="Function">is-truncation-equiv</a> <a id="3789" href="foundation.universal-property-truncation.html#3789" class="Bound">B</a> <a id="3791" href="foundation.universal-property-truncation.html#3791" class="Bound">e</a> <a id="3793" href="foundation.universal-property-truncation.html#3793" class="Bound">C</a> <a id="3795" class="Symbol">=</a>
    <a id="3801" href="foundation.equivalences.html#9061" class="Function">is-equiv-precomp-is-equiv</a>
      <a id="3833" class="Symbol">(</a> <a id="3835" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a> <a id="3845" href="foundation.universal-property-truncation.html#3791" class="Bound">e</a><a id="3846" class="Symbol">)</a>
      <a id="3854" class="Symbol">(</a> <a id="3856" href="foundation-core.equivalences.html#1862" class="Function">is-equiv-map-equiv</a> <a id="3875" href="foundation.universal-property-truncation.html#3791" class="Bound">e</a><a id="3876" class="Symbol">)</a>
      <a id="3884" class="Symbol">(</a> <a id="3886" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="3906" href="foundation.universal-property-truncation.html#3793" class="Bound">C</a><a id="3907" class="Symbol">)</a>
</pre>
### A map into a truncated type is a truncation if and only if it satisfies the universal property of the truncation

<pre class="Agda"><a id="4040" class="Keyword">module</a> <a id="4047" href="foundation.universal-property-truncation.html#4047" class="Module">_</a>
  <a id="4051" class="Symbol">{</a><a id="4052" href="foundation.universal-property-truncation.html#4052" class="Bound">l1</a> <a id="4055" href="foundation.universal-property-truncation.html#4055" class="Bound">l2</a> <a id="4058" class="Symbol">:</a> <a id="4060" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4065" class="Symbol">}</a> <a id="4067" class="Symbol">{</a><a id="4068" href="foundation.universal-property-truncation.html#4068" class="Bound">k</a> <a id="4070" class="Symbol">:</a> <a id="4072" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="4073" class="Symbol">}</a> <a id="4075" class="Symbol">{</a><a id="4076" href="foundation.universal-property-truncation.html#4076" class="Bound">A</a> <a id="4078" class="Symbol">:</a> <a id="4080" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="4083" href="foundation.universal-property-truncation.html#4052" class="Bound">l1</a><a id="4085" class="Symbol">}</a> <a id="4087" class="Symbol">(</a><a id="4088" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="4090" class="Symbol">:</a> <a id="4092" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="4107" href="foundation.universal-property-truncation.html#4055" class="Bound">l2</a> <a id="4110" href="foundation.universal-property-truncation.html#4068" class="Bound">k</a><a id="4111" class="Symbol">)</a>
  <a id="4115" class="Symbol">(</a><a id="4116" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a> <a id="4118" class="Symbol">:</a> <a id="4120" href="foundation.universal-property-truncation.html#4076" class="Bound">A</a> <a id="4122" class="Symbol">→</a> <a id="4124" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="4144" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a><a id="4145" class="Symbol">)</a>
  <a id="4149" class="Keyword">where</a>

  <a id="4158" class="Keyword">abstract</a>
    <a id="4171" href="foundation.universal-property-truncation.html#4171" class="Function">is-truncation-universal-property-truncation</a> <a id="4215" class="Symbol">:</a>
      <a id="4223" class="Symbol">({</a><a id="4225" href="foundation.universal-property-truncation.html#4225" class="Bound">l</a> <a id="4227" class="Symbol">:</a> <a id="4229" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4234" class="Symbol">}</a> <a id="4236" class="Symbol">→</a> <a id="4238" href="foundation.universal-property-truncation.html#2275" class="Function">universal-property-truncation</a> <a id="4268" href="foundation.universal-property-truncation.html#4225" class="Bound">l</a> <a id="4270" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="4272" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="4273" class="Symbol">)</a> <a id="4275" class="Symbol">→</a>
      <a id="4283" class="Symbol">({</a><a id="4285" href="foundation.universal-property-truncation.html#4285" class="Bound">l</a> <a id="4287" class="Symbol">:</a> <a id="4289" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4294" class="Symbol">}</a> <a id="4296" class="Symbol">→</a> <a id="4298" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="4312" href="foundation.universal-property-truncation.html#4285" class="Bound">l</a> <a id="4314" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="4316" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="4317" class="Symbol">)</a>
    <a id="4323" href="foundation.universal-property-truncation.html#4171" class="Function">is-truncation-universal-property-truncation</a> <a id="4367" href="foundation.universal-property-truncation.html#4367" class="Bound">H</a> <a id="4369" href="foundation.universal-property-truncation.html#4369" class="Bound">C</a> <a id="4371" class="Symbol">=</a>
      <a id="4379" href="foundation-core.contractible-maps.html#2368" class="Function">is-equiv-is-contr-map</a>
        <a id="4409" class="Symbol">(</a> <a id="4411" class="Symbol">λ</a> <a id="4413" href="foundation.universal-property-truncation.html#4413" class="Bound">g</a> <a id="4415" class="Symbol">→</a>
          <a id="4427" href="foundation-core.contractible-types.html#3230" class="Function">is-contr-equiv</a>
            <a id="4454" class="Symbol">(</a> <a id="4456" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="4458" class="Symbol">(</a><a id="4459" href="foundation.truncated-types.html#3483" class="Function">type-hom-Truncated-Type</a> <a id="4483" href="foundation.universal-property-truncation.html#4068" class="Bound">k</a> <a id="4485" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="4487" href="foundation.universal-property-truncation.html#4369" class="Bound">C</a><a id="4488" class="Symbol">)</a> <a id="4490" class="Symbol">(λ</a> <a id="4493" href="foundation.universal-property-truncation.html#4493" class="Bound">h</a> <a id="4495" class="Symbol">→</a> <a id="4497" class="Symbol">(</a><a id="4498" href="foundation.universal-property-truncation.html#4493" class="Bound">h</a> <a id="4500" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="4502" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="4503" class="Symbol">)</a> <a id="4505" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="4507" href="foundation.universal-property-truncation.html#4413" class="Bound">g</a><a id="4508" class="Symbol">))</a>
            <a id="4523" class="Symbol">(</a> <a id="4525" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a> <a id="4535" class="Symbol">(λ</a> <a id="4538" href="foundation.universal-property-truncation.html#4538" class="Bound">h</a> <a id="4540" class="Symbol">→</a> <a id="4542" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="4554" class="Symbol">))</a>
            <a id="4569" class="Symbol">(</a> <a id="4571" href="foundation.universal-property-truncation.html#4367" class="Bound">H</a> <a id="4573" href="foundation.universal-property-truncation.html#4369" class="Bound">C</a> <a id="4575" href="foundation.universal-property-truncation.html#4413" class="Bound">g</a><a id="4576" class="Symbol">))</a>

  <a id="4582" class="Keyword">abstract</a>
    <a id="4595" href="foundation.universal-property-truncation.html#4595" class="Function">universal-property-truncation-is-truncation</a> <a id="4639" class="Symbol">:</a>
      <a id="4647" class="Symbol">({</a><a id="4649" href="foundation.universal-property-truncation.html#4649" class="Bound">l</a> <a id="4651" class="Symbol">:</a> <a id="4653" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4658" class="Symbol">}</a> <a id="4660" class="Symbol">→</a> <a id="4662" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="4676" href="foundation.universal-property-truncation.html#4649" class="Bound">l</a> <a id="4678" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="4680" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="4681" class="Symbol">)</a> <a id="4683" class="Symbol">→</a>
      <a id="4691" class="Symbol">({</a><a id="4693" href="foundation.universal-property-truncation.html#4693" class="Bound">l</a> <a id="4695" class="Symbol">:</a> <a id="4697" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4702" class="Symbol">}</a> <a id="4704" class="Symbol">→</a> <a id="4706" href="foundation.universal-property-truncation.html#2275" class="Function">universal-property-truncation</a> <a id="4736" href="foundation.universal-property-truncation.html#4693" class="Bound">l</a> <a id="4738" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="4740" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="4741" class="Symbol">)</a>
    <a id="4747" href="foundation.universal-property-truncation.html#4595" class="Function">universal-property-truncation-is-truncation</a> <a id="4791" href="foundation.universal-property-truncation.html#4791" class="Bound">H</a> <a id="4793" href="foundation.universal-property-truncation.html#4793" class="Bound">C</a> <a id="4795" href="foundation.universal-property-truncation.html#4795" class="Bound">g</a> <a id="4797" class="Symbol">=</a>
      <a id="4805" href="foundation-core.contractible-types.html#3739" class="Function">is-contr-equiv&#39;</a>
        <a id="4829" class="Symbol">(</a> <a id="4831" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="4833" class="Symbol">(</a><a id="4834" href="foundation.truncated-types.html#3483" class="Function">type-hom-Truncated-Type</a> <a id="4858" href="foundation.universal-property-truncation.html#4068" class="Bound">k</a> <a id="4860" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="4862" href="foundation.universal-property-truncation.html#4793" class="Bound">C</a><a id="4863" class="Symbol">)</a> <a id="4865" class="Symbol">(λ</a> <a id="4868" href="foundation.universal-property-truncation.html#4868" class="Bound">h</a> <a id="4870" class="Symbol">→</a> <a id="4872" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="4875" class="Symbol">(</a><a id="4876" href="foundation.universal-property-truncation.html#4868" class="Bound">h</a> <a id="4878" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="4880" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="4881" class="Symbol">)</a> <a id="4883" href="foundation.universal-property-truncation.html#4795" class="Bound">g</a><a id="4884" class="Symbol">))</a>
        <a id="4895" class="Symbol">(</a> <a id="4897" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a> <a id="4907" class="Symbol">(λ</a> <a id="4910" href="foundation.universal-property-truncation.html#4910" class="Bound">h</a> <a id="4912" class="Symbol">→</a> <a id="4914" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="4926" class="Symbol">))</a>
        <a id="4937" class="Symbol">(</a> <a id="4939" href="foundation-core.contractible-maps.html#3850" class="Function">is-contr-map-is-equiv</a> <a id="4961" class="Symbol">(</a><a id="4962" href="foundation.universal-property-truncation.html#4791" class="Bound">H</a> <a id="4964" href="foundation.universal-property-truncation.html#4793" class="Bound">C</a><a id="4965" class="Symbol">)</a> <a id="4967" href="foundation.universal-property-truncation.html#4795" class="Bound">g</a><a id="4968" class="Symbol">)</a>

  <a id="4973" href="foundation.universal-property-truncation.html#4973" class="Function">map-is-truncation</a> <a id="4991" class="Symbol">:</a>
    <a id="4997" class="Symbol">({</a><a id="4999" href="foundation.universal-property-truncation.html#4999" class="Bound">l</a> <a id="5001" class="Symbol">:</a> <a id="5003" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5008" class="Symbol">}</a> <a id="5010" class="Symbol">→</a> <a id="5012" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="5026" href="foundation.universal-property-truncation.html#4999" class="Bound">l</a> <a id="5028" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="5030" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="5031" class="Symbol">)</a> <a id="5033" class="Symbol">→</a>
    <a id="5039" class="Symbol">({</a><a id="5041" href="foundation.universal-property-truncation.html#5041" class="Bound">l</a> <a id="5043" class="Symbol">:</a> <a id="5045" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5050" class="Symbol">}</a> <a id="5052" class="Symbol">(</a><a id="5053" href="foundation.universal-property-truncation.html#5053" class="Bound">C</a> <a id="5055" class="Symbol">:</a> <a id="5057" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="5072" href="foundation.universal-property-truncation.html#5041" class="Bound">l</a> <a id="5074" href="foundation.universal-property-truncation.html#4068" class="Bound">k</a><a id="5075" class="Symbol">)</a> <a id="5077" class="Symbol">(</a><a id="5078" href="foundation.universal-property-truncation.html#5078" class="Bound">g</a> <a id="5080" class="Symbol">:</a> <a id="5082" href="foundation.universal-property-truncation.html#4076" class="Bound">A</a> <a id="5084" class="Symbol">→</a> <a id="5086" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="5106" href="foundation.universal-property-truncation.html#5053" class="Bound">C</a><a id="5107" class="Symbol">)</a> <a id="5109" class="Symbol">→</a>
    <a id="5115" href="foundation.truncated-types.html#3483" class="Function">type-hom-Truncated-Type</a> <a id="5139" href="foundation.universal-property-truncation.html#4068" class="Bound">k</a> <a id="5141" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="5143" href="foundation.universal-property-truncation.html#5053" class="Bound">C</a><a id="5144" class="Symbol">)</a>
  <a id="5148" href="foundation.universal-property-truncation.html#4973" class="Function">map-is-truncation</a> <a id="5166" href="foundation.universal-property-truncation.html#5166" class="Bound">H</a> <a id="5168" href="foundation.universal-property-truncation.html#5168" class="Bound">C</a> <a id="5170" href="foundation.universal-property-truncation.html#5170" class="Bound">g</a> <a id="5172" class="Symbol">=</a>
    <a id="5178" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="5182" class="Symbol">(</a><a id="5183" href="foundation-core.contractible-types.html#1018" class="Function">center</a> <a id="5190" class="Symbol">(</a><a id="5191" href="foundation.universal-property-truncation.html#4595" class="Function">universal-property-truncation-is-truncation</a> <a id="5235" href="foundation.universal-property-truncation.html#5166" class="Bound">H</a> <a id="5237" href="foundation.universal-property-truncation.html#5168" class="Bound">C</a> <a id="5239" href="foundation.universal-property-truncation.html#5170" class="Bound">g</a><a id="5240" class="Symbol">))</a>

  <a id="5246" href="foundation.universal-property-truncation.html#5246" class="Function">triangle-is-truncation</a> <a id="5269" class="Symbol">:</a>
    <a id="5275" class="Symbol">(</a><a id="5276" href="foundation.universal-property-truncation.html#5276" class="Bound">H</a> <a id="5278" class="Symbol">:</a> <a id="5280" class="Symbol">{</a><a id="5281" href="foundation.universal-property-truncation.html#5281" class="Bound">l</a> <a id="5283" class="Symbol">:</a> <a id="5285" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5290" class="Symbol">}</a> <a id="5292" class="Symbol">→</a> <a id="5294" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="5308" href="foundation.universal-property-truncation.html#5281" class="Bound">l</a> <a id="5310" href="foundation.universal-property-truncation.html#4088" class="Bound">B</a> <a id="5312" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="5313" class="Symbol">)</a> <a id="5315" class="Symbol">→</a>
    <a id="5321" class="Symbol">{</a><a id="5322" href="foundation.universal-property-truncation.html#5322" class="Bound">l</a> <a id="5324" class="Symbol">:</a> <a id="5326" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5331" class="Symbol">}</a> <a id="5333" class="Symbol">(</a><a id="5334" href="foundation.universal-property-truncation.html#5334" class="Bound">C</a> <a id="5336" class="Symbol">:</a> <a id="5338" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="5353" href="foundation.universal-property-truncation.html#5322" class="Bound">l</a> <a id="5355" href="foundation.universal-property-truncation.html#4068" class="Bound">k</a><a id="5356" class="Symbol">)</a> <a id="5358" class="Symbol">(</a><a id="5359" href="foundation.universal-property-truncation.html#5359" class="Bound">g</a> <a id="5361" class="Symbol">:</a> <a id="5363" href="foundation.universal-property-truncation.html#4076" class="Bound">A</a> <a id="5365" class="Symbol">→</a> <a id="5367" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="5387" href="foundation.universal-property-truncation.html#5334" class="Bound">C</a><a id="5388" class="Symbol">)</a> <a id="5390" class="Symbol">→</a>
    <a id="5396" class="Symbol">(</a><a id="5397" href="foundation.universal-property-truncation.html#4973" class="Function">map-is-truncation</a> <a id="5415" href="foundation.universal-property-truncation.html#5276" class="Bound">H</a> <a id="5417" href="foundation.universal-property-truncation.html#5334" class="Bound">C</a> <a id="5419" href="foundation.universal-property-truncation.html#5359" class="Bound">g</a> <a id="5421" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="5423" href="foundation.universal-property-truncation.html#4116" class="Bound">f</a><a id="5424" class="Symbol">)</a> <a id="5426" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="5428" href="foundation.universal-property-truncation.html#5359" class="Bound">g</a>
  <a id="5432" href="foundation.universal-property-truncation.html#5246" class="Function">triangle-is-truncation</a> <a id="5455" href="foundation.universal-property-truncation.html#5455" class="Bound">H</a> <a id="5457" href="foundation.universal-property-truncation.html#5457" class="Bound">C</a> <a id="5459" href="foundation.universal-property-truncation.html#5459" class="Bound">g</a> <a id="5461" class="Symbol">=</a>
    <a id="5467" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="5471" class="Symbol">(</a><a id="5472" href="foundation-core.contractible-types.html#1018" class="Function">center</a> <a id="5479" class="Symbol">(</a><a id="5480" href="foundation.universal-property-truncation.html#4595" class="Function">universal-property-truncation-is-truncation</a> <a id="5524" href="foundation.universal-property-truncation.html#5455" class="Bound">H</a> <a id="5526" href="foundation.universal-property-truncation.html#5457" class="Bound">C</a> <a id="5528" href="foundation.universal-property-truncation.html#5459" class="Bound">g</a><a id="5529" class="Symbol">))</a>
</pre>
### A map into a truncated type is a truncation if and only if it satisfies the dependent universal property of the truncation

<pre class="Agda"><a id="5673" class="Keyword">module</a> <a id="5680" href="foundation.universal-property-truncation.html#5680" class="Module">_</a>
  <a id="5684" class="Symbol">{</a><a id="5685" href="foundation.universal-property-truncation.html#5685" class="Bound">l1</a> <a id="5688" href="foundation.universal-property-truncation.html#5688" class="Bound">l2</a> <a id="5691" class="Symbol">:</a> <a id="5693" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5698" class="Symbol">}</a> <a id="5700" class="Symbol">{</a><a id="5701" href="foundation.universal-property-truncation.html#5701" class="Bound">k</a> <a id="5703" class="Symbol">:</a> <a id="5705" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="5706" class="Symbol">}</a> <a id="5708" class="Symbol">{</a><a id="5709" href="foundation.universal-property-truncation.html#5709" class="Bound">A</a> <a id="5711" class="Symbol">:</a> <a id="5713" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="5716" href="foundation.universal-property-truncation.html#5685" class="Bound">l1</a><a id="5718" class="Symbol">}</a> <a id="5720" class="Symbol">(</a><a id="5721" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="5723" class="Symbol">:</a> <a id="5725" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="5740" href="foundation.universal-property-truncation.html#5688" class="Bound">l2</a> <a id="5743" href="foundation.universal-property-truncation.html#5701" class="Bound">k</a><a id="5744" class="Symbol">)</a>
  <a id="5748" class="Symbol">(</a><a id="5749" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a> <a id="5751" class="Symbol">:</a> <a id="5753" href="foundation.universal-property-truncation.html#5709" class="Bound">A</a> <a id="5755" class="Symbol">→</a> <a id="5757" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="5777" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a><a id="5778" class="Symbol">)</a>
  <a id="5782" class="Keyword">where</a>

  <a id="5791" class="Keyword">abstract</a>
    <a id="5804" href="foundation.universal-property-truncation.html#5804" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="5858" class="Symbol">:</a>
      <a id="5866" class="Symbol">({</a><a id="5868" href="foundation.universal-property-truncation.html#5868" class="Bound">l</a> <a id="5870" class="Symbol">:</a> <a id="5872" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5877" class="Symbol">}</a> <a id="5879" class="Symbol">→</a> <a id="5881" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="5895" href="foundation.universal-property-truncation.html#5868" class="Bound">l</a> <a id="5897" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="5899" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a><a id="5900" class="Symbol">)</a> <a id="5902" class="Symbol">→</a>
      <a id="5910" class="Symbol">{</a><a id="5911" href="foundation.universal-property-truncation.html#5911" class="Bound">l</a> <a id="5913" class="Symbol">:</a> <a id="5915" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5920" class="Symbol">}</a> <a id="5922" class="Symbol">→</a> <a id="5924" href="foundation.universal-property-truncation.html#2939" class="Function">dependent-universal-property-truncation</a> <a id="5964" href="foundation.universal-property-truncation.html#5911" class="Bound">l</a> <a id="5966" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="5968" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a>
    <a id="5974" href="foundation.universal-property-truncation.html#5804" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="6028" href="foundation.universal-property-truncation.html#6028" class="Bound">H</a> <a id="6030" href="foundation.universal-property-truncation.html#6030" class="Bound">X</a> <a id="6032" class="Symbol">=</a>
      <a id="6040" href="foundation-core.functoriality-dependent-pair-types.html#10750" class="Function">is-fiberwise-equiv-is-equiv-map-Σ</a>
        <a id="6082" class="Symbol">(</a> <a id="6084" class="Symbol">λ</a> <a id="6086" class="Symbol">(</a><a id="6087" href="foundation.universal-property-truncation.html#6087" class="Bound">h</a> <a id="6089" class="Symbol">:</a> <a id="6091" href="foundation.universal-property-truncation.html#5709" class="Bound">A</a> <a id="6093" class="Symbol">→</a> <a id="6095" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="6115" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a><a id="6116" class="Symbol">)</a> <a id="6118" class="Symbol">→</a>
          <a id="6130" class="Symbol">(</a><a id="6131" href="foundation.universal-property-truncation.html#6131" class="Bound">a</a> <a id="6133" class="Symbol">:</a> <a id="6135" href="foundation.universal-property-truncation.html#5709" class="Bound">A</a><a id="6136" class="Symbol">)</a> <a id="6138" class="Symbol">→</a> <a id="6140" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="6160" class="Symbol">(</a><a id="6161" href="foundation.universal-property-truncation.html#6030" class="Bound">X</a> <a id="6163" class="Symbol">(</a><a id="6164" href="foundation.universal-property-truncation.html#6087" class="Bound">h</a> <a id="6166" href="foundation.universal-property-truncation.html#6131" class="Bound">a</a><a id="6167" class="Symbol">)))</a>
        <a id="6179" class="Symbol">(</a> <a id="6181" class="Symbol">λ</a> <a id="6183" class="Symbol">(</a><a id="6184" href="foundation.universal-property-truncation.html#6184" class="Bound">g</a> <a id="6186" class="Symbol">:</a> <a id="6188" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="6208" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="6210" class="Symbol">→</a> <a id="6212" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="6232" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a><a id="6233" class="Symbol">)</a> <a id="6235" class="Symbol">→</a> <a id="6237" href="foundation.universal-property-truncation.html#6184" class="Bound">g</a> <a id="6239" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="6241" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a><a id="6242" class="Symbol">)</a>
        <a id="6252" class="Symbol">(</a> <a id="6254" class="Symbol">λ</a> <a id="6256" href="foundation.universal-property-truncation.html#6256" class="Bound">g</a> <a id="6258" class="Symbol">(</a><a id="6259" href="foundation.universal-property-truncation.html#6259" class="Bound">s</a> <a id="6261" class="Symbol">:</a> <a id="6263" class="Symbol">(</a><a id="6264" href="foundation.universal-property-truncation.html#6264" class="Bound">b</a> <a id="6266" class="Symbol">:</a> <a id="6268" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="6288" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a><a id="6289" class="Symbol">)</a> <a id="6291" class="Symbol">→</a>
          <a id="6303" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="6323" class="Symbol">(</a><a id="6324" href="foundation.universal-property-truncation.html#6030" class="Bound">X</a> <a id="6326" class="Symbol">(</a><a id="6327" href="foundation.universal-property-truncation.html#6256" class="Bound">g</a> <a id="6329" href="foundation.universal-property-truncation.html#6264" class="Bound">b</a><a id="6330" class="Symbol">)))</a> <a id="6334" class="Symbol">(</a><a id="6335" href="foundation.universal-property-truncation.html#6335" class="Bound">a</a> <a id="6337" class="Symbol">:</a> <a id="6339" href="foundation.universal-property-truncation.html#5709" class="Bound">A</a><a id="6340" class="Symbol">)</a> <a id="6342" class="Symbol">→</a> <a id="6344" href="foundation.universal-property-truncation.html#6259" class="Bound">s</a> <a id="6346" class="Symbol">(</a><a id="6347" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a> <a id="6349" href="foundation.universal-property-truncation.html#6335" class="Bound">a</a><a id="6350" class="Symbol">))</a>
        <a id="6361" class="Symbol">(</a> <a id="6363" href="foundation.universal-property-truncation.html#6028" class="Bound">H</a> <a id="6365" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a><a id="6366" class="Symbol">)</a>
        <a id="6376" class="Symbol">(</a> <a id="6378" href="foundation-core.equivalences.html#12773" class="Function">is-equiv-equiv</a>
          <a id="6403" class="Symbol">(</a> <a id="6405" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="6425" class="Symbol">)</a>
          <a id="6437" class="Symbol">(</a> <a id="6439" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="6459" class="Symbol">)</a>
          <a id="6471" class="Symbol">(</a> <a id="6473" href="foundation-core.dependent-pair-types.html#687" class="Function">ind-Σ</a> <a id="6479" class="Symbol">(λ</a> <a id="6482" href="foundation.universal-property-truncation.html#6482" class="Bound">g</a> <a id="6484" href="foundation.universal-property-truncation.html#6484" class="Bound">s</a> <a id="6486" class="Symbol">→</a> <a id="6488" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="6492" class="Symbol">))</a>
          <a id="6505" class="Symbol">(</a> <a id="6507" href="foundation.universal-property-truncation.html#6028" class="Bound">H</a> <a id="6509" class="Symbol">(</a><a id="6510" href="foundation-core.truncated-types.html#6022" class="Function">Σ-Truncated-Type</a> <a id="6527" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="6529" href="foundation.universal-property-truncation.html#6030" class="Bound">X</a><a id="6530" class="Symbol">)))</a>
        <a id="6542" class="Symbol">(</a> <a id="6544" href="foundation-core.functions.html#309" class="Function">id</a><a id="6546" class="Symbol">)</a>

  <a id="6551" class="Keyword">abstract</a>
    <a id="6564" href="foundation.universal-property-truncation.html#6564" class="Function">is-truncation-dependent-universal-property-truncation</a> <a id="6618" class="Symbol">:</a>
      <a id="6626" class="Symbol">({</a><a id="6628" href="foundation.universal-property-truncation.html#6628" class="Bound">l</a> <a id="6630" class="Symbol">:</a> <a id="6632" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6637" class="Symbol">}</a> <a id="6639" class="Symbol">→</a> <a id="6641" href="foundation.universal-property-truncation.html#2939" class="Function">dependent-universal-property-truncation</a> <a id="6681" href="foundation.universal-property-truncation.html#6628" class="Bound">l</a> <a id="6683" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="6685" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a><a id="6686" class="Symbol">)</a> <a id="6688" class="Symbol">→</a>
      <a id="6696" class="Symbol">{</a><a id="6697" href="foundation.universal-property-truncation.html#6697" class="Bound">l</a> <a id="6699" class="Symbol">:</a> <a id="6701" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6706" class="Symbol">}</a> <a id="6708" class="Symbol">→</a> <a id="6710" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="6724" href="foundation.universal-property-truncation.html#6697" class="Bound">l</a> <a id="6726" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="6728" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a>
    <a id="6734" href="foundation.universal-property-truncation.html#6564" class="Function">is-truncation-dependent-universal-property-truncation</a> <a id="6788" href="foundation.universal-property-truncation.html#6788" class="Bound">H</a> <a id="6790" href="foundation.universal-property-truncation.html#6790" class="Bound">X</a> <a id="6792" class="Symbol">=</a>
      <a id="6800" href="foundation.universal-property-truncation.html#6788" class="Bound">H</a> <a id="6802" class="Symbol">(λ</a> <a id="6805" href="foundation.universal-property-truncation.html#6805" class="Bound">b</a> <a id="6807" class="Symbol">→</a> <a id="6809" href="foundation.universal-property-truncation.html#6790" class="Bound">X</a><a id="6810" class="Symbol">)</a>

  <a id="6815" href="foundation.universal-property-truncation.html#6815" class="Function">sec-is-truncation</a> <a id="6833" class="Symbol">:</a>
    <a id="6839" class="Symbol">({</a><a id="6841" href="foundation.universal-property-truncation.html#6841" class="Bound">l</a> <a id="6843" class="Symbol">:</a> <a id="6845" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6850" class="Symbol">}</a> <a id="6852" class="Symbol">→</a> <a id="6854" href="foundation.universal-property-truncation.html#1985" class="Function">is-truncation</a> <a id="6868" href="foundation.universal-property-truncation.html#6841" class="Bound">l</a> <a id="6870" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="6872" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a><a id="6873" class="Symbol">)</a> <a id="6875" class="Symbol">→</a>
    <a id="6881" class="Symbol">{</a><a id="6882" href="foundation.universal-property-truncation.html#6882" class="Bound">l3</a> <a id="6885" class="Symbol">:</a> <a id="6887" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6892" class="Symbol">}</a> <a id="6894" class="Symbol">(</a><a id="6895" href="foundation.universal-property-truncation.html#6895" class="Bound">C</a> <a id="6897" class="Symbol">:</a> <a id="6899" href="foundation-core.truncated-types.html#1651" class="Function">Truncated-Type</a> <a id="6914" href="foundation.universal-property-truncation.html#6882" class="Bound">l3</a> <a id="6917" href="foundation.universal-property-truncation.html#5701" class="Bound">k</a><a id="6918" class="Symbol">)</a>
    <a id="6924" class="Symbol">(</a><a id="6925" href="foundation.universal-property-truncation.html#6925" class="Bound">h</a> <a id="6927" class="Symbol">:</a> <a id="6929" href="foundation.universal-property-truncation.html#5709" class="Bound">A</a> <a id="6931" class="Symbol">→</a> <a id="6933" href="foundation-core.truncated-types.html#1786" class="Function">type-Truncated-Type</a> <a id="6953" href="foundation.universal-property-truncation.html#6895" class="Bound">C</a><a id="6954" class="Symbol">)</a> <a id="6956" class="Symbol">(</a><a id="6957" href="foundation.universal-property-truncation.html#6957" class="Bound">g</a> <a id="6959" class="Symbol">:</a> <a id="6961" href="foundation.truncated-types.html#3483" class="Function">type-hom-Truncated-Type</a> <a id="6985" href="foundation.universal-property-truncation.html#5701" class="Bound">k</a> <a id="6987" href="foundation.universal-property-truncation.html#6895" class="Bound">C</a> <a id="6989" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a><a id="6990" class="Symbol">)</a> <a id="6992" class="Symbol">→</a>
    <a id="6998" href="foundation.universal-property-truncation.html#5749" class="Bound">f</a> <a id="7000" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="7002" class="Symbol">(</a><a id="7003" href="foundation.universal-property-truncation.html#6957" class="Bound">g</a> <a id="7005" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="7007" href="foundation.universal-property-truncation.html#6925" class="Bound">h</a><a id="7008" class="Symbol">)</a> <a id="7010" class="Symbol">→</a> <a id="7012" href="foundation-core.sections.html#521" class="Function">sec</a> <a id="7016" href="foundation.universal-property-truncation.html#6957" class="Bound">g</a>
  <a id="7020" href="foundation.universal-property-truncation.html#6815" class="Function">sec-is-truncation</a> <a id="7038" href="foundation.universal-property-truncation.html#7038" class="Bound">H</a> <a id="7040" href="foundation.universal-property-truncation.html#7040" class="Bound">C</a> <a id="7042" href="foundation.universal-property-truncation.html#7042" class="Bound">h</a> <a id="7044" href="foundation.universal-property-truncation.html#7044" class="Bound">g</a> <a id="7046" href="foundation.universal-property-truncation.html#7046" class="Bound">K</a> <a id="7048" class="Symbol">=</a>
    <a id="7054" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#2808" class="Function">map-distributive-Π-Σ</a>
      <a id="7081" class="Symbol">(</a> <a id="7083" href="foundation-core.equivalences.html#4173" class="Function">map-inv-is-equiv</a>
        <a id="7108" class="Symbol">(</a> <a id="7110" href="foundation.universal-property-truncation.html#5804" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="7164" href="foundation.universal-property-truncation.html#7038" class="Bound">H</a>
          <a id="7176" class="Symbol">(</a> <a id="7178" href="foundation-core.truncated-types.html#6396" class="Function">fib-Truncated-Type</a> <a id="7197" href="foundation.universal-property-truncation.html#7040" class="Bound">C</a> <a id="7199" href="foundation.universal-property-truncation.html#5721" class="Bound">B</a> <a id="7201" href="foundation.universal-property-truncation.html#7044" class="Bound">g</a><a id="7202" class="Symbol">))</a>
        <a id="7213" class="Symbol">(</a> <a id="7215" class="Symbol">λ</a> <a id="7217" href="foundation.universal-property-truncation.html#7217" class="Bound">a</a> <a id="7219" class="Symbol">→</a> <a id="7221" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="7226" class="Symbol">(</a><a id="7227" href="foundation.universal-property-truncation.html#7042" class="Bound">h</a> <a id="7229" href="foundation.universal-property-truncation.html#7217" class="Bound">a</a><a id="7230" class="Symbol">)</a> <a id="7232" class="Symbol">(</a><a id="7233" href="foundation-core.identity-types.html#1552" class="Function">inv</a> <a id="7237" class="Symbol">(</a><a id="7238" href="foundation.universal-property-truncation.html#7046" class="Bound">K</a> <a id="7240" href="foundation.universal-property-truncation.html#7217" class="Bound">a</a><a id="7241" class="Symbol">))))</a>
</pre>
## To do

<pre class="Agda">
<a id="7270" class="Comment">{-

-- Theorem 18.5.2 (iii) implies (i)

reflects-mere-eq :
  {l1 l2 : Level} {A : UU l1} (X : UU-Set l2) (f : A → type-Set X) →
  reflects-Eq-Rel (mere-eq-Eq-Rel A) f
reflects-mere-eq X f {x} {y} r =
  apply-universal-property-trunc-Prop r
    ( Id-Prop X (f x) (f y))
    ( ap f)

reflecting-map-mere-eq :
  {l1 l2 : Level} {A : UU l1} (X : UU-Set l2) (f : A → type-Set X) →
  reflecting-map-Eq-Rel (mere-eq-Eq-Rel A) (type-Set X)
reflecting-map-mere-eq X f = pair f (reflects-mere-eq X f)

abstract
  is-set-truncation-is-set-quotient :
    {l1 l2 l3 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B) →
    ( {l : Level} →
      is-set-quotient l (mere-eq-Eq-Rel A) B (reflecting-map-mere-eq B f)) →
    is-set-truncation l3 B f
  is-set-truncation-is-set-quotient {A = A} B f H X =
    is-equiv-comp
      ( precomp-Set f X)
      ( pr1)
      ( precomp-Set-Quotient
        ( mere-eq-Eq-Rel A)
        ( B)
        ( reflecting-map-mere-eq B f)
        ( X))
      ( refl-htpy)
      ( H X)
      ( is-equiv-pr1-is-contr
        ( λ h →
          is-proof-irrelevant-is-prop
            ( is-prop-reflects-Eq-Rel (mere-eq-Eq-Rel A) X h)
            ( reflects-mere-eq X h)))

abstract
  is-set-quotient-is-set-truncation :
    {l1 l2 l3 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B) →
    ( {l : Level} → is-set-truncation l B f) →
    is-set-quotient l3 (mere-eq-Eq-Rel A) B (reflecting-map-mere-eq B f)
  is-set-quotient-is-set-truncation {A = A} B f H X =
    is-equiv-right-factor
      ( precomp-Set f X)
      ( pr1)
      ( precomp-Set-Quotient
        ( mere-eq-Eq-Rel A)
        ( B)
        ( reflecting-map-mere-eq B f)
        ( X))
      ( refl-htpy)
      ( is-equiv-pr1-is-contr
        ( λ h →
          is-proof-irrelevant-is-prop
            ( is-prop-reflects-Eq-Rel (mere-eq-Eq-Rel A) X h)
            ( reflects-mere-eq X h)))
      ( H X)

-- Definition 18.5.3

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