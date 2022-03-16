# The divisibility relation on the standard finite types

<pre class="Agda"><a id="67" class="Symbol">{-#</a> <a id="71" class="Keyword">OPTIONS</a> <a id="79" class="Pragma">--without-K</a> <a id="91" class="Pragma">--exact-split</a> <a id="105" class="Symbol">#-}</a>

<a id="110" class="Keyword">module</a> <a id="117" href="elementary-number-theory.divisibility-standard-finite-types.html" class="Module">elementary-number-theory.divisibility-standard-finite-types</a> <a id="177" class="Keyword">where</a>

<a id="184" class="Keyword">open</a> <a id="189" class="Keyword">import</a>
  <a id="198" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html" class="Module">elementary-number-theory.modular-arithmetic-standard-finite-types</a> <a id="264" class="Keyword">using</a>
  <a id="272" class="Symbol">(</a> <a id="274" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#12046" class="Function">mul-Fin</a><a id="281" class="Symbol">;</a> <a id="283" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#14090" class="Function">left-unit-law-mul-Fin</a><a id="304" class="Symbol">;</a> <a id="306" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#12642" class="Function">associative-mul-Fin</a><a id="325" class="Symbol">;</a> <a id="327" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#14742" class="Function">left-zero-law-mul-Fin</a><a id="348" class="Symbol">;</a>
    <a id="354" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#14565" class="Function">right-unit-law-mul-Fin</a><a id="376" class="Symbol">;</a> <a id="378" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#15243" class="Function">right-zero-law-mul-Fin</a><a id="400" class="Symbol">)</a>
<a id="402" class="Keyword">open</a> <a id="407" class="Keyword">import</a> <a id="414" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="455" class="Keyword">using</a> <a id="461" class="Symbol">(</a><a id="462" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="463" class="Symbol">;</a> <a id="465" href="elementary-number-theory.natural-numbers.html#1465" class="InductiveConstructor">zero-ℕ</a><a id="471" class="Symbol">;</a> <a id="473" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a><a id="479" class="Symbol">)</a>

<a id="482" class="Keyword">open</a> <a id="487" class="Keyword">import</a> <a id="494" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a> <a id="521" class="Keyword">using</a> <a id="527" class="Symbol">(</a><a id="528" href="foundation.decidable-types.html#1741" class="Function">is-decidable</a><a id="540" class="Symbol">)</a>
<a id="542" class="Keyword">open</a> <a id="547" class="Keyword">import</a> <a id="554" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="586" class="Keyword">using</a> <a id="592" class="Symbol">(</a><a id="593" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="594" class="Symbol">;</a> <a id="596" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="600" class="Symbol">;</a> <a id="602" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="605" class="Symbol">;</a> <a id="607" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="610" class="Symbol">)</a>
<a id="612" class="Keyword">open</a> <a id="617" class="Keyword">import</a> <a id="624" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="650" class="Keyword">using</a> <a id="656" class="Symbol">(</a><a id="657" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="659" class="Symbol">;</a> <a id="661" href="foundation-core.identity-types.html#1239" class="Function Operator">_∙_</a><a id="664" class="Symbol">;</a> <a id="666" href="foundation-core.identity-types.html#2853" class="Function">ap</a><a id="668" class="Symbol">;</a> <a id="670" href="foundation-core.identity-types.html#1552" class="Function">inv</a><a id="673" class="Symbol">)</a>
<a id="675" class="Keyword">open</a> <a id="680" class="Keyword">import</a> <a id="687" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="714" class="Keyword">using</a> <a id="720" class="Symbol">(</a><a id="721" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="723" class="Symbol">;</a> <a id="725" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="730" class="Symbol">)</a>

<a id="733" class="Keyword">open</a> <a id="738" class="Keyword">import</a> <a id="745" href="univalent-combinatorics.decidable-dependent-pair-types.html" class="Module">univalent-combinatorics.decidable-dependent-pair-types</a> <a id="800" class="Keyword">using</a>
  <a id="808" class="Symbol">(</a> <a id="810" href="univalent-combinatorics.decidable-dependent-pair-types.html#1284" class="Function">is-decidable-Σ-Fin</a><a id="828" class="Symbol">)</a>
<a id="830" class="Keyword">open</a> <a id="835" class="Keyword">import</a> <a id="842" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a> <a id="897" class="Keyword">using</a>
  <a id="905" class="Symbol">(</a> <a id="907" href="univalent-combinatorics.equality-standard-finite-types.html#2783" class="Function">has-decidable-equality-Fin</a><a id="933" class="Symbol">)</a>
<a id="935" class="Keyword">open</a> <a id="940" class="Keyword">import</a> <a id="947" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a> <a id="993" class="Keyword">using</a>
  <a id="1001" class="Symbol">(</a> <a id="1003" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a><a id="1006" class="Symbol">;</a> <a id="1008" href="univalent-combinatorics.standard-finite-types.html#8241" class="Function">one-Fin</a><a id="1015" class="Symbol">;</a> <a id="1017" href="univalent-combinatorics.standard-finite-types.html#7006" class="Function">zero-Fin</a><a id="1025" class="Symbol">;</a> <a id="1027" href="univalent-combinatorics.standard-finite-types.html#7107" class="Function">is-zero-Fin</a><a id="1038" class="Symbol">)</a>
</pre>
## Idea

Given two elements `x y : Fin k`, we say that `x` divides `y` if there is an element `u : Fin k` such that `mul-Fin u x = y`.

## Definition

<pre class="Agda"><a id="div-Fin"></a><a id="1204" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="1212" class="Symbol">:</a> <a id="1214" class="Symbol">{</a><a id="1215" href="elementary-number-theory.divisibility-standard-finite-types.html#1215" class="Bound">k</a> <a id="1217" class="Symbol">:</a> <a id="1219" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1220" class="Symbol">}</a> <a id="1222" class="Symbol">→</a> <a id="1224" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1228" href="elementary-number-theory.divisibility-standard-finite-types.html#1215" class="Bound">k</a> <a id="1230" class="Symbol">→</a> <a id="1232" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1236" href="elementary-number-theory.divisibility-standard-finite-types.html#1215" class="Bound">k</a> <a id="1238" class="Symbol">→</a> <a id="1240" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1243" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="1249" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="1257" class="Symbol">{</a><a id="1258" href="elementary-number-theory.divisibility-standard-finite-types.html#1258" class="Bound">k</a><a id="1259" class="Symbol">}</a> <a id="1261" href="elementary-number-theory.divisibility-standard-finite-types.html#1261" class="Bound">x</a> <a id="1263" href="elementary-number-theory.divisibility-standard-finite-types.html#1263" class="Bound">y</a> <a id="1265" class="Symbol">=</a> <a id="1267" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1269" class="Symbol">(</a><a id="1270" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1274" href="elementary-number-theory.divisibility-standard-finite-types.html#1258" class="Bound">k</a><a id="1275" class="Symbol">)</a> <a id="1277" class="Symbol">(λ</a> <a id="1280" href="elementary-number-theory.divisibility-standard-finite-types.html#1280" class="Bound">u</a> <a id="1282" class="Symbol">→</a> <a id="1284" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1287" class="Symbol">(</a><a id="1288" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#12046" class="Function">mul-Fin</a> <a id="1296" href="elementary-number-theory.divisibility-standard-finite-types.html#1280" class="Bound">u</a> <a id="1298" href="elementary-number-theory.divisibility-standard-finite-types.html#1261" class="Bound">x</a><a id="1299" class="Symbol">)</a> <a id="1301" href="elementary-number-theory.divisibility-standard-finite-types.html#1263" class="Bound">y</a><a id="1302" class="Symbol">)</a>
</pre>
## Properties

### The divisibility relation is reflexive

<pre class="Agda"><a id="refl-div-Fin"></a><a id="1376" href="elementary-number-theory.divisibility-standard-finite-types.html#1376" class="Function">refl-div-Fin</a> <a id="1389" class="Symbol">:</a> <a id="1391" class="Symbol">{</a><a id="1392" href="elementary-number-theory.divisibility-standard-finite-types.html#1392" class="Bound">k</a> <a id="1394" class="Symbol">:</a> <a id="1396" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1397" class="Symbol">}</a> <a id="1399" class="Symbol">(</a><a id="1400" href="elementary-number-theory.divisibility-standard-finite-types.html#1400" class="Bound">x</a> <a id="1402" class="Symbol">:</a> <a id="1404" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1408" href="elementary-number-theory.divisibility-standard-finite-types.html#1392" class="Bound">k</a><a id="1409" class="Symbol">)</a> <a id="1411" class="Symbol">→</a> <a id="1413" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="1421" href="elementary-number-theory.divisibility-standard-finite-types.html#1400" class="Bound">x</a> <a id="1423" href="elementary-number-theory.divisibility-standard-finite-types.html#1400" class="Bound">x</a>
<a id="1425" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1429" class="Symbol">(</a><a id="1430" href="elementary-number-theory.divisibility-standard-finite-types.html#1376" class="Function">refl-div-Fin</a> <a id="1443" class="Symbol">{</a><a id="1444" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a> <a id="1451" href="elementary-number-theory.divisibility-standard-finite-types.html#1451" class="Bound">k</a><a id="1452" class="Symbol">}</a> <a id="1454" href="elementary-number-theory.divisibility-standard-finite-types.html#1454" class="Bound">x</a><a id="1455" class="Symbol">)</a> <a id="1457" class="Symbol">=</a> <a id="1459" href="univalent-combinatorics.standard-finite-types.html#8241" class="Function">one-Fin</a>
<a id="1467" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1471" class="Symbol">(</a><a id="1472" href="elementary-number-theory.divisibility-standard-finite-types.html#1376" class="Function">refl-div-Fin</a> <a id="1485" class="Symbol">{</a><a id="1486" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a> <a id="1493" href="elementary-number-theory.divisibility-standard-finite-types.html#1493" class="Bound">k</a><a id="1494" class="Symbol">}</a> <a id="1496" href="elementary-number-theory.divisibility-standard-finite-types.html#1496" class="Bound">x</a><a id="1497" class="Symbol">)</a> <a id="1499" class="Symbol">=</a> <a id="1501" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#14090" class="Function">left-unit-law-mul-Fin</a> <a id="1523" href="elementary-number-theory.divisibility-standard-finite-types.html#1496" class="Bound">x</a>
</pre>
### The divisibility relation is transitive

<pre class="Agda"><a id="trans-div-Fin"></a><a id="1583" href="elementary-number-theory.divisibility-standard-finite-types.html#1583" class="Function">trans-div-Fin</a> <a id="1597" class="Symbol">:</a>
  <a id="1601" class="Symbol">{</a><a id="1602" href="elementary-number-theory.divisibility-standard-finite-types.html#1602" class="Bound">k</a> <a id="1604" class="Symbol">:</a> <a id="1606" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1607" class="Symbol">}</a> <a id="1609" class="Symbol">(</a><a id="1610" href="elementary-number-theory.divisibility-standard-finite-types.html#1610" class="Bound">x</a> <a id="1612" href="elementary-number-theory.divisibility-standard-finite-types.html#1612" class="Bound">y</a> <a id="1614" href="elementary-number-theory.divisibility-standard-finite-types.html#1614" class="Bound">z</a> <a id="1616" class="Symbol">:</a> <a id="1618" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1622" href="elementary-number-theory.divisibility-standard-finite-types.html#1602" class="Bound">k</a><a id="1623" class="Symbol">)</a> <a id="1625" class="Symbol">→</a> <a id="1627" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="1635" href="elementary-number-theory.divisibility-standard-finite-types.html#1610" class="Bound">x</a> <a id="1637" href="elementary-number-theory.divisibility-standard-finite-types.html#1612" class="Bound">y</a> <a id="1639" class="Symbol">→</a> <a id="1641" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="1649" href="elementary-number-theory.divisibility-standard-finite-types.html#1612" class="Bound">y</a> <a id="1651" href="elementary-number-theory.divisibility-standard-finite-types.html#1614" class="Bound">z</a> <a id="1653" class="Symbol">→</a> <a id="1655" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="1663" href="elementary-number-theory.divisibility-standard-finite-types.html#1610" class="Bound">x</a> <a id="1665" href="elementary-number-theory.divisibility-standard-finite-types.html#1614" class="Bound">z</a>
<a id="1667" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1671" class="Symbol">(</a><a id="1672" href="elementary-number-theory.divisibility-standard-finite-types.html#1583" class="Function">trans-div-Fin</a> <a id="1686" href="elementary-number-theory.divisibility-standard-finite-types.html#1686" class="Bound">x</a> <a id="1688" href="elementary-number-theory.divisibility-standard-finite-types.html#1688" class="Bound">y</a> <a id="1690" href="elementary-number-theory.divisibility-standard-finite-types.html#1690" class="Bound">z</a> <a id="1692" class="Symbol">(</a><a id="1693" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1698" href="elementary-number-theory.divisibility-standard-finite-types.html#1698" class="Bound">u</a> <a id="1700" href="elementary-number-theory.divisibility-standard-finite-types.html#1700" class="Bound">p</a><a id="1701" class="Symbol">)</a> <a id="1703" class="Symbol">(</a><a id="1704" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1709" href="elementary-number-theory.divisibility-standard-finite-types.html#1709" class="Bound">v</a> <a id="1711" href="elementary-number-theory.divisibility-standard-finite-types.html#1711" class="Bound">q</a><a id="1712" class="Symbol">))</a> <a id="1715" class="Symbol">=</a> <a id="1717" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#12046" class="Function">mul-Fin</a> <a id="1725" href="elementary-number-theory.divisibility-standard-finite-types.html#1709" class="Bound">v</a> <a id="1727" href="elementary-number-theory.divisibility-standard-finite-types.html#1698" class="Bound">u</a>
<a id="1729" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1733" class="Symbol">(</a><a id="1734" href="elementary-number-theory.divisibility-standard-finite-types.html#1583" class="Function">trans-div-Fin</a> <a id="1748" href="elementary-number-theory.divisibility-standard-finite-types.html#1748" class="Bound">x</a> <a id="1750" href="elementary-number-theory.divisibility-standard-finite-types.html#1750" class="Bound">y</a> <a id="1752" href="elementary-number-theory.divisibility-standard-finite-types.html#1752" class="Bound">z</a> <a id="1754" class="Symbol">(</a><a id="1755" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1760" href="elementary-number-theory.divisibility-standard-finite-types.html#1760" class="Bound">u</a> <a id="1762" href="elementary-number-theory.divisibility-standard-finite-types.html#1762" class="Bound">p</a><a id="1763" class="Symbol">)</a> <a id="1765" class="Symbol">(</a><a id="1766" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1771" href="elementary-number-theory.divisibility-standard-finite-types.html#1771" class="Bound">v</a> <a id="1773" href="elementary-number-theory.divisibility-standard-finite-types.html#1773" class="Bound">q</a><a id="1774" class="Symbol">))</a> <a id="1777" class="Symbol">=</a>
  <a id="1781" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#12642" class="Function">associative-mul-Fin</a> <a id="1801" href="elementary-number-theory.divisibility-standard-finite-types.html#1771" class="Bound">v</a> <a id="1803" href="elementary-number-theory.divisibility-standard-finite-types.html#1760" class="Bound">u</a> <a id="1805" href="elementary-number-theory.divisibility-standard-finite-types.html#1748" class="Bound">x</a> <a id="1807" href="foundation-core.identity-types.html#1239" class="Function Operator">∙</a> <a id="1809" class="Symbol">(</a><a id="1810" href="foundation-core.identity-types.html#2853" class="Function">ap</a> <a id="1813" class="Symbol">(</a><a id="1814" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#12046" class="Function">mul-Fin</a> <a id="1822" href="elementary-number-theory.divisibility-standard-finite-types.html#1771" class="Bound">v</a><a id="1823" class="Symbol">)</a> <a id="1825" href="elementary-number-theory.divisibility-standard-finite-types.html#1762" class="Bound">p</a> <a id="1827" href="foundation-core.identity-types.html#1239" class="Function Operator">∙</a> <a id="1829" href="elementary-number-theory.divisibility-standard-finite-types.html#1773" class="Bound">q</a><a id="1830" class="Symbol">)</a>
</pre>
### Every element divides zero

<pre class="Agda"><a id="div-zero-Fin"></a><a id="1877" href="elementary-number-theory.divisibility-standard-finite-types.html#1877" class="Function">div-zero-Fin</a> <a id="1890" class="Symbol">:</a> <a id="1892" class="Symbol">{</a><a id="1893" href="elementary-number-theory.divisibility-standard-finite-types.html#1893" class="Bound">k</a> <a id="1895" class="Symbol">:</a> <a id="1897" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1898" class="Symbol">}</a> <a id="1900" class="Symbol">(</a><a id="1901" href="elementary-number-theory.divisibility-standard-finite-types.html#1901" class="Bound">x</a> <a id="1903" class="Symbol">:</a> <a id="1905" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="1909" class="Symbol">(</a><a id="1910" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a> <a id="1917" href="elementary-number-theory.divisibility-standard-finite-types.html#1893" class="Bound">k</a><a id="1918" class="Symbol">))</a> <a id="1921" class="Symbol">→</a> <a id="1923" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="1931" href="elementary-number-theory.divisibility-standard-finite-types.html#1901" class="Bound">x</a> <a id="1933" href="univalent-combinatorics.standard-finite-types.html#7006" class="Function">zero-Fin</a>
<a id="1942" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1946" class="Symbol">(</a><a id="1947" href="elementary-number-theory.divisibility-standard-finite-types.html#1877" class="Function">div-zero-Fin</a> <a id="1960" href="elementary-number-theory.divisibility-standard-finite-types.html#1960" class="Bound">x</a><a id="1961" class="Symbol">)</a> <a id="1963" class="Symbol">=</a> <a id="1965" href="univalent-combinatorics.standard-finite-types.html#7006" class="Function">zero-Fin</a>
<a id="1974" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1978" class="Symbol">(</a><a id="1979" href="elementary-number-theory.divisibility-standard-finite-types.html#1877" class="Function">div-zero-Fin</a> <a id="1992" href="elementary-number-theory.divisibility-standard-finite-types.html#1992" class="Bound">x</a><a id="1993" class="Symbol">)</a> <a id="1995" class="Symbol">=</a> <a id="1997" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#14742" class="Function">left-zero-law-mul-Fin</a> <a id="2019" href="elementary-number-theory.divisibility-standard-finite-types.html#1992" class="Bound">x</a>
</pre>
### Every element is divisible by one

<pre class="Agda"><a id="div-one-Fin"></a><a id="2073" href="elementary-number-theory.divisibility-standard-finite-types.html#2073" class="Function">div-one-Fin</a> <a id="2085" class="Symbol">:</a> <a id="2087" class="Symbol">{</a><a id="2088" href="elementary-number-theory.divisibility-standard-finite-types.html#2088" class="Bound">k</a> <a id="2090" class="Symbol">:</a> <a id="2092" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="2093" class="Symbol">}</a> <a id="2095" class="Symbol">(</a><a id="2096" href="elementary-number-theory.divisibility-standard-finite-types.html#2096" class="Bound">x</a> <a id="2098" class="Symbol">:</a> <a id="2100" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="2104" class="Symbol">(</a><a id="2105" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a> <a id="2112" href="elementary-number-theory.divisibility-standard-finite-types.html#2088" class="Bound">k</a><a id="2113" class="Symbol">))</a> <a id="2116" class="Symbol">→</a> <a id="2118" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="2126" href="univalent-combinatorics.standard-finite-types.html#8241" class="Function">one-Fin</a> <a id="2134" href="elementary-number-theory.divisibility-standard-finite-types.html#2096" class="Bound">x</a>
<a id="2136" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2140" class="Symbol">(</a><a id="2141" href="elementary-number-theory.divisibility-standard-finite-types.html#2073" class="Function">div-one-Fin</a> <a id="2153" href="elementary-number-theory.divisibility-standard-finite-types.html#2153" class="Bound">x</a><a id="2154" class="Symbol">)</a> <a id="2156" class="Symbol">=</a> <a id="2158" href="elementary-number-theory.divisibility-standard-finite-types.html#2153" class="Bound">x</a>
<a id="2160" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2164" class="Symbol">(</a><a id="2165" href="elementary-number-theory.divisibility-standard-finite-types.html#2073" class="Function">div-one-Fin</a> <a id="2177" href="elementary-number-theory.divisibility-standard-finite-types.html#2177" class="Bound">x</a><a id="2178" class="Symbol">)</a> <a id="2180" class="Symbol">=</a> <a id="2182" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#14565" class="Function">right-unit-law-mul-Fin</a> <a id="2205" href="elementary-number-theory.divisibility-standard-finite-types.html#2177" class="Bound">x</a>
</pre>
### The only element that is divisible by zero is zero itself

<pre class="Agda"><a id="is-zero-div-zero-Fin"></a><a id="2283" href="elementary-number-theory.divisibility-standard-finite-types.html#2283" class="Function">is-zero-div-zero-Fin</a> <a id="2304" class="Symbol">:</a>
  <a id="2308" class="Symbol">{</a><a id="2309" href="elementary-number-theory.divisibility-standard-finite-types.html#2309" class="Bound">k</a> <a id="2311" class="Symbol">:</a> <a id="2313" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="2314" class="Symbol">}</a> <a id="2316" class="Symbol">(</a><a id="2317" href="elementary-number-theory.divisibility-standard-finite-types.html#2317" class="Bound">x</a> <a id="2319" class="Symbol">:</a> <a id="2321" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="2325" class="Symbol">(</a><a id="2326" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a> <a id="2333" href="elementary-number-theory.divisibility-standard-finite-types.html#2309" class="Bound">k</a><a id="2334" class="Symbol">))</a> <a id="2337" class="Symbol">→</a> <a id="2339" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="2347" href="univalent-combinatorics.standard-finite-types.html#7006" class="Function">zero-Fin</a> <a id="2356" href="elementary-number-theory.divisibility-standard-finite-types.html#2317" class="Bound">x</a> <a id="2358" class="Symbol">→</a> <a id="2360" href="univalent-combinatorics.standard-finite-types.html#7107" class="Function">is-zero-Fin</a> <a id="2372" href="elementary-number-theory.divisibility-standard-finite-types.html#2317" class="Bound">x</a>
<a id="2374" href="elementary-number-theory.divisibility-standard-finite-types.html#2283" class="Function">is-zero-div-zero-Fin</a> <a id="2395" class="Symbol">{</a><a id="2396" href="elementary-number-theory.divisibility-standard-finite-types.html#2396" class="Bound">k</a><a id="2397" class="Symbol">}</a> <a id="2399" href="elementary-number-theory.divisibility-standard-finite-types.html#2399" class="Bound">x</a> <a id="2401" class="Symbol">(</a><a id="2402" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2407" href="elementary-number-theory.divisibility-standard-finite-types.html#2407" class="Bound">u</a> <a id="2409" href="elementary-number-theory.divisibility-standard-finite-types.html#2409" class="Bound">p</a><a id="2410" class="Symbol">)</a> <a id="2412" class="Symbol">=</a> <a id="2414" href="foundation-core.identity-types.html#1552" class="Function">inv</a> <a id="2418" href="elementary-number-theory.divisibility-standard-finite-types.html#2409" class="Bound">p</a> <a id="2420" href="foundation-core.identity-types.html#1239" class="Function Operator">∙</a> <a id="2422" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#15243" class="Function">right-zero-law-mul-Fin</a> <a id="2445" href="elementary-number-theory.divisibility-standard-finite-types.html#2407" class="Bound">u</a>
</pre>
### The divisibility relation is decidable

<pre class="Agda"><a id="is-decidable-div-Fin"></a><a id="2504" href="elementary-number-theory.divisibility-standard-finite-types.html#2504" class="Function">is-decidable-div-Fin</a> <a id="2525" class="Symbol">:</a> <a id="2527" class="Symbol">{</a><a id="2528" href="elementary-number-theory.divisibility-standard-finite-types.html#2528" class="Bound">k</a> <a id="2530" class="Symbol">:</a> <a id="2532" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="2533" class="Symbol">}</a> <a id="2535" class="Symbol">(</a><a id="2536" href="elementary-number-theory.divisibility-standard-finite-types.html#2536" class="Bound">x</a> <a id="2538" href="elementary-number-theory.divisibility-standard-finite-types.html#2538" class="Bound">y</a> <a id="2540" class="Symbol">:</a> <a id="2542" href="univalent-combinatorics.standard-finite-types.html#2072" class="Function">Fin</a> <a id="2546" href="elementary-number-theory.divisibility-standard-finite-types.html#2528" class="Bound">k</a><a id="2547" class="Symbol">)</a> <a id="2549" class="Symbol">→</a> <a id="2551" href="foundation.decidable-types.html#1741" class="Function">is-decidable</a> <a id="2564" class="Symbol">(</a><a id="2565" href="elementary-number-theory.divisibility-standard-finite-types.html#1204" class="Function">div-Fin</a> <a id="2573" href="elementary-number-theory.divisibility-standard-finite-types.html#2536" class="Bound">x</a> <a id="2575" href="elementary-number-theory.divisibility-standard-finite-types.html#2538" class="Bound">y</a><a id="2576" class="Symbol">)</a>
<a id="2578" href="elementary-number-theory.divisibility-standard-finite-types.html#2504" class="Function">is-decidable-div-Fin</a> <a id="2599" href="elementary-number-theory.divisibility-standard-finite-types.html#2599" class="Bound">x</a> <a id="2601" href="elementary-number-theory.divisibility-standard-finite-types.html#2601" class="Bound">y</a> <a id="2603" class="Symbol">=</a>
  <a id="2607" href="univalent-combinatorics.decidable-dependent-pair-types.html#1284" class="Function">is-decidable-Σ-Fin</a> <a id="2626" class="Symbol">(λ</a> <a id="2629" href="elementary-number-theory.divisibility-standard-finite-types.html#2629" class="Bound">u</a> <a id="2631" class="Symbol">→</a> <a id="2633" href="univalent-combinatorics.equality-standard-finite-types.html#2783" class="Function">has-decidable-equality-Fin</a> <a id="2660" class="Symbol">(</a><a id="2661" href="elementary-number-theory.modular-arithmetic-standard-finite-types.html#12046" class="Function">mul-Fin</a> <a id="2669" href="elementary-number-theory.divisibility-standard-finite-types.html#2629" class="Bound">u</a> <a id="2671" href="elementary-number-theory.divisibility-standard-finite-types.html#2599" class="Bound">x</a><a id="2672" class="Symbol">)</a> <a id="2674" href="elementary-number-theory.divisibility-standard-finite-types.html#2601" class="Bound">y</a><a id="2675" class="Symbol">)</a>
</pre>