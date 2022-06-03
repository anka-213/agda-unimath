---
title: Inverse semigroups
---

<pre class="Agda"><a id="44" class="Symbol">{-#</a> <a id="48" class="Keyword">OPTIONS</a> <a id="56" class="Pragma">--without-K</a> <a id="68" class="Pragma">--exact-split</a> <a id="82" class="Symbol">#-}</a>

<a id="87" class="Keyword">module</a> <a id="94" href="group-theory.inverse-semigroups.html" class="Module">group-theory.inverse-semigroups</a> <a id="126" class="Keyword">where</a>

<a id="133" class="Keyword">open</a> <a id="138" class="Keyword">import</a> <a id="145" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a> <a id="180" class="Keyword">using</a> <a id="186" class="Symbol">(</a><a id="187" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">_×_</a><a id="190" class="Symbol">)</a>
<a id="192" class="Keyword">open</a> <a id="197" class="Keyword">import</a> <a id="204" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a> <a id="234" class="Keyword">using</a> <a id="240" class="Symbol">(</a><a id="241" href="foundation-core.contractible-types.html#992" class="Function">is-contr</a><a id="249" class="Symbol">;</a> <a id="251" href="foundation-core.contractible-types.html#1085" class="Function">center</a><a id="257" class="Symbol">)</a>
<a id="259" class="Keyword">open</a> <a id="264" class="Keyword">import</a> <a id="271" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="303" class="Keyword">using</a> <a id="309" class="Symbol">(</a><a id="310" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="311" class="Symbol">;</a> <a id="313" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="317" class="Symbol">;</a> <a id="319" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="322" class="Symbol">;</a> <a id="324" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="327" class="Symbol">)</a>
<a id="329" class="Keyword">open</a> <a id="334" class="Keyword">import</a> <a id="341" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="367" class="Keyword">using</a> <a id="373" class="Symbol">(</a><a id="374" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="376" class="Symbol">)</a>
<a id="378" class="Keyword">open</a> <a id="383" class="Keyword">import</a> <a id="390" href="foundation.sets.html" class="Module">foundation.sets</a> <a id="406" class="Keyword">using</a> <a id="412" class="Symbol">(</a><a id="413" href="foundation-core.sets.html#1177" class="Function">UU-Set</a><a id="419" class="Symbol">;</a> <a id="421" href="foundation-core.sets.html#1099" class="Function">is-set</a><a id="427" class="Symbol">)</a>
<a id="429" class="Keyword">open</a> <a id="434" class="Keyword">import</a> <a id="441" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="468" class="Keyword">using</a> <a id="474" class="Symbol">(</a><a id="475" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="480" class="Symbol">;</a> <a id="482" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="484" class="Symbol">;</a> <a id="486" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="490" class="Symbol">)</a>

<a id="493" class="Keyword">open</a> <a id="498" class="Keyword">import</a> <a id="505" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a> <a id="529" class="Keyword">using</a>
  <a id="537" class="Symbol">(</a> <a id="539" href="group-theory.semigroups.html#737" class="Function">Semigroup</a><a id="548" class="Symbol">;</a> <a id="550" href="group-theory.semigroups.html#881" class="Function">set-Semigroup</a><a id="563" class="Symbol">;</a> <a id="565" href="group-theory.semigroups.html#933" class="Function">type-Semigroup</a><a id="579" class="Symbol">;</a> <a id="581" href="group-theory.semigroups.html#1000" class="Function">is-set-type-Semigroup</a><a id="602" class="Symbol">;</a>
    <a id="608" href="group-theory.semigroups.html#1215" class="Function">mul-Semigroup</a><a id="621" class="Symbol">;</a> <a id="623" href="group-theory.semigroups.html#1335" class="Function">mul-Semigroup&#39;</a><a id="637" class="Symbol">;</a> <a id="639" href="group-theory.semigroups.html#1445" class="Function">associative-mul-Semigroup</a><a id="664" class="Symbol">)</a>
</pre>
## Idea

An inverse semigroup is an algebraic structure that models partial bijections. In an inverse semigroup, elements have unique inverses in the sense that for each `x` there is a unique `y` such that `xyx = x` and `yxy = y`.

## Definition

<pre class="Agda"><a id="is-inverse-Semigroup"></a><a id="926" href="group-theory.inverse-semigroups.html#926" class="Function">is-inverse-Semigroup</a> <a id="947" class="Symbol">:</a>
  <a id="951" class="Symbol">{</a><a id="952" href="group-theory.inverse-semigroups.html#952" class="Bound">l</a> <a id="954" class="Symbol">:</a> <a id="956" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="961" class="Symbol">}</a> <a id="963" class="Symbol">(</a><a id="964" href="group-theory.inverse-semigroups.html#964" class="Bound">S</a> <a id="966" class="Symbol">:</a> <a id="968" href="group-theory.semigroups.html#737" class="Function">Semigroup</a> <a id="978" href="group-theory.inverse-semigroups.html#952" class="Bound">l</a><a id="979" class="Symbol">)</a> <a id="981" class="Symbol">→</a> <a id="983" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="986" href="group-theory.inverse-semigroups.html#952" class="Bound">l</a>
<a id="988" href="group-theory.inverse-semigroups.html#926" class="Function">is-inverse-Semigroup</a> <a id="1009" href="group-theory.inverse-semigroups.html#1009" class="Bound">S</a> <a id="1011" class="Symbol">=</a>
  <a id="1015" class="Symbol">(</a><a id="1016" href="group-theory.inverse-semigroups.html#1016" class="Bound">x</a> <a id="1018" class="Symbol">:</a> <a id="1020" href="group-theory.semigroups.html#933" class="Function">type-Semigroup</a> <a id="1035" href="group-theory.inverse-semigroups.html#1009" class="Bound">S</a><a id="1036" class="Symbol">)</a> <a id="1038" class="Symbol">→</a>
  <a id="1042" href="foundation-core.contractible-types.html#992" class="Function">is-contr</a>
    <a id="1055" class="Symbol">(</a> <a id="1057" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1059" class="Symbol">(</a> <a id="1061" href="group-theory.semigroups.html#933" class="Function">type-Semigroup</a> <a id="1076" href="group-theory.inverse-semigroups.html#1009" class="Bound">S</a><a id="1077" class="Symbol">)</a>
        <a id="1087" class="Symbol">(</a> <a id="1089" class="Symbol">λ</a> <a id="1091" href="group-theory.inverse-semigroups.html#1091" class="Bound">y</a> <a id="1093" class="Symbol">→</a>
          <a id="1105" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1108" class="Symbol">(</a><a id="1109" href="group-theory.semigroups.html#1215" class="Function">mul-Semigroup</a> <a id="1123" href="group-theory.inverse-semigroups.html#1009" class="Bound">S</a> <a id="1125" class="Symbol">(</a><a id="1126" href="group-theory.semigroups.html#1215" class="Function">mul-Semigroup</a> <a id="1140" href="group-theory.inverse-semigroups.html#1009" class="Bound">S</a> <a id="1142" href="group-theory.inverse-semigroups.html#1016" class="Bound">x</a> <a id="1144" href="group-theory.inverse-semigroups.html#1091" class="Bound">y</a><a id="1145" class="Symbol">)</a> <a id="1147" href="group-theory.inverse-semigroups.html#1016" class="Bound">x</a><a id="1148" class="Symbol">)</a> <a id="1150" href="group-theory.inverse-semigroups.html#1016" class="Bound">x</a> <a id="1152" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a>
          <a id="1164" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1167" class="Symbol">(</a><a id="1168" href="group-theory.semigroups.html#1215" class="Function">mul-Semigroup</a> <a id="1182" href="group-theory.inverse-semigroups.html#1009" class="Bound">S</a> <a id="1184" class="Symbol">(</a><a id="1185" href="group-theory.semigroups.html#1215" class="Function">mul-Semigroup</a> <a id="1199" href="group-theory.inverse-semigroups.html#1009" class="Bound">S</a> <a id="1201" href="group-theory.inverse-semigroups.html#1091" class="Bound">y</a> <a id="1203" href="group-theory.inverse-semigroups.html#1016" class="Bound">x</a><a id="1204" class="Symbol">)</a> <a id="1206" href="group-theory.inverse-semigroups.html#1091" class="Bound">y</a><a id="1207" class="Symbol">)</a> <a id="1209" href="group-theory.inverse-semigroups.html#1091" class="Bound">y</a><a id="1210" class="Symbol">))</a>

<a id="Inverse-Semigroup"></a><a id="1214" href="group-theory.inverse-semigroups.html#1214" class="Function">Inverse-Semigroup</a> <a id="1232" class="Symbol">:</a> <a id="1234" class="Symbol">(</a><a id="1235" href="group-theory.inverse-semigroups.html#1235" class="Bound">l</a> <a id="1237" class="Symbol">:</a> <a id="1239" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1244" class="Symbol">)</a> <a id="1246" class="Symbol">→</a> <a id="1248" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1251" class="Symbol">(</a><a id="1252" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1257" href="group-theory.inverse-semigroups.html#1235" class="Bound">l</a><a id="1258" class="Symbol">)</a>
<a id="1260" href="group-theory.inverse-semigroups.html#1214" class="Function">Inverse-Semigroup</a> <a id="1278" href="group-theory.inverse-semigroups.html#1278" class="Bound">l</a> <a id="1280" class="Symbol">=</a> <a id="1282" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1284" class="Symbol">(</a><a id="1285" href="group-theory.semigroups.html#737" class="Function">Semigroup</a> <a id="1295" href="group-theory.inverse-semigroups.html#1278" class="Bound">l</a><a id="1296" class="Symbol">)</a> <a id="1298" href="group-theory.inverse-semigroups.html#926" class="Function">is-inverse-Semigroup</a>

<a id="1320" class="Keyword">module</a> <a id="1327" href="group-theory.inverse-semigroups.html#1327" class="Module">_</a>
  <a id="1331" class="Symbol">{</a><a id="1332" href="group-theory.inverse-semigroups.html#1332" class="Bound">l</a> <a id="1334" class="Symbol">:</a> <a id="1336" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1341" class="Symbol">}</a> <a id="1343" class="Symbol">(</a><a id="1344" href="group-theory.inverse-semigroups.html#1344" class="Bound">S</a> <a id="1346" class="Symbol">:</a> <a id="1348" href="group-theory.inverse-semigroups.html#1214" class="Function">Inverse-Semigroup</a> <a id="1366" href="group-theory.inverse-semigroups.html#1332" class="Bound">l</a><a id="1367" class="Symbol">)</a>
  <a id="1371" class="Keyword">where</a>

  <a id="1380" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a> <a id="1408" class="Symbol">:</a> <a id="1410" href="group-theory.semigroups.html#737" class="Function">Semigroup</a> <a id="1420" href="group-theory.inverse-semigroups.html#1332" class="Bound">l</a>
  <a id="1424" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a> <a id="1452" class="Symbol">=</a> <a id="1454" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1458" href="group-theory.inverse-semigroups.html#1344" class="Bound">S</a>

  <a id="1463" href="group-theory.inverse-semigroups.html#1463" class="Function">set-Inverse-Semigroup</a> <a id="1485" class="Symbol">:</a> <a id="1487" href="foundation-core.sets.html#1177" class="Function">UU-Set</a> <a id="1494" href="group-theory.inverse-semigroups.html#1332" class="Bound">l</a>
  <a id="1498" href="group-theory.inverse-semigroups.html#1463" class="Function">set-Inverse-Semigroup</a> <a id="1520" class="Symbol">=</a> <a id="1522" href="group-theory.semigroups.html#881" class="Function">set-Semigroup</a> <a id="1536" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a>

  <a id="1567" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a> <a id="1590" class="Symbol">:</a> <a id="1592" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1595" href="group-theory.inverse-semigroups.html#1332" class="Bound">l</a>
  <a id="1599" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a> <a id="1622" class="Symbol">=</a> <a id="1624" href="group-theory.semigroups.html#933" class="Function">type-Semigroup</a> <a id="1639" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a>

  <a id="1670" href="group-theory.inverse-semigroups.html#1670" class="Function">is-set-type-Inverse-Semigroup</a> <a id="1700" class="Symbol">:</a> <a id="1702" href="foundation-core.sets.html#1099" class="Function">is-set</a> <a id="1709" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a>
  <a id="1734" href="group-theory.inverse-semigroups.html#1670" class="Function">is-set-type-Inverse-Semigroup</a> <a id="1764" class="Symbol">=</a>
    <a id="1770" href="group-theory.semigroups.html#1000" class="Function">is-set-type-Semigroup</a> <a id="1792" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a>

  <a id="1823" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="1845" class="Symbol">:</a>
    <a id="1851" class="Symbol">(</a><a id="1852" href="group-theory.inverse-semigroups.html#1852" class="Bound">x</a> <a id="1854" href="group-theory.inverse-semigroups.html#1854" class="Bound">y</a> <a id="1856" class="Symbol">:</a> <a id="1858" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a><a id="1880" class="Symbol">)</a> <a id="1882" class="Symbol">→</a> <a id="1884" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a>
  <a id="1909" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="1931" class="Symbol">=</a> <a id="1933" href="group-theory.semigroups.html#1215" class="Function">mul-Semigroup</a> <a id="1947" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a>

  <a id="1978" href="group-theory.inverse-semigroups.html#1978" class="Function">mul-Inverse-Semigroup&#39;</a> <a id="2001" class="Symbol">:</a>
    <a id="2007" class="Symbol">(</a><a id="2008" href="group-theory.inverse-semigroups.html#2008" class="Bound">x</a> <a id="2010" href="group-theory.inverse-semigroups.html#2010" class="Bound">y</a> <a id="2012" class="Symbol">:</a> <a id="2014" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a><a id="2036" class="Symbol">)</a> <a id="2038" class="Symbol">→</a> <a id="2040" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a>
  <a id="2065" href="group-theory.inverse-semigroups.html#1978" class="Function">mul-Inverse-Semigroup&#39;</a> <a id="2088" class="Symbol">=</a> <a id="2090" href="group-theory.semigroups.html#1335" class="Function">mul-Semigroup&#39;</a> <a id="2105" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a>

  <a id="2136" href="group-theory.inverse-semigroups.html#2136" class="Function">associative-mul-Inverse-Semigroup</a> <a id="2170" class="Symbol">:</a>
    <a id="2176" class="Symbol">(</a><a id="2177" href="group-theory.inverse-semigroups.html#2177" class="Bound">x</a> <a id="2179" href="group-theory.inverse-semigroups.html#2179" class="Bound">y</a> <a id="2181" href="group-theory.inverse-semigroups.html#2181" class="Bound">z</a> <a id="2183" class="Symbol">:</a> <a id="2185" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a><a id="2207" class="Symbol">)</a> <a id="2209" class="Symbol">→</a>
    <a id="2215" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="2218" class="Symbol">(</a> <a id="2220" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="2242" class="Symbol">(</a><a id="2243" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="2265" href="group-theory.inverse-semigroups.html#2177" class="Bound">x</a> <a id="2267" href="group-theory.inverse-semigroups.html#2179" class="Bound">y</a><a id="2268" class="Symbol">)</a> <a id="2270" href="group-theory.inverse-semigroups.html#2181" class="Bound">z</a><a id="2271" class="Symbol">)</a>
       <a id="2280" class="Symbol">(</a> <a id="2282" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="2304" href="group-theory.inverse-semigroups.html#2177" class="Bound">x</a> <a id="2306" class="Symbol">(</a><a id="2307" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="2329" href="group-theory.inverse-semigroups.html#2179" class="Bound">y</a> <a id="2331" href="group-theory.inverse-semigroups.html#2181" class="Bound">z</a><a id="2332" class="Symbol">))</a>
  <a id="2337" href="group-theory.inverse-semigroups.html#2136" class="Function">associative-mul-Inverse-Semigroup</a> <a id="2371" class="Symbol">=</a>
    <a id="2377" href="group-theory.semigroups.html#1445" class="Function">associative-mul-Semigroup</a> <a id="2403" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a>

  <a id="2434" href="group-theory.inverse-semigroups.html#2434" class="Function">is-inverse-semigroup-Inverse-Semigroup</a> <a id="2473" class="Symbol">:</a>
    <a id="2479" href="group-theory.inverse-semigroups.html#926" class="Function">is-inverse-Semigroup</a> <a id="2500" href="group-theory.inverse-semigroups.html#1380" class="Function">semigroup-Inverse-Semigroup</a>
  <a id="2530" href="group-theory.inverse-semigroups.html#2434" class="Function">is-inverse-semigroup-Inverse-Semigroup</a> <a id="2569" class="Symbol">=</a> <a id="2571" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2575" href="group-theory.inverse-semigroups.html#1344" class="Bound">S</a>

  <a id="2580" href="group-theory.inverse-semigroups.html#2580" class="Function">inv-Inverse-Semigroup</a> <a id="2602" class="Symbol">:</a> <a id="2604" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a> <a id="2627" class="Symbol">→</a> <a id="2629" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a>
  <a id="2654" href="group-theory.inverse-semigroups.html#2580" class="Function">inv-Inverse-Semigroup</a> <a id="2676" href="group-theory.inverse-semigroups.html#2676" class="Bound">x</a> <a id="2678" class="Symbol">=</a>
    <a id="2684" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2688" class="Symbol">(</a><a id="2689" href="foundation-core.contractible-types.html#1085" class="Function">center</a> <a id="2696" class="Symbol">(</a><a id="2697" href="group-theory.inverse-semigroups.html#2434" class="Function">is-inverse-semigroup-Inverse-Semigroup</a> <a id="2736" href="group-theory.inverse-semigroups.html#2676" class="Bound">x</a><a id="2737" class="Symbol">))</a>

  <a id="2743" href="group-theory.inverse-semigroups.html#2743" class="Function">inner-inverse-law-mul-Inverse-Semigroup</a> <a id="2783" class="Symbol">:</a>
    <a id="2789" class="Symbol">(</a><a id="2790" href="group-theory.inverse-semigroups.html#2790" class="Bound">x</a> <a id="2792" class="Symbol">:</a> <a id="2794" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a><a id="2816" class="Symbol">)</a> <a id="2818" class="Symbol">→</a>
    <a id="2824" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="2827" class="Symbol">(</a> <a id="2829" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a>
         <a id="2860" class="Symbol">(</a> <a id="2862" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="2884" href="group-theory.inverse-semigroups.html#2790" class="Bound">x</a> <a id="2886" class="Symbol">(</a><a id="2887" href="group-theory.inverse-semigroups.html#2580" class="Function">inv-Inverse-Semigroup</a> <a id="2909" href="group-theory.inverse-semigroups.html#2790" class="Bound">x</a><a id="2910" class="Symbol">))</a>
         <a id="2922" class="Symbol">(</a> <a id="2924" href="group-theory.inverse-semigroups.html#2790" class="Bound">x</a><a id="2925" class="Symbol">))</a>
       <a id="2935" class="Symbol">(</a> <a id="2937" href="group-theory.inverse-semigroups.html#2790" class="Bound">x</a><a id="2938" class="Symbol">)</a>
  <a id="2942" href="group-theory.inverse-semigroups.html#2743" class="Function">inner-inverse-law-mul-Inverse-Semigroup</a> <a id="2982" href="group-theory.inverse-semigroups.html#2982" class="Bound">x</a> <a id="2984" class="Symbol">=</a>
    <a id="2990" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2994" class="Symbol">(</a><a id="2995" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2999" class="Symbol">(</a><a id="3000" href="foundation-core.contractible-types.html#1085" class="Function">center</a> <a id="3007" class="Symbol">(</a><a id="3008" href="group-theory.inverse-semigroups.html#2434" class="Function">is-inverse-semigroup-Inverse-Semigroup</a> <a id="3047" href="group-theory.inverse-semigroups.html#2982" class="Bound">x</a><a id="3048" class="Symbol">)))</a>

  <a id="3055" href="group-theory.inverse-semigroups.html#3055" class="Function">outer-inverse-law-mul-Inverse-Semigroup</a> <a id="3095" class="Symbol">:</a>
    <a id="3101" class="Symbol">(</a><a id="3102" href="group-theory.inverse-semigroups.html#3102" class="Bound">x</a> <a id="3104" class="Symbol">:</a> <a id="3106" href="group-theory.inverse-semigroups.html#1567" class="Function">type-Inverse-Semigroup</a><a id="3128" class="Symbol">)</a> <a id="3130" class="Symbol">→</a>
    <a id="3136" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="3139" class="Symbol">(</a> <a id="3141" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a>
         <a id="3172" class="Symbol">(</a> <a id="3174" href="group-theory.inverse-semigroups.html#1823" class="Function">mul-Inverse-Semigroup</a> <a id="3196" class="Symbol">(</a><a id="3197" href="group-theory.inverse-semigroups.html#2580" class="Function">inv-Inverse-Semigroup</a> <a id="3219" href="group-theory.inverse-semigroups.html#3102" class="Bound">x</a><a id="3220" class="Symbol">)</a> <a id="3222" href="group-theory.inverse-semigroups.html#3102" class="Bound">x</a><a id="3223" class="Symbol">)</a>
         <a id="3234" class="Symbol">(</a> <a id="3236" href="group-theory.inverse-semigroups.html#2580" class="Function">inv-Inverse-Semigroup</a> <a id="3258" href="group-theory.inverse-semigroups.html#3102" class="Bound">x</a><a id="3259" class="Symbol">))</a>
       <a id="3269" class="Symbol">(</a> <a id="3271" href="group-theory.inverse-semigroups.html#2580" class="Function">inv-Inverse-Semigroup</a> <a id="3293" href="group-theory.inverse-semigroups.html#3102" class="Bound">x</a><a id="3294" class="Symbol">)</a>
  <a id="3298" href="group-theory.inverse-semigroups.html#3055" class="Function">outer-inverse-law-mul-Inverse-Semigroup</a> <a id="3338" href="group-theory.inverse-semigroups.html#3338" class="Bound">x</a> <a id="3340" class="Symbol">=</a>
    <a id="3346" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="3350" class="Symbol">(</a><a id="3351" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="3355" class="Symbol">(</a><a id="3356" href="foundation-core.contractible-types.html#1085" class="Function">center</a> <a id="3363" class="Symbol">(</a><a id="3364" href="group-theory.inverse-semigroups.html#2434" class="Function">is-inverse-semigroup-Inverse-Semigroup</a> <a id="3403" href="group-theory.inverse-semigroups.html#3338" class="Bound">x</a><a id="3404" class="Symbol">)))</a>
</pre>