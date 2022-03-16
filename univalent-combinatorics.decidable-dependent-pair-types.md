# Decidability of dependent pair types

<pre class="Agda"><a id="49" class="Symbol">{-#</a> <a id="53" class="Keyword">OPTIONS</a> <a id="61" class="Pragma">--without-K</a> <a id="73" class="Pragma">--exact-split</a> <a id="87" class="Symbol">#-}</a>

<a id="92" class="Keyword">module</a> <a id="99" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a> <a id="154" class="Keyword">where</a>

<a id="161" class="Keyword">open</a> <a id="166" class="Keyword">import</a> <a id="173" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="214" class="Keyword">using</a> <a id="220" class="Symbol">(</a><a id="221" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="222" class="Symbol">;</a> <a id="224" href="elementary-number-theory.natural-numbers.html#1465" class="InductiveConstructor">zero-ℕ</a><a id="230" class="Symbol">;</a> <a id="232" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a><a id="238" class="Symbol">)</a>

<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a> <a id="280" class="Keyword">using</a> <a id="286" class="Symbol">(</a><a id="287" href="foundation.coproduct-types.html#1168" class="Datatype">coprod</a><a id="293" class="Symbol">;</a> <a id="295" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a><a id="298" class="Symbol">;</a> <a id="300" href="foundation.coproduct-types.html#1262" class="InductiveConstructor">inr</a><a id="303" class="Symbol">)</a>
<a id="305" class="Keyword">open</a> <a id="310" class="Keyword">import</a> <a id="317" href="foundation.decidable-dependent-pair-types.html" class="Module">foundation.decidable-dependent-pair-types</a> <a id="359" class="Keyword">using</a>
  <a id="367" class="Symbol">(</a> <a id="369" href="foundation.decidable-dependent-pair-types.html#1650" class="Function">is-decidable-Σ-equiv</a><a id="389" class="Symbol">)</a>
<a id="391" class="Keyword">open</a> <a id="396" class="Keyword">import</a> <a id="403" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a> <a id="430" class="Keyword">using</a>
  <a id="438" class="Symbol">(</a> <a id="440" href="foundation.decidable-types.html#1741" class="Function">is-decidable</a><a id="452" class="Symbol">;</a> <a id="454" href="foundation.decidable-types.html#5377" class="Function">is-decidable-iff</a><a id="470" class="Symbol">)</a>
<a id="472" class="Keyword">open</a> <a id="477" class="Keyword">import</a> <a id="484" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="516" class="Keyword">using</a> <a id="522" class="Symbol">(</a><a id="523" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="524" class="Symbol">;</a> <a id="526" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="530" class="Symbol">;</a> <a id="532" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="535" class="Symbol">;</a> <a id="537" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="540" class="Symbol">)</a>
<a id="542" class="Keyword">open</a> <a id="547" class="Keyword">import</a> <a id="554" href="foundation.empty-types.html" class="Module">foundation.empty-types</a> <a id="577" class="Keyword">using</a> <a id="583" class="Symbol">(</a><a id="584" href="foundation-core.empty-types.html#1147" class="Function">ex-falso</a><a id="592" class="Symbol">)</a>
<a id="594" class="Keyword">open</a> <a id="599" class="Keyword">import</a> <a id="606" href="foundation.functions.html" class="Module">foundation.functions</a> <a id="627" class="Keyword">using</a> <a id="633" class="Symbol">(</a><a id="634" href="foundation-core.functions.html#407" class="Function Operator">_∘_</a><a id="637" class="Symbol">)</a>
<a id="639" class="Keyword">open</a> <a id="644" class="Keyword">import</a> <a id="651" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="675" class="Keyword">using</a> <a id="681" class="Symbol">(</a><a id="682" href="foundation-core.equivalences.html#2480" class="Function">id-equiv</a><a id="690" class="Symbol">)</a>
<a id="692" class="Keyword">open</a> <a id="697" class="Keyword">import</a> <a id="704" href="foundation.unit-type.html" class="Module">foundation.unit-type</a> <a id="725" class="Keyword">using</a> <a id="731" class="Symbol">(</a><a id="732" href="foundation.unit-type.html#975" class="Datatype">unit</a><a id="736" class="Symbol">;</a> <a id="738" href="foundation.unit-type.html#999" class="InductiveConstructor">star</a><a id="742" class="Symbol">)</a>
<a id="744" class="Keyword">open</a> <a id="749" class="Keyword">import</a> <a id="756" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="783" class="Keyword">using</a> <a id="789" class="Symbol">(</a><a id="790" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="795" class="Symbol">;</a> <a id="797" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="799" class="Symbol">)</a>

<a id="802" class="Keyword">open</a> <a id="807" class="Keyword">import</a> <a id="814" href="univalent-combinatorics.counting.html" class="Module">univalent-combinatorics.counting</a> <a id="847" class="Keyword">using</a>
  <a id="855" class="Symbol">(</a> <a id="857" href="univalent-combinatorics.counting.html#1746" class="Function">count</a><a id="862" class="Symbol">;</a> <a id="864" href="univalent-combinatorics.counting.html#1943" class="Function">equiv-count</a><a id="875" class="Symbol">;</a> <a id="877" href="univalent-combinatorics.counting.html#2017" class="Function">map-equiv-count</a><a id="892" class="Symbol">)</a>
<a id="894" class="Keyword">open</a> <a id="899" class="Keyword">import</a> <a id="906" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a> <a id="952" class="Keyword">using</a> <a id="958" class="Symbol">(</a><a id="959" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a><a id="962" class="Symbol">)</a>
</pre>
## Idea

We describe conditions under which dependent sums are decidable. Note that it is _not_ the case for a family `B` of decidable types over a finite type `A`, that the dependent pair type `Σ A B` is decidable.

## Properties

### The Σ-type of any family of decidable types over `Fin k` is decidable

<pre class="Agda"><a id="is-decidable-Σ-Fin"></a><a id="1284" href="univalent-combinatorics.decidable-dependent-pair-types.html#1284" class="Function">is-decidable-Σ-Fin</a> <a id="1303" class="Symbol">:</a>
  <a id="1307" class="Symbol">{</a><a id="1308" href="univalent-combinatorics.decidable-dependent-pair-types.html#1308" class="Bound">l</a> <a id="1310" class="Symbol">:</a> <a id="1312" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1317" class="Symbol">}</a> <a id="1319" class="Symbol">{</a><a id="1320" href="univalent-combinatorics.decidable-dependent-pair-types.html#1320" class="Bound">k</a> <a id="1322" class="Symbol">:</a> <a id="1324" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1325" class="Symbol">}</a> <a id="1327" class="Symbol">{</a><a id="1328" href="univalent-combinatorics.decidable-dependent-pair-types.html#1328" class="Bound">P</a> <a id="1330" class="Symbol">:</a> <a id="1332" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1336" href="univalent-combinatorics.decidable-dependent-pair-types.html#1320" class="Bound">k</a> <a id="1338" class="Symbol">→</a> <a id="1340" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1343" href="univalent-combinatorics.decidable-dependent-pair-types.html#1308" class="Bound">l</a><a id="1344" class="Symbol">}</a> <a id="1346" class="Symbol">→</a>
  <a id="1350" class="Symbol">((</a><a id="1352" href="univalent-combinatorics.decidable-dependent-pair-types.html#1352" class="Bound">x</a> <a id="1354" class="Symbol">:</a> <a id="1356" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1360" href="univalent-combinatorics.decidable-dependent-pair-types.html#1320" class="Bound">k</a><a id="1361" class="Symbol">)</a> <a id="1363" class="Symbol">→</a> <a id="1365" href="foundation.decidable-types.html#1741" class="Function">is-decidable</a> <a id="1378" class="Symbol">(</a><a id="1379" href="univalent-combinatorics.decidable-dependent-pair-types.html#1328" class="Bound">P</a> <a id="1381" href="univalent-combinatorics.decidable-dependent-pair-types.html#1352" class="Bound">x</a><a id="1382" class="Symbol">))</a> <a id="1385" class="Symbol">→</a> <a id="1387" href="foundation.decidable-types.html#1741" class="Function">is-decidable</a> <a id="1400" class="Symbol">(</a><a id="1401" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1403" class="Symbol">(</a><a id="1404" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1408" href="univalent-combinatorics.decidable-dependent-pair-types.html#1320" class="Bound">k</a><a id="1409" class="Symbol">)</a> <a id="1411" href="univalent-combinatorics.decidable-dependent-pair-types.html#1328" class="Bound">P</a><a id="1412" class="Symbol">)</a>
<a id="1414" href="univalent-combinatorics.decidable-dependent-pair-types.html#1284" class="Function">is-decidable-Σ-Fin</a> <a id="1433" class="Symbol">{</a><a id="1434" href="univalent-combinatorics.decidable-dependent-pair-types.html#1434" class="Bound">l</a><a id="1435" class="Symbol">}</a> <a id="1437" class="Symbol">{</a><a id="1438" href="elementary-number-theory.natural-numbers.html#1465" class="InductiveConstructor">zero-ℕ</a><a id="1444" class="Symbol">}</a> <a id="1446" class="Symbol">{</a><a id="1447" href="univalent-combinatorics.decidable-dependent-pair-types.html#1447" class="Bound">P</a><a id="1448" class="Symbol">}</a> <a id="1450" href="univalent-combinatorics.decidable-dependent-pair-types.html#1450" class="Bound">d</a> <a id="1452" class="Symbol">=</a> <a id="1454" href="foundation.coproduct-types.html#1262" class="InductiveConstructor">inr</a> <a id="1458" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a>
<a id="1462" href="univalent-combinatorics.decidable-dependent-pair-types.html#1284" class="Function">is-decidable-Σ-Fin</a> <a id="1481" class="Symbol">{</a><a id="1482" href="univalent-combinatorics.decidable-dependent-pair-types.html#1482" class="Bound">l</a><a id="1483" class="Symbol">}</a> <a id="1485" class="Symbol">{</a><a id="1486" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a> <a id="1493" href="univalent-combinatorics.decidable-dependent-pair-types.html#1493" class="Bound">k</a><a id="1494" class="Symbol">}</a> <a id="1496" class="Symbol">{</a><a id="1497" href="univalent-combinatorics.decidable-dependent-pair-types.html#1497" class="Bound">P</a><a id="1498" class="Symbol">}</a> <a id="1500" href="univalent-combinatorics.decidable-dependent-pair-types.html#1500" class="Bound">d</a> <a id="1502" class="Keyword">with</a> <a id="1507" href="univalent-combinatorics.decidable-dependent-pair-types.html#1500" class="Bound">d</a> <a id="1509" class="Symbol">(</a><a id="1510" href="foundation.coproduct-types.html#1262" class="InductiveConstructor">inr</a> <a id="1514" href="foundation.unit-type.html#999" class="InductiveConstructor">star</a><a id="1518" class="Symbol">)</a>
<a id="1520" class="Symbol">...</a> <a id="1524" class="Symbol">|</a> <a id="1526" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a> <a id="1530" href="univalent-combinatorics.decidable-dependent-pair-types.html#1530" class="Bound">p</a> <a id="1532" class="Symbol">=</a> <a id="1534" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a> <a id="1538" class="Symbol">(</a><a id="1539" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1544" class="Symbol">(</a><a id="1545" href="foundation.coproduct-types.html#1262" class="InductiveConstructor">inr</a> <a id="1549" href="foundation.unit-type.html#999" class="InductiveConstructor">star</a><a id="1553" class="Symbol">)</a> <a id="1555" href="univalent-combinatorics.decidable-dependent-pair-types.html#1530" class="Bound">p</a><a id="1556" class="Symbol">)</a>
<a id="1558" class="Symbol">...</a> <a id="1562" class="Symbol">|</a> <a id="1564" href="foundation.coproduct-types.html#1262" class="InductiveConstructor">inr</a> <a id="1568" href="univalent-combinatorics.decidable-dependent-pair-types.html#1568" class="Bound">f</a> <a id="1570" class="Symbol">=</a>
  <a id="1574" href="foundation.decidable-types.html#5377" class="Function">is-decidable-iff</a>
    <a id="1595" class="Symbol">(</a> <a id="1597" class="Symbol">λ</a> <a id="1599" href="univalent-combinatorics.decidable-dependent-pair-types.html#1599" class="Bound">t</a> <a id="1601" class="Symbol">→</a> <a id="1603" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1608" class="Symbol">(</a><a id="1609" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a> <a id="1613" class="Symbol">(</a><a id="1614" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1618" href="univalent-combinatorics.decidable-dependent-pair-types.html#1599" class="Bound">t</a><a id="1619" class="Symbol">))</a> <a id="1622" class="Symbol">(</a><a id="1623" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1627" href="univalent-combinatorics.decidable-dependent-pair-types.html#1599" class="Bound">t</a><a id="1628" class="Symbol">))</a>
    <a id="1635" class="Symbol">(</a> <a id="1637" href="univalent-combinatorics.decidable-dependent-pair-types.html#1712" class="Function">g</a><a id="1638" class="Symbol">)</a>
    <a id="1644" class="Symbol">(</a> <a id="1646" href="univalent-combinatorics.decidable-dependent-pair-types.html#1284" class="Function">is-decidable-Σ-Fin</a> <a id="1665" class="Symbol">{</a><a id="1666" class="Bound">l</a><a id="1667" class="Symbol">}</a> <a id="1669" class="Symbol">{</a><a id="1670" class="Bound">k</a><a id="1671" class="Symbol">}</a> <a id="1673" class="Symbol">{</a><a id="1674" class="Bound">P</a> <a id="1676" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="1678" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a><a id="1681" class="Symbol">}</a> <a id="1683" class="Symbol">(λ</a> <a id="1686" href="univalent-combinatorics.decidable-dependent-pair-types.html#1686" class="Bound">x</a> <a id="1688" class="Symbol">→</a> <a id="1690" class="Bound">d</a> <a id="1692" class="Symbol">(</a><a id="1693" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a> <a id="1697" href="univalent-combinatorics.decidable-dependent-pair-types.html#1686" class="Bound">x</a><a id="1698" class="Symbol">)))</a>
  <a id="1704" class="Keyword">where</a>
  <a id="1712" href="univalent-combinatorics.decidable-dependent-pair-types.html#1712" class="Function">g</a> <a id="1714" class="Symbol">:</a> <a id="1716" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1718" class="Symbol">(</a><a id="1719" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1723" class="Symbol">(</a><a id="1724" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a> <a id="1731" class="Bound">k</a><a id="1732" class="Symbol">))</a> <a id="1735" class="Bound">P</a> <a id="1737" class="Symbol">→</a> <a id="1739" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1741" class="Symbol">(</a><a id="1742" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1746" class="Bound">k</a><a id="1747" class="Symbol">)</a> <a id="1749" class="Symbol">(</a><a id="1750" class="Bound">P</a> <a id="1752" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="1754" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a><a id="1757" class="Symbol">)</a>
  <a id="1761" href="univalent-combinatorics.decidable-dependent-pair-types.html#1712" class="Function">g</a> <a id="1763" class="Symbol">(</a><a id="1764" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1769" class="Symbol">(</a><a id="1770" href="foundation.coproduct-types.html#1239" class="InductiveConstructor">inl</a> <a id="1774" href="univalent-combinatorics.decidable-dependent-pair-types.html#1774" class="Bound">x</a><a id="1775" class="Symbol">)</a> <a id="1777" href="univalent-combinatorics.decidable-dependent-pair-types.html#1777" class="Bound">p</a><a id="1778" class="Symbol">)</a> <a id="1780" class="Symbol">=</a> <a id="1782" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1787" href="univalent-combinatorics.decidable-dependent-pair-types.html#1774" class="Bound">x</a> <a id="1789" href="univalent-combinatorics.decidable-dependent-pair-types.html#1777" class="Bound">p</a>
  <a id="1793" href="univalent-combinatorics.decidable-dependent-pair-types.html#1712" class="Function">g</a> <a id="1795" class="Symbol">(</a><a id="1796" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1801" class="Symbol">(</a><a id="1802" href="foundation.coproduct-types.html#1262" class="InductiveConstructor">inr</a> <a id="1806" href="foundation.unit-type.html#999" class="InductiveConstructor">star</a><a id="1810" class="Symbol">)</a> <a id="1812" href="univalent-combinatorics.decidable-dependent-pair-types.html#1812" class="Bound">p</a><a id="1813" class="Symbol">)</a> <a id="1815" class="Symbol">=</a> <a id="1817" href="foundation-core.empty-types.html#1147" class="Function">ex-falso</a> <a id="1826" class="Symbol">(</a><a id="1827" href="univalent-combinatorics.decidable-dependent-pair-types.html#1568" class="Bound">f</a> <a id="1829" href="univalent-combinatorics.decidable-dependent-pair-types.html#1812" class="Bound">p</a><a id="1830" class="Symbol">)</a>
</pre>
### The Σ-type of any family of decidable types over a type equipped with count is decidable

<pre class="Agda"><a id="is-decidable-Σ-count"></a><a id="1939" href="univalent-combinatorics.decidable-dependent-pair-types.html#1939" class="Function">is-decidable-Σ-count</a> <a id="1960" class="Symbol">:</a>
  <a id="1964" class="Symbol">{</a><a id="1965" href="univalent-combinatorics.decidable-dependent-pair-types.html#1965" class="Bound">l1</a> <a id="1968" href="univalent-combinatorics.decidable-dependent-pair-types.html#1968" class="Bound">l2</a> <a id="1971" class="Symbol">:</a> <a id="1973" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1978" class="Symbol">}</a> <a id="1980" class="Symbol">{</a><a id="1981" href="univalent-combinatorics.decidable-dependent-pair-types.html#1981" class="Bound">A</a> <a id="1983" class="Symbol">:</a> <a id="1985" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1988" href="univalent-combinatorics.decidable-dependent-pair-types.html#1965" class="Bound">l1</a><a id="1990" class="Symbol">}</a> <a id="1992" class="Symbol">{</a><a id="1993" href="univalent-combinatorics.decidable-dependent-pair-types.html#1993" class="Bound">B</a> <a id="1995" class="Symbol">:</a> <a id="1997" href="univalent-combinatorics.decidable-dependent-pair-types.html#1981" class="Bound">A</a> <a id="1999" class="Symbol">→</a> <a id="2001" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="2004" href="univalent-combinatorics.decidable-dependent-pair-types.html#1968" class="Bound">l2</a><a id="2006" class="Symbol">}</a> <a id="2008" class="Symbol">→</a> <a id="2010" href="univalent-combinatorics.counting.html#1746" class="Function">count</a> <a id="2016" href="univalent-combinatorics.decidable-dependent-pair-types.html#1981" class="Bound">A</a> <a id="2018" class="Symbol">→</a>
  <a id="2022" class="Symbol">((</a><a id="2024" href="univalent-combinatorics.decidable-dependent-pair-types.html#2024" class="Bound">x</a> <a id="2026" class="Symbol">:</a> <a id="2028" href="univalent-combinatorics.decidable-dependent-pair-types.html#1981" class="Bound">A</a><a id="2029" class="Symbol">)</a> <a id="2031" class="Symbol">→</a> <a id="2033" href="foundation.decidable-types.html#1741" class="Function">is-decidable</a> <a id="2046" class="Symbol">(</a><a id="2047" href="univalent-combinatorics.decidable-dependent-pair-types.html#1993" class="Bound">B</a> <a id="2049" href="univalent-combinatorics.decidable-dependent-pair-types.html#2024" class="Bound">x</a><a id="2050" class="Symbol">))</a> <a id="2053" class="Symbol">→</a> <a id="2055" href="foundation.decidable-types.html#1741" class="Function">is-decidable</a> <a id="2068" class="Symbol">(</a><a id="2069" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="2071" href="univalent-combinatorics.decidable-dependent-pair-types.html#1981" class="Bound">A</a> <a id="2073" href="univalent-combinatorics.decidable-dependent-pair-types.html#1993" class="Bound">B</a><a id="2074" class="Symbol">)</a>
<a id="2076" href="univalent-combinatorics.decidable-dependent-pair-types.html#1939" class="Function">is-decidable-Σ-count</a> <a id="2097" href="univalent-combinatorics.decidable-dependent-pair-types.html#2097" class="Bound">e</a> <a id="2099" href="univalent-combinatorics.decidable-dependent-pair-types.html#2099" class="Bound">d</a> <a id="2101" class="Symbol">=</a>
  <a id="2105" href="foundation.decidable-dependent-pair-types.html#1650" class="Function">is-decidable-Σ-equiv</a>
    <a id="2130" class="Symbol">(</a> <a id="2132" href="univalent-combinatorics.counting.html#1943" class="Function">equiv-count</a> <a id="2144" href="univalent-combinatorics.decidable-dependent-pair-types.html#2097" class="Bound">e</a><a id="2145" class="Symbol">)</a>
    <a id="2151" class="Symbol">(</a> <a id="2153" class="Symbol">λ</a> <a id="2155" href="univalent-combinatorics.decidable-dependent-pair-types.html#2155" class="Bound">x</a> <a id="2157" class="Symbol">→</a> <a id="2159" href="foundation-core.equivalences.html#2480" class="Function">id-equiv</a><a id="2167" class="Symbol">)</a>
    <a id="2173" class="Symbol">(</a> <a id="2175" href="univalent-combinatorics.decidable-dependent-pair-types.html#1284" class="Function">is-decidable-Σ-Fin</a> <a id="2194" class="Symbol">(λ</a> <a id="2197" href="univalent-combinatorics.decidable-dependent-pair-types.html#2197" class="Bound">x</a> <a id="2199" class="Symbol">→</a> <a id="2201" href="univalent-combinatorics.decidable-dependent-pair-types.html#2099" class="Bound">d</a> <a id="2203" class="Symbol">(</a><a id="2204" href="univalent-combinatorics.counting.html#2017" class="Function">map-equiv-count</a> <a id="2220" href="univalent-combinatorics.decidable-dependent-pair-types.html#2097" class="Bound">e</a> <a id="2222" href="univalent-combinatorics.decidable-dependent-pair-types.html#2197" class="Bound">x</a><a id="2223" class="Symbol">)))</a>
</pre>