# Relatively prime natural numbers

<pre class="Agda"><a id="45" class="Symbol">{-#</a> <a id="49" class="Keyword">OPTIONS</a> <a id="57" class="Pragma">--without-K</a> <a id="69" class="Pragma">--exact-split</a> <a id="83" class="Pragma">--allow-unsolved-metas</a> <a id="106" class="Symbol">#-}</a>

<a id="111" class="Keyword">module</a> <a id="118" href="elementary-number-theory.relatively-prime-natural-numbers.html" class="Module">elementary-number-theory.relatively-prime-natural-numbers</a> <a id="176" class="Keyword">where</a>

<a id="183" class="Keyword">open</a> <a id="188" class="Keyword">import</a> <a id="195" href="elementary-number-theory.equality-natural-numbers.html" class="Module">elementary-number-theory.equality-natural-numbers</a> <a id="245" class="Keyword">using</a>
  <a id="253" class="Symbol">(</a> <a id="255" href="elementary-number-theory.equality-natural-numbers.html#3412" class="Function">is-decidable-is-one-ℕ</a><a id="276" class="Symbol">;</a> <a id="278" href="elementary-number-theory.equality-natural-numbers.html#2249" class="Function">is-set-ℕ</a><a id="286" class="Symbol">)</a>
<a id="288" class="Keyword">open</a> <a id="293" class="Keyword">import</a> <a id="300" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html" class="Module">elementary-number-theory.greatest-common-divisor-natural-numbers</a>
  <a id="367" class="Keyword">using</a> <a id="373" class="Symbol">(</a><a id="374" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html#5655" class="Function">gcd-ℕ</a><a id="379" class="Symbol">)</a>
<a id="381" class="Keyword">open</a> <a id="386" class="Keyword">import</a> <a id="393" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="434" class="Keyword">using</a>
  <a id="442" class="Symbol">(</a> <a id="444" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="445" class="Symbol">;</a> <a id="447" href="elementary-number-theory.natural-numbers.html#1465" class="InductiveConstructor">zero-ℕ</a><a id="453" class="Symbol">;</a> <a id="455" href="elementary-number-theory.natural-numbers.html#1478" class="InductiveConstructor">succ-ℕ</a><a id="461" class="Symbol">;</a> <a id="463" href="elementary-number-theory.natural-numbers.html#1988" class="Function">is-one-ℕ</a><a id="471" class="Symbol">)</a>

<a id="474" class="Keyword">open</a> <a id="479" class="Keyword">import</a> <a id="486" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a> <a id="520" class="Keyword">using</a>
  <a id="528" class="Symbol">(</a> <a id="530" href="foundation.decidable-propositions.html#1787" class="Function">is-decidable-prop</a><a id="547" class="Symbol">)</a>
<a id="549" class="Keyword">open</a> <a id="554" class="Keyword">import</a> <a id="561" href="foundation.decidable-types.html" class="Module">foundation.decidable-types</a> <a id="588" class="Keyword">using</a> <a id="594" class="Symbol">(</a><a id="595" href="foundation.decidable-types.html#1905" class="Function">is-decidable</a><a id="607" class="Symbol">)</a>
<a id="609" class="Keyword">open</a> <a id="614" class="Keyword">import</a> <a id="621" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="653" class="Keyword">using</a> <a id="659" class="Symbol">(</a><a id="660" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="661" class="Symbol">;</a> <a id="663" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="667" class="Symbol">;</a> <a id="669" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="672" class="Symbol">;</a> <a id="674" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="677" class="Symbol">)</a>
<a id="679" class="Keyword">open</a> <a id="684" class="Keyword">import</a> <a id="691" href="foundation.propositions.html" class="Module">foundation.propositions</a> <a id="715" class="Keyword">using</a> <a id="721" class="Symbol">(</a><a id="722" href="foundation-core.propositions.html#1246" class="Function">is-prop</a><a id="729" class="Symbol">;</a> <a id="731" href="foundation-core.propositions.html#1322" class="Function">UU-Prop</a><a id="738" class="Symbol">)</a>
<a id="740" class="Keyword">open</a> <a id="745" class="Keyword">import</a> <a id="752" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="779" class="Keyword">using</a> <a id="785" class="Symbol">(</a><a id="786" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="788" class="Symbol">;</a> <a id="790" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="795" class="Symbol">)</a>
</pre>
## Idea

Two natural numbers `x` and `y` are said to be relatively prime if their greatest common divisor is `1`.

## Definition

<pre class="Agda"><a id="relatively-prime-ℕ"></a><a id="940" href="elementary-number-theory.relatively-prime-natural-numbers.html#940" class="Function">relatively-prime-ℕ</a> <a id="959" class="Symbol">:</a> <a id="961" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a> <a id="963" class="Symbol">→</a> <a id="965" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a> <a id="967" class="Symbol">→</a> <a id="969" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="972" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="978" href="elementary-number-theory.relatively-prime-natural-numbers.html#940" class="Function">relatively-prime-ℕ</a> <a id="997" href="elementary-number-theory.relatively-prime-natural-numbers.html#997" class="Bound">x</a> <a id="999" href="elementary-number-theory.relatively-prime-natural-numbers.html#999" class="Bound">y</a> <a id="1001" class="Symbol">=</a> <a id="1003" href="elementary-number-theory.natural-numbers.html#1988" class="Function">is-one-ℕ</a> <a id="1012" class="Symbol">(</a><a id="1013" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html#5655" class="Function">gcd-ℕ</a> <a id="1019" href="elementary-number-theory.relatively-prime-natural-numbers.html#997" class="Bound">x</a> <a id="1021" href="elementary-number-theory.relatively-prime-natural-numbers.html#999" class="Bound">y</a><a id="1022" class="Symbol">)</a>
</pre>
## Properties

### Being relatively prime is a proposition

<pre class="Agda"><a id="is-prop-relatively-prime-ℕ"></a><a id="1097" href="elementary-number-theory.relatively-prime-natural-numbers.html#1097" class="Function">is-prop-relatively-prime-ℕ</a> <a id="1124" class="Symbol">:</a> <a id="1126" class="Symbol">(</a><a id="1127" href="elementary-number-theory.relatively-prime-natural-numbers.html#1127" class="Bound">x</a> <a id="1129" href="elementary-number-theory.relatively-prime-natural-numbers.html#1129" class="Bound">y</a> <a id="1131" class="Symbol">:</a> <a id="1133" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1134" class="Symbol">)</a> <a id="1136" class="Symbol">→</a> <a id="1138" href="foundation-core.propositions.html#1246" class="Function">is-prop</a> <a id="1146" class="Symbol">(</a><a id="1147" href="elementary-number-theory.relatively-prime-natural-numbers.html#940" class="Function">relatively-prime-ℕ</a> <a id="1166" href="elementary-number-theory.relatively-prime-natural-numbers.html#1127" class="Bound">x</a> <a id="1168" href="elementary-number-theory.relatively-prime-natural-numbers.html#1129" class="Bound">y</a><a id="1169" class="Symbol">)</a>
<a id="1171" href="elementary-number-theory.relatively-prime-natural-numbers.html#1097" class="Function">is-prop-relatively-prime-ℕ</a> <a id="1198" href="elementary-number-theory.relatively-prime-natural-numbers.html#1198" class="Bound">x</a> <a id="1200" href="elementary-number-theory.relatively-prime-natural-numbers.html#1200" class="Bound">y</a> <a id="1202" class="Symbol">=</a> <a id="1204" href="elementary-number-theory.equality-natural-numbers.html#2249" class="Function">is-set-ℕ</a> <a id="1213" class="Symbol">(</a><a id="1214" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html#5655" class="Function">gcd-ℕ</a> <a id="1220" href="elementary-number-theory.relatively-prime-natural-numbers.html#1198" class="Bound">x</a> <a id="1222" href="elementary-number-theory.relatively-prime-natural-numbers.html#1200" class="Bound">y</a><a id="1223" class="Symbol">)</a> <a id="1225" class="Number">1</a>

<a id="relatively-prime-ℕ-Prop"></a><a id="1228" href="elementary-number-theory.relatively-prime-natural-numbers.html#1228" class="Function">relatively-prime-ℕ-Prop</a> <a id="1252" class="Symbol">:</a> <a id="1254" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a> <a id="1256" class="Symbol">→</a> <a id="1258" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a> <a id="1260" class="Symbol">→</a> <a id="1262" href="foundation-core.propositions.html#1322" class="Function">UU-Prop</a> <a id="1270" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="1276" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1280" class="Symbol">(</a><a id="1281" href="elementary-number-theory.relatively-prime-natural-numbers.html#1228" class="Function">relatively-prime-ℕ-Prop</a> <a id="1305" href="elementary-number-theory.relatively-prime-natural-numbers.html#1305" class="Bound">x</a> <a id="1307" href="elementary-number-theory.relatively-prime-natural-numbers.html#1307" class="Bound">y</a><a id="1308" class="Symbol">)</a> <a id="1310" class="Symbol">=</a> <a id="1312" href="elementary-number-theory.relatively-prime-natural-numbers.html#940" class="Function">relatively-prime-ℕ</a> <a id="1331" href="elementary-number-theory.relatively-prime-natural-numbers.html#1305" class="Bound">x</a> <a id="1333" href="elementary-number-theory.relatively-prime-natural-numbers.html#1307" class="Bound">y</a>
<a id="1335" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1339" class="Symbol">(</a><a id="1340" href="elementary-number-theory.relatively-prime-natural-numbers.html#1228" class="Function">relatively-prime-ℕ-Prop</a> <a id="1364" href="elementary-number-theory.relatively-prime-natural-numbers.html#1364" class="Bound">x</a> <a id="1366" href="elementary-number-theory.relatively-prime-natural-numbers.html#1366" class="Bound">y</a><a id="1367" class="Symbol">)</a> <a id="1369" class="Symbol">=</a> <a id="1371" href="elementary-number-theory.relatively-prime-natural-numbers.html#1097" class="Function">is-prop-relatively-prime-ℕ</a> <a id="1398" href="elementary-number-theory.relatively-prime-natural-numbers.html#1364" class="Bound">x</a> <a id="1400" href="elementary-number-theory.relatively-prime-natural-numbers.html#1366" class="Bound">y</a>
</pre>
### Being relatively prime is decidable

<pre class="Agda"><a id="is-decidable-relatively-prime-ℕ"></a><a id="1456" href="elementary-number-theory.relatively-prime-natural-numbers.html#1456" class="Function">is-decidable-relatively-prime-ℕ</a> <a id="1488" class="Symbol">:</a>
  <a id="1492" class="Symbol">(</a><a id="1493" href="elementary-number-theory.relatively-prime-natural-numbers.html#1493" class="Bound">x</a> <a id="1495" href="elementary-number-theory.relatively-prime-natural-numbers.html#1495" class="Bound">y</a> <a id="1497" class="Symbol">:</a> <a id="1499" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1500" class="Symbol">)</a> <a id="1502" class="Symbol">→</a> <a id="1504" href="foundation.decidable-types.html#1905" class="Function">is-decidable</a> <a id="1517" class="Symbol">(</a><a id="1518" href="elementary-number-theory.relatively-prime-natural-numbers.html#940" class="Function">relatively-prime-ℕ</a> <a id="1537" href="elementary-number-theory.relatively-prime-natural-numbers.html#1493" class="Bound">x</a> <a id="1539" href="elementary-number-theory.relatively-prime-natural-numbers.html#1495" class="Bound">y</a><a id="1540" class="Symbol">)</a>
<a id="1542" href="elementary-number-theory.relatively-prime-natural-numbers.html#1456" class="Function">is-decidable-relatively-prime-ℕ</a> <a id="1574" href="elementary-number-theory.relatively-prime-natural-numbers.html#1574" class="Bound">x</a> <a id="1576" href="elementary-number-theory.relatively-prime-natural-numbers.html#1576" class="Bound">y</a> <a id="1578" class="Symbol">=</a> <a id="1580" href="elementary-number-theory.equality-natural-numbers.html#3412" class="Function">is-decidable-is-one-ℕ</a> <a id="1602" class="Symbol">(</a><a id="1603" href="elementary-number-theory.greatest-common-divisor-natural-numbers.html#5655" class="Function">gcd-ℕ</a> <a id="1609" href="elementary-number-theory.relatively-prime-natural-numbers.html#1574" class="Bound">x</a> <a id="1611" href="elementary-number-theory.relatively-prime-natural-numbers.html#1576" class="Bound">y</a><a id="1612" class="Symbol">)</a>

<a id="is-decidable-prop-relatively-prime-ℕ"></a><a id="1615" href="elementary-number-theory.relatively-prime-natural-numbers.html#1615" class="Function">is-decidable-prop-relatively-prime-ℕ</a> <a id="1652" class="Symbol">:</a>
  <a id="1656" class="Symbol">(</a><a id="1657" href="elementary-number-theory.relatively-prime-natural-numbers.html#1657" class="Bound">x</a> <a id="1659" href="elementary-number-theory.relatively-prime-natural-numbers.html#1659" class="Bound">y</a> <a id="1661" class="Symbol">:</a> <a id="1663" href="elementary-number-theory.natural-numbers.html#1444" class="Datatype">ℕ</a><a id="1664" class="Symbol">)</a> <a id="1666" class="Symbol">→</a> <a id="1668" href="foundation.decidable-propositions.html#1787" class="Function">is-decidable-prop</a> <a id="1686" class="Symbol">(</a><a id="1687" href="elementary-number-theory.relatively-prime-natural-numbers.html#940" class="Function">relatively-prime-ℕ</a> <a id="1706" href="elementary-number-theory.relatively-prime-natural-numbers.html#1657" class="Bound">x</a> <a id="1708" href="elementary-number-theory.relatively-prime-natural-numbers.html#1659" class="Bound">y</a><a id="1709" class="Symbol">)</a>
<a id="1711" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1715" class="Symbol">(</a><a id="1716" href="elementary-number-theory.relatively-prime-natural-numbers.html#1615" class="Function">is-decidable-prop-relatively-prime-ℕ</a> <a id="1753" href="elementary-number-theory.relatively-prime-natural-numbers.html#1753" class="Bound">x</a> <a id="1755" href="elementary-number-theory.relatively-prime-natural-numbers.html#1755" class="Bound">y</a><a id="1756" class="Symbol">)</a> <a id="1758" class="Symbol">=</a>
  <a id="1762" href="elementary-number-theory.relatively-prime-natural-numbers.html#1097" class="Function">is-prop-relatively-prime-ℕ</a> <a id="1789" href="elementary-number-theory.relatively-prime-natural-numbers.html#1753" class="Bound">x</a> <a id="1791" href="elementary-number-theory.relatively-prime-natural-numbers.html#1755" class="Bound">y</a>
<a id="1793" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1797" class="Symbol">(</a><a id="1798" href="elementary-number-theory.relatively-prime-natural-numbers.html#1615" class="Function">is-decidable-prop-relatively-prime-ℕ</a> <a id="1835" href="elementary-number-theory.relatively-prime-natural-numbers.html#1835" class="Bound">x</a> <a id="1837" href="elementary-number-theory.relatively-prime-natural-numbers.html#1837" class="Bound">y</a><a id="1838" class="Symbol">)</a> <a id="1840" class="Symbol">=</a>
  <a id="1844" href="elementary-number-theory.relatively-prime-natural-numbers.html#1456" class="Function">is-decidable-relatively-prime-ℕ</a> <a id="1876" href="elementary-number-theory.relatively-prime-natural-numbers.html#1835" class="Bound">x</a> <a id="1878" href="elementary-number-theory.relatively-prime-natural-numbers.html#1837" class="Bound">y</a>
</pre>
### A number y is relatively prime to x if and only if `[y] mod x` is a unit in `ℤ-Mod x`

<pre class="Agda"><a id="1984" class="Comment">-- relatively-prime-is-unit-mod-ℕ :</a>
<a id="2020" class="Comment">--   (x y : ℕ) → is-unit-ℤ-Mod x (mod-ℕ y) → relatively-prime-ℕ x y</a>
<a id="2088" class="Comment">-- relatively-prime-is-unit-mod-ℕ x y H = ?</a>
</pre>