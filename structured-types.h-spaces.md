---
title: H-spaces
---

<pre class="Agda"><a id="34" class="Symbol">{-#</a> <a id="38" class="Keyword">OPTIONS</a> <a id="46" class="Pragma">--without-K</a> <a id="58" class="Pragma">--exact-split</a> <a id="72" class="Symbol">#-}</a>

<a id="77" class="Keyword">module</a> <a id="84" href="structured-types.h-spaces.html" class="Module">structured-types.h-spaces</a> <a id="110" class="Keyword">where</a>

<a id="117" class="Keyword">open</a> <a id="122" class="Keyword">import</a> <a id="129" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="164" class="Keyword">open</a> <a id="169" class="Keyword">import</a> <a id="176" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="208" class="Keyword">open</a> <a id="213" class="Keyword">import</a> <a id="220" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="275" class="Keyword">open</a> <a id="280" class="Keyword">import</a> <a id="287" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="313" class="Keyword">open</a> <a id="318" class="Keyword">import</a> <a id="325" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="353" class="Keyword">open</a> <a id="358" class="Keyword">import</a> <a id="365" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
</pre>
## Idea

An H-space is a pointed type `A` equipped with a binary operation `μ` and homotopies `(λ x → μ pt x) ~ id` and `λ x → μ x pt ~ id`. If `A` is a connected H-space, then `λ x → μ a x` and `λ x → μ x a` are equivalences for each `a : A`.

## Definitions

<pre class="Agda"><a id="h-space-structure"></a><a id="670" href="structured-types.h-spaces.html#670" class="Function">h-space-structure</a> <a id="688" class="Symbol">:</a>
  <a id="692" class="Symbol">{</a><a id="693" href="structured-types.h-spaces.html#693" class="Bound">l</a> <a id="695" class="Symbol">:</a> <a id="697" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="702" class="Symbol">}</a> <a id="704" class="Symbol">(</a><a id="705" href="structured-types.h-spaces.html#705" class="Bound">A</a> <a id="707" class="Symbol">:</a> <a id="709" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="722" href="structured-types.h-spaces.html#693" class="Bound">l</a><a id="723" class="Symbol">)</a> <a id="725" class="Symbol">→</a> <a id="727" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="730" href="structured-types.h-spaces.html#693" class="Bound">l</a>
<a id="732" href="structured-types.h-spaces.html#670" class="Function">h-space-structure</a> <a id="750" href="structured-types.h-spaces.html#750" class="Bound">A</a> <a id="752" class="Symbol">=</a>
  <a id="756" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="758" class="Symbol">(</a> <a id="760" class="Symbol">(</a><a id="761" href="structured-types.h-spaces.html#761" class="Bound">x</a> <a id="763" href="structured-types.h-spaces.html#763" class="Bound">y</a> <a id="765" class="Symbol">:</a> <a id="767" href="structured-types.pointed-types.html#518" class="Function">type-Pointed-Type</a> <a id="785" href="structured-types.h-spaces.html#750" class="Bound">A</a><a id="786" class="Symbol">)</a> <a id="788" class="Symbol">→</a> <a id="790" href="structured-types.pointed-types.html#518" class="Function">type-Pointed-Type</a> <a id="808" href="structured-types.h-spaces.html#750" class="Bound">A</a><a id="809" class="Symbol">)</a>
    <a id="815" class="Symbol">(</a> <a id="817" class="Symbol">λ</a> <a id="819" href="structured-types.h-spaces.html#819" class="Bound">μ</a> <a id="821" class="Symbol">→</a>
      <a id="829" class="Symbol">(</a> <a id="831" href="structured-types.h-spaces.html#819" class="Bound">μ</a> <a id="833" class="Symbol">(</a><a id="834" href="structured-types.pointed-types.html#576" class="Function">pt-Pointed-Type</a> <a id="850" href="structured-types.h-spaces.html#750" class="Bound">A</a><a id="851" class="Symbol">)</a> <a id="853" href="foundation-core.homotopies.html#545" class="Function Operator">~</a> <a id="855" href="foundation-core.functions.html#309" class="Function">id</a><a id="857" class="Symbol">)</a> <a id="859" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a>
      <a id="867" class="Symbol">(</a> <a id="869" class="Symbol">(λ</a> <a id="872" href="structured-types.h-spaces.html#872" class="Bound">x</a> <a id="874" class="Symbol">→</a> <a id="876" href="structured-types.h-spaces.html#819" class="Bound">μ</a> <a id="878" href="structured-types.h-spaces.html#872" class="Bound">x</a> <a id="880" class="Symbol">(</a><a id="881" href="structured-types.pointed-types.html#576" class="Function">pt-Pointed-Type</a> <a id="897" href="structured-types.h-spaces.html#750" class="Bound">A</a><a id="898" class="Symbol">))</a> <a id="901" href="foundation-core.homotopies.html#545" class="Function Operator">~</a> <a id="903" href="foundation-core.functions.html#309" class="Function">id</a><a id="905" class="Symbol">))</a>

<a id="H-Space"></a><a id="909" href="structured-types.h-spaces.html#909" class="Function">H-Space</a> <a id="917" class="Symbol">:</a> <a id="919" class="Symbol">(</a><a id="920" href="structured-types.h-spaces.html#920" class="Bound">l</a> <a id="922" class="Symbol">:</a> <a id="924" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="929" class="Symbol">)</a> <a id="931" class="Symbol">→</a> <a id="933" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="936" class="Symbol">(</a><a id="937" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="942" href="structured-types.h-spaces.html#920" class="Bound">l</a><a id="943" class="Symbol">)</a>
<a id="945" href="structured-types.h-spaces.html#909" class="Function">H-Space</a> <a id="953" href="structured-types.h-spaces.html#953" class="Bound">l</a> <a id="955" class="Symbol">=</a> <a id="957" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="959" class="Symbol">(</a><a id="960" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="973" href="structured-types.h-spaces.html#953" class="Bound">l</a><a id="974" class="Symbol">)</a> <a id="976" href="structured-types.h-spaces.html#670" class="Function">h-space-structure</a>

<a id="995" class="Keyword">module</a> <a id="1002" href="structured-types.h-spaces.html#1002" class="Module">_</a>
  <a id="1006" class="Symbol">{</a><a id="1007" href="structured-types.h-spaces.html#1007" class="Bound">l</a> <a id="1009" class="Symbol">:</a> <a id="1011" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1016" class="Symbol">}</a> <a id="1018" class="Symbol">(</a><a id="1019" href="structured-types.h-spaces.html#1019" class="Bound">A</a> <a id="1021" class="Symbol">:</a> <a id="1023" href="structured-types.h-spaces.html#909" class="Function">H-Space</a> <a id="1031" href="structured-types.h-spaces.html#1007" class="Bound">l</a><a id="1032" class="Symbol">)</a>
  <a id="1036" class="Keyword">where</a>

  <a id="1045" href="structured-types.h-spaces.html#1045" class="Function">pointed-type-H-Space</a> <a id="1066" class="Symbol">:</a> <a id="1068" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="1081" href="structured-types.h-spaces.html#1007" class="Bound">l</a>
  <a id="1085" href="structured-types.h-spaces.html#1045" class="Function">pointed-type-H-Space</a> <a id="1106" class="Symbol">=</a> <a id="1108" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1112" href="structured-types.h-spaces.html#1019" class="Bound">A</a>

  <a id="1117" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a> <a id="1130" class="Symbol">:</a> <a id="1132" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1135" href="structured-types.h-spaces.html#1007" class="Bound">l</a>
  <a id="1139" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a> <a id="1152" class="Symbol">=</a> <a id="1154" href="structured-types.pointed-types.html#518" class="Function">type-Pointed-Type</a> <a id="1172" href="structured-types.h-spaces.html#1045" class="Function">pointed-type-H-Space</a>

  <a id="1196" href="structured-types.h-spaces.html#1196" class="Function">pt-H-Space</a> <a id="1207" class="Symbol">:</a> <a id="1209" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a>
  <a id="1224" href="structured-types.h-spaces.html#1196" class="Function">pt-H-Space</a> <a id="1235" class="Symbol">=</a> <a id="1237" href="structured-types.pointed-types.html#576" class="Function">pt-Pointed-Type</a> <a id="1253" href="structured-types.h-spaces.html#1045" class="Function">pointed-type-H-Space</a>

  <a id="1277" href="structured-types.h-spaces.html#1277" class="Function">mul-H-Space</a> <a id="1289" class="Symbol">:</a> <a id="1291" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a> <a id="1304" class="Symbol">→</a> <a id="1306" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a> <a id="1319" class="Symbol">→</a> <a id="1321" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a>
  <a id="1336" href="structured-types.h-spaces.html#1277" class="Function">mul-H-Space</a> <a id="1348" class="Symbol">=</a> <a id="1350" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1354" class="Symbol">(</a><a id="1355" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1359" href="structured-types.h-spaces.html#1019" class="Bound">A</a><a id="1360" class="Symbol">)</a>

  <a id="1365" href="structured-types.h-spaces.html#1365" class="Function">left-unit-law-mul-H-Space</a> <a id="1391" class="Symbol">:</a>
    <a id="1397" class="Symbol">(</a><a id="1398" href="structured-types.h-spaces.html#1398" class="Bound">x</a> <a id="1400" class="Symbol">:</a> <a id="1402" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a><a id="1414" class="Symbol">)</a> <a id="1416" class="Symbol">→</a> <a id="1418" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1421" class="Symbol">(</a><a id="1422" href="structured-types.h-spaces.html#1277" class="Function">mul-H-Space</a> <a id="1434" href="structured-types.h-spaces.html#1196" class="Function">pt-H-Space</a> <a id="1445" href="structured-types.h-spaces.html#1398" class="Bound">x</a><a id="1446" class="Symbol">)</a> <a id="1448" href="structured-types.h-spaces.html#1398" class="Bound">x</a>
  <a id="1452" href="structured-types.h-spaces.html#1365" class="Function">left-unit-law-mul-H-Space</a> <a id="1478" class="Symbol">=</a> <a id="1480" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1484" class="Symbol">(</a><a id="1485" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1489" class="Symbol">(</a><a id="1490" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1494" href="structured-types.h-spaces.html#1019" class="Bound">A</a><a id="1495" class="Symbol">))</a>

  <a id="1501" href="structured-types.h-spaces.html#1501" class="Function">right-unit-law-mul-H-Space</a> <a id="1528" class="Symbol">:</a>
    <a id="1534" class="Symbol">(</a><a id="1535" href="structured-types.h-spaces.html#1535" class="Bound">x</a> <a id="1537" class="Symbol">:</a> <a id="1539" href="structured-types.h-spaces.html#1117" class="Function">type-H-Space</a><a id="1551" class="Symbol">)</a> <a id="1553" class="Symbol">→</a> <a id="1555" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1558" class="Symbol">(</a><a id="1559" href="structured-types.h-spaces.html#1277" class="Function">mul-H-Space</a> <a id="1571" href="structured-types.h-spaces.html#1535" class="Bound">x</a> <a id="1573" href="structured-types.h-spaces.html#1196" class="Function">pt-H-Space</a><a id="1583" class="Symbol">)</a> <a id="1585" href="structured-types.h-spaces.html#1535" class="Bound">x</a>
  <a id="1589" href="structured-types.h-spaces.html#1501" class="Function">right-unit-law-mul-H-Space</a> <a id="1616" class="Symbol">=</a> <a id="1618" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1622" class="Symbol">(</a><a id="1623" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1627" class="Symbol">(</a><a id="1628" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1632" href="structured-types.h-spaces.html#1019" class="Bound">A</a><a id="1633" class="Symbol">))</a>
</pre>
## Properties