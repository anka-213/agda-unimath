---
title: Wedges of types
---

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="synthetic-homotopy-theory.wedges-of-pointed-types.html" class="Module">synthetic-homotopy-theory.wedges-of-pointed-types</a> <a id="141" class="Keyword">where</a>

<a id="148" class="Keyword">open</a> <a id="153" class="Keyword">import</a> <a id="160" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="195" class="Keyword">open</a> <a id="200" class="Keyword">import</a> <a id="207" href="foundation.constant-maps.html" class="Module">foundation.constant-maps</a>
<a id="232" class="Keyword">open</a> <a id="237" class="Keyword">import</a> <a id="244" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="276" class="Keyword">open</a> <a id="281" class="Keyword">import</a> <a id="288" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="312" class="Keyword">open</a> <a id="317" class="Keyword">import</a> <a id="324" href="foundation.homotopies.html" class="Module">foundation.homotopies</a>
<a id="346" class="Keyword">open</a> <a id="351" class="Keyword">import</a> <a id="358" href="foundation.unit-type.html" class="Module">foundation.unit-type</a>
<a id="379" class="Keyword">open</a> <a id="384" class="Keyword">import</a> <a id="391" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="419" class="Keyword">open</a> <a id="424" class="Keyword">import</a> <a id="431" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>

