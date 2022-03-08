# The universal property of truncations

<pre class="Agda"><a id="50" class="Symbol">{-#</a> <a id="54" class="Keyword">OPTIONS</a> <a id="62" class="Pragma">--without-K</a> <a id="74" class="Pragma">--exact-split</a> <a id="88" class="Pragma">--allow-unsolved-metas</a> <a id="111" class="Symbol">#-}</a>

<a id="116" class="Keyword">module</a> <a id="123" href="foundation.universal-property-truncation.html" class="Module">foundation.universal-property-truncation</a> <a id="164" class="Keyword">where</a>

<a id="171" class="Keyword">open</a> <a id="176" class="Keyword">import</a> <a id="183" href="foundation.contractible-maps.html" class="Module">foundation.contractible-maps</a> <a id="212" class="Keyword">using</a>
  <a id="220" class="Symbol">(</a> <a id="222" href="foundation-core.contractible-maps.html#2368" class="Function">is-equiv-is-contr-map</a><a id="243" class="Symbol">;</a> <a id="245" href="foundation-core.contractible-maps.html#3850" class="Function">is-contr-map-is-equiv</a><a id="266" class="Symbol">)</a>
<a id="268" class="Keyword">open</a> <a id="273" class="Keyword">import</a> <a id="280" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a> <a id="310" class="Keyword">using</a>
  <a id="318" class="Symbol">(</a> <a id="320" href="foundation-core.contractible-types.html#925" class="Function">is-contr</a><a id="328" class="Symbol">;</a> <a id="330" href="foundation-core.contractible-types.html#3230" class="Function">is-contr-equiv</a><a id="344" class="Symbol">;</a> <a id="346" href="foundation-core.contractible-types.html#3739" class="Function">is-contr-equiv&#39;</a><a id="361" class="Symbol">;</a> <a id="363" href="foundation-core.contractible-types.html#1018" class="Function">center</a><a id="369" class="Symbol">)</a>
<a id="371" class="Keyword">open</a> <a id="376" class="Keyword">import</a> <a id="383" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="415" class="Keyword">using</a> <a id="421" class="Symbol">(</a><a id="422" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="423" class="Symbol">;</a> <a id="425" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="429" class="Symbol">;</a> <a id="431" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="434" class="Symbol">;</a> <a id="436" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="439" class="Symbol">;</a> <a id="441" href="foundation-core.dependent-pair-types.html#687" class="Function">ind-Σ</a><a id="446" class="Symbol">)</a>
<a id="448" class="Keyword">open</a> <a id="453" class="Keyword">import</a>
  <a id="462" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html" class="Module">foundation.distributivity-of-dependent-functions-over-dependent-pairs</a> <a id="532" class="Keyword">using</a>
  <a id="540" class="Symbol">(</a> <a id="542" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="562" class="Symbol">;</a> <a id="564" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#2808" class="Function">map-distributive-Π-Σ</a><a id="584" class="Symbol">)</a>
<a id="586" class="Keyword">open</a> <a id="591" class="Keyword">import</a> <a id="598" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="622" class="Keyword">using</a>
  <a id="630" class="Symbol">(</a> <a id="632" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a><a id="640" class="Symbol">;</a> <a id="642" href="foundation-core.equivalences.html#12773" class="Function">is-equiv-equiv</a><a id="656" class="Symbol">;</a> <a id="658" href="foundation-core.equivalences.html#4173" class="Function">map-inv-is-equiv</a><a id="674" class="Symbol">;</a> <a id="676" href="foundation.equivalences.html#9064" class="Function">is-equiv-precomp-is-equiv</a><a id="701" class="Symbol">;</a>
    <a id="707" href="foundation-core.equivalences.html#2309" class="Function">is-equiv-id</a><a id="718" class="Symbol">;</a> <a id="720" href="foundation-core.equivalences.html#1607" class="Function Operator">_≃_</a><a id="723" class="Symbol">;</a> <a id="725" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a><a id="734" class="Symbol">;</a> <a id="736" href="foundation-core.equivalences.html#1862" class="Function">is-equiv-map-equiv</a><a id="754" class="Symbol">)</a>
<a id="756" class="Keyword">open</a> <a id="761" class="Keyword">import</a> <a id="768" href="foundation.function-extensionality.html" class="Module">foundation.function-extensionality</a> <a id="803" class="Keyword">using</a> <a id="809" class="Symbol">(</a><a id="810" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="822" class="Symbol">)</a>
<a id="824" class="Keyword">open</a> <a id="829" class="Keyword">import</a> <a id="836" href="foundation.functions.html" class="Module">foundation.functions</a> <a id="857" class="Keyword">using</a> <a id="863" class="Symbol">(</a><a id="864" href="foundation-core.functions.html#925" class="Function">precomp</a><a id="871" class="Symbol">;</a> <a id="873" href="foundation-core.functions.html#407" class="Function Operator">_∘_</a><a id="876" class="Symbol">;</a> <a id="878" href="foundation-core.functions.html#309" class="Function">id</a><a id="880" class="Symbol">)</a>
<a id="882" class="Keyword">open</a> <a id="887" class="Keyword">import</a> <a id="894" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a> <a id="940" class="Keyword">using</a>
  <a id="948" class="Symbol">(</a> <a id="950" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a><a id="959" class="Symbol">;</a> <a id="961" href="foundation-core.functoriality-dependent-pair-types.html#10750" class="Function">is-fiberwise-equiv-is-equiv-map-Σ</a><a id="994" class="Symbol">)</a>
<a id="996" class="Keyword">open</a> <a id="1001" class="Keyword">import</a> <a id="1008" href="foundation.homotopies.html" class="Module">foundation.homotopies</a> <a id="1030" class="Keyword">using</a> <a id="1036" class="Symbol">(</a><a id="1037" href="foundation-core.homotopies.html#467" class="Function Operator">_~_</a><a id="1040" class="Symbol">)</a>
<a id="1042" class="Keyword">open</a> <a id="1047" class="Keyword">import</a> <a id="1054" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="1080" class="Keyword">using</a> <a id="1086" class="Symbol">(</a><a id="1087" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="1089" class="Symbol">;</a> <a id="1091" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="1095" class="Symbol">;</a> <a id="1097" href="foundation-core.identity-types.html#1552" class="Function">inv</a><a id="1100" class="Symbol">)</a>
<a id="1102" class="Keyword">open</a> <a id="1107" class="Keyword">import</a> <a id="1114" href="foundation.sections.html" class="Module">foundation.sections</a> <a id="1134" class="Keyword">using</a> <a id="1140" class="Symbol">(</a><a id="1141" href="foundation-core.sections.html#521" class="Function">sec</a><a id="1144" class="Symbol">)</a>
<a id="1146" class="Keyword">open</a> <a id="1151" class="Keyword">import</a> <a id="1158" href="foundation.truncated-types.html" class="Module">foundation.truncated-types</a> <a id="1185" class="Keyword">using</a>
  <a id="1193" class="Symbol">(</a> <a id="1195" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a><a id="1212" class="Symbol">;</a> <a id="1214" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a><a id="1233" class="Symbol">;</a> <a id="1235" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a><a id="1258" class="Symbol">;</a>
    <a id="1264" href="foundation-core.truncated-types.html#6052" class="Function">Σ-Truncated-Type</a><a id="1280" class="Symbol">;</a> <a id="1282" href="foundation-core.truncated-types.html#6435" class="Function">fib-Truncated-Type</a><a id="1300" class="Symbol">;</a> <a id="1302" href="foundation-core.truncated-types.html#1466" class="Function">is-trunc</a><a id="1310" class="Symbol">)</a>
<a id="1312" class="Keyword">open</a> <a id="1317" class="Keyword">import</a> <a id="1324" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a> <a id="1353" class="Keyword">using</a> <a id="1359" class="Symbol">(</a><a id="1360" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="1361" class="Symbol">)</a>
<a id="1363" class="Keyword">open</a> <a id="1368" class="Keyword">import</a> <a id="1375" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="1402" class="Keyword">using</a> <a id="1408" class="Symbol">(</a><a id="1409" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="1411" class="Symbol">;</a> <a id="1413" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1418" class="Symbol">;</a> <a id="1420" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="1423" class="Symbol">;</a> <a id="1425" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="1429" class="Symbol">)</a>
</pre>
## Idea

We say that a map `f : A → B` into a `k`-truncated type `B` is a `k`-truncation of `A` -- or that it satisfies the universal property of the `k`-truncation of `A` -- if any map `g : A → C` into a `k`-truncated type `C` extends uniquely along `f` to a map `B → C`.

## Definition

### The condition on a map to be a truncation

<pre class="Agda"><a id="precomp-Trunc"></a><a id="1780" href="foundation.universal-property-truncation.html#1780" class="Function">precomp-Trunc</a> <a id="1794" class="Symbol">:</a>
  <a id="1798" class="Symbol">{</a><a id="1799" href="foundation.universal-property-truncation.html#1799" class="Bound">l1</a> <a id="1802" href="foundation.universal-property-truncation.html#1802" class="Bound">l2</a> <a id="1805" href="foundation.universal-property-truncation.html#1805" class="Bound">l3</a> <a id="1808" class="Symbol">:</a> <a id="1810" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1815" class="Symbol">}</a> <a id="1817" class="Symbol">{</a><a id="1818" href="foundation.universal-property-truncation.html#1818" class="Bound">k</a> <a id="1820" class="Symbol">:</a> <a id="1822" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="1823" class="Symbol">}</a> <a id="1825" class="Symbol">{</a><a id="1826" href="foundation.universal-property-truncation.html#1826" class="Bound">A</a> <a id="1828" class="Symbol">:</a> <a id="1830" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1833" href="foundation.universal-property-truncation.html#1799" class="Bound">l1</a><a id="1835" class="Symbol">}</a> <a id="1837" class="Symbol">{</a><a id="1838" href="foundation.universal-property-truncation.html#1838" class="Bound">B</a> <a id="1840" class="Symbol">:</a> <a id="1842" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1845" href="foundation.universal-property-truncation.html#1802" class="Bound">l2</a><a id="1847" class="Symbol">}</a> <a id="1849" class="Symbol">(</a><a id="1850" href="foundation.universal-property-truncation.html#1850" class="Bound">f</a> <a id="1852" class="Symbol">:</a> <a id="1854" href="foundation.universal-property-truncation.html#1826" class="Bound">A</a> <a id="1856" class="Symbol">→</a> <a id="1858" href="foundation.universal-property-truncation.html#1838" class="Bound">B</a><a id="1859" class="Symbol">)</a>
  <a id="1863" class="Symbol">(</a><a id="1864" href="foundation.universal-property-truncation.html#1864" class="Bound">C</a> <a id="1866" class="Symbol">:</a> <a id="1868" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="1886" href="foundation.universal-property-truncation.html#1805" class="Bound">l3</a> <a id="1889" href="foundation.universal-property-truncation.html#1818" class="Bound">k</a><a id="1890" class="Symbol">)</a> <a id="1892" class="Symbol">→</a>
  <a id="1896" class="Symbol">(</a><a id="1897" href="foundation.universal-property-truncation.html#1838" class="Bound">B</a> <a id="1899" class="Symbol">→</a> <a id="1901" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="1921" href="foundation.universal-property-truncation.html#1864" class="Bound">C</a><a id="1922" class="Symbol">)</a> <a id="1924" class="Symbol">→</a> <a id="1926" class="Symbol">(</a><a id="1927" href="foundation.universal-property-truncation.html#1826" class="Bound">A</a> <a id="1929" class="Symbol">→</a> <a id="1931" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="1951" href="foundation.universal-property-truncation.html#1864" class="Bound">C</a><a id="1952" class="Symbol">)</a>
<a id="1954" href="foundation.universal-property-truncation.html#1780" class="Function">precomp-Trunc</a> <a id="1968" href="foundation.universal-property-truncation.html#1968" class="Bound">f</a> <a id="1970" href="foundation.universal-property-truncation.html#1970" class="Bound">C</a> <a id="1972" class="Symbol">=</a> <a id="1974" href="foundation-core.functions.html#925" class="Function">precomp</a> <a id="1982" href="foundation.universal-property-truncation.html#1968" class="Bound">f</a> <a id="1984" class="Symbol">(</a><a id="1985" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2005" href="foundation.universal-property-truncation.html#1970" class="Bound">C</a><a id="2006" class="Symbol">)</a>

<a id="is-truncation"></a><a id="2009" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="2023" class="Symbol">:</a>
  <a id="2027" class="Symbol">{</a><a id="2028" href="foundation.universal-property-truncation.html#2028" class="Bound">l1</a> <a id="2031" href="foundation.universal-property-truncation.html#2031" class="Bound">l2</a> <a id="2034" class="Symbol">:</a> <a id="2036" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2041" class="Symbol">}</a> <a id="2043" class="Symbol">(</a><a id="2044" href="foundation.universal-property-truncation.html#2044" class="Bound">l</a> <a id="2046" class="Symbol">:</a> <a id="2048" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2053" class="Symbol">)</a> <a id="2055" class="Symbol">{</a><a id="2056" href="foundation.universal-property-truncation.html#2056" class="Bound">k</a> <a id="2058" class="Symbol">:</a> <a id="2060" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="2061" class="Symbol">}</a> <a id="2063" class="Symbol">{</a><a id="2064" href="foundation.universal-property-truncation.html#2064" class="Bound">A</a> <a id="2066" class="Symbol">:</a> <a id="2068" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2071" href="foundation.universal-property-truncation.html#2028" class="Bound">l1</a><a id="2073" class="Symbol">}</a>
  <a id="2077" class="Symbol">(</a><a id="2078" href="foundation.universal-property-truncation.html#2078" class="Bound">B</a> <a id="2080" class="Symbol">:</a> <a id="2082" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="2100" href="foundation.universal-property-truncation.html#2031" class="Bound">l2</a> <a id="2103" href="foundation.universal-property-truncation.html#2056" class="Bound">k</a><a id="2104" class="Symbol">)</a> <a id="2106" class="Symbol">→</a> <a id="2108" class="Symbol">(</a><a id="2109" href="foundation.universal-property-truncation.html#2064" class="Bound">A</a> <a id="2111" class="Symbol">→</a> <a id="2113" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2133" href="foundation.universal-property-truncation.html#2078" class="Bound">B</a><a id="2134" class="Symbol">)</a> <a id="2136" class="Symbol">→</a>
  <a id="2140" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2143" class="Symbol">(</a><a id="2144" href="foundation.universal-property-truncation.html#2028" class="Bound">l1</a> <a id="2147" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2149" href="foundation.universal-property-truncation.html#2031" class="Bound">l2</a> <a id="2152" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2154" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="2159" href="foundation.universal-property-truncation.html#2044" class="Bound">l</a><a id="2160" class="Symbol">)</a>
<a id="2162" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="2176" href="foundation.universal-property-truncation.html#2176" class="Bound">l</a> <a id="2178" class="Symbol">{</a><a id="2179" href="foundation.universal-property-truncation.html#2179" class="Bound">k</a><a id="2180" class="Symbol">}</a> <a id="2182" href="foundation.universal-property-truncation.html#2182" class="Bound">B</a> <a id="2184" href="foundation.universal-property-truncation.html#2184" class="Bound">f</a> <a id="2186" class="Symbol">=</a>
  <a id="2190" class="Symbol">(</a><a id="2191" href="foundation.universal-property-truncation.html#2191" class="Bound">C</a> <a id="2193" class="Symbol">:</a> <a id="2195" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="2213" href="foundation.universal-property-truncation.html#2176" class="Bound">l</a> <a id="2215" href="foundation.universal-property-truncation.html#2179" class="Bound">k</a><a id="2216" class="Symbol">)</a> <a id="2218" class="Symbol">→</a> <a id="2220" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="2229" class="Symbol">(</a><a id="2230" href="foundation.universal-property-truncation.html#1780" class="Function">precomp-Trunc</a> <a id="2244" href="foundation.universal-property-truncation.html#2184" class="Bound">f</a> <a id="2246" href="foundation.universal-property-truncation.html#2191" class="Bound">C</a><a id="2247" class="Symbol">)</a>
</pre>
### The universal property of truncations

<pre class="Agda"><a id="universal-property-truncation"></a><a id="2305" href="foundation.universal-property-truncation.html#2305" class="Function">universal-property-truncation</a> <a id="2335" class="Symbol">:</a>
  <a id="2339" class="Symbol">(</a><a id="2340" href="foundation.universal-property-truncation.html#2340" class="Bound">l</a> <a id="2342" class="Symbol">:</a> <a id="2344" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2349" class="Symbol">)</a> <a id="2351" class="Symbol">{</a><a id="2352" href="foundation.universal-property-truncation.html#2352" class="Bound">l1</a> <a id="2355" href="foundation.universal-property-truncation.html#2355" class="Bound">l2</a> <a id="2358" class="Symbol">:</a> <a id="2360" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2365" class="Symbol">}</a> <a id="2367" class="Symbol">{</a><a id="2368" href="foundation.universal-property-truncation.html#2368" class="Bound">k</a> <a id="2370" class="Symbol">:</a> <a id="2372" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="2373" class="Symbol">}</a> <a id="2375" class="Symbol">{</a><a id="2376" href="foundation.universal-property-truncation.html#2376" class="Bound">A</a> <a id="2378" class="Symbol">:</a> <a id="2380" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2383" href="foundation.universal-property-truncation.html#2352" class="Bound">l1</a><a id="2385" class="Symbol">}</a>
  <a id="2389" class="Symbol">(</a><a id="2390" href="foundation.universal-property-truncation.html#2390" class="Bound">B</a> <a id="2392" class="Symbol">:</a> <a id="2394" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="2412" href="foundation.universal-property-truncation.html#2355" class="Bound">l2</a> <a id="2415" href="foundation.universal-property-truncation.html#2368" class="Bound">k</a><a id="2416" class="Symbol">)</a> <a id="2418" class="Symbol">(</a><a id="2419" href="foundation.universal-property-truncation.html#2419" class="Bound">f</a> <a id="2421" class="Symbol">:</a> <a id="2423" href="foundation.universal-property-truncation.html#2376" class="Bound">A</a> <a id="2425" class="Symbol">→</a> <a id="2427" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2447" href="foundation.universal-property-truncation.html#2390" class="Bound">B</a><a id="2448" class="Symbol">)</a> <a id="2450" class="Symbol">→</a>
  <a id="2454" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2457" class="Symbol">(</a><a id="2458" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="2463" href="foundation.universal-property-truncation.html#2340" class="Bound">l</a> <a id="2465" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2467" href="foundation.universal-property-truncation.html#2352" class="Bound">l1</a> <a id="2470" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2472" href="foundation.universal-property-truncation.html#2355" class="Bound">l2</a><a id="2474" class="Symbol">)</a>
<a id="2476" href="foundation.universal-property-truncation.html#2305" class="Function">universal-property-truncation</a> <a id="2506" href="foundation.universal-property-truncation.html#2506" class="Bound">l</a> <a id="2508" class="Symbol">{</a><a id="2509" class="Argument">k</a> <a id="2511" class="Symbol">=</a> <a id="2513" href="foundation.universal-property-truncation.html#2513" class="Bound">k</a><a id="2514" class="Symbol">}</a> <a id="2516" class="Symbol">{</a><a id="2517" href="foundation.universal-property-truncation.html#2517" class="Bound">A</a><a id="2518" class="Symbol">}</a> <a id="2520" href="foundation.universal-property-truncation.html#2520" class="Bound">B</a> <a id="2522" href="foundation.universal-property-truncation.html#2522" class="Bound">f</a> <a id="2524" class="Symbol">=</a>
  <a id="2528" class="Symbol">(</a><a id="2529" href="foundation.universal-property-truncation.html#2529" class="Bound">C</a> <a id="2531" class="Symbol">:</a> <a id="2533" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="2551" href="foundation.universal-property-truncation.html#2506" class="Bound">l</a> <a id="2553" href="foundation.universal-property-truncation.html#2513" class="Bound">k</a><a id="2554" class="Symbol">)</a> <a id="2556" class="Symbol">(</a><a id="2557" href="foundation.universal-property-truncation.html#2557" class="Bound">g</a> <a id="2559" class="Symbol">:</a> <a id="2561" href="foundation.universal-property-truncation.html#2517" class="Bound">A</a> <a id="2563" class="Symbol">→</a> <a id="2565" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2585" href="foundation.universal-property-truncation.html#2529" class="Bound">C</a><a id="2586" class="Symbol">)</a> <a id="2588" class="Symbol">→</a>
  <a id="2592" href="foundation-core.contractible-types.html#925" class="Function">is-contr</a> <a id="2601" class="Symbol">(</a><a id="2602" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="2604" class="Symbol">(</a><a id="2605" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="2629" href="foundation.universal-property-truncation.html#2513" class="Bound">k</a> <a id="2631" href="foundation.universal-property-truncation.html#2520" class="Bound">B</a> <a id="2633" href="foundation.universal-property-truncation.html#2529" class="Bound">C</a><a id="2634" class="Symbol">)</a> <a id="2636" class="Symbol">(λ</a> <a id="2639" href="foundation.universal-property-truncation.html#2639" class="Bound">h</a> <a id="2641" class="Symbol">→</a> <a id="2643" class="Symbol">(</a><a id="2644" href="foundation.universal-property-truncation.html#2639" class="Bound">h</a> <a id="2646" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="2648" href="foundation.universal-property-truncation.html#2522" class="Bound">f</a><a id="2649" class="Symbol">)</a> <a id="2651" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="2653" href="foundation.universal-property-truncation.html#2557" class="Bound">g</a><a id="2654" class="Symbol">))</a>
</pre>
### The dependent universal property of truncations

<pre class="Agda"><a id="precomp-Π-Truncated-Type"></a><a id="2719" href="foundation.universal-property-truncation.html#2719" class="Function">precomp-Π-Truncated-Type</a> <a id="2744" class="Symbol">:</a>
  <a id="2748" class="Symbol">{</a><a id="2749" href="foundation.universal-property-truncation.html#2749" class="Bound">l1</a> <a id="2752" href="foundation.universal-property-truncation.html#2752" class="Bound">l2</a> <a id="2755" href="foundation.universal-property-truncation.html#2755" class="Bound">l3</a> <a id="2758" class="Symbol">:</a> <a id="2760" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2765" class="Symbol">}</a> <a id="2767" class="Symbol">{</a><a id="2768" href="foundation.universal-property-truncation.html#2768" class="Bound">k</a> <a id="2770" class="Symbol">:</a> <a id="2772" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="2773" class="Symbol">}</a> <a id="2775" class="Symbol">{</a><a id="2776" href="foundation.universal-property-truncation.html#2776" class="Bound">A</a> <a id="2778" class="Symbol">:</a> <a id="2780" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2783" href="foundation.universal-property-truncation.html#2749" class="Bound">l1</a><a id="2785" class="Symbol">}</a> <a id="2787" class="Symbol">{</a><a id="2788" href="foundation.universal-property-truncation.html#2788" class="Bound">B</a> <a id="2790" class="Symbol">:</a> <a id="2792" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2795" href="foundation.universal-property-truncation.html#2752" class="Bound">l2</a><a id="2797" class="Symbol">}</a> <a id="2799" class="Symbol">(</a><a id="2800" href="foundation.universal-property-truncation.html#2800" class="Bound">f</a> <a id="2802" class="Symbol">:</a> <a id="2804" href="foundation.universal-property-truncation.html#2776" class="Bound">A</a> <a id="2806" class="Symbol">→</a> <a id="2808" href="foundation.universal-property-truncation.html#2788" class="Bound">B</a><a id="2809" class="Symbol">)</a>
  <a id="2813" class="Symbol">(</a><a id="2814" href="foundation.universal-property-truncation.html#2814" class="Bound">C</a> <a id="2816" class="Symbol">:</a> <a id="2818" href="foundation.universal-property-truncation.html#2788" class="Bound">B</a> <a id="2820" class="Symbol">→</a> <a id="2822" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="2840" href="foundation.universal-property-truncation.html#2755" class="Bound">l3</a> <a id="2843" href="foundation.universal-property-truncation.html#2768" class="Bound">k</a><a id="2844" class="Symbol">)</a> <a id="2846" class="Symbol">→</a>
  <a id="2850" class="Symbol">((</a><a id="2852" href="foundation.universal-property-truncation.html#2852" class="Bound">b</a> <a id="2854" class="Symbol">:</a> <a id="2856" href="foundation.universal-property-truncation.html#2788" class="Bound">B</a><a id="2857" class="Symbol">)</a> <a id="2859" class="Symbol">→</a> <a id="2861" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2881" class="Symbol">(</a><a id="2882" href="foundation.universal-property-truncation.html#2814" class="Bound">C</a> <a id="2884" href="foundation.universal-property-truncation.html#2852" class="Bound">b</a><a id="2885" class="Symbol">))</a> <a id="2888" class="Symbol">→</a>
  <a id="2892" class="Symbol">((</a><a id="2894" href="foundation.universal-property-truncation.html#2894" class="Bound">a</a> <a id="2896" class="Symbol">:</a> <a id="2898" href="foundation.universal-property-truncation.html#2776" class="Bound">A</a><a id="2899" class="Symbol">)</a> <a id="2901" class="Symbol">→</a> <a id="2903" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2923" class="Symbol">(</a><a id="2924" href="foundation.universal-property-truncation.html#2814" class="Bound">C</a> <a id="2926" class="Symbol">(</a><a id="2927" href="foundation.universal-property-truncation.html#2800" class="Bound">f</a> <a id="2929" href="foundation.universal-property-truncation.html#2894" class="Bound">a</a><a id="2930" class="Symbol">)))</a>
<a id="2934" href="foundation.universal-property-truncation.html#2719" class="Function">precomp-Π-Truncated-Type</a> <a id="2959" href="foundation.universal-property-truncation.html#2959" class="Bound">f</a> <a id="2961" href="foundation.universal-property-truncation.html#2961" class="Bound">C</a> <a id="2963" href="foundation.universal-property-truncation.html#2963" class="Bound">h</a> <a id="2965" href="foundation.universal-property-truncation.html#2965" class="Bound">a</a> <a id="2967" class="Symbol">=</a> <a id="2969" href="foundation.universal-property-truncation.html#2963" class="Bound">h</a> <a id="2971" class="Symbol">(</a><a id="2972" href="foundation.universal-property-truncation.html#2959" class="Bound">f</a> <a id="2974" href="foundation.universal-property-truncation.html#2965" class="Bound">a</a><a id="2975" class="Symbol">)</a>

<a id="dependent-universal-property-truncation"></a><a id="2978" href="foundation.universal-property-truncation.html#2978" class="Function">dependent-universal-property-truncation</a> <a id="3018" class="Symbol">:</a>
  <a id="3022" class="Symbol">{</a><a id="3023" href="foundation.universal-property-truncation.html#3023" class="Bound">l1</a> <a id="3026" href="foundation.universal-property-truncation.html#3026" class="Bound">l2</a> <a id="3029" class="Symbol">:</a> <a id="3031" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3036" class="Symbol">}</a> <a id="3038" class="Symbol">(</a><a id="3039" href="foundation.universal-property-truncation.html#3039" class="Bound">l</a> <a id="3041" class="Symbol">:</a> <a id="3043" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3048" class="Symbol">)</a> <a id="3050" class="Symbol">{</a><a id="3051" href="foundation.universal-property-truncation.html#3051" class="Bound">k</a> <a id="3053" class="Symbol">:</a> <a id="3055" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3056" class="Symbol">}</a> <a id="3058" class="Symbol">{</a><a id="3059" href="foundation.universal-property-truncation.html#3059" class="Bound">A</a> <a id="3061" class="Symbol">:</a> <a id="3063" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3066" href="foundation.universal-property-truncation.html#3023" class="Bound">l1</a><a id="3068" class="Symbol">}</a> <a id="3070" class="Symbol">(</a><a id="3071" href="foundation.universal-property-truncation.html#3071" class="Bound">B</a> <a id="3073" class="Symbol">:</a> <a id="3075" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="3093" href="foundation.universal-property-truncation.html#3026" class="Bound">l2</a> <a id="3096" href="foundation.universal-property-truncation.html#3051" class="Bound">k</a><a id="3097" class="Symbol">)</a>
  <a id="3101" class="Symbol">(</a><a id="3102" href="foundation.universal-property-truncation.html#3102" class="Bound">f</a> <a id="3104" class="Symbol">:</a> <a id="3106" href="foundation.universal-property-truncation.html#3059" class="Bound">A</a> <a id="3108" class="Symbol">→</a> <a id="3110" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3130" href="foundation.universal-property-truncation.html#3071" class="Bound">B</a><a id="3131" class="Symbol">)</a> <a id="3133" class="Symbol">→</a> <a id="3135" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3138" class="Symbol">(</a><a id="3139" href="foundation.universal-property-truncation.html#3023" class="Bound">l1</a> <a id="3142" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3144" href="foundation.universal-property-truncation.html#3026" class="Bound">l2</a> <a id="3147" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3149" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="3154" href="foundation.universal-property-truncation.html#3039" class="Bound">l</a><a id="3155" class="Symbol">)</a>
<a id="3157" href="foundation.universal-property-truncation.html#2978" class="Function">dependent-universal-property-truncation</a> <a id="3197" href="foundation.universal-property-truncation.html#3197" class="Bound">l</a> <a id="3199" class="Symbol">{</a><a id="3200" href="foundation.universal-property-truncation.html#3200" class="Bound">k</a><a id="3201" class="Symbol">}</a> <a id="3203" href="foundation.universal-property-truncation.html#3203" class="Bound">B</a> <a id="3205" href="foundation.universal-property-truncation.html#3205" class="Bound">f</a> <a id="3207" class="Symbol">=</a>
  <a id="3211" class="Symbol">(</a><a id="3212" href="foundation.universal-property-truncation.html#3212" class="Bound">X</a> <a id="3214" class="Symbol">:</a> <a id="3216" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3236" href="foundation.universal-property-truncation.html#3203" class="Bound">B</a> <a id="3238" class="Symbol">→</a> <a id="3240" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="3258" href="foundation.universal-property-truncation.html#3197" class="Bound">l</a> <a id="3260" href="foundation.universal-property-truncation.html#3200" class="Bound">k</a><a id="3261" class="Symbol">)</a> <a id="3263" class="Symbol">→</a>
  <a id="3267" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="3276" class="Symbol">(</a><a id="3277" href="foundation.universal-property-truncation.html#2719" class="Function">precomp-Π-Truncated-Type</a> <a id="3302" href="foundation.universal-property-truncation.html#3205" class="Bound">f</a> <a id="3304" href="foundation.universal-property-truncation.html#3212" class="Bound">X</a><a id="3305" class="Symbol">)</a>
</pre>
## Properties

### Equivalences into `k`-truncated types are truncations

<pre class="Agda"><a id="3394" class="Keyword">abstract</a>
  <a id="is-truncation-id"></a><a id="3405" href="foundation.universal-property-truncation.html#3405" class="Function">is-truncation-id</a> <a id="3422" class="Symbol">:</a>
    <a id="3428" class="Symbol">{</a><a id="3429" href="foundation.universal-property-truncation.html#3429" class="Bound">l1</a> <a id="3432" class="Symbol">:</a> <a id="3434" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3439" class="Symbol">}</a> <a id="3441" class="Symbol">{</a><a id="3442" href="foundation.universal-property-truncation.html#3442" class="Bound">k</a> <a id="3444" class="Symbol">:</a> <a id="3446" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3447" class="Symbol">}</a> <a id="3449" class="Symbol">{</a><a id="3450" href="foundation.universal-property-truncation.html#3450" class="Bound">A</a> <a id="3452" class="Symbol">:</a> <a id="3454" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3457" href="foundation.universal-property-truncation.html#3429" class="Bound">l1</a><a id="3459" class="Symbol">}</a> <a id="3461" class="Symbol">(</a><a id="3462" href="foundation.universal-property-truncation.html#3462" class="Bound">H</a> <a id="3464" class="Symbol">:</a> <a id="3466" href="foundation-core.truncated-types.html#1466" class="Function">is-trunc</a> <a id="3475" href="foundation.universal-property-truncation.html#3442" class="Bound">k</a> <a id="3477" href="foundation.universal-property-truncation.html#3450" class="Bound">A</a><a id="3478" class="Symbol">)</a> <a id="3480" class="Symbol">→</a>
    <a id="3486" class="Symbol">{</a><a id="3487" href="foundation.universal-property-truncation.html#3487" class="Bound">l</a> <a id="3489" class="Symbol">:</a> <a id="3491" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3496" class="Symbol">}</a> <a id="3498" class="Symbol">→</a> <a id="3500" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="3514" href="foundation.universal-property-truncation.html#3487" class="Bound">l</a> <a id="3516" class="Symbol">(</a><a id="3517" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="3522" href="foundation.universal-property-truncation.html#3450" class="Bound">A</a> <a id="3524" href="foundation.universal-property-truncation.html#3462" class="Bound">H</a><a id="3525" class="Symbol">)</a> <a id="3527" href="foundation-core.functions.html#309" class="Function">id</a>
  <a id="3532" href="foundation.universal-property-truncation.html#3405" class="Function">is-truncation-id</a> <a id="3549" href="foundation.universal-property-truncation.html#3549" class="Bound">H</a> <a id="3551" href="foundation.universal-property-truncation.html#3551" class="Bound">B</a> <a id="3553" class="Symbol">=</a>
    <a id="3559" href="foundation.equivalences.html#9064" class="Function">is-equiv-precomp-is-equiv</a> <a id="3585" href="foundation-core.functions.html#309" class="Function">id</a> <a id="3588" href="foundation-core.equivalences.html#2309" class="Function">is-equiv-id</a> <a id="3600" class="Symbol">(</a><a id="3601" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3621" href="foundation.universal-property-truncation.html#3551" class="Bound">B</a><a id="3622" class="Symbol">)</a>

<a id="3625" class="Keyword">abstract</a>
  <a id="is-truncation-equiv"></a><a id="3636" href="foundation.universal-property-truncation.html#3636" class="Function">is-truncation-equiv</a> <a id="3656" class="Symbol">:</a>
    <a id="3662" class="Symbol">{</a><a id="3663" href="foundation.universal-property-truncation.html#3663" class="Bound">l1</a> <a id="3666" href="foundation.universal-property-truncation.html#3666" class="Bound">l2</a> <a id="3669" class="Symbol">:</a> <a id="3671" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3676" class="Symbol">}</a> <a id="3678" class="Symbol">{</a><a id="3679" href="foundation.universal-property-truncation.html#3679" class="Bound">k</a> <a id="3681" class="Symbol">:</a> <a id="3683" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3684" class="Symbol">}</a> <a id="3686" class="Symbol">{</a><a id="3687" href="foundation.universal-property-truncation.html#3687" class="Bound">A</a> <a id="3689" class="Symbol">:</a> <a id="3691" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="3694" href="foundation.universal-property-truncation.html#3663" class="Bound">l1</a><a id="3696" class="Symbol">}</a> <a id="3698" class="Symbol">(</a><a id="3699" href="foundation.universal-property-truncation.html#3699" class="Bound">B</a> <a id="3701" class="Symbol">:</a> <a id="3703" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="3721" href="foundation.universal-property-truncation.html#3666" class="Bound">l2</a> <a id="3724" href="foundation.universal-property-truncation.html#3679" class="Bound">k</a><a id="3725" class="Symbol">)</a>
    <a id="3731" class="Symbol">(</a><a id="3732" href="foundation.universal-property-truncation.html#3732" class="Bound">e</a> <a id="3734" class="Symbol">:</a> <a id="3736" href="foundation.universal-property-truncation.html#3687" class="Bound">A</a> <a id="3738" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="3740" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3760" href="foundation.universal-property-truncation.html#3699" class="Bound">B</a><a id="3761" class="Symbol">)</a> <a id="3763" class="Symbol">→</a>
    <a id="3769" class="Symbol">{</a><a id="3770" href="foundation.universal-property-truncation.html#3770" class="Bound">l</a> <a id="3772" class="Symbol">:</a> <a id="3774" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3779" class="Symbol">}</a> <a id="3781" class="Symbol">→</a> <a id="3783" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="3797" href="foundation.universal-property-truncation.html#3770" class="Bound">l</a> <a id="3799" href="foundation.universal-property-truncation.html#3699" class="Bound">B</a> <a id="3801" class="Symbol">(</a><a id="3802" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a> <a id="3812" href="foundation.universal-property-truncation.html#3732" class="Bound">e</a><a id="3813" class="Symbol">)</a>
  <a id="3817" href="foundation.universal-property-truncation.html#3636" class="Function">is-truncation-equiv</a> <a id="3837" href="foundation.universal-property-truncation.html#3837" class="Bound">B</a> <a id="3839" href="foundation.universal-property-truncation.html#3839" class="Bound">e</a> <a id="3841" href="foundation.universal-property-truncation.html#3841" class="Bound">C</a> <a id="3843" class="Symbol">=</a>
    <a id="3849" href="foundation.equivalences.html#9064" class="Function">is-equiv-precomp-is-equiv</a>
      <a id="3881" class="Symbol">(</a> <a id="3883" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a> <a id="3893" href="foundation.universal-property-truncation.html#3839" class="Bound">e</a><a id="3894" class="Symbol">)</a>
      <a id="3902" class="Symbol">(</a> <a id="3904" href="foundation-core.equivalences.html#1862" class="Function">is-equiv-map-equiv</a> <a id="3923" href="foundation.universal-property-truncation.html#3839" class="Bound">e</a><a id="3924" class="Symbol">)</a>
      <a id="3932" class="Symbol">(</a> <a id="3934" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3954" href="foundation.universal-property-truncation.html#3841" class="Bound">C</a><a id="3955" class="Symbol">)</a>
</pre>
### A map into a truncated type is a truncation if and only if it satisfies the universal property of the truncation

<pre class="Agda"><a id="4088" class="Keyword">module</a> <a id="4095" href="foundation.universal-property-truncation.html#4095" class="Module">_</a>
  <a id="4099" class="Symbol">{</a><a id="4100" href="foundation.universal-property-truncation.html#4100" class="Bound">l1</a> <a id="4103" href="foundation.universal-property-truncation.html#4103" class="Bound">l2</a> <a id="4106" class="Symbol">:</a> <a id="4108" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4113" class="Symbol">}</a> <a id="4115" class="Symbol">{</a><a id="4116" href="foundation.universal-property-truncation.html#4116" class="Bound">k</a> <a id="4118" class="Symbol">:</a> <a id="4120" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="4121" class="Symbol">}</a> <a id="4123" class="Symbol">{</a><a id="4124" href="foundation.universal-property-truncation.html#4124" class="Bound">A</a> <a id="4126" class="Symbol">:</a> <a id="4128" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="4131" href="foundation.universal-property-truncation.html#4100" class="Bound">l1</a><a id="4133" class="Symbol">}</a> <a id="4135" class="Symbol">(</a><a id="4136" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="4138" class="Symbol">:</a> <a id="4140" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="4158" href="foundation.universal-property-truncation.html#4103" class="Bound">l2</a> <a id="4161" href="foundation.universal-property-truncation.html#4116" class="Bound">k</a><a id="4162" class="Symbol">)</a>
  <a id="4166" class="Symbol">(</a><a id="4167" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a> <a id="4169" class="Symbol">:</a> <a id="4171" href="foundation.universal-property-truncation.html#4124" class="Bound">A</a> <a id="4173" class="Symbol">→</a> <a id="4175" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4195" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a><a id="4196" class="Symbol">)</a>
  <a id="4200" class="Keyword">where</a>

  <a id="4209" class="Keyword">abstract</a>
    <a id="4222" href="foundation.universal-property-truncation.html#4222" class="Function">is-truncation-universal-property-truncation</a> <a id="4266" class="Symbol">:</a>
      <a id="4274" class="Symbol">({</a><a id="4276" href="foundation.universal-property-truncation.html#4276" class="Bound">l</a> <a id="4278" class="Symbol">:</a> <a id="4280" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4285" class="Symbol">}</a> <a id="4287" class="Symbol">→</a> <a id="4289" href="foundation.universal-property-truncation.html#2305" class="Function">universal-property-truncation</a> <a id="4319" href="foundation.universal-property-truncation.html#4276" class="Bound">l</a> <a id="4321" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="4323" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="4324" class="Symbol">)</a> <a id="4326" class="Symbol">→</a>
      <a id="4334" class="Symbol">({</a><a id="4336" href="foundation.universal-property-truncation.html#4336" class="Bound">l</a> <a id="4338" class="Symbol">:</a> <a id="4340" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4345" class="Symbol">}</a> <a id="4347" class="Symbol">→</a> <a id="4349" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="4363" href="foundation.universal-property-truncation.html#4336" class="Bound">l</a> <a id="4365" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="4367" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="4368" class="Symbol">)</a>
    <a id="4374" href="foundation.universal-property-truncation.html#4222" class="Function">is-truncation-universal-property-truncation</a> <a id="4418" href="foundation.universal-property-truncation.html#4418" class="Bound">H</a> <a id="4420" href="foundation.universal-property-truncation.html#4420" class="Bound">C</a> <a id="4422" class="Symbol">=</a>
      <a id="4430" href="foundation-core.contractible-maps.html#2368" class="Function">is-equiv-is-contr-map</a>
        <a id="4460" class="Symbol">(</a> <a id="4462" class="Symbol">λ</a> <a id="4464" href="foundation.universal-property-truncation.html#4464" class="Bound">g</a> <a id="4466" class="Symbol">→</a>
          <a id="4478" href="foundation-core.contractible-types.html#3230" class="Function">is-contr-equiv</a>
            <a id="4505" class="Symbol">(</a> <a id="4507" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="4509" class="Symbol">(</a><a id="4510" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="4534" href="foundation.universal-property-truncation.html#4116" class="Bound">k</a> <a id="4536" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="4538" href="foundation.universal-property-truncation.html#4420" class="Bound">C</a><a id="4539" class="Symbol">)</a> <a id="4541" class="Symbol">(λ</a> <a id="4544" href="foundation.universal-property-truncation.html#4544" class="Bound">h</a> <a id="4546" class="Symbol">→</a> <a id="4548" class="Symbol">(</a><a id="4549" href="foundation.universal-property-truncation.html#4544" class="Bound">h</a> <a id="4551" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="4553" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="4554" class="Symbol">)</a> <a id="4556" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="4558" href="foundation.universal-property-truncation.html#4464" class="Bound">g</a><a id="4559" class="Symbol">))</a>
            <a id="4574" class="Symbol">(</a> <a id="4576" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a> <a id="4586" class="Symbol">(λ</a> <a id="4589" href="foundation.universal-property-truncation.html#4589" class="Bound">h</a> <a id="4591" class="Symbol">→</a> <a id="4593" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="4605" class="Symbol">))</a>
            <a id="4620" class="Symbol">(</a> <a id="4622" href="foundation.universal-property-truncation.html#4418" class="Bound">H</a> <a id="4624" href="foundation.universal-property-truncation.html#4420" class="Bound">C</a> <a id="4626" href="foundation.universal-property-truncation.html#4464" class="Bound">g</a><a id="4627" class="Symbol">))</a>

  <a id="4633" class="Keyword">abstract</a>
    <a id="4646" href="foundation.universal-property-truncation.html#4646" class="Function">universal-property-truncation-is-truncation</a> <a id="4690" class="Symbol">:</a>
      <a id="4698" class="Symbol">({</a><a id="4700" href="foundation.universal-property-truncation.html#4700" class="Bound">l</a> <a id="4702" class="Symbol">:</a> <a id="4704" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4709" class="Symbol">}</a> <a id="4711" class="Symbol">→</a> <a id="4713" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="4727" href="foundation.universal-property-truncation.html#4700" class="Bound">l</a> <a id="4729" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="4731" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="4732" class="Symbol">)</a> <a id="4734" class="Symbol">→</a>
      <a id="4742" class="Symbol">({</a><a id="4744" href="foundation.universal-property-truncation.html#4744" class="Bound">l</a> <a id="4746" class="Symbol">:</a> <a id="4748" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4753" class="Symbol">}</a> <a id="4755" class="Symbol">→</a> <a id="4757" href="foundation.universal-property-truncation.html#2305" class="Function">universal-property-truncation</a> <a id="4787" href="foundation.universal-property-truncation.html#4744" class="Bound">l</a> <a id="4789" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="4791" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="4792" class="Symbol">)</a>
    <a id="4798" href="foundation.universal-property-truncation.html#4646" class="Function">universal-property-truncation-is-truncation</a> <a id="4842" href="foundation.universal-property-truncation.html#4842" class="Bound">H</a> <a id="4844" href="foundation.universal-property-truncation.html#4844" class="Bound">C</a> <a id="4846" href="foundation.universal-property-truncation.html#4846" class="Bound">g</a> <a id="4848" class="Symbol">=</a>
      <a id="4856" href="foundation-core.contractible-types.html#3739" class="Function">is-contr-equiv&#39;</a>
        <a id="4880" class="Symbol">(</a> <a id="4882" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="4884" class="Symbol">(</a><a id="4885" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="4909" href="foundation.universal-property-truncation.html#4116" class="Bound">k</a> <a id="4911" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="4913" href="foundation.universal-property-truncation.html#4844" class="Bound">C</a><a id="4914" class="Symbol">)</a> <a id="4916" class="Symbol">(λ</a> <a id="4919" href="foundation.universal-property-truncation.html#4919" class="Bound">h</a> <a id="4921" class="Symbol">→</a> <a id="4923" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="4926" class="Symbol">(</a><a id="4927" href="foundation.universal-property-truncation.html#4919" class="Bound">h</a> <a id="4929" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="4931" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="4932" class="Symbol">)</a> <a id="4934" href="foundation.universal-property-truncation.html#4846" class="Bound">g</a><a id="4935" class="Symbol">))</a>
        <a id="4946" class="Symbol">(</a> <a id="4948" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a> <a id="4958" class="Symbol">(λ</a> <a id="4961" href="foundation.universal-property-truncation.html#4961" class="Bound">h</a> <a id="4963" class="Symbol">→</a> <a id="4965" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="4977" class="Symbol">))</a>
        <a id="4988" class="Symbol">(</a> <a id="4990" href="foundation-core.contractible-maps.html#3850" class="Function">is-contr-map-is-equiv</a> <a id="5012" class="Symbol">(</a><a id="5013" href="foundation.universal-property-truncation.html#4842" class="Bound">H</a> <a id="5015" href="foundation.universal-property-truncation.html#4844" class="Bound">C</a><a id="5016" class="Symbol">)</a> <a id="5018" href="foundation.universal-property-truncation.html#4846" class="Bound">g</a><a id="5019" class="Symbol">)</a>

  <a id="5024" href="foundation.universal-property-truncation.html#5024" class="Function">map-is-truncation</a> <a id="5042" class="Symbol">:</a>
    <a id="5048" class="Symbol">({</a><a id="5050" href="foundation.universal-property-truncation.html#5050" class="Bound">l</a> <a id="5052" class="Symbol">:</a> <a id="5054" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5059" class="Symbol">}</a> <a id="5061" class="Symbol">→</a> <a id="5063" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="5077" href="foundation.universal-property-truncation.html#5050" class="Bound">l</a> <a id="5079" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="5081" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="5082" class="Symbol">)</a> <a id="5084" class="Symbol">→</a>
    <a id="5090" class="Symbol">({</a><a id="5092" href="foundation.universal-property-truncation.html#5092" class="Bound">l</a> <a id="5094" class="Symbol">:</a> <a id="5096" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5101" class="Symbol">}</a> <a id="5103" class="Symbol">(</a><a id="5104" href="foundation.universal-property-truncation.html#5104" class="Bound">C</a> <a id="5106" class="Symbol">:</a> <a id="5108" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="5126" href="foundation.universal-property-truncation.html#5092" class="Bound">l</a> <a id="5128" href="foundation.universal-property-truncation.html#4116" class="Bound">k</a><a id="5129" class="Symbol">)</a> <a id="5131" class="Symbol">(</a><a id="5132" href="foundation.universal-property-truncation.html#5132" class="Bound">g</a> <a id="5134" class="Symbol">:</a> <a id="5136" href="foundation.universal-property-truncation.html#4124" class="Bound">A</a> <a id="5138" class="Symbol">→</a> <a id="5140" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="5160" href="foundation.universal-property-truncation.html#5104" class="Bound">C</a><a id="5161" class="Symbol">)</a> <a id="5163" class="Symbol">→</a>
    <a id="5169" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="5193" href="foundation.universal-property-truncation.html#4116" class="Bound">k</a> <a id="5195" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="5197" href="foundation.universal-property-truncation.html#5104" class="Bound">C</a><a id="5198" class="Symbol">)</a>
  <a id="5202" href="foundation.universal-property-truncation.html#5024" class="Function">map-is-truncation</a> <a id="5220" href="foundation.universal-property-truncation.html#5220" class="Bound">H</a> <a id="5222" href="foundation.universal-property-truncation.html#5222" class="Bound">C</a> <a id="5224" href="foundation.universal-property-truncation.html#5224" class="Bound">g</a> <a id="5226" class="Symbol">=</a>
    <a id="5232" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="5236" class="Symbol">(</a><a id="5237" href="foundation-core.contractible-types.html#1018" class="Function">center</a> <a id="5244" class="Symbol">(</a><a id="5245" href="foundation.universal-property-truncation.html#4646" class="Function">universal-property-truncation-is-truncation</a> <a id="5289" href="foundation.universal-property-truncation.html#5220" class="Bound">H</a> <a id="5291" href="foundation.universal-property-truncation.html#5222" class="Bound">C</a> <a id="5293" href="foundation.universal-property-truncation.html#5224" class="Bound">g</a><a id="5294" class="Symbol">))</a>

  <a id="5300" href="foundation.universal-property-truncation.html#5300" class="Function">triangle-is-truncation</a> <a id="5323" class="Symbol">:</a>
    <a id="5329" class="Symbol">(</a><a id="5330" href="foundation.universal-property-truncation.html#5330" class="Bound">H</a> <a id="5332" class="Symbol">:</a> <a id="5334" class="Symbol">{</a><a id="5335" href="foundation.universal-property-truncation.html#5335" class="Bound">l</a> <a id="5337" class="Symbol">:</a> <a id="5339" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5344" class="Symbol">}</a> <a id="5346" class="Symbol">→</a> <a id="5348" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="5362" href="foundation.universal-property-truncation.html#5335" class="Bound">l</a> <a id="5364" href="foundation.universal-property-truncation.html#4136" class="Bound">B</a> <a id="5366" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="5367" class="Symbol">)</a> <a id="5369" class="Symbol">→</a>
    <a id="5375" class="Symbol">{</a><a id="5376" href="foundation.universal-property-truncation.html#5376" class="Bound">l</a> <a id="5378" class="Symbol">:</a> <a id="5380" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5385" class="Symbol">}</a> <a id="5387" class="Symbol">(</a><a id="5388" href="foundation.universal-property-truncation.html#5388" class="Bound">C</a> <a id="5390" class="Symbol">:</a> <a id="5392" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="5410" href="foundation.universal-property-truncation.html#5376" class="Bound">l</a> <a id="5412" href="foundation.universal-property-truncation.html#4116" class="Bound">k</a><a id="5413" class="Symbol">)</a> <a id="5415" class="Symbol">(</a><a id="5416" href="foundation.universal-property-truncation.html#5416" class="Bound">g</a> <a id="5418" class="Symbol">:</a> <a id="5420" href="foundation.universal-property-truncation.html#4124" class="Bound">A</a> <a id="5422" class="Symbol">→</a> <a id="5424" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="5444" href="foundation.universal-property-truncation.html#5388" class="Bound">C</a><a id="5445" class="Symbol">)</a> <a id="5447" class="Symbol">→</a>
    <a id="5453" class="Symbol">(</a><a id="5454" href="foundation.universal-property-truncation.html#5024" class="Function">map-is-truncation</a> <a id="5472" href="foundation.universal-property-truncation.html#5330" class="Bound">H</a> <a id="5474" href="foundation.universal-property-truncation.html#5388" class="Bound">C</a> <a id="5476" href="foundation.universal-property-truncation.html#5416" class="Bound">g</a> <a id="5478" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="5480" href="foundation.universal-property-truncation.html#4167" class="Bound">f</a><a id="5481" class="Symbol">)</a> <a id="5483" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="5485" href="foundation.universal-property-truncation.html#5416" class="Bound">g</a>
  <a id="5489" href="foundation.universal-property-truncation.html#5300" class="Function">triangle-is-truncation</a> <a id="5512" href="foundation.universal-property-truncation.html#5512" class="Bound">H</a> <a id="5514" href="foundation.universal-property-truncation.html#5514" class="Bound">C</a> <a id="5516" href="foundation.universal-property-truncation.html#5516" class="Bound">g</a> <a id="5518" class="Symbol">=</a>
    <a id="5524" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="5528" class="Symbol">(</a><a id="5529" href="foundation-core.contractible-types.html#1018" class="Function">center</a> <a id="5536" class="Symbol">(</a><a id="5537" href="foundation.universal-property-truncation.html#4646" class="Function">universal-property-truncation-is-truncation</a> <a id="5581" href="foundation.universal-property-truncation.html#5512" class="Bound">H</a> <a id="5583" href="foundation.universal-property-truncation.html#5514" class="Bound">C</a> <a id="5585" href="foundation.universal-property-truncation.html#5516" class="Bound">g</a><a id="5586" class="Symbol">))</a>
</pre>
### A map into a truncated type is a truncation if and only if it satisfies the dependent universal property of the truncation

<pre class="Agda"><a id="5730" class="Keyword">module</a> <a id="5737" href="foundation.universal-property-truncation.html#5737" class="Module">_</a>
  <a id="5741" class="Symbol">{</a><a id="5742" href="foundation.universal-property-truncation.html#5742" class="Bound">l1</a> <a id="5745" href="foundation.universal-property-truncation.html#5745" class="Bound">l2</a> <a id="5748" class="Symbol">:</a> <a id="5750" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5755" class="Symbol">}</a> <a id="5757" class="Symbol">{</a><a id="5758" href="foundation.universal-property-truncation.html#5758" class="Bound">k</a> <a id="5760" class="Symbol">:</a> <a id="5762" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="5763" class="Symbol">}</a> <a id="5765" class="Symbol">{</a><a id="5766" href="foundation.universal-property-truncation.html#5766" class="Bound">A</a> <a id="5768" class="Symbol">:</a> <a id="5770" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="5773" href="foundation.universal-property-truncation.html#5742" class="Bound">l1</a><a id="5775" class="Symbol">}</a> <a id="5777" class="Symbol">(</a><a id="5778" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="5780" class="Symbol">:</a> <a id="5782" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="5800" href="foundation.universal-property-truncation.html#5745" class="Bound">l2</a> <a id="5803" href="foundation.universal-property-truncation.html#5758" class="Bound">k</a><a id="5804" class="Symbol">)</a>
  <a id="5808" class="Symbol">(</a><a id="5809" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a> <a id="5811" class="Symbol">:</a> <a id="5813" href="foundation.universal-property-truncation.html#5766" class="Bound">A</a> <a id="5815" class="Symbol">→</a> <a id="5817" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="5837" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a><a id="5838" class="Symbol">)</a>
  <a id="5842" class="Keyword">where</a>

  <a id="5851" class="Keyword">abstract</a>
    <a id="5864" href="foundation.universal-property-truncation.html#5864" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="5918" class="Symbol">:</a>
      <a id="5926" class="Symbol">({</a><a id="5928" href="foundation.universal-property-truncation.html#5928" class="Bound">l</a> <a id="5930" class="Symbol">:</a> <a id="5932" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5937" class="Symbol">}</a> <a id="5939" class="Symbol">→</a> <a id="5941" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="5955" href="foundation.universal-property-truncation.html#5928" class="Bound">l</a> <a id="5957" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="5959" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a><a id="5960" class="Symbol">)</a> <a id="5962" class="Symbol">→</a>
      <a id="5970" class="Symbol">{</a><a id="5971" href="foundation.universal-property-truncation.html#5971" class="Bound">l</a> <a id="5973" class="Symbol">:</a> <a id="5975" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5980" class="Symbol">}</a> <a id="5982" class="Symbol">→</a> <a id="5984" href="foundation.universal-property-truncation.html#2978" class="Function">dependent-universal-property-truncation</a> <a id="6024" href="foundation.universal-property-truncation.html#5971" class="Bound">l</a> <a id="6026" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="6028" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a>
    <a id="6034" href="foundation.universal-property-truncation.html#5864" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="6088" href="foundation.universal-property-truncation.html#6088" class="Bound">H</a> <a id="6090" href="foundation.universal-property-truncation.html#6090" class="Bound">X</a> <a id="6092" class="Symbol">=</a>
      <a id="6100" href="foundation-core.functoriality-dependent-pair-types.html#10750" class="Function">is-fiberwise-equiv-is-equiv-map-Σ</a>
        <a id="6142" class="Symbol">(</a> <a id="6144" class="Symbol">λ</a> <a id="6146" class="Symbol">(</a><a id="6147" href="foundation.universal-property-truncation.html#6147" class="Bound">h</a> <a id="6149" class="Symbol">:</a> <a id="6151" href="foundation.universal-property-truncation.html#5766" class="Bound">A</a> <a id="6153" class="Symbol">→</a> <a id="6155" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="6175" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a><a id="6176" class="Symbol">)</a> <a id="6178" class="Symbol">→</a>
          <a id="6190" class="Symbol">(</a><a id="6191" href="foundation.universal-property-truncation.html#6191" class="Bound">a</a> <a id="6193" class="Symbol">:</a> <a id="6195" href="foundation.universal-property-truncation.html#5766" class="Bound">A</a><a id="6196" class="Symbol">)</a> <a id="6198" class="Symbol">→</a> <a id="6200" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="6220" class="Symbol">(</a><a id="6221" href="foundation.universal-property-truncation.html#6090" class="Bound">X</a> <a id="6223" class="Symbol">(</a><a id="6224" href="foundation.universal-property-truncation.html#6147" class="Bound">h</a> <a id="6226" href="foundation.universal-property-truncation.html#6191" class="Bound">a</a><a id="6227" class="Symbol">)))</a>
        <a id="6239" class="Symbol">(</a> <a id="6241" class="Symbol">λ</a> <a id="6243" class="Symbol">(</a><a id="6244" href="foundation.universal-property-truncation.html#6244" class="Bound">g</a> <a id="6246" class="Symbol">:</a> <a id="6248" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="6268" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="6270" class="Symbol">→</a> <a id="6272" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="6292" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a><a id="6293" class="Symbol">)</a> <a id="6295" class="Symbol">→</a> <a id="6297" href="foundation.universal-property-truncation.html#6244" class="Bound">g</a> <a id="6299" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="6301" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a><a id="6302" class="Symbol">)</a>
        <a id="6312" class="Symbol">(</a> <a id="6314" class="Symbol">λ</a> <a id="6316" href="foundation.universal-property-truncation.html#6316" class="Bound">g</a> <a id="6318" class="Symbol">(</a><a id="6319" href="foundation.universal-property-truncation.html#6319" class="Bound">s</a> <a id="6321" class="Symbol">:</a> <a id="6323" class="Symbol">(</a><a id="6324" href="foundation.universal-property-truncation.html#6324" class="Bound">b</a> <a id="6326" class="Symbol">:</a> <a id="6328" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="6348" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a><a id="6349" class="Symbol">)</a> <a id="6351" class="Symbol">→</a>
          <a id="6363" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="6383" class="Symbol">(</a><a id="6384" href="foundation.universal-property-truncation.html#6090" class="Bound">X</a> <a id="6386" class="Symbol">(</a><a id="6387" href="foundation.universal-property-truncation.html#6316" class="Bound">g</a> <a id="6389" href="foundation.universal-property-truncation.html#6324" class="Bound">b</a><a id="6390" class="Symbol">)))</a> <a id="6394" class="Symbol">(</a><a id="6395" href="foundation.universal-property-truncation.html#6395" class="Bound">a</a> <a id="6397" class="Symbol">:</a> <a id="6399" href="foundation.universal-property-truncation.html#5766" class="Bound">A</a><a id="6400" class="Symbol">)</a> <a id="6402" class="Symbol">→</a> <a id="6404" href="foundation.universal-property-truncation.html#6319" class="Bound">s</a> <a id="6406" class="Symbol">(</a><a id="6407" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a> <a id="6409" href="foundation.universal-property-truncation.html#6395" class="Bound">a</a><a id="6410" class="Symbol">))</a>
        <a id="6421" class="Symbol">(</a> <a id="6423" href="foundation.universal-property-truncation.html#6088" class="Bound">H</a> <a id="6425" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a><a id="6426" class="Symbol">)</a>
        <a id="6436" class="Symbol">(</a> <a id="6438" href="foundation-core.equivalences.html#12773" class="Function">is-equiv-equiv</a>
          <a id="6463" class="Symbol">(</a> <a id="6465" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="6485" class="Symbol">)</a>
          <a id="6497" class="Symbol">(</a> <a id="6499" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="6519" class="Symbol">)</a>
          <a id="6531" class="Symbol">(</a> <a id="6533" href="foundation-core.dependent-pair-types.html#687" class="Function">ind-Σ</a> <a id="6539" class="Symbol">(λ</a> <a id="6542" href="foundation.universal-property-truncation.html#6542" class="Bound">g</a> <a id="6544" href="foundation.universal-property-truncation.html#6544" class="Bound">s</a> <a id="6546" class="Symbol">→</a> <a id="6548" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="6552" class="Symbol">))</a>
          <a id="6565" class="Symbol">(</a> <a id="6567" href="foundation.universal-property-truncation.html#6088" class="Bound">H</a> <a id="6569" class="Symbol">(</a><a id="6570" href="foundation-core.truncated-types.html#6052" class="Function">Σ-Truncated-Type</a> <a id="6587" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="6589" href="foundation.universal-property-truncation.html#6090" class="Bound">X</a><a id="6590" class="Symbol">)))</a>
        <a id="6602" class="Symbol">(</a> <a id="6604" href="foundation-core.functions.html#309" class="Function">id</a><a id="6606" class="Symbol">)</a>

  <a id="6611" class="Keyword">abstract</a>
    <a id="6624" href="foundation.universal-property-truncation.html#6624" class="Function">is-truncation-dependent-universal-property-truncation</a> <a id="6678" class="Symbol">:</a>
      <a id="6686" class="Symbol">({</a><a id="6688" href="foundation.universal-property-truncation.html#6688" class="Bound">l</a> <a id="6690" class="Symbol">:</a> <a id="6692" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6697" class="Symbol">}</a> <a id="6699" class="Symbol">→</a> <a id="6701" href="foundation.universal-property-truncation.html#2978" class="Function">dependent-universal-property-truncation</a> <a id="6741" href="foundation.universal-property-truncation.html#6688" class="Bound">l</a> <a id="6743" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="6745" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a><a id="6746" class="Symbol">)</a> <a id="6748" class="Symbol">→</a>
      <a id="6756" class="Symbol">{</a><a id="6757" href="foundation.universal-property-truncation.html#6757" class="Bound">l</a> <a id="6759" class="Symbol">:</a> <a id="6761" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6766" class="Symbol">}</a> <a id="6768" class="Symbol">→</a> <a id="6770" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="6784" href="foundation.universal-property-truncation.html#6757" class="Bound">l</a> <a id="6786" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="6788" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a>
    <a id="6794" href="foundation.universal-property-truncation.html#6624" class="Function">is-truncation-dependent-universal-property-truncation</a> <a id="6848" href="foundation.universal-property-truncation.html#6848" class="Bound">H</a> <a id="6850" href="foundation.universal-property-truncation.html#6850" class="Bound">X</a> <a id="6852" class="Symbol">=</a>
      <a id="6860" href="foundation.universal-property-truncation.html#6848" class="Bound">H</a> <a id="6862" class="Symbol">(λ</a> <a id="6865" href="foundation.universal-property-truncation.html#6865" class="Bound">b</a> <a id="6867" class="Symbol">→</a> <a id="6869" href="foundation.universal-property-truncation.html#6850" class="Bound">X</a><a id="6870" class="Symbol">)</a>

  <a id="6875" href="foundation.universal-property-truncation.html#6875" class="Function">sec-is-truncation</a> <a id="6893" class="Symbol">:</a>
    <a id="6899" class="Symbol">({</a><a id="6901" href="foundation.universal-property-truncation.html#6901" class="Bound">l</a> <a id="6903" class="Symbol">:</a> <a id="6905" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6910" class="Symbol">}</a> <a id="6912" class="Symbol">→</a> <a id="6914" href="foundation.universal-property-truncation.html#2009" class="Function">is-truncation</a> <a id="6928" href="foundation.universal-property-truncation.html#6901" class="Bound">l</a> <a id="6930" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="6932" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a><a id="6933" class="Symbol">)</a> <a id="6935" class="Symbol">→</a>
    <a id="6941" class="Symbol">{</a><a id="6942" href="foundation.universal-property-truncation.html#6942" class="Bound">l3</a> <a id="6945" class="Symbol">:</a> <a id="6947" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6952" class="Symbol">}</a> <a id="6954" class="Symbol">(</a><a id="6955" href="foundation.universal-property-truncation.html#6955" class="Bound">C</a> <a id="6957" class="Symbol">:</a> <a id="6959" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="6977" href="foundation.universal-property-truncation.html#6942" class="Bound">l3</a> <a id="6980" href="foundation.universal-property-truncation.html#5758" class="Bound">k</a><a id="6981" class="Symbol">)</a>
    <a id="6987" class="Symbol">(</a><a id="6988" href="foundation.universal-property-truncation.html#6988" class="Bound">h</a> <a id="6990" class="Symbol">:</a> <a id="6992" href="foundation.universal-property-truncation.html#5766" class="Bound">A</a> <a id="6994" class="Symbol">→</a> <a id="6996" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="7016" href="foundation.universal-property-truncation.html#6955" class="Bound">C</a><a id="7017" class="Symbol">)</a> <a id="7019" class="Symbol">(</a><a id="7020" href="foundation.universal-property-truncation.html#7020" class="Bound">g</a> <a id="7022" class="Symbol">:</a> <a id="7024" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="7048" href="foundation.universal-property-truncation.html#5758" class="Bound">k</a> <a id="7050" href="foundation.universal-property-truncation.html#6955" class="Bound">C</a> <a id="7052" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a><a id="7053" class="Symbol">)</a> <a id="7055" class="Symbol">→</a>
    <a id="7061" href="foundation.universal-property-truncation.html#5809" class="Bound">f</a> <a id="7063" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="7065" class="Symbol">(</a><a id="7066" href="foundation.universal-property-truncation.html#7020" class="Bound">g</a> <a id="7068" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="7070" href="foundation.universal-property-truncation.html#6988" class="Bound">h</a><a id="7071" class="Symbol">)</a> <a id="7073" class="Symbol">→</a> <a id="7075" href="foundation-core.sections.html#521" class="Function">sec</a> <a id="7079" href="foundation.universal-property-truncation.html#7020" class="Bound">g</a>
  <a id="7083" href="foundation.universal-property-truncation.html#6875" class="Function">sec-is-truncation</a> <a id="7101" href="foundation.universal-property-truncation.html#7101" class="Bound">H</a> <a id="7103" href="foundation.universal-property-truncation.html#7103" class="Bound">C</a> <a id="7105" href="foundation.universal-property-truncation.html#7105" class="Bound">h</a> <a id="7107" href="foundation.universal-property-truncation.html#7107" class="Bound">g</a> <a id="7109" href="foundation.universal-property-truncation.html#7109" class="Bound">K</a> <a id="7111" class="Symbol">=</a>
    <a id="7117" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#2808" class="Function">map-distributive-Π-Σ</a>
      <a id="7144" class="Symbol">(</a> <a id="7146" href="foundation-core.equivalences.html#4173" class="Function">map-inv-is-equiv</a>
        <a id="7171" class="Symbol">(</a> <a id="7173" href="foundation.universal-property-truncation.html#5864" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="7227" href="foundation.universal-property-truncation.html#7101" class="Bound">H</a>
          <a id="7239" class="Symbol">(</a> <a id="7241" href="foundation-core.truncated-types.html#6435" class="Function">fib-Truncated-Type</a> <a id="7260" href="foundation.universal-property-truncation.html#7103" class="Bound">C</a> <a id="7262" href="foundation.universal-property-truncation.html#5778" class="Bound">B</a> <a id="7264" href="foundation.universal-property-truncation.html#7107" class="Bound">g</a><a id="7265" class="Symbol">))</a>
        <a id="7276" class="Symbol">(</a> <a id="7278" class="Symbol">λ</a> <a id="7280" href="foundation.universal-property-truncation.html#7280" class="Bound">a</a> <a id="7282" class="Symbol">→</a> <a id="7284" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="7289" class="Symbol">(</a><a id="7290" href="foundation.universal-property-truncation.html#7105" class="Bound">h</a> <a id="7292" href="foundation.universal-property-truncation.html#7280" class="Bound">a</a><a id="7293" class="Symbol">)</a> <a id="7295" class="Symbol">(</a><a id="7296" href="foundation-core.identity-types.html#1552" class="Function">inv</a> <a id="7300" class="Symbol">(</a><a id="7301" href="foundation.universal-property-truncation.html#7109" class="Bound">K</a> <a id="7303" href="foundation.universal-property-truncation.html#7280" class="Bound">a</a><a id="7304" class="Symbol">))))</a>
</pre>
## To do

<pre class="Agda">
<a id="7333" class="Comment">{-

-- Theorem 18.5.2 Condition (iii)

mere-eq-Eq-Rel : {l1 : Level} (A : UU l1) → Eq-Rel l1 A
mere-eq-Eq-Rel A =
  pair
    mere-eq-Prop
    ( pair refl-mere-eq (pair symm-mere-eq trans-mere-eq))

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

-- We postulate the existence of set truncations

postulate type-trunc-Set : {l : Level} → UU l → UU l

postulate
  is-set-type-trunc-Set : {l : Level} {A : UU l} → is-set (type-trunc-Set A)

trunc-Set : {l : Level} → UU l → UU-Set l
trunc-Set A = pair (type-trunc-Set A) is-set-type-trunc-Set

postulate unit-trunc-Set : {l : Level} {A : UU l} → A → type-Set (trunc-Set A)

postulate
  is-set-truncation-trunc-Set :
    {l1 l2 : Level} (A : UU l1) →
    is-set-truncation l2 (trunc-Set A) unit-trunc-Set

equiv-universal-property-trunc-Set :
  {l1 l2 : Level} (A : UU l1) (B : UU-Set l2) →
  (type-trunc-Set A → type-Set B) ≃ (A → type-Set B)
equiv-universal-property-trunc-Set A B =
  pair
    ( precomp-Set unit-trunc-Set B)
    ( is-set-truncation-trunc-Set A B)

abstract
  universal-property-trunc-Set : {l1 l2 : Level} (A : UU l1) →
    universal-property-set-truncation l2
      ( trunc-Set A)
      ( unit-trunc-Set)
  universal-property-trunc-Set A =
    universal-property-is-set-truncation _
      ( trunc-Set A)
      ( unit-trunc-Set)
      ( is-set-truncation-trunc-Set A)

map-universal-property-trunc-Set :
  {l1 l2 : Level} {A : UU l1} (B : UU-Set l2) →
  (A → type-Set B) → type-hom-Set (trunc-Set A) B
map-universal-property-trunc-Set {A = A} B f =
  map-is-set-truncation
    ( trunc-Set A)
    ( unit-trunc-Set)
    ( is-set-truncation-trunc-Set A)
    ( B)
    ( f)

triangle-universal-property-trunc-Set :
  {l1 l2 : Level} {A : UU l1} (B : UU-Set l2) →
  (f : A → type-Set B) →
  (map-universal-property-trunc-Set B f ∘ unit-trunc-Set) ~ f
triangle-universal-property-trunc-Set {A = A} B f =
  triangle-is-set-truncation
    ( trunc-Set A)
    ( unit-trunc-Set)
    ( is-set-truncation-trunc-Set A)
    ( B)
    ( f)

apply-universal-property-trunc-Set :
  {l1 l2 : Level} {A : UU l1} (t : type-trunc-Set A) (B : UU-Set l2) →
  (A → type-Set B) → type-Set B
apply-universal-property-trunc-Set t B f =
  map-universal-property-trunc-Set B f t

abstract
  dependent-universal-property-trunc-Set :
    {l1 l2 : Level} {A : UU l1} (B : type-trunc-Set A → UU-Set l2) → 
    is-equiv (precomp-Π-Set unit-trunc-Set B)
  dependent-universal-property-trunc-Set {A = A} =
    dependent-universal-property-is-set-truncation
      ( trunc-Set A)
      ( unit-trunc-Set)
      ( λ {l} → is-set-truncation-trunc-Set A)

equiv-dependent-universal-property-trunc-Set :
  {l1 l2 : Level} {A : UU l1} (B : type-trunc-Set A → UU-Set l2) →
  ((x : type-trunc-Set A) → type-Set (B x)) ≃
  ((a : A) → type-Set (B (unit-trunc-Set a)))
equiv-dependent-universal-property-trunc-Set B =
  pair ( precomp-Π-Set unit-trunc-Set B)
       ( dependent-universal-property-trunc-Set B)

apply-dependent-universal-property-trunc-Set :
  {l1 l2 : Level} {A : UU l1}
  (B : type-trunc-Set A → UU-Set l2) →
  ((x : A) → type-Set (B (unit-trunc-Set x))) →
  (x : type-trunc-Set A) → type-Set (B x)
apply-dependent-universal-property-trunc-Set B =
  map-inv-equiv (equiv-dependent-universal-property-trunc-Set B)

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