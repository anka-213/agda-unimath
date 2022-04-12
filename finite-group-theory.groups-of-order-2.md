# Groups of order 2

<pre class="Agda"><a id="30" class="Symbol">{-#</a> <a id="34" class="Keyword">OPTIONS</a> <a id="42" class="Pragma">--without-K</a> <a id="54" class="Pragma">--exact-split</a> <a id="68" class="Pragma">--allow-unsolved-metas</a> <a id="91" class="Symbol">#-}</a>

<a id="96" class="Keyword">module</a> <a id="103" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a> <a id="141" class="Keyword">where</a>

<a id="148" class="Keyword">open</a> <a id="153" class="Keyword">import</a> <a id="160" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>

<a id="215" class="Keyword">open</a> <a id="220" class="Keyword">import</a> <a id="227" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a>

<a id="262" class="Keyword">open</a> <a id="267" class="Keyword">import</a> <a id="274" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a>
<a id="304" class="Keyword">open</a> <a id="309" class="Keyword">import</a> <a id="316" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="348" class="Keyword">open</a> <a id="353" class="Keyword">import</a> <a id="360" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="384" class="Keyword">open</a> <a id="389" class="Keyword">import</a> <a id="396" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="425" class="Keyword">open</a> <a id="430" class="Keyword">import</a> <a id="437" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="474" class="Keyword">open</a> <a id="479" class="Keyword">import</a> <a id="486" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="502" class="Keyword">open</a> <a id="507" class="Keyword">import</a> <a id="514" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="542" class="Keyword">open</a> <a id="547" class="Keyword">import</a> <a id="554" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="574" class="Keyword">open</a> <a id="579" class="Keyword">import</a> <a id="586" href="group-theory.symmetric-groups.html" class="Module">group-theory.symmetric-groups</a>

<a id="617" class="Keyword">open</a> <a id="622" class="Keyword">import</a> <a id="629" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="669" class="Keyword">open</a> <a id="674" class="Keyword">import</a> <a id="681" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>

<a id="719" class="Keyword">open</a> <a id="724" class="Keyword">import</a> <a id="731" href="univalent-combinatorics.equality-standard-finite-types.html" class="Module">univalent-combinatorics.equality-standard-finite-types</a>
<a id="786" class="Keyword">open</a> <a id="791" class="Keyword">import</a> <a id="798" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Idea

The type of groups of order 2 is contractible

## Definitions

### The type of groups of order 2

<pre class="Agda"><a id="Group-of-Order-2"></a><a id="964" href="finite-group-theory.groups-of-order-2.html#964" class="Function">Group-of-Order-2</a> <a id="981" class="Symbol">:</a> <a id="983" class="Symbol">(</a><a id="984" href="finite-group-theory.groups-of-order-2.html#984" class="Bound">l</a> <a id="986" class="Symbol">:</a> <a id="988" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="993" class="Symbol">)</a> <a id="995" class="Symbol">→</a> <a id="997" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1000" class="Symbol">(</a><a id="1001" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1006" href="finite-group-theory.groups-of-order-2.html#984" class="Bound">l</a><a id="1007" class="Symbol">)</a>
<a id="1009" href="finite-group-theory.groups-of-order-2.html#964" class="Function">Group-of-Order-2</a> <a id="1026" href="finite-group-theory.groups-of-order-2.html#1026" class="Bound">l</a> <a id="1028" class="Symbol">=</a> <a id="1030" href="finite-group-theory.finite-groups.html#2126" class="Function">Group-of-Order</a> <a id="1045" href="finite-group-theory.groups-of-order-2.html#1026" class="Bound">l</a> <a id="1047" class="Number">2</a>