<a id="463" class="Keyword">open</a> <a id="468" class="Keyword">import</a> <a id="475" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a>
<a id="513" class="Keyword">open</a> <a id="518" class="Keyword">import</a> <a id="525" href="synthetic-homotopy-theory.cofibers.html" class="Module">synthetic-homotopy-theory.cofibers</a>
</pre>
<pre class="Agda"><a id="_∨_"></a><a id="573" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#573" class="Function Operator">_∨_</a> <a id="577" class="Symbol">:</a>
  <a id="581" class="Symbol">{</a><a id="582" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#582" class="Bound">l1</a> <a id="585" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#585" class="Bound">l2</a> <a id="588" class="Symbol">:</a> <a id="590" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="595" class="Symbol">}</a> <a id="597" class="Symbol">(</a><a id="598" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#598" class="Bound">A</a> <a id="600" class="Symbol">:</a> <a id="602" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="615" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#582" class="Bound">l1</a><a id="617" class="Symbol">)</a> <a id="619" class="Symbol">(</a><a id="620" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#620" class="Bound">B</a> <a id="622" class="Symbol">:</a> <a id="624" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="637" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#585" class="Bound">l2</a><a id="639" class="Symbol">)</a> <a id="641" class="Symbol">→</a> <a id="643" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="656" class="Symbol">(</a><a id="657" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#582" class="Bound">l1</a> <a id="660" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="662" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#585" class="Bound">l2</a><a id="664" class="Symbol">)</a>
<a id="666" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#666" class="Bound">A</a> <a id="668" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#573" class="Function Operator">∨</a> <a id="670" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#670" class="Bound">B</a> <a id="672" class="Symbol">=</a>
  <a id="676" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
    <a id="685" class="Symbol">(</a> <a id="687" href="synthetic-homotopy-theory.24-pushouts.html#11039" class="Postulate">pushout</a>
      <a id="701" class="Symbol">(</a> <a id="703" href="foundation-core.constant-maps.html#203" class="Function">const</a> <a id="709" href="foundation.unit-type.html#1075" class="Datatype">unit</a> <a id="714" class="Symbol">(</a><a id="715" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="719" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#666" class="Bound">A</a><a id="720" class="Symbol">)</a> <a id="722" class="Symbol">(</a><a id="723" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="727" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#666" class="Bound">A</a><a id="728" class="Symbol">))</a>
      <a id="737" class="Symbol">(</a> <a id="739" href="foundation-core.constant-maps.html#203" class="Function">const</a> <a id="745" href="foundation.unit-type.html#1075" class="Datatype">unit</a> <a id="750" class="Symbol">(</a><a id="751" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="755" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#670" class="Bound">B</a><a id="756" class="Symbol">)</a> <a id="758" class="Symbol">(</a><a id="759" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="763" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#670" class="Bound">B</a><a id="764" class="Symbol">)))</a>
    <a id="772" class="Symbol">(</a> <a id="774" href="synthetic-homotopy-theory.24-pushouts.html#11169" class="Postulate">inl-pushout</a>
      <a id="792" class="Symbol">(</a> <a id="794" href="foundation-core.constant-maps.html#203" class="Function">const</a> <a id="800" href="foundation.unit-type.html#1075" class="Datatype">unit</a> <a id="805" class="Symbol">(</a><a id="806" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="810" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#666" class="Bound">A</a><a id="811" class="Symbol">)</a> <a id="813" class="Symbol">(</a><a id="814" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="818" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#666" class="Bound">A</a><a id="819" class="Symbol">))</a>
      <a id="828" class="Symbol">(</a> <a id="830" href="foundation-core.constant-maps.html#203" class="Function">const</a> <a id="836" href="foundation.unit-type.html#1075" class="Datatype">unit</a> <a id="841" class="Symbol">(</a><a id="842" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="846" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#670" class="Bound">B</a><a id="847" class="Symbol">)</a> <a id="849" class="Symbol">(</a><a id="850" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="854" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#670" class="Bound">B</a><a id="855" class="Symbol">))</a>
      <a id="864" class="Symbol">(</a> <a id="866" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="870" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#666" class="Bound">A</a><a id="871" class="Symbol">))</a>

<a id="indexed-wedge"></a><a id="875" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#875" class="Function">indexed-wedge</a> <a id="889" class="Symbol">:</a>
  <a id="893" class="Symbol">{</a><a id="894" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#894" class="Bound">l1</a> <a id="897" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#897" class="Bound">l2</a> <a id="900" class="Symbol">:</a> <a id="902" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="907" class="Symbol">}</a> <a id="909" class="Symbol">(</a><a id="910" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#910" class="Bound">I</a> <a id="912" class="Symbol">:</a> <a id="914" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="917" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#894" class="Bound">l1</a><a id="919" class="Symbol">)</a> <a id="921" class="Symbol">(</a><a id="922" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#922" class="Bound">A</a> <a id="924" class="Symbol">:</a> <a id="926" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#910" class="Bound">I</a> <a id="928" class="Symbol">→</a> <a id="930" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="943" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#897" class="Bound">l2</a><a id="945" class="Symbol">)</a> <a id="947" class="Symbol">→</a> <a id="949" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="962" class="Symbol">(</a><a id="963" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#894" class="Bound">l1</a> <a id="966" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="968" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#897" class="Bound">l2</a><a id="970" class="Symbol">)</a>
<a id="972" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#875" class="Function">indexed-wedge</a> <a id="986" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#986" class="Bound">I</a> <a id="988" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#988" class="Bound">A</a> <a id="990" class="Symbol">=</a>
  <a id="994" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
    <a id="1003" class="Symbol">(</a> <a id="1005" href="synthetic-homotopy-theory.cofibers.html#563" class="Function">cofiber</a> <a id="1013" class="Symbol">(λ</a> <a id="1016" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1016" class="Bound">i</a> <a id="1018" class="Symbol">→</a> <a id="1020" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1025" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1016" class="Bound">i</a> <a id="1027" class="Symbol">(</a><a id="1028" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1032" class="Symbol">(</a><a id="1033" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#988" class="Bound">A</a> <a id="1035" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1016" class="Bound">i</a><a id="1036" class="Symbol">))))</a>
    <a id="1045" class="Symbol">(</a> <a id="1047" href="synthetic-homotopy-theory.cofibers.html#1137" class="Function">pt-cofiber</a> <a id="1058" class="Symbol">(λ</a> <a id="1061" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1061" class="Bound">i</a> <a id="1063" class="Symbol">→</a> <a id="1065" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1070" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1061" class="Bound">i</a> <a id="1072" class="Symbol">(</a><a id="1073" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1077" class="Symbol">(</a><a id="1078" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#988" class="Bound">A</a> <a id="1080" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1061" class="Bound">i</a><a id="1081" class="Symbol">))))</a>

<a id="wedge-inclusion"></a><a id="1087" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1087" class="Function">wedge-inclusion</a> <a id="1103" class="Symbol">:</a>
  <a id="1107" class="Symbol">{</a><a id="1108" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1108" class="Bound">l1</a> <a id="1111" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1111" class="Bound">l2</a> <a id="1114" class="Symbol">:</a> <a id="1116" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1121" class="Symbol">}</a> <a id="1123" class="Symbol">(</a><a id="1124" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1124" class="Bound">A</a> <a id="1126" class="Symbol">:</a> <a id="1128" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="1141" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1108" class="Bound">l1</a><a id="1143" class="Symbol">)</a> <a id="1145" class="Symbol">(</a><a id="1146" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1146" class="Bound">B</a> <a id="1148" class="Symbol">:</a> <a id="1150" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="1163" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1111" class="Bound">l2</a><a id="1165" class="Symbol">)</a> <a id="1167" class="Symbol">→</a>
  <a id="1171" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1175" class="Symbol">(</a><a id="1176" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1124" class="Bound">A</a> <a id="1178" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#573" class="Function Operator">∨</a> <a id="1180" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1146" class="Bound">B</a><a id="1181" class="Symbol">)</a> <a id="1183" class="Symbol">→</a> <a id="1185" class="Symbol">(</a><a id="1186" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1190" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1124" class="Bound">A</a><a id="1191" class="Symbol">)</a> <a id="1193" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1195" class="Symbol">(</a><a id="1196" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1200" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1146" class="Bound">B</a><a id="1201" class="Symbol">)</a>
<a id="1203" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1087" class="Function">wedge-inclusion</a> <a id="1219" class="Symbol">{</a><a id="1220" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1220" class="Bound">l1</a><a id="1222" class="Symbol">}</a> <a id="1224" class="Symbol">{</a><a id="1225" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1225" class="Bound">l2</a><a id="1227" class="Symbol">}</a> <a id="1229" class="Symbol">(</a><a id="1230" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1235" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1235" class="Bound">A</a> <a id="1237" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1237" class="Bound">a</a><a id="1238" class="Symbol">)</a> <a id="1240" class="Symbol">(</a><a id="1241" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1246" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1246" class="Bound">B</a> <a id="1248" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1248" class="Bound">b</a><a id="1249" class="Symbol">)</a> <a id="1251" class="Symbol">=</a>
  <a id="1255" href="foundation-core.equivalences.html#4173" class="Function">map-inv-is-equiv</a>
    <a id="1276" class="Symbol">(</a> <a id="1278" href="synthetic-homotopy-theory.24-pushouts.html#11842" class="Postulate">up-pushout</a>
      <a id="1295" class="Symbol">(</a> <a id="1297" href="foundation-core.constant-maps.html#203" class="Function">const</a> <a id="1303" href="foundation.unit-type.html#1075" class="Datatype">unit</a> <a id="1308" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1235" class="Bound">A</a> <a id="1310" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1237" class="Bound">a</a><a id="1311" class="Symbol">)</a>
      <a id="1319" class="Symbol">(</a> <a id="1321" href="foundation-core.constant-maps.html#203" class="Function">const</a> <a id="1327" href="foundation.unit-type.html#1075" class="Datatype">unit</a> <a id="1332" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1246" class="Bound">B</a> <a id="1334" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1248" class="Bound">b</a><a id="1335" class="Symbol">)</a>
      <a id="1343" class="Symbol">(</a> <a id="1345" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1235" class="Bound">A</a> <a id="1347" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1349" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1246" class="Bound">B</a><a id="1350" class="Symbol">))</a>
    <a id="1357" class="Symbol">(</a> <a id="1359" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="1370" class="Symbol">(</a> <a id="1372" class="Symbol">λ</a> <a id="1374" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1374" class="Bound">x</a> <a id="1376" class="Symbol">→</a> <a id="1378" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1383" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1374" class="Bound">x</a> <a id="1385" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1248" class="Bound">b</a><a id="1386" class="Symbol">)</a>
      <a id="1394" class="Symbol">(</a> <a id="1396" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
        <a id="1409" class="Symbol">(</a> <a id="1411" class="Symbol">λ</a> <a id="1413" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1413" class="Bound">y</a> <a id="1415" class="Symbol">→</a> <a id="1417" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1422" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1237" class="Bound">a</a> <a id="1424" href="synthetic-homotopy-theory.wedges-of-pointed-types.html#1413" class="Bound">y</a><a id="1425" class="Symbol">)</a>
        <a id="1435" class="Symbol">(</a> <a id="1437" href="foundation-core.homotopies.html#710" class="Function">refl-htpy</a><a id="1446" class="Symbol">)))</a>
</pre>