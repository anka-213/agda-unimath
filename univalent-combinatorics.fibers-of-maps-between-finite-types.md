# Fibers of maps between finite types

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html" class="Module">univalent-combinatorics.fibers-of-maps-between-finite-types</a> <a id="158" class="Keyword">where</a>

<a id="165" class="Keyword">open</a> <a id="170" class="Keyword">import</a> <a id="177" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a> <a id="207" class="Keyword">using</a> <a id="213" class="Symbol">(</a><a id="214" href="foundation-core.contractible-types.html#2189" class="Function">is-contr-total-path&#39;</a><a id="234" class="Symbol">)</a>
<a id="236" class="Keyword">open</a> <a id="241" class="Keyword">import</a> <a id="248" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="280" class="Keyword">using</a> <a id="286" class="Symbol">(</a><a id="287" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="288" class="Symbol">;</a> <a id="290" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="294" class="Symbol">;</a> <a id="296" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="299" class="Symbol">;</a> <a id="301" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="304" class="Symbol">)</a>
<a id="306" class="Keyword">open</a> <a id="311" class="Keyword">import</a> <a id="318" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a> <a id="359" class="Keyword">using</a>
  <a id="367" class="Symbol">(</a> <a id="369" href="foundation.equality-dependent-pair-types.html#2407" class="Function">equiv-pair-eq-Σ</a><a id="384" class="Symbol">)</a>
<a id="386" class="Keyword">open</a> <a id="391" class="Keyword">import</a> <a id="398" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="422" class="Keyword">using</a> <a id="428" class="Symbol">(</a><a id="429" href="foundation-core.equivalences.html#7843" class="Function Operator">_∘e_</a><a id="433" class="Symbol">)</a>
<a id="435" class="Keyword">open</a> <a id="440" class="Keyword">import</a> <a id="447" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a> <a id="473" class="Keyword">using</a> <a id="479" class="Symbol">(</a><a id="480" href="foundation-core.fibers-of-maps.html#928" class="Function">fib</a><a id="483" class="Symbol">)</a>
<a id="485" class="Keyword">open</a> <a id="490" class="Keyword">import</a> <a id="497" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a> <a id="543" class="Keyword">using</a> <a id="549" class="Symbol">(</a><a id="550" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a><a id="559" class="Symbol">)</a>
<a id="561" class="Keyword">open</a> <a id="566" class="Keyword">import</a> <a id="573" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="599" class="Keyword">using</a> <a id="605" class="Symbol">(</a><a id="606" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="608" class="Symbol">;</a> <a id="610" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="614" class="Symbol">;</a> <a id="616" href="foundation-core.identity-types.html#4584" class="Function">tr</a><a id="618" class="Symbol">)</a>
<a id="620" class="Keyword">open</a> <a id="625" class="Keyword">import</a> <a id="632" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a> <a id="669" class="Keyword">using</a>
  <a id="677" class="Symbol">(</a> <a id="679" href="foundation.propositional-truncations.html#5148" class="Function">apply-universal-property-trunc-Prop</a><a id="714" class="Symbol">;</a> <a id="716" href="foundation.propositional-truncations.html#1756" class="Postulate">unit-trunc-Prop</a><a id="731" class="Symbol">)</a>
<a id="733" class="Keyword">open</a> <a id="738" class="Keyword">import</a> <a id="745" href="foundation.sections.html" class="Module">foundation.sections</a> <a id="765" class="Keyword">using</a> <a id="771" class="Symbol">(</a><a id="772" href="foundation.sections.html#1762" class="Function">map-section</a><a id="783" class="Symbol">)</a>
<a id="785" class="Keyword">open</a> <a id="790" class="Keyword">import</a> <a id="797" href="foundation.type-arithmetic-dependent-pair-types.html" class="Module">foundation.type-arithmetic-dependent-pair-types</a> <a id="845" class="Keyword">using</a>
  <a id="853" class="Symbol">(</a> <a id="855" href="foundation-core.type-arithmetic-dependent-pair-types.html#3077" class="Function">left-unit-law-Σ-is-contr</a><a id="879" class="Symbol">;</a> <a id="881" href="foundation-core.type-arithmetic-dependent-pair-types.html#5795" class="Function">inv-assoc-Σ</a><a id="892" class="Symbol">)</a>
<a id="894" class="Keyword">open</a> <a id="899" class="Keyword">import</a> <a id="906" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="933" class="Keyword">using</a> <a id="939" class="Symbol">(</a><a id="940" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="945" class="Symbol">;</a> <a id="947" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="949" class="Symbol">;</a> <a id="951" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="954" class="Symbol">)</a>

<a id="957" class="Keyword">open</a> <a id="962" class="Keyword">import</a> <a id="969" href="univalent-combinatorics.counting-fibers-of-maps.html" class="Module">univalent-combinatorics.counting-fibers-of-maps</a> <a id="1017" class="Keyword">using</a>
  <a id="1025" class="Symbol">(</a> <a id="1027" href="univalent-combinatorics.counting-fibers-of-maps.html#834" class="Function">count-fib</a><a id="1036" class="Symbol">)</a>
<a id="1038" class="Keyword">open</a> <a id="1043" class="Keyword">import</a> <a id="1050" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a> <a id="1096" class="Keyword">using</a>
  <a id="1104" class="Symbol">(</a> <a id="1106" href="univalent-combinatorics.equality-finite-types.html#3302" class="Function">is-finite-eq</a><a id="1118" class="Symbol">;</a> <a id="1120" href="univalent-combinatorics.equality-finite-types.html#1960" class="Function">has-decidable-equality-is-finite</a><a id="1152" class="Symbol">)</a>
<a id="1154" class="Keyword">open</a> <a id="1159" class="Keyword">import</a> <a id="1166" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="1203" class="Keyword">using</a>
  <a id="1211" class="Symbol">(</a> <a id="1213" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a><a id="1222" class="Symbol">;</a> <a id="1224" href="univalent-combinatorics.finite-types.html#3641" class="Function">is-finite-Prop</a><a id="1238" class="Symbol">;</a> <a id="1240" href="univalent-combinatorics.finite-types.html#4123" class="Function">𝔽</a><a id="1241" class="Symbol">;</a> <a id="1243" href="univalent-combinatorics.finite-types.html#4171" class="Function">type-𝔽</a><a id="1249" class="Symbol">;</a> <a id="1251" href="univalent-combinatorics.finite-types.html#4222" class="Function">is-finite-type-𝔽</a><a id="1267" class="Symbol">;</a> <a id="1269" href="univalent-combinatorics.finite-types.html#6492" class="Function">is-finite-equiv&#39;</a><a id="1285" class="Symbol">)</a>
</pre>
## Idea

The fibers of maps between finite types are finite.

## Theorem

<pre class="Agda"><a id="1374" class="Keyword">abstract</a>
  <a id="is-finite-fib"></a><a id="1385" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1385" class="Function">is-finite-fib</a> <a id="1399" class="Symbol">:</a>
    <a id="1405" class="Symbol">{</a><a id="1406" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1406" class="Bound">l1</a> <a id="1409" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1409" class="Bound">l2</a> <a id="1412" class="Symbol">:</a> <a id="1414" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1419" class="Symbol">}</a> <a id="1421" class="Symbol">{</a><a id="1422" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1422" class="Bound">X</a> <a id="1424" class="Symbol">:</a> <a id="1426" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1429" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1406" class="Bound">l1</a><a id="1431" class="Symbol">}</a> <a id="1433" class="Symbol">{</a><a id="1434" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1434" class="Bound">Y</a> <a id="1436" class="Symbol">:</a> <a id="1438" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1441" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1409" class="Bound">l2</a><a id="1443" class="Symbol">}</a> <a id="1445" class="Symbol">(</a><a id="1446" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1446" class="Bound">f</a> <a id="1448" class="Symbol">:</a> <a id="1450" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1422" class="Bound">X</a> <a id="1452" class="Symbol">→</a> <a id="1454" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1434" class="Bound">Y</a><a id="1455" class="Symbol">)</a> <a id="1457" class="Symbol">→</a>
    <a id="1463" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="1473" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1422" class="Bound">X</a> <a id="1475" class="Symbol">→</a> <a id="1477" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="1487" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1434" class="Bound">Y</a> <a id="1489" class="Symbol">→</a> <a id="1491" class="Symbol">(</a><a id="1492" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1492" class="Bound">y</a> <a id="1494" class="Symbol">:</a> <a id="1496" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1434" class="Bound">Y</a><a id="1497" class="Symbol">)</a> <a id="1499" class="Symbol">→</a> <a id="1501" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="1511" class="Symbol">(</a><a id="1512" href="foundation-core.fibers-of-maps.html#928" class="Function">fib</a> <a id="1516" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1446" class="Bound">f</a> <a id="1518" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1492" class="Bound">y</a><a id="1519" class="Symbol">)</a>
  <a id="1523" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1385" class="Function">is-finite-fib</a> <a id="1537" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1537" class="Bound">f</a> <a id="1539" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1539" class="Bound">is-finite-X</a> <a id="1551" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1551" class="Bound">is-finite-Y</a> <a id="1563" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1563" class="Bound">y</a> <a id="1565" class="Symbol">=</a>
    <a id="1571" href="foundation.propositional-truncations.html#5148" class="Function">apply-universal-property-trunc-Prop</a>
      <a id="1613" class="Symbol">(</a> <a id="1615" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1539" class="Bound">is-finite-X</a><a id="1626" class="Symbol">)</a>
      <a id="1634" class="Symbol">(</a> <a id="1636" href="univalent-combinatorics.finite-types.html#3641" class="Function">is-finite-Prop</a> <a id="1651" class="Symbol">(</a><a id="1652" href="foundation-core.fibers-of-maps.html#928" class="Function">fib</a> <a id="1656" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1537" class="Bound">f</a> <a id="1658" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1563" class="Bound">y</a><a id="1659" class="Symbol">))</a>
      <a id="1668" class="Symbol">(</a> <a id="1670" class="Symbol">λ</a> <a id="1672" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1672" class="Bound">H</a> <a id="1674" class="Symbol">→</a>
        <a id="1684" href="foundation.propositional-truncations.html#5148" class="Function">apply-universal-property-trunc-Prop</a>
          <a id="1730" class="Symbol">(</a> <a id="1732" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1551" class="Bound">is-finite-Y</a><a id="1743" class="Symbol">)</a>
          <a id="1755" class="Symbol">(</a> <a id="1757" href="univalent-combinatorics.finite-types.html#3641" class="Function">is-finite-Prop</a> <a id="1772" class="Symbol">(</a><a id="1773" href="foundation-core.fibers-of-maps.html#928" class="Function">fib</a> <a id="1777" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1537" class="Bound">f</a> <a id="1779" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1563" class="Bound">y</a><a id="1780" class="Symbol">))</a>
          <a id="1793" class="Symbol">(</a> <a id="1795" class="Symbol">λ</a> <a id="1797" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1797" class="Bound">K</a> <a id="1799" class="Symbol">→</a> <a id="1801" href="foundation.propositional-truncations.html#1756" class="Postulate">unit-trunc-Prop</a> <a id="1817" class="Symbol">(</a><a id="1818" href="univalent-combinatorics.counting-fibers-of-maps.html#834" class="Function">count-fib</a> <a id="1828" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1537" class="Bound">f</a> <a id="1830" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1672" class="Bound">H</a> <a id="1832" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1797" class="Bound">K</a> <a id="1834" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1563" class="Bound">y</a><a id="1835" class="Symbol">)))</a>

<a id="fib-𝔽"></a><a id="1840" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1840" class="Function">fib-𝔽</a> <a id="1846" class="Symbol">:</a> <a id="1848" class="Symbol">(</a><a id="1849" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1849" class="Bound">X</a> <a id="1851" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1851" class="Bound">Y</a> <a id="1853" class="Symbol">:</a> <a id="1855" href="univalent-combinatorics.finite-types.html#4123" class="Function">𝔽</a><a id="1856" class="Symbol">)</a> <a id="1858" class="Symbol">(</a><a id="1859" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1859" class="Bound">f</a> <a id="1861" class="Symbol">:</a> <a id="1863" href="univalent-combinatorics.finite-types.html#4171" class="Function">type-𝔽</a> <a id="1870" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1849" class="Bound">X</a> <a id="1872" class="Symbol">→</a> <a id="1874" href="univalent-combinatorics.finite-types.html#4171" class="Function">type-𝔽</a> <a id="1881" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1851" class="Bound">Y</a><a id="1882" class="Symbol">)</a> <a id="1884" class="Symbol">→</a> <a id="1886" href="univalent-combinatorics.finite-types.html#4171" class="Function">type-𝔽</a> <a id="1893" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1851" class="Bound">Y</a> <a id="1895" class="Symbol">→</a> <a id="1897" href="univalent-combinatorics.finite-types.html#4123" class="Function">𝔽</a>
<a id="1899" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1903" class="Symbol">(</a><a id="1904" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1840" class="Function">fib-𝔽</a> <a id="1910" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1910" class="Bound">X</a> <a id="1912" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1912" class="Bound">Y</a> <a id="1914" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1914" class="Bound">f</a> <a id="1916" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1916" class="Bound">y</a><a id="1917" class="Symbol">)</a> <a id="1919" class="Symbol">=</a> <a id="1921" href="foundation-core.fibers-of-maps.html#928" class="Function">fib</a> <a id="1925" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1914" class="Bound">f</a> <a id="1927" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1916" class="Bound">y</a>
<a id="1929" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1933" class="Symbol">(</a><a id="1934" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1840" class="Function">fib-𝔽</a> <a id="1940" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1940" class="Bound">X</a> <a id="1942" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1942" class="Bound">Y</a> <a id="1944" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1944" class="Bound">f</a> <a id="1946" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1946" class="Bound">y</a><a id="1947" class="Symbol">)</a> <a id="1949" class="Symbol">=</a>
  <a id="1953" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1385" class="Function">is-finite-fib</a> <a id="1967" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1944" class="Bound">f</a> <a id="1969" class="Symbol">(</a><a id="1970" href="univalent-combinatorics.finite-types.html#4222" class="Function">is-finite-type-𝔽</a> <a id="1987" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1940" class="Bound">X</a><a id="1988" class="Symbol">)</a> <a id="1990" class="Symbol">(</a><a id="1991" href="univalent-combinatorics.finite-types.html#4222" class="Function">is-finite-type-𝔽</a> <a id="2008" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1942" class="Bound">Y</a><a id="2009" class="Symbol">)</a> <a id="2011" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#1946" class="Bound">y</a>
</pre>
<pre class="Agda"><a id="2026" class="Keyword">abstract</a>
  <a id="is-finite-fib-map-section"></a><a id="2037" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2037" class="Function">is-finite-fib-map-section</a> <a id="2063" class="Symbol">:</a>
    <a id="2069" class="Symbol">{</a><a id="2070" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2070" class="Bound">l1</a> <a id="2073" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2073" class="Bound">l2</a> <a id="2076" class="Symbol">:</a> <a id="2078" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2083" class="Symbol">}</a> <a id="2085" class="Symbol">{</a><a id="2086" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2086" class="Bound">A</a> <a id="2088" class="Symbol">:</a> <a id="2090" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2093" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2070" class="Bound">l1</a><a id="2095" class="Symbol">}</a> <a id="2097" class="Symbol">{</a><a id="2098" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2098" class="Bound">B</a> <a id="2100" class="Symbol">:</a> <a id="2102" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2086" class="Bound">A</a> <a id="2104" class="Symbol">→</a> <a id="2106" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2109" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2073" class="Bound">l2</a><a id="2111" class="Symbol">}</a> <a id="2113" class="Symbol">(</a><a id="2114" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2114" class="Bound">b</a> <a id="2116" class="Symbol">:</a> <a id="2118" class="Symbol">(</a><a id="2119" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2119" class="Bound">x</a> <a id="2121" class="Symbol">:</a> <a id="2123" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2086" class="Bound">A</a><a id="2124" class="Symbol">)</a> <a id="2126" class="Symbol">→</a> <a id="2128" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2098" class="Bound">B</a> <a id="2130" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2119" class="Bound">x</a><a id="2131" class="Symbol">)</a> <a id="2133" class="Symbol">→</a>
    <a id="2139" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="2149" class="Symbol">(</a><a id="2150" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="2152" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2086" class="Bound">A</a> <a id="2154" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2098" class="Bound">B</a><a id="2155" class="Symbol">)</a> <a id="2157" class="Symbol">→</a> <a id="2159" class="Symbol">((</a><a id="2161" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2161" class="Bound">x</a> <a id="2163" class="Symbol">:</a> <a id="2165" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2086" class="Bound">A</a><a id="2166" class="Symbol">)</a> <a id="2168" class="Symbol">→</a> <a id="2170" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="2180" class="Symbol">(</a><a id="2181" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2098" class="Bound">B</a> <a id="2183" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2161" class="Bound">x</a><a id="2184" class="Symbol">))</a> <a id="2187" class="Symbol">→</a>
    <a id="2193" class="Symbol">(</a><a id="2194" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2194" class="Bound">t</a> <a id="2196" class="Symbol">:</a> <a id="2198" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="2200" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2086" class="Bound">A</a> <a id="2202" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2098" class="Bound">B</a><a id="2203" class="Symbol">)</a> <a id="2205" class="Symbol">→</a> <a id="2207" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="2217" class="Symbol">(</a><a id="2218" href="foundation-core.fibers-of-maps.html#928" class="Function">fib</a> <a id="2222" class="Symbol">(</a><a id="2223" href="foundation.sections.html#1762" class="Function">map-section</a> <a id="2235" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2114" class="Bound">b</a><a id="2236" class="Symbol">)</a> <a id="2238" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2194" class="Bound">t</a><a id="2239" class="Symbol">)</a>
  <a id="2243" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2037" class="Function">is-finite-fib-map-section</a> <a id="2269" class="Symbol">{</a><a id="2270" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2270" class="Bound">l1</a><a id="2272" class="Symbol">}</a> <a id="2274" class="Symbol">{</a><a id="2275" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2275" class="Bound">l2</a><a id="2277" class="Symbol">}</a> <a id="2279" class="Symbol">{</a><a id="2280" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2280" class="Bound">A</a><a id="2281" class="Symbol">}</a> <a id="2283" class="Symbol">{</a><a id="2284" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2284" class="Bound">B</a><a id="2285" class="Symbol">}</a> <a id="2287" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2287" class="Bound">b</a> <a id="2289" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2289" class="Bound">f</a> <a id="2291" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2291" class="Bound">g</a> <a id="2293" class="Symbol">(</a><a id="2294" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2299" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2299" class="Bound">y</a> <a id="2301" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2301" class="Bound">z</a><a id="2302" class="Symbol">)</a> <a id="2304" class="Symbol">=</a>
    <a id="2310" href="univalent-combinatorics.finite-types.html#6492" class="Function">is-finite-equiv&#39;</a>
      <a id="2333" class="Symbol">(</a> <a id="2335" class="Symbol">(</a> <a id="2337" class="Symbol">(</a> <a id="2339" href="foundation-core.type-arithmetic-dependent-pair-types.html#3077" class="Function">left-unit-law-Σ-is-contr</a>
            <a id="2376" class="Symbol">(</a> <a id="2378" href="foundation-core.contractible-types.html#2189" class="Function">is-contr-total-path&#39;</a> <a id="2399" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2299" class="Bound">y</a><a id="2400" class="Symbol">)</a>
            <a id="2414" class="Symbol">(</a> <a id="2416" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2421" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2299" class="Bound">y</a> <a id="2423" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="2427" class="Symbol">))</a> <a id="2430" href="foundation-core.equivalences.html#7843" class="Function Operator">∘e</a>
          <a id="2443" class="Symbol">(</a> <a id="2445" href="foundation-core.type-arithmetic-dependent-pair-types.html#5795" class="Function">inv-assoc-Σ</a> <a id="2457" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2280" class="Bound">A</a>
            <a id="2471" class="Symbol">(</a> <a id="2473" class="Symbol">λ</a> <a id="2475" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2475" class="Bound">x</a> <a id="2477" class="Symbol">→</a> <a id="2479" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="2482" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2475" class="Bound">x</a> <a id="2484" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2299" class="Bound">y</a><a id="2485" class="Symbol">)</a>
            <a id="2499" class="Symbol">(</a> <a id="2501" class="Symbol">λ</a> <a id="2503" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2503" class="Bound">t</a> <a id="2505" class="Symbol">→</a> <a id="2507" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="2510" class="Symbol">(</a><a id="2511" href="foundation-core.identity-types.html#4584" class="Function">tr</a> <a id="2514" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2284" class="Bound">B</a> <a id="2516" class="Symbol">(</a><a id="2517" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2521" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2503" class="Bound">t</a><a id="2522" class="Symbol">)</a> <a id="2524" class="Symbol">(</a><a id="2525" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2287" class="Bound">b</a> <a id="2527" class="Symbol">(</a><a id="2528" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2532" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2503" class="Bound">t</a><a id="2533" class="Symbol">)))</a> <a id="2537" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2301" class="Bound">z</a><a id="2538" class="Symbol">)))</a> <a id="2542" href="foundation-core.equivalences.html#7843" class="Function Operator">∘e</a>
        <a id="2553" class="Symbol">(</a> <a id="2555" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a> <a id="2565" class="Symbol">(λ</a> <a id="2568" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2568" class="Bound">x</a> <a id="2570" class="Symbol">→</a> <a id="2572" href="foundation.equality-dependent-pair-types.html#2407" class="Function">equiv-pair-eq-Σ</a> <a id="2588" class="Symbol">(</a><a id="2589" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2594" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2568" class="Bound">x</a> <a id="2596" class="Symbol">(</a><a id="2597" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2287" class="Bound">b</a> <a id="2599" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2568" class="Bound">x</a><a id="2600" class="Symbol">))</a> <a id="2603" class="Symbol">(</a><a id="2604" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2609" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2299" class="Bound">y</a> <a id="2611" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2301" class="Bound">z</a><a id="2612" class="Symbol">))))</a>
      <a id="2623" class="Symbol">(</a> <a id="2625" href="univalent-combinatorics.equality-finite-types.html#3302" class="Function">is-finite-eq</a> <a id="2638" class="Symbol">(</a><a id="2639" href="univalent-combinatorics.equality-finite-types.html#1960" class="Function">has-decidable-equality-is-finite</a> <a id="2672" class="Symbol">(</a><a id="2673" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2291" class="Bound">g</a> <a id="2675" href="univalent-combinatorics.fibers-of-maps-between-finite-types.html#2299" class="Bound">y</a><a id="2676" class="Symbol">)))</a>
</pre>