<a id="1050" class="Keyword">module</a> <a id="1057" href="finite-group-theory.groups-of-order-2.html#1057" class="Module">_</a>
  <a id="1061" class="Symbol">{</a><a id="1062" href="finite-group-theory.groups-of-order-2.html#1062" class="Bound">l</a> <a id="1064" class="Symbol">:</a> <a id="1066" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1071" class="Symbol">}</a> <a id="1073" class="Symbol">(</a><a id="1074" href="finite-group-theory.groups-of-order-2.html#1074" class="Bound">G</a> <a id="1076" class="Symbol">:</a> <a id="1078" href="finite-group-theory.groups-of-order-2.html#964" class="Function">Group-of-Order-2</a> <a id="1095" href="finite-group-theory.groups-of-order-2.html#1062" class="Bound">l</a><a id="1096" class="Symbol">)</a>
  <a id="1100" class="Keyword">where</a>

  <a id="1109" href="finite-group-theory.groups-of-order-2.html#1109" class="Function">group-Group-of-Order-2</a> <a id="1132" class="Symbol">:</a> <a id="1134" href="group-theory.groups.html#2398" class="Function">Group</a> <a id="1140" href="finite-group-theory.groups-of-order-2.html#1062" class="Bound">l</a>
  <a id="1144" href="finite-group-theory.groups-of-order-2.html#1109" class="Function">group-Group-of-Order-2</a> <a id="1167" class="Symbol">=</a> <a id="1169" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1173" href="finite-group-theory.groups-of-order-2.html#1074" class="Bound">G</a>

  <a id="1178" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a> <a id="1200" class="Symbol">:</a> <a id="1202" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1205" href="finite-group-theory.groups-of-order-2.html#1062" class="Bound">l</a>
  <a id="1209" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a> <a id="1231" class="Symbol">=</a> <a id="1233" href="group-theory.groups.html#2641" class="Function">type-Group</a> <a id="1244" href="finite-group-theory.groups-of-order-2.html#1109" class="Function">group-Group-of-Order-2</a>

  <a id="1270" href="finite-group-theory.groups-of-order-2.html#1270" class="Function">is-set-type-Group-of-Order-2</a> <a id="1299" class="Symbol">:</a> <a id="1301" href="foundation-core.sets.html#1099" class="Function">is-set</a> <a id="1308" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a>
  <a id="1332" href="finite-group-theory.groups-of-order-2.html#1270" class="Function">is-set-type-Group-of-Order-2</a> <a id="1361" class="Symbol">=</a> <a id="1363" href="group-theory.groups.html#2693" class="Function">is-set-type-Group</a> <a id="1381" href="finite-group-theory.groups-of-order-2.html#1109" class="Function">group-Group-of-Order-2</a>

  <a id="1407" href="finite-group-theory.groups-of-order-2.html#1407" class="Function">mul-Group-of-Order-2</a> <a id="1428" class="Symbol">:</a> <a id="1430" class="Symbol">(</a><a id="1431" href="finite-group-theory.groups-of-order-2.html#1431" class="Bound">x</a> <a id="1433" href="finite-group-theory.groups-of-order-2.html#1433" class="Bound">y</a> <a id="1435" class="Symbol">:</a> <a id="1437" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a><a id="1458" class="Symbol">)</a> <a id="1460" class="Symbol">→</a> <a id="1462" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a>
  <a id="1486" href="finite-group-theory.groups-of-order-2.html#1407" class="Function">mul-Group-of-Order-2</a> <a id="1507" class="Symbol">=</a> <a id="1509" href="group-theory.groups.html#2886" class="Function">mul-Group</a> <a id="1519" href="finite-group-theory.groups-of-order-2.html#1109" class="Function">group-Group-of-Order-2</a>

  <a id="1545" href="finite-group-theory.groups-of-order-2.html#1545" class="Function">unit-Group-of-Order-2</a> <a id="1567" class="Symbol">:</a> <a id="1569" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a>
  <a id="1593" href="finite-group-theory.groups-of-order-2.html#1545" class="Function">unit-Group-of-Order-2</a> <a id="1615" class="Symbol">=</a> <a id="1617" href="group-theory.groups.html#3677" class="Function">unit-Group</a> <a id="1628" href="finite-group-theory.groups-of-order-2.html#1109" class="Function">group-Group-of-Order-2</a>

  <a id="1654" href="finite-group-theory.groups-of-order-2.html#1654" class="Function">has-cardinality-2-Group-of-Order-2</a> <a id="1689" class="Symbol">:</a>
    <a id="1695" href="univalent-combinatorics.finite-types.html#4443" class="Function">has-cardinality</a> <a id="1711" class="Number">2</a> <a id="1713" class="Symbol">(</a><a id="1714" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a><a id="1735" class="Symbol">)</a>
  <a id="1739" href="finite-group-theory.groups-of-order-2.html#1654" class="Function">has-cardinality-2-Group-of-Order-2</a> <a id="1774" class="Symbol">=</a> <a id="1776" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1780" href="finite-group-theory.groups-of-order-2.html#1074" class="Bound">G</a>

  <a id="1785" href="finite-group-theory.groups-of-order-2.html#1785" class="Function">2-element-type-Group-of-Order-2</a> <a id="1817" class="Symbol">:</a> <a id="1819" href="univalent-combinatorics.2-element-types.html#4709" class="Function">2-Element-Type</a> <a id="1834" href="finite-group-theory.groups-of-order-2.html#1062" class="Bound">l</a>
  <a id="1838" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1842" href="finite-group-theory.groups-of-order-2.html#1785" class="Function">2-element-type-Group-of-Order-2</a> <a id="1874" class="Symbol">=</a> <a id="1876" href="finite-group-theory.groups-of-order-2.html#1178" class="Function">type-Group-of-Order-2</a>
  <a id="1900" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1904" href="finite-group-theory.groups-of-order-2.html#1785" class="Function">2-element-type-Group-of-Order-2</a> <a id="1936" class="Symbol">=</a> <a id="1938" href="finite-group-theory.groups-of-order-2.html#1654" class="Function">has-cardinality-2-Group-of-Order-2</a>
</pre>
### The group ℤ/2 of order 2

<pre class="Agda"><a id="ℤ-Mod-2-Group-of-Order-2"></a><a id="2016" href="finite-group-theory.groups-of-order-2.html#2016" class="Function">ℤ-Mod-2-Group-of-Order-2</a> <a id="2041" class="Symbol">:</a> <a id="2043" href="finite-group-theory.groups-of-order-2.html#964" class="Function">Group-of-Order-2</a> <a id="2060" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="2066" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2070" href="finite-group-theory.groups-of-order-2.html#2016" class="Function">ℤ-Mod-2-Group-of-Order-2</a> <a id="2095" class="Symbol">=</a> <a id="2097" href="elementary-number-theory.groups-of-modular-arithmetic.html#991" class="Function">ℤ-Mod-Group</a> <a id="2109" class="Number">2</a>
<a id="2111" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2115" href="finite-group-theory.groups-of-order-2.html#2016" class="Function">ℤ-Mod-2-Group-of-Order-2</a> <a id="2140" class="Symbol">=</a> <a id="2142" href="foundation.mere-equivalences.html#1762" class="Function">refl-mere-equiv</a> <a id="2158" class="Symbol">(</a><a id="2159" href="univalent-combinatorics.standard-finite-types.html#2085" class="Function">Fin</a> <a id="2163" class="Number">2</a><a id="2164" class="Symbol">)</a>
</pre>
### The permutation group S₂ of order 2

<pre class="Agda"><a id="symmetric-Group-of-Order-2"></a><a id="2220" href="finite-group-theory.groups-of-order-2.html#2220" class="Function">symmetric-Group-of-Order-2</a> <a id="2247" class="Symbol">:</a> <a id="2249" class="Symbol">(</a><a id="2250" href="finite-group-theory.groups-of-order-2.html#2250" class="Bound">l</a> <a id="2252" class="Symbol">:</a> <a id="2254" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2259" class="Symbol">)</a> <a id="2261" class="Symbol">→</a> <a id="2263" href="finite-group-theory.groups-of-order-2.html#964" class="Function">Group-of-Order-2</a> <a id="2280" href="finite-group-theory.groups-of-order-2.html#2250" class="Bound">l</a>
<a id="2282" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2286" class="Symbol">(</a><a id="2287" href="finite-group-theory.groups-of-order-2.html#2220" class="Function">symmetric-Group-of-Order-2</a> <a id="2314" href="finite-group-theory.groups-of-order-2.html#2314" class="Bound">l</a><a id="2315" class="Symbol">)</a> <a id="2317" class="Symbol">=</a> <a id="2319" href="group-theory.symmetric-groups.html#2105" class="Function">symmetric-Group</a> <a id="2335" class="Symbol">(</a><a id="2336" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2341" class="Symbol">(</a><a id="2342" href="univalent-combinatorics.standard-finite-types.html#2999" class="Function">raise-Fin</a> <a id="2352" href="finite-group-theory.groups-of-order-2.html#2314" class="Bound">l</a> <a id="2354" class="Number">2</a><a id="2355" class="Symbol">)</a> <a id="2357" class="Hole">{!!}</a><a id="2361" class="Symbol">)</a>
<a id="2363" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2367" class="Symbol">(</a><a id="2368" href="finite-group-theory.groups-of-order-2.html#2220" class="Function">symmetric-Group-of-Order-2</a> <a id="2395" href="finite-group-theory.groups-of-order-2.html#2395" class="Bound">l</a><a id="2396" class="Symbol">)</a> <a id="2398" class="Symbol">=</a> <a id="2400" class="Hole">{!!}</a>
<a id="2405" class="Comment">--  unit-trunc-Prop (inv-equiv equiv-ev-zero-aut-Fin-two-ℕ)</a>
</pre>
## Properties

### The type of groups of order 2 is contractible

<pre class="Agda"><a id="is-contr-Group-of-Order-2"></a><a id="2544" href="finite-group-theory.groups-of-order-2.html#2544" class="Function">is-contr-Group-of-Order-2</a> <a id="2570" class="Symbol">:</a> <a id="2572" class="Symbol">(</a><a id="2573" href="finite-group-theory.groups-of-order-2.html#2573" class="Bound">l</a> <a id="2575" class="Symbol">:</a> <a id="2577" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2582" class="Symbol">)</a> <a id="2584" class="Symbol">→</a> <a id="2586" href="foundation-core.contractible-types.html#925" class="Function">is-contr</a> <a id="2595" class="Symbol">(</a><a id="2596" href="finite-group-theory.groups-of-order-2.html#964" class="Function">Group-of-Order-2</a> <a id="2613" href="finite-group-theory.groups-of-order-2.html#2573" class="Bound">l</a><a id="2614" class="Symbol">)</a>
<a id="2616" href="finite-group-theory.groups-of-order-2.html#2544" class="Function">is-contr-Group-of-Order-2</a> <a id="2642" href="finite-group-theory.groups-of-order-2.html#2642" class="Bound">l</a> <a id="2644" class="Symbol">=</a> <a id="2646" class="Hole">{!!}</a>
</pre>